# Comparing `tmp/edx-enterprise-3.9.7.tar.gz` & `tmp/edx-enterprise-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/edx-enterprise-3.9.7.tar", last modified: Tue Oct 27 05:31:41 2020, max compression
+gzip compressed data, was "dist/edx-enterprise-3.9.9.tar", last modified: Tue Oct 27 15:04:33 2020, max compression
```

## Comparing `edx-enterprise-3.9.7.tar` & `edx-enterprise-3.9.9.tar`

### file list

```diff
@@ -1,529 +1,529 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)    83898 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   115792 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/consent/
--rw-rw-r--   0 travis    (2000) travis    (2000)      247 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/consent/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5431 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/migrations/0004_datasharingconsenttextoverrides.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3713 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2683 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      427 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/migrations/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/consent/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/api/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      824 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/api/permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/api/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/consent/api/v1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/api/v1/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/api/v1/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11366 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/api/v1/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15773 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      407 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3965 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/mixins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      679 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2956 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      682 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/consent/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3485 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/consent/admin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)   115792 2020-10-27 05:31:40.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-27 05:31:40.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-10-27 05:31:40.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-27 05:31:40.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)    23947 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2020-10-27 05:31:40.000000 edx-enterprise-3.9.7/edx_enterprise.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templatetags/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3667 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templatetags/enterprise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templatetags/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17586 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/signals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/validators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7757 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/decorators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1262 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/enterprise_login_page.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     5143 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/manage_learners.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/program_enrollment_landing_page.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/course_modal.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      890 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/enterprise_customer.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/enterprise_selection_page.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/bundles/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16059 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/bundles/main.style.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      328 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/bundles/main-admin.style.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     5894 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/rules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2776 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/templatetags/
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/templatetags/alert_messages.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      313 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/templatetags/expand_button.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5642 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/templatetags/course_modal.html
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/templatetags/fa_icon.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      443 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_customer_select_form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      312 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_policy.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/emails/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1209 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/emails/user_notification.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1060 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/emails/user_notification.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/grant_data_sharing_permissions.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      614 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1573 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_customer_login_page.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_decline_modal.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4334 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/widgets/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/widgets/segment-io-django.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    10275 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1851 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7410 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/manage_learners.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1839 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/base.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1608 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_user_input.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/heartbeat/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3979 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/heartbeat/checks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      288 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/heartbeat/throttles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/heartbeat/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/heartbeat/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/heartbeat/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/heartbeat/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5277 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5640 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0046_remove_unique_constraints.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0060_upgrade_django_simple_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2330 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0097_auto_20200619_1130.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3116 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      867 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0069_auto_20190613_0607.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2936 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0024_enterprisecustomercatalog_historicalenterprisecustomercatalog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      679 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0089_auto_20200305_0652.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1281 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0051_add_enterprise_slug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      877 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      814 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0095_auto_20200507_1138.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0058_auto_20181212_0145.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      728 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0007_auto_20161109_1511.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0107_remove_branding_config_banner_fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0101_move_data_to_saved_for_later.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      861 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0059_add_code_management_portal_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1819 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0025_auto_20170828_1412.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      758 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0012_auto_20170125_1033.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      813 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0112_auto_20200914_0926.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0048_enterprisecustomeruser_active.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3009 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1307 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0020_auto_20170624_2316.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0063_systemwideenterpriserole_description.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1431 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0044_reporting_config_multiple_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0010_auto_20161222_1212.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      855 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0102_auto_20200708_1615.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0056_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      687 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0040_auto_20180129_1428.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      317 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0054_merge_20180914_1511.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1685 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0008_auto_20161124_2355.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0028_link_enterprise_to_enrollment_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      511 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0029_auto_20170925_1909.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0099_auto_20200702_1537.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3647 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57493 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1384 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0027_remove_account_level_consent.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1406 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0081_UpdateEnterpriseEnrollmentSource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10636 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0016_auto_20170405_0647.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      998 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0034_auto_20171023_0727.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      969 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0031_auto_20171012_1249.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0073_enterprisecustomerreportingconfiguration_uuid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0037_auto_20180110_0450.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0030_auto_20171005_1600.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      590 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0057_enterprisecustomerreportingconfiguration_enterprise_customer_catalogs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0092_auto_20200312_1650.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1155 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0082_AddManagementEnterpriseEnrollmentSource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      649 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0050_progress_v2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      951 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0113_auto_20200914_2054.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0061_systemwideenterpriserole_systemwideenterpriseuserroleassignment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0017_auto_20170508_1341.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      644 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0053_auto_20180911_0811.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0032_reporting_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2484 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0036_sftp_reporting_support.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      861 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0015_auto_20170130_0003.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      689 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0087_auto_20200206_1151.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0052_create_unique_slugs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1065 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0022_auto_20170720_1543.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2188 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0070_enterprise_catalog_query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0068_remove_role_based_access_control_switch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0005_pendingenterprisecustomeruser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0085_enterprisecustomeruser_linked.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3119 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3298 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0079_AddEnterpriseEnrollmentSource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      958 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0021_auto_20170711_0712.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2349 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0088_auto_20200224_1341.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      903 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0039_auto_20180129_1034.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0071_historicalpendingenrollment_historicalpendingenterprisecustomeruser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      809 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0035_auto_20171212_1129.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      479 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0084_auto_20200120_1137.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0080_auto_20191113_1708.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1461 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0076_auto_20190918_2037.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1405 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2318 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0043_auto_20180507_0138.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      922 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0067_add_role_based_access_control_switch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      832 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0055_auto_20181015_1112.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0033_add_history_change_reason_field.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1044 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0062_add_system_wide_enterprise_roles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0038_auto_20180122_1427.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0083_enterprisecustomerreportingconfiguration_include_date.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0042_replace_sensitive_sso_username.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      951 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0026_make_require_account_level_consent_nullable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1218 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0096_enterprise_catalog_admin_role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      881 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0077_auto_20191002_1529.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0006_auto_20161121_0241.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0065_add_enterprise_feature_roles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0019_auto_20170606_1853.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0014_enrollmentnotificationemailtemplate_historicalenrollmentnotificationemailtemplate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      862 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0047_auto_20180517_0457.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0053_pendingenrollment_cohort_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      624 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0049_auto_20180531_0321.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0072_add_enterprise_report_config_feature_role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2114 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0090_update_content_filter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0023_audit_data_reporting_flag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0074_auto_20190904_1143.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      811 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0098_auto_20200629_1756.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1374 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0106_move_branding_config_colors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0064_enterprisefeaturerole_enterprisefeatureuserroleassignment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0078_auto_20191107_1536.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0018_auto_20170511_1357.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      995 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0114_auto_20201020_0142.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0103_remove_marked_done.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      618 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0045_report_type_json.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1163 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0110_add_default_contract_discount.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      639 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0104_sync_query_field.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0003_auto_20161104_0937.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1412 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0086_auto_20200128_1726.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      934 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0066_add_system_wide_enterprise_operator_role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0004_auto_20161114_0434.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0011_enterprisecustomerentitlement_historicalenterprisecustomerentitlement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0002_enterprisecustomerbrandingconfiguration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0013_auto_20170125_1157.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0075_auto_20190916_1030.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0091_add_sales_force_id_in_pendingenrollment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0105_add_branding_config_color_fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      549 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0041_auto_20180212_1507.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/migrations/0009_auto_20161130_1651.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2552 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1350 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/pagination.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/throttles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3384 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/api/v1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1707 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      822 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35766 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/serializers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4371 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/mixins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40370 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api/v1/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44894 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95933 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3160 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/middleware.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   107284 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/management/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12459 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/seed_enterprise_devstack_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4358 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/migrate_enterprise_catalogs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7791 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/create_enterprise_course_enrollments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1393 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/save_enterprise_customer_users.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8034 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/assign_enterprise_user_roles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2089 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/create_missing_dsc_records.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/management/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5825 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/tpa_pipeline.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/settings/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8736 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/settings/test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/settings/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1318 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/views_error_codes.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/widgets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9587 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      838 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/paginator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3653 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29811 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39968 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22724 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/admin/forms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3383 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/forms.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise/api_client/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4123 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api_client/enterprise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10316 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api_client/enterprise_catalog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16482 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api_client/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api_client/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api_client/ecommerce.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19909 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise/api_client/lms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7447 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      910 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/dev.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/doc.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/travis.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/js_test.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    19658 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/edx-platform-constraints.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/travis.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      809 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/base.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     7635 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/doc.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7603 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/test-master.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/constraints.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      704 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/test.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/js_test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/django.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    15018 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/requirements/test-master.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/degreed/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/degreed/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1259 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/degreed/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3549 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      828 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7351 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      960 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1137 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9166 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      225 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9290 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/degreed/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/degreed/admin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2636 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5928 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      531 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      942 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6879 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      824 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1366 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1120 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8135 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      237 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4239 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3561 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/cornerstone/admin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5084 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11029 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20821 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6712 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0002_delete_enterpriseintegratedchannel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0004_catalogtransmissionaudit_channel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0007_auto_20190925_0730.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0006_delete_catalogtransmissionaudit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2800 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1440 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0005_auto_20180306_1251.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0003_catalogtransmissionaudit_learnerdatatransmissionaudit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9926 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6359 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      372 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      303 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1089 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4665 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2653 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2230 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/integrated_channel/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1846 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4600 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7420 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0012_auto_20180109_0712.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1660 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0003_auto_20170317_1402.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7772 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0010_move_audit_tables_to_base_integrated_channel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      916 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactors_use_enterprise_enrollment_page_waffle_flag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      676 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0015_auto_20180510_1259.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      622 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0014_drop_historical_table.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0005_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0017_sapsuccessfactorsglobalconfiguration_search_student_api_path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5802 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0016_sapsuccessfactorsenterprisecustomerconfiguration_additional_locales.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0002_auto_20170224_1545.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      877 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0019_auto_20190925_0730.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactors_remove_enterprise_enrollment_page_waffle_flag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      434 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0007_remove_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0020_sapsuccessfactorsenterprisecustomerconfiguration_catalogs_to_transmit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      562 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0021_sapsuccessfactorsenterprisecustomerconfiguration_show_total_hours.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      860 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0013_auto_20180306_1251.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0018_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      992 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0022_auto_20200206_1046.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      446 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0004_catalogtransmissionaudit_audit_summary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4495 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0011_auto_20180104_0103.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0008_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9854 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      234 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13476 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3222 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/sap_success_factors/admin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/canvas/
--rw-rw-r--   0 travis    (2000) travis    (2000)      312 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/canvas/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/canvas/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2605 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6806 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      816 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1020 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      314 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6421 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4184 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20416 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/canvas/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/canvas/admin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/moodle/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/moodle/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7255 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/moodle/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2873 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4484 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/moodle/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6261 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1487 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6769 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13982 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/moodle/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/moodle/admin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/xapi/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/xapi/statements/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2273 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/statements/learner_course_completion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2807 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/statements/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/statements/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1504 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/statements/learner_course_enrollment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/xapi/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1874 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      451 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5085 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3529 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      303 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      193 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/xapi/management/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/xapi/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13660 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/management/commands/send_course_completions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12186 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/management/commands/send_course_enrollments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/management/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1524 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/xapi/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/xapi/admin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/
--rw-rw-r--   0 travis    (2000) travis    (2000)      332 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/transmitters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1304 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/transmitters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/transmitters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/transmitters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2921 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/exporters/learner_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2519 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/exporters/content_metadata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6057 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1982 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0002_auto_20200930_1723.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      881 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0004_blackboard_tx_chunk_size_default_1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1583 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0003_blackboardlearnerdatatransmissionaudit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6882 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      234 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5437 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25739 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/admin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1116 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/blackboard/admin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10668 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/integrated_channels/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise_learner_portal/
--rw-rw-r--   0 travis    (2000) travis    (2000)      216 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise_learner_portal/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/migrations/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)      232 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 05:31:41.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3091 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/serializers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4204 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/enterprise_learner_portal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2813 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/README.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4242 2020-10-27 05:27:17.000000 edx-enterprise-3.9.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84110 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/CHANGELOG.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116100 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/consent/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      247 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/consent/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5431 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/migrations/0004_datasharingconsenttextoverrides.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3713 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2683 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      427 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/migrations/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/consent/api/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/api/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      824 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/api/permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/api/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/consent/api/v1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/api/v1/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/api/v1/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11366 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/api/v1/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15773 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      407 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3965 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/mixins.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      679 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2956 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      682 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/consent/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3485 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/consent/admin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116100 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23947 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/edx_enterprise.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templatetags/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3667 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templatetags/enterprise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templatetags/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17586 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/signals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/validators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7757 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/decorators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1262 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/enterprise_login_page.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5143 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/manage_learners.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/program_enrollment_landing_page.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/course_modal.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      890 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/enterprise_customer.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/enterprise_selection_page.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/bundles/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16059 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/bundles/main.style.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      328 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/bundles/main-admin.style.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5894 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/rules.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2776 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/templatetags/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/templatetags/alert_messages.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      313 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/templatetags/expand_button.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5642 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/templatetags/course_modal.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)       77 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/templatetags/fa_icon.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      443 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_customer_select_form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      312 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_policy.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/emails/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1209 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/emails/user_notification.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1060 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/emails/user_notification.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/grant_data_sharing_permissions.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      614 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1573 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_customer_login_page.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_decline_modal.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4334 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/widgets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/widgets/segment-io-django.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10275 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1851 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7410 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/manage_learners.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1839 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/base.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1608 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_user_input.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/heartbeat/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3979 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/heartbeat/checks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      288 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/heartbeat/throttles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/heartbeat/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/heartbeat/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/heartbeat/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/heartbeat/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4734 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5640 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      402 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0046_remove_unique_constraints.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0060_upgrade_django_simple_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2330 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0097_auto_20200619_1130.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3116 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      867 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0069_auto_20190613_0607.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2936 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0024_enterprisecustomercatalog_historicalenterprisecustomercatalog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      679 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0089_auto_20200305_0652.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1281 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0051_add_enterprise_slug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      877 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      814 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0095_auto_20200507_1138.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0058_auto_20181212_0145.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      728 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0007_auto_20161109_1511.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0107_remove_branding_config_banner_fields.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      608 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0101_move_data_to_saved_for_later.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      861 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0059_add_code_management_portal_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1819 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0025_auto_20170828_1412.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      758 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0012_auto_20170125_1033.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      813 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0112_auto_20200914_0926.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0048_enterprisecustomeruser_active.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3009 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1307 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0020_auto_20170624_2316.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0063_systemwideenterpriserole_description.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1431 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0044_reporting_config_multiple_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0010_auto_20161222_1212.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      855 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0102_auto_20200708_1615.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      575 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0056_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      687 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0040_auto_20180129_1428.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      317 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0054_merge_20180914_1511.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1685 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0008_auto_20161124_2355.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0028_link_enterprise_to_enrollment_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      511 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0029_auto_20170925_1909.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0099_auto_20200702_1537.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3647 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57493 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1384 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0027_remove_account_level_consent.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1406 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0081_UpdateEnterpriseEnrollmentSource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10636 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0016_auto_20170405_0647.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      998 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0034_auto_20171023_0727.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      969 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0031_auto_20171012_1249.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0073_enterprisecustomerreportingconfiguration_uuid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      863 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0037_auto_20180110_0450.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      483 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0030_auto_20171005_1600.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      590 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0057_enterprisecustomerreportingconfiguration_enterprise_customer_catalogs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0092_auto_20200312_1650.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1155 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0082_AddManagementEnterpriseEnrollmentSource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      649 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0050_progress_v2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      951 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0113_auto_20200914_2054.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0061_systemwideenterpriserole_systemwideenterpriseuserroleassignment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0017_auto_20170508_1341.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      644 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0053_auto_20180911_0811.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      844 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0032_reporting_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2484 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0036_sftp_reporting_support.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      861 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0015_auto_20170130_0003.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      689 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0087_auto_20200206_1151.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0052_create_unique_slugs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1065 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0022_auto_20170720_1543.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2188 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0070_enterprise_catalog_query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      883 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0068_remove_role_based_access_control_switch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0005_pendingenterprisecustomeruser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0085_enterprisecustomeruser_linked.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3119 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3298 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0079_AddEnterpriseEnrollmentSource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      958 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0021_auto_20170711_0712.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2349 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0088_auto_20200224_1341.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      903 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0039_auto_20180129_1034.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0071_historicalpendingenrollment_historicalpendingenterprisecustomeruser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      809 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0035_auto_20171212_1129.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      479 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0084_auto_20200120_1137.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      520 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0080_auto_20191113_1708.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1461 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0076_auto_20190918_2037.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1405 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2318 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0043_auto_20180507_0138.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      922 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0067_add_role_based_access_control_switch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      832 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0055_auto_20181015_1112.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0033_add_history_change_reason_field.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1044 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0062_add_system_wide_enterprise_roles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0038_auto_20180122_1427.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0083_enterprisecustomerreportingconfiguration_include_date.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0042_replace_sensitive_sso_username.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      951 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0026_make_require_account_level_consent_nullable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1218 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0096_enterprise_catalog_admin_role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      881 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0077_auto_20191002_1529.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      468 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0006_auto_20161121_0241.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0065_add_enterprise_feature_roles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0019_auto_20170606_1853.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0014_enrollmentnotificationemailtemplate_historicalenrollmentnotificationemailtemplate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      862 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0047_auto_20180517_0457.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0053_pendingenrollment_cohort_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      624 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0049_auto_20180531_0321.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0072_add_enterprise_report_config_feature_role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2114 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0090_update_content_filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0023_audit_data_reporting_flag.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      844 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0074_auto_20190904_1143.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      811 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0098_auto_20200629_1756.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1374 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0106_move_branding_config_colors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0064_enterprisefeaturerole_enterprisefeatureuserroleassignment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      508 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0078_auto_20191107_1536.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0018_auto_20170511_1357.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      995 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0114_auto_20201020_0142.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0103_remove_marked_done.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      618 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0045_report_type_json.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1163 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0110_add_default_contract_discount.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      639 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0104_sync_query_field.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0003_auto_20161104_0937.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1412 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0086_auto_20200128_1726.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      934 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0066_add_system_wide_enterprise_operator_role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      664 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0004_auto_20161114_0434.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0011_enterprisecustomerentitlement_historicalenterprisecustomerentitlement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0002_enterprisecustomerbrandingconfiguration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0013_auto_20170125_1157.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0075_auto_20190916_1030.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      664 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0091_add_sales_force_id_in_pendingenrollment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0105_add_branding_config_color_fields.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      549 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0041_auto_20180212_1507.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/migrations/0009_auto_20161130_1651.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/api/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2552 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1350 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/pagination.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      203 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/throttles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3384 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/api/v1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1707 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      822 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35766 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/serializers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4371 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/mixins.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40370 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api/v1/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44894 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95933 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3160 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/middleware.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   109156 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      208 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/management/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12459 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/seed_enterprise_devstack_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4358 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/migrate_enterprise_catalogs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7791 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/create_enterprise_course_enrollments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1393 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/save_enterprise_customer_users.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8034 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/assign_enterprise_user_roles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2089 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/create_missing_dsc_records.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/management/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5825 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/tpa_pipeline.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/settings/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8736 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/settings/test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/settings/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/views_error_codes.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      275 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/widgets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9587 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      838 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/paginator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3653 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29811 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39968 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22724 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/admin/forms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3383 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/forms.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise/api_client/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4123 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api_client/enterprise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10316 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api_client/enterprise_catalog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16482 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api_client/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api_client/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api_client/ecommerce.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19909 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise/api_client/lms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/requirements/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7447 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      910 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/dev.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/doc.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/travis.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/js_test.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19658 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/edx-platform-constraints.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/travis.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      809 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/base.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7635 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/doc.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7603 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/test-master.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/constraints.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      704 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/test.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/js_test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      302 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/django.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15018 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/requirements/test-master.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/degreed/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/degreed/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1259 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/degreed/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3549 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      828 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7351 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      960 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1137 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9166 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      225 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9290 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/degreed/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/degreed/admin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2636 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5928 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      531 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      942 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6879 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      824 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1366 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1120 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8135 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      237 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4239 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3561 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/cornerstone/admin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5084 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11029 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20821 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6712 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      301 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0002_delete_enterpriseintegratedchannel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      477 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0004_catalogtransmissionaudit_channel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0007_auto_20190925_0730.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      309 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0006_delete_catalogtransmissionaudit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2800 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1440 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0005_auto_20180306_1251.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0003_catalogtransmissionaudit_learnerdatatransmissionaudit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9926 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6359 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      372 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      303 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1089 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4665 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2653 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2230 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/integrated_channel/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1846 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4600 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7420 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0012_auto_20180109_0712.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1660 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0003_auto_20170317_1402.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7772 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0010_move_audit_tables_to_base_integrated_channel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      916 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactors_use_enterprise_enrollment_page_waffle_flag.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      676 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0015_auto_20180510_1259.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      622 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0014_drop_historical_table.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0005_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0017_sapsuccessfactorsglobalconfiguration_search_student_api_path.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5802 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0016_sapsuccessfactorsenterprisecustomerconfiguration_additional_locales.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0002_auto_20170224_1545.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      877 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0019_auto_20190925_0730.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactors_remove_enterprise_enrollment_page_waffle_flag.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0007_remove_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0020_sapsuccessfactorsenterprisecustomerconfiguration_catalogs_to_transmit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      562 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0021_sapsuccessfactorsenterprisecustomerconfiguration_show_total_hours.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      860 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0013_auto_20180306_1251.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0018_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      992 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0022_auto_20200206_1046.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      446 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0004_catalogtransmissionaudit_audit_summary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4495 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0011_auto_20180104_0103.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0008_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9854 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      422 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      234 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13476 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3222 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/sap_success_factors/admin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/canvas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      312 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/canvas/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/canvas/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2605 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6806 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      816 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1020 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      314 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6421 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4184 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20416 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/canvas/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/canvas/admin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/moodle/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/moodle/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7255 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/moodle/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2873 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4484 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/moodle/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6261 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1487 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      865 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6769 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13982 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/moodle/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/moodle/admin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/xapi/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/xapi/statements/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2273 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/statements/learner_course_completion.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2807 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/statements/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/statements/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1504 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/statements/learner_course_enrollment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      358 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/xapi/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1874 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      451 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      863 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5085 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3529 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      303 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      193 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/xapi/management/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/xapi/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13660 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/management/commands/send_course_completions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12186 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/management/commands/send_course_enrollments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/management/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/management/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1524 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/xapi/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/xapi/admin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      332 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/transmitters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1304 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/transmitters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/transmitters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/transmitters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2921 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/exporters/learner_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2519 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/exporters/content_metadata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6057 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1982 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0002_auto_20200930_1723.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      881 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0004_blackboard_tx_chunk_size_default_1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1583 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0003_blackboardlearnerdatatransmissionaudit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6882 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      234 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5437 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25739 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/admin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1116 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/blackboard/admin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10668 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/integrated_channels/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise_learner_portal/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      216 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise_learner_portal/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/migrations/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      232 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-27 15:04:33.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3091 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/serializers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4204 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/enterprise_learner_portal/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2813 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/README.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4242 2020-10-27 14:59:54.000000 edx-enterprise-3.9.9/setup.py
```

### Comparing `edx-enterprise-3.9.7/CHANGELOG.rst` & `edx-enterprise-3.9.9/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,26 @@
    the package is published.
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
+-----------
+
+[3.9.9]
+--------
+
+* upgrade version to create new release on pypi.
+
+
+[3.9.8]
+--------
+
+* added error_codes in the logging/error messages for the CourseEnrollmentView for better debugging capability.
 
 [3.9.7]
 --------
 
 * Unset learners language so that default_language from enterprise customer may take effect.
 
 [3.9.6]
