# Comparing `tmp/allianceauth-corptools-2.5.4.tar.gz` & `tmp/allianceauth-corptools-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-corptools-2.5.4.tar", last modified: Fri Apr 14 09:34:32 2023, max compression
+gzip compressed data, was "allianceauth-corptools-2.5.5.tar", last modified: Mon May  8 08:29:30 2023, max compression
```

## Comparing `allianceauth-corptools-2.5.4.tar` & `allianceauth-corptools-2.5.5.tar`

### file list

```diff
@@ -1,218 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.114345 allianceauth-corptools-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-04-14 09:34:32.114345 allianceauth-corptools-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.046345 allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.050345 allianceauth-corptools-2.5.4/corptools/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    83911 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.054345 allianceauth-corptools-2.5.4/corptools/audit_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/audit_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/audit_views/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/audit_views/corporation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.054345 allianceauth-corptools-2.5.4/corptools/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/cogs/locate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/cogs/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.038345 allianceauth-corptools-2.5.4/corptools/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.054345 allianceauth-corptools-2.5.4/corptools/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/management/commands/__init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/management/commands/ct_import_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/management/commands/ct_import_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/management/commands/ct_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.082345 allianceauth-corptools-2.5.4/corptools/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0002_auto_20200507_1104.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0003_auto_20200507_1115.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0004_auto_20200507_1133.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0005_auto_20200508_1506.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0006_invtypematerials_type_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0007_auto_20200510_1357.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0008_auto_20200511_0801.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0009_auto_20200511_0816.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0010_auto_20200511_0853.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0011_characterwalletjournalentry_corporationwalletdivision_corporationwalletjournalentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0012_skilltotals.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0013_eveitemdogmaattribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0014_characteraudit_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0015_auto_20200614_0935.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0016_auto_20200622_0643.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0017_auto_20200727_0041.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0018_corporationwalletdivision_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0019_implant_jumpclone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0020_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0021_auto_20200804_0941.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0022_mapsystemgate_skilllist.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0023_auto_20200810_1350.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0024_auto_20200810_1458.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0025_mapjumpbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0026_auto_20200811_0846.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0027_skilllistfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0028_delete_skilllistfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0029_auto_20200815_0554.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0030_charactermarketorder_corporationmarketorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0031_auto_20200828_0855.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0032_auto_20200901_0537.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0033_skilllist_order_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0034_auto_20200928_0005.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0035_auto_20200929_0114.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0036_auto_20201017_0641.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0037_mapsystemmoon_mapsystemplanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0038_auto_20210112_0102.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0039_auto_20210112_0402.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0040_auto_20210112_0449.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0041_auto_20210112_1359.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0042_remove_skilllist_eft.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0043_auto_20210125_0758.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0044_auto_20210322_0805.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0045_bigkey_assets_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0046_auto_20210427_0734.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0047_auto_20210531_1025.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0048_maillabel_mailmessage_mailrecipient.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0049_alter_mailmessage_is_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0050_auto_20210713_0408.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0051_auto_20210713_0557.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0052_charactercontact_charactercontactlabel_corporationcontact_corporationcontactlabel.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0053_characteraudit_last_update_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0054_auto_20210808_0138.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0055_alter_characterroles_character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0056_auto_20210808_0414.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0057_alter_titlefilter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0058_auto_20210808_0635.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0059_invtypematerials_met_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0060_bridgeozonelevel.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0061_notificationtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0062_notificaiton_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0063_notification_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0064_notification_note_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0065_notification_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0066_final_notification_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0067_remove_notification_notification_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0068_rename_note_text_notification_notification_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0069_corptoolsconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0070_create_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0071_alter_corptoolsconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0072_alter_corporationaudit_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0073_remove_miningtaxpaymentcorp_corp_delete_miningtax_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0074_evelocation_managed_evelocation_managed_char_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0075_remove_notification_corptools_n_notific_77c7f2_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0076_remove_characterasset_corptools_c_type_id_05ccc2_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0077_fullyloadedfilter_reversed_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0078_characterwalletjournalentry_corptools_c_date_aebcea_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0079_characteraudit_last_update_location_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0080_alter_characterlocation_character.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0081_characterlocation_current_ship_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0082_characteraudit_last_update_contracts_contract_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0083_skilltotalhistory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/0084_characteraudit_last_update_loyaltypoints_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60116 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.038345 allianceauth-corptools-2.5.4/corptools/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.038345 allianceauth-corptools-2.5.4/corptools/static/corptools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.082345 allianceauth-corptools-2.5.4/corptools/static/corptools/char/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/asset-manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.038345 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.082345 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.094345 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1243160 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/2.826f313a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  4291100 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    80920 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   194548 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-04-14 09:34:31.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.094345 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/asset-manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.038345 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.094345 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.102345 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   573811 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2079719 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    41196 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   100264 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-14 09:33:08.000000 allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.102345 allianceauth-corptools-2.5.4/corptools/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.102345 allianceauth-corptools-2.5.4/corptools/task_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59336 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/char_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29753 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/corp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/etag_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/housekeeping_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/skill_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/task_helpers/update_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29225 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.102345 allianceauth-corptools-2.5.4/corptools/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.106345 allianceauth-corptools-2.5.4/corptools/templates/corptools/
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/admin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.110345 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/assets.html
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/assets_lists.html
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/char_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/char_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/clones.html
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/contacts.html
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/doctrine_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/market.html
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/notifications.html
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/public.html
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/react_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/roles.html
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/skills.html
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/status.html
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/character/wallet.html
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/corp_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.110345 allianceauth-corptools-2.5.4/corptools/templates/corptools/corporation/
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/corporation/corp_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/corporation/react_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.110345 allianceauth-corptools-2.5.4/corptools/templates/corptools/fittings/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/fittings/characters.html
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templates/corptools/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.110345 allianceauth-corptools-2.5.4/corptools/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templatetags/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templatetags/fittings_skill_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/templatetags/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.114345 allianceauth-corptools-2.5.4/corptools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/task_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/test_access_corp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50022 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/corptools/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:34:32.114345 allianceauth-corptools-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:34:32.114345 allianceauth-corptools-2.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/tests/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 09:31:15.000000 allianceauth-corptools-2.5.4/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.377477 allianceauth-corptools-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-08 08:29:30.377477 allianceauth-corptools-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.353477 allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.353477 allianceauth-corptools-2.5.5/corptools/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83911 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.353477 allianceauth-corptools-2.5.5/corptools/audit_views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/audit_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/audit_views/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/audit_views/corporation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.353477 allianceauth-corptools-2.5.5/corptools/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/cogs/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/cogs/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.349477 allianceauth-corptools-2.5.5/corptools/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.353477 allianceauth-corptools-2.5.5/corptools/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/management/commands/__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/management/commands/ct_import_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/management/commands/ct_import_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/management/commands/ct_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.361477 allianceauth-corptools-2.5.5/corptools/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0002_auto_20200507_1104.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0003_auto_20200507_1115.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0004_auto_20200507_1133.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0005_auto_20200508_1506.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0006_invtypematerials_type_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0007_auto_20200510_1357.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0008_auto_20200511_0801.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0009_auto_20200511_0816.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0010_auto_20200511_0853.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0011_characterwalletjournalentry_corporationwalletdivision_corporationwalletjournalentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0012_skilltotals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0013_eveitemdogmaattribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0014_characteraudit_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0015_auto_20200614_0935.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0016_auto_20200622_0643.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0017_auto_20200727_0041.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0018_corporationwalletdivision_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0019_implant_jumpclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0020_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0021_auto_20200804_0941.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0022_mapsystemgate_skilllist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0023_auto_20200810_1350.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0024_auto_20200810_1458.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0025_mapjumpbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0026_auto_20200811_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0027_skilllistfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0028_delete_skilllistfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0029_auto_20200815_0554.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0030_charactermarketorder_corporationmarketorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0031_auto_20200828_0855.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0032_auto_20200901_0537.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0033_skilllist_order_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0034_auto_20200928_0005.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0035_auto_20200929_0114.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0036_auto_20201017_0641.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0037_mapsystemmoon_mapsystemplanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0038_auto_20210112_0102.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0039_auto_20210112_0402.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0040_auto_20210112_0449.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0041_auto_20210112_1359.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0042_remove_skilllist_eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0043_auto_20210125_0758.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0044_auto_20210322_0805.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0045_bigkey_assets_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0046_auto_20210427_0734.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0047_auto_20210531_1025.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0048_maillabel_mailmessage_mailrecipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0049_alter_mailmessage_is_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0050_auto_20210713_0408.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0051_auto_20210713_0557.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0052_charactercontact_charactercontactlabel_corporationcontact_corporationcontactlabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0053_characteraudit_last_update_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0054_auto_20210808_0138.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0055_alter_characterroles_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0056_auto_20210808_0414.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0057_alter_titlefilter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0058_auto_20210808_0635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0059_invtypematerials_met_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0060_bridgeozonelevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0061_notificationtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0062_notificaiton_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0063_notification_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0064_notification_note_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0065_notification_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0066_final_notification_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0067_remove_notification_notification_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0068_rename_note_text_notification_notification_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0069_corptoolsconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0070_create_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0071_alter_corptoolsconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0072_alter_corporationaudit_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0073_remove_miningtaxpaymentcorp_corp_delete_miningtax_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0074_evelocation_managed_evelocation_managed_char_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0075_remove_notification_corptools_n_notific_77c7f2_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0076_remove_characterasset_corptools_c_type_id_05ccc2_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0077_fullyloadedfilter_reversed_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0078_characterwalletjournalentry_corptools_c_date_aebcea_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0079_characteraudit_last_update_location_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0080_alter_characterlocation_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0081_characterlocation_current_ship_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0082_characteraudit_last_update_contracts_contract_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0083_skilltotalhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0084_characteraudit_last_update_loyaltypoints_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/0085_characteraudit_last_update_mining_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61086 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.349477 allianceauth-corptools-2.5.5/corptools/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.349477 allianceauth-corptools-2.5.5/corptools/static/corptools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.361477 allianceauth-corptools-2.5.5/corptools/static/corptools/char/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/asset-manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.349477 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.361477 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.369477 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1243160 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/2.826f313a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  4291100 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    80920 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194548 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 08:29:30.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-08 08:29:29.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.369477 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/asset-manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.349477 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.369477 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   573811 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2079719 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    41196 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   100264 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-08 08:28:23.000000 allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/task_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61948 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/char_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29753 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/corp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/etag_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/housekeeping_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/skill_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19371 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/task_helpers/update_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/templates/corptools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/admin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/assets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/assets_lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/char_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/char_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/clones.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/contacts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/doctrine_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/market.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/notifications.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/public.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/react_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/roles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/skills.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/character/wallet.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/corp_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/templates/corptools/corporation/
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/corporation/corp_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/corporation/react_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/dashboard.corptools.status.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.373477 allianceauth-corptools-2.5.5/corptools/templates/corptools/fittings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/fittings/characters.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templates/corptools/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.377477 allianceauth-corptools-2.5.5/corptools/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templatetags/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templatetags/fittings_skill_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/templatetags/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.377477 allianceauth-corptools-2.5.5/corptools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/task_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/test_access_corp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50022 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/corptools/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:29:30.377477 allianceauth-corptools-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:30.377477 allianceauth-corptools-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/tests/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 08:26:40.000000 allianceauth-corptools-2.5.5/tests/views.py
```

### Comparing `allianceauth-corptools-2.5.4/LICENCE` & `allianceauth-corptools-2.5.5/LICENCE`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/PKG-INFO` & `allianceauth-corptools-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-corptools
-Version: 2.5.4
+Version: 2.5.5
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-corp-tools
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-corptools-2.5.4/README.md` & `allianceauth-corptools-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/PKG-INFO` & `allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-corptools
-Version: 2.5.4
+Version: 2.5.5
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-corp-tools
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-corptools-2.5.4/allianceauth_corptools.egg-info/SOURCES.txt` & `allianceauth-corptools-2.5.5/allianceauth_corptools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 corptools/migrations/0078_characterwalletjournalentry_corptools_c_date_aebcea_idx_and_more.py
 corptools/migrations/0079_characteraudit_last_update_location_and_more.py
 corptools/migrations/0080_alter_characterlocation_character.py
 corptools/migrations/0081_characterlocation_current_ship_name_and_more.py
 corptools/migrations/0082_characteraudit_last_update_contracts_contract_and_more.py
 corptools/migrations/0083_skilltotalhistory.py
 corptools/migrations/0084_characteraudit_last_update_loyaltypoints_and_more.py
+corptools/migrations/0085_characteraudit_last_update_mining_and_more.py
 corptools/migrations/__init__.py
 corptools/static/corptools/char/asset-manifest.json
 corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css
 corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css.map
 corptools/static/corptools/char/static/js/2.826f313a.chunk.js
 corptools/static/corptools/char/static/js/2.826f313a.chunk.js.LICENSE.txt
 corptools/static/corptools/char/static/js/2.826f313a.chunk.js.map
@@ -146,14 +147,15 @@
 corptools/task_helpers/housekeeping_tasks.py
 corptools/task_helpers/skill_helpers.py
 corptools/task_helpers/update_tasks.py
 corptools/templates/__init__.py
 corptools/templates/corptools/admin.html
 corptools/templates/corptools/base.html
 corptools/templates/corptools/corp_menu.html
+corptools/templates/corptools/dashboard.corptools.status.html
 corptools/templates/corptools/menu.html
 corptools/templates/corptools/character/assets.html
 corptools/templates/corptools/character/assets_lists.html
 corptools/templates/corptools/character/char_base.html
 corptools/templates/corptools/character/char_menu.html
 corptools/templates/corptools/character/clones.html
 corptools/templates/corptools/character/contacts.html
```

