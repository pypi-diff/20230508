# Comparing `tmp/aa_memberaudit-2.7.0.tar.gz` & `tmp/aa_memberaudit-2.8.0.tar.gz`

## Comparing `aa_memberaudit-2.7.0.tar` & `aa_memberaudit-2.8.0.tar`

### file list

```diff
@@ -1,233 +1,234 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/__init__.py
--rw-r--r--   0        0        0    22972 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/admin.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/app_settings.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/apps.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/auth_hooks.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/checks.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/constants.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/decorators.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/forms.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/helpers.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/providers.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/signals.py
--rw-r--r--   0        0        0   881821 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/swagger.json
--rw-r--r--   0        0        0    40138 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tasks.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/__init__.py
--rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/data_exporters.py
--rw-r--r--   0        0        0    19049 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/eft_parser.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/fittings.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/skill_plans.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/skills.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/xml_converter.py
--rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/django.pot
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40935 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    40291 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40932 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40925 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41080 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41163 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40925 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_data_export.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_load_eve.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_stats.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_update_characters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/__init__.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/character.py
--rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/general.py
--rw-r--r--   0        0        0    48513 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/sections.py
--rw-r--r--   0        0        0    65995 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0003_add_notify_permission.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0004_character_is_disabled.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0005_add_fw_stats.py
--rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0006_add_localizations.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0007_add_localization_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/__init__.py
--rw-r--r--   0        0        0    54096 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/character.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/constants.py
--rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/general.py
--rw-r--r--   0        0        0    40017 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/sections.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/admin.css
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_finder.css
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.css
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/data_export.css
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.css
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.min.css
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.css
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.min.css
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.css
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/reports.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/charisma.png
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/eve-prism.png
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/evelogo.png
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/evesearch.png
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/intelligence.png
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/memory.png
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/perception.png
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/willpower.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/zkillboard.png
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/base.html
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_finder.html
--rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_viewer.html
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/data_export.html
--rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/launcher.html
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/reports.html
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/menu.html
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templatetags/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templatetags/memberaudit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/__init__.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_admin.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_checks.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_commands.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_decorators.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_factories.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_forms.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_helpers.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_integration.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_signals.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_tasks.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_templatetags.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/__init__.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_core_xml_converter.py
--rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_data_exporters.py
--rw-r--r--   0        0        0    20438 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_eft_parser.py
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_fittings.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_skill_plans.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_skills.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/__init__.py
--rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/test_character.py
--rw-r--r--   0        0        0    41576 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/test_general.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/test_sections.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/__init__.py
--rw-r--r--   0        0        0    36061 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_1.py
--rw-r--r--   0        0        0    35834 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_2.py
--rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_3.py
--rw-r--r--   0        0        0    28275 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_4.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_5.py
--rw-r--r--   0        0        0    10448 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_general.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_sections.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/utils.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/__init__.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/entities.json
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0    40192 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_testdata.json
--rw-r--r--   0        0        0  1159197 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/factories.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_character.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_doctrines.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_entities.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_locations.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/profiler_toolbox.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/__init__.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_admin.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_finder.py
--rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_1.py
--rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_2.py
--rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_characters.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_data_export.py
--rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_reports.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tools/drop_tables.sql
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tools/total_size.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/__init__.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/_common.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/admin.py
--rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/character_finder.py
--rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/character_viewer_1.py
--rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/character_viewer_2.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/characters.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/data_export.py
--rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/reports.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/LICENSE
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/README.md
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/__init__.py
+-rw-r--r--   0        0        0    23256 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/admin.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/apps.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/checks.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/constants.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/forms.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/helpers.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/providers.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/signals.py
+-rw-r--r--   0        0        0   881821 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/swagger.json
+-rw-r--r--   0        0        0    40138 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tasks.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19266 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0    40962 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41012 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    41009 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41009 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41081 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41069 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41007 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41019 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26859 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    54511 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41002 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    48513 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/sections.py
+-rw-r--r--   0        0        0    65995 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    54096 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/character.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/general.py
+-rw-r--r--   0        0        0    40017 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/sections.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    22356 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    41576 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/test_sections.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0    36061 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_1.py
+-rw-r--r--   0        0        0    35834 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_2.py
+-rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_3.py
+-rw-r--r--   0        0        0    28275 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_4.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_5.py
+-rw-r--r--   0        0        0    10448 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_sections.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/utils.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    40192 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1159197 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/reports.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/LICENSE
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/README.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/PKG-INFO
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/admin.py` & `aa_memberaudit-2.8.0/memberaudit/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List, Optional
+
 from django import forms
 from django.contrib import admin
 from django.contrib.auth.models import Group
 from django.core.exceptions import ValidationError
 from django.db.models import Max, Prefetch
 from django.forms.models import BaseInlineFormSet
 from django.shortcuts import redirect, render
@@ -53,21 +55,21 @@
         qs = super().get_queryset(request)
         return qs.select_related("group").prefetch_related("group__authgroup__states")
 
     def save_model(self, request, obj, *args, **kwargs) -> None:
         super().save_model(request, obj, *args, **kwargs)
         tasks.add_compliant_users_to_group.apply_async(
             args=[obj.group.pk], priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
-        )
+        )  # type: ignore
 
     def delete_queryset(self, request, queryset) -> None:
         for obj in queryset:
             tasks.clear_users_from_group.apply_async(
                 args=[obj.group.pk], priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
-            )
+            )  # type: ignore
             obj.delete()
 
     @admin.display(ordering="group__name")
     def _group_name(self, obj) -> str:
         return obj.group.name
 
     @admin.display(description=_("Restricted to states"))
@@ -273,45 +275,42 @@
     def _enabled(self, obj: Character) -> bool:
         return not obj.is_disabled
 
     @admin.display(
         ordering="eve_character__character_ownership__user__profile__main_character",
         description=_("main"),
     )
-    def _main(self, obj: Character) -> str:
+    def _main(self, obj: Character) -> Optional[str]:
         try:
             name = obj.main_character.character_name
         except AttributeError:
             return None
         return str(name)
 
     @admin.display(
         ordering="eve_character__character_ownership__user__profile__state__name",
         description=_("state"),
     )
-    def _state(self, obj: Character) -> str:
+    def _state(self, obj: Character) -> Optional[str]:
         try:
             return str(obj.user.profile.state)
         except AttributeError:
             return None
 
     @admin.display(
         ordering="eve_character__character_ownership__user__profile__main_character__corporation_name",
         description=_("organization"),
     )
-    def _organization(self, obj: Character) -> str:
-        try:
-            return "{}{}".format(
-                obj.main_character.corporation_name,
-                f" [{obj.main_character.alliance_ticker}]"
-                if obj.main_character.alliance_ticker
-                else "",
-            )
-        except AttributeError:
+    def _organization(self, obj: Character) -> Optional[str]:
+        if not obj.main_character:
             return None
+        result = obj.main_character.corporation_name
+        if result and obj.main_character.alliance_ticker:
+            result += f" [{obj.main_character.alliance_ticker}]"
+        return result
 
     @admin.display(ordering="update_status", description=_("update status"))
     def _update_status(self, obj: Character):
         css_class_map = {
             Character.UpdateStatus.INCOMPLETE: "text-warning",
             Character.UpdateStatus.ERROR: "text-danger",
             Character.UpdateStatus.DISABLED: "text-muted",
@@ -352,15 +351,15 @@
     @admin.display(description=_("Delete selected characters"))
     def delete_characters(self, request, queryset):
         if "apply" in request.POST:
             for obj in queryset:
                 tasks.delete_character.apply_async(
                     kwargs={"character_pk": obj.pk},
                     priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
-                )
+                )  # type: ignore
             self.message_user(
                 request,
                 _(
                     "Started deleting %d character(s). "
                     "This can take a minute." % queryset.count()
                 ),
             )
@@ -376,28 +375,28 @@
 
     @admin.display(description=_("Update selected characters from EVE server"))
     def update_characters(self, request, queryset):
         for obj in queryset:
             tasks.update_character.apply_async(
                 kwargs={"character_pk": obj.pk, "force_update": True},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
-            )
-            self.message_user(request, _("Started updating character: %s. " % obj))
+            )  # type: ignore
+            self.message_user(request, _("Started updating character %s." % obj))
 
     @admin.display(
         description=_("Update assets for selected characters from EVE server")
     )
     def update_assets(self, request, queryset):
         for obj in queryset:
             tasks.update_character_assets.apply_async(
                 kwargs={"character_pk": obj.pk, "force_update": True},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
-            )
+            )  # type: ignore
             self.message_user(
-                request, _("Started updating assets for character: %s." % obj)
+                request, _("Started updating assets for character %s." % obj)
             )
 
     @admin.display(
         description=(
             _(
                 "Update %s for selected characters from EVE server"
                 % {
@@ -410,19 +409,19 @@
     )
     def update_location(self, request, queryset):
         section = Character.UpdateSection.LOCATION
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
-            )
+            )  # type: ignore
             self.message_user(
                 request,
                 _(
-                    "Started updating %s for character: %s. "
+                    "Started updating %s for character %s."
                     % (Character.UpdateSection.display_name(section), obj)
                 ),
             )
 
     @admin.display(
         description=(
             _(
@@ -435,20 +434,23 @@
     )
     def update_online_status(self, request, queryset):
         section = Character.UpdateSection.ONLINE_STATUS
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
-            )
+            )  # type: ignore
             self.message_user(
                 request,
                 _(
-                    "Started updating %s for character: %s."
-                    % (Character.UpdateSection.display_name(section), obj)
+                    "Started updating %(section)s for character %(character)s."
+                    % {
+                        "section": Character.UpdateSection.display_name(section),
+                        "character": obj,
+                    }
                 ),
             )
 
     @admin.display(description=_("Enable selected characters"))
     def enable_characters(self, request, queryset):
         pks = list(queryset.values_list("pk", flat=True))
         queryset.filter(pk__in=pks).update(is_disabled=False)
@@ -563,15 +565,15 @@
                         row
                         and row.get("DELETE") is False
                         and not row.get("required_level")
                         and not row.get("recommended_level")
                     ):
                         eve_type = row.get("eve_type")
                         raise ValidationError(
-                            _("Skill '%s' must have a level.", eve_type.name)
+                            _("Skill '%s' must have a level." % eve_type.name)
                         )
 
 
 class SkillSetSkillAdminInline(MinValidatedInlineMixIn, admin.TabularInline):
     model = SkillSetSkill
     verbose_name = "skill"
     verbose_name_plural = "skills"
@@ -651,15 +653,15 @@
                 skill.eve_type.name,
                 skill.required_level if skill.required_level else "",
                 f"[{skill.recommended_level}]" if skill.recommended_level else "",
             )
             for skill in obj.skills_ordered
         ]
 
-    def _groups(self, obj) -> list:
+    def _groups(self, obj) -> Optional[List[str]]:
         groups = [f"{group.name}" for group in obj.groups_ordered]
         return groups if groups else None
 
     inlines = (SkillSetSkillAdminInline,)
 
     def formfield_for_foreignkey(self, db_field, request, **kwargs):
         if db_field.name == "ship_type":
@@ -671,15 +673,15 @@
         return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
     def save_model(self, request, obj, form, change):
         obj.user = request.user
         super().save_model(request, obj, form, change)
         tasks.update_characters_skill_checks.apply_async(
             kwargs={"force_update": True}, priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
-        )
+        )  # type: ignore
 
     def delete_model(self, request, obj):
         obj.user = request.user
         super().delete_model(request, obj)
         tasks.update_characters_skill_checks.apply_async(
             kwargs={"force_update": True}, priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
-        )
+        )  # type: ignore
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/app_settings.py` & `aa_memberaudit-2.8.0/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/auth_hooks.py` & `aa_memberaudit-2.8.0/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/checks.py` & `aa_memberaudit-2.8.0/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/constants.py` & `aa_memberaudit-2.8.0/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/decorators.py` & `aa_memberaudit-2.8.0/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/forms.py` & `aa_memberaudit-2.8.0/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/helpers.py` & `aa_memberaudit-2.8.0/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/swagger.json` & `aa_memberaudit-2.8.0/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tasks.py` & `aa_memberaudit-2.8.0/memberaudit/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/urls.py` & `aa_memberaudit-2.8.0/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.8.0/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.8.0/memberaudit/core/eft_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Parser for fitting in EFT Format"""
 from dataclasses import dataclass, field
 from enum import Enum, auto
-from typing import Dict, Iterable, List, Optional, Set, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 from bravado.exception import HTTPNotFound
 
 from eveuniverse.models import EveEntity, EveType
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
@@ -17,14 +17,18 @@
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class EftParserError(Exception):
     """Base error for EFT parser."""
 
 
+class UnknownShipTypeError(EftParserError):
+    """Ship type is unknown."""
+
+
 class MissingTitleError(EftParserError):
     """Title is missing."""
 
 
 class MissingSectionsError(EftParserError):
     """Insufficient sections defined."""
 
@@ -72,15 +76,15 @@
 
     @classmethod
     def _fetch_types_from_db(cls, type_names: Iterable[str]) -> Dict[str, EveType]:
         eve_types_query = (
             EveType.objects.select_related("eve_group")
             .prefetch_related("dogma_effects")
             .filter(
-                enabled_sections=EveType.enabled_sections.dogmas, name__in=type_names
+                enabled_sections=EveType.enabled_sections.dogmas, name__in=type_names  # type: ignore
             )
         )
         eve_types = {obj.name: obj for obj in eve_types_query}
         return eve_types
 
     @classmethod
     def _fetch_missing_types_from_esi(
@@ -115,15 +119,15 @@
             try:
                 obj, _ = EveType.objects.get_or_create_esi(
                     id=entity_id, enabled_sections=[EveType.Section.DOGMAS]
                 )
             except HTTPNotFound:
                 pass
             else:
-                eve_types[obj.name] = obj
+                eve_types[obj.name] = obj  # type: ignore
         return eve_types
 
     # @classmethod
     # def _fetch_types_from_esi(cls, entity_ids) -> Dict[str, EveType]:
     #     """Fetch types from ESI concurrently using threads."""
     #     max_workers = getattr(settings, "ESI_CONNECTION_POOL_MAXSIZE", 10)
     #     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
@@ -139,15 +143,14 @@
     #         )
     #     except HTTPNotFound:
     #         return None
     #     else:
     #         return obj
 
 
-@dataclass
 class _EftSlotType(Enum):
     NONE = auto()
     LOW_SLOT = auto()
     MEDIUM_SLOT = auto()
     HIGH_SLOT = auto()
     RIG_SLOT = auto()
     SUBSYSTEM_SLOT = auto()
@@ -410,15 +413,15 @@
                 objs.append(Module(**params))
         return objs
 
     def to_items(self) -> List[Item]:
         """Convert eft items into fitting items."""
         objs = []
         for item in self.items:
-            params = {"item_type": item.item_type}
+            params: Dict[str, Any] = {"item_type": item.item_type}
             if item.quantity:
                 params["quantity"] = item.quantity
             objs.append(Item(**params))
         return objs
 
     @classmethod
     def create_from_eft_text_section(
@@ -442,14 +445,16 @@
     eve_types, unknown_types = _load_eve_types(ship_type_name, eft_sections)
     sections = [
         _EftSection.create_from_eft_text_section(section, eve_types)
         for section in eft_sections
     ]
     sections = _try_to_identify_sections(sections)
     ship_type = eve_types.from_name(ship_type_name)
+    if not ship_type:
+        raise UnknownShipTypeError(f"Unknown ship type: {ship_type_name}")
     fitting = _create_fitting_from_sections(fitting_name, ship_type, sections)
     errors = _unknown_types_to_errors(unknown_types)
     return fitting, errors
 
 
 def _text_to_lines(eft_text: str) -> List[str]:
     """Convert text into lines."""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/core/fittings.py` & `aa_memberaudit-2.8.0/memberaudit/core/fittings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Eve Online Fittings"""
 from dataclasses import dataclass, field
-from typing import List, Optional, Set, Tuple
+from typing import List, Optional, Set, Tuple, Union
 
 from eveuniverse.models import EveType
 
 from .skills import Skill, compress_skills, required_skills_from_eve_types
 
 
 @dataclass(frozen=True)
@@ -23,33 +23,35 @@
         raise RuntimeError("No instantiation from abstract base class")
 
 
 @dataclass(frozen=True)
 class Module(_BaseFittingItem):
     """A ship module used in a fitting."""
 
-    module_type: EveType = None
-    charge_type: EveType = None
+    module_type: Optional[EveType] = None
+    charge_type: Optional[EveType] = None
     is_offline: bool = False
 
     @property
     def is_empty(self) -> bool:
         return self.module_type is None
 
-    def eve_types(self) -> Set[EveType]:
+    def eve_types(self) -> Union[Set[EveType], set]:
         """Eve types used in this module."""
-        if self.is_empty:
-            return set()
-        types = {self.module_type}
+        types = set()
+        if self.module_type:
+            types.add(self.module_type)
         if self.charge_type:
             types.add(self.charge_type)
         return types
 
     def to_eft(self) -> str:
         """Convert to EFT format."""
+        if not self.module_type:
+            raise ValueError("Module is empty")
         text = self.module_type.name
         if self.charge_type:
             text += f", {self.charge_type.name}"
         if self.is_offline:
             text += " /OFFLINE"
         return text
 
@@ -94,15 +96,15 @@
     boosters: List[Item] = field(default_factory=list)
     cargo_bay: List[Item] = field(default_factory=list)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
     @property
-    def modules(self) -> List[EveType]:
+    def modules(self) -> List[Module]:
         """All fitted modules."""
         return (
             self.high_slots
             + self.medium_slots
             + self.low_slots
             + self.rig_slots
             + self.subsystem_slots
@@ -127,15 +129,15 @@
         """Skills required to fly this fitting."""
 
         eve_types = self.eve_types()
         skills = required_skills_from_eve_types(eve_types)
         return compress_skills(skills)
 
     def to_eft(self) -> str:
-        def add_section(objs, keyword: str = None) -> List[str]:
+        def add_section(objs, keyword: Optional[str] = None) -> List[str]:
             lines = [""]
             for obj in objs:
                 lines.append(
                     obj.to_eft() if not obj.is_empty else f"[Empty {keyword} slot]"
                 )
             return lines
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.8.0/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/core/skills.py` & `aa_memberaudit-2.8.0/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.8.0/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/django.pot` & `aa_memberaudit-2.8.0/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:134 admin.py:312
 msgid "update status"
@@ -72,80 +73,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -360,15 +361,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -721,31 +723,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -839,24 +855,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -866,22 +872,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1567,43 +1578,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1641,20 +1636,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1702,10 +1697,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
-"PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: German (https://app.transifex.com/kalkoken-apps/teams/107978/"
-"de/)\n"
-"Language: de\n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:73
 msgid "Restricted to states"
@@ -73,80 +73,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -361,15 +361,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -722,31 +723,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -840,24 +855,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -867,22 +872,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1568,43 +1578,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1642,20 +1636,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1703,10 +1697,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,453 +4,486 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-16 17:58+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: Korean (Korea) (https://app.transifex.com/kalkoken-apps/"
+"teams/107978/ko_KR/)\n"
+"Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:72
+#: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:133 admin.py:311
+#: admin.py:134 admin.py:312
 msgid "update status"
 msgstr ""
 
-#: admin.py:159 admin.py:288
+#: admin.py:160 admin.py:289
 msgid "state"
 msgstr ""
 
-#: admin.py:185
+#: admin.py:186
 msgid "No main"
 msgstr ""
 
-#: admin.py:267
+#: admin.py:268 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:271
+#: admin.py:272
 msgid "enabled"
 msgstr ""
 
-#: admin.py:277
+#: admin.py:278
 msgid "main"
 msgstr ""
 
-#: admin.py:298
+#: admin.py:299
 msgid "organization"
 msgstr ""
 
-#: admin.py:323
+#: admin.py:324
 msgid "created"
 msgstr ""
 
-#: admin.py:327
+#: admin.py:328
 msgid "last update"
 msgstr ""
 
-#: admin.py:351
+#: admin.py:352
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:371
+#: admin.py:372
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:376
+#: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:383
+#: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:386
+#: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:395
+#: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:401 admin.py:428
+#: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:420
+#: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
-#: admin.py:445
+#: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:450
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:454
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:456
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:460
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:492 models/general.py:259 models/general.py:294
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:496
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:569
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
 
-#: models/character.py:67
+#: models/character.py:69
 msgid "assets"
 msgstr ""
 
-#: models/character.py:69
+#: models/character.py:71
 msgid "contacts"
 msgstr ""
 
-#: models/character.py:70
+#: models/character.py:72
 msgid "contracts"
 msgstr ""
 
-#: models/character.py:71
+#: models/character.py:73
 msgid "corporation history"
 msgstr ""
 
-#: models/character.py:72
+#: models/character.py:74
 msgid "faction warfare statistics"
 msgstr ""
 
-#: models/character.py:73
+#: models/character.py:75
 msgid "implants"
 msgstr ""
 
-#: models/character.py:74
+#: models/character.py:76
 msgid "jump clones"
 msgstr ""
 
-#: models/character.py:75
+#: models/character.py:77 models/general.py:185
 msgid "location"
 msgstr ""
 
-#: models/character.py:76
+#: models/character.py:78
 msgid "loyalty"
 msgstr ""
 
-#: models/character.py:77
+#: models/character.py:79
 msgid "mails"
 msgstr ""
 
-#: models/character.py:78
+#: models/character.py:80
 msgid "mining ledger"
 msgstr ""
 
-#: models/character.py:79
+#: models/character.py:81
 msgid "online status"
 msgstr ""
 
-#: models/character.py:80
+#: models/character.py:82
 msgid "ship"
 msgstr ""
 
-#: models/character.py:81 models/general.py:335
+#: models/character.py:83 models/general.py:353 models/general.py:386
 msgid "skills"
 msgstr ""
 
-#: models/character.py:82
+#: models/character.py:84
 msgid "skill queue"
 msgstr ""
 
-#: models/character.py:83 models/general.py:263
+#: models/character.py:85 models/general.py:271 models/general.py:340
 msgid "skill sets"
 msgstr ""
 
-#: models/character.py:84
+#: models/character.py:86
 msgid "wallet balance"
 msgstr ""
 
-#: models/character.py:85
+#: models/character.py:87
 msgid "wallet journal"
 msgstr ""
 
-#: models/character.py:86
+#: models/character.py:88
 msgid "wallet transactions"
 msgstr ""
 
-#: models/character.py:87
+#: models/character.py:89
 msgid "attributes"
 msgstr ""
 
-#: models/character.py:139
+#: models/character.py:141
 msgid "ok"
 msgstr ""
 
-#: models/character.py:140 models/sections.py:233
+#: models/character.py:142 models/sections.py:234
 msgid "in progress"
 msgstr ""
 
-#: models/character.py:141
+#: models/character.py:143
 msgid "incomplete"
 msgstr ""
 
-#: models/character.py:142
+#: models/character.py:144
 msgid "error"
 msgstr ""
 
-#: models/character.py:143
+#: models/character.py:145
 msgid "disabled"
 msgstr ""
 
-#: models/character.py:150
+#: models/character.py:152
 msgid "eve character"
 msgstr ""
 
-#: models/character.py:154
+#: models/character.py:156
 msgid "created at"
 msgstr ""
 
-#: models/character.py:158
+#: models/character.py:160
 msgid "is shared"
 msgstr ""
 
-#: models/character.py:163
+#: models/character.py:165
 msgid "is disabled"
 msgstr ""
 
-#: models/character.py:167
+#: models/character.py:169
 msgid "mailing lists"
 msgstr ""
 
-#: models/general.py:261 models/general.py:296
+#: models/character.py:177
+msgid "characters"
+msgstr ""
+
+#: models/character.py:1294 models/character.py:1295
+msgid "character update status"
+msgstr ""
+
+#: models/general.py:116
+msgid "compliance group designation"
+msgstr ""
+
+#: models/general.py:117
+msgid "compliance group designations"
+msgstr ""
+
+#: models/general.py:186
+msgid "locations"
+msgstr ""
+
+#: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr ""
 
-#: models/general.py:268
+#: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
-#: models/general.py:270
+#: models/general.py:278
 msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
-#: models/general.py:276
+#: models/general.py:284
 msgid "is active"
 msgstr ""
 
-#: models/general.py:277
+#: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr ""
 
-#: models/general.py:285
+#: models/general.py:290
+msgid "skill set group"
+msgstr ""
+
+#: models/general.py:291
+msgid "skill set groups"
+msgstr ""
+
+#: models/general.py:298
 msgid "Doctrine: "
 msgstr ""
 
-#: models/general.py:304
+#: models/general.py:317
 msgid "ship type"
 msgstr ""
 
-#: models/general.py:307
+#: models/general.py:320
 msgid ""
 "Ship type is used for visual presentation only. All skill requirements must "
 "be explicitly defined."
 msgstr ""
 
-#: models/general.py:315
+#: models/general.py:328
 msgid "is visible"
 msgstr ""
 
-#: models/general.py:317
+#: models/general.py:330
 msgid ""
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 
-#: models/general.py:340
+#: models/general.py:339
+msgid "skill set"
+msgstr ""
+
+#: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr ""
 
-#: models/general.py:349
+#: models/general.py:367
 msgid "required level"
 msgstr ""
 
-#: models/general.py:356
+#: models/general.py:374
 msgid "recommended level"
 msgstr ""
 
-#: models/general.py:412 templates/memberaudit/reports.html:75
+#: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:413
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
-#: models/general.py:414
+#: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
 #: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
-#: models/general.py:415
+#: models/general.py:436
 msgid "Mailing List"
 msgstr ""
 
-#: models/general.py:416
+#: models/general.py:437
 msgid "Unknown"
 msgstr ""
 
-#: models/sections.py:146
+#: models/sections.py:147
 msgid "excellent standing"
 msgstr ""
 
-#: models/sections.py:147
+#: models/sections.py:148
 msgid "good standing"
 msgstr ""
 
-#: models/sections.py:148
+#: models/sections.py:149
 msgid "neutral standing"
 msgstr ""
 
-#: models/sections.py:149
+#: models/sections.py:150
 msgid "bad standing"
 msgstr ""
 
-#: models/sections.py:150
+#: models/sections.py:151
 msgid "terrible standing"
 msgstr ""
 
-#: models/sections.py:204
+#: models/sections.py:205
 msgid "alliance"
 msgstr ""
 
-#: models/sections.py:205
+#: models/sections.py:206
 msgid "corporation"
 msgstr ""
 
-#: models/sections.py:206
+#: models/sections.py:207
 msgid "private"
 msgstr ""
 
-#: models/sections.py:207
+#: models/sections.py:208
 msgid "public"
 msgstr ""
 
-#: models/sections.py:227
+#: models/sections.py:228
 msgid "canceled"
 msgstr ""
 
-#: models/sections.py:228
+#: models/sections.py:229
 msgid "deleted"
 msgstr ""
 
-#: models/sections.py:229
+#: models/sections.py:230
 msgid "failed"
 msgstr ""
 
-#: models/sections.py:230
+#: models/sections.py:231
 msgid "finished"
 msgstr ""
 
-#: models/sections.py:231
+#: models/sections.py:232
 msgid "finished contractor"
 msgstr ""
 
-#: models/sections.py:232
+#: models/sections.py:233
 msgid "finished issuer"
 msgstr ""
 
-#: models/sections.py:234
+#: models/sections.py:235
 msgid "outstanding"
 msgstr ""
 
-#: models/sections.py:235
+#: models/sections.py:236
 msgid "rejected"
 msgstr ""
 
-#: models/sections.py:236
+#: models/sections.py:237
 msgid "reversed"
 msgstr ""
 
-#: models/sections.py:257
+#: models/sections.py:258
 msgid "auction"
 msgstr ""
 
-#: models/sections.py:258
+#: models/sections.py:259
 msgid "courier"
 msgstr ""
 
-#: models/sections.py:259
+#: models/sections.py:260
 msgid "item exchange"
 msgstr ""
 
-#: models/sections.py:260
+#: models/sections.py:261
 msgid "loan"
 msgstr ""
 
-#: models/sections.py:261
+#: models/sections.py:262
 msgid "unknown"
 msgstr ""
 
-#: models/sections.py:419
+#: models/sections.py:421
 msgid "[Multiple Items]"
 msgstr ""
 
 #: models/sections.py:520
 msgid "male"
 msgstr ""
 
@@ -690,31 +723,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -808,24 +855,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -835,22 +872,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1516,15 +1558,15 @@
 msgid "Character Finder"
 msgstr ""
 
 #: templates/memberaudit/partials/menu.html:50 views/reports.py:39
 msgid "Reports"
 msgstr ""
 
-#: templates/memberaudit/partials/menu.html:58 views/data_export.py:25
+#: templates/memberaudit/partials/menu.html:58 views/data_export.py:24
 msgid "Data Export"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:3
 msgid "Color code:"
 msgstr ""
 
@@ -1536,43 +1578,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1610,20 +1636,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1668,13 +1694,13 @@
 msgstr ""
 
 #: views/characters.py:156
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
-#: views/data_export.py:55
+#: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:134 admin.py:312
 msgid "update status"
@@ -73,80 +73,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -361,15 +361,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -722,31 +723,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -840,24 +855,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -867,22 +872,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1568,43 +1578,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1642,20 +1636,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1703,10 +1697,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -72,80 +72,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -360,15 +360,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -721,31 +722,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -839,24 +854,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -866,22 +871,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1567,43 +1577,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1641,20 +1635,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1702,10 +1696,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: German (https://app.transifex.com/kalkoken-apps/teams/107978/"
+"de/)\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:134 admin.py:312
 msgid "update status"
@@ -72,80 +73,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -360,15 +361,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -721,31 +723,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -839,24 +855,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -866,22 +872,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1567,43 +1578,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1641,20 +1636,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1702,10 +1697,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/ja/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: French (France) (https://app.transifex.com/kalkoken-apps/"
+"teams/107978/fr_FR/)\n"
+"Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 #: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:134 admin.py:312
 msgid "update status"
@@ -73,80 +74,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -361,15 +362,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -722,31 +724,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -840,24 +856,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -867,22 +873,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1568,43 +1579,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1642,20 +1637,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1703,10 +1698,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: Italian (Italy) (https://app.transifex.com/kalkoken-apps/"
+"teams/107978/it_IT/)\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
+"1 : 2;\n"
 
 #: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:134 admin.py:312
 msgid "update status"
@@ -72,80 +74,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -360,15 +362,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -721,31 +724,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -839,24 +856,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -866,22 +873,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1567,43 +1579,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1641,20 +1637,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1702,10 +1698,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: Russian (https://app.transifex.com/kalkoken-apps/teams/107978/"
-"ru/)\n"
-"Language: ru\n"
+"Language-Team: Japanese (https://app.transifex.com/kalkoken-apps/"
+"teams/107978/ja/)\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:134 admin.py:312
 msgid "update status"
@@ -75,80 +73,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -363,15 +361,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -724,31 +723,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -842,24 +855,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -869,22 +872,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1570,43 +1578,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1644,20 +1636,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1705,10 +1697,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/locale/uk/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 22:04+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: Ukrainian (https://app.transifex.com/kalkoken-apps/"
+"teams/107978/uk/)\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
@@ -76,80 +76,80 @@
 
 #: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
 #: admin.py:384
 #, python-format
-msgid "Started updating character: %s. "
+msgid "Started updating character %s."
 msgstr ""
 
 #: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:396
 #, python-format
-msgid "Started updating assets for character: %s."
+msgid "Started updating assets for character %s."
 msgstr ""
 
 #: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
 #: admin.py:421
 #, python-format
-msgid "Started updating %s for character: %s. "
+msgid "Started updating %s for character %s."
 msgstr ""
 
 #: admin.py:446
 #, python-format
-msgid "Started updating %s for character: %s."
+msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:451
+#: admin.py:454
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:455
+#: admin.py:458
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:457
+#: admin.py:460
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:461
+#: admin.py:464
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:493 models/general.py:267 models/general.py:307
+#: admin.py:496 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:497
+#: admin.py:500
 msgid "solar system"
 msgstr ""
 
-#: admin.py:501
+#: admin.py:504
 msgid "type"
 msgstr ""
 
-#: admin.py:505
+#: admin.py:508
 msgid "group"
 msgstr ""
 
-#: admin.py:509
+#: admin.py:512
 msgid "updated at"
 msgstr ""
 
-#: admin.py:570
+#: admin.py:573
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -364,15 +364,16 @@
 
 #: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:434
+#: models/general.py:434 templates/memberaudit/character_finder.html:18
+#: templates/memberaudit/character_finder.html:19
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
@@ -725,31 +726,45 @@
 #: templates/memberaudit/character_finder.html:10
 #: templates/memberaudit/launcher.html:11
 #: templates/memberaudit/partials/character_viewer/sidebar.html:7
 msgid "Characters"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:18
-msgid "Character<br>Name"
+#: templates/memberaudit/character_finder.html:20
+#: templates/memberaudit/data_export.html:15
+#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
+#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
+#: templates/memberaudit/modals/character_viewer/contract_items.html:6
+#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
+#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
+#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
+msgid "Name"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:19
-msgid "Character<br>Organization"
+#: templates/memberaudit/character_finder.html:21
+#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
+msgid "Organization"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:20
-msgid "Main<br>Name"
-msgstr ""
-
 #: templates/memberaudit/character_finder.html:21
-msgid "Main<br>Organization"
+#: templates/memberaudit/character_finder.html:22
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
+msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
-msgid "Main<br>State"
+#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
+#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
 msgid "Main character"
@@ -843,24 +858,14 @@
 msgid "Buy and Sell"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:10
 msgid "Topics"
 msgstr ""
 
-#: templates/memberaudit/data_export.html:15
-#: templates/memberaudit/modals/character_viewer/asset_container_content.html:26
-#: templates/memberaudit/modals/character_viewer/character_skill_set_details.html:22
-#: templates/memberaudit/modals/character_viewer/contract_items.html:6
-#: templates/memberaudit/modals/character_viewer/skill_set_content.html:45
-#: templates/memberaudit/partials/character_viewer/tabs/assets.html:9
-#: templates/memberaudit/partials/character_viewer/tabs/contacts.html:10
-msgid "Name"
-msgstr ""
-
 #: templates/memberaudit/data_export.html:16
 #: templates/memberaudit/modals/character_viewer/skill_set_content.html:37
 #: templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html:15
 msgid "Description"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:17
@@ -870,22 +875,27 @@
 #: templates/memberaudit/data_export.html:18
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
-"\n"
-"                    Export files contain the complete data of all "
-"<strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format "
-"and zipped.\n"
-"                    Existing export files can updated after "
-"%(minutes_until_next_update)s minutes.\n"
-"                "
+"Export files contain the complete data of all %(amount_of_characters)s "
+"characters known to Member Audit."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:46
+msgid "They are in CSV format and zipped."
+msgstr ""
+
+#: templates/memberaudit/data_export.html:47
+#, python-format
+msgid ""
+"Existing export files are updated after %(minutes_until_next_update)s "
+"minutes."
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
 #: templates/memberaudit/launcher.html:29
@@ -1571,43 +1581,27 @@
 msgid "partly compliant"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:6
 msgid "not compliant"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:8
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:12
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:10
-msgid "Organization"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:9
 msgid "Total Users"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:10
 msgid "Total Characters"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/corporation_compliance.html:11
 #, python-format
 msgid "Compliance %%"
 msgstr ""
 
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
-msgid "Main"
-msgstr ""
-
-#: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
-#: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
-msgid "State"
-msgstr ""
-
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:8
 msgid "User"
 msgstr ""
@@ -1645,20 +1639,20 @@
 #: views/admin.py:37
 #, python-format
 msgid "A skill set with the name %s already exists."
 msgstr ""
 
 #: views/admin.py:51 views/admin.py:89
 #, python-format
-msgid "Skill Set <b>%s</b> has been created"
+msgid "Skill Set %s has been created"
 msgstr ""
 
 #: views/admin.py:53 views/admin.py:91
 #, python-format
-msgid "Skill Set <b>%s</b> has been updated"
+msgid "Skill Set %s has been updated"
 msgstr ""
 
 #: views/admin.py:67
 msgid "Create skill set from fitting"
 msgstr ""
 
 #: views/admin.py:105
@@ -1706,10 +1700,10 @@
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
-"Data export for topic <strong>%s</strong> has been started. This can take a "
-"couple of minutes. You will get a notification once it is completed."
+"Data export for topic %s has been started. This can take a couple of "
+"minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/managers/character.py` & `aa_memberaudit-2.8.0/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/managers/general.py` & `aa_memberaudit-2.8.0/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/managers/sections.py` & `aa_memberaudit-2.8.0/memberaudit/managers/sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/migrations/0007_add_localization_2.py` & `aa_memberaudit-2.8.0/memberaudit/migrations/0007_add_localization_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/models/__init__.py` & `aa_memberaudit-2.8.0/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/models/character.py` & `aa_memberaudit-2.8.0/memberaudit/models/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/models/general.py` & `aa_memberaudit-2.8.0/memberaudit/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/models/sections.py` & `aa_memberaudit-2.8.0/memberaudit/models/sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_finder.html`

 * *Files 16% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         </div>
 
         <div class="panel-body">
             <div class="table-responsive">
                 <table class="table table-striped table-width-fix" id="tab_characters">
                     <thead>
                         <tr>
