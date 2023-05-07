# Comparing `tmp/monopyly-1.2.3.tar.gz` & `tmp/monopyly-1.3.0.tar.gz`

## Comparing `monopyly-1.2.3.tar` & `monopyly-1.3.0.tar`

### file list

```diff
@@ -1,194 +1,202 @@
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/auth/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/auth/actions.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/auth/blueprint.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/auth/routes.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/auth/tools.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/__init__.py
--rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/accounts.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/actions.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/banks.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/blueprint.py
--rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/forms.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/routes.py
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/banking/transactions.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/cli/backup_db.py
--rwxr-xr-x   0        0        0     2643 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/cli/run.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/__init__.py
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/transactions.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/utils.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/forms/__init__.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/forms/_forms.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/forms/fields.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/forms/utils.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/common/forms/validators.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/config/__init__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/config/default_settings.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/config/settings.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/core/__init__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/core/blueprint.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/core/context_processors.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/core/filters.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/core/internal_transactions.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/core/routes.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/accounts.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/actions.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/blueprint.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/cards.py
--rw-r--r--   0        0        0    13180 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/forms.py
--rw-r--r--   0        0        0    18115 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/routes.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/statements.py
--rw-r--r--   0        0        0    13011 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/credit/transactions.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/__init__.py
--rw-r--r--   0        0        0    14294 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/handler.py
--rw-r--r--   0        0        0    17774 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/models.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/preloads.sql
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/schema.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/schema.sql
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/utils.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/database/views.sql
--rw-r--r--   0        0        0    88146 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/jquery-3.4.1.js
--rw-r--r--   0        0        0    45136 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/css/style.css
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/browserconfig.xml
--rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-114.png
--rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-120.png
--rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-144.png
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-150.png
--rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-152.png
--rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-16.png
--rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-160.png
--rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-180.png
--rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-192.png
--rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-310.png
--rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-32.png
--rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-57.png
--rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-60.png
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-64.png
--rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-70.png
--rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-72.png
--rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-76.png
--rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon-96.png
--rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon.ico
--rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/favicon/favicon.png
--rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/statement.png
--rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/cards/chase-card.png
--rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/cards/discover-card.png
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/cards/new-card.png
--rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/cards/template-card.png
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/arrow-down.png
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/arrow-left.png
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/arrow-up.png
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/checkmark.png
--rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/delete-orange-thick.png
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/delete-orange.png
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/delete-thick.png
--rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/delete.png
--rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/edit.png
--rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/link.png
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/minus-thick.png
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/minus.png
--rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/plus-thick.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/plus.png
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/refresh.png
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/save.png
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/sort-asc.png
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/sort-desc.png
--rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/statement.png
--rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/img/icons/x-thick.png
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/add_subtransaction.js
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/add_transfer.js
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/autocomplete_banking_transaction.js
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/autocomplete_credit_transaction.js
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/bind_tag_actions.js
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/define_filter.js
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/display_new_account_type_inputs.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/display_new_bank_inputs.js
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/display_new_credit_account_inputs.js
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/expand_bank_account.js
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/expand_transaction.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/flip_card.js
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/infer_card.js
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/infer_statement.js
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/make_payment.js
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/show_linked_transaction.js
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/update_account_statement_parameters.js
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/update_card_status.js
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/update_statement_parameters.js
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/update_statements_display.js
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/update_transactions_display.js
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/ajax.js
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/autocomplete_input.js
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/expand_transaction.js
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/manage_acquisition_form.js
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/manage_overlays.js
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/manage_subforms.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/update_database_widget.js
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/static/js/modules/update_display_ajax.js
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/about.html
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credits.html
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/index.html
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/layout.html
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/settings.html
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/auth/login.html
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/auth/register.html
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/account_page.html
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/account_summaries.html
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/account_summaries_page.html
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/account_summary.html
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/accounts_page.html
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/account_form/account_form.html
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/account_form/account_form_page_new.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/bank_info_form.html
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/subtransaction_form.html
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transaction_form/transfer_form.html
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/banking/transactions_table/transactions.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/form_page.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transaction_form/subform.html
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/linked_bank_transaction.html
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/linked_credit_transaction.html
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/subtransactions.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/transaction_condensed.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/transaction_expanded.html
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/common/transactions_table/transactions.html
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/account_page.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/card_submission_page.html
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/cards.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/cards_page.html
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/statement_page.html
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/statement_summary.html
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/statements.html
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/statements_page.html
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/tags_page.html
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transaction_submission_page.html
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transactions_page.html
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/card_form/card_form.html
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/card_form/card_form_page_new.html
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/card_graphic/card_back.html
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/card_graphic/card_front.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/tag_tree/subtag_tree.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/tag_tree/tag_tree.html
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transaction_form/subtransaction_form.html
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.2.3/monopyly/templates/credit/transactions_table/transactions.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 monopyly-1.2.3/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.2.3/COPYING
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.2.3/LICENSE
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 monopyly-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     9455 2020-02-02 00:00:00.000000 monopyly-1.2.3/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.3.0/README.md -> monopyly/README.md
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/README.md
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/_version.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/actions.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/blueprint.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/routes.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/auth/tools.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/__init__.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/accounts.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/actions.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/banks.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/blueprint.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/forms.py
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/routes.py
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/banking/transactions.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/cli/run.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/__init__.py
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/transactions.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/utils.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/__init__.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/_forms.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/fields.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/utils.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/common/forms/validators.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/config/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/config/default_settings.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/config/settings.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/__init__.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/actions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/blueprint.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/context_processors.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/filters.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/internal_transactions.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/core/routes.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/__init__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/accounts.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/actions.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/blueprint.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/cards.py
+-rw-r--r--   0        0        0    12008 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/forms.py
+-rw-r--r--   0        0        0    18257 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/routes.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/statements.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/credit/transactions.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/__init__.py
+-rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/models.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/preloads.sql
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/schema.sql
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/database/views.sql
+-rw-r--r--   0        0        0    88146 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/jquery-3.4.1.js
+-rw-r--r--   0        0        0    47317 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/css/style.css
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/browserconfig.xml
+-rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-114.png
+-rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-120.png
+-rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-144.png
+-rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-150.png
+-rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-152.png
+-rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-16.png
+-rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-160.png
+-rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-180.png
+-rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-192.png
+-rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-310.png
+-rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-32.png
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-57.png
+-rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-60.png
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-64.png
+-rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-70.png
+-rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-72.png
+-rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-76.png
+-rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon-96.png
+-rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon.ico
+-rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/favicon/favicon.png
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/statement.png
+-rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/bank-account-details.png
+-rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/bank-account-summaries.png
+-rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/bank-accounts.png
+-rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/credit-account-details.png
+-rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/credit-transactions.png
+-rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/homepage-user.png
+-rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/homepage.png
+-rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/about/statement-details.png
+-rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/chase-card.png
+-rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/discover-card.png
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/new-card.png
+-rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/cards/template-card.png
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/arrow-down.png
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/arrow-left.png
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/arrow-up.png
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/checkmark.png
+-rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete-orange-thick.png
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete-orange.png
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete-thick.png
+-rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/delete.png
+-rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/edit.png
+-rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/link.png
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/minus-thick.png
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/minus.png
+-rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/plus-thick.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/plus.png
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/refresh.png
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/save.png
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/sort-asc.png
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/sort-desc.png
+-rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/statement.png
+-rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/img/icons/x-thick.png
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/add_subtransaction.js
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/add_transfer.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/autocomplete_transaction.js
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/bind_tag_actions.js
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/define_filter.js
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/display_new_account_type_inputs.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/display_new_bank_inputs.js
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/display_new_credit_account_inputs.js
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/expand_bank.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/expand_bank_account.js
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/expand_transaction.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/flip_card.js
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/infer_card.js
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/infer_statement.js
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/make_payment.js
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/show_linked_transaction.js
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_account_statement_parameters.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_bank_name.js
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_card_status.js
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_statement_parameters.js
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_statements_display.js
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/update_transactions_display.js
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/ajax.js
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/autocomplete_input.js
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/expand_box_row.js
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/expand_transaction.js
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/manage_acquisition_form.js
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/manage_overlays.js
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/manage_subforms.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/update_database_widget.js
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/static/js/modules/update_display_ajax.js
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credits.html
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/index.html
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/layout.html
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/profile.html
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/story.html
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/auth/login.html
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/auth/register.html
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_page.html
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_summaries.html
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_summaries_page.html
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_summary.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/accounts_page.html
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_form/account_form.html
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/account_form/account_form_page_new.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/bank_info_form.html
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transaction_form/transfer_form.html
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/banking/transactions_table/transactions.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/form_page.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transaction_form/subform.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transaction_form/subtransaction_subform.html
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_bank_transaction.html
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_credit_transaction.html
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/subtransactions.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/transaction_condensed.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/transaction_expanded.html
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/common/transactions_table/transactions.html
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/account_page.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_submission_page.html
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/cards.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/cards_page.html
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statement_page.html
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statement_summary.html
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statements.html
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/statements_page.html
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/tags_page.html
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_submission_page.html
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_page.html
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_form/card_form.html
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_form/card_form_page_new.html
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_back.html
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_front.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/tag_tree/subtag_tree.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/tag_tree/tag_tree.html
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.3.0/monopyly/templates/credit/transactions_table/transactions.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 monopyly-1.3.0/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.3.0/COPYING
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 monopyly-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 monopyly-1.3.0/PKG-INFO
```

### Comparing `monopyly-1.2.3/monopyly/__init__.py` & `monopyly-1.3.0/monopyly/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 """
 import warnings
 from pathlib import Path
 
 from flask import Flask
 
 from monopyly.config import DevelopmentConfig, ProductionConfig
-from monopyly.database import DB_NAME, SQLAlchemy, close_db, db, init_db_command
+from monopyly.database import (
+    DB_NAME,
+    SQLAlchemy,
+    back_up_db_command,
+    db,
+    init_db_command,
+)
 
 
 def create_app(test_config=None):
     # Create and configure the app
-    app = Flask(
-        __name__,
-        instance_relative_config=True,
-    )
+    app = Flask(__name__, instance_relative_config=True)
 
+    # Prepare the app configuration
     if test_config:
-        # Load the test config if that is passed instead
         config = test_config
     else:
         # Ensure the instance path exists
         instance_path = Path(app.instance_path)
         instance_path.mkdir(parents=True, exist_ok=True)
         # Load the development/production config when not testing
         if app.debug:
@@ -35,42 +38,31 @@
             db_path = instance_path / DB_NAME
             config = ProductionConfig(db_path=db_path)
             # Give a while the secret key remains insecure
             warnings.formatwarning = lambda msg, *args, **kwargs: f"\n{msg}\n"
             warnings.warn("INSECURE: Production mode has not yet been fully configured")
     app.config.from_object(config)
 
-    # Allow the databases to be initialized from the command line
+    # Initialize the app, including CLI commands and blueprints
     init_app(app)
-    register_blueprints(app)
     return app
 
 
 def _get_preload_data_path(instance_path):
     dev_data_path = instance_path / "preload_dev_data.sql"
     return dev_data_path if dev_data_path.exists() else None
 
 
+@SQLAlchemy.interface_selector(db)
 def init_app(app):
     """Initialize the app."""
-    # Establish behavior for closing the database
-    app.teardown_appcontext(close_db)
-    # Register the database intialization with the app
+    register_blueprints(app)
+    # Register the database actions with the app
     app.cli.add_command(init_db_command)
-    # Prepare database access with SQLAlchemy
-    #   - Use the `app.db` attribute like the `app.extensions` dict
-    #     (but not actually that dict because this is not an extension)
-    if app.testing:
-        app.db = SQLAlchemy()
-    else:
-        app.db = db
-    app.db.setup_engine(db_path=app.config["DATABASE"])
-    # If the database is new, it will not yet have been properly populated
-    if not app.testing and Path(app.config["DATABASE"]).exists():
-        app.db.access_tables()
+    app.cli.add_command(back_up_db_command)
 
 
 def register_blueprints(app):
     """
     Register blueprints with the app.
 
     Note
```

### Comparing `monopyly-1.2.3/monopyly/auth/routes.py` & `monopyly-1.3.0/monopyly/auth/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/auth/tools.py` & `monopyly-1.3.0/monopyly/auth/tools.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/banking/accounts.py` & `monopyly-1.3.0/monopyly/banking/accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Tools for interacting with bank accounts in the database.
 """
 import sqlalchemy.sql.functions as sql_func
+from authanor.database.handler import DatabaseViewHandler
 from werkzeug.exceptions import abort
 
 from ..common.forms.utils import execute_on_form_validation
-from ..database.handler import DatabaseViewHandler
 from ..database.models import (
     Bank,
     BankAccount,
     BankAccountType,
     BankAccountTypeView,
     BankAccountView,
 )
@@ -81,19 +81,18 @@
         Returns
         -------
         account_type : database.models.BankAccountType
             A model containing bank account type information from the
             database matching the given criteria. If no matching account
             type is found, returns `None`.
         """
-        criteria = [
-            cls._filter_value(cls.model.type_name, type_name),
-            cls._filter_value(cls.model.type_abbreviation, type_abbreviation),
-        ]
-        account_type = super().find_entry(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(cls.model, "type_name", type_name)
+        criteria.add_match_filter(cls.model, "type_abbreviation", type_abbreviation)
+        account_type = super().find_entry(criteria=criteria)
         return account_type
 
     @classmethod
     def add_entry(cls, **mapping):
         # To Do: Should prevent a user from duplicating the common entries
         return super().add_entry(**mapping)
 
@@ -110,16 +109,16 @@
         ----------
         entry_id : int
             The ID of the account type to be deleted.
         """
         super().delete_entry(entry_id)
 
     @classmethod
-    def _confirm_manipulation_authorization(cls, entry_id):
-        account_type = super()._confirm_manipulation_authorization(entry_id)
+    def _validate_authorization(cls, entry_id):
+        account_type = super()._validate_authorization(entry_id)
         # Limit manipulation to only the user (excluding common entries)
         if account_type.user_id != cls.user_id:
             abort_msg = (
                 "The current user is not authorized to manipulate "
                 "this account type entry."
             )
             abort(404, abort_msg)
@@ -162,19 +161,18 @@
             selected).
 
         Returns
         -------
         accounts : sqlalchemy.engine.ScalarResult
             Returns bank accounts matching the criteria.
         """
-        criteria = [
-            cls._filter_values(cls.model.bank_id, bank_ids),
-            cls._filter_values(cls.model.account_type_id, account_type_ids),
-        ]
-        accounts = super().get_entries(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(cls.model, "bank_id", bank_ids)
+        criteria.add_match_filter(cls.model, "account_type_id", account_type_ids)
+        accounts = super().get_entries(criteria=criteria)
         return accounts
 
     @classmethod
     @DatabaseViewHandler.view_query
     def get_bank_balance(cls, bank_id):
         """Get the balance of all accounts at one bank."""
         query = cls.model.select_for_user(sql_func.sum(cls.model.balance))
@@ -218,27 +216,26 @@
 
         Returns
         -------
         account : database.models.BankAccountView
             A bank account entry matching the given criteria. If no
             matching account is found, returns `None`.
         """