### Comparing `allianceauth-corptools-2.5.4/corptools/admin.py` & `allianceauth-corptools-2.5.5/corptools/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/api.py` & `allianceauth-corptools-2.5.5/corptools/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/app_settings.py` & `allianceauth-corptools-2.5.5/corptools/app_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 CORPTOOLS_APP_NAME = getattr(settings, "CORPTOOLS_APP_NAME", "Character Audit")
 
 CORPTOOLS_DISCORD_BOT_COGS = getattr(
     settings, 'CORPTOOLS_DISCORD_BOT_COGS', ["corptools.cogs.routes", "corptools.cogs.locate"])
 
 CT_CHAR_MAX_INACTIVE_DAYS = getattr(settings, 'CT_CHAR_MAX_INACTIVE_DAYS', 3)
+
 CT_CHAR_ASSETS_MODULE = getattr(settings, 'CT_CHAR_ASSETS_MODULE', True)
 CT_CHAR_STANDINGS_MODULE = getattr(settings, 'CT_CHAR_STANDINGS_MODULE', True)
 CT_CHAR_KILLMAILS_MODULE = getattr(settings, 'CT_CHAR_KILLMAILS_MODULE', True)
 CT_CHAR_FITTINGS_MODULE = getattr(settings, 'CT_CHAR_FITTINGS_MODULE', True)