-                            <th>{% translate 'Character<br>Name' %}</th>
-                            <th>{% translate 'Character<br>Organization' %}</th>
-                            <th>{% translate 'Main<br>Name' %}</th>
-                            <th>{% translate 'Main<br>Organization' %}</th>
-                            <th>{% translate 'Main<br>State' %}</th>
+                            <th>{% translate 'Character' %}<br>{% translate 'Name' %}</th>
+                            <th>{% translate 'Character' %}<br>{% translate 'Organization' %}</th>
+                            <th>{% translate 'Main' %}<br>{% translate 'Name' %}</th>
+                            <th>{% translate 'Main' %}<br>{% translate 'Organization' %}</th>
+                            <th>{% translate 'Main' %}<br>{% translate 'State' %}</th>
                             <th></th>
                         </tr>
                     </thead>
 
                     <tbody></tbody>
                 </table>
             </div>
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/data_export.html`

 * *Files 15% similar despite different names*

```diff
@@ -38,19 +38,17 @@
                                 {% endif %}
                             </td>
                         </tr>
                     {% endfor %}
                 </tbody>
             </table>
             <p class="text-muted">
-                {% blocktranslate with amount_of_characters=character_count|intcomma %}
-                    Export files contain the complete data of all <strong>{{ amount_of_characters }}</strong>
-                    characters known to Member Audit. They are in CSV format and zipped.
-                    Existing export files can updated after {{ minutes_until_next_update }} minutes.
-                {% endblocktranslate %}
+                {% blocktranslate with amount_of_characters=character_count|intcomma %}Export files contain the complete data of all {{ amount_of_characters }} characters known to Member Audit.{% endblocktranslate %}
+                {% blocktranslate %}They are in CSV format and zipped.{% endblocktranslate %}
+                {% blocktranslate %}Existing export files are updated after {{ minutes_until_next_update }} minutes.{% endblocktranslate %}
             </p>
         </div>
     </div>
 {% endblock details %}
 
 {% block extra_css %}
     <link rel="stylesheet" href="{% static 'memberaudit/css/global.css' %}" type="text/css">