```

### Comparing `edx-enterprise-3.9.7/PKG-INFO` & `edx-enterprise-3.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 3.9.7
+Version: 3.9.9
 Summary: Your project description goes here
 Home-page: https://github.com/edx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -96,14 +96,26 @@
            the package is published.
         
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
+        -----------
+        
+        [3.9.9]
+        --------
+        
+        * upgrade version to create new release on pypi.
+        
+        
+        [3.9.8]
+        --------
+        
+        * added error_codes in the logging/error messages for the CourseEnrollmentView for better debugging capability.
         
         [3.9.7]
         --------
         
         * Unset learners language so that default_language from enterprise customer may take effect.
         
         [3.9.6]
```

### Comparing `edx-enterprise-3.9.7/consent/migrations/0004_datasharingconsenttextoverrides.py` & `edx-enterprise-3.9.9/consent/migrations/0004_datasharingconsenttextoverrides.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/migrations/0001_initial.py` & `edx-enterprise-3.9.9/consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/migrations/0002_migrate_to_new_data_sharing_consent.py` & `edx-enterprise-3.9.9/consent/migrations/0002_migrate_to_new_data_sharing_consent.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/api/permissions.py` & `edx-enterprise-3.9.9/consent/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/api/v1/views.py` & `edx-enterprise-3.9.9/consent/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/models.py` & `edx-enterprise-3.9.9/consent/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/mixins.py` & `edx-enterprise-3.9.9/consent/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/__init__.py` & `edx-enterprise-3.9.9/consent/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/helpers.py` & `edx-enterprise-3.9.9/consent/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/errors.py` & `edx-enterprise-3.9.9/consent/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/consent/admin/__init__.py` & `edx-enterprise-3.9.9/consent/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/edx_enterprise.egg-info/PKG-INFO` & `edx-enterprise-3.9.9/edx_enterprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 3.9.7
+Version: 3.9.9
 Summary: Your project description goes here
 Home-page: https://github.com/edx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -96,14 +96,26 @@
            the package is published.
         
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
+        -----------
+        
+        [3.9.9]
+        --------
+        
+        * upgrade version to create new release on pypi.
+        
+        
+        [3.9.8]
+        --------
+        
+        * added error_codes in the logging/error messages for the CourseEnrollmentView for better debugging capability.
         
         [3.9.7]
         --------
         
         * Unset learners language so that default_language from enterprise customer may take effect.
         
         [3.9.6]