-CT_CHAR_CALLENDAR_MODULE = getattr(settings, 'CT_CHAR_CALLENDAR_MODULE', True)
+CT_CHAR_CALENDAR_MODULE = getattr(settings, 'CT_CHAR_CALENDAR_MODULE', True)
 CT_CHAR_CONTACTS_MODULE = getattr(settings, 'CT_CHAR_CONTACTS_MODULE', True)
 CT_CHAR_NOTIFICATIONS_MODULE = getattr(
     settings, 'CT_CHAR_NOTIFICATIONS_MODULE', True)
 CT_CHAR_ROLES_MODULE = getattr(settings, 'CT_CHAR_ROLES_MODULE', True)
 CT_CHAR_INDUSTRY_MODULE = getattr(settings, 'CT_CHAR_INDUSTRY_MODULE', True)
 CT_CHAR_MINING_MODULE = getattr(settings, 'CT_CHAR_MINING_MODULE', True)
 CT_CHAR_WALLET_MODULE = getattr(settings, 'CT_CHAR_WALLET_MODULE', True)
@@ -43,16 +44,14 @@
     settings, 'CT_CHAR_ACTIVE_IGNORE_CONTACTS_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_NOTIFICATIONS_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_NOTIFICATIONS_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_ROLES_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_ROLES_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_INDUSTRY_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_INDUSTRY_MODULE', False)