```

#### html2text {}

```diff
@@ -5,16 +5,17 @@
                                                                                            %} Download {% else
 {           {                 {                   {                                        %} Download {% endif
 {           {                 {                   {                                        %} {% if
 topic.title topic.description topic.rows|intcomma topic.last_updated_at|timesince|default: topic.update_allowed
 }}          }}                }}                  "no file" }}                             %} Update_now {%
                                                                                            else %} Update_now
                                                                                            {% endif %}
-{% blocktranslate with amount_of_characters=character_count|intcomma %} Export
+{% blocktranslate with amount_of_characters=character_count|intcomma %}Export
 files contain the complete data of all {{ amount_of_characters }} characters
-known to Member Audit. They are in CSV format and zipped. Existing export files
-can updated after {{ minutes_until_next_update }} minutes. {% endblocktranslate
-%}
+known to Member Audit.{% endblocktranslate %} {% blocktranslate %}They are in
+CSV format and zipped.{% endblocktranslate %} {% blocktranslate %}Existing
+export files are updated after {{ minutes_until_next_update }} minutes.{%
+endblocktranslate %}
 {% endblock details %} {% block extra_css %}
 
 
  {% endblock %} {% block extra_script %} {% endblock %}
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest.mock import patch
 
 from django.contrib.admin.sites import AdminSite