-        criteria = [
-            cls._filter_value(Bank.bank_name, bank_name),
-            cls._filter_value(BankAccountTypeView.type_name, account_type_name),
-            cls._filter_value(cls.model.last_four_digits, last_four_digits),
-        ]
-        account = super().find_entry(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(Bank, "bank_name", bank_name)
+        criteria.add_match_filter(BankAccountTypeView, "type_name", account_type_name)
+        criteria.add_match_filter(cls.model, "last_four_digits", last_four_digits)
+        account = super().find_entry(criteria=criteria)
         return account
 
     @classmethod
-    def _filter_entries(cls, query, filters):
+    def _filter_entries(cls, query, criteria):
         # Add a join to enable filtering by bank account type
         query = query.join(BankAccountTypeView)
-        return super()._filter_entries(query, filters)
+        return super()._filter_entries(query, criteria)
 
     @classmethod
     def delete_entry(cls, entry_id):
         """
         Delete a bank account from the database.
 
         Given an account ID, delete the bank account from the database.
```

### Comparing `monopyly-1.2.3/monopyly/banking/actions.py` & `monopyly-1.3.0/monopyly/banking/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/banking/banks.py` & `monopyly-1.3.0/monopyly/banking/banks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tools for interacting with banks in the database.
 """
-from ..database.handler import DatabaseHandler
+from authanor.database.handler import DatabaseHandler
+
 from ..database.models import Bank
 
 
 class BankHandler(DatabaseHandler, model=Bank):
     """
     A database handler for managing bank information.
 
@@ -35,16 +36,17 @@
             (if `None`, all banks will be selected).
 
         Returns
         -------
         banks : sqlalchemy.engine.ScalarResult
             Returns bank entries matching the criteria.
         """
-        criteria = [cls._filter_values(cls.model.bank_name, bank_names)]
-        return super().get_entries(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(cls.model, "bank_name", bank_names)
+        return super().get_entries(criteria=criteria)
 
     @classmethod
     def delete_entry(cls, entry_id):
         """
         Delete a bank from the database.
 
         Given a bank ID, delete the bank from the database. Deleting an
```

### Comparing `monopyly-1.2.3/monopyly/banking/forms.py` & `monopyly-1.3.0/monopyly/banking/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """
 Generate banking forms for the user to complete.
 """
 from wtforms.fields import BooleanField, FieldList, FormField, StringField, SubmitField
 from wtforms.validators import DataRequired, Optional
 
 from ..common.forms import AcquisitionSubform, EntryForm, EntrySubform, TransactionForm
-from ..common.forms.fields import CustomChoiceSelectField, LastFourDigitsField
+from ..common.forms.fields import (
+    CustomChoiceSelectField,
+    DateField,
+    LastFourDigitsField,
+    StringField,
+)
 from ..common.forms.utils import Autocompleter
 from ..common.utils import parse_date
 from ..database.models import (
     Bank,
     BankAccountTypeView,
     BankAccountView,
     BankSubtransaction,
     BankTransaction,
     BankTransactionView,
+    TransactionTag,
 )
 from .accounts import BankAccountHandler, BankAccountTypeHandler
 from .banks import BankHandler
 
 
 class BankSelectField(CustomChoiceSelectField):
     """Bank field that uses the database to prepare field choices."""
@@ -179,27 +185,20 @@
             else:
                 self._raise_gather_fail_error((BankAccountView, Bank), entry)
             return data
 
     class SubtransactionSubform(TransactionForm.SubtransactionSubform):
         """Form to input/edit bank subtransactions."""
 
-        def gather_entry_data(self, entry):
-            """Gather data for the form from the given database entry."""
-            if isinstance(entry, BankSubtransaction):
-                data = {
-                    "subtotal": entry.subtotal,
-                    "note": entry.note,
-                }
-            else:
-                self._raise_gather_fail_error((BankSubtransaction,), entry)
-            return data
+        subtransaction_model = BankSubtransaction
 
     # Fields to identify the bank account information for the transaction
     account_info = FormField(AccountSubform)
+    # Fields pertaining to the bank transaction
+    merchant = StringField("Merchant")
     # Subtransaction fields (must be at least 1 subtransaction)
     subtransactions = FieldList(
         FormField(SubtransactionSubform, render_kw={"class": "subtransaction-form"}),
         min_entries=1,
     )
     # Fields to identify a second bank involved in a funds transfer
     transfer_accounts_info = FieldList(
@@ -209,15 +208,17 @@
     )
     # Define an autocompleter for the form
     _autocompleter = Autocompleter(
         {
             "bank_name": Bank,
             "type_name": BankAccountTypeView,
             "last_four_digits": BankAccountView,
+            "merchant": BankTransaction,
             "note": BankSubtransaction,
+            "tags": TransactionTag,
         }
     )
 
     @property
     def transfer_account_info(self):
         if not self.transfer_accounts_info:
             return None
@@ -248,14 +249,16 @@
         different and the subtotals of subtransactions have the opposite
         (negated) amount.
         """
         if not self.transfer_account_info:
             return None
         account = self.get_transfer_account()
         transfer_data = self._prepare_transaction_data(account)
+        # Use the bank initiating the transaction as the merchant
+        transfer_data["merchant"] = self.get_transaction_account().bank.bank_name
         # Negate transfer subtotals as the opposite of the original transaction
         for subtransaction_data in transfer_data["subtransactions"]:
             subtransaction_data["subtotal"] = -subtransaction_data["subtotal"]
         return transfer_data
 
     def get_transaction_account(self):
         """Get the bank account associated with the transaction."""
```

### Comparing `monopyly-1.2.3/monopyly/banking/routes.py` & `monopyly-1.3.0/monopyly/banking/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     # Add a new subtransaction to the form
     new_subform = extend_field_list_for_ajax(
         BankTransactionForm,
         "subtransactions",
         subtransaction_count,
     )
     return render_template(
-        "banking/transaction_form/subtransaction_form.html",
+        "common/transaction_form/subtransaction_subform.html",
         subform=new_subform,
         field_list_optional_member=True,
     )
 
 
 @bp.route("/_add_transfer_field", methods=("POST",))
 @login_required
@@ -216,9 +216,30 @@
 
 @bp.route("/_suggest_transaction_autocomplete", methods=("POST",))
 @login_required
 def suggest_transaction_autocomplete():
     # Get the autocomplete field from the AJAX request
     post_args = request.get_json()
     field = post_args["field"]
-    suggestions = BankTransactionForm.autocomplete(field)
+    if field == "tags":
+        suggestions = BankTransactionForm.autocomplete("tags", db_field_name="tag_name")
+    else:
+        suggestions = BankTransactionForm.autocomplete(field)
     return jsonify(suggestions)
+
+
+@bp.route("/_update_bank_name/<int:bank_id>", methods=("POST",))
+@login_required
+@db_transaction
+def update_bank_name(bank_id):
+    # Get the bank name from the AJAX request
+    bank_name = request.get_json()
+    BankHandler.update_entry(bank_id, bank_name=bank_name)
+    return bank_name
+
+
+@bp.route("/delete_bank/<int:bank_id>")
+@login_required
+@db_transaction
+def delete_bank(bank_id):
+    BankHandler.delete_entry(bank_id)
+    return redirect(url_for("core.load_profile"))
```

### Comparing `monopyly-1.2.3/monopyly/cli/run.py` & `monopyly-1.3.0/monopyly/cli/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,32 @@
 
 
 def main():
     args = parse_arguments()
     app_runner = Runner(args.mode, host=args.host, port=args.port)
     # Initialize the database and run the app
     app_runner.initialize_database()
+    if args.backup:
+        app_runner.backup_database()
     app_runner.run()
     app_runner.open_browser(delay=1)
     # Wait for the exit command to stop
     app_runner.wait_for_exit()
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("--host", help="The host address where the app will be run.")
     parser.add_argument("--port", help="The port where the app will be accessible.")
     parser.add_argument(
+        "--backup",
+        action="store_true",
+        help="A flag indicating if the database should be backed up.",
+    )
+    parser.add_argument(
         "mode",
         help="The runtime mode for the app; defaults to `development`.",
         choices=["development", "production"],
     )
     return parser.parse_args()
 
 
@@ -44,28 +51,33 @@
     """A tool to build and execute Flask commands."""
 
     _exit = Event()
 
     def __init__(self, mode, host=None, port=None):
         self.mode = mode
         self.host = host
-        self.port = port
+        self.port = port if port else "5000"
 
     @property
     def command(self):
         _command = ["flask"]
         if self.mode == "development":
             _command.append("--debug")
         return _command
 
     def initialize_database(self):
         """Run the database initializer."""
         instruction = self.command + ["init-db"]
         subprocess.run(instruction)
 
+    def backup_database(self):
+        """Back up the app database."""
+        instruction = self.command + ["back-up-db"]
+        subprocess.run(instruction)
+
     def run(self):
         """Run the Monopyly application."""
         instruction = self.command + ["run"]
         if self.host:
             instruction += ["--host", self.host]
         if self.port:
             instruction += ["--port", self.port]
```

### Comparing `monopyly-1.2.3/monopyly/common/utils.py` & `monopyly-1.3.0/monopyly/common/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/common/forms/fields.py` & `monopyly-1.3.0/monopyly/common/forms/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class StringField(wtforms_fields.StringField):
     """A custom string field."""
 
     def __init__(self, *args, filters=(), **kwargs):
         filters = list(filters)
-        filters.append(lambda x: x.strip() if x else "")
+        filters.append(lambda x: x.strip() if x else None)
         super().__init__(*args, filters=filters, **kwargs)
 
 
 class LastFourDigitsField(StringField):
     """A custom field for collecting the last four digits of cards/accounts."""
 
     def __init__(self, *args, validators=(), **kwargs):
```

### Comparing `monopyly-1.2.3/monopyly/common/forms/utils.py` & `monopyly-1.3.0/monopyly/common/forms/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,47 +25,52 @@
         A mapping between fields supporting autocompletion and the model
         object that is used to access that field.
     """
 
     def __init__(self, field_map):
         self._field_map = field_map
 
-    def autocomplete(self, field, **priority_sort_fields):
+    def autocomplete(self, field, db_field_name=None, **priority_sort_fields):
         """
         Provide autocomplete suggestions for the field.
 
         Given a form field name (which should match a database field),
         get potential entries that should be suggested as autocompletion
         options. Sort the suggestions by their frequency and return
         them.
 
         Parameters
         ----------
         field : str
             The name of the form field for which to provide
             autocompletion.
+        db_field_name : str, None
+            The name of the database field mapping to the form field;
+            the default is `None` where the form field name will be
+            used.
         priority_sort_field : dict
             A mapping of fields and a value of that field which will
             take precedence over a suggestion's frequency in the data
             when sorting the suggestions. The fields should be provided
             in order of increasing importance.
 
         Returns
         -------
         suggestions : list of str
             A list of autocompletion suggestions that are sorted by
             their frequency of appearance in the database.
         """
+        db_field_name = db_field_name if db_field_name else field
         model = self._field_map[field]
-        suggestions = self._get_autocomplete_suggestions(model, field)
+        suggestions = self._get_autocomplete_suggestions(model, db_field_name)
         for sort_field, precedence_value in priority_sort_fields.items():
             self._sort_suggestions_by_field(
                 suggestions, model, field, sort_field, precedence_value
             )
-        return suggestions
+        return list(filter(None, suggestions))
 
     @staticmethod
     def _get_autocomplete_suggestions(model, field):
         """Get autocomplete suggestions for a field."""
         # Get information from the database to use for autocompletion
         query = model.select_for_user(getattr(model, field))
         values = current_app.db.session.execute(query).scalars()
```

### Comparing `monopyly-1.2.3/monopyly/common/forms/validators.py` & `monopyly-1.3.0/monopyly/common/forms/validators.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/config/settings.py` & `monopyly-1.3.0/monopyly/config/settings.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/core/context_processors.py` & `monopyly-1.3.0/monopyly/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/core/filters.py` & `monopyly-1.3.0/monopyly/core/filters.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/credit/accounts.py` & `monopyly-1.3.0/monopyly/credit/accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tools for interacting with credit accounts in the database.
 """
-from ..database.handler import DatabaseHandler
+from authanor.database.handler import DatabaseHandler
+
 from ..database.models import CreditAccount
 
 
 class CreditAccountHandler(DatabaseHandler, model=CreditAccount):
     """
     A database handler for managing credit accounts.
 
@@ -35,18 +36,17 @@
             (if `None`, all banks will be selected).
 
         Returns
         -------
         accounts : sqlalchemy.engine.ScalarResult
             Returns credit accounts matching the criteria.
         """
-        criteria = [
-            cls._filter_values(cls.model.bank_id, bank_ids),
-        ]
-        accounts = super().get_entries(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(cls.model, "bank_id", bank_ids)
+        accounts = super().get_entries(criteria=criteria)
         return accounts
 
     @classmethod
     def delete_entry(cls, entry_id):
         """
         Delete a credit card account from the database.
```

### Comparing `monopyly-1.2.3/monopyly/credit/actions.py` & `monopyly-1.3.0/monopyly/credit/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,20 +111,25 @@
         card,
         payment_date,
         creation=True,
     )
     # Add the payment as a transaction in the database
     if payment_account_id:
         # Populate a mapping for the transfer
-        payment_note = f"Credit card payment ({payee}-{card.last_four_digits})"
+        payment_note = f"Credit card payment ({payee} – {card.last_four_digits})"
         bank_mapping = {
             "account_id": payment_account_id,
+            "merchant": payee,
             "transaction_date": payment_date,
             "subtransactions": [
-                {"subtotal": -payment_amount, "note": payment_note},
+                {
+                    "subtotal": -payment_amount,
+                    "note": payment_note,
+                    "tags": ["Credit payments"],
+                }
             ],
         }
         transfer = record_new_transfer(bank_mapping)
         internal_transaction_id = transfer.internal_transaction_id
     else:
         internal_transaction_id = None
     credit_mapping = {
@@ -132,12 +137,12 @@
         "statement_id": payment_statement.id,
         "transaction_date": payment_date,
         "merchant": payee,
         "subtransactions": [
             {
                 "subtotal": -payment_amount,
                 "note": "Card payment",
-                "tags": ["Payments"],
+                "tags": ["Credit payments"],
             }
         ],
     }
     CreditTransactionHandler.add_entry(**credit_mapping)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `monopyly-1.2.3/monopyly/credit/cards.py` & `monopyly-1.3.0/monopyly/credit/cards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tools for interacting with credit cards in the database.
 """
+from authanor.database.handler import DatabaseHandler
+
 from ..common.forms.utils import execute_on_form_validation
-from ..database.handler import DatabaseHandler
 from ..database.models import Bank, CreditAccount, CreditCard
 
 
 class CreditCardHandler(DatabaseHandler, model=CreditCard):
     """
     A database handler for managing credit cards.
 
@@ -50,21 +51,20 @@
             returned regardless of the card's active status.
 
         Returns
         -------
         cards : sqlalchemy.engine.ScalarResult
             Returns credit cards matching the criteria.
         """
-        criteria = [
-            cls._filter_values(CreditAccount.bank_id, bank_ids),
-            cls._filter_values(cls.model.account_id, account_ids),
-            cls._filter_values(cls.model.last_four_digits, last_four_digits),
-            cls._filter_value(cls.model.active, active),
-        ]
-        cards = super().get_entries(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(CreditAccount, "bank_id", bank_ids)
+        criteria.add_match_filter(cls.model, "account_id", account_ids)
+        criteria.add_match_filter(cls.model, "last_four_digits", last_four_digits)
+        criteria.add_match_filter(cls.model, "active", active)
+        cards = super().get_entries(criteria=criteria)
         return cards
 
     @classmethod
     def find_card(cls, bank_name=None, last_four_digits=None):
         """
         Find a credit card using uniquely identifying characteristics.
 
@@ -87,19 +87,18 @@
 
         Returns
         -------
         card : sqlite3.Row
             A credit card entry matching the given criteria. If no
             matching card is found, returns `None`.
         """
-        criteria = [
-            cls._filter_value(Bank.bank_name, bank_name),
-            cls._filter_value(cls.model.last_four_digits, last_four_digits),
-        ]
-        card = super().find_entry(*criteria)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(Bank, "bank_name", bank_name)
+        criteria.add_match_filter(cls.model, "last_four_digits", last_four_digits)
+        card = super().find_entry(criteria=criteria)
         return card
 
     @classmethod
     def _customize_entries_query(cls, query, filters, sort_order):
         query = super()._customize_entries_query(query, filters, sort_order)
         # Order cards by active status (active cards first)
         query = query.order_by(cls.model.active.desc())
```

### Comparing `monopyly-1.2.3/monopyly/credit/forms.py` & `monopyly-1.3.0/monopyly/credit/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ..database.models import (
     Bank,
     CreditAccount,
     CreditCard,
     CreditStatementView,
     CreditSubtransaction,
     CreditTransactionView,
+    TransactionTag,
 )
 from .accounts import CreditAccountHandler
 from .cards import CreditCardHandler
 from .statements import CreditStatementHandler
 
 
 class CreditAccountSelectField(CustomChoiceSelectField):
@@ -248,39 +249,15 @@
             # Prepare data for the card subforms
             data["card_info"] = self.card_info.gather_entry_data(card_info)
             return data
 
     class SubtransactionSubform(TransactionForm.SubtransactionSubform):
         """Form to input/edit credit card subtransactions."""
 
-        # Fields pertaining to the credit subtransaction
-        tags = StringField("Tags")
-
-        @property
-        def subtransaction_data(self):
-            """
-            Produce a dictionary corresponding to a database subtransaction.
-            """
-            raw_tag_data = self.tags.data.split(",")
-            data = super().subtransaction_data
-            data["tags"] = [tag.strip() for tag in raw_tag_data if tag]
-            return data
-
-        def gather_entry_data(self, entry):
-            """Gather data for the form from the given database entry."""
-            if isinstance(entry, CreditSubtransaction):
-                tag_names = [tag.tag_name for tag in entry.tags]
-                data = {
-                    "subtotal": entry.subtotal,
-                    "note": entry.note,
-                    "tags": ", ".join(tag_names),
-                }
-            else:
-                self._raise_gather_fail_error((CreditSubtransaction,), entry)
-            return data
+        subtransaction_model = CreditSubtransaction
 
     # Fields to identify the statement information for the transaction
     statement_info = FormField(StatementSubform)
     # Fields pertaining to the credit transaction
     merchant = StringField("Merchant", [DataRequired()])
     # Subtransaction fields (must be at least 1 subtransaction)
     subtransactions = FieldList(
@@ -290,14 +267,15 @@
     # Define an autocompleter for the form
     _autocompleter = Autocompleter(
         {
             "bank_name": Bank,
             "last_four_digits": CreditCard,
             "merchant": CreditTransactionView,
             "note": CreditSubtransaction,
+            "tags": TransactionTag,
         }
     )
 
     @property
     def transaction_data(self):
         """
         Produce a dictionary corresponding to a database transaction.
@@ -314,15 +292,14 @@
     def get_transaction_statement(self):
         """Get the credit card statement associated with the transaction."""
         return self.statement_info.get_statement(self.transaction_date.data)
 
     def _prepare_transaction_data(self, statement):
         data = super()._prepare_transaction_data()
         data["statement_id"] = statement.id
-        data["merchant"] = self.merchant.data
         return data
 
     def gather_entry_data(self, entry):
         """Gather data for the form from the given database entry."""
         if isinstance(entry, CreditTransactionView):
             data = self._gather_transaction_data(entry)
             statement_info = entry.statement
@@ -330,13 +307,7 @@
             data = {}
             statement_info = entry
         else:
             self._raise_gather_fail_error((CreditCard, CreditStatementView), entry)
         # Prepare data for the statement/subtransaction subforms
         data["statement_info"] = self.statement_info.gather_entry_data(statement_info)
         return data
-
-    def _gather_transaction_data(self, transaction):
-        """Gather credit transaction-specific data."""
-        data = super()._gather_transaction_data(transaction)
-        data["merchant"] = transaction.merchant
-        return data
```

### Comparing `monopyly-1.2.3/monopyly/credit/routes.py` & `monopyly-1.3.0/monopyly/credit/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
     # Add a new subtransaction to the form
     new_subform = extend_field_list_for_ajax(
         CreditTransactionForm,
         "subtransactions",
         subtransaction_count,
     )
     return render_template(
-        "credit/transaction_form/subtransaction_form.html",
+        "common/transaction_form/subtransaction_subform.html",
         subform=new_subform,
         field_list_optional_member=True,
     )
 
 
 @bp.route("/delete_transaction/<int:transaction_id>")
 @login_required
@@ -446,19 +446,23 @@
 
 @bp.route("/_suggest_transaction_autocomplete", methods=("POST",))
 @login_required
 def suggest_transaction_autocomplete():
     # Get the autocomplete field from the AJAX request
     post_args = request.get_json()
     field = post_args["field"]
-    if field != "note":
-        suggestions = CreditTransactionForm.autocomplete(field)
-    else:
+    if field == "note":
         merchant = post_args["merchant"]
         suggestions = CreditTransactionForm.autocomplete("note", merchant=merchant)
+    elif field == "tags":
+        suggestions = CreditTransactionForm.autocomplete(
+            "tags", db_field_name="tag_name"
+        )
+    else:
+        suggestions = CreditTransactionForm.autocomplete(field)
     return jsonify(suggestions)
 
 
 @bp.route("/_infer_card", methods=("POST",))
 @login_required
 def infer_card():
     # Separate the arguments of the POST method
```

### Comparing `monopyly-1.2.3/monopyly/credit/statements.py` & `monopyly-1.3.0/monopyly/credit/statements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tools for interacting with the credit statements in the database.
 """
+from authanor.database.handler import DatabaseViewHandler
+
 from ..common.utils import get_next_occurrence_of_day
-from ..database.handler import DatabaseViewHandler
 from ..database.models import (
     CreditAccount,
     CreditCard,
     CreditStatement,
     CreditStatementView,
 )
 
@@ -58,20 +59,22 @@
             order. The default is descending order.
 
         Returns
         -------
         statements : sqlalchemy.engine.ScalarResult
             Returns credit card statements matching the criteria.
         """
-        criteria = [
-            cls._filter_values(cls.model.card_id, card_ids),
-            cls._filter_values(CreditAccount.bank_id, bank_ids),
-            cls._filter_value(CreditCard.active, active),
-        ]
-        statements = super().get_entries(*criteria, sort_order=sort_order)
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(cls.model, "card_id", card_ids)
+        criteria.add_match_filter(CreditAccount, "bank_id", bank_ids)
+        criteria.add_match_filter(CreditCard, "active", active)
+        statements = super().get_entries(
+            criteria=criteria,
+            column_orders={cls.model.issue_date: sort_order, CreditCard.active: "DESC"},
+        )
         return statements
 
     @classmethod
     @DatabaseViewHandler.view_query
     def find_statement(cls, card_id, issue_date=None):
         """
         Find a statement using uniquely identifying characteristics.
@@ -92,35 +95,25 @@
 
         Returns
         -------
         statement : database.models.CreditStatementView
             The statement entry matching the given criteria. If no
             matching statement is found, returns `None`.
         """
-        criteria = [
-            cls._filter_value(CreditCard.id, card_id),
-            cls._filter_value(cls.model.issue_date, issue_date),
-        ]
+        criteria = cls._initialize_criteria_list()
+        criteria.add_match_filter(CreditCard, "id", card_id)
+        criteria.add_match_filter(cls.model, "issue_date", issue_date)
         statement = super().find_entry(
-            *criteria, sort_order="DESC", require_unique=False
+            criteria=criteria,
+            column_orders={cls.model.issue_date: "DESC", CreditCard.active: "DESC"},
+            require_unique=False,
         )
         return statement
 
     @classmethod
-    def _customize_entries_query(cls, query, filters, sort_order):
-        query = super()._customize_entries_query(query, filters, sort_order)
-        # Order by statement issue date
-        query = cls._sort_query(
-            query,
-            (cls.model.issue_date, sort_order),
-            (CreditCard.active, "DESC"),
-        )
-        return query
-
-    @classmethod
     def infer_statement(cls, card, transaction_date, creation=False):
         """
         Infer the statement corresponding to the date of a transaction.
 
         Given the date of a transaction and the card used, infer the
         statement that the transaction belongs to. If the given card
         issues statements on a date later in the month than the
```

### Comparing `monopyly-1.2.3/monopyly/credit/transactions.py` & `monopyly-1.3.0/monopyly/common/transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,185 +1,216 @@
 """
-Tools for interacting with the credit transactions in the database.
+Tools for building a common transaction interface.
 """
-from ..common.forms.utils import execute_on_form_validation
-from ..common.transactions import TransactionHandler
-from ..database.handler import DatabaseHandler, DatabaseViewHandler
+from abc import abstractmethod
+
+from authanor.database.handler import DatabaseHandler, DatabaseViewHandler
+from flask import current_app
+
 from ..database.models import (
-    Bank,
-    CreditAccount,
-    CreditCard,
-    CreditStatementView,
-    CreditSubtransaction,
-    CreditTag,
-    CreditTransaction,
+    BankAccountTypeView,
+    BankTransactionView,
     CreditTransactionView,
-    tag_link_table,
+    TransactionTag,
 )
 
 
-class CreditTransactionHandler(
-    TransactionHandler, model=CreditTransaction, model_view=CreditTransactionView
-):
+class TransactionHandler(DatabaseViewHandler):
     """
-    A database handler for accessing credit transactions.
+    An abstract database handler for accessing transactions.
 
     Attributes
     ----------
     user_id : int
         The ID of the user who is the subject of database access.
     model : type
         The type of database model that the handler is primarily
         designed to manage.
     table : str
         The name of the database table that this handler manages.
     """
 
     @classmethod
-    @DatabaseViewHandler.view_query
-    def get_transactions(
-        cls, statement_ids=None, card_ids=None, active=None, sort_order="DESC"
-    ):
-        """
-        Get credit card transactions from the database.
-
-        Query the database to select credit card transaction information.
-        Transaction information includes details specific to the
-        transaction, the transaction's statement, and the credit card
-        used to make the transaction. Transactions can be filtered by
-        statement or the credit card used. Query results can be ordered
-        by either ascending or descending transaction date.
-
-        Parameters
-        ----------
-        statement_ids : tuple of str, optional
-            A sequence of statement IDs with which to filter
-            transactions (if `None`, all statement IDs will be shown).
-        card_ids : tuple of int, optional
-            A sequence of card IDs with which to filter transactions (if
-            `None`, all card IDs will be shown).
-        active : bool, optional
-            A flag indicating whether only transactions for active cards
-            will be returned. The default is `None` (all transactions
-            are returned).
-        sort_order : {'ASC', 'DESC'}
-            An indicator of whether the transactions should be ordered
-            in ascending (oldest at top) or descending (newest at top)
-            order.
+    def _customize_entries_query(cls, query, criteria, column_orders):
+        # Group transactions and order by transaction date
+        query = query.group_by(cls.model.id)
+        return super()._customize_entries_query(query, criteria, column_orders)
 
-        Returns
-        -------
-        transactions : sqlalchemy.engine.ScalarResult
-            Returns credit card transactions matching the criteria.
-        """
-        criteria = [
-            cls._filter_values(cls.model.statement_id, statement_ids),
-            cls._filter_values(CreditCard.id, card_ids),
-            cls._filter_value(CreditCard.active, active),
-        ]
-        transactions = super().get_entries(*criteria, sort_order=sort_order)
-        return transactions
+    @classmethod
+    def _get_transactions(cls, criteria=None, sort_order="DESC"):
+        # Specify transaction order
+        column_orders = {cls.model.transaction_date: sort_order}
+        entries = cls.get_entries(
+            entry_ids=None, criteria=criteria, column_orders=column_orders
+        )
+        return entries
 
     @classmethod
     def add_entry(cls, **field_values):
         """
         Add a transaction to the database.
 
-        Uses values acquired from a `CreditTransactionForm` to add a new
+        Uses values acquired from a `TransactionForm` to add a new
         transaction into the database. The values include information
         for the transaction, along with information for all
-        subtransactions (including tags associated with each
-        subtransaction).
+        subtransactions.
 
         Parameters
         ----------
         **field_values :
             Values for each field in the transaction (including
-            subtransaction values and tags).
+            subtransaction values).
 
         Returns
         -------
-        transaction : database.models.CreditTransaction
+        transaction : database.models.BankTransaction
             The saved transaction.
         """
-        return super().add_entry(**field_values)
+        # Extend the default method to account for subtransactions
+        subtransactions_data = field_values.pop("subtransactions")
+        transaction = super().add_entry(**field_values)
+        cls._add_subtransactions(transaction, subtransactions_data)
+        # Refresh the transaction with the subtransaction information
+        cls._db.session.refresh(transaction)
+        return transaction
+
+    @classmethod
+    def update_entry(cls, entry_id, **field_values):
+        """Update a transaction in the database."""
+        # Extend the default method to account for subtransactions
+        subtransactions_data = field_values.pop("subtransactions", None)
+        transaction = super().update_entry(entry_id, **field_values)
+        if subtransactions_data:
+            # Replace all subtransactions when updating any subtransaction
+            for subtransaction in transaction.subtransactions:
+                cls._db.session.delete(subtransaction)
+            cls._add_subtransactions(transaction, subtransactions_data)
+        # Refresh the transaction with the subtransaction information
+        cls._db.session.refresh(transaction)
+        return transaction
+
+    @classmethod
+    def _add_subtransactions(cls, transaction, subtransactions_data):
+        """Add subtransactions to the database for the data given."""
+        for subtransaction_data in subtransactions_data:
+            subtransaction = cls._prepare_subtransaction(
+                transaction, subtransaction_data
+            )
+            cls._db.session.add(subtransaction)
+        # Flush to the database after all subtransactions have been added
+        cls._db.session.flush()
+
+
+def get_linked_transaction(transaction):
+    """
+    Find a transaction that is linked to the given transaction.
+
+    Checks all transaction databases for a transaction that matches
+    the given transaction.
+
+    Parameters
+    ----------
+    transaction : Transaction
+        The transaction for which to find a linked transaction.
 
-    @staticmethod
-    def _prepare_subtransaction(transaction, subtransaction_data):
-        """Prepare a subtransaction for the given transaction."""
-        # NOTE I don't believe that this adds new tags to the database
-        tag_names = subtransaction_data.pop("tags")
-        return CreditSubtransaction(
-            transaction_id=transaction.id,
-            **subtransaction_data,
-            tags=CreditTagHandler.get_tags(tag_names, ancestors=True),
+    Returns
+    -------
+    linked_transaction : Transaction
+        A transaction that is linked to the given transaction. If no
+        linked transaction is found, `None` is returned.
+    """
+    internal_transaction_id = transaction.internal_transaction_id
+    if not internal_transaction_id:
+        return None
+    # First, check if there is a matching bank transaction
+    linked_transaction = _get_linked_bank_transaction(
+        transaction.id, internal_transaction_id
+    )
+    if not linked_transaction:
+        # Otherwise, check if there is a matching credit transaction
+        linked_transaction = _get_linked_credit_transaction(
+            transaction.id, internal_transaction_id
         )
+    return linked_transaction
+
+
+def _get_linked_bank_transaction(transaction_id, internal_transaction_id):
+    """Get a bank transaction linked to the given transaction."""
+    query = BankTransactionView.select_for_user().join(BankAccountTypeView)
+    criteria = [
+        BankTransactionView.id != transaction_id,
+        BankTransactionView.internal_transaction_id == internal_transaction_id,
+    ]
+    query = query.where(*criteria)
+    transaction = current_app.db.session.execute(query).scalar_one_or_none()
+    return transaction
 
 
-class CreditTagHandler(DatabaseHandler, model=CreditTag):
+def _get_linked_credit_transaction(transaction_id, internal_transaction_id):
+    """Get a credit transaction linked to the given transaction."""
+    query = CreditTransactionView.select_for_user()
+    criteria = [
+        CreditTransactionView.id != transaction_id,
+        CreditTransactionView.internal_transaction_id == internal_transaction_id,
+    ]
+    query = query.where(*criteria)
+    transaction = current_app.db.session.execute(query).scalar_one_or_none()
+    return transaction
+
+
+class TransactionTagHandler(DatabaseHandler, model=TransactionTag):
     """
-    A database handler for managing credit transaction tags.
+    A database handler for managing transaction tags.
 
     Attributes
     ----------
     user_id : int
         The ID of the user who is the subject of database access.
     model : type
         The type of database model that the handler is primarily
         designed to manage.
     table : str
         The name of the database table that this handler manages.
     """
 
     @classmethod
-    def get_tags(
+    def _get_tags(
         cls,
+        criteria,
         tag_names=None,
         transaction_ids=None,
         subtransaction_ids=None,
         ancestors=None,
     ):
         """
-        Get credit card transaction tags from the database.
+        Get transaction tags from the database.
 
-        Query the database to select credit transaction tag fields. Tags
-        can be filtered by tag name or transaction.
+        Query the database to select transaction tag fields. Tags can
+        be filtered by tag name or transaction.
 
         Parameters
         ----------
-        tag_names : tuple of str, optional
-            A sequence of names of tags to be selected (if `None`, all
-            tag names will be selected).
-        transaction_ids : tuple of int, optional
-            A sequence of transaction IDs for which tags will be
-            selected (if `None`, all transaction tags will be selected).
-        subtransaction_ids : tuple of int, optional
-            A sequence of subtransaction IDs for which tags will be
-            selected (if `None`, all subtransaction tags will be selected).
+        criteria : database.handler.QueryCriteria
+            Criteria used to select tags from the database.
         ancestors : bool, optional
             A flag indicating whether the query should include tags
             that are the ancestor tags of other explictly selected tags
             returned from the database based on selection criteria. If
             `True`, all tags matching the criteria will be returned
             along with their ancestor tags. If `False`, any tag that is
             an ancestor of another tag in the list will be removed from
             the list. The default is `None`, in which case all tags
             matching the criteria will be returned, and no others.
 
         Returns
         -------
-        tags : list of database.models.CreditTag
-            Returns credit card transaction tags matching the criteria.
+        tags : list of database.models.TransactionTag
+            Returns transaction tags matching the criteria.
         """
-        criteria = [
-            cls._filter_values(cls.model.tag_name, tag_names),
-            cls._filter_values(CreditTransactionView.id, transaction_ids),
-            cls._filter_values(CreditSubtransaction.id, subtransaction_ids),
-        ]
-        tags = super().get_entries(*criteria).all()
+        tags = super().get_entries(criteria=criteria).all()
         if ancestors is True:
             # Add all ancestors for each tag in the list
             for tag in tags:
                 for ancestor in cls.get_ancestors(tag):
                     if ancestor not in tags:
                         tags.append(ancestor)
         elif ancestors is False:
@@ -187,68 +218,58 @@
             for tag in tags:
                 for ancestor in cls.get_ancestors(tag):
                     if ancestor in tags:
                         tags.remove(ancestor)
         return tags
 
     @classmethod
-    def _filter_entries(cls, query, filters):
-        # Add a join to enable filtering by transaction ID or subtransaction ID
-        query = (
-            query.join(tag_link_table)
-            .join(CreditSubtransaction)
-            .join(CreditTransactionView)
-            .join(CreditStatementView)
-            .join(CreditCard)
-            .join(CreditAccount)
-            .join(Bank)
-        )
+    def _filter_entries(cls, query, criteria):
         # Only get distinct tag entries
         query = query.distinct()
-        return super()._filter_entries(query, filters)
+        return super()._filter_entries(query, criteria)
 
     @classmethod
     def get_subtags(cls, tag):
         """
-        Get subcategories (children) of a given credit transaction tag.
+        Get subcategories (children) of a given transaction tag.
 
         Parameters
         ----------
-        tag : database.models.CreditTag
+        tag : database.models.TransactionTag
             The parent tag for which to find subtags. (A value of `None`
             indicates that top level tags should be found.)
 
         Returns
         -------
         subtags : sqlalchemy.engine.ScalarResult
-            A list of credit card transaction tags that are
-            subcategories of the given parent tag.
+            A list of transaction tags that are subcategories of the
+            given parent tag.
         """
         query = cls.model.select_for_user()
         # Filter the query to get only subtags of the given tag
         parent_id = tag.id if tag else None
         query = query.where(cls.model.parent_id == parent_id)
         subtags = cls._db.session.execute(query).scalars()
         return subtags
 
     @classmethod
     def get_supertag(cls, tag):
         """
-        Get the supercategory (parent) of a credit transaction tag.
+        Get the supercategory (parent) of a transaction tag.
 
         Parameters
         ----------
         tag_id : int
             The child tag for which to find supertags.
 
         Returns
         -------
-        supertag : database.models.CreditTag
-            The credit card transaction tag that is the parent category
-            of the given tag. Returns `None` if no parent tag is found.
+        supertag : database.models.TransactionTag
+            The transaction tag that is the parent category of the given
+            tag. Returns `None` if no parent tag is found.
         """
         parent_id = tag.parent_id
         supertag = cls.get_entry(parent_id) if parent_id else None
         return supertag
 
     @classmethod
     def get_hierarchy(cls, root_tag=None):
@@ -259,24 +280,24 @@
         representation of the tags. The dictionary has keys representing
         each tag, and each key is paired to a similar dictionary of
         subtags for that tag. The top level of the dictionary consists
         only of tags without root tags.
 
         Parameters
         ----------
-        root_tag : database.models.CreditTag
+        root_tag : database.models.TransactionTag
             The root tag to use as the starting point when recursing
             through the tree. If the parent is `None`, the recursion
             begins at the highest level of tags.
 
         Returns
         -------
         hierarchy : dict
             The dictionary representing the user's tags. Keys are
-            `CreditTag` objects.
+            `TransactionTag` objects.
         """
         hierarchy = {}
         for tag in cls.get_subtags(root_tag):
             hierarchy[tag] = cls.get_hierarchy(tag)
         return hierarchy
 
     @classmethod
@@ -285,20 +306,20 @@
         Get the ancestor tags of a given tag.
 
         Traverses the hierarchy, starting from the given tag and returns
         a list of all tags that are ancestors of the given tag.
 
         Parameters
         ----------
-        tag : database.models.CreditTag
+        tag : database.models.TransactionTag
             The tag for which to find ancestors.
 
         Returns
         -------
-        ancestors : list of database.models.CreditTag
+        ancestors : list of database.models.TransactionTag
             The ancestors of the given tag.
         """
         ancestors = []
         ancestor = cls.get_supertag(tag)
         while ancestor:
             ancestors.append(ancestor)
             ancestor = cls.get_supertag(ancestor)
@@ -315,55 +336,15 @@
         Parameters
         ----------
         tag_name : str
             The name of the tag to be found.
 
         Returns
         -------
-        tag : database.models.CreditTag
+        tag : database.models.TransactionTag
             The tag entry matching the given criteria. If no matching
             tag is found, returns `None`.
         """
         criteria = [cls.model.tag_name == tag_name]
         query = cls.model.select_for_user().where(*criteria)
         tag = cls._db.session.execute(query).scalar_one_or_none()
         return tag
-
-
-@execute_on_form_validation
-def save_transaction(form, transaction_id=None):
-    """
-    Save a credit transaction.
-
-    Saves a transaction in the database. If a transaction ID is given,
-    then the transaction is updated with the form information. Otherwise
-    the form information is added as a new entry.
-
-    Parameters
-    ----------
-    form : CreditTransactionForm
-        The form being used to provide the data being saved.
-    transaction_id : int
-        The ID of the transaction to be saved. If provided, the
-        named transaction will be updated in the database. Otherwise, if
-        the transaction ID is `None`, a new transaction will be added.
-
-    Returns
-    -------
-    transaction : database.models.CreditTransactionView
-        The saved transaction.
-    """
-    transaction_data = form.transaction_data
-    if transaction_id:
-        transaction = CreditTransactionHandler.get_entry(transaction_id)
-        transaction_data.update(
-            internal_transaction_id=transaction.internal_transaction_id
-        )
-        # Update the database with the updated transaction
-        transaction = CreditTransactionHandler.update_entry(
-            transaction_id,
-            **transaction_data,
-        )
-    else:
-        # Insert the new transaction into the database
-        transaction = CreditTransactionHandler.add_entry(**transaction_data)
-    return transaction
```

### Comparing `monopyly-1.2.3/monopyly/database/__init__.py` & `monopyly-1.3.0/monopyly/database/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,57 @@
 """
 Expose commonly used database functionality to the rest of the package.
 """
+import sqlite3
 from functools import wraps
 from pathlib import Path
 
 import click
-from flask import current_app, g
+from authanor.database import SQLAlchemy as _SQLAlchemy
+from flask import current_app
 from flask.cli import with_appcontext
-from sqlalchemy import MetaData, create_engine, event
-from sqlalchemy.engine import Engine
-from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.schema import Table
 
-from .models import Model
-from .schema import DATABASE_SCHEMA
+from ..core.actions import get_timestamp
 
-DIALECT = "sqlite"
-DBAPI = "pysqlite"
 DB_NAME = "monopyly.sqlite"
 
 
-class SQLAlchemy:
-    """Store SQLAlchemy database objects."""
+class SQLAlchemy(_SQLAlchemy):
+    """Store an interface to SQLAlchemy database objects."""
 
-    _base = Model
-
-    def __init__(self, db_path=None):
-        self.engine = None
-        self.metadata = None
-        self.scoped_session = None
-
-    @property
-    def tables(self):
-        return self.metadata.tables
-
-    @property
-    def session(self):
-        # Returns the current `Session` object
-        return self.scoped_session()
-
-    def setup_engine(self, db_path, echo_engine=False):
-        """Setup the database engine, a session factory, and metadata."""
-        # Create the engine using the custom database URL
-        db_url = f"{DIALECT}+{DBAPI}:///{db_path}"
-        self.engine = create_engine(db_url, echo=echo_engine)
-        # Use a session factory to generate sessions
-        session_factory = sessionmaker(
-            bind=self.engine,
-            autoflush=False,
-            future=True,
-        )
-        self.scoped_session = scoped_session(session_factory)
-        self._base.query = self.scoped_session.query_property()
-        # Add metadata
-        self.metadata = MetaData()
-
-    def access_tables(self):
-        for table_name in DATABASE_SCHEMA.keys():
-            Table(table_name, self.metadata, autoload_with=self.engine)
+    def initialize(self, app):
+        """
+        Initialize the database.
+
+        Initialize the database by executing the SQL schema to clear
+        existing data and create new tables.
+
+        Parameters
+        ----------
+        app : flask.Flask
+            The app object, which may pass initialization parameters via
+            its configuration.
+        """
+        with app.app_context():
+            # Establish a raw connection in order to execute the complete files
+            raw_conn = self.engine.raw_connection()
+            # Load the tables, table views, and preloaded data
+            sql_dir = Path(__file__).parent
+            sql_filepaths = [
+                sql_dir / path for path in ("schema.sql", "views.sql", "preloads.sql")
+            ]
+            auxiliary_preload_path = app.config["PRELOAD_DATA_PATH"]
+            if auxiliary_preload_path:
+                sql_filepaths.append(auxiliary_preload_path)
+            for sql_filepath in sql_filepaths:
+                with current_app.open_resource(sql_filepath) as sql_file:
+                    raw_conn.executescript(sql_file.read().decode("utf8"))
+            raw_conn.close()
+        super().initialize(app)
 
 
 db = SQLAlchemy()
 
 
 def db_transaction(func):
     """A decorator denoting the wrapped function as a database transaction."""
@@ -70,52 +60,47 @@
     def wrapper(*args, **kwargs):
         with current_app.db.session.begin():
             return func(*args, **kwargs)
 
     return wrapper
 
 
-@event.listens_for(Engine, "connect")
-def set_sqlite_pragma(dbapi_connection, connection_record):
-    cursor = dbapi_connection.cursor()
-    cursor.execute("PRAGMA foreign_keys=ON")
-    cursor.close()
-
-
 @click.command("init-db")
 @with_appcontext
 def init_db_command():
     """Initialize the database from the command line (if it does not exist)."""
     db_path = current_app.config["DATABASE"]
     if not db_path.is_file():
         preload_path = current_app.config.get("PRELOAD_DATA_PATH")
-        init_db(current_app.db, preload_path)
+        current_app.db.initialize(current_app)
         click.echo(f"Initialized the database ('{db_path}')")
         if preload_path:
             click.echo(f"Prepopulated the database using '{preload_path}'")
     else:
         click.echo(f"Database exists, using '{db_path}'")
 
 
-def init_db(db, auxiliary_preload_path=None):
-    """Execute the SQL schema to clear existing data and create new tables."""
-    # Establish a raw connection in order to execute the complete files
-    raw_conn = db.engine.raw_connection()
-    # Load the tables, table views, and preloaded data
-    sql_dir = Path(__file__).parent
-    sql_filepaths = [
-        sql_dir / path for path in ("schema.sql", "views.sql", "preloads.sql")
-    ]
-    if auxiliary_preload_path:
-        sql_filepaths.append(auxiliary_preload_path)
-    for sql_filepath in sql_filepaths:
-        with current_app.open_resource(sql_filepath) as sql_file:
-            raw_conn.executescript(sql_file.read().decode("utf8"))
-    raw_conn.close()
-    # Register tables with the SQLAlchemy metadata
-    db.metadata.create_all(bind=db.engine)
-
-
-def close_db(exception=None):
-    """Close the database if it is open."""
-    if current_app.db.scoped_session is not None:
-        current_app.db.scoped_session.remove()
+@click.command("back-up-db")
+@with_appcontext
+def back_up_db_command():
+    """Back up the database from the command line."""
+    timestamp = get_timestamp()
+    # Connect to the database
+    db = sqlite3.connect(current_app.config["DATABASE"])
+    # Create and connect to the backup database
+    backup_db_dir_path = Path(current_app.instance_path) / "db_backups"
+    backup_db_dir_path.mkdir(exist_ok=True, parents=True)
+    backup_db_path = backup_db_dir_path / f"backup_{timestamp}.sqlite"
+    backup_db = sqlite3.connect(backup_db_path)
+    # Back up the database and print status
+    back_up_db(db, backup_db)
+    click.echo(f"Backup complete ({timestamp})")
+
+
+def back_up_db(db, backup_db):
+    """Create a backup of the database."""
+    # Backup the database
+    with backup_db:
+        db.backup(backup_db)
+    # Close the connections
+    backup_db.close()
+    db.close()
```

### Comparing `monopyly-1.2.3/monopyly/database/schema.sql` & `monopyly-1.3.0/monopyly/database/schema.sql`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 DROP TABLE IF EXISTS users;
 DROP TABLE IF EXISTS internal_transactions;
+DROP TABLE IF EXISTS transaction_tags;
 DROP TABLE IF EXISTS banks;
 DROP TABLE IF EXISTS bank_accounts;
 DROP TABLE IF EXISTS bank_account_types;
 DROP TABLE IF EXISTS bank_transactions;
 DROP TABLE IF EXISTS bank_subtransactions;
+DROP TABLE IF EXISTS bank_tag_links;
 DROP TABLE IF EXISTS credit_accounts;
 DROP TABLE IF EXISTS credit_cards;
 DROP TABLE IF EXISTS credit_statements;
 DROP TABLE IF EXISTS credit_transactions;
 DROP TABLE IF EXISTS credit_subtransactions;
-DROP TABLE IF EXISTS credit_tags;
 DROP TABLE IF EXISTS credit_tag_links;
 
 
 /* Store user information */
 CREATE TABLE users (
   id INTEGER PRIMARY KEY,
   username TEXT UNIQUE NOT NULL,
   password TEXT NOT NULL
 );
 
 
+/* Store a common link for paired transactions */
+CREATE TABLE internal_transactions (
+  id INTEGER PRIMARY KEY
+);
+
+
+/* Store transaction tags */
+CREATE TABLE transaction_tags (
+  id INTEGER PRIMARY KEY,
+  user_id INTEGER NOT NULL REFERENCES users (id),
+  parent_id INTEGER REFERENCES transaction_tags (id)
+    ON DELETE CASCADE,
+  tag_name TEXT NOT NULL COLLATE NOCASE,
+  UNIQUE(user_id, tag_name)
+);
+
+
 /* Store information about banks */
 CREATE TABLE banks (
   id INTEGER PRIMARY KEY,
   user_id INTEGER NOT NULL REFERENCES users (id),
   bank_name TEXT NOT NULL,
   UNIQUE(user_id, bank_name)
 );
@@ -57,28 +75,39 @@
 
 /* Store bank transaction information */
 CREATE TABLE bank_transactions (
   id INTEGER PRIMARY KEY,
   internal_transaction_id INTEGER DEFAULT NULL REFERENCES internal_transactions (id),
   account_id INTEGER NOT NULL REFERENCES bank_accounts (id)
     ON DELETE CASCADE,
-  transaction_date DATE NOT NULL
+  transaction_date DATE NOT NULL,
+  merchant TEXT
 );
 
 
 /* Store bank subtransaction infromation */
 CREATE TABLE bank_subtransactions (
   id INTEGER PRIMARY KEY,
   transaction_id INTEGER NOT NULL REFERENCES bank_transactions (id)
     ON DELETE CASCADE,
   subtotal REAL NOT NULL,
   note TEXT NOT NULL
 );
 
 
+/* Associate bank transactions with tags in a link table */
+CREATE TABLE bank_tag_links (
+  subtransaction_id INTEGER NOT NULL REFERENCES bank_subtransactions (id)
+    ON DELETE CASCADE,
+  tag_id INTEGER NOT NULL REFERENCES transaction_tags (id)
+    ON DELETE CASCADE,
+  PRIMARY KEY (subtransaction_id, tag_id)
+);
+
+
 /* Store credit account information */
 CREATE TABLE credit_accounts (
   id INTEGER PRIMARY KEY,
   bank_id INTEGER NOT NULL REFERENCES banks (id)
     ON DELETE CASCADE,
   statement_issue_day INTEGER NOT NULL
     CHECK(statement_issue_day > 0 AND statement_issue_day < 28),
@@ -125,33 +154,16 @@
   transaction_id INTEGER NOT NULL REFERENCES credit_transactions (id)
     ON DELETE CASCADE,
   subtotal REAL NOT NULL,
   note TEXT NOT NULL
 );
 
 
-/* Store credit card transaction tags */
-CREATE TABLE credit_tags (
-  id INTEGER PRIMARY KEY,
-  user_id INTEGER NOT NULL REFERENCES users (id),
-  parent_id INTEGER REFERENCES credit_tags (id)
-    ON DELETE CASCADE,
-  tag_name TEXT NOT NULL COLLATE NOCASE,
-  UNIQUE(user_id, tag_name)
-);
-
-
 /* Associate credit transactions with tags in a link table */
 CREATE TABLE credit_tag_links (
   subtransaction_id INTEGER NOT NULL REFERENCES credit_subtransactions (id)
     ON DELETE CASCADE,
-  tag_id INTEGER NOT NULL REFERENCES credit_tags (id)
+  tag_id INTEGER NOT NULL REFERENCES transaction_tags (id)
     ON DELETE CASCADE,
   PRIMARY KEY (subtransaction_id, tag_id)
 );
 
-
-/* Store a common link for paired transactions */
-CREATE TABLE internal_transactions (
-  id INTEGER PRIMARY KEY
-);
-
```

### Comparing `monopyly-1.2.3/monopyly/database/views.sql` & `monopyly-1.3.0/monopyly/database/views.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/jquery-3.4.1.js` & `monopyly-1.3.0/monopyly/static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/css/style.css` & `monopyly-1.3.0/monopyly/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 /*-------------------------------------------*/
 /*     Style sheet for the Monopyly app      */
 /*-------------------------------------------*/
 
+
+/* Define custom colors for consistent branding */
+:root {
+  --moneytree: #5e8f40;
+  --moneytree-leaves: #85bb65;
+}
+
 html {
   height: 100%;
 }
 
 body {
   display: flex;
   flex-direction: column;
@@ -14,24 +21,24 @@
   margin: 0;
   padding: 0;
   color: #444444;
   font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
 }
 
 a {
-  color: #5e8f40;
+  color: var(--moneytree);
   text-decoration: none;
 }
 
 a:hover {
   text-decoration: underline;
 }
 
 a:focus {
-  color: #85bb65;
+  color: var(--moneytree-leaves);
   outline: none;
 }
 
 form {
   width: 50%;
   margin: auto;
 }
@@ -39,42 +46,53 @@
 input {
   color: inherit;
   font-size: inherit;
   font-family: inherit;
 }
 
 input:focus-visible {
-  outline: #85bb65 solid medium;
+  outline: var(--moneytree-leaves) solid medium;
 }
 
 input[type="text"],
 select {
   box-sizing: border-box;
   color: inherit;
 }
 
 ::selection {
   background-color: #dfdfdf;
 }
 
+code {
+  display: inline-block;
+  width: 100%;
+  box-sizing: border-box;
+  margin: 5px 0;
+  padding: 10px 20px;
+  background-color: #f5f5f5;
+  border: 1px solid #eeeeee;
+  border-radius: 3px;
+}
+
 
 /*
  * Create dark grey header with a white logo
  */
 header#masthead {
   position: fixed;
   top: 0;
   z-index: 99;
   display: flex;
   align-items: center;
   height: 50px;
   width: 100%;
   border-width: 0 0 4px 3px;
   border-style: solid;
-  border-color: #85bb65;
+  border-color: var(--moneytree-leaves);
   background-color: #2b2b2b;
   opacity: 0.9;
 }
 
 #masthead a {
   text-decoration: none;
 }
@@ -117,14 +135,22 @@
   color: #bbbbbb;
 }
 
 #nav-menu li a:hover {
   color: #cdcdcd;
 }
 
+#nav-menu li .username {
+  color: #777;
+}
+
+#nav-menu li .username:hover {
+  color: var(--moneytree-leaves);
+}
+
 
 /*
  * Create a footer with site information
  */
 footer#site-info {
   margin-top: auto;
 }
@@ -215,22 +241,28 @@
   text-decoration: none;
 }
 
 .button-block:focus {
   color: inherit;
 }
 
+.screenshot {
+  width: 100%; /* override the markdown default */
+  border: 1px solid #f3f3f3;
+  box-shadow: 3px 3px 2px #fafafa;
+}
+
 .grouping {
   border-radius: 15px;
   box-shadow: 0 0 20px #eeeeee;
   background-color: #eef5eb;
 }
 
 .paid-notice {
-  color: #85bb65;
+  color: var(--moneytree-leaves);
   font-weight: bold;
   letter-spacing: 1px;
 }
 
 .card-background {
   width: 100%;
 }
@@ -458,15 +490,15 @@
 }
 
 form .autocomplete-box .item:hover {
   background-color: #cccccc;
 }
 
 form .autocomplete-box .item.active {
-  background-color: #85bb65;
+  background-color: var(--moneytree-leaves);
   color: black;
   font-weight: bold;
 }
 
 
 /*
  * Style the sidebar menus
@@ -536,27 +568,22 @@
   margin: 3px auto;
 }
 
 
 /*
  * Style the widget for performing "live" database updates
  */
-.update-db-widget {
-  display: flex;
-  align-items: center;
-}
-
 .update-db-widget .widget-text {
   position: relative;
   font-size: inherit;
   font-weight: inherit;
 }
 
 .update-db-widget .widget-display {
-  padding: 0 5px;
+  padding: 0 6px;
   font-size: inherit;
   font-weight: inherit;
 }
 
 .update-db-widget .widget-input {
   position: absolute;
   top: 0;
@@ -564,23 +591,32 @@
   width: 100%;
   margin-top: -1px;
   padding: 0 4px;
   font-size: inherit;
   font-weight: inherit;
 }
 
-.update-db-widget .widget-edit-button {
+
+/*
+ * Style the "right-hover-style" version of the update widget
+ */
+.update-db-widget.right-hover-style {
+  display: flex;
+  align-items: center;
+}
+
+.update-db-widget.right-hover-style .widget-edit-button {
   height: 20px;
   width: 20px;
   margin-left: 5px;
   cursor: pointer;
   visibility: hidden;
 }
 
-.update-db-widget:hover .widget-edit-button {
+.update-db-widget.right-hover-style:hover .widget-edit-button {
   visibility: visible;
 }
 
 
 /*
  * Style the gadget to reveal text (sideways slide) on hover
  */
@@ -703,28 +739,60 @@
   box-sizing: border-box;
   border-radius: 50%;
   background-color: #eeeeee;
   transition: inherit;
 }
 
 .toggle-switch-gadget input:checked + .option .text {
-  color: #85bb65;
+  color: var(--moneytree-leaves);
   filter: none;
 }
 
 .toggle-switch-gadget input:checked + .option .slider {
-  background-color: #85bb65;
+  background-color: var(--moneytree-leaves);
 }
 
 .toggle-switch-gadget input:checked + .option .slider .switch {
   margin-left: 50%;
 }
 
 
 /*
+ * Style generic box tables
+ */
+.box-table {
+  border: 2px solid #dddddd;
+}
+
+.box-table .icon-button {
+  display: inline-block;
+  height: 25px;
+  width: 25px;
+  margin: 0 5px;
+  background-size: 25px;
+  filter: brightness(0.8);
+}
+
+.box-table .icon-button:hover {
+  filter: none;
+}
+
+.box-table .box-row {
+  border-top: 0.5px solid #dddddd;
+  border-bottom: 0.5px solid #dddddd;
+  background-color: #f5f5f5;
+}
+
+.box-table .box-row:hover {
+  cursor: pointer;
+  filter: brightness(0.98);
+}
+
+
+/*
  * Style the card filter
  */
 #card-filter {
   display: flex;
   justify-content: center;
   margin-bottom: 20px;
 }
@@ -893,15 +961,15 @@
 
 .transaction .description-header {
   display: flex;
   justify-content: space-between;
   align-items: flex-end;
   padding-bottom: 5px;
   margin-bottom: 10px;
-  border-bottom: 2px solid #85bb65;
+  border-bottom: 2px solid var(--moneytree-leaves);
   color: #444444;
   font-size: 24pt;
 }
 
 .transaction .description-header .total {
   flex: 1;
   text-align: right;
@@ -1376,14 +1444,15 @@
 
 .transactions-table .transaction .expanded .payment .card-number {
   position: absolute;
   top: 70%;
   left: 0;
   width: 100%;
   text-align: center;
+  color: #999999;
   font-size: 1.5em;
   transition: font-size 0.3s;
 }
 @media screen and (max-width: 1500px) {
   /* Size downshift */
   .transactions-table .transaction .expanded .payment .card-number {
     font-size: 1.2em;
@@ -1448,15 +1517,15 @@
   flex-direction: column;
   width: 100%;
   margin: 30px 0;
   padding: 20px 40px;
 }
 
 #linked-transaction-display .linked-transaction.selected {
-  border: 5px solid #85bb65;
+  border: 5px solid var(--moneytree-leaves);
 }
 
 #linked-transaction-display .linked-transaction .date {
   margin-bottom: 20px;
   color: #888888;
   font-size: 14pt;
   font-weight: bold;
@@ -1790,57 +1859,120 @@
 #bank.panel h2,
 #investments.panel h2 {
   color: #bbbbbb;
 }
 
 
 /*
- * Customization for the 'About' page
+ * Customization for the 'About' page(s)
  */
-#about {
+.about {
   width: 75%;
   margin: auto;
   text-align: justify;
 }
 
-#about .signature {
+#readme #header {
+  margin: 40px 0;
+}
+
+#readme #title {
+  margin: 0;
+  font-size: 32pt;
+  text-align: center;
+}
+
+#readme #tagline {
+  margin: 10px 0 0 0;
+  color: var(--moneytree-leaves);
+  font-size: 16pt;
+  text-align: center;
+}
+
+#readme h2 {
+  margin-top: 50px;
+}
+
+#story .signature {
   margin-bottom: 100px;
   font-weight: bold;
   font-style: oblique;
   text-align: right;
 }
 
 
 /*
+ * Customization for the 'Profile' page
+ */
+#profile h2 {
+  font-size: 24pt;
+}
+
+#profile .username-section {
+  font-size: 24pt;
+}
+
+#profile .username-section .username {
+  color: gray;
+  font-weight: 500;
+  text-align: center;
+}
+
+#profile .profile-sections-container {
+  display: flex;
+  flex-wrap: wrap;
+}
+
+#profile .profile-section {
+  width: 40%;
+  min-width: 300px;
+  margin-right: 10%;
+  margin-bottom: 60px;
+}
+
+#profile .settings.profile-section {
+  flex-basis: 100%;
+  margin-right: 0;
+  padding-bottom: 50px;
+  border-bottom: 0.5px solid #dddddd;
+}
+
+#profile .banking.profile-section .bank-list {
+  width: 90%;
+}
+
+#profile .banking.profile-section .bank-list .bank-block {
+  padding: 10px 30px;
+}
+
+#profile .banking.profile-section .bank-list .bank-block .bank {
+  font-weight: bold;
+}
+
+#profile .banking.profile-section .bank-list .bank-block .expanded {
+  display: none;
+  margin-top: 20px;
+}
+
+/*
  * Customization for the 'Bank Accounts' page
  */
 #bank-container .bank-block {
   margin: 25px 0;
   padding: 30px;
 }
 
 #bank-container .bank-block h3 {
   margin-top: 0;
   padding: 0 30px;
   /*text-align: center;*/
 }
 
-#bank-container .account-blocks {
-  border: 2px solid #dddddd;
-}
-
 #bank-container .account-block {
   padding: 25px 30px;
-  border-top: 0.5px solid #dddddd;
-  border-bottom: 0.5px solid #dddddd;
-  background-color: #f5f5f5;
-}
-
-#bank-container .account-block:hover {
-  filter: brightness(0.98);
 }
 
 #bank-container .account-block .account-info {
   display: flex;
   align-items: center;
   color: inherit;
 }
@@ -1851,25 +1983,16 @@
 }
 
 #bank-container .account-block .expanded {
   display: none;
   margin-top: 20px;
 }
 
-#bank-container .icon-button {
-  display: inline-block;
-  height: 25px;
-  width: 25px;
-  margin: 0 15px;
-  background-size: 25px;
-  filter: brightness(0.8);
-}
-
-#bank-container .icon-button:hover {
-  filter: none;
+#bank-container .box-row .expanded .options {
+  margin: 0 25px;
 }
 
 #bank-account-settings {
   margin: 50px 0 25px;
   padding: 0 25px;
 }
 
@@ -2336,15 +2459,15 @@
 
 
 form#pay #make-payment {
   position: absolute;
   top: 0;
   left: 0;
   background-color: green;
-  background-image: linear-gradient(90deg, #85bb65, #73a457);
+  background-image: linear-gradient(90deg, var(--moneytree-leaves), #73a457);
   color: white;
   transition: 0.1s;
 }
 
 form#pay #make-payment:hover {
   filter: brightness(1.08);
 }
@@ -2448,24 +2571,24 @@
 }
 
 #transaction-tags input.new-tag {
   display: none;
   width: 200px;
   margin: 5px 0;
   padding: 2px 15px;
-  border: 0 solid #85bb65;
+  border: 0 solid var(--moneytree-leaves);
   border-radius: 20px;
   text-align: center;
   outline: none;
   caret-color: #cccccc;
   transition: border 0.1s ease;
 }
 
 #transaction-tags input.new-tag.visible {
-  border: 1.5px solid #85bb65;
+  border: 1.5px solid var(--moneytree-leaves);
 }
 
 #transaction-tags .tag {
   z-index: 1;
   display: flex;
   justify-content: center;
   align-items: center;
```

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-114.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-114.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-120.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-120.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-144.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-144.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-150.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-150.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-152.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-152.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-16.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-16.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-160.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-160.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-180.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-180.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-192.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-192.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-310.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-310.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-32.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-32.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-57.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-57.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-60.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-60.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-64.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-64.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-70.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-70.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-72.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-72.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-76.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-76.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon-96.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon-96.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon.ico` & `monopyly-1.3.0/monopyly/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/favicon/favicon.png` & `monopyly-1.3.0/monopyly/static/favicon/favicon.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/statement.png` & `monopyly-1.3.0/monopyly/static/img/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/cards/chase-card.png` & `monopyly-1.3.0/monopyly/static/img/cards/chase-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/cards/discover-card.png` & `monopyly-1.3.0/monopyly/static/img/cards/discover-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/cards/new-card.png` & `monopyly-1.3.0/monopyly/static/img/cards/new-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/cards/template-card.png` & `monopyly-1.3.0/monopyly/static/img/cards/template-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/arrow-down.png` & `monopyly-1.3.0/monopyly/static/img/icons/arrow-down.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/arrow-left.png` & `monopyly-1.3.0/monopyly/static/img/icons/arrow-left.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/arrow-up.png` & `monopyly-1.3.0/monopyly/static/img/icons/arrow-up.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/checkmark.png` & `monopyly-1.3.0/monopyly/static/img/icons/checkmark.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/delete-orange-thick.png` & `monopyly-1.3.0/monopyly/static/img/icons/delete-orange-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/delete-orange.png` & `monopyly-1.3.0/monopyly/static/img/icons/delete-orange.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/delete-thick.png` & `monopyly-1.3.0/monopyly/static/img/icons/delete-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/delete.png` & `monopyly-1.3.0/monopyly/static/img/icons/delete.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/edit.png` & `monopyly-1.3.0/monopyly/static/img/icons/edit.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/link.png` & `monopyly-1.3.0/monopyly/static/img/icons/link.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/minus-thick.png` & `monopyly-1.3.0/monopyly/static/img/icons/minus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/minus.png` & `monopyly-1.3.0/monopyly/static/img/icons/minus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/plus-thick.png` & `monopyly-1.3.0/monopyly/static/img/icons/plus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/plus.png` & `monopyly-1.3.0/monopyly/static/img/icons/plus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/refresh.png` & `monopyly-1.3.0/monopyly/static/img/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/save.png` & `monopyly-1.3.0/monopyly/static/img/icons/save.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/sort-asc.png` & `monopyly-1.3.0/monopyly/static/img/icons/sort-asc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/sort-desc.png` & `monopyly-1.3.0/monopyly/static/img/icons/sort-desc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/statement.png` & `monopyly-1.3.0/monopyly/static/img/icons/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/img/icons/x-thick.png` & `monopyly-1.3.0/monopyly/static/img/icons/x-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/add_subtransaction.js` & `monopyly-1.3.0/monopyly/static/js/add_subtransaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/add_transfer.js` & `monopyly-1.3.0/monopyly/static/js/add_transfer.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/bind_tag_actions.js` & `monopyly-1.3.0/monopyly/static/js/bind_tag_actions.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/define_filter.js` & `monopyly-1.3.0/monopyly/static/js/define_filter.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/display_new_account_type_inputs.js` & `monopyly-1.3.0/monopyly/static/js/display_new_account_type_inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/display_new_credit_account_inputs.js` & `monopyly-1.3.0/monopyly/static/js/display_new_credit_account_inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/expand_transaction.js` & `monopyly-1.3.0/monopyly/static/js/expand_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/flip_card.js` & `monopyly-1.3.0/monopyly/static/js/flip_card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/infer_card.js` & `monopyly-1.3.0/monopyly/static/js/infer_card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/infer_statement.js` & `monopyly-1.3.0/monopyly/static/js/infer_statement.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/make_payment.js` & `monopyly-1.3.0/monopyly/static/js/make_payment.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/show_linked_transaction.js` & `monopyly-1.3.0/monopyly/static/js/show_linked_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/update_account_statement_parameters.js` & `monopyly-1.3.0/monopyly/static/js/update_account_statement_parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/update_card_status.js` & `monopyly-1.3.0/monopyly/static/js/update_card_status.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/update_statement_parameters.js` & `monopyly-1.3.0/monopyly/static/js/update_statement_parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/update_statements_display.js` & `monopyly-1.3.0/monopyly/static/js/update_statements_display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/update_transactions_display.js` & `monopyly-1.3.0/monopyly/static/js/update_transactions_display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/autocomplete_input.js` & `monopyly-1.3.0/monopyly/static/js/modules/autocomplete_input.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,24 +7,24 @@
  */
 
 import {
     executeAjaxRequest
 } from './ajax.js';
 
 
-function anchoredMatch(string1, string2) {
+function isAnchoredMatch(string1, string2) {
     if (string2.startsWith(string1)) {
         return true;
     } else {
         return false;
     }
 }
 
 
-function containedMatch(string1, string2) {
+function isContainedMatch(string1, string2) {
     if (string2.includes(string1)) {
         return true;
     } else {
         return false;
     }
 }
 
@@ -126,42 +126,46 @@
         // Select a suggestion from the list
         if (suggestion !== null) {
             this.fill(suggestion);
         }
         this.close();
     }
 
+    /**
+     * Populate the input element text using the chosen suggestion.
+     */
     fill(suggestion) {
-        // Populate the input element text using the chosen suggestion
         this.inputElement.value = suggestion.textContent;
     }
 
     advanceFocus() {
         // Shift the focus to the next input element
         const nextInputIndex = this.$inputElements.index(this.inputElement) + 1;
         this.$inputElements.eq(nextInputIndex).focus();
     }
 
     #needsRefresh(userInput) {
         // Check if the list of matches needs to be refreshed
-        this.#refreshMatches(userInput);
+        this.refreshMatches(userInput);
         const matchCount = this.matches.length;
         const matchIsUserInput = (matchCount == 1 && userInput == this.matches[0]);
         if (matchCount < 1 || matchIsUserInput || !userInput) {
             return false;
         } else {
             return true;
         }
     }
 
-    #refreshMatches(userInput) {
-        // Refresh autocomplete suggestions using the AJAX response
+    /**
+     * Refresh autocomplete suggestions using the AJAX response.
+     */
+    refreshMatches(userInput) {
         this.matches = [];
-        this.#testMatches(userInput, anchoredMatch);
-        this.#testMatches(userInput, containedMatch);
+        this.#testMatches(userInput, isAnchoredMatch);
+        this.#testMatches(userInput, isContainedMatch);
     }
 
     #testMatches(userInput, testFunction) {
         // Add responses matching the user input to the set of matching suggestions
         for (let i = 0; i < this.response.length; i++) {
             const responseSuggestion = this.response[i];
             // Test (lowercase) match status and if already recorded
```

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/expand_transaction.js` & `monopyly-1.3.0/monopyly/static/js/modules/expand_transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/manage_acquisition_form.js` & `monopyly-1.3.0/monopyly/static/js/modules/manage_acquisition_form.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/manage_overlays.js` & `monopyly-1.3.0/monopyly/static/js/modules/manage_overlays.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/manage_subforms.js` & `monopyly-1.3.0/monopyly/static/js/modules/manage_subforms.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/update_database_widget.js` & `monopyly-1.3.0/monopyly/static/js/modules/update_database_widget.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/static/js/modules/update_display_ajax.js` & `monopyly-1.3.0/monopyly/static/js/modules/update_display_ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/about.html` & `monopyly-1.3.0/monopyly/templates/story.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,192 +1,201 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6c61 796f  {% extends "layo
 00000010: 7574 2e68 746d 6c22 2025 7d0a 0a7b 2520  ut.html" %}..{% 
 00000020: 626c 6f63 6b20 7469 746c 6520 257d 0a20  block title %}. 
-00000030: 2041 626f 7574 0a7b 2520 656e 6462 6c6f   About.{% endblo
+00000030: 2053 746f 7279 0a7b 2520 656e 6462 6c6f   Story.{% endblo
 00000040: 636b 2025 7d0a 0a7b 2520 626c 6f63 6b20  ck %}..{% block 
 00000050: 6865 6164 6572 2025 7d0a 2020 3c68 313e  header %}.  <h1>
 00000060: 5061 7373 2067 6f20 616e 6420 636f 6c6c  Pass go and coll
 00000070: 6563 7420 2432 3030 3c2f 6831 3e0a 7b25  ect $200</h1>.{%
 00000080: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
 00000090: 2062 6c6f 636b 2063 6f6e 7465 6e74 2025   block content %
-000000a0: 7d0a 2020 3c64 6976 2069 643d 2261 626f  }.  <div id="abo
-000000b0: 7574 223e 0a20 2020 203c 703e 4974 2073  ut">.    <p>It s
-000000c0: 7461 7274 6564 2077 6974 6820 4d69 6372  tarted with Micr
-000000d0: 6f73 6f66 7420 4578 6365 6c2e 203c 2f70  osoft Excel. </p
-000000e0: 3e0a 2020 2020 3c70 3e57 6865 6e20 4920  >.    <p>When I 
-000000f0: 676f 7420 6d79 2066 6972 7374 2062 616e  got my first ban
-00000100: 6b20 6163 636f 756e 742c 206d 7920 6461  k account, my da
-00000110: 6420 7461 7567 6874 206d 6520 686f 7720  d taught me how 
-00000120: 746f 206b 6565 7020 7472 6163 6b20 6f66  to keep track of
-00000130: 2061 6c6c 206d 7920 6669 6e61 6e63 6573   all my finances
-00000140: 2069 6e20 616e 2045 7863 656c 2077 6f72   in an Excel wor
-00000150: 6b62 6f6f 6b2e 0a20 2020 2041 7320 4920  kbook..    As I 
-00000160: 6163 7175 6972 6564 2061 2068 616e 6466  acquired a handf
-00000170: 756c 206f 6620 6372 6564 6974 2063 6172  ul of credit car
-00000180: 6473 2c20 696e 7665 7374 6d65 6e74 732c  ds, investments,
-00000190: 2061 6e64 206f 7468 6572 2074 7970 6573   and other types
-000001a0: 206f 6620 6261 6e6b 2061 6363 6f75 6e74   of bank account
-000001b0: 732c 2049 206b 6570 7420 6164 6469 6e67  s, I kept adding
-000001c0: 2073 6865 6574 7320 746f 2074 6865 2066   sheets to the f
-000001d0: 696c 652e 0a20 2020 2041 7420 7468 6520  ile..    At the 
-000001e0: 7361 6d65 2074 696d 652c 2049 2077 6173  same time, I was
-000001f0: 2066 696e 6469 6e67 206d 6f72 6520 616e   finding more an
-00000200: 6420 6d6f 7265 2077 6179 7320 746f 2069  d more ways to i
-00000210: 6e63 6c75 6465 2069 6e63 7265 6173 696e  nclude increasin
-00000220: 676c 7920 636f 6d70 6c69 6361 7465 6420  gly complicated 
-00000230: 616e 616c 7973 6973 2074 6f20 7472 6163  analysis to trac
-00000240: 6b20 6d79 2073 6176 696e 6773 2061 6e64  k my savings and
-00000250: 206d 6f6e 6974 6f72 206d 7920 7370 656e   monitor my spen
-00000260: 6469 6e67 2e0a 2020 2020 4920 6861 6420  ding..    I had 
-00000270: 616c 6c20 7468 6973 2064 6174 612c 2061  all this data, a
-00000280: 6e64 2049 2077 616e 7465 6420 746f 2067  nd I wanted to g
-00000290: 6574 2061 7320 6d75 6368 206f 7574 206f  et as much out o
-000002a0: 6620 6974 2061 7320 4920 706f 7373 6962  f it as I possib
-000002b0: 6c79 2063 6f75 6c64 2e0a 2020 2020 5468  ly could..    Th
-000002c0: 6973 2061 6c6c 206b 6570 7420 6d65 2073  is all kept me s
-000002d0: 6174 6973 6669 6564 2075 6e74 696c 2061  atisfied until a
-000002e0: 626f 7574 2068 616c 6677 6179 2074 6872  bout halfway thr
-000002f0: 6f75 6768 2063 6f6c 6c65 6765 2c20 7768  ough college, wh
-00000300: 656e 2049 2072 6561 6c69 7a65 6420 7468  en I realized th
-00000310: 6174 2049 2063 6f75 6c64 2064 6f20 7761  at I could do wa
-00000320: 7920 6d6f 7265 2075 7369 6e67 2064 6174  y more using dat
-00000330: 6162 6173 6573 2061 6e64 2050 7974 686f  abases and Pytho
-00000340: 6e2e 0a20 2020 2049 2063 6f75 6c64 2073  n..    I could s
-00000350: 6f72 7420 616e 6420 7461 6720 7479 7065  ort and tag type
-00000360: 7320 6f66 2074 7261 6e73 6163 7469 6f6e  s of transaction
-00000370: 732c 206c 696e 6b20 6372 6564 6974 2063  s, link credit c
-00000380: 6172 6420 7061 796d 656e 7473 2077 6974  ard payments wit
-00000390: 6820 6261 6e6b 2077 6974 6864 7261 7761  h bank withdrawa
-000003a0: 6c73 2c20 616e 6420 6372 6561 7465 2073  ls, and create s
-000003b0: 7065 6e64 696e 6720 7265 706f 7274 732e  pending reports.
-000003c0: 0a20 2020 2057 6869 6c65 2061 6c6c 2074  .    While all t
-000003d0: 6869 7320 7374 7566 6620 6973 2070 726f  his stuff is pro
-000003e0: 6261 626c 7920 646f 6162 6c65 2069 6e20  bably doable in 
-000003f0: 4578 6365 6c2c 2069 7420 6465 6669 6e69  Excel, it defini
-00000400: 7465 6c79 2069 7320 6e6f 7420 7768 6174  tely is not what
-00000410: 2069 7420 6973 2064 6573 6967 6e65 6420   it is designed 
-00000420: 746f 2064 6fe2 8094 4578 6365 6c20 6765  to do...Excel ge
-00000430: 7473 2063 6c75 6e6b 7920 6661 7374 2e0a  ts clunky fast..
-00000440: 2020 2020 4173 2049 2074 7261 6e73 6974      As I transit
-00000450: 696f 6e65 6420 746f 2067 7261 6475 6174  ioned to graduat
-00000460: 6520 7363 686f 6f6c 2c20 4920 616c 736f  e school, I also
-00000470: 2074 7261 6e73 6974 696f 6e65 6420 746f   transitioned to
-00000480: 2074 7261 636b 696e 6720 6d79 2066 696e   tracking my fin
-00000490: 616e 6365 7320 696e 2061 204d 7953 514c  ances in a MySQL
-000004a0: 2064 6174 6162 6173 652c 2061 6363 6573   database, acces
-000004b0: 7365 6420 7468 726f 7567 6820 5079 7468  sed through Pyth
-000004c0: 6f6e 2061 6e64 2061 2073 6574 206f 6620  on and a set of 
-000004d0: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-000004e0: 732e 0a20 2020 2054 6861 7420 6170 7072  s..    That appr
-000004f0: 6f61 6368 2067 6176 6520 6d65 206d 6f72  oach gave me mor
-00000500: 6520 706f 7765 7220 616e 6420 666c 6578  e power and flex
-00000510: 6962 696c 7479 2c20 6275 7420 4920 666f  ibilty, but I fo
-00000520: 756e 6420 6974 2074 6f20 6265 2061 2062  und it to be a b
-00000530: 6974 2074 6f6f 2063 756d 6265 7273 6f6d  it too cumbersom
-00000540: 6520 666f 7220 6461 7920 746f 2064 6179  e for day to day
-00000550: 2075 7365 2e3c 2f70 3e0a 0a20 2020 203c   use.</p>..    <
-00000560: 703e 4d79 2069 6465 616c 2073 6974 7561  p>My ideal situa
-00000570: 7469 6f6e 3f3c 2f70 3e0a 0a20 2020 203c  tion?</p>..    <
-00000580: 703e 4920 756c 7469 6d61 7465 6c79 2077  p>I ultimately w
-00000590: 616e 7465 6420 6120 7379 7374 656d 2074  anted a system t
-000005a0: 6861 7420 6b65 6570 2074 7261 636b 206f  hat keep track o
-000005b0: 6620 6576 6572 7974 6869 6e67 2028 6372  f everything (cr
-000005c0: 6564 6974 2063 6172 6420 7472 616e 7361  edit card transa
-000005d0: 6374 696f 6e73 2c20 6261 6e6b 2061 6363  ctions, bank acc
-000005e0: 6f75 6e74 732c 2069 6e76 6573 746d 656e  ounts, investmen
-000005f0: 7473 2c20 7265 7469 7265 6d65 6e74 2061  ts, retirement a
-00000600: 6363 6f75 6e74 732c 2061 6c6c 2074 6861  ccounts, all tha
-00000610: 7420 2429 2069 6e20 6f6e 6520 706c 6163  t $) in one plac
-00000620: 652e 0a20 2020 2049 206b 6e6f 7720 7468  e..    I know th
-00000630: 6174 2074 6865 7265 2065 7869 7374 2073  at there exist s
-00000640: 6f6c 7574 696f 6e73 206f 7574 2074 6865  olutions out the
-00000650: 7265 2061 6c72 6561 6479 2074 6f20 646f  re already to do
-00000660: 2074 6869 73e2 8094 4d69 6e74 2c20 666f   this...Mint, fo
-00000670: 7220 6f6e 65e2 8094 6275 7420 4920 6e65  r one...but I ne
-00000680: 7665 7220 7761 6e74 6564 2074 6f20 676f  ver wanted to go
-00000690: 2074 6861 7420 726f 7574 652e 0a20 2020   that route..   
-000006a0: 2046 6f72 206f 6e65 2074 6869 6e67 2c20   For one thing, 
-000006b0: 4920 7761 6e74 6564 2073 6f6d 6574 6869  I wanted somethi
-000006c0: 6e67 2077 6974 686f 7574 203c 656d 3e61  ng without <em>a
-000006d0: 6c6c 3c2f 656d 3e20 7468 6520 6265 6c6c  ll</em> the bell
-000006e0: 7320 616e 6420 7768 6973 746c 6573 2028  s and whistles (
-000006f0: 616e 6420 6164 7665 7274 6973 656d 656e  and advertisemen
-00000700: 7473 292c 2062 7574 2077 6869 6368 2073  ts), but which s
-00000710: 7469 6c6c 2068 6164 2077 6861 7420 4920  till had what I 
-00000720: 636f 6e73 6964 6572 6564 2075 7365 6675  considered usefu
-00000730: 6c20 6675 6e63 7469 6f6e 616c 6974 792e  l functionality.
-00000740: 0a20 2020 2049 2061 6c73 6f20 7761 6e74  .    I also want
-00000750: 6564 2073 6f6d 6574 6869 6e67 2074 6861  ed something tha
-00000760: 7420 4920 636f 756c 6420 6375 7374 6f6d  t I could custom
-00000770: 697a 6520 7768 656e 2049 2064 6964 6e27  ize when I didn'
-00000780: 7420 6c69 6b65 2061 2066 6561 7475 7265  t like a feature
-00000790: 2c20 6f72 2077 6865 6e20 4920 7761 6e74  , or when I want
-000007a0: 6564 206d 6f72 652e 3c2f 703e 0a0a 2020  ed more.</p>..  
-000007b0: 2020 3c70 3e54 6861 7427 7320 686f 7720    <p>That's how 
-000007c0: 7468 6973 2061 7070 2063 616d 6520 6162  this app came ab
-000007d0: 6f75 742e 0a20 2020 2049 2073 7461 7274  out..    I start
-000007e0: 6564 2062 7920 7472 7969 6e67 2074 6f20  ed by trying to 
-000007f0: 6a75 7374 2063 7265 6174 6520 6120 4755  just create a GU
-00000800: 4920 666f 7220 6d79 2050 7974 686f 6e20  I for my Python 
-00000810: 6461 7461 6261 7365 2069 6e74 6572 6661  database interfa
-00000820: 6365 2c20 6275 7420 4920 736f 6f6e 2072  ce, but I soon r
-00000830: 6561 6c69 7a65 6420 7468 6174 2049 2065  ealized that I e
-00000840: 7665 6e74 7561 6c6c 7920 7761 6e74 6564  ventually wanted
-00000850: 2074 6f20 6861 7665 2072 656d 6f74 6520   to have remote 
-00000860: 6163 6365 7373 2e0a 2020 2020 5768 7920  access..    Why 
-00000870: 6372 6561 7465 2061 2054 6b69 6e74 6572  create a Tkinter
-00000880: 2047 5549 2069 6620 6576 656e 7475 616c   GUI if eventual
-00000890: 6c79 2049 2764 206e 6565 6420 746f 2067  ly I'd need to g
-000008a0: 6f20 6261 636b 2061 6e64 2063 6861 6e67  o back and chang
-000008b0: 6520 7468 6520 696e 7465 7266 6163 6520  e the interface 
-000008c0: 746f 2077 6f72 6b20 7468 726f 7567 6820  to work through 
-000008d0: 6120 6272 6f77 7365 7220 6f72 2061 7070  a browser or app
-000008e0: 2065 6e76 6972 6f6e 6d65 6e74 3f0a 2020   environment?.  
-000008f0: 2020 2854 6b69 6e74 6572 2069 7320 616c    (Tkinter is al
-00000900: 736f 2061 2062 6974 206f 6620 6120 7061  so a bit of a pa
-00000910: 696e 2074 6f20 636f 6465 2c20 616e 6420  in to code, and 
-00000920: 6120 6269 6767 6572 2070 6169 6e20 746f  a bigger pain to
-00000930: 2074 6573 742c 2061 6e64 2074 6861 7420   test, and that 
-00000940: 6365 7274 6169 6e6c 7920 776f 756c 646e  certainly wouldn
-00000950: 2774 2064 6f2e 290a 2020 2020 416e 7977  't do.).    Anyw
-00000960: 6179 2c20 4927 6420 616c 7761 7973 2077  ay, I'd always w
-00000970: 616e 7465 6420 746f 2063 7265 6174 6520  anted to create 
-00000980: 616e 2061 7070 2c20 616e 6420 4920 6669  an app, and I fi
-00000990: 6775 7265 6420 7468 6973 2077 6173 2061  gured this was a
-000009a0: 7320 676f 6f64 2061 2063 6861 6e63 6520  s good a chance 
-000009b0: 6173 2061 6e79 2074 6f20 6765 7420 7374  as any to get st
-000009c0: 6172 7465 642e 0a20 2020 2057 696e 2d77  arted..    Win-w
-000009d0: 696e 2e3c 2f70 3e0a 0a20 2020 203c 703e  in.</p>..    <p>
-000009e0: 4966 2079 6f75 2772 6520 7265 6164 696e  If you're readin
-000009f0: 6720 7468 6973 2c20 4920 7375 7070 6f73  g this, I suppos
-00000a00: 6520 6974 206d 6561 6e73 2079 6f75 2772  e it means you'r
-00000a10: 6520 696e 7465 7265 7374 6564 2069 6e20  e interested in 
-00000a20: 7468 6520 7072 6f67 7261 6d20 286f 7220  the program (or 
-00000a30: 6d61 7962 6520 6a75 7374 2063 7572 696f  maybe just curio
-00000a40: 7573 2077 6861 7420 7468 6520 6865 6c6c  us what the hell
-00000a50: 2074 6869 7320 6e75 746a 6f62 2069 7320   this nutjob is 
-00000a60: 7761 7374 696e 6720 6869 7320 7469 6d65  wasting his time
-00000a70: 206f 6e29 2e20 4966 2074 6865 2066 6f72   on). If the for
-00000a80: 6d65 722c 2074 6861 7420 6d61 6b65 7320  mer, that makes 
-00000a90: 6d65 2072 6561 6c6c 7920 6861 7070 792c  me really happy,
-00000aa0: 2061 6e64 2049 2068 6f70 6520 7468 6174   and I hope that
-00000ab0: 2069 6620 796f 7520 7468 696e 6b20 6974   if you think it
-00000ac0: 2773 2063 6f6f 6c20 6f72 2069 6e74 6572  's cool or inter
-00000ad0: 6573 7469 6e67 2079 6f75 2067 6976 6520  esting you give 
-00000ae0: 6974 2061 2074 7279 2c20 6375 7374 6f6d  it a try, custom
-00000af0: 697a 6520 6974 2074 6865 2077 6179 2079  ize it the way y
-00000b00: 6f75 2077 616e 742c 206f 7220 6d61 6b65  ou want, or make
-00000b10: 2073 7567 6765 7374 696f 6e73 2e20 4920   suggestions. I 
-00000b20: 696e 7465 6e64 2074 6f20 616c 7761 7973  intend to always
-00000b30: 206b 6565 7020 7468 6520 6261 7369 6320   keep the basic 
-00000b40: 636f 6e63 6570 7420 6f70 656e 2073 6f75  concept open sou
-00000b50: 7263 652c 2073 6f20 706c 6179 2061 726f  rce, so play aro
-00000b60: 756e 6420 6173 206d 7563 6820 6173 2079  und as much as y
-00000b70: 6f75 2764 206c 696b 6521 3c2f 703e 0a0a  ou'd like!</p>..
-00000b80: 2020 2020 3c70 2063 6c61 7373 3d22 7369      <p class="si
-00000b90: 676e 6174 7572 6522 3e2d 4d69 7463 683c  gnature">-Mitch<
-00000ba0: 2f70 3e0a 2020 3c2f 6469 763e 0a0a 2020  /p>.  </div>..  
-00000bb0: 3c61 2068 7265 663d 227b 7b20 7572 6c5f  <a href="{{ url_
-00000bc0: 666f 7228 2763 6f72 652e 6372 6564 6974  for('core.credit
-00000bd0: 7327 2920 7d7d 223e 4372 6564 6974 733c  s') }}">Credits<
-00000be0: 2f61 3e0a 7b25 2065 6e64 626c 6f63 6b20  /a>.{% endblock 
-00000bf0: 257d 0a                                  %}.
+000000a0: 7d0a 2020 3c64 6976 2069 643d 2273 746f  }.  <div id="sto
+000000b0: 7279 2220 636c 6173 733d 2261 626f 7574  ry" class="about
+000000c0: 223e 0a20 2020 203c 703e 4974 2073 7461  ">.    <p>It sta
+000000d0: 7274 6564 2077 6974 6820 4d69 6372 6f73  rted with Micros
+000000e0: 6f66 7420 4578 6365 6c2e 203c 2f70 3e0a  oft Excel. </p>.
+000000f0: 2020 2020 3c70 3e57 6865 6e20 4920 676f      <p>When I go
+00000100: 7420 6d79 2066 6972 7374 2062 616e 6b20  t my first bank 
+00000110: 6163 636f 756e 742c 206d 7920 6461 6420  account, my dad 
+00000120: 7461 7567 6874 206d 6520 686f 7720 746f  taught me how to
+00000130: 206b 6565 7020 7472 6163 6b20 6f66 2061   keep track of a
+00000140: 6c6c 206d 7920 6669 6e61 6e63 6573 2069  ll my finances i
+00000150: 6e20 616e 2045 7863 656c 2077 6f72 6b62  n an Excel workb
+00000160: 6f6f 6b2e 0a20 2020 2049 7420 776f 726b  ook..    It work
+00000170: 6564 2066 6f72 2061 2077 6869 6c65 2c20  ed for a while, 
+00000180: 616e 6420 6173 2049 2061 6371 7569 7265  and as I acquire
+00000190: 6420 6120 6861 6e64 6675 6c20 6f66 2063  d a handful of c
+000001a0: 7265 6469 7420 6361 7264 732c 2069 6e76  redit cards, inv
+000001b0: 6573 746d 656e 7473 2c20 616e 6420 6f74  estments, and ot
+000001c0: 6865 7220 7479 7065 7320 6f66 2062 616e  her types of ban
+000001d0: 6b20 6163 636f 756e 7473 2c20 4920 6b65  k accounts, I ke
+000001e0: 7074 2061 6464 696e 6720 7368 6565 7473  pt adding sheets
+000001f0: 2074 6f20 7468 6174 2066 696c 652e 0a20   to that file.. 
+00000200: 2020 204f 6620 636f 7572 7365 2c20 7369     Of course, si
+00000210: 6e63 6520 4920 7761 7320 7472 6163 6b69  nce I was tracki
+00000220: 6e67 2061 6c6c 2074 6861 7420 6461 7461  ng all that data
+00000230: 2c20 4920 7761 6e74 6564 2074 6f20 7772  , I wanted to wr
+00000240: 696e 6720 6173 206d 7563 6820 696e 666f  ing as much info
+00000250: 726d 6174 696f 6e20 6f75 7420 6f66 2069  rmation out of i
+00000260: 7420 6173 2049 2070 6f73 7369 626c 7920  t as I possibly 
+00000270: 636f 756c 64e2 8094 616e 6420 736f 2049  could...and so I
+00000280: 2073 7461 7274 6564 2077 6f72 6b69 6e67   started working
+00000290: 2072 7564 696d 656e 7461 7279 2061 6e61   rudimentary ana
+000002a0: 6c79 7469 6373 2069 6e74 6f20 7468 6520  lytics into the 
+000002b0: 7370 7265 6164 7368 6565 742e 0a20 2020  spreadsheet..   
+000002c0: 203c 2f70 3e0a 0a20 2020 203c 2f70 3e0a   </p>..    </p>.
+000002d0: 2020 2020 5468 6973 2061 6c6c 206b 6570      This all kep
+000002e0: 7420 6d65 2073 6174 6973 6669 6564 2075  t me satisfied u
+000002f0: 6e74 696c 2061 626f 7574 2068 616c 6677  ntil about halfw
+00000300: 6179 2074 6872 6f75 6768 2063 6f6c 6c65  ay through colle
+00000310: 6765 2077 6865 6e20 4920 6265 6761 6e20  ge when I began 
+00000320: 6c65 6172 6e69 6e67 2050 7974 686f 6e2e  learning Python.
+00000330: 0a20 2020 2045 7863 656c 2077 6173 2067  .    Excel was g
+00000340: 6574 7469 6e67 2063 756d 6265 7273 6f6d  etting cumbersom
+00000350: 652c 2061 6e64 2049 2077 616e 7465 6420  e, and I wanted 
+00000360: 746f 2062 6520 6162 6c65 2074 6f20 736f  to be able to so
+00000370: 7274 2061 6e64 2074 6167 2074 7970 6573  rt and tag types
+00000380: 206f 6620 7472 616e 7361 6374 696f 6e73   of transactions
+00000390: 2c20 6c69 6e6b 2063 7265 6469 7420 6361  , link credit ca
+000003a0: 7264 2070 6179 6d65 6e74 7320 7769 7468  rd payments with
+000003b0: 2062 616e 6b20 7769 7468 6472 6177 616c   bank withdrawal
+000003c0: 732c 2061 6e64 2063 7265 6174 6520 7370  s, and create sp
+000003d0: 656e 6469 6e67 2072 6570 6f72 7473 2e0a  ending reports..
+000003e0: 2020 2020 5365 6569 6e67 2074 6865 2070      Seeing the p
+000003f0: 6f74 656e 7469 616c 2077 6179 7320 4920  otential ways I 
+00000400: 636f 756c 6420 7573 6520 6120 7374 616e  could use a stan
+00000410: 6461 6c6f 6e65 2070 726f 6772 616d 6d69  dalone programmi
+00000420: 6e67 206c 616e 6775 6167 6520 746f 2075  ng language to u
+00000430: 7020 6d79 2067 616d 652c 2049 2072 6561  p my game, I rea
+00000440: 6c69 7a65 6420 7468 6174 2077 6861 7420  lized that what 
+00000450: 4920 7265 616c 6c79 206e 6565 6465 6420  I really needed 
+00000460: 7761 7320 6120 6461 7461 6261 7365 2e0a  was a database..
+00000470: 2020 2020 4173 2049 2074 7261 6e73 6974      As I transit
+00000480: 696f 6e65 6420 746f 2067 7261 6475 6174  ioned to graduat
+00000490: 6520 7363 686f 6f6c 2c20 4920 616c 736f  e school, I also
+000004a0: 2074 7261 6e73 6974 696f 6e65 6420 746f   transitioned to
+000004b0: 2074 7261 636b 696e 6720 6d79 2066 696e   tracking my fin
+000004c0: 616e 6365 7320 696e 2061 204d 7953 514c  ances in a MySQL
+000004d0: 2064 6174 6162 6173 652c 2061 6363 6573   database, acces
+000004e0: 7365 6420 7769 7468 2050 7974 686f 6e20  sed with Python 
+000004f0: 7468 726f 7567 6820 6120 7365 7420 6f66  through a set of
+00000500: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
+00000510: 6b73 2e0a 2020 2020 5468 6174 2061 7070  ks..    That app
+00000520: 726f 6163 6820 6761 7665 206d 6520 736f  roach gave me so
+00000530: 206d 7563 6820 6d6f 7265 2070 6f77 6572   much more power
+00000540: 2061 6e64 2066 6c65 7869 6269 6c74 792c   and flexibilty,
+00000550: 2062 7574 2069 7420 7374 696c 6c20 6665   but it still fe
+00000560: 6c74 2061 206c 6974 746c 6520 636c 756e  lt a little clun
+00000570: 6b79 2e3c 2f70 3e0a 0a20 2020 203c 703e  ky.</p>..    <p>
+00000580: 4d79 2069 6465 616c 2073 6974 7561 7469  My ideal situati
+00000590: 6f6e 3f3c 2f70 3e0a 0a20 2020 203c 703e  on?</p>..    <p>
+000005a0: 4920 756c 7469 6d61 7465 6c79 2077 616e  I ultimately wan
+000005b0: 7465 6420 6120 7379 7374 656d 2074 6861  ted a system tha
+000005c0: 7420 6b65 6570 2074 7261 636b 206f 6620  t keep track of 
+000005d0: 6576 6572 7974 6869 6e67 e280 9463 7265  everything...cre
+000005e0: 6469 7420 6361 7264 2074 7261 6e73 6163  dit card transac
+000005f0: 7469 6f6e 732c 2062 616e 6b20 6163 636f  tions, bank acco
+00000600: 756e 7473 2c20 696e 7665 7374 6d65 6e74  unts, investment
+00000610: 732c 2072 6574 6972 656d 656e 7420 6163  s, retirement ac
+00000620: 636f 756e 7473 2c20 616c 6c20 7468 6174  counts, all that
+00000630: 2024 e280 9469 6e20 6f6e 6520 706c 6163   $...in one plac
+00000640: 652e 0a20 2020 204f 6276 696f 7573 6c79  e..    Obviously
+00000650: 2074 6865 7265 2061 7265 206d 6567 612d   there are mega-
+00000660: 6170 7073 2074 6861 7420 616c 7265 6164  apps that alread
+00000670: 7920 646f 2061 6c6c 2074 6869 732c 2062  y do all this, b
+00000680: 7574 2049 206e 6576 6572 2077 616e 7465  ut I never wante
+00000690: 6420 746f 2067 6f20 7468 6174 2072 6f75  d to go that rou
+000006a0: 7465 2e0a 2020 2020 4927 6420 616c 7761  te..    I'd alwa
+000006b0: 7973 206d 616e 6167 6564 206d 7920 6669  ys managed my fi
+000006c0: 6e61 6e63 6573 2069 6e64 6570 656e 6465  nances independe
+000006d0: 6e74 6c79 2c20 616e 6420 6861 6420 7a65  ntly, and had ze
+000006e0: 726f 2069 6e74 6572 6573 7420 696e 2063  ro interest in c
+000006f0: 6564 696e 6720 7468 6174 2063 6f6e 7472  eding that contr
+00000700: 6f6c 2e0a 2020 2020 466f 7220 6f6e 652c  ol..    For one,
+00000710: 2049 2077 616e 7465 6420 746f 206d 6169   I wanted to mai
+00000720: 6e74 6169 6e20 736f 6d65 2070 7269 7661  ntain some priva
+00000730: 6379 2072 6567 6172 6469 6e67 206d 7920  cy regarding my 
+00000740: 6669 6e61 6e63 6961 6c20 6461 7461 2c20  financial data, 
+00000750: 6265 6361 7573 6520 7768 6f20 6b6e 6f77  because who know
+00000760: 7320 686f 7720 7468 6f73 6520 6170 7073  s how those apps
+00000770: 2061 7265 2075 7369 6e67 2074 6861 7420   are using that 
+00000780: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
+00000790: 2054 776f 2c20 4920 6469 646e 2774 2077   Two, I didn't w
+000007a0: 616e 7420 3c65 6d3e 616c 6c3c 2f65 6d3e  ant <em>all</em>
+000007b0: 2074 6865 2062 656c 6c73 2061 6e64 2077   the bells and w
+000007c0: 6869 7374 6c65 7320 2861 6e64 2061 6476  histles (and adv
+000007d0: 6572 7469 7365 6d65 6e74 7329 2074 6861  ertisements) tha
+000007e0: 7420 7468 6f73 6520 6d65 6761 2d61 7070  t those mega-app
+000007f0: 7320 776f 756c 6420 666f 7263 6520 7570  s would force up
+00000800: 6f6e 206d 652c 2062 7574 2049 2061 6c73  on me, but I als
+00000810: 6f20 7761 6e74 6564 2073 6f6d 6574 6869  o wanted somethi
+00000820: 6e67 2049 2063 6f75 6c64 2063 7573 746f  ng I could custo
+00000830: 6d69 7a65 2077 6865 6e20 4920 6469 646e  mize when I didn
+00000840: 2774 206c 696b 6520 6120 6665 6174 7572  't like a featur
+00000850: 652e 2e2e 206f 7220 7768 656e 2049 2077  e... or when I w
+00000860: 616e 7465 6420 6d6f 7265 2e0a 2020 2020  anted more..    
+00000870: 416e 6420 7468 7265 652c 206d 6f73 7420  And three, most 
+00000880: 696d 706f 7274 616e 746c 792c 2069 7420  importantly, it 
+00000890: 7365 656d 6564 206c 696b 6520 6120 6675  seemed like a fu
+000008a0: 6e20 6368 616c 6c65 6e67 6520 7468 6174  n challenge that
+000008b0: 2077 6f75 6c64 206b 6565 7020 6d65 2064   would keep me d
+000008c0: 6565 706c 7920 656e 6761 6765 6420 696e  eeply engaged in
+000008d0: 206d 616e 6167 696e 6720 6d79 206f 776e   managing my own
+000008e0: 2066 696e 616e 6369 616c 2070 6963 7475   financial pictu
+000008f0: 7265 2e0a 0a20 2020 203c 703e 5468 6174  re...    <p>That
+00000900: 2773 2068 6f77 2074 6869 7320 6170 7020  's how this app 
+00000910: 6361 6d65 2061 626f 7574 2e0a 2020 2020  came about..    
+00000920: 4920 7374 6172 7465 6420 6279 2074 7279  I started by try
+00000930: 696e 6720 746f 206a 7573 7420 6372 6561  ing to just crea
+00000940: 7465 2061 2047 5549 2066 6f72 206d 7920  te a GUI for my 
+00000950: 5079 7468 6f6e 2064 6174 6162 6173 6520  Python database 
+00000960: 696e 7465 7266 6163 652c 2062 7574 2074  interface, but t
+00000970: 6861 7420 6469 646e 2774 206f 6666 6572  hat didn't offer
+00000980: 2074 6865 2067 7261 7068 6963 2066 6c65   the graphic fle
+00000990: 7869 6269 6c69 7479 206f 6620 6120 7765  xibility of a we
+000009a0: 6220 6170 702e 0a20 2020 2057 6879 2066  b app..    Why f
+000009b0: 6967 6874 2074 6f20 6275 696c 6420 6120  ight to build a 
+000009c0: 6e69 6365 2054 6b69 6e74 6572 2047 5549  nice Tkinter GUI
+000009d0: 2069 6620 4927 6420 6576 656e 7475 616c   if I'd eventual
+000009e0: 6c79 2067 6574 2073 6963 6b20 6f66 2074  ly get sick of t
+000009f0: 6861 7420 746f 6f3f 0a20 2020 2028 546b  hat too?.    (Tk
+00000a00: 696e 7465 7220 6973 2061 6c73 6f20 6120  inter is also a 
+00000a10: 6269 7420 6f66 2061 2070 6169 6e20 746f  bit of a pain to
+00000a20: 2063 6f64 652c 2061 6e64 2061 2062 6967   code, and a big
+00000a30: 6765 7220 7061 696e 2074 6f20 7465 7374  ger pain to test
+00000a40: 2c20 616e 6420 3c65 6d3e 7468 6174 3c2f  , and <em>that</
+00000a50: 656d 3e20 6365 7274 6169 6e6c 7920 776f  em> certainly wo
+00000a60: 756c 646e 2774 2064 6f2e 290a 2020 2020  uldn't do.).    
+00000a70: 416e 7977 6179 2c20 4927 6420 616c 7761  Anyway, I'd alwa
+00000a80: 7973 2077 616e 7465 6420 746f 2063 7265  ys wanted to cre
+00000a90: 6174 6520 616e 2061 7070 2c20 616e 6420  ate an app, and 
+00000aa0: 4920 6669 6775 7265 6420 7468 6973 2077  I figured this w
+00000ab0: 6173 2061 7320 676f 6f64 2061 2063 6861  as as good a cha
+00000ac0: 6e63 6520 6173 2061 6e79 2074 6f20 6765  nce as any to ge
+00000ad0: 7420 7374 6172 7465 642e 0a20 2020 2057  t started..    W
+00000ae0: 696e 2d77 696e 2e3c 2f70 3e0a 0a20 2020  in-win.</p>..   
+00000af0: 203c 703e 4966 2079 6f75 2772 6520 7265   <p>If you're re
+00000b00: 6164 696e 6720 7468 6973 2c20 4920 7375  ading this, I su
+00000b10: 7070 6f73 6520 6974 206d 6561 6e73 2079  ppose it means y
+00000b20: 6f75 2776 6520 7374 756d 626c 6564 2061  ou've stumbled a
+00000b30: 6372 6f73 7320 7468 6520 7072 6f67 7261  cross the progra
+00000b40: 6d20 6f75 7420 6f66 2069 6e74 6572 6573  m out of interes
+00000b50: 7420 286f 7220 6d61 7962 6520 796f 7527  t (or maybe you'
+00000b60: 7265 206a 7573 7420 6375 7269 6f75 7320  re just curious 
+00000b70: 7768 6174 2074 6865 2068 656c 6c20 7468  what the hell th
+00000b80: 6973 206e 7574 6a6f 6220 6973 2077 6173  is nutjob is was
+00000b90: 7469 6e67 2068 6973 2074 696d 6520 6f6e  ting his time on
+00000ba0: 292e 2049 6620 7468 6520 666f 726d 6572  ). If the former
+00000bb0: 2c20 636f 6f6c 2120 4665 656c 2066 7265  , cool! Feel fre
+00000bc0: 6520 746f 206c 6f6f 6b20 6172 6f75 6e64  e to look around
+00000bd0: 206f 7220 7461 6b65 2069 7420 666f 7220   or take it for 
+00000be0: 6120 7370 696e 2e20 4920 696e 7465 6e64  a spin. I intend
+00000bf0: 2074 6f20 616c 7761 7973 206b 6565 7020   to always keep 
+00000c00: 7468 6520 6261 7369 6320 636f 6e63 6570  the basic concep
+00000c10: 7420 6f70 656e 2073 6f75 7263 652c 2073  t open source, s
+00000c20: 6f20 706c 6179 2061 726f 756e 6420 6173  o play around as
+00000c30: 206d 7563 6820 6173 2079 6f75 2764 206c   much as you'd l
+00000c40: 696b 6521 3c2f 703e 0a0a 2020 2020 3c70  ike!</p>..    <p
+00000c50: 2063 6c61 7373 3d22 7369 676e 6174 7572   class="signatur
+00000c60: 6522 3e2d 4d69 7463 683c 2f70 3e0a 2020  e">-Mitch</p>.  
+00000c70: 3c2f 6469 763e 0a0a 7b25 2065 6e64 626c  </div>..{% endbl
+00000c80: 6f63 6b20 257d 0a                        ock %}.
```

### Comparing `monopyly-1.2.3/monopyly/templates/index.html` & `monopyly-1.3.0/monopyly/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,19 @@
             </a>
           </li>
           <li>
             <a href="{{ url_for('banking.add_account') }}">
               Add a new account
             </a>
           </li>
+          <li>
+            <a href="{{ url_for('credit.load_tags') }}">
+              Manage transaction tags
+            </a>
+          </li>
         </ul>
 
         <h3>Banks</h3>
 
         {% for bank in bank_accounts %}
           <ul class="category">
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 **** A homemade personal finance manager, built in Flask. ****
 
 {% if g.user %}
 ***** Bank Accounts *****
 *** Profile ***
 Manage_accounts
 Add_a_new_account
+Manage_transaction_tags
 **** Banks ****
 {% for bank in bank_accounts %}
 *** {{ bank.bank_name }} ***
 See_account_summaries
     * {% for account in bank_accounts[bank] %}
     * {{_account.account_type.type_common_name_}}_{{_account.last_four_digits
       }}
```

### Comparing `monopyly-1.2.3/monopyly/templates/layout.html` & `monopyly-1.3.0/monopyly/templates/layout.html`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         <nav id="nav-menu">
           <ul></strong>
 
             <li><a href="{{ url_for('core.index') }}">Home</a></li>
             <li><a href="{{ url_for('core.about') }}">About</a></li>
             {% if g.user %}
-              <li><span>{{ g.user.username }}</span></li>
+              <li><a href="{{url_for('core.load_profile') }}" class="username">{{ g.user.username }}</a></li>
               <li><a href="{{ url_for('auth.logout') }}">Log Out</a></li>
             {% else %}
               <li><a href="{{ url_for('auth.register') }}">Register</a></li>
               <li><a href="{{ url_for('auth.login') }}">Log In</a></li>
             {% endif %}
 
           </ul></strong>
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
 
 
 ******_Monopyly_******
 
 Home
 About
 {% if g.user %}
-{{ g.user.username }}
+{{_g.user.username_}}
 Log_Out
 {% else %}
 Register
 Log_In
 {% endif %}
 
  {% block left_sidebar %}{% endblock %}    {% block header %}{% endblock %}  {%
```

### Comparing `monopyly-1.2.3/monopyly/templates/banking/account_page.html` & `monopyly-1.3.0/monopyly/templates/banking/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/banking/account_summaries.html` & `monopyly-1.3.0/monopyly/templates/banking/account_summaries.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/banking/account_summaries_page.html` & `monopyly-1.3.0/monopyly/templates/banking/account_summaries_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/banking/accounts_page.html` & `monopyly-1.3.0/monopyly/templates/banking/accounts_page.html`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,32 @@
     {% for bank in banks %}
       {% set bank_accounts = bank.bank_accounts %}
       {% if bank_accounts %}
 
         <div class="bank-block grouping">
           <h3>{{ bank.bank_name }}</h3>
 
-          <div class="account-blocks">
+          <div class="account-blocks box-table">
             {% for account in bank_accounts %}
-              <div class="account-block">
+
+              <div class="account-block box-row">
 
                 <div class="account-info">
                   <span class="digits">{{ account.last_four_digits }}</span> <b>{{ account.account_type.type_name }}</b>
                </div>
 
                 <div class="expanded">
                   <div class="options">
                     <a class="icon-button action delete" href="{{ url_for('banking.delete_account', account_id=account.id) }}" onclick="return confirm('Are you sure you want to delete this account?');">
                     </a>
                   </div>
                 </div>
 
               </div>
+
             {% endfor %}
           </div>
 
         </div>
 
       {% endif %}
     {% endfor %}
@@ -84,10 +86,10 @@
 
     </div>
 
 {% endblock %}
 
 
 {% block javascript %}
-  <script src="{{ url_for('static', filename='js/expand_bank_account.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/expand_bank_account.js') }}">
   </script>
 {% endblock %}
```

### Comparing `monopyly-1.2.3/monopyly/templates/banking/account_form/account_form.html` & `monopyly-1.3.0/monopyly/templates/banking/account_form/account_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/banking/account_form/account_form_page_new.html` & `monopyly-1.3.0/monopyly/templates/banking/account_form/account_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/banking/transaction_form/bank_info_form.html` & `monopyly-1.3.0/monopyly/templates/banking/transaction_form/bank_info_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/banking/transaction_form/transaction_form.html` & `monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,24 @@
   <div class="form-line">
 
     <div class="form-field transaction-date-field">
       {{ form.transaction_date.label }}
       {{ form.transaction_date }}
     </div>
 
+    <div class="form-field merchant-field autocomplete">
+      {{ form.merchant.label }}
+      {{ form.merchant }}
+    </div>
+
   </div>
 
   <div id="subtransactions">
     {% for subform in form.subtransactions %}
-      {% include 'banking/transaction_form/subtransaction_form.html' %}
+      {% include 'common/transaction_form/subtransaction_subform.html' %}
     {% endfor %}
   </div>
 
   <div class="add-info buttons">
 
     <div id="new-subtransaction" class="add-info button">
       + Add Subtransaction
```

### Comparing `monopyly-1.2.3/monopyly/templates/banking/transaction_form/transaction_form_page.html` & `monopyly-1.3.0/monopyly/templates/banking/transaction_form/transaction_form_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {% block javascript %}
 
   <script>
     const AUTOCOMPLETE_ENDPOINT = "{{ url_for('banking.suggest_transaction_autocomplete') }}";
     const ADD_SUBTRANSACTION_FORM_ENDPOINT = "{{ url_for('banking.add_subtransaction_fields') }}";
     const ADD_TRANSFER_FORM_ENDPOINT = "{{ url_for('banking.add_transfer_field') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/autocomplete_banking_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/autocomplete_transaction.js') }}">
   </script>
   <script type="module" src="{{ url_for('static', filename='js/add_subtransaction.js') }}">
   </script>
   <script type="module" src="{{ url_for('static', filename='js/add_transfer.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.2.3/monopyly/templates/banking/transactions_table/transaction_field_titles.html` & `monopyly-1.3.0/monopyly/templates/banking/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/common/transactions_table/linked_bank_transaction.html` & `monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_bank_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/common/transactions_table/linked_credit_transaction.html` & `monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_credit_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/common/transactions_table/linked_transaction_overlay.html` & `monopyly-1.3.0/monopyly/templates/common/transactions_table/linked_transaction_overlay.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/common/transactions_table/transaction_expanded.html` & `monopyly-1.3.0/monopyly/templates/common/transactions_table/transaction_expanded.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/account_page.html` & `monopyly-1.3.0/monopyly/templates/credit/account_page.html`

 * *Files 7% similar despite different names*

```diff
@@ -44,30 +44,30 @@
           {% endfor %}
         </div>
       </div>
 
       <div class="info-row">
         <div class="info-title">Statement Issue Day</div>
         <div>
-          <div id="statement-issue-day" class="update-db-widget key-day">
+          <div id="statement-issue-day" class="update-db-widget right-hover-style key-day">
             <div class="widget-text">
               <div class="widget-display">
                 {{- account.statement_issue_day -}}
               </div>
               <input class="widget-input" type="text" name="issue_day" value="{{ account.statement_issue_day }}" />
             </div>
             <img class="widget-edit-button" src="{{ url_for('static', filename='img/icons/edit.png') }}" />
           </div>
         </div>
       </div>
 
       <div class="info-row">
         <div class="info-title">Statement Due Day</div>
         <div>
-          <div id="statement-due-day" class="update-db-widget key-day">
+          <div id="statement-due-day" class="update-db-widget right-hover-style key-day">
             <div class="widget-text">
               <div class="widget-display">
                 {{- account.statement_due_day -}}
               </div>
               <input class="widget-input" type="text" name="due_day" value="{{ account.statement_due_day }}" />
             </div>
             <img class="widget-edit-button" src="{{ url_for('static', filename='img/icons/edit.png') }}" />
```

### Comparing `monopyly-1.2.3/monopyly/templates/credit/cards.html` & `monopyly-1.3.0/monopyly/templates/credit/cards.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/statement_page.html` & `monopyly-1.3.0/monopyly/templates/credit/statement_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/statement_summary.html` & `monopyly-1.3.0/monopyly/templates/credit/statement_summary.html`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     <div>{{ statement.balance|currency }}</div>
   </div>
 
   <div id="payment">
 
     <div id="due">
       <div>DUE</div>
-      <div id="due-date" class="update-db-widget">
+      <div id="due-date" class="update-db-widget right-hover-style">
         <div class="widget-text">
           <div class="widget-display">{{ statement.due_date }}</div>
           <input class="widget-input" type="text" name="due_date" value="{{ statement.due_date }}" />
         </div>
         <img class="widget-edit-button" src="{{ url_for('static', filename='img/icons/edit.png') }}" />
       </div>
     </div>
```

### Comparing `monopyly-1.2.3/monopyly/templates/credit/statements.html` & `monopyly-1.3.0/monopyly/templates/credit/statements.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/statements_page.html` & `monopyly-1.3.0/monopyly/templates/credit/statements_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/tags_page.html` & `monopyly-1.3.0/monopyly/templates/credit/tags_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transaction_submission_page.html` & `monopyly-1.3.0/monopyly/templates/credit/transaction_submission_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transactions_page.html` & `monopyly-1.3.0/monopyly/templates/credit/transactions_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/card_form/card_form.html` & `monopyly-1.3.0/monopyly/templates/credit/card_form/card_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/card_form/card_form_page_new.html` & `monopyly-1.3.0/monopyly/templates/credit/card_form/card_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/card_form/transfer_statement_inquiry.html` & `monopyly-1.3.0/monopyly/templates/credit/card_form/transfer_statement_inquiry.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/card_graphic/card_back.html` & `monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_back.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/card_graphic/card_front.html` & `monopyly-1.3.0/monopyly/templates/credit/card_graphic/card_front.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/tag_tree/subtag_tree.html` & `monopyly-1.3.0/monopyly/templates/credit/tag_tree/subtag_tree.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transaction_form/subtransaction_form.html` & `monopyly-1.3.0/monopyly/templates/common/transaction_form/subtransaction_subform.html`

 * *Files 20% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     <div class="form-field note-field autocomplete">
       {{ subform.note.label }}
       {{ subform.note }}
     </div>
 
   </div>
 
-  <div class="form-field">
+  <div class="form-field autocomplete">
     {{ subform.tags.label }}
     {{ subform.tags }}
   </div>
 
 {% endblock %}
```

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transaction_form/transaction_form.html` & `monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form.html`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     {{ form.statement_info.issue_date.label }}
     {{ form.statement_info.issue_date }}
   </div>
 
 
   <div id="subtransactions">
     {% for subform in form.subtransactions %}
-      {% include 'credit/transaction_form/subtransaction_form.html' %}
+      {% include 'common/transaction_form/subtransaction_subform.html' %}
     {% endfor %}
   </div>
 
   <div class="add-info buttons">
     <div id="new-subtransaction" class="add-info button">
       + Add Subtransaction
     </div>
```

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transaction_form/transaction_form_page.html` & `monopyly-1.3.0/monopyly/templates/credit/transaction_form/transaction_form_page.html`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
   <script>
     const AUTOCOMPLETE_ENDPOINT = "{{ url_for('credit.suggest_transaction_autocomplete') }}";
     const INFER_CARD_ENDPOINT = "{{ url_for('credit.infer_card') }}";
     const INFER_STATEMENT_ENDPOINT = "{{ url_for('credit.infer_statement') }}";
     const ADD_SUBTRANSACTION_FORM_ENDPOINT = "{{ url_for('credit.add_subtransaction_fields') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/autocomplete_credit_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/autocomplete_transaction.js') }}">
   </script>
   <script type="module" src="{{ url_for('static', filename='js/infer_card.js') }}">
   </script>
   <script type="module" src="{{ url_for('static', filename='js/infer_statement.js') }}">
   </script>
   <script type="module" src="{{ url_for('static', filename='js/add_subtransaction.js') }}">
   </script>
```

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transactions_table/condensed_row_content.html` & `monopyly-1.3.0/monopyly/templates/credit/transactions_table/condensed_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transactions_table/expanded_row_content.html` & `monopyly-1.3.0/monopyly/templates/credit/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/monopyly/templates/credit/transactions_table/transaction_field_titles.html` & `monopyly-1.3.0/monopyly/templates/credit/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/.gitignore` & `monopyly-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/COPYING` & `monopyly-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `monopyly-1.2.3/pyproject.toml` & `monopyly-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 authors = [
     { name = 'Mitch Negus', email = 'mitchnegus57@gmail.com' },
 ]
 description = 'A homemade personal finance manager.'
 license = { text = 'GNU GPLv3' }
 requires-python = '>=3.9,<3.11'
 dependencies = [
+    'authanor>=1.0.1',
     'flask>=2.2.2',
     'flask-wtf',
+    'markdown>=3.4.3',
     'python-dateutil',
     'sqlalchemy>=2.0.0',
 ]
 keywords = [
   'Finance',
   'Personal Finance',
 ]
@@ -46,33 +48,53 @@
 Changelog = 'https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md'
 
 [tool.hatch.version]
 source = 'vcs'
 
 [tool.hatch.build.targets.sdist]
 include = [
+  '/README.md',
   '/monopyly',
 ]
+exclude = [
+  '*.pyc',
+]
 
 [tool.hatch.build.hooks.vcs]
 version-file = 'monopyly/_version.py'
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = 'text/markdown'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-path = 'README.md'
+path = 'monopyly/README.md'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = 'src="((?!https?:\/\/)\S+?)"'
 replacement = 'src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/\1"'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/mitchnegus/monopyly/blob/main/\g<2>)'
 
+[tool.pytest.ini_options]
+filterwarnings = [
+    'ignore::DeprecationWarning',
+    'ignore:INSECURE:UserWarning',
+]
+
+[tool.coverage.run]
+omit = [
+    'tests/*',
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    'raise NotImplementedError',
+]
+
 [tool.black]
 force-exclude = 'monopyly/_version.py'
 
 [tool.isort]
 profile = 'black'
-src_paths = ['monopyly', 'test']
+src_paths = ['monopyly', 'tests']
```

### Comparing `monopyly-1.2.3/PKG-INFO` & `monopyly-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopyly
-Version: 1.2.3
+Version: 1.3.0
 Summary: A homemade personal finance manager.
 Project-URL: Download, https://pypi.org/project/monopyly
 Project-URL: Homepage, https://github.com/mitchnegus/monopyly
 Project-URL: Repository, https://github.com/mitchnegus/monopyly
 Project-URL: Changelog, https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
@@ -19,23 +19,26 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Requires-Python: <3.11,>=3.9
+Requires-Dist: authanor>=1.0.1
 Requires-Dist: flask-wtf
 Requires-Dist: flask>=2.2.2
+Requires-Dist: markdown>=3.4.3
 Requires-Dist: python-dateutil
 Requires-Dist: sqlalchemy>=2.0.0
 Description-Content-Type: text/markdown
 
-# Monopyly
-
-#### _The Money Game_
+<div id="header">
+  <h1 id="title">Monopyly</h1>
+  <h4 id="tagline"><em>The Money Game</em></h4>
+</div>
 
 This is a package designed to help manage personal finances.
 The current functionality is fairly limited, with only the ability to track bank account and credit card history.
 Eventually the app will provide a full set of features including purchase history, investment profiles, and budgeting.
 
 The app is designed to be run at a small scale.
 Information is stored in a local SQLite database and accessed using a frontend served by Flask.
@@ -45,62 +48,62 @@
 
 ## Installation
 
 The _Monopyly_ app is registered on the [Python Package Index (PyPI)](https://pypi.org/project/monopyly) for easy installation.
 To install the app, simply run
 
 ```
-pip install monopyly
+$ pip install monopyly
 ```
 
 The package requires a recent version of Python (3.9+).
 
 
 ## Getting started
 
-Once the package is properly installed, run the app from the command line:
+Once the package is properly installed, run the app from the command line (the default options should be sensible, but you may customize the host and port if necessary):
 
 ```
-monopyly
+$ monopyly production [--host HOST] [--port PORT]
 ```
 
 This will open to an empty homepage with a welcome message.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/homepage.png" alt="user homepage" width="800px">
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/homepage.png" alt="user homepage" width="800px">
 
 To use the app, register a new profile and then log in using your newly created credentials.
 A successful login will return you to the homepage, now with several different feature panels.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/homepage-user.png" alt="user homepage" width="800px">
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/homepage-user.png" alt="user homepage" width="800px">
 
 Your username should now appear at the top right of the screen, and the 'Log In' button will be replaced with a 'Log Out' button.
 
 
 ## Features
 
 ### Bank Accounts
 
 _Monopyly_ provides an accounting system for a user's bank transactions.
 Banks can be added from the 'Manage accounts' page, where a user will be able to specify bank information including the bank and account type.
 While some account types are preloaded into the _Monopyly_ database (such as checking accounts, savings accounts, and certificates of deposit) each user can add additional custom account types as they need them.
 
 After you have created a bank account, either using a bank that already exists in the _Monopyly_ system or with a new bank, the app will redirect you back to the 'Manage accounts' page.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/bank-accounts.png" alt="bank accounts" width="800px" />
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/bank-accounts.png" alt="bank accounts" width="800px" />
 
 Once at least one bank account has been added, you can head on back to the account homepage to view balances and add transactions.
 On the left side of the page, each bank will have a section in the 'Bank Accounts' box.
 By clicking the 'See account summaries' button, you will be transferred to a page showing all of the bank accounts at the given bank, as well as the account balances of each account.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/bank-account-summaries.png" alt="bank account summaries" width="800px" />
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/bank-account-summaries.png" alt="bank account summaries" width="800px" />
 
 Clicking on any of these accounts will pull up a detailed summary of that account—a page that is also accessible directly from the _Monopyly_ homepage.
 This detailed summary will show the current balance, but also a comprehensive set of (recent) transactions on that account.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/bank-account-details.png" alt="bank account details" width="800px" />
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/bank-account-details.png" alt="bank account details" width="800px" />
 
 Transactions can be created from either this page or the homepage, specifying the bank account and all transaction details (date, amount, notes, etc.).
 Transactions can also be recorded as transfers between banks, such that they are automatically input into the database for both accounts.
 
 Clicking the plus icon next to any listed transaction will bring up an expanded view of the transaction describing the transaction in more detail, as well as a set of buttons for editing the transaction or seeing any other transactions to which this transaction is linked.
 
 
@@ -111,15 +114,15 @@
 From there, the app will allow you to add credit cards and associate each with an account.
 If an account does not already exist for the card you are trying to add, a card can be added to a new account.
 This account will be associated with a specific bank, and will track all of the cards for that account (cards are ID'd by the last four digits of the credit card number).
 Additionally, each account must also be initialized with the date when the account issues statements and the date when those statements are due.
 
 Following the addition of a new credit card, you will be redirected to a page displaying the account details, including all cards for that account.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/credit-account-details.png" alt="credit account details" width="800px" />
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/credit-account-details.png" alt="credit account details" width="800px" />
 
 Transactions can be added to each card using the 'Create a new transaction' links found on the 'Credit Cards' homepage panel.
 The link under the 'History' heading is a generic option that allows transactions to be created for any credit card in the system.
 If the card is already known, however, the 'Create a new transaction' links under the 'CARDS' section will prepopulate the transaction form to contain information for the desired card.
 
 In either case, you will move to a page where you can enter credit card transaction information.
 The interface for adding a transaction provides some convenient automatic features.
@@ -132,28 +135,28 @@
 These tags can generally be seen and managed from the 'Manage transaction tags' link off the app homepage.
 
 Since each transaction may consist of multiple components—each with it's own subtotal, notes, and tags—transactions can be split into subtransactions.
 Click the 'Add subtransaction' button on the transaction form to add a subtransaction.
 
 Once the transaction information has been successfully entered and submitted, the transaction will appear on the full transaction history page.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/credit-transactions.png" alt="transaction history" width="800px" />
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/credit-transactions.png" alt="transaction history" width="800px" />
 
 Card balances are also visible by visiting the pages for individual statements.
 A full history of statements for each card is available off the homepage.
 Each statement's page gives the statement's balance, transactions, and due date.
 
-<img src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/img/statement-details.png" alt="statement details" width="800px" />
+<img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/statement-details.png" alt="statement details" width="800px" />
 
 Payments can be made directly from a statement's page and can be linked to a bank account in the _Monopyly_ system for simplified tracking.
 (Note that even linked transactions must be edited independently, as there are times when a user may wish to have separate values for linked transactions. For example, a credit card payment may be processed on a given date while it is only registered as a bank account transaction several days later.)
 
 
 ## License
 
 This project is licensed under the GNU General Public License, Version 3.
-It is fully open-source, and while you are more than welcome to fork, add, modify, etc. it is required that you also keep those changes and additions open-source.
+It is fully open-source, and while you are more than welcome to fork, add, modify, etc. it is required that you keep any distributed changes and additions open-source.
 
 
 ## Changes
 
 Changes between versions are tracked in the [changelog](https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md).
```