-CT_CHAR_ACTIVE_IGNORE_MINING_MODULE = getattr(
-    settings, 'CT_CHAR_ACTIVE_IGNORE_MINING_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_WALLET_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_WALLET_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_SKILLS_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_SKILLS_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_CLONES_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_CLONES_MODULE', False)
 CT_CHAR_ACTIVE_IGNORE_LOCATIONS_MODULE = getattr(
@@ -63,14 +62,18 @@
     settings, 'CT_CHAR_ACTIVE_IGNORE_HELPER_MODULE', False)
 CT_CHAR_PAUSE_CONTRACTS = getattr(settings, 'CT_CHAR_PAUSE_CONTRACTS', False)
 
 # New scopes so existing all will fail so lets ignore this by default.
 CT_CHAR_ACTIVE_IGNORE_LOYALTYPOINTS_MODULE = getattr(
     settings, 'CT_CHAR_ACTIVE_IGNORE_LOYALTYPOINTS_MODULE', True)
 
+# Swap to true for a release or 2
+CT_CHAR_ACTIVE_IGNORE_MINING_MODULE = getattr(
+    settings, 'CT_CHAR_ACTIVE_IGNORE_MINING_MODULE', True)
+
 
 def get_character_scopes():
     _scopes = [
         # Base
         'publicData',
     ]
 
@@ -95,15 +98,15 @@
 
     if CT_CHAR_FITTINGS_MODULE:
         _scopes += [
             # Fittings
             'esi-fittings.read_fittings.v1',
         ]
 
-    if CT_CHAR_CALLENDAR_MODULE:
+    if CT_CHAR_CALENDAR_MODULE:
         _scopes += [
             # Callendar
             'esi-calendar.read_calendar_events.v1',
         ]
 
     if CT_CHAR_CONTACTS_MODULE:
         _scopes += [
@@ -224,14 +227,19 @@
         ]
 
     if CT_CHAR_NOTIFICATIONS_MODULE:
         _attribs += [
             # Notifications
             ("Notifications", 'last_update_notif'),
         ]
+    if CT_CHAR_NOTIFICATIONS_MODULE:
+        _attribs += [
+            # Notifications
+            ("Mining", 'last_update_mining'),
+        ]
 
     if CT_CHAR_ROLES_MODULE:
         _attribs += [
             # Roles
             ("Roles", 'last_update_roles'),
             ("Titles", 'last_update_titles'),
         ]
```

### Comparing `allianceauth-corptools-2.5.4/corptools/audit_views/character.py` & `allianceauth-corptools-2.5.5/corptools/audit_views/character.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/audit_views/corporation.py` & `allianceauth-corptools-2.5.5/corptools/audit_views/corporation.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/auth_hooks.py` & `allianceauth-corptools-2.5.5/corptools/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/cogs/locate.py` & `allianceauth-corptools-2.5.5/corptools/cogs/locate.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/cogs/routes.py` & `allianceauth-corptools-2.5.5/corptools/cogs/routes.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/management/commands/ct_import_cat.py` & `allianceauth-corptools-2.5.5/corptools/management/commands/ct_import_cat.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/management/commands/ct_import_tokens.py` & `allianceauth-corptools-2.5.5/corptools/management/commands/ct_import_tokens.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/management/commands/ct_setup.py` & `allianceauth-corptools-2.5.5/corptools/management/commands/ct_setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/managers.py` & `allianceauth-corptools-2.5.5/corptools/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0001_initial.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0004_auto_20200507_1133.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0004_auto_20200507_1133.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0005_auto_20200508_1506.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0005_auto_20200508_1506.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0007_auto_20200510_1357.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0007_auto_20200510_1357.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0008_auto_20200511_0801.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0008_auto_20200511_0801.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0009_auto_20200511_0816.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0009_auto_20200511_0816.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0010_auto_20200511_0853.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0010_auto_20200511_0853.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0011_characterwalletjournalentry_corporationwalletdivision_corporationwalletjournalentry.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0011_characterwalletjournalentry_corporationwalletdivision_corporationwalletjournalentry.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0012_skilltotals.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0012_skilltotals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0013_eveitemdogmaattribute.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0013_eveitemdogmaattribute.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0016_auto_20200622_0643.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0016_auto_20200622_0643.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0017_auto_20200727_0041.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0017_auto_20200727_0041.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0019_implant_jumpclone.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0019_implant_jumpclone.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0020_clone.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0020_clone.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0021_auto_20200804_0941.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0021_auto_20200804_0941.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0022_mapsystemgate_skilllist.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0022_mapsystemgate_skilllist.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0023_auto_20200810_1350.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0023_auto_20200810_1350.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0024_auto_20200810_1458.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0024_auto_20200810_1458.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0025_mapjumpbridge.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0025_mapjumpbridge.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0027_skilllistfile.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0027_skilllistfile.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0029_auto_20200815_0554.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0029_auto_20200815_0554.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0030_charactermarketorder_corporationmarketorder.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0030_charactermarketorder_corporationmarketorder.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0031_auto_20200828_0855.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0031_auto_20200828_0855.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0032_auto_20200901_0537.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0032_auto_20200901_0537.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0034_auto_20200928_0005.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0034_auto_20200928_0005.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0035_auto_20200929_0114.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0035_auto_20200929_0114.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0036_auto_20201017_0641.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0036_auto_20201017_0641.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0037_mapsystemmoon_mapsystemplanet.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0037_mapsystemmoon_mapsystemplanet.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0038_auto_20210112_0102.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0038_auto_20210112_0102.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0039_auto_20210112_0402.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0039_auto_20210112_0402.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0040_auto_20210112_0449.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0040_auto_20210112_0449.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0041_auto_20210112_1359.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0041_auto_20210112_1359.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0043_auto_20210125_0758.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0043_auto_20210125_0758.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0044_auto_20210322_0805.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0044_auto_20210322_0805.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0045_bigkey_assets_fix.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0045_bigkey_assets_fix.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0046_auto_20210427_0734.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0046_auto_20210427_0734.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0047_auto_20210531_1025.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0047_auto_20210531_1025.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0048_maillabel_mailmessage_mailrecipient.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0048_maillabel_mailmessage_mailrecipient.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0050_auto_20210713_0408.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0050_auto_20210713_0408.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0051_auto_20210713_0557.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0051_auto_20210713_0557.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0052_charactercontact_charactercontactlabel_corporationcontact_corporationcontactlabel.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0052_charactercontact_charactercontactlabel_corporationcontact_corporationcontactlabel.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0054_auto_20210808_0138.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0054_auto_20210808_0138.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0055_alter_characterroles_character.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0055_alter_characterroles_character.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0056_auto_20210808_0414.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0056_auto_20210808_0414.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0058_auto_20210808_0635.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0058_auto_20210808_0635.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0059_invtypematerials_met_type.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0059_invtypematerials_met_type.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0060_bridgeozonelevel.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0060_bridgeozonelevel.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0061_notificationtext.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0061_notificationtext.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0062_notificaiton_refactor.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0062_notificaiton_refactor.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0063_notification_verification.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0063_notification_verification.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0064_notification_note_text.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0064_notification_note_text.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0065_notification_sync.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0065_notification_sync.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0066_final_notification_checks.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0066_final_notification_checks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0069_corptoolsconfiguration.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0069_corptoolsconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0071_alter_corptoolsconfiguration_options.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0071_alter_corptoolsconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0072_alter_corporationaudit_options.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0072_alter_corporationaudit_options.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0074_evelocation_managed_evelocation_managed_char_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0074_evelocation_managed_evelocation_managed_char_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0076_remove_characterasset_corptools_c_type_id_05ccc2_idx_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0076_remove_characterasset_corptools_c_type_id_05ccc2_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0077_fullyloadedfilter_reversed_logic.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0077_fullyloadedfilter_reversed_logic.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0078_characterwalletjournalentry_corptools_c_date_aebcea_idx_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0078_characterwalletjournalentry_corptools_c_date_aebcea_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0079_characteraudit_last_update_location_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0079_characteraudit_last_update_location_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0080_alter_characterlocation_character.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0080_alter_characterlocation_character.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0081_characterlocation_current_ship_name_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0081_characterlocation_current_ship_name_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0082_characteraudit_last_update_contracts_contract_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0082_characteraudit_last_update_contracts_contract_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0083_skilltotalhistory.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0083_skilltotalhistory.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/migrations/0084_characteraudit_last_update_loyaltypoints_and_more.py` & `allianceauth-corptools-2.5.5/corptools/migrations/0084_characteraudit_last_update_loyaltypoints_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/models.py` & `allianceauth-corptools-2.5.5/corptools/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
     last_update_location = models.DateTimeField(
         null=True, default=None, blank=True)
 
     last_update_loyaltypoints = models.DateTimeField(
         null=True, default=None, blank=True)
 