+from django.contrib.auth.models import User
 from django.test import RequestFactory, TestCase, override_settings
 from django.urls import reverse
 
 from allianceauth.eveonline.models import EveCorporationInfo
 from app_utils.testing import (
     create_authgroup,
     create_state,
@@ -286,7 +287,75 @@
     #     # Make sure the correct queryset is returned
     #     request = self.factory.get("/", {"is_ship_type": "no"})
     #     request.user = self.user
     #     changelist = my_modeladmin.get_changelist_instance(request)
     #     queryset = changelist.get_queryset(request)
     #     expected = {ss_1}
     #     self.assertSetEqual(set(queryset), expected)
+
+
+class TestSkillSetSkillAdmin(TestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        cls.factory = RequestFactory()
+        load_eveuniverse()
+        cls.superuser = User.objects.create_superuser("Superman")
+
+    def test_should_create_new_skill_set_with_required_level_only(self):
+        # given
+        self.client.force_login(self.superuser)
+        # when
+        response = self.client.post(
+            "/admin/memberaudit/skillset/add/",
+            data={
+                "name": "Bla Bla",
+                "skills-TOTAL_FORMS": 1,
+                "skills-INITIAL_FORMS": 0,
+                "skills-MIN_NUM_FORMS": 1,
+                "skills-MAX_NUM_FORMS": 1000,
+                "skills-0-eve_type": 24311,
+                "skills-0-required_level": 1,
+            },
+        )
+        # then
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(SkillSet.objects.filter(name="Bla Bla").count(), 1)
+
+    def test_should_create_new_skill_set_with_recommended_level_only(self):
+        # given
+        self.client.force_login(self.superuser)
+        # when
+        response = self.client.post(
+            "/admin/memberaudit/skillset/add/",
+            data={
+                "name": "Bla Bla",
+                "skills-TOTAL_FORMS": 1,
+                "skills-INITIAL_FORMS": 0,
+                "skills-MIN_NUM_FORMS": 1,
+                "skills-MAX_NUM_FORMS": 1000,
+                "skills-0-eve_type": 24311,
+                "skills-0-recommended_level": 1,
+            },
+        )
+        # then
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(SkillSet.objects.filter(name="Bla Bla").count(), 1)
+
+    def test_should_raise_error_when_no_level_given(self):
+        # given
+        self.client.force_login(self.superuser)
+        # when
+        response = self.client.post(
+            "/admin/memberaudit/skillset/add/",
+            data={
+                "name": "Bla Bla",
+                "skills-TOTAL_FORMS": 1,
+                "skills-INITIAL_FORMS": 0,
+                "skills-MIN_NUM_FORMS": 1,
+                "skills-MAX_NUM_FORMS": 1000,
+                "skills-0-eve_type": 24311,
+            },
+        )
+        # then
+        self.assertEqual(response.status_code, 200)
+        self.assertIn("error", response.content.decode("utf-8"))
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.8.0/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/utils.py` & `aa_memberaudit-2.8.0/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.8.0/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.8.0/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.8.0/memberaudit/tests/core/test_eft_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 from app_utils.esi_testing import BravadoResponseStub
 from app_utils.testing import NoSocketsTestCase
 
 from ...core.eft_parser import (
     MissingSectionsError,
     MissingTitleError,
+    UnknownShipTypeError,
     _EftItem,
     _EftSection,
+    _EftSlotType,
     _EftTextItem,
     _EftTextSection,
     _EveTypes,
     create_fitting_from_eft,
 )
 from ..testdata.factories import create_fitting_text
 from ..testdata.load_eveuniverse import load_eveuniverse
@@ -92,14 +94,23 @@
             create_fitting_from_eft(fitting_text)
 
     def test_should_raise_error_when_text_is_empty(self):
         # when
         with self.assertRaises(MissingSectionsError):
             create_fitting_from_eft("")
 
+    def test_should_raise_error_when_ship_type_is_invalid(self):
+        # given
+        fitting_text = create_fitting_text("fitting_unknown_ship_type.txt")
+        # when
+        with self.assertRaises(UnknownShipTypeError):
+            with patch(MODULE_PATH + "._load_eve_types") as m:
+                m.return_value = _EveTypes(), {"Unknown"}
+                create_fitting_from_eft(fitting_text)
+
     def test_should_report_unknown_types(self):
         # given
         fitting_text = create_fitting_text("fitting_tristan_unknown_types.txt")
         # when
         with patch(MODULE_PATH + ".EveEntity.objects.fetch_by_names_esi") as mock:
             mock.return_value = EveEntity.objects.none()
             fitting, errors = create_fitting_from_eft(fitting_text)
@@ -257,14 +268,19 @@
                 ["Drones", "Unknown-Type"]
             )
         # then
         self.assertEqual(eve_types.from_name("Drones"), drones)
         self.assertIsNone(eve_types.from_name("Unknown-Type"))
         self.assertIn("Unknown-Type", unknown_types)
 
+    def test_should_raise_error_when_not_passing_iterable(self):
+        # when/then
+        with self.assertRaises(TypeError):
+            _EveTypes.create_from_names("not an allowed iterable")
+
 
 class TestEftTextItem(NoSocketsTestCase):
     def test_should_create_slot_module(self):
         #  when
         item = _EftTextItem.create_from_line("Warp Disruptor II")
         # then
         self.assertEqual(item, _EftTextItem(item_type="Warp Disruptor II"))
@@ -282,19 +298,27 @@
         #  when
         item = _EftTextItem.create_from_line("Warp Disruptor II /OFFLINE")
         # then
         self.assertEqual(
             item, _EftTextItem(item_type="Warp Disruptor II", is_offline=True)
         )
 
-    def test_should_create_slot_module_empty(self):
+    def test_should_create_slot_empty_high_slot(self):
         #  when
         item = _EftTextItem.create_from_line("[Empty High slot]")
         # then
-        self.assertEqual(item, _EftTextItem())
+        expected = _EftTextItem(slot_type=_EftSlotType.HIGH_SLOT)
+        self.assertEqual(item, expected)
+
+    def test_should_create_slot_empty_sub_system_slot(self):
+        #  when
+        item = _EftTextItem.create_from_line("[Empty Subsystem slot]")
+        # then
+        expected = _EftTextItem(slot_type=_EftSlotType.SUBSYSTEM_SLOT)
+        self.assertEqual(item, expected)
 
     def test_should_create_non_slot_item(self):
         #  when
         item = _EftTextItem.create_from_line("Acolyte II x5")
         # then
         self.assertEqual(item, _EftTextItem(item_type="Acolyte II", quantity=5))
 
@@ -417,15 +441,15 @@
         # given
         item = _EftItem(
             item_type=EveType.objects.get(name="Agency 'Pyrolancea' DB5 Dose II")
         )
         # when/then
         self.assertTrue(item.is_booster())
 
-    def test_should_be_cyberimplant(self):
+    def test_should_be_cyber_implant(self):
         # given
         item = _EftItem(item_type=EveType.objects.get(name="High-grade Snake Alpha"))
         # when/then
         self.assertTrue(item.is_cyber_implant())
 
     def test_should_be_drone(self):
         # given
@@ -485,14 +509,29 @@
         )
         # when/then
         self.assertFalse(item.is_high_slot())
         self.assertFalse(item.is_med_slot())
         self.assertFalse(item.is_low_slot())
         self.assertTrue(item.is_rig_slot())
 