```

### Comparing `edx-enterprise-3.9.7/edx_enterprise.egg-info/SOURCES.txt` & `edx-enterprise-3.9.9/edx_enterprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/edx_enterprise.egg-info/requires.txt` & `edx-enterprise-3.9.9/edx_enterprise.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templatetags/enterprise.py` & `edx-enterprise-3.9.9/enterprise/templatetags/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/signals.py` & `edx-enterprise-3.9.9/enterprise/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/validators.py` & `edx-enterprise-3.9.9/enterprise/validators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/decorators.py` & `edx-enterprise-3.9.9/enterprise/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/enterprise_login_page.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/enterprise_login_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/manage_learners.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/manage_learners.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/program_enrollment_landing_page.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/program_enrollment_landing_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/course_modal.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/course_modal.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/enterprise_customer.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/enterprise_customer.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/enterprise_selection_page.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/enterprise_selection_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/js/grant_data_sharing_permissions.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/js/grant_data_sharing_permissions.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/bundles/main.style.css` & `edx-enterprise-3.9.9/enterprise/static/enterprise/bundles/main.style.css`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/static/enterprise/admin/enterprise_customer_catalog.js` & `edx-enterprise-3.9.9/enterprise/static/enterprise/admin/enterprise_customer_catalog.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/rules.py` & `edx-enterprise-3.9.9/enterprise/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/urls.py` & `edx-enterprise-3.9.9/enterprise/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/templatetags/course_modal.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/templatetags/course_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_customer_select_form.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_customer_select_form.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/emails/user_notification.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/emails/user_notification.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/emails/user_notification.txt` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/emails/user_notification.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/grant_data_sharing_permissions.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/grant_data_sharing_permissions.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_top_paragraph.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_top_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_customer_login_page.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_customer_login_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_decline_modal.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_decline_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_course_enrollment_page.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_course_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/widgets/segment-io-django.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/widgets/segment-io-django.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/enterprise_program_enrollment_page.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/enterprise_program_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/manage_learners.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/manage_learners.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/admin/transmit_courses_metadata.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/admin/transmit_courses_metadata.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/base.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/base.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/templates/enterprise/_data_sharing_user_input.html` & `edx-enterprise-3.9.9/enterprise/templates/enterprise/_data_sharing_user_input.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/heartbeat/checks.py` & `edx-enterprise-3.9.9/enterprise/heartbeat/checks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/heartbeat/exceptions.py` & `edx-enterprise-3.9.9/enterprise/heartbeat/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/heartbeat/utils.py` & `edx-enterprise-3.9.9/enterprise/heartbeat/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/heartbeat/views.py` & `edx-enterprise-3.9.9/enterprise/heartbeat/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/messages.py` & `edx-enterprise-3.9.9/enterprise/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,37 +92,14 @@
             strong_end='</strong>',
             span_start='<span>',
             span_end='</span>',
         )
     )
 
 