+    last_update_mining = models.DateTimeField(
+        null=True, default=None, blank=True)
+
     balance = models.DecimalField(
         max_digits=20, decimal_places=2, null=True, default=None)
 
     def __str__(self):
         return "{}'s Character Data".format(self.character.character_name)
 
     class Meta:
@@ -140,14 +143,16 @@
             if app_settings.CT_CHAR_ROLES_MODULE and not app_settings.CT_CHAR_ACTIVE_IGNORE_ROLES_MODULE:
                 is_active = is_active and (self.last_update_roles > time_ref)
             if app_settings.CT_CHAR_MAIL_MODULE and not app_settings.CT_CHAR_ACTIVE_IGNORE_MAIL_MODULE:
                 is_active = is_active and (self.last_update_mails > time_ref)
             if app_settings.CT_CHAR_LOYALTYPOINTS_MODULE and not app_settings.CT_CHAR_ACTIVE_IGNORE_LOYALTYPOINTS_MODULE:
                 is_active = is_active and (
                     self.last_update_loyaltypoints > time_ref)
+            if app_settings.CT_CHAR_MINING_MODULE and not app_settings.CT_CHAR_ACTIVE_IGNORE_MINING_MODULE:
+                is_active = is_active and (self.last_update_mining > time_ref)
 
             if self.active != is_active:
                 self.active = is_active
                 self.save()
 
             return is_active
         except:
@@ -643,14 +648,32 @@
 class CharacterWalletJournalEntry(WalletJournalEntry):
     character = models.ForeignKey(CharacterAudit, on_delete=models.CASCADE)
     first_party_name = models.ForeignKey(
         EveName, on_delete=models.SET_NULL, null=True, default=None, related_name='char_first_party')
     second_party_name = models.ForeignKey(
         EveName, on_delete=models.SET_NULL, null=True, default=None, related_name='char_second_party')
 
+
+# Mining Models
+
+class CharacterMiningLedger(models.Model):
+    id = models.CharField(max_length=50, primary_key=True)
+    character = models.ForeignKey(CharacterAudit, on_delete=models.CASCADE)
+    date = models.DateField()
+    type_name = models.ForeignKey(EveItemType, on_delete=models.CASCADE)
+    system = models.ForeignKey(MapSystem, on_delete=models.CASCADE)
+    quantity = models.IntegerField()
+
+    @staticmethod
+    def create_primary_key(character_id, mining_record):
+        """
+            TODO investigate something else...
+        """
+        return f"{mining_record['date'].strftime('%Y%m%d')}-{mining_record['type_id']}-{character_id}-{mining_record['solar_system_id']}"
+
 # Market Models
 
 
 class MarketOrder(models.Model):
     order_id = models.BigIntegerField(primary_key=True)
 
     duration = models.IntegerField()