+    def test_should_handle_empty_item(self):
+        # given
+        empty_item = _EftItem()
+        # when/then
+        self.assertTrue(empty_item.is_empty)
+        self.assertFalse(empty_item.is_booster())
+        self.assertFalse(empty_item.is_cyber_implant())
+        self.assertFalse(empty_item.is_drone())
+        self.assertFalse(empty_item.is_fighter())
+        self.assertFalse(empty_item.is_high_slot())
+        self.assertFalse(empty_item.is_med_slot())
+        self.assertFalse(empty_item.is_low_slot())
+        self.assertFalse(empty_item.is_rig_slot())
+        self.assertFalse(empty_item.is_subsystem())
+
 
 class TestEftSection(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
 
@@ -522,15 +561,15 @@
         # given
         section = _EftSection(
             [_EftItem(item_type=EveType.objects.get(name="Acolyte II"), quantity=5)]
         )
         # when/then
         self.assertEqual(section.guess_category(), _EftSection.Category.DRONES_BAY)
 
-    def test_should_be_figher_bay(self):
+    def test_should_be_fighter_bay(self):
         # given
         section = _EftSection(
             [_EftItem(item_type=EveType.objects.get(name="Firbolg I"), quantity=5)]
         )
         # when/then
         self.assertEqual(section.guess_category(), _EftSection.Category.FIGHTER_BAY)
 
@@ -583,7 +622,19 @@
                 _EftItem(
                     item_type=EveType.objects.get(name="Small EM Shield Reinforcer I")
                 )
             ]
         )
         # when/then
         self.assertEqual(section.guess_category(), _EftSection.Category.RIG_SLOTS)