-def add_generic_info_message_for_error(request):
-    """
-    Add message to request indicating that there was an issue processing request.
-
-    Arguments:
-        request: The current request.
-
-    """
-    messages.info(
-        request,
-        _(
-            '{strong_start}Something happened.{strong_end} '
-            '{span_start}This course link is currently invalid. '
-            'Please reach out to your Administrator for assistance to this course.{span_end}'
-        ).format(
-            span_start='<span>',
-            span_end='</span>',
-            strong_start='<strong>',
-            strong_end='</strong>',
-        )
-    )
-
-
 def add_generic_error_message_with_code(request, error_code):
     """
     Add message to request indicating that there was an issue processing request.
 
     Arguments:
         request: The current request.
         error_code: A string error code to be used to point devs to the spot in
@@ -132,15 +109,17 @@
     messages.error(
         request,
         _(
             '{strong_start}Something happened.{strong_end} '
             '{span_start}Please reach out to your learning administrator with '
             'the following error code and they will be able to help you out.{span_end}'
             '{span_start}Error code: {error_code}{span_end}'
+            '{span_start}Username: {username}{span_end}'
         ).format(
             error_code=error_code,
+            username=request.user.username,
             strong_start='<strong>',
             strong_end='</strong>',
             span_start='<span>',
             span_end='</span>',
         )
     )
```

### Comparing `edx-enterprise-3.9.7/enterprise/constants.py` & `edx-enterprise-3.9.9/enterprise/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0060_upgrade_django_simple_history.py` & `edx-enterprise-3.9.9/enterprise/migrations/0060_upgrade_django_simple_history.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0097_auto_20200619_1130.py` & `edx-enterprise-3.9.9/enterprise/migrations/0097_auto_20200619_1130.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py` & `edx-enterprise-3.9.9/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py` & `edx-enterprise-3.9.9/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0069_auto_20190613_0607.py` & `edx-enterprise-3.9.9/enterprise/migrations/0069_auto_20190613_0607.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0024_enterprisecustomercatalog_historicalenterprisecustomercatalog.py` & `edx-enterprise-3.9.9/enterprise/migrations/0024_enterprisecustomercatalog_historicalenterprisecustomercatalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0089_auto_20200305_0652.py` & `edx-enterprise-3.9.9/enterprise/migrations/0089_auto_20200305_0652.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0051_add_enterprise_slug.py` & `edx-enterprise-3.9.9/enterprise/migrations/0051_add_enterprise_slug.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py` & `edx-enterprise-3.9.9/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0095_auto_20200507_1138.py` & `edx-enterprise-3.9.9/enterprise/migrations/0095_auto_20200507_1138.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0058_auto_20181212_0145.py` & `edx-enterprise-3.9.9/enterprise/migrations/0058_auto_20181212_0145.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0007_auto_20161109_1511.py` & `edx-enterprise-3.9.9/enterprise/migrations/0007_auto_20161109_1511.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0107_remove_branding_config_banner_fields.py` & `edx-enterprise-3.9.9/enterprise/migrations/0107_remove_branding_config_banner_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0101_move_data_to_saved_for_later.py` & `edx-enterprise-3.9.9/enterprise/migrations/0101_move_data_to_saved_for_later.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0059_add_code_management_portal_config.py` & `edx-enterprise-3.9.9/enterprise/migrations/0059_add_code_management_portal_config.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0025_auto_20170828_1412.py` & `edx-enterprise-3.9.9/enterprise/migrations/0025_auto_20170828_1412.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0012_auto_20170125_1033.py` & `edx-enterprise-3.9.9/enterprise/migrations/0012_auto_20170125_1033.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0112_auto_20200914_0926.py` & `edx-enterprise-3.9.9/enterprise/migrations/0112_auto_20200914_0926.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py` & `edx-enterprise-3.9.9/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0020_auto_20170624_2316.py` & `edx-enterprise-3.9.9/enterprise/migrations/0020_auto_20170624_2316.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0044_reporting_config_multiple_types.py` & `edx-enterprise-3.9.9/enterprise/migrations/0044_reporting_config_multiple_types.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0010_auto_20161222_1212.py` & `edx-enterprise-3.9.9/enterprise/migrations/0010_auto_20161222_1212.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0102_auto_20200708_1615.py` & `edx-enterprise-3.9.9/enterprise/migrations/0102_auto_20200708_1615.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0056_enterprisecustomerreportingconfiguration_pgp_encryption_key.py` & `edx-enterprise-3.9.9/enterprise/migrations/0056_enterprisecustomerreportingconfiguration_pgp_encryption_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0040_auto_20180129_1428.py` & `edx-enterprise-3.9.9/enterprise/migrations/0040_auto_20180129_1428.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0008_auto_20161124_2355.py` & `edx-enterprise-3.9.9/enterprise/migrations/0008_auto_20161124_2355.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0028_link_enterprise_to_enrollment_template.py` & `edx-enterprise-3.9.9/enterprise/migrations/0028_link_enterprise_to_enrollment_template.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0099_auto_20200702_1537.py` & `edx-enterprise-3.9.9/enterprise/migrations/0099_auto_20200702_1537.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0001_initial.py` & `edx-enterprise-3.9.9/enterprise/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py` & `edx-enterprise-3.9.9/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0027_remove_account_level_consent.py` & `edx-enterprise-3.9.9/enterprise/migrations/0027_remove_account_level_consent.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0081_UpdateEnterpriseEnrollmentSource.py` & `edx-enterprise-3.9.9/enterprise/migrations/0081_UpdateEnterpriseEnrollmentSource.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0016_auto_20170405_0647.py` & `edx-enterprise-3.9.9/enterprise/migrations/0016_auto_20170405_0647.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0034_auto_20171023_0727.py` & `edx-enterprise-3.9.9/enterprise/migrations/0034_auto_20171023_0727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0031_auto_20171012_1249.py` & `edx-enterprise-3.9.9/enterprise/migrations/0031_auto_20171012_1249.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0073_enterprisecustomerreportingconfiguration_uuid.py` & `edx-enterprise-3.9.9/enterprise/migrations/0073_enterprisecustomerreportingconfiguration_uuid.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0037_auto_20180110_0450.py` & `edx-enterprise-3.9.9/enterprise/migrations/0037_auto_20180110_0450.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0057_enterprisecustomerreportingconfiguration_enterprise_customer_catalogs.py` & `edx-enterprise-3.9.9/enterprise/migrations/0057_enterprisecustomerreportingconfiguration_enterprise_customer_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0092_auto_20200312_1650.py` & `edx-enterprise-3.9.9/enterprise/migrations/0092_auto_20200312_1650.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0082_AddManagementEnterpriseEnrollmentSource.py` & `edx-enterprise-3.9.9/enterprise/migrations/0082_AddManagementEnterpriseEnrollmentSource.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0050_progress_v2.py` & `edx-enterprise-3.9.9/enterprise/migrations/0050_progress_v2.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0113_auto_20200914_2054.py` & `edx-enterprise-3.9.9/enterprise/migrations/0113_auto_20200914_2054.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0061_systemwideenterpriserole_systemwideenterpriseuserroleassignment.py` & `edx-enterprise-3.9.9/enterprise/migrations/0061_systemwideenterpriserole_systemwideenterpriseuserroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0017_auto_20170508_1341.py` & `edx-enterprise-3.9.9/enterprise/migrations/0017_auto_20170508_1341.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0053_auto_20180911_0811.py` & `edx-enterprise-3.9.9/enterprise/migrations/0053_auto_20180911_0811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py` & `edx-enterprise-3.9.9/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0032_reporting_model.py` & `edx-enterprise-3.9.9/enterprise/migrations/0032_reporting_model.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0036_sftp_reporting_support.py` & `edx-enterprise-3.9.9/enterprise/migrations/0036_sftp_reporting_support.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0015_auto_20170130_0003.py` & `edx-enterprise-3.9.9/enterprise/migrations/0015_auto_20170130_0003.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0087_auto_20200206_1151.py` & `edx-enterprise-3.9.9/enterprise/migrations/0087_auto_20200206_1151.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0052_create_unique_slugs.py` & `edx-enterprise-3.9.9/enterprise/migrations/0052_create_unique_slugs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0022_auto_20170720_1543.py` & `edx-enterprise-3.9.9/enterprise/migrations/0022_auto_20170720_1543.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0070_enterprise_catalog_query.py` & `edx-enterprise-3.9.9/enterprise/migrations/0070_enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0068_remove_role_based_access_control_switch.py` & `edx-enterprise-3.9.9/enterprise/migrations/0068_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0005_pendingenterprisecustomeruser.py` & `edx-enterprise-3.9.9/enterprise/migrations/0005_pendingenterprisecustomeruser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py` & `edx-enterprise-3.9.9/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0079_AddEnterpriseEnrollmentSource.py` & `edx-enterprise-3.9.9/enterprise/migrations/0079_AddEnterpriseEnrollmentSource.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0021_auto_20170711_0712.py` & `edx-enterprise-3.9.9/enterprise/migrations/0021_auto_20170711_0712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0088_auto_20200224_1341.py` & `edx-enterprise-3.9.9/enterprise/migrations/0088_auto_20200224_1341.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0039_auto_20180129_1034.py` & `edx-enterprise-3.9.9/enterprise/migrations/0039_auto_20180129_1034.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0071_historicalpendingenrollment_historicalpendingenterprisecustomeruser.py` & `edx-enterprise-3.9.9/enterprise/migrations/0071_historicalpendingenrollment_historicalpendingenterprisecustomeruser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0035_auto_20171212_1129.py` & `edx-enterprise-3.9.9/enterprise/migrations/0035_auto_20171212_1129.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0080_auto_20191113_1708.py` & `edx-enterprise-3.9.9/enterprise/migrations/0080_auto_20191113_1708.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0076_auto_20190918_2037.py` & `edx-enterprise-3.9.9/enterprise/migrations/0076_auto_20190918_2037.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py` & `edx-enterprise-3.9.9/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0043_auto_20180507_0138.py` & `edx-enterprise-3.9.9/enterprise/migrations/0043_auto_20180507_0138.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0067_add_role_based_access_control_switch.py` & `edx-enterprise-3.9.9/enterprise/migrations/0067_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0055_auto_20181015_1112.py` & `edx-enterprise-3.9.9/enterprise/migrations/0055_auto_20181015_1112.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0033_add_history_change_reason_field.py` & `edx-enterprise-3.9.9/enterprise/migrations/0033_add_history_change_reason_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0062_add_system_wide_enterprise_roles.py` & `edx-enterprise-3.9.9/enterprise/migrations/0062_add_system_wide_enterprise_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0038_auto_20180122_1427.py` & `edx-enterprise-3.9.9/enterprise/migrations/0038_auto_20180122_1427.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0083_enterprisecustomerreportingconfiguration_include_date.py` & `edx-enterprise-3.9.9/enterprise/migrations/0083_enterprisecustomerreportingconfiguration_include_date.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0042_replace_sensitive_sso_username.py` & `edx-enterprise-3.9.9/enterprise/migrations/0042_replace_sensitive_sso_username.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0026_make_require_account_level_consent_nullable.py` & `edx-enterprise-3.9.9/enterprise/migrations/0026_make_require_account_level_consent_nullable.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0096_enterprise_catalog_admin_role.py` & `edx-enterprise-3.9.9/enterprise/migrations/0096_enterprise_catalog_admin_role.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0077_auto_20191002_1529.py` & `edx-enterprise-3.9.9/enterprise/migrations/0077_auto_20191002_1529.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0065_add_enterprise_feature_roles.py` & `edx-enterprise-3.9.9/enterprise/migrations/0065_add_enterprise_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0019_auto_20170606_1853.py` & `edx-enterprise-3.9.9/enterprise/migrations/0019_auto_20170606_1853.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0014_enrollmentnotificationemailtemplate_historicalenrollmentnotificationemailtemplate.py` & `edx-enterprise-3.9.9/enterprise/migrations/0014_enrollmentnotificationemailtemplate_historicalenrollmentnotificationemailtemplate.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0047_auto_20180517_0457.py` & `edx-enterprise-3.9.9/enterprise/migrations/0047_auto_20180517_0457.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0049_auto_20180531_0321.py` & `edx-enterprise-3.9.9/enterprise/migrations/0049_auto_20180531_0321.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0072_add_enterprise_report_config_feature_role.py` & `edx-enterprise-3.9.9/enterprise/migrations/0072_add_enterprise_report_config_feature_role.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0090_update_content_filter.py` & `edx-enterprise-3.9.9/enterprise/migrations/0090_update_content_filter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0023_audit_data_reporting_flag.py` & `edx-enterprise-3.9.9/enterprise/migrations/0023_audit_data_reporting_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0074_auto_20190904_1143.py` & `edx-enterprise-3.9.9/enterprise/migrations/0074_auto_20190904_1143.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0098_auto_20200629_1756.py` & `edx-enterprise-3.9.9/enterprise/migrations/0098_auto_20200629_1756.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0106_move_branding_config_colors.py` & `edx-enterprise-3.9.9/enterprise/migrations/0106_move_branding_config_colors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0064_enterprisefeaturerole_enterprisefeatureuserroleassignment.py` & `edx-enterprise-3.9.9/enterprise/migrations/0064_enterprisefeaturerole_enterprisefeatureuserroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0018_auto_20170511_1357.py` & `edx-enterprise-3.9.9/enterprise/migrations/0018_auto_20170511_1357.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0114_auto_20201020_0142.py` & `edx-enterprise-3.9.9/enterprise/migrations/0114_auto_20201020_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0045_report_type_json.py` & `edx-enterprise-3.9.9/enterprise/migrations/0045_report_type_json.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0110_add_default_contract_discount.py` & `edx-enterprise-3.9.9/enterprise/migrations/0110_add_default_contract_discount.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0104_sync_query_field.py` & `edx-enterprise-3.9.9/enterprise/migrations/0104_sync_query_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0003_auto_20161104_0937.py` & `edx-enterprise-3.9.9/enterprise/migrations/0003_auto_20161104_0937.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0086_auto_20200128_1726.py` & `edx-enterprise-3.9.9/enterprise/migrations/0086_auto_20200128_1726.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0066_add_system_wide_enterprise_operator_role.py` & `edx-enterprise-3.9.9/enterprise/migrations/0066_add_system_wide_enterprise_operator_role.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0004_auto_20161114_0434.py` & `edx-enterprise-3.9.9/enterprise/migrations/0004_auto_20161114_0434.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0011_enterprisecustomerentitlement_historicalenterprisecustomerentitlement.py` & `edx-enterprise-3.9.9/enterprise/migrations/0011_enterprisecustomerentitlement_historicalenterprisecustomerentitlement.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0002_enterprisecustomerbrandingconfiguration.py` & `edx-enterprise-3.9.9/enterprise/migrations/0002_enterprisecustomerbrandingconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0013_auto_20170125_1157.py` & `edx-enterprise-3.9.9/enterprise/migrations/0013_auto_20170125_1157.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0075_auto_20190916_1030.py` & `edx-enterprise-3.9.9/enterprise/migrations/0075_auto_20190916_1030.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0091_add_sales_force_id_in_pendingenrollment.py` & `edx-enterprise-3.9.9/enterprise/migrations/0091_add_sales_force_id_in_pendingenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0105_add_branding_config_color_fields.py` & `edx-enterprise-3.9.9/enterprise/migrations/0105_add_branding_config_color_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0041_auto_20180212_1507.py` & `edx-enterprise-3.9.9/enterprise/migrations/0041_auto_20180212_1507.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/migrations/0009_auto_20161130_1651.py` & `edx-enterprise-3.9.9/enterprise/migrations/0009_auto_20161130_1651.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/filters.py` & `edx-enterprise-3.9.9/enterprise/api/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/pagination.py` & `edx-enterprise-3.9.9/enterprise/api/pagination.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/throttles.py` & `edx-enterprise-3.9.9/enterprise/api/throttles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/utils.py` & `edx-enterprise-3.9.9/enterprise/api/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/v1/decorators.py` & `edx-enterprise-3.9.9/enterprise/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/v1/urls.py` & `edx-enterprise-3.9.9/enterprise/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/v1/permissions.py` & `edx-enterprise-3.9.9/enterprise/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/v1/serializers.py` & `edx-enterprise-3.9.9/enterprise/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/v1/mixins.py` & `edx-enterprise-3.9.9/enterprise/api/v1/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api/v1/views.py` & `edx-enterprise-3.9.9/enterprise/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/utils.py` & `edx-enterprise-3.9.9/enterprise/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/models.py` & `edx-enterprise-3.9.9/enterprise/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/middleware.py` & `edx-enterprise-3.9.9/enterprise/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/tasks.py` & `edx-enterprise-3.9.9/enterprise/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/apps.py` & `edx-enterprise-3.9.9/enterprise/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/views.py` & `edx-enterprise-3.9.9/enterprise/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1293,32 +1293,48 @@
 
         The provided EnterpriseCustomerCatalog is used to filter and order the
         course modes returned using the EnterpriseCustomerCatalog's
         field "enabled_course_modes".
         """
         modes = EnrollmentApiClient().get_course_modes(course_run_id)
         if not modes:
-            LOGGER.warning('[Enterprise Enrollment] Unable to get course modes. '
-                           'CourseRun: {course_run_id}'.format(course_run_id=course_run_id))
-            messages.add_generic_info_message_for_error(request)
+            error_code = 'ENTCEV000'
+            LOGGER.warning(
+                '[Enterprise Enrollment] Unable to get course modes. '
+                'ErrorCode: {error_code}, '
+                'CourseRun: {course_run_id}, '
+                'Username: {username}, '
+                'EnterpruseCatalog: {enterprise_catalog}'.format(
+                    error_code=error_code,
+                    course_run_id=course_run_id,
+                    username=request.user.username,
+                    enterprise_catalog=enterprise_catalog,
+                )
+            )
+            messages.add_generic_error_message_with_code(request, error_code)
 
         if enterprise_catalog:
             # filter and order course modes according to the enterprise catalog
             modes = [mode for mode in modes if mode['slug'] in enterprise_catalog.enabled_course_modes]
             modes.sort(key=lambda course_mode: enterprise_catalog.enabled_course_modes.index(course_mode['slug']))
             if not modes:
+                error_code = 'ENTCEV001'
                 LOGGER.info(
                     '[Enterprise Enrollment] Matching course modes were not found in EnterpriseCustomerCatalog. '
+                    'ErrorCode: {error_code}, '
                     'CourseRun: {course_run_id}, '
+                    'Username: {username}, '
                     'EnterpriseCatalog: {enterprise_catalog_uuid}'.format(
+                        error_code=error_code,
                         course_run_id=course_run_id,
+                        username=request.user.username,
                         enterprise_catalog_uuid=enterprise_catalog,
                     )
                 )