```

### Comparing `allianceauth-corptools-2.5.4/corptools/providers.py` & `allianceauth-corptools-2.5.5/corptools/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/schema.py` & `allianceauth-corptools-2.5.5/corptools/schema.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/asset-manifest.json` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/css/main.cbcba1c2.chunk.css.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/2.826f313a.chunk.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/2.826f313a.chunk.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.LICENSE.txt` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/2.826f313a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/main.61f2c55d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/char/static/js/runtime-main.80926ca1.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/asset-manifest.json` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/css/main.e430055c.chunk.css.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.LICENSE.txt` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/2.af7ad74b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/3.d54d0f0c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/main.764a1c86.chunk.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js.map` & `allianceauth-corptools-2.5.5/corptools/static/corptools/corp/static/js/runtime-main.60f313d0.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/static/css/style.css` & `allianceauth-corptools-2.5.5/corptools/static/css/style.css`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/task_helpers/char_tasks.py` & `allianceauth-corptools-2.5.5/corptools/task_helpers/char_tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import time
+from datetime import timedelta
 
 from allianceauth.eveonline.models import EveCorporationInfo
 from bravado import exception
 from celery import shared_task
 from django.core.cache import cache
 from django.utils import timezone
 from esi.models import Token
 
 from corptools.task_helpers.update_tasks import fetch_location_name
 
 from .. import providers
 from ..models import (CharacterAsset, CharacterAudit, CharacterContact,
                       CharacterContactLabel, CharacterLocation,
-                      CharacterMarketOrder, CharacterRoles, CharacterTitle,
+                      CharacterMarketOrder, CharacterMiningLedger,
+                      CharacterRoles, CharacterTitle,
                       CharacterWalletJournalEntry, Clone, Contract,
                       ContractItem, CorporationHistory, EveItemType,
                       EveLocation, EveName, Implant, JumpClone, LoyaltyPoint,
                       MailLabel, MailMessage, MailRecipient, Notification,
                       NotificationText, Skill, SkillQueue, SkillTotalHistory,
                       SkillTotals)
 from .etag_helpers import NotModifiedError, etag_results
@@ -367,14 +369,81 @@
     audit_char.last_update_assets = timezone.now()
     audit_char.save()
     audit_char.is_active()
 
     return "CT: Finished assets for: {}".format(audit_char.character.character_name)
 
 
+def update_character_mining(character_id, force_refresh=False):
+    audit_char = CharacterAudit.objects.get(
+        character__character_id=character_id)
+    logger.debug("Updating Mining for: {}".format(
+        audit_char.character.character_name))
+
+    req_scopes = ['esi-industry.read_character_mining.v1']
+
+    token = get_token(character_id, req_scopes)
+
+    if not token:
+        return "No Tokens"
+    try:
+        mining_op = providers.esi.client.Industry.get_characters_character_id_mining(
+            character_id=character_id)
+
+        ledger = etag_results(mining_op, token, force_refresh=force_refresh)
+
+        _st = time.perf_counter()
+        existings_pks = set(CharacterMiningLedger.objects.filter(
+            character=audit_char, date__gte=timezone.now()-timedelta(days=30)
+        ).values_list("id", flat=True))
+        type_ids = set()
+        new_events = []
+        old_events = []
+        for event in ledger:
+
+            type_ids.add(event.get('type_id'))
+            pk = CharacterMiningLedger.create_primary_key(character_id, event)
+            _e = CharacterMiningLedger(
+                character=audit_char,
+                id=pk,
+                date=event.get('date'),
+                type_name_id=event.get('type_id'),
+                system_id=event.get('solar_system_id'),
+                quantity=event.get('quantity')
+            )
+            if pk in existings_pks:
+                old_events.append(_e)
+            else:
+                new_events.append(_e)
+
+        EveItemType.objects.create_bulk_from_esi(list(type_ids))
+
+        if len(new_events):
+            CharacterMiningLedger.objects.bulk_create(
+                new_events, ignore_conflicts=True)
+
+        if len(old_events):
+            CharacterMiningLedger.objects.bulk_update(
+                old_events, fields=['quantity'])
+
+        logger.debug(
+            f"CT_TIME: {time.perf_counter()-_st} update_character_mining {character_id}")
+
+    except NotModifiedError:
+        logger.info("CT: No New Mining for: {}".format(
+            audit_char.character.character_name))
+        pass
+
+    audit_char.last_update_mining = timezone.now()
+    audit_char.save()
+    audit_char.is_active()
+
+    return "CT: Finished Mining for: {}".format(audit_char.character.character_name)
+
+
 def get_current_ship_location(character_id, force_refresh=False):
     audit_char = CharacterAudit.objects.get(
         character__character_id=character_id)
     req_scopes = ['esi-location.read_location.v1',
                   'esi-location.read_ship_type.v1']
 
     token = get_token(character_id, req_scopes)
@@ -543,15 +612,15 @@
                     character=audit_char,
                     context_id_type="market_transaction_id",
                     reason__exact="",
                     context_id=item.get('transaction_id')
                 ).update(
                     reason=message
                 )
-                print(f"{audit_char.character.character_name} {message}")
+                #print(f"{audit_char.character.character_name} {message}")
         logger.debug(
             f"CT_TIME: {time.perf_counter()-_st} update_character_transactions {character_id}")
 
     except NotModifiedError:
         logger.info("CT: No New wallet data for: {}".format(
             audit_char.character.character_name))
         pass
@@ -645,34 +714,38 @@
     req_scopes = ['esi-characters.read_loyalty.v1', ]
 
     token = get_token(character_id, req_scopes)
 
     if not token:
         return "No Tokens"
 
-    loyaltypoints_op = providers.esi.client.Loyalty.get_characters_character_id_loyalty_points(
-        character_id=character_id)
+    try:
+        loyaltypoints_op = providers.esi.client.Loyalty.get_characters_character_id_loyalty_points(
+            character_id=character_id)
 
-    loyaltypoints = etag_results(
-        loyaltypoints_op, token, force_refresh=force_refresh)
+        loyaltypoints = etag_results(
+            loyaltypoints_op, token, force_refresh=force_refresh)
 
-    _bulkcreate = []
+        _bulkcreate = []
 
-    for lp in loyaltypoints:
-        lp_corp, _ = EveName.objects.get_or_create_from_esi(
-            lp.get('corporation_id'))
+        for lp in loyaltypoints:
+            lp_corp, _ = EveName.objects.get_or_create_from_esi(
+                lp.get('corporation_id'))
 
-        _bulkcreate.append(
-            LoyaltyPoint(
-                character=audit_char,
-                corporation=lp_corp,
-                amount=lp.get('loyalty_points')))
+            _bulkcreate.append(
+                LoyaltyPoint(
+                    character=audit_char,
+                    corporation=lp_corp,
+                    amount=lp.get('loyalty_points')))
 
-    LoyaltyPoint.objects.bulk_create(
-        _bulkcreate, ignore_conflicts=True, batch_size=500)
+        LoyaltyPoint.objects.bulk_create(
+            _bulkcreate, ignore_conflicts=True, batch_size=500)
+    except NotModifiedError:
+        logger.info("CT: No New LP data for: {}".format(
+            audit_char.character.character_name))
 
     audit_char.last_update_loyaltypoints = timezone.now()
     audit_char.save()
     audit_char.is_active()
 
     return f"CT: Finished Loyalty Points for: {audit_char.character.character_name}"
 
@@ -1309,14 +1382,16 @@
     audit_char = CharacterAudit.objects.get(
         character__character_id=character_id)
 
     req_scopes = ['esi-contracts.read_character_contracts.v1']
 
     token = get_token(character_id, req_scopes)
 
+    new_contract_ids = []
+
     if not token:
         return False, []
     try:
         contracts_op = providers.esi.client.Contracts.get_characters_character_id_contracts(
             character_id=character_id)
 
         contracts = etag_results(
@@ -1378,27 +1453,27 @@
             Contract.objects.bulk_update(contract_models_old, batch_size=1000,
                                          fields=['date_accepted', 'date_completed', 'acceptor_id', 'date_expired', 'status',
                                                  'assignee_name', 'acceptor_name', 'issuer_corporation_name', 'issuer_name'])
 
         logger.debug(
             f"CT_TIME: {time.perf_counter()-_st} update_character_titles {character_id}")
 
+        new_contract_ids = [c.contract_id for c in contract_models_new]
+        if force_refresh:
+            new_contract_ids += [c.contract_id for c in contract_models_old]
+
     except NotModifiedError:
         logger.info("CT: No New Contracts for: {}".format(
             audit_char.character.character_name))
         pass
 
     audit_char.last_update_contracts = timezone.now()
     audit_char.save()
     audit_char.is_active()
 
-    new_contract_ids = [c.contract_id for c in contract_models_new]
-    if force_refresh:
-        new_contract_ids += [c.contract_id for c in contract_models_old]
-
     return "CT: Completed Contracts for: %s" % str(character_id), new_contract_ids
 
 
 def update_character_contract_items(character_id, contract_id, force_refresh=False):
     logger.debug("updating contract items for: %s (%s)" %
                  (str(character_id), str(contract_id)))
```