+
+    def test_should_be_slots(self):
+        # given
+        section = _EftSection(
+            [
+                _EftItem(
+                    item_type=EveType.objects.get(name="Small EM Shield Reinforcer I")
+                )
+            ]
+        )
+        # when/then
+        self.assertTrue(section.is_slots)
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.8.0/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.8.0/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.8.0/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.8.0/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/managers/test_sections.py` & `aa_memberaudit-2.8.0/memberaudit/tests/managers/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_1.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_2.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_3.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_4.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_4.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_5.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_5.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/test_sections.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/models/utils.py` & `aa_memberaudit-2.8.0/memberaudit/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         )
         request.user = self.superuser
         # when
         response = admin.admin_create_skillset_from_fitting(request)
         # then
         self.assertEqual(response.status_code, 302)
         self.assertTrue(mock_tasks.update_characters_skill_checks.delay.called)
-        self.assertTrue(mock_messages.warning.info)
+        self.assertTrue(mock_messages.info.called)
         skill_set.refresh_from_db()
         self.assertGreater(skill_set.skills.count(), 0)
 
     def test_should_create_new_skillset_and_assign_group(
         self, mock_tasks, mock_messages
     ):
         # given
@@ -172,15 +172,15 @@
         )
         request.user = self.superuser
         # when
         response = admin.admin_create_skillset_from_skill_plan(request)
         # then
         self.assertEqual(response.status_code, 302)
         self.assertTrue(mock_tasks.update_characters_skill_checks.delay.called)