-                messages.add_generic_info_message_for_error(request)
+                messages.add_generic_error_message_with_code(request, error_code)
 
         return modes
 
     def get_base_details(self, request, enterprise_uuid, course_run_id):
         """
         Retrieve fundamental details used by both POST and GET versions of this view.
 
@@ -1335,68 +1351,94 @@
         if enterprise_catalog_uuid:
             try:
                 enterprise_catalog_uuid = UUID(enterprise_catalog_uuid)
                 enterprise_catalog = enterprise_customer.enterprise_customer_catalogs.get(
                     uuid=enterprise_catalog_uuid
                 )
             except (ValueError, EnterpriseCustomerCatalog.DoesNotExist):
+                error_code = 'ENTCEV002'
                 LOGGER.warning(
                     '[Enterprise Enrollment] EnterpriseCustomerCatalog does not exist. '
-                    'EnterpriseCatalog: {enterprise_catalog_uuid}'.format(
+                    'ErrorCode: {error_code}, '
+                    'EnterpriseCatalog: {enterprise_catalog_uuid}, '
+                    'EnterpriseCustomer: {enterprise_uuid}, '
+                    'CourseRun: {course_run_id}, '
+                    'Username: {username}.'.format(
+                        error_code=error_code,
                         enterprise_catalog_uuid=enterprise_catalog_uuid,
+                        enterprise_uuid=enterprise_uuid,
+                        course_run_id=course_run_id,
+                        username=request.user.username,
                     )
                 )
-                messages.add_generic_info_message_for_error(request)
+                messages.add_generic_error_message_with_code(request, error_code)
 
         course = None
         course_run = None
         course_modes = []
         if enterprise_catalog:
             course, course_run = enterprise_catalog.get_course_and_course_run(course_run_id)
         else:
             try:
                 course, course_run = get_course_catalog_api_service_client(
                     enterprise_customer.site
                 ).get_course_and_course_run(course_run_id)
             except ImproperlyConfigured:
-                LOGGER.warning('[Enterprise Enrollment] CourseCatalogApiServiceClient is improperly configured. '
-                               'Site: {enterprise_customer_site}'.format(
-                                   enterprise_customer_site=enterprise_customer.site.domain))
-                messages.add_generic_info_message_for_error(request)
+                error_code = 'ENTCEV003'
+                LOGGER.warning(
+                    '[Enterprise Enrollment] CourseCatalogApiServiceClient is improperly configured. '
+                    'ErrorCode: {error_code}, '
+                    'Site: {enterprise_customer_site} '
+                    'EnterpriseCustomer: {enterprise_uuid}, '
+                    'CourseRun: {course_run_id}, '
+                    'Username: {username}.'.format(
+                        enterprise_customer_site=enterprise_customer.site.domain,
+                        error_code=error_code,
+                        enterprise_uuid=enterprise_uuid,
+                        course_run_id=course_run_id,
+                        username=request.user.username,
+                    )
+                )
+                messages.add_generic_error_message_with_code(request, error_code)
                 return enterprise_customer, course, course_run, course_modes
 
         if not course or not course_run:
+            error_code = 'ENTCEV004'
             course_id = course['key'] if course else "Not Found"
             course_title = course['title'] if course else "Not Found"
             course_run_title = course_run['title'] if course_run else "Not Found"
             enterprise_catalog_title = enterprise_catalog.title if enterprise_catalog else "Not Found"
             # The specified course either does not exist in the specified
             # EnterpriseCustomerCatalog, or does not exist at all in the
             # discovery service.
             LOGGER.warning(
                 '[Enterprise Enrollment] Failed to fetch details for course or course run. '
+                'ErrorCode: {error_code}, '
                 'Course: {course_id}, '
                 'CourseRun: {course_run_id}, '
                 'CourseRunTitle: {course_run_title}, '
                 'CourseTitle: {course_title}, '
+                'Username: {username}, '
                 'EnterpriseCatalog: {enterprise_catalog_uuid}, '
                 'EnterpriseCatalogTitle: {enterprise_catalog_title}, '
                 'EnterpriseCustomer: {enterprise_uuid}, '
                 'EnterpriseName: {enterprise_name}'.format(
+                    error_code=error_code,
                     course_title=course_title,
                     course_id=course_id,
                     course_run_title=course_run_title,
                     course_run_id=course_run_id,
+                    username=request.user.username,
                     enterprise_name=enterprise_customer.name,
                     enterprise_uuid=enterprise_customer.uuid,
                     enterprise_catalog_title=enterprise_catalog_title,
                     enterprise_catalog_uuid=enterprise_catalog_uuid,
                 )
             )
-            messages.add_generic_info_message_for_error(request)
+            messages.add_generic_error_message_with_code(request, error_code)
             return enterprise_customer, course, course_run, course_modes
 
         if enterprise_catalog_uuid and not enterprise_catalog:
             # A catalog query parameter was given, but the specified
             # EnterpriseCustomerCatalog does not exist, so just return and
             # display the generic error message.
             return enterprise_customer, course, course_run, course_modes
```

### Comparing `edx-enterprise-3.9.7/enterprise/management/commands/seed_enterprise_devstack_data.py` & `edx-enterprise-3.9.9/enterprise/management/commands/seed_enterprise_devstack_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/management/commands/migrate_enterprise_catalogs.py` & `edx-enterprise-3.9.9/enterprise/management/commands/migrate_enterprise_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/management/commands/create_enterprise_course_enrollments.py` & `edx-enterprise-3.9.9/enterprise/management/commands/create_enterprise_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/management/commands/save_enterprise_customer_users.py` & `edx-enterprise-3.9.9/enterprise/management/commands/save_enterprise_customer_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/management/commands/assign_enterprise_user_roles.py` & `edx-enterprise-3.9.9/enterprise/management/commands/assign_enterprise_user_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/management/commands/create_missing_dsc_records.py` & `edx-enterprise-3.9.9/enterprise/management/commands/create_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/tpa_pipeline.py` & `edx-enterprise-3.9.9/enterprise/tpa_pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/settings/test.py` & `edx-enterprise-3.9.9/enterprise/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/views_error_codes.txt` & `edx-enterprise-3.9.9/enterprise/views_error_codes.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,7 +19,13 @@
 ENTPEV001 - No course details or course run details available
 ENTPEV002 - Course catalog api configuration error
 ENTPEV003 - No program details available
 ENTPEV004 - No program type available
 
 ENTRV000 - No course_run_id available
 ENTRV001 - No course_run_id available, or course catalog configuration error
+
+ENTCEV000 - Unable to get course modes
+ENTCEV001 - Matching course modes were not found in EnterpriseCustomerCatalog
+ENTCEV002 - EnterpriseCustomerCatalog does not exist
+ENTCEV003 - CourseCatalogApiServiceClient is improperly configured
+ENTCEV004 - Failed to fetch details for course or course run
```

### Comparing `edx-enterprise-3.9.7/enterprise/admin/utils.py` & `edx-enterprise-3.9.9/enterprise/admin/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/admin/paginator.py` & `edx-enterprise-3.9.9/enterprise/admin/paginator.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/admin/actions.py` & `edx-enterprise-3.9.9/enterprise/admin/actions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/admin/__init__.py` & `edx-enterprise-3.9.9/enterprise/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/admin/views.py` & `edx-enterprise-3.9.9/enterprise/admin/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/admin/forms.py` & `edx-enterprise-3.9.9/enterprise/admin/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/forms.py` & `edx-enterprise-3.9.9/enterprise/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api_client/enterprise.py` & `edx-enterprise-3.9.9/enterprise/api_client/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api_client/enterprise_catalog.py` & `edx-enterprise-3.9.9/enterprise/api_client/enterprise_catalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api_client/discovery.py` & `edx-enterprise-3.9.9/enterprise/api_client/discovery.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api_client/ecommerce.py` & `edx-enterprise-3.9.9/enterprise/api_client/ecommerce.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise/api_client/lms.py` & `edx-enterprise-3.9.9/enterprise/api_client/lms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/test.txt` & `edx-enterprise-3.9.9/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/dev.in` & `edx-enterprise-3.9.9/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/edx-platform-constraints.txt` & `edx-enterprise-3.9.9/requirements/edx-platform-constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/travis.txt` & `edx-enterprise-3.9.9/requirements/travis.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/base.in` & `edx-enterprise-3.9.9/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/doc.txt` & `edx-enterprise-3.9.9/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/test-master.txt` & `edx-enterprise-3.9.9/requirements/test-master.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/constraints.txt` & `edx-enterprise-3.9.9/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/test.in` & `edx-enterprise-3.9.9/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/js_test.txt` & `edx-enterprise-3.9.9/requirements/js_test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/requirements/dev.txt` & `edx-enterprise-3.9.9/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/models.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/client.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/degreed/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/degreed/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/utils.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/models.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/views.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/client.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/cornerstone/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/cornerstone/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0005_auto_20180306_1251.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0005_auto_20180306_1251.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/migrations/0003_catalogtransmissionaudit_learnerdatatransmissionaudit.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/migrations/0003_catalogtransmissionaudit_learnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/models.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/tasks.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/integrated_channel/client.py` & `edx-enterprise-3.9.9/integrated_channels/integrated_channel/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/constants.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/utils.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0012_auto_20180109_0712.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0012_auto_20180109_0712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0003_auto_20170317_1402.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0003_auto_20170317_1402.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0010_move_audit_tables_to_base_integrated_channel.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0010_move_audit_tables_to_base_integrated_channel.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactors_use_enterprise_enrollment_page_waffle_flag.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactors_use_enterprise_enrollment_page_waffle_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0015_auto_20180510_1259.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0015_auto_20180510_1259.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0014_drop_historical_table.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0014_drop_historical_table.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0005_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0005_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0017_sapsuccessfactorsglobalconfiguration_search_student_api_path.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0017_sapsuccessfactorsglobalconfiguration_search_student_api_path.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0016_sapsuccessfactorsenterprisecustomerconfiguration_additional_locales.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0016_sapsuccessfactorsenterprisecustomerconfiguration_additional_locales.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0002_auto_20170224_1545.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0002_auto_20170224_1545.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0019_auto_20190925_0730.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0019_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactors_remove_enterprise_enrollment_page_waffle_flag.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactors_remove_enterprise_enrollment_page_waffle_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0020_sapsuccessfactorsenterprisecustomerconfiguration_catalogs_to_transmit.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0020_sapsuccessfactorsenterprisecustomerconfiguration_catalogs_to_transmit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0021_sapsuccessfactorsenterprisecustomerconfiguration_show_total_hours.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0021_sapsuccessfactorsenterprisecustomerconfiguration_show_total_hours.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0013_auto_20180306_1251.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0013_auto_20180306_1251.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0018_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0018_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0022_auto_20200206_1046.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0022_auto_20200206_1046.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0011_auto_20180104_0103.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0011_auto_20180104_0103.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/migrations/0008_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/migrations/0008_historicalsapsuccessfactorsenterprisecustomerconfiguration_history_change_reason.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/models.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/client.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/sap_success_factors/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/sap_success_factors/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/models.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/views.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/client.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/canvas/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/canvas/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/models.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/client.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/moodle/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/moodle/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/statements/learner_course_completion.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/statements/learner_course_completion.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/statements/base.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/statements/base.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/statements/learner_course_enrollment.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/statements/learner_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/utils.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/models.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/management/commands/send_course_completions.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/management/commands/send_course_completions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/management/commands/send_course_enrollments.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/management/commands/send_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/client.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/xapi/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/xapi/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/transmitters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/transmitters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/exporters/learner_data.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/exporters/content_metadata.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0001_initial.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0002_auto_20200930_1723.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0002_auto_20200930_1723.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0004_blackboard_tx_chunk_size_default_1.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0004_blackboard_tx_chunk_size_default_1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/migrations/0003_blackboardlearnerdatatransmissionaudit.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/migrations/0003_blackboardlearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/models.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/views.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/client.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/blackboard/admin/__init__.py` & `edx-enterprise-3.9.9/integrated_channels/blackboard/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/integrated_channels/utils.py` & `edx-enterprise-3.9.9/integrated_channels/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/serializers.py` & `edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise_learner_portal/api/v1/views.py` & `edx-enterprise-3.9.9/enterprise_learner_portal/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/enterprise_learner_portal/utils.py` & `edx-enterprise-3.9.9/enterprise_learner_portal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/README.rst` & `edx-enterprise-3.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-3.9.7/setup.py` & `edx-enterprise-3.9.9/setup.py`

 * *Files identical despite different names*