### Comparing `allianceauth-corptools-2.5.4/corptools/task_helpers/corp_helpers.py` & `allianceauth-corptools-2.5.5/corptools/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/task_helpers/etag_helpers.py` & `allianceauth-corptools-2.5.5/corptools/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/task_helpers/housekeeping_tasks.py` & `allianceauth-corptools-2.5.5/corptools/task_helpers/housekeeping_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/task_helpers/skill_helpers.py` & `allianceauth-corptools-2.5.5/corptools/task_helpers/skill_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/task_helpers/update_tasks.py` & `allianceauth-corptools-2.5.5/corptools/task_helpers/update_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             _region_models_updates.append(__region_upd)
         if __region_new:
             _region_models_creates.append(__region_new)
 
     MapRegion.objects.bulk_update(_region_models_updates, [
                                   'name', 'description'], batch_size=1000)  # bulk update
     MapRegion.objects.bulk_create(
-        _region_models_creates, batch_size=1000)  # bulk create
+        _region_models_creates, batch_size=1000, ignore_conflicts=True)  # bulk create
     # sample_mem()
     _processes = []
     _current_constellations = MapConstellation.objects.all(
     ).values_list('constellation_id', flat=True)
     with ThreadPoolExecutor(max_workers=20) as executor:
         for constellation in _constelations:
             _processes.append(executor.submit(
@@ -70,15 +70,15 @@
             _constelation_model_updates.append(__constelation_upd)
         if __constelation_new:
             _constelation_model_creates.append(__constelation_new)
 
     MapConstellation.objects.bulk_update(_constelation_model_updates, [
                                          'name', 'region_id'], batch_size=1000)  # bulk update
     MapConstellation.objects.bulk_create(
-        _constelation_model_creates, batch_size=1000)  # bulk create
+        _constelation_model_creates, batch_size=1000, ignore_conflicts=True)  # bulk create
     # sample_mem()
     _processes = []
     _current_systems = MapSystem.objects.all().values_list('system_id', flat=True)
     with ThreadPoolExecutor(max_workers=50) as executor:
         for system in _systems:
             _processes.append(executor.submit(
                 providers.esi._get_system, system, _current_systems))
@@ -91,15 +91,15 @@
             _system_models_creates.append(__system_new)
         if _gates:
             _gate_links_array += _gates
 
     MapSystem.objects.bulk_update(_system_models_updates, [
                                   'name', 'constellation_id', 'star_id', 'security_class', 'x', 'y', 'z', 'security_status'], batch_size=1000)  # bulk update
     MapSystem.objects.bulk_create(
-        _system_models_creates, batch_size=1000)  # bulk update
+        _system_models_creates, batch_size=1000, ignore_conflicts=True)  # bulk update
     # sample_mem()
     _processes = []
     _gate_links_array = set(_gate_links_array)
     with ThreadPoolExecutor(max_workers=50) as executor:
         for gate in _gate_links_array:
             _processes.append(executor.submit(
                 providers.esi._get_stargate, gate))