-        self.assertTrue(mock_messages.warning.info)
+        self.assertTrue(mock_messages.info.called)
         skill_set.refresh_from_db()
         self.assertGreater(skill_set.skills.count(), 0)
 
     def test_should_create_new_skillset_and_assign_group(
         self, mock_tasks, mock_messages
     ):
         # given
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.8.0/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.8.0/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/_common.py` & `aa_memberaudit-2.8.0/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/admin.py` & `aa_memberaudit-2.8.0/memberaudit/views/admin.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,48 +19,27 @@
 @login_required
 @staff_member_required
 def admin_create_skillset_from_fitting(request):
     if request.method == "POST":
         form = ImportFittingForm(request.POST)
         if form.is_valid():
             fitting = form.cleaned_data["_fitting"]
-            skill_set_name = (
-                form.cleaned_data["skill_set_name"]
-                if form.cleaned_data["skill_set_name"]
-                else fitting.name
-            )
-            if (
-                not form.cleaned_data["can_overwrite"]
-                and SkillSet.objects.filter(name=skill_set_name).exists()
-            ):
-                messages.warning(
-                    request,
-                    _("A skill set with the name %s already exists." % fitting.name),
-                )
+            params = {"fitting": fitting, "user": request.user}
+            if form.cleaned_data["skill_set_group"]:
+                params["skill_set_group"] = form.cleaned_data["skill_set_group"]
+            if form.cleaned_data["skill_set_name"]:
+                params["skill_set_name"] = form.cleaned_data["skill_set_name"]
+            obj, created = SkillSet.objects.update_or_create_from_fitting(**params)
+            logger.info("Skill Set created from fitting with name: %s", fitting.name)
+            tasks.update_characters_skill_checks.delay(force_update=True)
+            if created:
+                msg = _("Skill Set %s has been created") % obj.name
             else:
-                params = {"fitting": fitting, "user": request.user}
-                if form.cleaned_data["skill_set_group"]:
-                    params["skill_set_group"] = form.cleaned_data["skill_set_group"]
-                if form.cleaned_data["skill_set_name"]:
-                    params["skill_set_name"] = form.cleaned_data["skill_set_name"]
-                obj, created = SkillSet.objects.update_or_create_from_fitting(**params)
-                logger.info(
-                    "Skill Set created from fitting with name: %s", fitting.name
-                )
-                tasks.update_characters_skill_checks.delay(force_update=True)
-                if created:
-                    msg = _("Skill Set <b>%s</b> has been created") % obj.name
-                else:
-                    msg = _("Skill Set <b>%s</b> has been updated") % obj.name
-                if form.cleaned_data["_errors"]:
-                    errors = form.cleaned_data["_errors"]
-                    msg += f" with issues:<br>- {'<br>- '.join(errors)}"
-                    messages.warning(request, format_html(msg))
-                else:
-                    messages.info(request, format_html(f"{msg}."))
+                msg = _("Skill Set %s has been updated") % obj.name
+            messages.info(request, format_html(f"{msg}."))
             return redirect("admin:memberaudit_skillset_changelist")
     else:
         form = ImportFittingForm()
     return render(
         request,
         "admin/memberaudit/skillset/import_skills.html",
         {
@@ -82,23 +61,18 @@
             params = {"skill_plan": skill_plan, "user": request.user}
             if form.cleaned_data["skill_set_group"]:
                 params["skill_set_group"] = form.cleaned_data["skill_set_group"]
             obj, created = SkillSet.objects.update_or_create_from_skill_plan(**params)
             logger.info("%s: Skill Set created from skill plan", skill_plan.name)
             tasks.update_characters_skill_checks.delay(force_update=True)
             if created:
-                msg = _("Skill Set <b>%s</b> has been created") % obj.name
-            else:
-                msg = _("Skill Set <b>%s</b> has been updated") % obj.name
-            if form.cleaned_data["_errors"]:
-                errors = form.cleaned_data["_errors"]
-                msg += f" {_('with issues')}:<br>- {'<br>- '.join(errors)}"
-                messages.warning(request, format_html(msg))
+                msg = _("Skill Set %s has been created") % obj.name
             else:
-                messages.info(request, format_html(f"{msg}."))
+                msg = _("Skill Set %s has been updated") % obj.name
+            messages.info(request, format_html(f"{msg}."))
             return redirect("admin:memberaudit_skillset_changelist")
     else:
         form = ImportSkillPlanForm()
     return render(
         request,
         "admin/memberaudit/skillset/import_skills.html",
         {
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/character_finder.py` & `aa_memberaudit-2.8.0/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.8.0/memberaudit/views/character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.8.0/memberaudit/views/character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/characters.py` & `aa_memberaudit-2.8.0/memberaudit/views/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/data_export.py` & `aa_memberaudit-2.8.0/memberaudit/views/data_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,14 @@
 @login_required
 @permission_required("memberaudit.exports_access")
 def data_export_run_update(request, topic: str):
     tasks.export_data_for_topic.delay(topic=topic, user_pk=request.user.pk)
     messages.info(
         request,
         _(
-            "Data export for topic <strong>%s</strong> has been started. "
+            "Data export for topic %s has been started. "
             "This can take a couple of minutes. "
             "You will get a notification once it is completed.",
         )
         % topic,
     )
     return redirect("memberaudit:data_export")
```

### Comparing `aa_memberaudit-2.7.0/memberaudit/views/reports.py` & `aa_memberaudit-2.8.0/memberaudit/views/reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/LICENSE` & `aa_memberaudit-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.7.0/README.md` & `aa_memberaudit-2.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 In addition character based reports gives leadership another valuable tool for managing their respective organization.
 
 For details on how to install and use Member Audit please see the [documentation](https://aa-memberaudit.readthedocs.io/en/latest/).
 
 ## Features
 
-Member Audit adds the following key features to Auth:
+Member Audit adds the following features to Auth:
 
 - Users can see an overview of all their characters with key information like their current location and wallet balance
 - Users can get full access to their characters to monitor them without having to open the Eve client (similar to the classic Eve ap "EveMon").
 - Applicants can temporarily share their characters with recruiters for vetting
 - Leadership can get full access to characters of their members for auditing (e.g. to check suspicious members)
 - Full access to characters currently includes the following information:
   - Assets
@@ -67,14 +67,15 @@
 - Admins can customize and configure Member Audit to fit their needs. e.g. change the app's name and define how often which type of data is updated from the Eve server
 
 - Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](https://aa-memberaudit.readthedocs.io/en/latest/user.html#compliance-groups))
 - Get notifications when a user removes a character that they had previously registered.
 - Designed to work efficiently with large number of characters
 - Data retention policy allows managing storage capacity needs
 - Data can be exported for processing it with third party apps like Google Sheets (currently wallet journal only)
+- Language support for English :us:, Russian :ru: and Chinese :cn:
 
 ## Highlights
 
 ### Character Launcher
 
 The main page for users to register their characters and get a key infos of all registered characters.
```

### Comparing `aa_memberaudit-2.7.0/pyproject.toml` & `aa_memberaudit-2.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 dynamic = ["version"]
 description = "An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [
     { name = "Erik Kalkoken", email = "kalkoken87@gmail.com" },
+    { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
+    { name = "Rebecca Murphy", email = "rebecca@rcmurphy.me" },
 ]
 keywords = [
     "allianceauth",
     "eveonline",
     "memberaudit",
 ]
 classifiers = [
@@ -24,19 +26,20 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
-    "allianceauth-app-utils>=1.16.1",
+    "allianceauth-app-utils>=1.18.0",
     "allianceauth>=3",
     "bleach",
     "dj-datatables-view",
     "django-eveuniverse>=0.19",
     "humanize",
     "unidecode",
 ]
```

### Comparing `aa_memberaudit-2.7.0/PKG-INFO` & `aa_memberaudit-2.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.7.0
+Version: 2.8.0
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-memberaudit
 Project-URL: Documentation, https://aa-memberaudit.readthedocs.io/en/latest/
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-memberaudit
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/issues
-Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Peter Pfeufer <develop@ppfeufer.de>, Rebecca Murphy <rebecca@rcmurphy.me>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: allianceauth,eveonline,memberaudit
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-Requires-Dist: allianceauth-app-utils>=1.16.1
+Requires-Dist: allianceauth-app-utils>=1.18.0
 Requires-Dist: allianceauth>=3
 Requires-Dist: bleach
 Requires-Dist: dj-datatables-view
 Requires-Dist: django-eveuniverse>=0.19
 Requires-Dist: humanize
 Requires-Dist: unidecode
 Description-Content-Type: text/markdown
@@ -65,15 +66,15 @@
 
 In addition character based reports gives leadership another valuable tool for managing their respective organization.
 
 For details on how to install and use Member Audit please see the [documentation](https://aa-memberaudit.readthedocs.io/en/latest/).
 
 ## Features
 
-Member Audit adds the following key features to Auth:
+Member Audit adds the following features to Auth:
 
 - Users can see an overview of all their characters with key information like their current location and wallet balance
 - Users can get full access to their characters to monitor them without having to open the Eve client (similar to the classic Eve ap "EveMon").
 - Applicants can temporarily share their characters with recruiters for vetting
 - Leadership can get full access to characters of their members for auditing (e.g. to check suspicious members)
 - Full access to characters currently includes the following information:
   - Assets
@@ -102,14 +103,15 @@
 - Admins can customize and configure Member Audit to fit their needs. e.g. change the app's name and define how often which type of data is updated from the Eve server
 
 - Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](https://aa-memberaudit.readthedocs.io/en/latest/user.html#compliance-groups))
 - Get notifications when a user removes a character that they had previously registered.
 - Designed to work efficiently with large number of characters
 - Data retention policy allows managing storage capacity needs
 - Data can be exported for processing it with third party apps like Google Sheets (currently wallet journal only)
+- Language support for English :us:, Russian :ru: and Chinese :cn:
 
 ## Highlights
 
 ### Character Launcher
 
 The main page for users to register their characters and get a key infos of all registered characters.
```