```

### Comparing `allianceauth-corptools-2.5.4/corptools/tasks.py` & `allianceauth-corptools-2.5.5/corptools/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
                                       update_character_clones,
                                       update_character_contacts,
                                       update_character_contract_items,
                                       update_character_contracts,
                                       update_character_location,
                                       update_character_loyaltypoints,
                                       update_character_mail_headers,
+                                      update_character_mining,
                                       update_character_notifications,
                                       update_character_order_history,
                                       update_character_orders,
                                       update_character_roles,
                                       update_character_skill_list,
                                       update_character_skill_queue,
                                       update_character_titles,
@@ -270,14 +271,19 @@
                 character.character.character_id, force_refresh=force_refresh))
 
     if app_settings.CT_CHAR_CONTACTS_MODULE:
         if (character.last_update_contacts or mindt) <= skip_date or force_refresh:
             que.append(update_char_contacts.si(
                 character.character.character_id, force_refresh=force_refresh))
 
+    if app_settings.CT_CHAR_MINING_MODULE:
+        if (character.last_update_mining or mindt) <= skip_date or force_refresh:
+            que.append(update_char_mining_ledger.si(
+                character.character.character_id, force_refresh=force_refresh))
+
     if app_settings.CT_CHAR_WALLET_MODULE:
         if (character.last_update_wallet or mindt) <= skip_date or force_refresh:
             que.append(update_char_wallet.si(
                 character.character.character_id, force_refresh=force_refresh))
             que.append(update_char_transactions.si(
                 character.character.character_id, force_refresh=force_refresh))
         if (character.last_update_orders or mindt) <= skip_date or force_refresh:
@@ -301,15 +307,14 @@
     if app_settings.CT_CHAR_LOYALTYPOINTS_MODULE:
         que.append(update_char_loyaltypoints.si(
             character.character.character_id, force_refresh=force_refresh))
 
     if app_settings.CT_CHAR_SKILLS_MODULE:
         # Must be last due to this being not a user level queue, Celery once will stall the queue here if characters on an account block.
         # TODO: make this better
-
         if (character.last_update_skills or mindt) <= skip_date or force_refresh:
             try:
                 que.append(cache_user_skill_list.si(
                     character.character.character_ownership.user_id, force_refresh=force_refresh))
             except ObjectDoesNotExist:
                 pass
 
@@ -372,14 +377,23 @@
         return update_character_skill_queue(character_id, force_refresh=force_refresh)
     except Exception as e:
         logger.exception(e)
         return "Failed"
 
 
 @shared_task(bind=True, base=QueueOnce)
+def update_char_mining_ledger(self, character_id, force_refresh=False):
+    try:
+        return update_character_mining(character_id, force_refresh=force_refresh)
+    except Exception as e:
+        logger.exception(e)
+        return "Failed"
+
+
+@shared_task(bind=True, base=QueueOnce)
 def update_char_notifications(self, character_id, force_refresh=False):
     try:
         return update_character_notifications(character_id, force_refresh=force_refresh)
     except Exception as e:
         logger.exception(e)
         return "Failed"
```

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/admin.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/admin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/base.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/assets.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/assets.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/assets_lists.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/assets_lists.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/char_base.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/char_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/char_menu.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/char_menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/clones.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/clones.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/contacts.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/contacts.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/market.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/market.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/notifications.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/notifications.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/public.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/public.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/react_base.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/react_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/roles.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/roles.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/skills.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/skills.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/status.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/status.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/character/wallet.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/character/wallet.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/corp_menu.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/corp_menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/corporation/corp_base.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/corporation/corp_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/corporation/react_base.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/corporation/react_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/fittings/characters.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/fittings/characters.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templates/corptools/menu.html` & `allianceauth-corptools-2.5.5/corptools/templates/corptools/menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templatetags/fittings_skill_tree.py` & `allianceauth-corptools-2.5.5/corptools/templatetags/fittings_skill_tree.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/templatetags/helpers.py` & `allianceauth-corptools-2.5.5/corptools/templatetags/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/__init__.py` & `allianceauth-corptools-2.5.5/corptools/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/test_access.py` & `allianceauth-corptools-2.5.5/corptools/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/test_access_corp.py` & `allianceauth-corptools-2.5.5/corptools/tests/test_access_corp.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/test_api.py` & `allianceauth-corptools-2.5.5/corptools/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/test_filters.py` & `allianceauth-corptools-2.5.5/corptools/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/test_provider.py` & `allianceauth-corptools-2.5.5/corptools/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/tests/test_templatetags.py` & `allianceauth-corptools-2.5.5/corptools/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/urls.py` & `allianceauth-corptools-2.5.5/corptools/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/corptools/views.py` & `allianceauth-corptools-2.5.5/corptools/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/setup.py` & `allianceauth-corptools-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/tests/celery.py` & `allianceauth-corptools-2.5.5/tests/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-2.5.4/tests/test_settings.py` & `allianceauth-corptools-2.5.5/tests/test_settings.py`

 * *Files identical despite different names*

