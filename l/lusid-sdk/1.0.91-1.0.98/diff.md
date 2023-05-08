# Comparing `tmp/lusid-sdk-1.0.91.tar.gz` & `tmp/lusid-sdk-1.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-sdk-1.0.91.tar", last modified: Fri Apr 21 11:00:47 2023, max compression
+gzip compressed data, was "dist/lusid-sdk-1.0.98.tar", last modified: Mon Apr 24 20:11:56 2023, max compression
```

## Comparing `lusid-sdk-1.0.91.tar` & `lusid-sdk-1.0.98.tar`

### file list

```diff
@@ -1,629 +1,629 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:47.031797 lusid-sdk-1.0.91/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-21 11:00:47.031797 lusid-sdk-1.0.91/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    95563 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:46.875796 lusid-sdk-1.0.91/lusid/
--rw-r--r--   0 root         (0) root         (0)    43051 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:46.881796 lusid-sdk-1.0.91/lusid/api/
--rw-r--r--   0 root         (0) root         (0)     2198 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31248 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/aggregation_api.py
--rw-r--r--   0 root         (0) root         (0)    39966 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/allocations_api.py
--rw-r--r--   0 root         (0) root         (0)    21670 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    38746 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/blocks_api.py
--rw-r--r--   0 root         (0) root         (0)   128587 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/calendars_api.py
--rw-r--r--   0 root         (0) root         (0)    37079 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/complex_market_data_api.py
--rw-r--r--   0 root         (0) root         (0)    37222 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/configuration_recipe_api.py
--rw-r--r--   0 root         (0) root         (0)    92916 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/corporate_action_sources_api.py
--rw-r--r--   0 root         (0) root         (0)    71078 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/counterparties_api.py
--rw-r--r--   0 root         (0) root         (0)   177517 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/custom_entities_api.py
--rw-r--r--   0 root         (0) root         (0)    36864 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/custom_entity_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    42662 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/cut_label_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    74825 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/data_types_api.py
--rw-r--r--   0 root         (0) root         (0)    21100 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/derived_transaction_portfolios_api.py
--rw-r--r--   0 root         (0) root         (0)    11463 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/entities_api.py
--rw-r--r--   0 root         (0) root         (0)    39316 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/executions_api.py
--rw-r--r--   0 root         (0) root         (0)   187527 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/instruments_api.py
--rw-r--r--   0 root         (0) root         (0)   246594 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/legal_entities_api.py
--rw-r--r--   0 root         (0) root         (0)    39239 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/orders_api.py
--rw-r--r--   0 root         (0) root         (0)    39890 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/participations_api.py
--rw-r--r--   0 root         (0) root         (0)   223059 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/persons_api.py
--rw-r--r--   0 root         (0) root         (0)    39318 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/placements_api.py
--rw-r--r--   0 root         (0) root         (0)   339276 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/portfolio_groups_api.py
--rw-r--r--   0 root         (0) root         (0)   297053 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/portfolios_api.py
--rw-r--r--   0 root         (0) root         (0)    71046 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/property_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    58376 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/quotes_api.py
--rw-r--r--   0 root         (0) root         (0)    70612 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/reconciliations_api.py
--rw-r--r--   0 root         (0) root         (0)    46624 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/reference_portfolio_api.py
--rw-r--r--   0 root         (0) root         (0)    51163 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/relationship_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    22586 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/relationships_api.py
--rw-r--r--   0 root         (0) root         (0)    27647 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/schemas_api.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/scopes_api.py
--rw-r--r--   0 root         (0) root         (0)    48100 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/search_api.py
--rw-r--r--   0 root         (0) root         (0)    39252 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/sequences_api.py
--rw-r--r--   0 root         (0) root         (0)    14427 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/system_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)   323847 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api/transaction_portfolios_api.py
--rw-r--r--   0 root         (0) root         (0)    27346 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16574 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:47.029796 lusid-sdk-1.0.91/lusid/models/
--rw-r--r--   0 root         (0) root         (0)    40149 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6341 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/a2_b_breakdown.py
--rw-r--r--   0 root         (0) root         (0)     5186 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/a2_b_category.py
--rw-r--r--   0 root         (0) root         (0)    17995 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/a2_b_data_record.py
--rw-r--r--   0 root         (0) root         (0)    21250 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/a2_b_movement_record.py
--rw-r--r--   0 root         (0) root         (0)     7105 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     8868 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     8024 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/access_metadata_operation.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/access_metadata_value.py
--rw-r--r--   0 root         (0) root         (0)     7199 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/action_result_of_portfolio.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/add_business_days_to_date_request.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/add_business_days_to_date_response.py
--rw-r--r--   0 root         (0) root         (0)    10981 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/address_definition.py
--rw-r--r--   0 root         (0) root         (0)     6299 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/address_key_filter.py
--rw-r--r--   0 root         (0) root         (0)     9173 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/address_key_option_definition.py
--rw-r--r--   0 root         (0) root         (0)     6833 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/adjust_holding.py
--rw-r--r--   0 root         (0) root         (0)    12009 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/adjust_holding_for_date_request.py
--rw-r--r--   0 root         (0) root         (0)    10263 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/adjust_holding_request.py
--rw-r--r--   0 root         (0) root         (0)     7501 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregate_spec.py
--rw-r--r--   0 root         (0) root         (0)    13025 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregated_return.py
--rw-r--r--   0 root         (0) root         (0)    13773 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregated_returns_request.py
--rw-r--r--   0 root         (0) root         (0)     6029 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregated_returns_response.py
--rw-r--r--   0 root         (0) root         (0)    10299 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregation_context.py
--rw-r--r--   0 root         (0) root         (0)     7086 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregation_measure_failure_detail.py
--rw-r--r--   0 root         (0) root         (0)     8776 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregation_options.py
--rw-r--r--   0 root         (0) root         (0)    25170 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/aggregation_query.py
--rw-r--r--   0 root         (0) root         (0)    24849 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/allocation.py
--rw-r--r--   0 root         (0) root         (0)    21189 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/allocation_request.py
--rw-r--r--   0 root         (0) root         (0)     4437 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/allocation_set_request.py
--rw-r--r--   0 root         (0) root         (0)    12995 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/amortisation_event.py
--rw-r--r--   0 root         (0) root         (0)    13135 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/amortisation_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7169 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/annul_quotes_response.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/annul_single_structured_data_response.py
--rw-r--r--   0 root         (0) root         (0)     7182 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/annul_structured_data_response.py
--rw-r--r--   0 root         (0) root         (0)     7903 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/barrier.py
--rw-r--r--   0 root         (0) root         (0)    10897 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/basket.py
--rw-r--r--   0 root         (0) root         (0)    10997 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/basket_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7621 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/basket_identifier.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/batch_adjust_holdings_response.py
--rw-r--r--   0 root         (0) root         (0)     7648 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/batch_upsert_portfolio_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)    18550 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/block.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/block_request.py
--rw-r--r--   0 root         (0) root         (0)     4110 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/block_set_request.py
--rw-r--r--   0 root         (0) root         (0)    23014 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/bond.py
--rw-r--r--   0 root         (0) root         (0)    23274 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/bond_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14818 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/bond_default_event.py
--rw-r--r--   0 root         (0) root         (0)    14978 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/bond_default_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)     9032 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/calendar.py
--rw-r--r--   0 root         (0) root         (0)    13375 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/calendar_date.py
--rw-r--r--   0 root         (0) root         (0)    13266 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cap_floor.py
--rw-r--r--   0 root         (0) root         (0)    13406 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cap_floor_all_of.py
--rw-r--r--   0 root         (0) root         (0)     9846 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_dividend_event.py
--rw-r--r--   0 root         (0) root         (0)     9946 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_dividend_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10170 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_event.py
--rw-r--r--   0 root         (0) root         (0)    10270 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10511 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_lineage.py
--rw-r--r--   0 root         (0) root         (0)    11250 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_value.py
--rw-r--r--   0 root         (0) root         (0)    11390 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_value_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6769 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_value_set.py
--rw-r--r--   0 root         (0) root         (0)     6829 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_flow_value_set_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6857 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_ladder_record.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_perpetual.py
--rw-r--r--   0 root         (0) root         (0)    10353 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cash_perpetual_all_of.py
--rw-r--r--   0 root         (0) root         (0)    24113 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cds_flow_conventions.py
--rw-r--r--   0 root         (0) root         (0)    17461 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cds_index.py
--rw-r--r--   0 root         (0) root         (0)    17661 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cds_index_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10138 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cds_protection_detail_specification.py
--rw-r--r--   0 root         (0) root         (0)    11016 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/change.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/change_history.py
--rw-r--r--   0 root         (0) root         (0)     8705 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/change_item.py
--rw-r--r--   0 root         (0) root         (0)     7847 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/close_event.py
--rw-r--r--   0 root         (0) root         (0)     7927 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/close_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    15718 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/complete_portfolio.py
--rw-r--r--   0 root         (0) root         (0)    14720 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/complete_relationship.py
--rw-r--r--   0 root         (0) root         (0)    11340 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/complex_bond.py
--rw-r--r--   0 root         (0) root         (0)    11440 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/complex_bond_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7097 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/complex_market_data.py
--rw-r--r--   0 root         (0) root         (0)    11522 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/complex_market_data_id.py
--rw-r--r--   0 root         (0) root         (0)    11638 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/compounding.py
--rw-r--r--   0 root         (0) root         (0)    14329 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/configuration_recipe.py
--rw-r--r--   0 root         (0) root         (0)    15248 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/configuration_recipe_snippet.py
--rw-r--r--   0 root         (0) root         (0)     6182 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/constituents_adjustment_header.py
--rw-r--r--   0 root         (0) root         (0)    19581 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/contract_for_difference.py
--rw-r--r--   0 root         (0) root         (0)    19801 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/contract_for_difference_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10864 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/corporate_action.py
--rw-r--r--   0 root         (0) root         (0)     9858 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/corporate_action_source.py
--rw-r--r--   0 root         (0) root         (0)     5719 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/corporate_action_transition.py
--rw-r--r--   0 root         (0) root         (0)    10626 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/corporate_action_transition_component.py
--rw-r--r--   0 root         (0) root         (0)     7358 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/corporate_action_transition_component_request.py
--rw-r--r--   0 root         (0) root         (0)     5647 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/corporate_action_transition_request.py
--rw-r--r--   0 root         (0) root         (0)    11823 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/counterparty_agreement.py
--rw-r--r--   0 root         (0) root         (0)     8525 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/counterparty_risk_information.py
--rw-r--r--   0 root         (0) root         (0)     6162 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/counterparty_signatory.py
--rw-r--r--   0 root         (0) root         (0)    10190 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_calendar_request.py
--rw-r--r--   0 root         (0) root         (0)    12687 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_corporate_action_source_request.py
--rw-r--r--   0 root         (0) root         (0)     9425 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_cut_label_definition_request.py
--rw-r--r--   0 root         (0) root         (0)    20418 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_data_type_request.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_date_request.py
--rw-r--r--   0 root         (0) root         (0)    15512 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_derived_property_definition_request.py
--rw-r--r--   0 root         (0) root         (0)    20648 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_derived_transaction_portfolio_request.py
--rw-r--r--   0 root         (0) root         (0)     4463 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_portfolio_details.py
--rw-r--r--   0 root         (0) root         (0)    12384 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_portfolio_group_request.py
--rw-r--r--   0 root         (0) root         (0)    17580 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_property_definition_request.py
--rw-r--r--   0 root         (0) root         (0)    11662 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_reference_portfolio_request.py
--rw-r--r--   0 root         (0) root         (0)    22107 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_relationship_definition_request.py
--rw-r--r--   0 root         (0) root         (0)    10114 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_relationship_request.py
--rw-r--r--   0 root         (0) root         (0)    11655 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_sequence_request.py
--rw-r--r--   0 root         (0) root         (0)    20654 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_transaction_portfolio_request.py
--rw-r--r--   0 root         (0) root         (0)     9311 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/create_unit_definition.py
--rw-r--r--   0 root         (0) root         (0)    18282 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/credit_default_swap.py
--rw-r--r--   0 root         (0) root         (0)    18482 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/credit_default_swap_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/credit_rating.py
--rw-r--r--   0 root         (0) root         (0)    17692 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/credit_spread_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    17912 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/credit_spread_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    20913 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/credit_support_annex.py
--rw-r--r--   0 root         (0) root         (0)     4643 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/currency_and_amount.py
--rw-r--r--   0 root         (0) root         (0)    15767 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custodian_account.py
--rw-r--r--   0 root         (0) root         (0)    11808 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_definition.py
--rw-r--r--   0 root         (0) root         (0)    10535 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     8071 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_field.py
--rw-r--r--   0 root         (0) root         (0)    11326 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_field_definition.py
--rw-r--r--   0 root         (0) root         (0)    12487 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_id.py
--rw-r--r--   0 root         (0) root         (0)     8386 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_request.py
--rw-r--r--   0 root         (0) root         (0)    13658 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/custom_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     8561 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cut_label_definition.py
--rw-r--r--   0 root         (0) root         (0)     4564 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/cut_local_time.py
--rw-r--r--   0 root         (0) root         (0)    15956 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/data_type.py
--rw-r--r--   0 root         (0) root         (0)    15139 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/data_type_summary.py
--rw-r--r--   0 root         (0) root         (0)    14148 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/date_attributes.py
--rw-r--r--   0 root         (0) root         (0)     4865 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/date_range.py
--rw-r--r--   0 root         (0) root         (0)     3459 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/day_of_week.py
--rw-r--r--   0 root         (0) root         (0)     5180 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/delete_instrument_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     6117 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/delete_instrument_response.py
--rw-r--r--   0 root         (0) root         (0)     6133 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/delete_instruments_response.py
--rw-r--r--   0 root         (0) root         (0)    10336 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/delete_relationship_request.py
--rw-r--r--   0 root         (0) root         (0)     7420 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     8388 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/dependency_source_filter.py
--rw-r--r--   0 root         (0) root         (0)    12366 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/discount_factor_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    12506 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/discount_factor_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)     5620 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/economic_dependency.py
--rw-r--r--   0 root         (0) root         (0)     6021 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/economic_dependency_with_complex_market_data.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/economic_dependency_with_quote.py
--rw-r--r--   0 root         (0) root         (0)     5399 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/empty_model_options.py
--rw-r--r--   0 root         (0) root         (0)     5439 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/empty_model_options_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/entity_identifier.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity.py
--rw-r--r--   0 root         (0) root         (0)     8658 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11925 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_all_of_identifiers.py
--rw-r--r--   0 root         (0) root         (0)    12573 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_curve_by_prices_data.py
--rw-r--r--   0 root         (0) root         (0)    12713 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_curve_by_prices_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7850 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_model_options.py
--rw-r--r--   0 root         (0) root         (0)     7910 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_model_options_all_of.py
--rw-r--r--   0 root         (0) root         (0)    24270 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_option.py
--rw-r--r--   0 root         (0) root         (0)    24570 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_option_all_of.py
--rw-r--r--   0 root         (0) root         (0)    23779 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_swap.py
--rw-r--r--   0 root         (0) root         (0)    24039 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_swap_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11232 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_vol_surface_data.py
--rw-r--r--   0 root         (0) root         (0)    11352 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/equity_vol_surface_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6807 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/error_detail.py
--rw-r--r--   0 root         (0) root         (0)     4532 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/event_date_range.py
--rw-r--r--   0 root         (0) root         (0)    11924 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exchange_traded_option.py
--rw-r--r--   0 root         (0) root         (0)    12044 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exchange_traded_option_all_of.py
--rw-r--r--   0 root         (0) root         (0)    23037 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exchange_traded_option_contract_details.py
--rw-r--r--   0 root         (0) root         (0)    24123 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/execution.py
--rw-r--r--   0 root         (0) root         (0)    21470 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/execution_request.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/execution_set_request.py
--rw-r--r--   0 root         (0) root         (0)    11001 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exercise_event.py
--rw-r--r--   0 root         (0) root         (0)    11121 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exercise_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10368 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exotic_instrument.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/exotic_instrument_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11175 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/expanded_group.py
--rw-r--r--   0 root         (0) root         (0)     6696 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/field_definition.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/field_schema.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/field_value.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/file_response.py
--rw-r--r--   0 root         (0) root         (0)    13199 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fixed_leg.py
--rw-r--r--   0 root         (0) root         (0)    13339 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fixed_leg_all_of.py
--rw-r--r--   0 root         (0) root         (0)     4916 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fixed_leg_all_of_overrides.py
--rw-r--r--   0 root         (0) root         (0)    13456 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/floating_leg.py
--rw-r--r--   0 root         (0) root         (0)    13596 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/floating_leg_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6593 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/flow_convention_name.py
--rw-r--r--   0 root         (0) root         (0)    26201 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/flow_conventions.py
--rw-r--r--   0 root         (0) root         (0)    15890 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/forward_rate_agreement.py
--rw-r--r--   0 root         (0) root         (0)    16070 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/forward_rate_agreement_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14096 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/funding_leg.py
--rw-r--r--   0 root         (0) root         (0)    14216 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/funding_leg_all_of.py
--rw-r--r--   0 root         (0) root         (0)    20280 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/future.py
--rw-r--r--   0 root         (0) root         (0)    20480 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/future_all_of.py
--rw-r--r--   0 root         (0) root         (0)    21010 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/futures_contract_details.py
--rw-r--r--   0 root         (0) root         (0)    20275 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward.py
--rw-r--r--   0 root         (0) root         (0)    20515 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_all_of.py
--rw-r--r--   0 root         (0) root         (0)    13820 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_curve_by_quote_reference.py
--rw-r--r--   0 root         (0) root         (0)    13980 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_curve_by_quote_reference_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14139 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    14319 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11328 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_model_options.py
--rw-r--r--   0 root         (0) root         (0)    11428 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_model_options_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_pips_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    14631 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_pips_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14327 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    14507 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14639 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_pips_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    14819 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_pips_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    28290 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_option.py
--rw-r--r--   0 root         (0) root         (0)    28650 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_option_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11104 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_swap.py
--rw-r--r--   0 root         (0) root         (0)    11204 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_swap_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11136 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/fx_vol_surface_data.py
--rw-r--r--   0 root         (0) root         (0)     7280 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_complex_market_data_response.py
--rw-r--r--   0 root         (0) root         (0)     7089 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_counterparty_agreement_response.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_credit_support_annex_response.py
--rw-r--r--   0 root         (0) root         (0)     7372 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_instruments_response.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_quotes_response.py
--rw-r--r--   0 root         (0) root         (0)     5690 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_recipe_response.py
--rw-r--r--   0 root         (0) root         (0)    12031 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/get_reference_portfolio_constituents_response.py
--rw-r--r--   0 root         (0) root         (0)    12536 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/holding_adjustment.py
--rw-r--r--   0 root         (0) root         (0)    13890 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/holding_adjustment_with_date.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/holding_context.py
--rw-r--r--   0 root         (0) root         (0)    10492 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/holdings_adjustment.py
--rw-r--r--   0 root         (0) root         (0)     9375 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/holdings_adjustment_header.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/i_data_record.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/i_unit_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)     7950 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9439 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)    18220 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/index_convention.py
--rw-r--r--   0 root         (0) root         (0)     7151 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/index_model_options.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/index_model_options_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7582 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/industry_classifier.py
--rw-r--r--   0 root         (0) root         (0)    36403 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/inflation_linked_bond.py
--rw-r--r--   0 root         (0) root         (0)    36803 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/inflation_linked_bond_all_of.py
--rw-r--r--   0 root         (0) root         (0)    25417 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/inflation_swap.py
--rw-r--r--   0 root         (0) root         (0)    25717 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/inflation_swap_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10091 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/informational_error_event.py
--rw-r--r--   0 root         (0) root         (0)    10191 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/informational_error_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    13186 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/informational_event.py
--rw-r--r--   0 root         (0) root         (0)    13326 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/informational_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    22491 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/inline_valuation_request.py
--rw-r--r--   0 root         (0) root         (0)     8211 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/inline_valuations_reconciliation_request.py
--rw-r--r--   0 root         (0) root         (0)     5482 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/input_transition.py
--rw-r--r--   0 root         (0) root         (0)    19962 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument.py
--rw-r--r--   0 root         (0) root         (0)     9471 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_definition.py
--rw-r--r--   0 root         (0) root         (0)     8349 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_definition_format.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_event.py
--rw-r--r--   0 root         (0) root         (0)    17158 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_event_holder.py
--rw-r--r--   0 root         (0) root         (0)     7701 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_id_type_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     5729 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_id_value.py
--rw-r--r--   0 root         (0) root         (0)     7217 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_leg.py
--rw-r--r--   0 root         (0) root         (0)     6782 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_leg_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6119 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_match.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_models.py
--rw-r--r--   0 root         (0) root         (0)     6890 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_properties.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/instrument_search_property.py
--rw-r--r--   0 root         (0) root         (0)    14360 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/interest_rate_swap.py
--rw-r--r--   0 root         (0) root         (0)    14500 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/interest_rate_swap_all_of.py
--rw-r--r--   0 root         (0) root         (0)    13593 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/interest_rate_swaption.py
--rw-r--r--   0 root         (0) root         (0)    13733 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/interest_rate_swaption_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11121 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/ir_vol_cube_data.py
--rw-r--r--   0 root         (0) root         (0)    11241 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/ir_vol_cube_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)     5576 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/is_business_day_response.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/label_value_set.py
--rw-r--r--   0 root         (0) root         (0)    17096 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/leg_definition.py
--rw-r--r--   0 root         (0) root         (0)    13347 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/legal_entity.py
--rw-r--r--   0 root         (0) root         (0)     5401 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/level_step.py
--rw-r--r--   0 root         (0) root         (0)     8321 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/life_cycle_event_lineage.py
--rw-r--r--   0 root         (0) root         (0)     8842 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/life_cycle_event_value.py
--rw-r--r--   0 root         (0) root         (0)     8942 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/life_cycle_event_value_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6624 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/list_aggregation_reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    10737 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/list_aggregation_response.py
--rw-r--r--   0 root         (0) root         (0)     6196 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/loan_period.py
--rw-r--r--   0 root         (0) root         (0)     8275 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/lusid_instrument.py
--rw-r--r--   0 root         (0) root         (0)     9507 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/lusid_unique_id.py
--rw-r--r--   0 root         (0) root         (0)    10707 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     6590 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/mapped_string.py
--rw-r--r--   0 root         (0) root         (0)    10566 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/mapping.py
--rw-r--r--   0 root         (0) root         (0)    10471 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/mapping_rule.py
--rw-r--r--   0 root         (0) root         (0)     9381 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_context.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_context_suppliers.py
--rw-r--r--   0 root         (0) root         (0)    26173 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_data_key_rule.py
--rw-r--r--   0 root         (0) root         (0)     5453 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_data_options.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_data_overrides.py
--rw-r--r--   0 root         (0) root         (0)    23810 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_data_specific_rule.py
--rw-r--r--   0 root         (0) root         (0)    14881 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_options.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/market_quote.py
--rw-r--r--   0 root         (0) root         (0)     4610 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/metric_value.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/model_options.py
--rw-r--r--   0 root         (0) root         (0)     7701 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/model_property.py
--rw-r--r--   0 root         (0) root         (0)     7506 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/model_selection.py
--rw-r--r--   0 root         (0) root         (0)     5120 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/next_value_in_sequence_response.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/opaque_market_data.py
--rw-r--r--   0 root         (0) root         (0)    12085 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/opaque_market_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/opaque_model_options.py
--rw-r--r--   0 root         (0) root         (0)     6368 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/opaque_model_options_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/open_event.py
--rw-r--r--   0 root         (0) root         (0)     6956 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/open_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/operation.py
--rw-r--r--   0 root         (0) root         (0)    22328 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/order.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/order_by_spec.py
--rw-r--r--   0 root         (0) root         (0)    18584 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/order_request.py
--rw-r--r--   0 root         (0) root         (0)     4247 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/order_set_request.py
--rw-r--r--   0 root         (0) root         (0)     4384 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/otc_confirmation.py
--rw-r--r--   0 root         (0) root         (0)    33019 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/output_transaction.py
--rw-r--r--   0 root         (0) root         (0)    10333 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/output_transition.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_allocation.py
--rw-r--r--   0 root         (0) root         (0)     7246 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_block.py
--rw-r--r--   0 root         (0) root         (0)     7330 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_calendar.py
--rw-r--r--   0 root         (0) root         (0)     7694 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_corporate_action_source.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_custom_entity_definition.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_custom_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     7610 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_cut_label_definition.py
--rw-r--r--   0 root         (0) root         (0)     7526 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_data_type_summary.py
--rw-r--r--   0 root         (0) root         (0)     7358 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_execution.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_instrument.py
--rw-r--r--   0 root         (0) root         (0)     7694 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_instrument_event_holder.py
--rw-r--r--   0 root         (0) root         (0)     7414 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_legal_entity.py
--rw-r--r--   0 root         (0) root         (0)     7246 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_order.py
--rw-r--r--   0 root         (0) root         (0)     7470 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_participation.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_person.py
--rw-r--r--   0 root         (0) root         (0)     7358 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_placement.py
--rw-r--r--   0 root         (0) root         (0)     7834 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_portfolio_group_search_result.py
--rw-r--r--   0 root         (0) root         (0)     7694 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_portfolio_search_result.py
--rw-r--r--   0 root         (0) root         (0)     7946 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_property_definition_search_result.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_relationship_definition.py
--rw-r--r--   0 root         (0) root         (0)     7610 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_sequence_definition.py
--rw-r--r--   0 root         (0) root         (0)     7483 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/participation.py
--rw-r--r--   0 root         (0) root         (0)     6927 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/participation_request.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/participation_set_request.py
--rw-r--r--   0 root         (0) root         (0)     8789 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/performance_return.py
--rw-r--r--   0 root         (0) root         (0)    10182 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/performance_returns_metric.py
--rw-r--r--   0 root         (0) root         (0)     5214 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/perpetual_property.py
--rw-r--r--   0 root         (0) root         (0)    11044 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/person.py
--rw-r--r--   0 root         (0) root         (0)    24250 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/placement.py
--rw-r--r--   0 root         (0) root         (0)    22675 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/placement_request.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/placement_set_request.py
--rw-r--r--   0 root         (0) root         (0)    21170 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio.py
--rw-r--r--   0 root         (0) root         (0)    23701 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_cash_flow.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_cash_ladder.py
--rw-r--r--   0 root         (0) root         (0)    15148 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_details.py
--rw-r--r--   0 root         (0) root         (0)     8461 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_entity_id.py
--rw-r--r--   0 root         (0) root         (0)    13608 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_group.py
--rw-r--r--   0 root         (0) root         (0)     6997 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_group_properties.py
--rw-r--r--   0 root         (0) root         (0)    12954 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_group_search_result.py
--rw-r--r--   0 root         (0) root         (0)    17792 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_holding.py
--rw-r--r--   0 root         (0) root         (0)     6864 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_properties.py
--rw-r--r--   0 root         (0) root         (0)     6776 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_reconciliation_request.py
--rw-r--r--   0 root         (0) root         (0)    17337 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_result_data_key_rule.py
--rw-r--r--   0 root         (0) root         (0)    17517 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_result_data_key_rule_all_of.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolio_search_result.py
--rw-r--r--   0 root         (0) root         (0)     7198 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/portfolios_reconciliation_request.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/premium.py
--rw-r--r--   0 root         (0) root         (0)     9446 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/pricing_context.py
--rw-r--r--   0 root         (0) root         (0)    27515 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/pricing_options.py
--rw-r--r--   0 root         (0) root         (0)     7871 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/processed_command.py
--rw-r--r--   0 root         (0) root         (0)    27011 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/property_definition.py
--rw-r--r--   0 root         (0) root         (0)    27875 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/property_definition_search_result.py
--rw-r--r--   0 root         (0) root         (0)     7836 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/property_filter.py
--rw-r--r--   0 root         (0) root         (0)     7970 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/property_interval.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/property_schema.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/property_value.py
--rw-r--r--   0 root         (0) root         (0)    10796 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/quote.py
--rw-r--r--   0 root         (0) root         (0)     5784 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/quote_id.py
--rw-r--r--   0 root         (0) root         (0)    14722 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/quote_series_id.py
--rw-r--r--   0 root         (0) root         (0)    11312 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/raw_vendor_event.py
--rw-r--r--   0 root         (0) root         (0)    11432 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/raw_vendor_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    17981 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/realised_gain_loss.py
--rw-r--r--   0 root         (0) root         (0)     9884 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconcile_date_time_rule.py
--rw-r--r--   0 root         (0) root         (0)     9984 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconcile_date_time_rule_all_of.py
--rw-r--r--   0 root         (0) root         (0)     9946 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconcile_numeric_rule.py
--rw-r--r--   0 root         (0) root         (0)    10046 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconcile_numeric_rule_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10717 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconcile_string_rule.py
--rw-r--r--   0 root         (0) root         (0)    10817 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconcile_string_rule_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7789 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciled_transaction.py
--rw-r--r--   0 root         (0) root         (0)    15669 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciliation_break.py
--rw-r--r--   0 root         (0) root         (0)     5469 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciliation_left_right_address_key_pair.py
--rw-r--r--   0 root         (0) root         (0)     7308 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciliation_line.py
--rw-r--r--   0 root         (0) root         (0)    10384 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciliation_request.py
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciliation_response.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reconciliation_rule.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reference_data.py
--rw-r--r--   0 root         (0) root         (0)    11182 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reference_instrument.py
--rw-r--r--   0 root         (0) root         (0)    11282 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reference_instrument_all_of.py
--rw-r--r--   0 root         (0) root         (0)    11193 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reference_portfolio_constituent.py
--rw-r--r--   0 root         (0) root         (0)     7557 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reference_portfolio_constituent_request.py
--rw-r--r--   0 root         (0) root         (0)    12678 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/related_entity.py
--rw-r--r--   0 root         (0) root         (0)    10236 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/relation.py
--rw-r--r--   0 root         (0) root         (0)    13987 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/relationship.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/relationship_definition.py
--rw-r--r--   0 root         (0) root         (0)    25647 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/repo.py
--rw-r--r--   0 root         (0) root         (0)    25907 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/repo_all_of.py
--rw-r--r--   0 root         (0) root         (0)    12034 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reset_event.py
--rw-r--r--   0 root         (0) root         (0)    12174 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/reset_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7658 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7572 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_access_metadata_value_of.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_aggregation_query.py
--rw-r--r--   0 root         (0) root         (0)     7266 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_allocation.py
--rw-r--r--   0 root         (0) root         (0)     7126 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_block.py
--rw-r--r--   0 root         (0) root         (0)     7322 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_calendar_date.py
--rw-r--r--   0 root         (0) root         (0)     7154 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_change.py
--rw-r--r--   0 root         (0) root         (0)     7350 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_change_history.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_constituents_adjustment_header.py
--rw-r--r--   0 root         (0) root         (0)     7406 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_corporate_action.py
--rw-r--r--   0 root         (0) root         (0)     7210 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_data_type.py
--rw-r--r--   0 root         (0) root         (0)     7238 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_execution.py
--rw-r--r--   0 root         (0) root         (0)     7882 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_get_counterparty_agreement_response.py
--rw-r--r--   0 root         (0) root         (0)     7798 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_get_credit_support_annex_response.py
--rw-r--r--   0 root         (0) root         (0)     7462 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_get_recipe_response.py
--rw-r--r--   0 root         (0) root         (0)     7658 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_holdings_adjustment_header.py
--rw-r--r--   0 root         (0) root         (0)     7490 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_i_unit_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)     7714 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_instrument_id_type_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     7294 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_legal_entity.py
--rw-r--r--   0 root         (0) root         (0)     7182 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_mapping.py
--rw-r--r--   0 root         (0) root         (0)     7126 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_order.py
--rw-r--r--   0 root         (0) root         (0)     7350 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_participation.py
--rw-r--r--   0 root         (0) root         (0)     7462 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_performance_return.py
--rw-r--r--   0 root         (0) root         (0)     7154 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_person.py
--rw-r--r--   0 root         (0) root         (0)     7238 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_placement.py
--rw-r--r--   0 root         (0) root         (0)     7238 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio.py
--rw-r--r--   0 root         (0) root         (0)     7462 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio_cash_flow.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio_cash_ladder.py
--rw-r--r--   0 root         (0) root         (0)     7378 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio_group.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_processed_command.py
--rw-r--r--   0 root         (0) root         (0)     7230 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_property.py
--rw-r--r--   0 root         (0) root         (0)     7490 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_property_definition.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_property_interval.py
--rw-r--r--   0 root         (0) root         (0)     7126 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_quote.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_reconciliation_break.py
--rw-r--r--   0 root         (0) root         (0)     7210 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_relation.py
--rw-r--r--   0 root         (0) root         (0)     7322 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_relationship.py
--rw-r--r--   0 root         (0) root         (0)     7406 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_scope_definition.py
--rw-r--r--   0 root         (0) root         (0)     7124 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_string.py
--rw-r--r--   0 root         (0) root         (0)     7238 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/resource_list_of_value_type.py
--rw-r--r--   0 root         (0) root         (0)     7132 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/response_meta_data.py
--rw-r--r--   0 root         (0) root         (0)    16885 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_data_key_rule.py
--rw-r--r--   0 root         (0) root         (0)    17065 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_data_key_rule_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_data_schema.py
--rw-r--r--   0 root         (0) root         (0)     5594 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_key_rule.py
--rw-r--r--   0 root         (0) root         (0)     6668 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value.py
--rw-r--r--   0 root         (0) root         (0)     8573 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value0_d.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value0_d_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_bool.py
--rw-r--r--   0 root         (0) root         (0)     6624 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_bool_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_currency.py
--rw-r--r--   0 root         (0) root         (0)     6634 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_currency_all_of.py
--rw-r--r--   0 root         (0) root         (0)     8005 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_date_time_offset.py
--rw-r--r--   0 root         (0) root         (0)     8085 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_date_time_offset_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7881 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_decimal.py
--rw-r--r--   0 root         (0) root         (0)     7961 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_decimal_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6782 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_dictionary.py
--rw-r--r--   0 root         (0) root         (0)     6842 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_dictionary_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7809 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_int.py
--rw-r--r--   0 root         (0) root         (0)     7889 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_int_all_of.py
--rw-r--r--   0 root         (0) root         (0)     6550 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_string.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/result_value_string_all_of.py
--rw-r--r--   0 root         (0) root         (0)     5299 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/schedule.py
--rw-r--r--   0 root         (0) root         (0)     5783 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/schema.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/scope_definition.py
--rw-r--r--   0 root         (0) root         (0)    12313 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/sequence_definition.py
--rw-r--r--   0 root         (0) root         (0)     4546 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/set_legal_entity_identifiers_request.py
--rw-r--r--   0 root         (0) root         (0)     4698 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/set_legal_entity_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     4488 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/set_person_identifiers_request.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/set_person_properties_request.py
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/side_configuration_data.py
--rw-r--r--   0 root         (0) root         (0)    12731 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/simple_cash_flow_loan.py
--rw-r--r--   0 root         (0) root         (0)    12851 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/simple_cash_flow_loan_all_of.py
--rw-r--r--   0 root         (0) root         (0)    14542 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/simple_instrument.py
--rw-r--r--   0 root         (0) root         (0)    14682 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/simple_instrument_all_of.py
--rw-r--r--   0 root         (0) root         (0)     9597 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/step_schedule.py
--rw-r--r--   0 root         (0) root         (0)     9697 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/step_schedule_all_of.py
--rw-r--r--   0 root         (0) root         (0)    10120 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/stock_split_event.py
--rw-r--r--   0 root         (0) root         (0)    10220 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/stock_split_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)     9230 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/stream.py
--rw-r--r--   0 root         (0) root         (0)     9014 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/supported_analytics_internal_request.py
--rw-r--r--   0 root         (0) root         (0)     9502 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/target_tax_lot.py
--rw-r--r--   0 root         (0) root         (0)     9698 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/target_tax_lot_request.py
--rw-r--r--   0 root         (0) root         (0)    18213 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/term_deposit.py
--rw-r--r--   0 root         (0) root         (0)    18373 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/term_deposit_all_of.py
--rw-r--r--   0 root         (0) root         (0)     7854 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/touch.py
--rw-r--r--   0 root         (0) root         (0)    30339 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7084 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_configuration_data.py
--rw-r--r--   0 root         (0) root         (0)     7209 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_configuration_data_request.py
--rw-r--r--   0 root         (0) root         (0)    15021 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_configuration_movement_data.py
--rw-r--r--   0 root         (0) root         (0)    13935 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_configuration_movement_data_request.py
--rw-r--r--   0 root         (0) root         (0)    14165 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_configuration_type_alias.py
--rw-r--r--   0 root         (0) root         (0)     5084 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_price.py
--rw-r--r--   0 root         (0) root         (0)     6460 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_property_mapping.py
--rw-r--r--   0 root         (0) root         (0)     6569 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_property_mapping_request.py
--rw-r--r--   0 root         (0) root         (0)     9882 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_query_parameters.py
--rw-r--r--   0 root         (0) root         (0)    11042 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_reconciliation_request.py
--rw-r--r--   0 root         (0) root         (0)    25204 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_request.py
--rw-r--r--   0 root         (0) root         (0)     6796 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transaction_set_configuration_data.py
--rw-r--r--   0 root         (0) root         (0)     5077 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transactions_reconciliations_response.py
--rw-r--r--   0 root         (0) root         (0)    12320 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transition_event.py
--rw-r--r--   0 root         (0) root         (0)    12480 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/transition_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)    12564 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/trigger_event.py
--rw-r--r--   0 root         (0) root         (0)    12704 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/trigger_event_all_of.py
--rw-r--r--   0 root         (0) root         (0)     9766 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/typed_resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7390 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_calendar_request.py
--rw-r--r--   0 root         (0) root         (0)     8385 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_custom_entity_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     8528 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_cut_label_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     9294 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_data_type_request.py
--rw-r--r--   0 root         (0) root         (0)     9254 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_derived_property_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     7188 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_instrument_identifier_request.py
--rw-r--r--   0 root         (0) root         (0)     5733 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_portfolio_group_request.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_portfolio_request.py
--rw-r--r--   0 root         (0) root         (0)     6202 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_property_definition_request.py
--rw-r--r--   0 root         (0) root         (0)    10185 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_relationship_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     7869 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/update_unit_request.py
--rw-r--r--   0 root         (0) root         (0)     5592 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_complex_market_data_request.py
--rw-r--r--   0 root         (0) root         (0)    13957 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_corporate_action_request.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_corporate_actions_response.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_counterparty_agreement_request.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_credit_support_annex_request.py
--rw-r--r--   0 root         (0) root         (0)     7424 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_custom_entities_response.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_custom_entity_access_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)    11531 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_instrument_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_instrument_events_response.py
--rw-r--r--   0 root         (0) root         (0)     5337 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_instrument_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     7967 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_instrument_property_request.py
--rw-r--r--   0 root         (0) root         (0)     8363 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_instruments_response.py
--rw-r--r--   0 root         (0) root         (0)     7362 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_legal_entities_response.py
--rw-r--r--   0 root         (0) root         (0)     4481 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_legal_entity_access_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)    11116 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_legal_entity_request.py
--rw-r--r--   0 root         (0) root         (0)     4423 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_person_access_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     9118 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_person_request.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_portfolio_access_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     4711 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_portfolio_group_access_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     7447 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_portfolio_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)     7603 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_quote_request.py
--rw-r--r--   0 root         (0) root         (0)     7045 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_quotes_response.py
--rw-r--r--   0 root         (0) root         (0)     5701 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_recipe_request.py
--rw-r--r--   0 root         (0) root         (0)    10646 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_reference_portfolio_constituents_request.py
--rw-r--r--   0 root         (0) root         (0)     5745 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_reference_portfolio_constituents_response.py
--rw-r--r--   0 root         (0) root         (0)     8082 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_returns_response.py
--rw-r--r--   0 root         (0) root         (0)     6073 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_single_structured_data_response.py
--rw-r--r--   0 root         (0) root         (0)     7226 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_structured_data_response.py
--rw-r--r--   0 root         (0) root         (0)     6949 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/upsert_transaction_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/user.py
--rw-r--r--   0 root         (0) root         (0)    21406 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/valuation_request.py
--rw-r--r--   0 root         (0) root         (0)    13909 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/valuation_schedule.py
--rw-r--r--   0 root         (0) root         (0)     8628 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/valuations_reconciliation_request.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/value_type.py
--rw-r--r--   0 root         (0) root         (0)    15640 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/vendor_model_rule.py
--rw-r--r--   0 root         (0) root         (0)    11535 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/version.py
--rw-r--r--   0 root         (0) root         (0)     6389 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/version_summary_dto.py
--rw-r--r--   0 root         (0) root         (0)     8592 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_a2_b_data_record.py
--rw-r--r--   0 root         (0) root         (0)     8720 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_a2_b_movement_record.py
--rw-r--r--   0 root         (0) root         (0)     8720 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_output_transaction.py
--rw-r--r--   0 root         (0) root         (0)     8688 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_portfolio_holding.py
--rw-r--r--   0 root         (0) root         (0)     8528 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_transaction.py
--rw-r--r--   0 root         (0) root         (0)     5794 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/weekend_mask.py
--rw-r--r--   0 root         (0) root         (0)     8442 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/weighted_instrument.py
--rw-r--r--   0 root         (0) root         (0)     4480 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/weighted_instruments.py
--rw-r--r--   0 root         (0) root         (0)    12115 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/yield_curve_data.py
--rw-r--r--   0 root         (0) root         (0)    12255 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/models/yield_curve_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    13518 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:47.029796 lusid-sdk-1.0.91/lusid/tcp/
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5321 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/tcp/tcp_keep_alive_probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:47.030796 lusid-sdk-1.0.91/lusid/utilities/
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/api_client_builder.py
--rw-r--r--   0 root         (0) root         (0)     5397 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/api_client_factory.py
--rw-r--r--   0 root         (0) root         (0)     3970 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/api_configuration.py
--rw-r--r--   0 root         (0) root         (0)     4065 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/api_configuration_loader.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)     1236 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/lusid_retry.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/proxy_config.py
--rw-r--r--   0 root         (0) root         (0)     9701 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/lusid/utilities/refreshing_token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:00:47.030796 lusid-sdk-1.0.91/lusid_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-21 11:00:46.000000 lusid-sdk-1.0.91/lusid_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24459 2023-04-21 11:00:46.000000 lusid-sdk-1.0.91/lusid_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 11:00:46.000000 lusid-sdk-1.0.91/lusid_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-04-21 11:00:46.000000 lusid-sdk-1.0.91/lusid_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-21 11:00:46.000000 lusid-sdk-1.0.91/lusid_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 11:00:47.031797 lusid-sdk-1.0.91/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2211 2023-04-21 10:39:12.000000 lusid-sdk-1.0.91/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.746071 lusid-sdk-1.0.98/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-24 20:11:56.746071 lusid-sdk-1.0.98/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    95563 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.686071 lusid-sdk-1.0.98/lusid/
+-rw-r--r--   0 root         (0) root         (0)    43051 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.691071 lusid-sdk-1.0.98/lusid/api/
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31248 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/aggregation_api.py
+-rw-r--r--   0 root         (0) root         (0)    39966 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/allocations_api.py
+-rw-r--r--   0 root         (0) root         (0)    21670 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    38746 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/blocks_api.py
+-rw-r--r--   0 root         (0) root         (0)   128587 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/calendars_api.py
+-rw-r--r--   0 root         (0) root         (0)    37079 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/complex_market_data_api.py
+-rw-r--r--   0 root         (0) root         (0)    37222 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/configuration_recipe_api.py
+-rw-r--r--   0 root         (0) root         (0)    92916 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/corporate_action_sources_api.py
+-rw-r--r--   0 root         (0) root         (0)    71078 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/counterparties_api.py
+-rw-r--r--   0 root         (0) root         (0)   177517 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/custom_entities_api.py
+-rw-r--r--   0 root         (0) root         (0)    36864 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/custom_entity_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    42662 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/cut_label_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    74825 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/data_types_api.py
+-rw-r--r--   0 root         (0) root         (0)    21100 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/derived_transaction_portfolios_api.py
+-rw-r--r--   0 root         (0) root         (0)    11463 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/entities_api.py
+-rw-r--r--   0 root         (0) root         (0)    39316 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/executions_api.py
+-rw-r--r--   0 root         (0) root         (0)   187527 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/instruments_api.py
+-rw-r--r--   0 root         (0) root         (0)   246594 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/legal_entities_api.py
+-rw-r--r--   0 root         (0) root         (0)    39239 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/orders_api.py
+-rw-r--r--   0 root         (0) root         (0)    39890 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/participations_api.py
+-rw-r--r--   0 root         (0) root         (0)   223059 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/persons_api.py
+-rw-r--r--   0 root         (0) root         (0)    39318 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/placements_api.py
+-rw-r--r--   0 root         (0) root         (0)   339276 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/portfolio_groups_api.py
+-rw-r--r--   0 root         (0) root         (0)   297053 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/portfolios_api.py
+-rw-r--r--   0 root         (0) root         (0)    71046 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/property_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    58376 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/quotes_api.py
+-rw-r--r--   0 root         (0) root         (0)    70612 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/reconciliations_api.py
+-rw-r--r--   0 root         (0) root         (0)    46624 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/reference_portfolio_api.py
+-rw-r--r--   0 root         (0) root         (0)    51163 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/relationship_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    22586 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/relationships_api.py
+-rw-r--r--   0 root         (0) root         (0)    27647 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/schemas_api.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/scopes_api.py
+-rw-r--r--   0 root         (0) root         (0)    48100 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/search_api.py
+-rw-r--r--   0 root         (0) root         (0)    39252 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/sequences_api.py
+-rw-r--r--   0 root         (0) root         (0)    14427 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/system_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)   323847 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api/transaction_portfolios_api.py
+-rw-r--r--   0 root         (0) root         (0)    27346 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16574 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.744071 lusid-sdk-1.0.98/lusid/models/
+-rw-r--r--   0 root         (0) root         (0)    40149 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6341 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/a2_b_breakdown.py
+-rw-r--r--   0 root         (0) root         (0)     5186 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/a2_b_category.py
+-rw-r--r--   0 root         (0) root         (0)    17995 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/a2_b_data_record.py
+-rw-r--r--   0 root         (0) root         (0)    21250 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/a2_b_movement_record.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     8868 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     8024 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/access_metadata_operation.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/access_metadata_value.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/action_result_of_portfolio.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/add_business_days_to_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/add_business_days_to_date_response.py
+-rw-r--r--   0 root         (0) root         (0)    10981 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/address_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/address_key_filter.py
+-rw-r--r--   0 root         (0) root         (0)     9173 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/address_key_option_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6833 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/adjust_holding.py
+-rw-r--r--   0 root         (0) root         (0)    12009 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/adjust_holding_for_date_request.py
+-rw-r--r--   0 root         (0) root         (0)    10263 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/adjust_holding_request.py
+-rw-r--r--   0 root         (0) root         (0)     7501 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregate_spec.py
+-rw-r--r--   0 root         (0) root         (0)    13025 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregated_return.py
+-rw-r--r--   0 root         (0) root         (0)    13773 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregated_returns_request.py
+-rw-r--r--   0 root         (0) root         (0)     6029 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregated_returns_response.py
+-rw-r--r--   0 root         (0) root         (0)    10299 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregation_context.py
+-rw-r--r--   0 root         (0) root         (0)     7086 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregation_measure_failure_detail.py
+-rw-r--r--   0 root         (0) root         (0)     8776 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregation_options.py
+-rw-r--r--   0 root         (0) root         (0)    25170 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/aggregation_query.py
+-rw-r--r--   0 root         (0) root         (0)    24849 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/allocation.py
+-rw-r--r--   0 root         (0) root         (0)    21189 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/allocation_request.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/allocation_set_request.py
+-rw-r--r--   0 root         (0) root         (0)    12995 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/amortisation_event.py
+-rw-r--r--   0 root         (0) root         (0)    13135 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/amortisation_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7169 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/annul_quotes_response.py
+-rw-r--r--   0 root         (0) root         (0)     6066 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/annul_single_structured_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     7182 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/annul_structured_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     7903 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/barrier.py
+-rw-r--r--   0 root         (0) root         (0)    10897 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/basket.py
+-rw-r--r--   0 root         (0) root         (0)    10997 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/basket_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/basket_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/batch_adjust_holdings_response.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/batch_upsert_portfolio_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)    18550 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/block.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/block_request.py
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/block_set_request.py
+-rw-r--r--   0 root         (0) root         (0)    23014 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/bond.py
+-rw-r--r--   0 root         (0) root         (0)    23274 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/bond_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14818 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/bond_default_event.py
+-rw-r--r--   0 root         (0) root         (0)    14978 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/bond_default_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     9032 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/calendar.py
+-rw-r--r--   0 root         (0) root         (0)    13375 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/calendar_date.py
+-rw-r--r--   0 root         (0) root         (0)    13266 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cap_floor.py
+-rw-r--r--   0 root         (0) root         (0)    13406 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cap_floor_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_dividend_event.py
+-rw-r--r--   0 root         (0) root         (0)     9946 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_dividend_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10170 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_event.py
+-rw-r--r--   0 root         (0) root         (0)    10270 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10511 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_lineage.py
+-rw-r--r--   0 root         (0) root         (0)    11250 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_value.py
+-rw-r--r--   0 root         (0) root         (0)    11390 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_value_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6769 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_value_set.py
+-rw-r--r--   0 root         (0) root         (0)     6829 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_flow_value_set_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6857 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_ladder_record.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_perpetual.py
+-rw-r--r--   0 root         (0) root         (0)    10353 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cash_perpetual_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    24113 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cds_flow_conventions.py
+-rw-r--r--   0 root         (0) root         (0)    17461 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cds_index.py
+-rw-r--r--   0 root         (0) root         (0)    17661 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cds_index_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10138 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cds_protection_detail_specification.py
+-rw-r--r--   0 root         (0) root         (0)    11016 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/change.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/change_history.py
+-rw-r--r--   0 root         (0) root         (0)     8705 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/change_item.py
+-rw-r--r--   0 root         (0) root         (0)     7847 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/close_event.py
+-rw-r--r--   0 root         (0) root         (0)     7927 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/close_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    15718 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/complete_portfolio.py
+-rw-r--r--   0 root         (0) root         (0)    14720 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/complete_relationship.py
+-rw-r--r--   0 root         (0) root         (0)    11340 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/complex_bond.py
+-rw-r--r--   0 root         (0) root         (0)    11440 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/complex_bond_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7097 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/complex_market_data.py
+-rw-r--r--   0 root         (0) root         (0)    11522 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/complex_market_data_id.py
+-rw-r--r--   0 root         (0) root         (0)    11638 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/compounding.py
+-rw-r--r--   0 root         (0) root         (0)    14329 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/configuration_recipe.py
+-rw-r--r--   0 root         (0) root         (0)    15248 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/configuration_recipe_snippet.py
+-rw-r--r--   0 root         (0) root         (0)     6182 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/constituents_adjustment_header.py
+-rw-r--r--   0 root         (0) root         (0)    19581 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/contract_for_difference.py
+-rw-r--r--   0 root         (0) root         (0)    19801 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/contract_for_difference_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10864 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/corporate_action.py
+-rw-r--r--   0 root         (0) root         (0)     9858 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/corporate_action_source.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/corporate_action_transition.py
+-rw-r--r--   0 root         (0) root         (0)    10626 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/corporate_action_transition_component.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/corporate_action_transition_component_request.py
+-rw-r--r--   0 root         (0) root         (0)     5647 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/corporate_action_transition_request.py
+-rw-r--r--   0 root         (0) root         (0)    11823 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/counterparty_agreement.py
+-rw-r--r--   0 root         (0) root         (0)     8525 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/counterparty_risk_information.py
+-rw-r--r--   0 root         (0) root         (0)     6162 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/counterparty_signatory.py
+-rw-r--r--   0 root         (0) root         (0)    10190 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_calendar_request.py
+-rw-r--r--   0 root         (0) root         (0)    12687 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_corporate_action_source_request.py
+-rw-r--r--   0 root         (0) root         (0)     9425 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_cut_label_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)    20418 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_data_type_request.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_date_request.py
+-rw-r--r--   0 root         (0) root         (0)    15512 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_derived_property_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)    20648 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_derived_transaction_portfolio_request.py
+-rw-r--r--   0 root         (0) root         (0)     4463 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_portfolio_details.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_portfolio_group_request.py
+-rw-r--r--   0 root         (0) root         (0)    17580 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_property_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_reference_portfolio_request.py
+-rw-r--r--   0 root         (0) root         (0)    22107 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_relationship_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)    10114 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_relationship_request.py
+-rw-r--r--   0 root         (0) root         (0)    11655 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_sequence_request.py
+-rw-r--r--   0 root         (0) root         (0)    20654 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_transaction_portfolio_request.py
+-rw-r--r--   0 root         (0) root         (0)     9311 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/create_unit_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18282 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/credit_default_swap.py
+-rw-r--r--   0 root         (0) root         (0)    18482 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/credit_default_swap_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/credit_rating.py
+-rw-r--r--   0 root         (0) root         (0)    17692 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/credit_spread_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    17912 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/credit_spread_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    20913 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/credit_support_annex.py
+-rw-r--r--   0 root         (0) root         (0)     4643 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/currency_and_amount.py
+-rw-r--r--   0 root         (0) root         (0)    15767 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custodian_account.py
+-rw-r--r--   0 root         (0) root         (0)    11808 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10535 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     8071 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_field.py
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_id.py
+-rw-r--r--   0 root         (0) root         (0)     8386 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_request.py
+-rw-r--r--   0 root         (0) root         (0)    13658 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/custom_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     8561 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cut_label_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4564 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/cut_local_time.py
+-rw-r--r--   0 root         (0) root         (0)    15956 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/data_type.py
+-rw-r--r--   0 root         (0) root         (0)    15139 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/data_type_summary.py
+-rw-r--r--   0 root         (0) root         (0)    14148 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/date_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/date_range.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/day_of_week.py
+-rw-r--r--   0 root         (0) root         (0)     5180 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/delete_instrument_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/delete_instrument_response.py
+-rw-r--r--   0 root         (0) root         (0)     6133 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/delete_instruments_response.py
+-rw-r--r--   0 root         (0) root         (0)    10336 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/delete_relationship_request.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     8388 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/dependency_source_filter.py
+-rw-r--r--   0 root         (0) root         (0)    12366 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/discount_factor_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    12506 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/discount_factor_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     5620 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/economic_dependency.py
+-rw-r--r--   0 root         (0) root         (0)     6021 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/economic_dependency_with_complex_market_data.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/economic_dependency_with_quote.py
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/empty_model_options.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/empty_model_options_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/entity_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11925 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_all_of_identifiers.py
+-rw-r--r--   0 root         (0) root         (0)    12573 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_curve_by_prices_data.py
+-rw-r--r--   0 root         (0) root         (0)    12713 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_curve_by_prices_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_model_options.py
+-rw-r--r--   0 root         (0) root         (0)     7910 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_model_options_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    24270 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_option.py
+-rw-r--r--   0 root         (0) root         (0)    24570 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_option_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    23779 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_swap.py
+-rw-r--r--   0 root         (0) root         (0)    24039 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_swap_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11232 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_vol_surface_data.py
+-rw-r--r--   0 root         (0) root         (0)    11352 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/equity_vol_surface_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6807 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/error_detail.py
+-rw-r--r--   0 root         (0) root         (0)     4532 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/event_date_range.py
+-rw-r--r--   0 root         (0) root         (0)    11924 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exchange_traded_option.py
+-rw-r--r--   0 root         (0) root         (0)    12044 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exchange_traded_option_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    23037 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exchange_traded_option_contract_details.py
+-rw-r--r--   0 root         (0) root         (0)    24123 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21470 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/execution_set_request.py
+-rw-r--r--   0 root         (0) root         (0)    11001 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exercise_event.py
+-rw-r--r--   0 root         (0) root         (0)    11121 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exercise_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10368 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exotic_instrument.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/exotic_instrument_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11175 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/expanded_group.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/field_schema.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/field_value.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/file_response.py
+-rw-r--r--   0 root         (0) root         (0)    13199 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fixed_leg.py
+-rw-r--r--   0 root         (0) root         (0)    13339 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fixed_leg_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     4916 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fixed_leg_all_of_overrides.py
+-rw-r--r--   0 root         (0) root         (0)    13456 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/floating_leg.py
+-rw-r--r--   0 root         (0) root         (0)    13596 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/floating_leg_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6593 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/flow_convention_name.py
+-rw-r--r--   0 root         (0) root         (0)    26201 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/flow_conventions.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/forward_rate_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    16070 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/forward_rate_agreement_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14096 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/funding_leg.py
+-rw-r--r--   0 root         (0) root         (0)    14216 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/funding_leg_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    20280 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/future.py
+-rw-r--r--   0 root         (0) root         (0)    20480 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/future_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    21010 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/futures_contract_details.py
+-rw-r--r--   0 root         (0) root         (0)    20275 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward.py
+-rw-r--r--   0 root         (0) root         (0)    20515 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    13820 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_curve_by_quote_reference.py
+-rw-r--r--   0 root         (0) root         (0)    13980 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_curve_by_quote_reference_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14139 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    14319 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11328 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_model_options.py
+-rw-r--r--   0 root         (0) root         (0)    11428 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_model_options_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_pips_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    14631 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_pips_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14327 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    14507 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14639 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_pips_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    14819 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_pips_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    28290 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_option.py
+-rw-r--r--   0 root         (0) root         (0)    28650 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_option_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11104 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_swap.py
+-rw-r--r--   0 root         (0) root         (0)    11204 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_swap_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11136 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/fx_vol_surface_data.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_complex_market_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_counterparty_agreement_response.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_credit_support_annex_response.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_instruments_response.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_quotes_response.py
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_recipe_response.py
+-rw-r--r--   0 root         (0) root         (0)    12031 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/get_reference_portfolio_constituents_response.py
+-rw-r--r--   0 root         (0) root         (0)    12536 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/holding_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)    13890 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/holding_adjustment_with_date.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/holding_context.py
+-rw-r--r--   0 root         (0) root         (0)    10492 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/holdings_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)     9375 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/holdings_adjustment_header.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/i_data_record.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/i_unit_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7950 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9439 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)    18220 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/index_convention.py
+-rw-r--r--   0 root         (0) root         (0)     7151 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/index_model_options.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/index_model_options_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7582 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/industry_classifier.py
+-rw-r--r--   0 root         (0) root         (0)    36403 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/inflation_linked_bond.py
+-rw-r--r--   0 root         (0) root         (0)    36803 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/inflation_linked_bond_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    25417 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/inflation_swap.py
+-rw-r--r--   0 root         (0) root         (0)    25717 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/inflation_swap_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10091 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/informational_error_event.py
+-rw-r--r--   0 root         (0) root         (0)    10191 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/informational_error_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    13186 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/informational_event.py
+-rw-r--r--   0 root         (0) root         (0)    13326 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/informational_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    22491 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/inline_valuation_request.py
+-rw-r--r--   0 root         (0) root         (0)     8211 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/inline_valuations_reconciliation_request.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/input_transition.py
+-rw-r--r--   0 root         (0) root         (0)    19962 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument.py
+-rw-r--r--   0 root         (0) root         (0)     9471 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_definition.py
+-rw-r--r--   0 root         (0) root         (0)     8349 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_definition_format.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_event.py
+-rw-r--r--   0 root         (0) root         (0)    17158 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_event_holder.py
+-rw-r--r--   0 root         (0) root         (0)     7701 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_id_type_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_id_value.py
+-rw-r--r--   0 root         (0) root         (0)     7217 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_leg.py
+-rw-r--r--   0 root         (0) root         (0)     6782 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_leg_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6119 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_match.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_models.py
+-rw-r--r--   0 root         (0) root         (0)     6890 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/instrument_search_property.py
+-rw-r--r--   0 root         (0) root         (0)    14360 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/interest_rate_swap.py
+-rw-r--r--   0 root         (0) root         (0)    14500 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/interest_rate_swap_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    13593 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/interest_rate_swaption.py
+-rw-r--r--   0 root         (0) root         (0)    13733 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/interest_rate_swaption_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11121 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/ir_vol_cube_data.py
+-rw-r--r--   0 root         (0) root         (0)    11241 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/ir_vol_cube_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     5576 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/is_business_day_response.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/label_value_set.py
+-rw-r--r--   0 root         (0) root         (0)    17096 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/leg_definition.py
+-rw-r--r--   0 root         (0) root         (0)    13347 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/legal_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/level_step.py
+-rw-r--r--   0 root         (0) root         (0)     8321 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/life_cycle_event_lineage.py
+-rw-r--r--   0 root         (0) root         (0)     8842 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/life_cycle_event_value.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/life_cycle_event_value_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6624 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/list_aggregation_reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    10737 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/list_aggregation_response.py
+-rw-r--r--   0 root         (0) root         (0)     6196 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/loan_period.py
+-rw-r--r--   0 root         (0) root         (0)     8275 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/lusid_instrument.py
+-rw-r--r--   0 root         (0) root         (0)     9507 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/lusid_unique_id.py
+-rw-r--r--   0 root         (0) root         (0)    10707 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     6590 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/mapped_string.py
+-rw-r--r--   0 root         (0) root         (0)    10566 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/mapping.py
+-rw-r--r--   0 root         (0) root         (0)    10471 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/mapping_rule.py
+-rw-r--r--   0 root         (0) root         (0)     9381 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_context.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_context_suppliers.py
+-rw-r--r--   0 root         (0) root         (0)    26173 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_data_key_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5453 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_data_options.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_data_overrides.py
+-rw-r--r--   0 root         (0) root         (0)    23810 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_data_specific_rule.py
+-rw-r--r--   0 root         (0) root         (0)    14881 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_options.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/market_quote.py
+-rw-r--r--   0 root         (0) root         (0)     4610 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/metric_value.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/model_options.py
+-rw-r--r--   0 root         (0) root         (0)     7701 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/model_property.py
+-rw-r--r--   0 root         (0) root         (0)     7506 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/model_selection.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/next_value_in_sequence_response.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/opaque_market_data.py
+-rw-r--r--   0 root         (0) root         (0)    12085 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/opaque_market_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/opaque_model_options.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/opaque_model_options_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6896 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/open_event.py
+-rw-r--r--   0 root         (0) root         (0)     6956 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/open_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/operation.py
+-rw-r--r--   0 root         (0) root         (0)    22328 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/order_by_spec.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/order_request.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/order_set_request.py
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/otc_confirmation.py
+-rw-r--r--   0 root         (0) root         (0)    33019 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/output_transaction.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/output_transition.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_allocation.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_block.py
+-rw-r--r--   0 root         (0) root         (0)     7330 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_calendar.py
+-rw-r--r--   0 root         (0) root         (0)     7694 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_corporate_action_source.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_custom_entity_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_custom_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     7610 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_cut_label_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_data_type_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_execution.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_instrument.py
+-rw-r--r--   0 root         (0) root         (0)     7694 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_instrument_event_holder.py
+-rw-r--r--   0 root         (0) root         (0)     7414 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_legal_entity.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     7470 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_participation.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_person.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_placement.py
+-rw-r--r--   0 root         (0) root         (0)     7834 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_portfolio_group_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     7694 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_portfolio_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     7946 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_property_definition_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_relationship_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7610 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_sequence_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7483 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/participation.py
+-rw-r--r--   0 root         (0) root         (0)     6927 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/participation_request.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/participation_set_request.py
+-rw-r--r--   0 root         (0) root         (0)     8789 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/performance_return.py
+-rw-r--r--   0 root         (0) root         (0)    10182 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/performance_returns_metric.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/perpetual_property.py
+-rw-r--r--   0 root         (0) root         (0)    11044 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/person.py
+-rw-r--r--   0 root         (0) root         (0)    24250 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/placement.py
+-rw-r--r--   0 root         (0) root         (0)    22675 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/placement_request.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/placement_set_request.py
+-rw-r--r--   0 root         (0) root         (0)    21170 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio.py
+-rw-r--r--   0 root         (0) root         (0)    23701 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_cash_flow.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_cash_ladder.py
+-rw-r--r--   0 root         (0) root         (0)    15148 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_details.py
+-rw-r--r--   0 root         (0) root         (0)     8461 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_entity_id.py
+-rw-r--r--   0 root         (0) root         (0)    13608 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_group.py
+-rw-r--r--   0 root         (0) root         (0)     6997 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_group_properties.py
+-rw-r--r--   0 root         (0) root         (0)    12954 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_group_search_result.py
+-rw-r--r--   0 root         (0) root         (0)    17792 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_holding.py
+-rw-r--r--   0 root         (0) root         (0)     6864 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6776 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_reconciliation_request.py
+-rw-r--r--   0 root         (0) root         (0)    17337 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_result_data_key_rule.py
+-rw-r--r--   0 root         (0) root         (0)    17517 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_result_data_key_rule_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolio_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/portfolios_reconciliation_request.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/premium.py
+-rw-r--r--   0 root         (0) root         (0)     9446 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/pricing_context.py
+-rw-r--r--   0 root         (0) root         (0)    27515 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/pricing_options.py
+-rw-r--r--   0 root         (0) root         (0)     7871 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/processed_command.py
+-rw-r--r--   0 root         (0) root         (0)    27011 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/property_definition.py
+-rw-r--r--   0 root         (0) root         (0)    27875 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/property_definition_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     7836 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/property_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7970 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/property_interval.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/property_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/property_value.py
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/quote.py
+-rw-r--r--   0 root         (0) root         (0)     5784 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/quote_id.py
+-rw-r--r--   0 root         (0) root         (0)    14722 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/quote_series_id.py
+-rw-r--r--   0 root         (0) root         (0)    11312 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/raw_vendor_event.py
+-rw-r--r--   0 root         (0) root         (0)    11432 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/raw_vendor_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    17981 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/realised_gain_loss.py
+-rw-r--r--   0 root         (0) root         (0)     9884 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconcile_date_time_rule.py
+-rw-r--r--   0 root         (0) root         (0)     9984 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconcile_date_time_rule_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     9946 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconcile_numeric_rule.py
+-rw-r--r--   0 root         (0) root         (0)    10046 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconcile_numeric_rule_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10717 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconcile_string_rule.py
+-rw-r--r--   0 root         (0) root         (0)    10817 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconcile_string_rule_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7789 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciled_transaction.py
+-rw-r--r--   0 root         (0) root         (0)    15669 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciliation_break.py
+-rw-r--r--   0 root         (0) root         (0)     5469 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciliation_left_right_address_key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     7308 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciliation_line.py
+-rw-r--r--   0 root         (0) root         (0)    10384 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciliation_request.py
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciliation_response.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reconciliation_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reference_data.py
+-rw-r--r--   0 root         (0) root         (0)    11182 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reference_instrument.py
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reference_instrument_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    11193 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reference_portfolio_constituent.py
+-rw-r--r--   0 root         (0) root         (0)     7557 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reference_portfolio_constituent_request.py
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/related_entity.py
+-rw-r--r--   0 root         (0) root         (0)    10236 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/relation.py
+-rw-r--r--   0 root         (0) root         (0)    13987 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/relationship.py
+-rw-r--r--   0 root         (0) root         (0)    19715 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/relationship_definition.py
+-rw-r--r--   0 root         (0) root         (0)    25647 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/repo.py
+-rw-r--r--   0 root         (0) root         (0)    25907 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/repo_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    12034 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reset_event.py
+-rw-r--r--   0 root         (0) root         (0)    12174 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/reset_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6066 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7658 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_access_metadata_value_of.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_aggregation_query.py
+-rw-r--r--   0 root         (0) root         (0)     7266 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_allocation.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_block.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_calendar_date.py
+-rw-r--r--   0 root         (0) root         (0)     7154 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_change.py
+-rw-r--r--   0 root         (0) root         (0)     7350 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_change_history.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_constituents_adjustment_header.py
+-rw-r--r--   0 root         (0) root         (0)     7406 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_corporate_action.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_execution.py
+-rw-r--r--   0 root         (0) root         (0)     7882 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_get_counterparty_agreement_response.py
+-rw-r--r--   0 root         (0) root         (0)     7798 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_get_credit_support_annex_response.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_get_recipe_response.py
+-rw-r--r--   0 root         (0) root         (0)     7658 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_holdings_adjustment_header.py
+-rw-r--r--   0 root         (0) root         (0)     7490 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_i_unit_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_instrument_id_type_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     7294 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_legal_entity.py
+-rw-r--r--   0 root         (0) root         (0)     7182 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     7350 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_participation.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_performance_return.py
+-rw-r--r--   0 root         (0) root         (0)     7154 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_person.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_placement.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio_cash_flow.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio_cash_ladder.py
+-rw-r--r--   0 root         (0) root         (0)     7378 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio_group.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_processed_command.py
+-rw-r--r--   0 root         (0) root         (0)     7230 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_property.py
+-rw-r--r--   0 root         (0) root         (0)     7490 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_property_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_property_interval.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_quote.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_reconciliation_break.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_relation.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     7406 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_scope_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_string.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/resource_list_of_value_type.py
+-rw-r--r--   0 root         (0) root         (0)     7132 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/response_meta_data.py
+-rw-r--r--   0 root         (0) root         (0)    16885 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_data_key_rule.py
+-rw-r--r--   0 root         (0) root         (0)    17065 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_data_key_rule_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_data_schema.py
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_key_rule.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value.py
+-rw-r--r--   0 root         (0) root         (0)     8573 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value0_d.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value0_d_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_bool.py
+-rw-r--r--   0 root         (0) root         (0)     6624 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_bool_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_currency.py
+-rw-r--r--   0 root         (0) root         (0)     6634 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_currency_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     8005 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_date_time_offset.py
+-rw-r--r--   0 root         (0) root         (0)     8085 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_date_time_offset_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_decimal.py
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_decimal_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6782 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_dictionary.py
+-rw-r--r--   0 root         (0) root         (0)     6842 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_dictionary_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7809 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_int.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_int_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     6550 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_string.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/result_value_string_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     5299 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/schedule.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/schema.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/scope_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12313 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/sequence_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4546 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/set_legal_entity_identifiers_request.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/set_legal_entity_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/set_person_identifiers_request.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/set_person_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/side_configuration_data.py
+-rw-r--r--   0 root         (0) root         (0)    12731 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/simple_cash_flow_loan.py
+-rw-r--r--   0 root         (0) root         (0)    12851 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/simple_cash_flow_loan_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    14542 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/simple_instrument.py
+-rw-r--r--   0 root         (0) root         (0)    14682 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/simple_instrument_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     9597 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/step_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/step_schedule_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    10120 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/stock_split_event.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/stock_split_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     9230 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/stream.py
+-rw-r--r--   0 root         (0) root         (0)     9014 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/supported_analytics_internal_request.py
+-rw-r--r--   0 root         (0) root         (0)     9502 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/target_tax_lot.py
+-rw-r--r--   0 root         (0) root         (0)     9698 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/target_tax_lot_request.py
+-rw-r--r--   0 root         (0) root         (0)    18213 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/term_deposit.py
+-rw-r--r--   0 root         (0) root         (0)    18373 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/term_deposit_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     7854 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/touch.py
+-rw-r--r--   0 root         (0) root         (0)    30339 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7084 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_configuration_data.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_configuration_data_request.py
+-rw-r--r--   0 root         (0) root         (0)    15021 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_configuration_movement_data.py
+-rw-r--r--   0 root         (0) root         (0)    13935 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_configuration_movement_data_request.py
+-rw-r--r--   0 root         (0) root         (0)    14165 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_configuration_type_alias.py
+-rw-r--r--   0 root         (0) root         (0)     5084 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_price.py
+-rw-r--r--   0 root         (0) root         (0)     6460 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_property_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     6569 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_property_mapping_request.py
+-rw-r--r--   0 root         (0) root         (0)     9882 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_query_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    11042 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_reconciliation_request.py
+-rw-r--r--   0 root         (0) root         (0)    25204 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_request.py
+-rw-r--r--   0 root         (0) root         (0)     6796 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transaction_set_configuration_data.py
+-rw-r--r--   0 root         (0) root         (0)     5077 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transactions_reconciliations_response.py
+-rw-r--r--   0 root         (0) root         (0)    12320 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transition_event.py
+-rw-r--r--   0 root         (0) root         (0)    12480 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/transition_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    12564 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/trigger_event.py
+-rw-r--r--   0 root         (0) root         (0)    12704 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/trigger_event_all_of.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/typed_resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7390 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_calendar_request.py
+-rw-r--r--   0 root         (0) root         (0)     8385 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_custom_entity_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_cut_label_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     9294 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_data_type_request.py
+-rw-r--r--   0 root         (0) root         (0)     9254 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_derived_property_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     7188 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_instrument_identifier_request.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_portfolio_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_portfolio_request.py
+-rw-r--r--   0 root         (0) root         (0)     6202 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_property_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)    10185 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_relationship_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     7869 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/update_unit_request.py
+-rw-r--r--   0 root         (0) root         (0)     5592 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_complex_market_data_request.py
+-rw-r--r--   0 root         (0) root         (0)    13957 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_corporate_action_request.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_corporate_actions_response.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_counterparty_agreement_request.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_credit_support_annex_request.py
+-rw-r--r--   0 root         (0) root         (0)     7424 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_custom_entities_response.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_custom_entity_access_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)    11531 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_instrument_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_instrument_events_response.py
+-rw-r--r--   0 root         (0) root         (0)     5337 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_instrument_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     7967 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_instrument_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     8363 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_instruments_response.py
+-rw-r--r--   0 root         (0) root         (0)     7362 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_legal_entities_response.py
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_legal_entity_access_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)    11116 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_legal_entity_request.py
+-rw-r--r--   0 root         (0) root         (0)     4423 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_person_access_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     9118 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_person_request.py
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_portfolio_access_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     4711 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_portfolio_group_access_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     7447 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_portfolio_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)     7603 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_quote_request.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_quotes_response.py
+-rw-r--r--   0 root         (0) root         (0)     5701 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_recipe_request.py
+-rw-r--r--   0 root         (0) root         (0)    10646 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_reference_portfolio_constituents_request.py
+-rw-r--r--   0 root         (0) root         (0)     5745 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_reference_portfolio_constituents_response.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_returns_response.py
+-rw-r--r--   0 root         (0) root         (0)     6073 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_single_structured_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     7226 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_structured_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/upsert_transaction_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/user.py
+-rw-r--r--   0 root         (0) root         (0)    21406 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/valuation_request.py
+-rw-r--r--   0 root         (0) root         (0)    13909 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/valuation_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     8628 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/valuations_reconciliation_request.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/value_type.py
+-rw-r--r--   0 root         (0) root         (0)    15640 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/vendor_model_rule.py
+-rw-r--r--   0 root         (0) root         (0)    11535 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/version.py
+-rw-r--r--   0 root         (0) root         (0)     6389 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/version_summary_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8592 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_a2_b_data_record.py
+-rw-r--r--   0 root         (0) root         (0)     8720 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_a2_b_movement_record.py
+-rw-r--r--   0 root         (0) root         (0)     8720 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_output_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     8688 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_portfolio_holding.py
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     5794 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/weekend_mask.py
+-rw-r--r--   0 root         (0) root         (0)     8442 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/weighted_instrument.py
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/weighted_instruments.py
+-rw-r--r--   0 root         (0) root         (0)    12115 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/yield_curve_data.py
+-rw-r--r--   0 root         (0) root         (0)    12255 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/models/yield_curve_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    13518 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.744071 lusid-sdk-1.0.98/lusid/tcp/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/tcp/tcp_keep_alive_probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.745071 lusid-sdk-1.0.98/lusid/utilities/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/api_client_builder.py
+-rw-r--r--   0 root         (0) root         (0)     5397 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/api_client_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/api_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4065 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/api_configuration_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/lusid_retry.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/proxy_config.py
+-rw-r--r--   0 root         (0) root         (0)     9701 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/lusid/utilities/refreshing_token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:11:56.745071 lusid-sdk-1.0.98/lusid_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-24 20:11:56.000000 lusid-sdk-1.0.98/lusid_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24459 2023-04-24 20:11:56.000000 lusid-sdk-1.0.98/lusid_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 20:11:56.000000 lusid-sdk-1.0.98/lusid_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-24 20:11:56.000000 lusid-sdk-1.0.98/lusid_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 20:11:56.000000 lusid-sdk-1.0.98/lusid_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 20:11:56.746071 lusid-sdk-1.0.98/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-04-24 19:28:16.000000 lusid-sdk-1.0.98/setup.py
```

### Comparing `lusid-sdk-1.0.91/README.md` & `lusid-sdk-1.0.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.91
-- Package version: 1.0.91
+- API version: 1.0.98
+- Package version: 1.0.98
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-sdk-1.0.91/lusid/__init__.py` & `lusid-sdk-1.0.98/lusid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.91"
+__version__ = "1.0.98"
 
 # import apis into sdk package
 from lusid.api.aggregation_api import AggregationApi
 from lusid.api.allocations_api import AllocationsApi
 from lusid.api.application_metadata_api import ApplicationMetadataApi
 from lusid.api.blocks_api import BlocksApi
 from lusid.api.calendars_api import CalendarsApi
```

### Comparing `lusid-sdk-1.0.91/lusid/api/__init__.py` & `lusid-sdk-1.0.98/lusid/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/api/aggregation_api.py` & `lusid-sdk-1.0.98/lusid/api/aggregation_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -184,15 +184,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAggregationQuery",
             400: "LusidValidationProblemDetails",
@@ -327,15 +327,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ListAggregationResponse",
             400: "LusidValidationProblemDetails",
@@ -470,15 +470,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ListAggregationResponse",
             400: "LusidValidationProblemDetails",
@@ -613,15 +613,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Aggregation",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/allocations_api.py` & `lusid-sdk-1.0.98/lusid/api/allocations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -182,15 +182,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -366,15 +366,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Allocation",
             400: "LusidValidationProblemDetails",
@@ -570,15 +570,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfAllocation",
             400: "LusidValidationProblemDetails",
@@ -713,15 +713,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAllocation",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/application_metadata_api.py` & `lusid-sdk-1.0.98/lusid/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "FileResponse",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VersionSummaryDto",
         }
@@ -439,15 +439,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/blocks_api.py` & `lusid-sdk-1.0.98/lusid/api/blocks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -182,15 +182,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -366,15 +366,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Block",
             400: "LusidValidationProblemDetails",
@@ -563,15 +563,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfBlock",
             400: "LusidValidationProblemDetails",
@@ -706,15 +706,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ResourceListOfBlock",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/calendars_api.py` & `lusid-sdk-1.0.98/lusid/api/calendars_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -185,15 +185,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AddBusinessDaysToDateResponse",
             400: "LusidValidationProblemDetails",
@@ -370,15 +370,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CalendarDate",
             400: "LusidValidationProblemDetails",
@@ -517,15 +517,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Calendar",
             400: "LusidValidationProblemDetails",
@@ -688,15 +688,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Calendar",
             400: "LusidValidationProblemDetails",
@@ -878,15 +878,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CalendarDate",
             400: "LusidValidationProblemDetails",
@@ -1051,15 +1051,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[datetime]",
             400: "LusidValidationProblemDetails",
@@ -1229,15 +1229,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Calendar",
             400: "LusidValidationProblemDetails",
@@ -1445,15 +1445,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfCalendarDate",
             400: "LusidValidationProblemDetails",
@@ -1634,15 +1634,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "IsBusinessDayResponse",
             400: "LusidValidationProblemDetails",
@@ -1815,15 +1815,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfCalendar",
             400: "LusidValidationProblemDetails",
@@ -2022,15 +2022,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfCalendar",
             400: "LusidValidationProblemDetails",
@@ -2207,15 +2207,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Calendar",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/complex_market_data_api.py` & `lusid-sdk-1.0.98/lusid/api/complex_market_data_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AnnulStructuredDataResponse",
             400: "LusidValidationProblemDetails",
@@ -374,15 +374,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetComplexMarketDataResponse",
             400: "LusidValidationProblemDetails",
@@ -540,15 +540,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertStructuredDataResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/configuration_recipe_api.py` & `lusid-sdk-1.0.98/lusid/api/configuration_recipe_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -184,15 +184,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AnnulSingleStructuredDataResponse",
             400: "LusidValidationProblemDetails",
@@ -362,15 +362,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetRecipeResponse",
             400: "LusidValidationProblemDetails",
@@ -517,15 +517,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfGetRecipeResponse",
             400: "LusidValidationProblemDetails",
@@ -664,15 +664,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertSingleStructuredDataResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/corporate_action_sources_api.py` & `lusid-sdk-1.0.98/lusid/api/corporate_action_sources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -199,15 +199,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "UpsertCorporateActionsResponse",
             400: "LusidValidationProblemDetails",
@@ -346,15 +346,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "CorporateActionSource",
             400: "LusidValidationProblemDetails",
@@ -529,15 +529,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -712,15 +712,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -950,15 +950,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfCorporateAction",
             400: "LusidValidationProblemDetails",
@@ -1165,15 +1165,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfInstrumentEventHolder",
             400: "LusidValidationProblemDetails",
@@ -1350,15 +1350,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfCorporateActionSource",
             400: "LusidValidationProblemDetails",
@@ -1531,15 +1531,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertInstrumentEventsResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/counterparties_api.py` & `lusid-sdk-1.0.98/lusid/api/counterparties_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -187,15 +187,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AnnulSingleStructuredDataResponse",
             400: "LusidValidationProblemDetails",
@@ -358,15 +358,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AnnulSingleStructuredDataResponse",
             400: "LusidValidationProblemDetails",
@@ -536,15 +536,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetCounterpartyAgreementResponse",
             400: "LusidValidationProblemDetails",
@@ -714,15 +714,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetCreditSupportAnnexResponse",
             400: "LusidValidationProblemDetails",
@@ -854,15 +854,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfGetCounterpartyAgreementResponse",
             400: "LusidValidationProblemDetails",
@@ -994,15 +994,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfGetCreditSupportAnnexResponse",
             400: "LusidValidationProblemDetails",
@@ -1141,15 +1141,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertSingleStructuredDataResponse",
             400: "LusidValidationProblemDetails",
@@ -1288,15 +1288,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertSingleStructuredDataResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/custom_entities_api.py` & `lusid-sdk-1.0.98/lusid/api/custom_entities_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -224,15 +224,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -466,15 +466,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -689,15 +689,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -926,15 +926,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CustomEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1168,15 +1168,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[AccessMetadataValue]",
             400: "LusidValidationProblemDetails",
@@ -1420,15 +1420,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelationship",
             400: "LusidValidationProblemDetails",
@@ -1641,15 +1641,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfCustomEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1878,15 +1878,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -2059,15 +2059,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertCustomEntitiesResponse",
             400: "LusidValidationProblemDetails",
@@ -2223,15 +2223,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CustomEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -2479,15 +2479,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[AccessMetadataValue]",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/custom_entity_definitions_api.py` & `lusid-sdk-1.0.98/lusid/api/custom_entity_definitions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CustomEntityDefinition",
             400: "LusidValidationProblemDetails",
@@ -316,15 +316,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CustomEntityDefinition",
             400: "LusidValidationProblemDetails",
@@ -497,15 +497,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfCustomEntityDefinition",
             400: "LusidValidationProblemDetails",
@@ -661,15 +661,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CustomEntityDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/cut_label_definitions_api.py` & `lusid-sdk-1.0.98/lusid/api/cut_label_definitions_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "CutLabelDefinition",
             400: "LusidValidationProblemDetails",
@@ -307,15 +307,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "datetime",
             400: "LusidValidationProblemDetails",
@@ -466,15 +466,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CutLabelDefinition",
             400: "LusidValidationProblemDetails",
@@ -658,15 +658,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfCutLabelDefinition",
             400: "LusidValidationProblemDetails",
@@ -820,15 +820,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "CutLabelDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/data_types_api.py` & `lusid-sdk-1.0.98/lusid/api/data_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -158,15 +158,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "DataType",
             400: "LusidValidationProblemDetails",
@@ -336,15 +336,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DataType",
             400: "LusidValidationProblemDetails",
@@ -537,15 +537,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfIUnitDefinitionDto",
             400: "LusidValidationProblemDetails",
@@ -733,15 +733,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfDataTypeSummary",
             400: "LusidValidationProblemDetails",
@@ -936,15 +936,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDataType",
             400: "LusidValidationProblemDetails",
@@ -1121,15 +1121,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DataType",
             400: "LusidValidationProblemDetails",
@@ -1306,15 +1306,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DataType",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/derived_transaction_portfolios_api.py` & `lusid-sdk-1.0.98/lusid/api/derived_transaction_portfolios_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -173,15 +173,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Portfolio",
             400: "LusidValidationProblemDetails",
@@ -359,15 +359,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/entities_api.py` & `lusid-sdk-1.0.98/lusid/api/entities_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -187,15 +187,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             400: "LusidValidationProblemDetails",
             200: "ResourceListOfChange",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/executions_api.py` & `lusid-sdk-1.0.98/lusid/api/executions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -182,15 +182,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -366,15 +366,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Execution",
             400: "LusidValidationProblemDetails",
@@ -563,15 +563,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfExecution",
             400: "LusidValidationProblemDetails",
@@ -706,15 +706,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ResourceListOfExecution",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/instruments_api.py` & `lusid-sdk-1.0.98/lusid/api/instruments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeleteInstrumentResponse",
             400: "LusidValidationProblemDetails",
@@ -386,15 +386,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeleteInstrumentPropertiesResponse",
             400: "LusidValidationProblemDetails",
@@ -555,15 +555,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeleteInstrumentsResponse",
             400: "LusidValidationProblemDetails",
@@ -766,15 +766,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "InstrumentModels",
             400: "LusidValidationProblemDetails",
@@ -966,15 +966,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Instrument",
             400: "LusidValidationProblemDetails",
@@ -1099,15 +1099,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfInstrumentIdTypeDescriptor",
         }
@@ -1282,15 +1282,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "InstrumentProperties",
             400: "LusidValidationProblemDetails",
@@ -1518,15 +1518,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPropertyInterval",
             400: "LusidValidationProblemDetails",
@@ -1749,15 +1749,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelationship",
             400: "LusidValidationProblemDetails",
@@ -1952,15 +1952,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetInstrumentsResponse",
             400: "LusidValidationProblemDetails",
@@ -2170,15 +2170,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfProperty",
             400: "LusidValidationProblemDetails",
@@ -2404,15 +2404,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfInstrument",
             400: "LusidValidationProblemDetails",
@@ -2588,15 +2588,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Instrument",
             400: "LusidValidationProblemDetails",
@@ -2750,15 +2750,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "UpsertInstrumentsResponse",
             400: "LusidValidationProblemDetails",
@@ -2912,15 +2912,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "UpsertInstrumentPropertiesResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/legal_entities_api.py` & `lusid-sdk-1.0.98/lusid/api/legal_entities_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -210,15 +210,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -433,15 +433,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -640,15 +640,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -847,15 +847,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1051,15 +1051,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -1277,15 +1277,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "LegalEntity",
             400: "LusidValidationProblemDetails",
@@ -1500,15 +1500,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[AccessMetadataValue]",
             400: "LusidValidationProblemDetails",
@@ -1747,15 +1747,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPropertyInterval",
             400: "LusidValidationProblemDetails",
@@ -1980,15 +1980,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelationship",
             400: "LusidValidationProblemDetails",
@@ -2184,15 +2184,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfLegalEntity",
             400: "LusidValidationProblemDetails",
@@ -2434,15 +2434,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfLegalEntity",
             400: "LusidValidationProblemDetails",
@@ -2652,15 +2652,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -2854,15 +2854,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "LegalEntity",
             400: "LusidValidationProblemDetails",
@@ -3056,15 +3056,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "LegalEntity",
             400: "LusidValidationProblemDetails",
@@ -3220,15 +3220,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "UpsertLegalEntitiesResponse",
             400: "LusidValidationProblemDetails",
@@ -3367,15 +3367,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "LegalEntity",
             400: "LusidValidationProblemDetails",
@@ -3604,15 +3604,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessMetadataValueOf",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/orders_api.py` & `lusid-sdk-1.0.98/lusid/api/orders_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -182,15 +182,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -366,15 +366,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Order",
             400: "LusidValidationProblemDetails",
@@ -570,15 +570,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfOrder",
             400: "LusidValidationProblemDetails",
@@ -713,15 +713,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ResourceListOfOrder",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/participations_api.py` & `lusid-sdk-1.0.98/lusid/api/participations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -182,15 +182,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -366,15 +366,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Participation",
             400: "LusidValidationProblemDetails",
@@ -563,15 +563,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfParticipation",
             400: "LusidValidationProblemDetails",
@@ -706,15 +706,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ResourceListOfParticipation",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/persons_api.py` & `lusid-sdk-1.0.98/lusid/api/persons_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -212,15 +212,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -419,15 +419,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -628,15 +628,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -837,15 +837,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1025,15 +1025,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -1229,15 +1229,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Person",
             400: "LusidValidationProblemDetails",
@@ -1430,15 +1430,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[AccessMetadataValue]",
             400: "LusidValidationProblemDetails",
@@ -1663,15 +1663,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPropertyInterval",
             400: "LusidValidationProblemDetails",
@@ -1874,15 +1874,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelation",
             400: "LusidValidationProblemDetails",
@@ -2109,15 +2109,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelationship",
             400: "LusidValidationProblemDetails",
@@ -2313,15 +2313,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPerson",
             400: "LusidValidationProblemDetails",
@@ -2546,15 +2546,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfPerson",
             400: "LusidValidationProblemDetails",
@@ -2748,15 +2748,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -2936,15 +2936,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Person",
             400: "LusidValidationProblemDetails",
@@ -3124,15 +3124,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Person",
             400: "LusidValidationProblemDetails",
@@ -3271,15 +3271,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Person",
             400: "LusidValidationProblemDetails",
@@ -3484,15 +3484,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessMetadataValueOf",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/placements_api.py` & `lusid-sdk-1.0.98/lusid/api/placements_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -182,15 +182,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -366,15 +366,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Placement",
             400: "LusidValidationProblemDetails",
@@ -563,15 +563,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfPlacement",
             400: "LusidValidationProblemDetails",
@@ -706,15 +706,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ResourceListOfPlacement",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/portfolio_groups_api.py` & `lusid-sdk-1.0.98/lusid/api/portfolio_groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -225,15 +225,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -421,15 +421,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -658,15 +658,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VersionedResourceListOfOutputTransaction",
             400: "LusidValidationProblemDetails",
@@ -820,15 +820,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -1012,15 +1012,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1214,15 +1214,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1438,15 +1438,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -1609,15 +1609,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1817,15 +1817,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -2054,15 +2054,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VersionedResourceListOfA2BDataRecord",
             400: "LusidValidationProblemDetails",
@@ -2239,15 +2239,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioGroupProperties",
             400: "LusidValidationProblemDetails",
@@ -2454,15 +2454,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VersionedResourceListOfPortfolioHolding",
             400: "LusidValidationProblemDetails",
@@ -2663,15 +2663,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -2865,15 +2865,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[AccessMetadataValue]",
             400: "LusidValidationProblemDetails",
@@ -3065,15 +3065,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfProcessedCommand",
             400: "LusidValidationProblemDetails",
@@ -3266,15 +3266,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ExpandedGroup",
             400: "LusidValidationProblemDetails",
@@ -3451,15 +3451,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -3688,15 +3688,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPropertyInterval",
             400: "LusidValidationProblemDetails",
@@ -3904,15 +3904,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelationship",
             400: "LusidValidationProblemDetails",
@@ -4148,15 +4148,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VersionedResourceListOfTransaction",
             400: "LusidValidationProblemDetails",
@@ -4353,15 +4353,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -4552,15 +4552,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -4748,15 +4748,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioGroup",
             400: "LusidValidationProblemDetails",
@@ -4929,15 +4929,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioGroupProperties",
             400: "LusidValidationProblemDetails",
@@ -5145,15 +5145,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessMetadataValueOf",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/portfolios_api.py` & `lusid-sdk-1.0.98/lusid/api/portfolios_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -231,15 +231,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -402,15 +402,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -592,15 +592,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -830,15 +830,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -1031,15 +1031,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Portfolio",
             400: "LusidValidationProblemDetails",
@@ -1237,15 +1237,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AggregatedReturnsResponse",
             400: "LusidValidationProblemDetails",
@@ -1463,15 +1463,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfProcessedCommand",
             400: "LusidValidationProblemDetails",
@@ -1648,15 +1648,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -1833,15 +1833,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioProperties",
             400: "LusidValidationProblemDetails",
@@ -2070,15 +2070,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPropertyInterval",
             400: "LusidValidationProblemDetails",
@@ -2286,15 +2286,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRelationship",
             400: "LusidValidationProblemDetails",
@@ -2523,15 +2523,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPerformanceReturn",
             400: "LusidValidationProblemDetails",
@@ -2725,15 +2725,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[AccessMetadataValue]",
             400: "LusidValidationProblemDetails",
@@ -2944,15 +2944,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfProperty",
             400: "LusidValidationProblemDetails",
@@ -3170,15 +3170,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPortfolio",
             400: "LusidValidationProblemDetails",
@@ -3400,15 +3400,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPortfolio",
             400: "LusidValidationProblemDetails",
@@ -3585,15 +3585,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ActionResultOfPortfolio",
             400: "LusidValidationProblemDetails",
@@ -3784,15 +3784,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "dict(str, list[AccessMetadataValue])",
             400: "LusidValidationProblemDetails",
@@ -3976,15 +3976,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Portfolio",
             400: "LusidValidationProblemDetails",
@@ -4192,15 +4192,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessMetadataValueOf",
             400: "LusidValidationProblemDetails",
@@ -4377,15 +4377,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PortfolioProperties",
             400: "LusidValidationProblemDetails",
@@ -4600,15 +4600,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertReturnsResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/property_definitions_api.py` & `lusid-sdk-1.0.98/lusid/api/property_definitions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -162,15 +162,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PropertyDefinition",
             400: "LusidValidationProblemDetails",
@@ -309,15 +309,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PropertyDefinition",
             400: "LusidValidationProblemDetails",
@@ -491,15 +491,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -658,15 +658,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfPropertyDefinition",
             400: "LusidValidationProblemDetails",
@@ -847,15 +847,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PropertyDefinition",
             400: "LusidValidationProblemDetails",
@@ -1043,15 +1043,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PropertyDefinition",
             400: "LusidValidationProblemDetails",
@@ -1239,15 +1239,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PropertyDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/quotes_api.py` & `lusid-sdk-1.0.98/lusid/api/quotes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -177,15 +177,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AnnulQuotesResponse",
             400: "LusidValidationProblemDetails",
@@ -360,15 +360,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetQuotesResponse",
             400: "LusidValidationProblemDetails",
@@ -563,15 +563,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfQuote",
             400: "LusidValidationProblemDetails",
@@ -766,15 +766,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfQuote",
             400: "LusidValidationProblemDetails",
@@ -928,15 +928,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertQuotesResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/reconciliations_api.py` & `lusid-sdk-1.0.98/lusid/api/reconciliations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -190,15 +190,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "str",
             400: "LusidValidationProblemDetails",
@@ -361,15 +361,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Mapping",
             400: "LusidValidationProblemDetails",
@@ -501,15 +501,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfMapping",
             400: "LusidValidationProblemDetails",
@@ -644,15 +644,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ReconciliationResponse",
             400: "LusidValidationProblemDetails",
@@ -824,15 +824,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfReconciliationBreak",
             400: "LusidValidationProblemDetails",
@@ -967,15 +967,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ListAggregationReconciliation",
             400: "LusidValidationProblemDetails",
@@ -1110,15 +1110,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TransactionsReconciliationsResponse",
             400: "LusidValidationProblemDetails",
@@ -1253,15 +1253,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ListAggregationReconciliation",
             400: "LusidValidationProblemDetails",
@@ -1396,15 +1396,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Mapping",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/reference_portfolio_api.py` & `lusid-sdk-1.0.98/lusid/api/reference_portfolio_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -180,15 +180,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Portfolio",
             400: "LusidValidationProblemDetails",
@@ -373,15 +373,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetReferencePortfolioConstituentsResponse",
             400: "LusidValidationProblemDetails",
@@ -573,15 +573,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfConstituentsAdjustmentHeader",
             400: "LusidValidationProblemDetails",
@@ -758,15 +758,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpsertReferencePortfolioConstituentsResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/relationship_definitions_api.py` & `lusid-sdk-1.0.98/lusid/api/relationship_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "RelationshipDefinition",
             400: "LusidValidationProblemDetails",
@@ -331,15 +331,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -509,15 +509,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RelationshipDefinition",
             400: "LusidValidationProblemDetails",
@@ -686,15 +686,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfRelationshipDefinition",
             400: "LusidValidationProblemDetails",
@@ -871,15 +871,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RelationshipDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/relationships_api.py` & `lusid-sdk-1.0.98/lusid/api/relationships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -197,15 +197,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "CompleteRelationship",
             400: "LusidValidationProblemDetails",
@@ -382,15 +382,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/schemas_api.py` & `lusid-sdk-1.0.98/lusid/api/schemas_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -164,15 +164,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Schema",
             400: "LusidValidationProblemDetails",
@@ -312,15 +312,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PropertySchema",
             400: "LusidValidationProblemDetails",
@@ -467,15 +467,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfValueType",
             400: "LusidValidationProblemDetails",
@@ -600,15 +600,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfString",
         }
```

### Comparing `lusid-sdk-1.0.91/lusid/api/scopes_api.py` & `lusid-sdk-1.0.98/lusid/api/scopes_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScopeDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/search_api.py` & `lusid-sdk-1.0.98/lusid/api/search_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -189,15 +189,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "list[InstrumentMatch]",
             400: "LusidValidationProblemDetails",
@@ -381,15 +381,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfPortfolioGroupSearchResult",
             400: "LusidValidationProblemDetails",
@@ -573,15 +573,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfPortfolioSearchResult",
             400: "LusidValidationProblemDetails",
@@ -765,15 +765,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfPropertyDefinitionSearchResult",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/sequences_api.py` & `lusid-sdk-1.0.98/lusid/api/sequences_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -178,15 +178,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "SequenceDefinition",
             400: "LusidValidationProblemDetails",
@@ -349,15 +349,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "SequenceDefinition",
             400: "LusidValidationProblemDetails",
@@ -523,15 +523,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfSequenceDefinition",
             400: "LusidValidationProblemDetails",
@@ -705,15 +705,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "NextValueInSequenceResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/system_configuration_api.py` & `lusid-sdk-1.0.98/lusid/api/system_configuration_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -153,15 +153,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TransactionSetConfigurationData",
             400: "LusidValidationProblemDetails",
@@ -293,15 +293,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '1.0.91'
+        header_params['X-LUSID-SDK-Version'] = '1.0.98'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TransactionSetConfigurationData",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-sdk-1.0.91/lusid/api/transaction_portfolios_api.py` & `lusid-sdk-1.0.98/lusid/api/transaction_portfolios_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 2320 636f 6469 6e67 3a20 7574 662d 380a  # coding: utf-8.
 00000010: 0a22 2222 0a20 2020 204c 5553 4944 2041  .""".    LUSID A
 00000020: 5049 0a0a 2020 2020 4649 4e42 4f55 524e  PI..    FINBOURN
 00000030: 4520 5465 6368 6e6f 6c6f 6779 2020 2320  E Technology  # 
 00000040: 6e6f 7161 3a20 4535 3031 0a0a 2020 2020  noqa: E501..    
 00000050: 5468 6520 7665 7273 696f 6e20 6f66 2074  The version of t
 00000060: 6865 204f 7065 6e41 5049 2064 6f63 756d  he OpenAPI docum
-00000070: 656e 743a 2031 2e30 2e39 310a 2020 2020  ent: 1.0.91.    
+00000070: 656e 743a 2031 2e30 2e39 380a 2020 2020  ent: 1.0.98.    
 00000080: 436f 6e74 6163 743a 2069 6e66 6f40 6669  Contact: info@fi
 00000090: 6e62 6f75 726e 652e 636f 6d0a 2020 2020  nbourne.com.    
 000000a0: 4765 6e65 7261 7465 6420 6279 3a20 6874  Generated by: ht
 000000b0: 7470 733a 2f2f 6f70 656e 6170 692d 6765  tps://openapi-ge
 000000c0: 6e65 7261 746f 722e 7465 6368 0a22 2222  nerator.tech."""
 000000d0: 0a0a 0a66 726f 6d20 5f5f 6675 7475 7265  ...from __future
 000000e0: 5f5f 2069 6d70 6f72 7420 6162 736f 6c75  __ import absolu
@@ -952,15 +952,15 @@
 00003b70: 7468 6520 4c55 5349 4420 6865 6164 6572  the LUSID header
 00003b80: 0a20 2020 2020 2020 2068 6561 6465 725f  .        header_
 00003b90: 7061 7261 6d73 5b27 582d 4c55 5349 442d  params['X-LUSID-
 00003ba0: 5344 4b2d 4c61 6e67 7561 6765 275d 203d  SDK-Language'] =
 00003bb0: 2027 5079 7468 6f6e 270a 2020 2020 2020   'Python'.      
 00003bc0: 2020 6865 6164 6572 5f70 6172 616d 735b    header_params[
 00003bd0: 2758 2d4c 5553 4944 2d53 444b 2d56 6572  'X-LUSID-SDK-Ver
-00003be0: 7369 6f6e 275d 203d 2027 312e 302e 3931  sion'] = '1.0.91
+00003be0: 7369 6f6e 275d 203d 2027 312e 302e 3938  sion'] = '1.0.98
 00003bf0: 270a 0a20 2020 2020 2020 2023 2041 7574  '..        # Aut
 00003c00: 6865 6e74 6963 6174 696f 6e20 7365 7474  hentication sett
 00003c10: 696e 670a 2020 2020 2020 2020 6175 7468  ing.        auth
 00003c20: 5f73 6574 7469 6e67 7320 3d20 5b27 6f61  _settings = ['oa
 00003c30: 7574 6832 275d 2020 2320 6e6f 7161 3a20  uth2']  # noqa: 
 00003c40: 4535 3031 0a0a 2020 2020 2020 2020 7265  E501..        re
 00003c50: 7370 6f6e 7365 5f74 7970 6573 5f6d 6170  sponse_types_map
@@ -1862,15 +1862,15 @@
 00007450: 6164 6572 0a20 2020 2020 2020 2068 6561  ader.        hea
 00007460: 6465 725f 7061 7261 6d73 5b27 582d 4c55  der_params['X-LU
 00007470: 5349 442d 5344 4b2d 4c61 6e67 7561 6765  SID-SDK-Language
 00007480: 275d 203d 2027 5079 7468 6f6e 270a 2020  '] = 'Python'.  
 00007490: 2020 2020 2020 6865 6164 6572 5f70 6172        header_par
 000074a0: 616d 735b 2758 2d4c 5553 4944 2d53 444b  ams['X-LUSID-SDK
 000074b0: 2d56 6572 7369 6f6e 275d 203d 2027 312e  -Version'] = '1.
-000074c0: 302e 3931 270a 0a20 2020 2020 2020 2023  0.91'..        #
+000074c0: 302e 3938 270a 0a20 2020 2020 2020 2023  0.98'..        #
 000074d0: 2041 7574 6865 6e74 6963 6174 696f 6e20   Authentication 
 000074e0: 7365 7474 696e 670a 2020 2020 2020 2020  setting.        
 000074f0: 6175 7468 5f73 6574 7469 6e67 7320 3d20  auth_settings = 
 00007500: 5b27 6f61 7574 6832 275d 2020 2320 6e6f  ['oauth2']  # no
 00007510: 7161 3a20 4535 3031 0a0a 2020 2020 2020  qa: E501..      
 00007520: 2020 7265 7370 6f6e 7365 5f74 7970 6573    response_types
 00007530: 5f6d 6170 203d 207b 0a20 2020 2020 2020  _map = {.       
@@ -2709,15 +2709,15 @@
 0000a940: 5349 4420 6865 6164 6572 0a20 2020 2020  SID header.     
 0000a950: 2020 2068 6561 6465 725f 7061 7261 6d73     header_params
 0000a960: 5b27 582d 4c55 5349 442d 5344 4b2d 4c61  ['X-LUSID-SDK-La
 0000a970: 6e67 7561 6765 275d 203d 2027 5079 7468  nguage'] = 'Pyth
 0000a980: 6f6e 270a 2020 2020 2020 2020 6865 6164  on'.        head
 0000a990: 6572 5f70 6172 616d 735b 2758 2d4c 5553  er_params['X-LUS
 0000a9a0: 4944 2d53 444b 2d56 6572 7369 6f6e 275d  ID-SDK-Version']
-0000a9b0: 203d 2027 312e 302e 3931 270a 0a20 2020   = '1.0.91'..   
+0000a9b0: 203d 2027 312e 302e 3938 270a 0a20 2020   = '1.0.98'..   
 0000a9c0: 2020 2020 2023 2041 7574 6865 6e74 6963       # Authentic
 0000a9d0: 6174 696f 6e20 7365 7474 696e 670a 2020  ation setting.  
 0000a9e0: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
 0000a9f0: 6e67 7320 3d20 5b27 6f61 7574 6832 275d  ngs = ['oauth2']
 0000aa00: 2020 2320 6e6f 7161 3a20 4535 3031 0a0a    # noqa: E501..
 0000aa10: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
 0000aa20: 5f74 7970 6573 5f6d 6170 203d 207b 0a20  _types_map = {. 
@@ -3765,15 +3765,15 @@
 0000eb40: 6865 6164 6572 0a20 2020 2020 2020 2068  header.        h
 0000eb50: 6561 6465 725f 7061 7261 6d73 5b27 582d  eader_params['X-
 0000eb60: 4c55 5349 442d 5344 4b2d 4c61 6e67 7561  LUSID-SDK-Langua
 0000eb70: 6765 275d 203d 2027 5079 7468 6f6e 270a  ge'] = 'Python'.
 0000eb80: 2020 2020 2020 2020 6865 6164 6572 5f70          header_p
 0000eb90: 6172 616d 735b 2758 2d4c 5553 4944 2d53  arams['X-LUSID-S
 0000eba0: 444b 2d56 6572 7369 6f6e 275d 203d 2027  DK-Version'] = '
-0000ebb0: 312e 302e 3931 270a 0a20 2020 2020 2020  1.0.91'..       
+0000ebb0: 312e 302e 3938 270a 0a20 2020 2020 2020  1.0.98'..       
 0000ebc0: 2023 2041 7574 6865 6e74 6963 6174 696f   # Authenticatio
 0000ebd0: 6e20 7365 7474 696e 670a 2020 2020 2020  n setting.      
 0000ebe0: 2020 6175 7468 5f73 6574 7469 6e67 7320    auth_settings 
 0000ebf0: 3d20 5b27 6f61 7574 6832 275d 2020 2320  = ['oauth2']  # 
 0000ec00: 6e6f 7161 3a20 4535 3031 0a0a 2020 2020  noqa: E501..    
 0000ec10: 2020 2020 7265 7370 6f6e 7365 5f74 7970      response_typ
 0000ec20: 6573 5f6d 6170 203d 207b 0a20 2020 2020  es_map = {.     
@@ -4444,15 +4444,15 @@
 000115b0: 6865 6164 6572 0a20 2020 2020 2020 2068  header.        h
 000115c0: 6561 6465 725f 7061 7261 6d73 5b27 582d  eader_params['X-
 000115d0: 4c55 5349 442d 5344 4b2d 4c61 6e67 7561  LUSID-SDK-Langua
 000115e0: 6765 275d 203d 2027 5079 7468 6f6e 270a  ge'] = 'Python'.
 000115f0: 2020 2020 2020 2020 6865 6164 6572 5f70          header_p
 00011600: 6172 616d 735b 2758 2d4c 5553 4944 2d53  arams['X-LUSID-S
 00011610: 444b 2d56 6572 7369 6f6e 275d 203d 2027  DK-Version'] = '
-00011620: 312e 302e 3931 270a 0a20 2020 2020 2020  1.0.91'..       
+00011620: 312e 302e 3938 270a 0a20 2020 2020 2020  1.0.98'..       
 00011630: 2023 2041 7574 6865 6e74 6963 6174 696f   # Authenticatio
 00011640: 6e20 7365 7474 696e 670a 2020 2020 2020  n setting.      
 00011650: 2020 6175 7468 5f73 6574 7469 6e67 7320    auth_settings 
 00011660: 3d20 5b27 6f61 7574 6832 275d 2020 2320  = ['oauth2']  # 
 00011670: 6e6f 7161 3a20 4535 3031 0a0a 2020 2020  noqa: E501..    
 00011680: 2020 2020 7265 7370 6f6e 7365 5f74 7970      response_typ
 00011690: 6573 5f6d 6170 203d 207b 0a20 2020 2020  es_map = {.     
@@ -5102,15 +5102,15 @@
 00013ed0: 4420 6865 6164 6572 0a20 2020 2020 2020  D header.       
 00013ee0: 2068 6561 6465 725f 7061 7261 6d73 5b27   header_params['
 00013ef0: 582d 4c55 5349 442d 5344 4b2d 4c61 6e67  X-LUSID-SDK-Lang
 00013f00: 7561 6765 275d 203d 2027 5079 7468 6f6e  uage'] = 'Python
 00013f10: 270a 2020 2020 2020 2020 6865 6164 6572  '.        header
 00013f20: 5f70 6172 616d 735b 2758 2d4c 5553 4944  _params['X-LUSID
 00013f30: 2d53 444b 2d56 6572 7369 6f6e 275d 203d  -SDK-Version'] =
-00013f40: 2027 312e 302e 3931 270a 0a20 2020 2020   '1.0.91'..     
+00013f40: 2027 312e 302e 3938 270a 0a20 2020 2020   '1.0.98'..     
 00013f50: 2020 2023 2041 7574 6865 6e74 6963 6174     # Authenticat
 00013f60: 696f 6e20 7365 7474 696e 670a 2020 2020  ion setting.    
 00013f70: 2020 2020 6175 7468 5f73 6574 7469 6e67      auth_setting
 00013f80: 7320 3d20 5b27 6f61 7574 6832 275d 2020  s = ['oauth2']  
 00013f90: 2320 6e6f 7161 3a20 4535 3031 0a0a 2020  # noqa: E501..  
 00013fa0: 2020 2020 2020 7265 7370 6f6e 7365 5f74        response_t
 00013fb0: 7970 6573 5f6d 6170 203d 207b 0a20 2020  ypes_map = {.   
@@ -5662,15 +5662,15 @@
 000161d0: 6561 6465 720a 2020 2020 2020 2020 6865  eader.        he
 000161e0: 6164 6572 5f70 6172 616d 735b 2758 2d4c  ader_params['X-L
 000161f0: 5553 4944 2d53 444b 2d4c 616e 6775 6167  USID-SDK-Languag
 00016200: 6527 5d20 3d20 2750 7974 686f 6e27 0a20  e'] = 'Python'. 
 00016210: 2020 2020 2020 2068 6561 6465 725f 7061         header_pa
 00016220: 7261 6d73 5b27 582d 4c55 5349 442d 5344  rams['X-LUSID-SD
 00016230: 4b2d 5665 7273 696f 6e27 5d20 3d20 2731  K-Version'] = '1
-00016240: 2e30 2e39 3127 0a0a 2020 2020 2020 2020  .0.91'..        
+00016240: 2e30 2e39 3827 0a0a 2020 2020 2020 2020  .0.98'..        
 00016250: 2320 4175 7468 656e 7469 6361 7469 6f6e  # Authentication
 00016260: 2073 6574 7469 6e67 0a20 2020 2020 2020   setting.       
 00016270: 2061 7574 685f 7365 7474 696e 6773 203d   auth_settings =
 00016280: 205b 276f 6175 7468 3227 5d20 2023 206e   ['oauth2']  # n
 00016290: 6f71 613a 2045 3530 310a 0a20 2020 2020  oqa: E501..     
 000162a0: 2020 2072 6573 706f 6e73 655f 7479 7065     response_type
 000162b0: 735f 6d61 7020 3d20 7b0a 2020 2020 2020  s_map = {.      
@@ -6418,15 +6418,15 @@
 00019110: 7468 6520 4c55 5349 4420 6865 6164 6572  the LUSID header
 00019120: 0a20 2020 2020 2020 2068 6561 6465 725f  .        header_
 00019130: 7061 7261 6d73 5b27 582d 4c55 5349 442d  params['X-LUSID-
 00019140: 5344 4b2d 4c61 6e67 7561 6765 275d 203d  SDK-Language'] =
 00019150: 2027 5079 7468 6f6e 270a 2020 2020 2020   'Python'.      
 00019160: 2020 6865 6164 6572 5f70 6172 616d 735b    header_params[
 00019170: 2758 2d4c 5553 4944 2d53 444b 2d56 6572  'X-LUSID-SDK-Ver
-00019180: 7369 6f6e 275d 203d 2027 312e 302e 3931  sion'] = '1.0.91
+00019180: 7369 6f6e 275d 203d 2027 312e 302e 3938  sion'] = '1.0.98
 00019190: 270a 0a20 2020 2020 2020 2023 2041 7574  '..        # Aut
 000191a0: 6865 6e74 6963 6174 696f 6e20 7365 7474  hentication sett
 000191b0: 696e 670a 2020 2020 2020 2020 6175 7468  ing.        auth
 000191c0: 5f73 6574 7469 6e67 7320 3d20 5b27 6f61  _settings = ['oa
 000191d0: 7574 6832 275d 2020 2320 6e6f 7161 3a20  uth2']  # noqa: 
 000191e0: 4535 3031 0a0a 2020 2020 2020 2020 7265  E501..        re
 000191f0: 7370 6f6e 7365 5f74 7970 6573 5f6d 6170  sponse_types_map
@@ -7409,15 +7409,15 @@
 0001cf00: 6572 0a20 2020 2020 2020 2068 6561 6465  er.        heade
 0001cf10: 725f 7061 7261 6d73 5b27 582d 4c55 5349  r_params['X-LUSI
 0001cf20: 442d 5344 4b2d 4c61 6e67 7561 6765 275d  D-SDK-Language']
 0001cf30: 203d 2027 5079 7468 6f6e 270a 2020 2020   = 'Python'.    
 0001cf40: 2020 2020 6865 6164 6572 5f70 6172 616d      header_param
 0001cf50: 735b 2758 2d4c 5553 4944 2d53 444b 2d56  s['X-LUSID-SDK-V
 0001cf60: 6572 7369 6f6e 275d 203d 2027 312e 302e  ersion'] = '1.0.
-0001cf70: 3931 270a 0a20 2020 2020 2020 2023 2041  91'..        # A
+0001cf70: 3938 270a 0a20 2020 2020 2020 2023 2041  98'..        # A
 0001cf80: 7574 6865 6e74 6963 6174 696f 6e20 7365  uthentication se
 0001cf90: 7474 696e 670a 2020 2020 2020 2020 6175  tting.        au
 0001cfa0: 7468 5f73 6574 7469 6e67 7320 3d20 5b27  th_settings = ['
 0001cfb0: 6f61 7574 6832 275d 2020 2320 6e6f 7161  oauth2']  # noqa
 0001cfc0: 3a20 4535 3031 0a0a 2020 2020 2020 2020  : E501..        
 0001cfd0: 7265 7370 6f6e 7365 5f74 7970 6573 5f6d  response_types_m
 0001cfe0: 6170 203d 207b 0a20 2020 2020 2020 2020  ap = {.         
@@ -8416,15 +8416,15 @@
 00020df0: 6561 6465 720a 2020 2020 2020 2020 6865  eader.        he
 00020e00: 6164 6572 5f70 6172 616d 735b 2758 2d4c  ader_params['X-L
 00020e10: 5553 4944 2d53 444b 2d4c 616e 6775 6167  USID-SDK-Languag
 00020e20: 6527 5d20 3d20 2750 7974 686f 6e27 0a20  e'] = 'Python'. 
 00020e30: 2020 2020 2020 2068 6561 6465 725f 7061         header_pa
 00020e40: 7261 6d73 5b27 582d 4c55 5349 442d 5344  rams['X-LUSID-SD
 00020e50: 4b2d 5665 7273 696f 6e27 5d20 3d20 2731  K-Version'] = '1
-00020e60: 2e30 2e39 3127 0a0a 2020 2020 2020 2020  .0.91'..        
+00020e60: 2e30 2e39 3827 0a0a 2020 2020 2020 2020  .0.98'..        
 00020e70: 2320 4175 7468 656e 7469 6361 7469 6f6e  # Authentication
 00020e80: 2073 6574 7469 6e67 0a20 2020 2020 2020   setting.       
 00020e90: 2061 7574 685f 7365 7474 696e 6773 203d   auth_settings =
 00020ea0: 205b 276f 6175 7468 3227 5d20 2023 206e   ['oauth2']  # n
 00020eb0: 6f71 613a 2045 3530 310a 0a20 2020 2020  oqa: E501..     
 00020ec0: 2020 2072 6573 706f 6e73 655f 7479 7065     response_type
 00020ed0: 735f 6d61 7020 3d20 7b0a 2020 2020 2020  s_map = {.      
@@ -9082,15 +9082,15 @@
 00023790: 6865 6164 6572 0a20 2020 2020 2020 2068  header.        h
 000237a0: 6561 6465 725f 7061 7261 6d73 5b27 582d  eader_params['X-
 000237b0: 4c55 5349 442d 5344 4b2d 4c61 6e67 7561  LUSID-SDK-Langua
 000237c0: 6765 275d 203d 2027 5079 7468 6f6e 270a  ge'] = 'Python'.
 000237d0: 2020 2020 2020 2020 6865 6164 6572 5f70          header_p
 000237e0: 6172 616d 735b 2758 2d4c 5553 4944 2d53  arams['X-LUSID-S
 000237f0: 444b 2d56 6572 7369 6f6e 275d 203d 2027  DK-Version'] = '
-00023800: 312e 302e 3931 270a 0a20 2020 2020 2020  1.0.91'..       
+00023800: 312e 302e 3938 270a 0a20 2020 2020 2020  1.0.98'..       
 00023810: 2023 2041 7574 6865 6e74 6963 6174 696f   # Authenticatio
 00023820: 6e20 7365 7474 696e 670a 2020 2020 2020  n setting.      
 00023830: 2020 6175 7468 5f73 6574 7469 6e67 7320    auth_settings 
 00023840: 3d20 5b27 6f61 7574 6832 275d 2020 2320  = ['oauth2']  # 
 00023850: 6e6f 7161 3a20 4535 3031 0a0a 2020 2020  noqa: E501..    
 00023860: 2020 2020 7265 7370 6f6e 7365 5f74 7970      response_typ
 00023870: 6573 5f6d 6170 203d 207b 0a20 2020 2020  es_map = {.     
@@ -9959,15 +9959,15 @@
 00026e60: 6572 0a20 2020 2020 2020 2068 6561 6465  er.        heade
 00026e70: 725f 7061 7261 6d73 5b27 582d 4c55 5349  r_params['X-LUSI
 00026e80: 442d 5344 4b2d 4c61 6e67 7561 6765 275d  D-SDK-Language']
 00026e90: 203d 2027 5079 7468 6f6e 270a 2020 2020   = 'Python'.    
 00026ea0: 2020 2020 6865 6164 6572 5f70 6172 616d      header_param
 00026eb0: 735b 2758 2d4c 5553 4944 2d53 444b 2d56  s['X-LUSID-SDK-V
 00026ec0: 6572 7369 6f6e 275d 203d 2027 312e 302e  ersion'] = '1.0.
-00026ed0: 3931 270a 0a20 2020 2020 2020 2023 2041  91'..        # A
+00026ed0: 3938 270a 0a20 2020 2020 2020 2023 2041  98'..        # A
 00026ee0: 7574 6865 6e74 6963 6174 696f 6e20 7365  uthentication se
 00026ef0: 7474 696e 670a 2020 2020 2020 2020 6175  tting.        au
 00026f00: 7468 5f73 6574 7469 6e67 7320 3d20 5b27  th_settings = ['
 00026f10: 6f61 7574 6832 275d 2020 2320 6e6f 7161  oauth2']  # noqa
 00026f20: 3a20 4535 3031 0a0a 2020 2020 2020 2020  : E501..        
 00026f30: 7265 7370 6f6e 7365 5f74 7970 6573 5f6d  response_types_m
 00026f40: 6170 203d 207b 0a20 2020 2020 2020 2020  ap = {.         
@@ -10732,15 +10732,15 @@
 00029eb0: 5553 4944 2068 6561 6465 720a 2020 2020  USID header.    
 00029ec0: 2020 2020 6865 6164 6572 5f70 6172 616d      header_param
 00029ed0: 735b 2758 2d4c 5553 4944 2d53 444b 2d4c  s['X-LUSID-SDK-L
 00029ee0: 616e 6775 6167 6527 5d20 3d20 2750 7974  anguage'] = 'Pyt
 00029ef0: 686f 6e27 0a20 2020 2020 2020 2068 6561  hon'.        hea
 00029f00: 6465 725f 7061 7261 6d73 5b27 582d 4c55  der_params['X-LU
 00029f10: 5349 442d 5344 4b2d 5665 7273 696f 6e27  SID-SDK-Version'
-00029f20: 5d20 3d20 2731 2e30 2e39 3127 0a0a 2020  ] = '1.0.91'..  
+00029f20: 5d20 3d20 2731 2e30 2e39 3827 0a0a 2020  ] = '1.0.98'..  
 00029f30: 2020 2020 2020 2320 4175 7468 656e 7469        # Authenti
 00029f40: 6361 7469 6f6e 2073 6574 7469 6e67 0a20  cation setting. 
 00029f50: 2020 2020 2020 2061 7574 685f 7365 7474         auth_sett
 00029f60: 696e 6773 203d 205b 276f 6175 7468 3227  ings = ['oauth2'
 00029f70: 5d20 2023 206e 6f71 613a 2045 3530 310a  ]  # noqa: E501.
 00029f80: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
 00029f90: 655f 7479 7065 735f 6d61 7020 3d20 7b0a  e_types_map = {.
@@ -11898,15 +11898,15 @@
 0002e790: 6465 720a 2020 2020 2020 2020 6865 6164  der.        head
 0002e7a0: 6572 5f70 6172 616d 735b 2758 2d4c 5553  er_params['X-LUS
 0002e7b0: 4944 2d53 444b 2d4c 616e 6775 6167 6527  ID-SDK-Language'
 0002e7c0: 5d20 3d20 2750 7974 686f 6e27 0a20 2020  ] = 'Python'.   
 0002e7d0: 2020 2020 2068 6561 6465 725f 7061 7261       header_para
 0002e7e0: 6d73 5b27 582d 4c55 5349 442d 5344 4b2d  ms['X-LUSID-SDK-
 0002e7f0: 5665 7273 696f 6e27 5d20 3d20 2731 2e30  Version'] = '1.0
-0002e800: 2e39 3127 0a0a 2020 2020 2020 2020 2320  .91'..        # 
+0002e800: 2e39 3827 0a0a 2020 2020 2020 2020 2320  .98'..        # 
 0002e810: 4175 7468 656e 7469 6361 7469 6f6e 2073  Authentication s
 0002e820: 6574 7469 6e67 0a20 2020 2020 2020 2061  etting.        a
 0002e830: 7574 685f 7365 7474 696e 6773 203d 205b  uth_settings = [
 0002e840: 276f 6175 7468 3227 5d20 2023 206e 6f71  'oauth2']  # noq
 0002e850: 613a 2045 3530 310a 0a20 2020 2020 2020  a: E501..       
 0002e860: 2072 6573 706f 6e73 655f 7479 7065 735f   response_types_
 0002e870: 6d61 7020 3d20 7b0a 2020 2020 2020 2020  map = {.        
@@ -12869,15 +12869,15 @@
 00032440: 204c 5553 4944 2068 6561 6465 720a 2020   LUSID header.  
 00032450: 2020 2020 2020 6865 6164 6572 5f70 6172        header_par
 00032460: 616d 735b 2758 2d4c 5553 4944 2d53 444b  ams['X-LUSID-SDK
 00032470: 2d4c 616e 6775 6167 6527 5d20 3d20 2750  -Language'] = 'P
 00032480: 7974 686f 6e27 0a20 2020 2020 2020 2068  ython'.        h
 00032490: 6561 6465 725f 7061 7261 6d73 5b27 582d  eader_params['X-
 000324a0: 4c55 5349 442d 5344 4b2d 5665 7273 696f  LUSID-SDK-Versio
-000324b0: 6e27 5d20 3d20 2731 2e30 2e39 3127 0a0a  n'] = '1.0.91'..
+000324b0: 6e27 5d20 3d20 2731 2e30 2e39 3827 0a0a  n'] = '1.0.98'..
 000324c0: 2020 2020 2020 2020 2320 4175 7468 656e          # Authen
 000324d0: 7469 6361 7469 6f6e 2073 6574 7469 6e67  tication setting
 000324e0: 0a20 2020 2020 2020 2061 7574 685f 7365  .        auth_se
 000324f0: 7474 696e 6773 203d 205b 276f 6175 7468  ttings = ['oauth
 00032500: 3227 5d20 2023 206e 6f71 613a 2045 3530  2']  # noqa: E50
 00032510: 310a 0a20 2020 2020 2020 2072 6573 706f  1..        respo
 00032520: 6e73 655f 7479 7065 735f 6d61 7020 3d20  nse_types_map = 
@@ -13563,15 +13563,15 @@
 00034fa0: 6520 4c55 5349 4420 6865 6164 6572 0a20  e LUSID header. 
 00034fb0: 2020 2020 2020 2068 6561 6465 725f 7061         header_pa
 00034fc0: 7261 6d73 5b27 582d 4c55 5349 442d 5344  rams['X-LUSID-SD
 00034fd0: 4b2d 4c61 6e67 7561 6765 275d 203d 2027  K-Language'] = '
 00034fe0: 5079 7468 6f6e 270a 2020 2020 2020 2020  Python'.        
 00034ff0: 6865 6164 6572 5f70 6172 616d 735b 2758  header_params['X
 00035000: 2d4c 5553 4944 2d53 444b 2d56 6572 7369  -LUSID-SDK-Versi
-00035010: 6f6e 275d 203d 2027 312e 302e 3931 270a  on'] = '1.0.91'.
+00035010: 6f6e 275d 203d 2027 312e 302e 3938 270a  on'] = '1.0.98'.
 00035020: 0a20 2020 2020 2020 2023 2041 7574 6865  .        # Authe
 00035030: 6e74 6963 6174 696f 6e20 7365 7474 696e  ntication settin
 00035040: 670a 2020 2020 2020 2020 6175 7468 5f73  g.        auth_s
 00035050: 6574 7469 6e67 7320 3d20 5b27 6f61 7574  ettings = ['oaut
 00035060: 6832 275d 2020 2320 6e6f 7161 3a20 4535  h2']  # noqa: E5
 00035070: 3031 0a0a 2020 2020 2020 2020 7265 7370  01..        resp
 00035080: 6f6e 7365 5f74 7970 6573 5f6d 6170 203d  onse_types_map =
@@ -14715,15 +14715,15 @@
 000397a0: 6164 6572 0a20 2020 2020 2020 2068 6561  ader.        hea
 000397b0: 6465 725f 7061 7261 6d73 5b27 582d 4c55  der_params['X-LU
 000397c0: 5349 442d 5344 4b2d 4c61 6e67 7561 6765  SID-SDK-Language
 000397d0: 275d 203d 2027 5079 7468 6f6e 270a 2020  '] = 'Python'.  
 000397e0: 2020 2020 2020 6865 6164 6572 5f70 6172        header_par
 000397f0: 616d 735b 2758 2d4c 5553 4944 2d53 444b  ams['X-LUSID-SDK
 00039800: 2d56 6572 7369 6f6e 275d 203d 2027 312e  -Version'] = '1.
-00039810: 302e 3931 270a 0a20 2020 2020 2020 2023  0.91'..        #
+00039810: 302e 3938 270a 0a20 2020 2020 2020 2023  0.98'..        #
 00039820: 2041 7574 6865 6e74 6963 6174 696f 6e20   Authentication 
 00039830: 7365 7474 696e 670a 2020 2020 2020 2020  setting.        
 00039840: 6175 7468 5f73 6574 7469 6e67 7320 3d20  auth_settings = 
 00039850: 5b27 6f61 7574 6832 275d 2020 2320 6e6f  ['oauth2']  # no
 00039860: 7161 3a20 4535 3031 0a0a 2020 2020 2020  qa: E501..      
 00039870: 2020 7265 7370 6f6e 7365 5f74 7970 6573    response_types
 00039880: 5f6d 6170 203d 207b 0a20 2020 2020 2020  _map = {.       
@@ -15453,15 +15453,15 @@
 0003c5c0: 6865 6164 6572 0a20 2020 2020 2020 2068  header.        h
 0003c5d0: 6561 6465 725f 7061 7261 6d73 5b27 582d  eader_params['X-
 0003c5e0: 4c55 5349 442d 5344 4b2d 4c61 6e67 7561  LUSID-SDK-Langua
 0003c5f0: 6765 275d 203d 2027 5079 7468 6f6e 270a  ge'] = 'Python'.
 0003c600: 2020 2020 2020 2020 6865 6164 6572 5f70          header_p
 0003c610: 6172 616d 735b 2758 2d4c 5553 4944 2d53  arams['X-LUSID-S
 0003c620: 444b 2d56 6572 7369 6f6e 275d 203d 2027  DK-Version'] = '
-0003c630: 312e 302e 3931 270a 0a20 2020 2020 2020  1.0.91'..       
+0003c630: 312e 302e 3938 270a 0a20 2020 2020 2020  1.0.98'..       
 0003c640: 2023 2041 7574 6865 6e74 6963 6174 696f   # Authenticatio
 0003c650: 6e20 7365 7474 696e 670a 2020 2020 2020  n setting.      
 0003c660: 2020 6175 7468 5f73 6574 7469 6e67 7320    auth_settings 
 0003c670: 3d20 5b27 6f61 7574 6832 275d 2020 2320  = ['oauth2']  # 
 0003c680: 6e6f 7161 3a20 4535 3031 0a0a 2020 2020  noqa: E501..    
 0003c690: 2020 2020 7265 7370 6f6e 7365 5f74 7970      response_typ
 0003c6a0: 6573 5f6d 6170 203d 207b 0a20 2020 2020  es_map = {.     
@@ -16218,15 +16218,15 @@
 0003f590: 720a 2020 2020 2020 2020 6865 6164 6572  r.        header
 0003f5a0: 5f70 6172 616d 735b 2758 2d4c 5553 4944  _params['X-LUSID
 0003f5b0: 2d53 444b 2d4c 616e 6775 6167 6527 5d20  -SDK-Language'] 
 0003f5c0: 3d20 2750 7974 686f 6e27 0a20 2020 2020  = 'Python'.     
 0003f5d0: 2020 2068 6561 6465 725f 7061 7261 6d73     header_params
 0003f5e0: 5b27 582d 4c55 5349 442d 5344 4b2d 5665  ['X-LUSID-SDK-Ve
 0003f5f0: 7273 696f 6e27 5d20 3d20 2731 2e30 2e39  rsion'] = '1.0.9
-0003f600: 3127 0a0a 2020 2020 2020 2020 2320 4175  1'..        # Au
+0003f600: 3827 0a0a 2020 2020 2020 2020 2320 4175  8'..        # Au
 0003f610: 7468 656e 7469 6361 7469 6f6e 2073 6574  thentication set
 0003f620: 7469 6e67 0a20 2020 2020 2020 2061 7574  ting.        aut
 0003f630: 685f 7365 7474 696e 6773 203d 205b 276f  h_settings = ['o
 0003f640: 6175 7468 3227 5d20 2023 206e 6f71 613a  auth2']  # noqa:
 0003f650: 2045 3530 310a 0a20 2020 2020 2020 2072   E501..        r
 0003f660: 6573 706f 6e73 655f 7479 7065 735f 6d61  esponse_types_ma
 0003f670: 7020 3d20 7b0a 2020 2020 2020 2020 2020  p = {.          
@@ -17129,15 +17129,15 @@
 00042e80: 6561 6465 720a 2020 2020 2020 2020 6865  eader.        he
 00042e90: 6164 6572 5f70 6172 616d 735b 2758 2d4c  ader_params['X-L
 00042ea0: 5553 4944 2d53 444b 2d4c 616e 6775 6167  USID-SDK-Languag
 00042eb0: 6527 5d20 3d20 2750 7974 686f 6e27 0a20  e'] = 'Python'. 
 00042ec0: 2020 2020 2020 2068 6561 6465 725f 7061         header_pa
 00042ed0: 7261 6d73 5b27 582d 4c55 5349 442d 5344  rams['X-LUSID-SD
 00042ee0: 4b2d 5665 7273 696f 6e27 5d20 3d20 2731  K-Version'] = '1
-00042ef0: 2e30 2e39 3127 0a0a 2020 2020 2020 2020  .0.91'..        
+00042ef0: 2e30 2e39 3827 0a0a 2020 2020 2020 2020  .0.98'..        
 00042f00: 2320 4175 7468 656e 7469 6361 7469 6f6e  # Authentication
 00042f10: 2073 6574 7469 6e67 0a20 2020 2020 2020   setting.       
 00042f20: 2061 7574 685f 7365 7474 696e 6773 203d   auth_settings =
 00042f30: 205b 276f 6175 7468 3227 5d20 2023 206e   ['oauth2']  # n
 00042f40: 6f71 613a 2045 3530 310a 0a20 2020 2020  oqa: E501..     
 00042f50: 2020 2072 6573 706f 6e73 655f 7479 7065     response_type
 00042f60: 735f 6d61 7020 3d20 7b0a 2020 2020 2020  s_map = {.      
@@ -17949,15 +17949,15 @@
 000461c0: 6865 6164 6572 0a20 2020 2020 2020 2068  header.        h
 000461d0: 6561 6465 725f 7061 7261 6d73 5b27 582d  eader_params['X-
 000461e0: 4c55 5349 442d 5344 4b2d 4c61 6e67 7561  LUSID-SDK-Langua
 000461f0: 6765 275d 203d 2027 5079 7468 6f6e 270a  ge'] = 'Python'.
 00046200: 2020 2020 2020 2020 6865 6164 6572 5f70          header_p
 00046210: 6172 616d 735b 2758 2d4c 5553 4944 2d53  arams['X-LUSID-S
 00046220: 444b 2d56 6572 7369 6f6e 275d 203d 2027  DK-Version'] = '
-00046230: 312e 302e 3931 270a 0a20 2020 2020 2020  1.0.91'..       
+00046230: 312e 302e 3938 270a 0a20 2020 2020 2020  1.0.98'..       
 00046240: 2023 2041 7574 6865 6e74 6963 6174 696f   # Authenticatio
 00046250: 6e20 7365 7474 696e 670a 2020 2020 2020  n setting.      
 00046260: 2020 6175 7468 5f73 6574 7469 6e67 7320    auth_settings 
 00046270: 3d20 5b27 6f61 7574 6832 275d 2020 2320  = ['oauth2']  # 
 00046280: 6e6f 7161 3a20 4535 3031 0a0a 2020 2020  noqa: E501..    
 00046290: 2020 2020 7265 7370 6f6e 7365 5f74 7970      response_typ
 000462a0: 6573 5f6d 6170 203d 207b 0a20 2020 2020  es_map = {.     
@@ -18708,15 +18708,15 @@
 00049130: 4c55 5349 4420 6865 6164 6572 0a20 2020  LUSID header.   
 00049140: 2020 2020 2068 6561 6465 725f 7061 7261       header_para
 00049150: 6d73 5b27 582d 4c55 5349 442d 5344 4b2d  ms['X-LUSID-SDK-
 00049160: 4c61 6e67 7561 6765 275d 203d 2027 5079  Language'] = 'Py
 00049170: 7468 6f6e 270a 2020 2020 2020 2020 6865  thon'.        he
 00049180: 6164 6572 5f70 6172 616d 735b 2758 2d4c  ader_params['X-L
 00049190: 5553 4944 2d53 444b 2d56 6572 7369 6f6e  USID-SDK-Version
-000491a0: 275d 203d 2027 312e 302e 3931 270a 0a20  '] = '1.0.91'.. 
+000491a0: 275d 203d 2027 312e 302e 3938 270a 0a20  '] = '1.0.98'.. 
 000491b0: 2020 2020 2020 2023 2041 7574 6865 6e74         # Authent
 000491c0: 6963 6174 696f 6e20 7365 7474 696e 670a  ication setting.
 000491d0: 2020 2020 2020 2020 6175 7468 5f73 6574          auth_set
 000491e0: 7469 6e67 7320 3d20 5b27 6f61 7574 6832  tings = ['oauth2
 000491f0: 275d 2020 2320 6e6f 7161 3a20 4535 3031  ']  # noqa: E501
 00049200: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
 00049210: 7365 5f74 7970 6573 5f6d 6170 203d 207b  se_types_map = {
@@ -19474,15 +19474,15 @@
 0004c110: 6520 4c55 5349 4420 6865 6164 6572 0a20  e LUSID header. 
 0004c120: 2020 2020 2020 2068 6561 6465 725f 7061         header_pa
 0004c130: 7261 6d73 5b27 582d 4c55 5349 442d 5344  rams['X-LUSID-SD
 0004c140: 4b2d 4c61 6e67 7561 6765 275d 203d 2027  K-Language'] = '
 0004c150: 5079 7468 6f6e 270a 2020 2020 2020 2020  Python'.        
 0004c160: 6865 6164 6572 5f70 6172 616d 735b 2758  header_params['X
 0004c170: 2d4c 5553 4944 2d53 444b 2d56 6572 7369  -LUSID-SDK-Versi
-0004c180: 6f6e 275d 203d 2027 312e 302e 3931 270a  on'] = '1.0.91'.
+0004c180: 6f6e 275d 203d 2027 312e 302e 3938 270a  on'] = '1.0.98'.
 0004c190: 0a20 2020 2020 2020 2023 2041 7574 6865  .        # Authe
 0004c1a0: 6e74 6963 6174 696f 6e20 7365 7474 696e  ntication settin
 0004c1b0: 670a 2020 2020 2020 2020 6175 7468 5f73  g.        auth_s
 0004c1c0: 6574 7469 6e67 7320 3d20 5b27 6f61 7574  ettings = ['oaut
 0004c1d0: 6832 275d 2020 2320 6e6f 7161 3a20 4535  h2']  # noqa: E5
 0004c1e0: 3031 0a0a 2020 2020 2020 2020 7265 7370  01..        resp
 0004c1f0: 6f6e 7365 5f74 7970 6573 5f6d 6170 203d  onse_types_map =
@@ -20169,15 +20169,15 @@
 0004ec80: 6164 6572 0a20 2020 2020 2020 2068 6561  ader.        hea
 0004ec90: 6465 725f 7061 7261 6d73 5b27 582d 4c55  der_params['X-LU
 0004eca0: 5349 442d 5344 4b2d 4c61 6e67 7561 6765  SID-SDK-Language
 0004ecb0: 275d 203d 2027 5079 7468 6f6e 270a 2020  '] = 'Python'.  
 0004ecc0: 2020 2020 2020 6865 6164 6572 5f70 6172        header_par
 0004ecd0: 616d 735b 2758 2d4c 5553 4944 2d53 444b  ams['X-LUSID-SDK
 0004ece0: 2d56 6572 7369 6f6e 275d 203d 2027 312e  -Version'] = '1.
-0004ecf0: 302e 3931 270a 0a20 2020 2020 2020 2023  0.91'..        #
+0004ecf0: 302e 3938 270a 0a20 2020 2020 2020 2023  0.98'..        #
 0004ed00: 2041 7574 6865 6e74 6963 6174 696f 6e20   Authentication 
 0004ed10: 7365 7474 696e 670a 2020 2020 2020 2020  setting.        
 0004ed20: 6175 7468 5f73 6574 7469 6e67 7320 3d20  auth_settings = 
 0004ed30: 5b27 6f61 7574 6832 275d 2020 2320 6e6f  ['oauth2']  # no
 0004ed40: 7161 3a20 4535 3031 0a0a 2020 2020 2020  qa: E501..      
 0004ed50: 2020 7265 7370 6f6e 7365 5f74 7970 6573    response_types
 0004ed60: 5f6d 6170 203d 207b 0a20 2020 2020 2020  _map = {.
```

### Comparing `lusid-sdk-1.0.91/lusid/api_client.py` & `lusid-sdk-1.0.98/lusid/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.91/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.98/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-sdk-1.0.91/lusid/configuration.py` & `lusid-sdk-1.0.98/lusid/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.91\n"\
-               "SDK Package Version: 1.0.91".\
+               "Version of the API: 1.0.98\n"\
+               "SDK Package Version: 1.0.98".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-sdk-1.0.91/lusid/exceptions.py` & `lusid-sdk-1.0.98/lusid/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-sdk-1.0.91/lusid/models/__init__.py` & `lusid-sdk-1.0.98/lusid/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-sdk-1.0.91/lusid/models/a2_b_breakdown.py` & `lusid-sdk-1.0.98/lusid/models/a2_b_breakdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/a2_b_category.py` & `lusid-sdk-1.0.98/lusid/models/a2_b_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/a2_b_data_record.py` & `lusid-sdk-1.0.98/lusid/models/a2_b_data_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/a2_b_movement_record.py` & `lusid-sdk-1.0.98/lusid/models/a2_b_movement_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/access_controlled_action.py` & `lusid-sdk-1.0.98/lusid/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/access_controlled_resource.py` & `lusid-sdk-1.0.98/lusid/models/access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/access_metadata_operation.py` & `lusid-sdk-1.0.98/lusid/models/access_metadata_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/access_metadata_value.py` & `lusid-sdk-1.0.98/lusid/models/access_metadata_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/action_id.py` & `lusid-sdk-1.0.98/lusid/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/action_result_of_portfolio.py` & `lusid-sdk-1.0.98/lusid/models/action_result_of_portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/add_business_days_to_date_request.py` & `lusid-sdk-1.0.98/lusid/models/add_business_days_to_date_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/add_business_days_to_date_response.py` & `lusid-sdk-1.0.98/lusid/models/add_business_days_to_date_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/address_definition.py` & `lusid-sdk-1.0.98/lusid/models/address_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/address_key_filter.py` & `lusid-sdk-1.0.98/lusid/models/address_key_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/address_key_option_definition.py` & `lusid-sdk-1.0.98/lusid/models/address_key_option_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/adjust_holding.py` & `lusid-sdk-1.0.98/lusid/models/adjust_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/adjust_holding_for_date_request.py` & `lusid-sdk-1.0.98/lusid/models/adjust_holding_for_date_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/adjust_holding_request.py` & `lusid-sdk-1.0.98/lusid/models/adjust_holding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregate_spec.py` & `lusid-sdk-1.0.98/lusid/models/aggregate_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregated_return.py` & `lusid-sdk-1.0.98/lusid/models/aggregated_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregated_returns_request.py` & `lusid-sdk-1.0.98/lusid/models/aggregated_returns_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregated_returns_response.py` & `lusid-sdk-1.0.98/lusid/models/aggregated_returns_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregation.py` & `lusid-sdk-1.0.98/lusid/models/aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregation_context.py` & `lusid-sdk-1.0.98/lusid/models/aggregation_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregation_measure_failure_detail.py` & `lusid-sdk-1.0.98/lusid/models/aggregation_measure_failure_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregation_options.py` & `lusid-sdk-1.0.98/lusid/models/aggregation_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/aggregation_query.py` & `lusid-sdk-1.0.98/lusid/models/aggregation_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/allocation.py` & `lusid-sdk-1.0.98/lusid/models/allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/allocation_request.py` & `lusid-sdk-1.0.98/lusid/models/allocation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/allocation_set_request.py` & `lusid-sdk-1.0.98/lusid/models/allocation_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/amortisation_event.py` & `lusid-sdk-1.0.98/lusid/models/amortisation_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/amortisation_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/amortisation_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/annul_quotes_response.py` & `lusid-sdk-1.0.98/lusid/models/annul_quotes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/annul_single_structured_data_response.py` & `lusid-sdk-1.0.98/lusid/models/annul_single_structured_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/annul_structured_data_response.py` & `lusid-sdk-1.0.98/lusid/models/annul_structured_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/barrier.py` & `lusid-sdk-1.0.98/lusid/models/barrier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/basket.py` & `lusid-sdk-1.0.98/lusid/models/basket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/basket_all_of.py` & `lusid-sdk-1.0.98/lusid/models/basket_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/basket_identifier.py` & `lusid-sdk-1.0.98/lusid/models/basket_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/batch_adjust_holdings_response.py` & `lusid-sdk-1.0.98/lusid/models/batch_adjust_holdings_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/batch_upsert_portfolio_transactions_response.py` & `lusid-sdk-1.0.98/lusid/models/batch_upsert_portfolio_transactions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/block.py` & `lusid-sdk-1.0.98/lusid/models/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/block_request.py` & `lusid-sdk-1.0.98/lusid/models/block_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/block_set_request.py` & `lusid-sdk-1.0.98/lusid/models/block_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/bond.py` & `lusid-sdk-1.0.98/lusid/models/bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/bond_all_of.py` & `lusid-sdk-1.0.98/lusid/models/bond_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/bond_default_event.py` & `lusid-sdk-1.0.98/lusid/models/bond_default_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/bond_default_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/bond_default_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/calendar.py` & `lusid-sdk-1.0.98/lusid/models/calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/calendar_date.py` & `lusid-sdk-1.0.98/lusid/models/calendar_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cap_floor.py` & `lusid-sdk-1.0.98/lusid/models/cap_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cap_floor_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cap_floor_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_dividend_event.py` & `lusid-sdk-1.0.98/lusid/models/cash_dividend_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_dividend_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cash_dividend_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_event.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_lineage.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_lineage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_value.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_value_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_value_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_value_set.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_value_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_flow_value_set_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cash_flow_value_set_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_ladder_record.py` & `lusid-sdk-1.0.98/lusid/models/cash_ladder_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_perpetual.py` & `lusid-sdk-1.0.98/lusid/models/cash_perpetual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cash_perpetual_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cash_perpetual_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cds_flow_conventions.py` & `lusid-sdk-1.0.98/lusid/models/cds_flow_conventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cds_index.py` & `lusid-sdk-1.0.98/lusid/models/cds_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cds_index_all_of.py` & `lusid-sdk-1.0.98/lusid/models/cds_index_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cds_protection_detail_specification.py` & `lusid-sdk-1.0.98/lusid/models/cds_protection_detail_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/change.py` & `lusid-sdk-1.0.98/lusid/models/change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/change_history.py` & `lusid-sdk-1.0.98/lusid/models/change_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/change_item.py` & `lusid-sdk-1.0.98/lusid/models/change_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/close_event.py` & `lusid-sdk-1.0.98/lusid/models/close_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/close_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/close_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/complete_portfolio.py` & `lusid-sdk-1.0.98/lusid/models/complete_portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/complete_relationship.py` & `lusid-sdk-1.0.98/lusid/models/complete_relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/complex_bond.py` & `lusid-sdk-1.0.98/lusid/models/complex_bond.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/complex_bond_all_of.py` & `lusid-sdk-1.0.98/lusid/models/complex_bond_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/complex_market_data.py` & `lusid-sdk-1.0.98/lusid/models/complex_market_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/complex_market_data_id.py` & `lusid-sdk-1.0.98/lusid/models/complex_market_data_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/compounding.py` & `lusid-sdk-1.0.98/lusid/models/compounding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/configuration_recipe.py` & `lusid-sdk-1.0.98/lusid/models/configuration_recipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/configuration_recipe_snippet.py` & `lusid-sdk-1.0.98/lusid/models/configuration_recipe_snippet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/constituents_adjustment_header.py` & `lusid-sdk-1.0.98/lusid/models/constituents_adjustment_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/contract_for_difference.py` & `lusid-sdk-1.0.98/lusid/models/contract_for_difference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/contract_for_difference_all_of.py` & `lusid-sdk-1.0.98/lusid/models/contract_for_difference_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/corporate_action.py` & `lusid-sdk-1.0.98/lusid/models/corporate_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/corporate_action_source.py` & `lusid-sdk-1.0.98/lusid/models/corporate_action_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/corporate_action_transition.py` & `lusid-sdk-1.0.98/lusid/models/corporate_action_transition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/corporate_action_transition_component.py` & `lusid-sdk-1.0.98/lusid/models/corporate_action_transition_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/corporate_action_transition_component_request.py` & `lusid-sdk-1.0.98/lusid/models/corporate_action_transition_component_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/corporate_action_transition_request.py` & `lusid-sdk-1.0.98/lusid/models/corporate_action_transition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/counterparty_agreement.py` & `lusid-sdk-1.0.98/lusid/models/counterparty_agreement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/counterparty_risk_information.py` & `lusid-sdk-1.0.98/lusid/models/counterparty_risk_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/counterparty_signatory.py` & `lusid-sdk-1.0.98/lusid/models/counterparty_signatory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_calendar_request.py` & `lusid-sdk-1.0.98/lusid/models/create_calendar_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_corporate_action_source_request.py` & `lusid-sdk-1.0.98/lusid/models/create_corporate_action_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_cut_label_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/create_cut_label_definition_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_data_type_request.py` & `lusid-sdk-1.0.98/lusid/models/create_data_type_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_date_request.py` & `lusid-sdk-1.0.98/lusid/models/create_date_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_derived_property_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/create_derived_property_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_derived_transaction_portfolio_request.py` & `lusid-sdk-1.0.98/lusid/models/create_derived_transaction_portfolio_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_portfolio_details.py` & `lusid-sdk-1.0.98/lusid/models/create_portfolio_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_portfolio_group_request.py` & `lusid-sdk-1.0.98/lusid/models/create_portfolio_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_property_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/create_property_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_reference_portfolio_request.py` & `lusid-sdk-1.0.98/lusid/models/create_reference_portfolio_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_relationship_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/create_relationship_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_relationship_request.py` & `lusid-sdk-1.0.98/lusid/models/create_relationship_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_sequence_request.py` & `lusid-sdk-1.0.98/lusid/models/create_sequence_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_transaction_portfolio_request.py` & `lusid-sdk-1.0.98/lusid/models/create_transaction_portfolio_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/create_unit_definition.py` & `lusid-sdk-1.0.98/lusid/models/create_unit_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/credit_default_swap.py` & `lusid-sdk-1.0.98/lusid/models/credit_default_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/credit_default_swap_all_of.py` & `lusid-sdk-1.0.98/lusid/models/credit_default_swap_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/credit_rating.py` & `lusid-sdk-1.0.98/lusid/models/credit_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/credit_spread_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/credit_spread_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/credit_spread_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/credit_spread_curve_data_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/credit_support_annex.py` & `lusid-sdk-1.0.98/lusid/models/credit_support_annex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/currency_and_amount.py` & `lusid-sdk-1.0.98/lusid/models/currency_and_amount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custodian_account.py` & `lusid-sdk-1.0.98/lusid/models/custodian_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_definition.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_field.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_field_definition.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_id.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_request.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/custom_entity_response.py` & `lusid-sdk-1.0.98/lusid/models/custom_entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cut_label_definition.py` & `lusid-sdk-1.0.98/lusid/models/cut_label_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/cut_local_time.py` & `lusid-sdk-1.0.98/lusid/models/cut_local_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/data_type.py` & `lusid-sdk-1.0.98/lusid/models/data_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/data_type_summary.py` & `lusid-sdk-1.0.98/lusid/models/data_type_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/date_attributes.py` & `lusid-sdk-1.0.98/lusid/models/date_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/date_range.py` & `lusid-sdk-1.0.98/lusid/models/date_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/day_of_week.py` & `lusid-sdk-1.0.98/lusid/models/day_of_week.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/delete_instrument_properties_response.py` & `lusid-sdk-1.0.98/lusid/models/delete_instrument_properties_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/delete_instrument_response.py` & `lusid-sdk-1.0.98/lusid/models/delete_instrument_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/delete_instruments_response.py` & `lusid-sdk-1.0.98/lusid/models/delete_instruments_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/delete_relationship_request.py` & `lusid-sdk-1.0.98/lusid/models/delete_relationship_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/deleted_entity_response.py` & `lusid-sdk-1.0.98/lusid/models/deleted_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/dependency_source_filter.py` & `lusid-sdk-1.0.98/lusid/models/dependency_source_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/discount_factor_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/discount_factor_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/discount_factor_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/discount_factor_curve_data_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/economic_dependency.py` & `lusid-sdk-1.0.98/lusid/models/economic_dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/economic_dependency_with_complex_market_data.py` & `lusid-sdk-1.0.98/lusid/models/economic_dependency_with_complex_market_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/economic_dependency_with_quote.py` & `lusid-sdk-1.0.98/lusid/models/economic_dependency_with_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/empty_model_options.py` & `lusid-sdk-1.0.98/lusid/models/empty_model_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/empty_model_options_all_of.py` & `lusid-sdk-1.0.98/lusid/models/empty_model_options_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/entity_identifier.py` & `lusid-sdk-1.0.98/lusid/models/entity_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity.py` & `lusid-sdk-1.0.98/lusid/models/equity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_all_of.py` & `lusid-sdk-1.0.98/lusid/models/equity_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_all_of_identifiers.py` & `lusid-sdk-1.0.98/lusid/models/equity_all_of_identifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_curve_by_prices_data.py` & `lusid-sdk-1.0.98/lusid/models/equity_curve_by_prices_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_curve_by_prices_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/equity_curve_by_prices_data_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_model_options.py` & `lusid-sdk-1.0.98/lusid/models/equity_model_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_model_options_all_of.py` & `lusid-sdk-1.0.98/lusid/models/equity_model_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_option.py` & `lusid-sdk-1.0.98/lusid/models/equity_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_option_all_of.py` & `lusid-sdk-1.0.98/lusid/models/equity_option_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_swap.py` & `lusid-sdk-1.0.98/lusid/models/equity_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_swap_all_of.py` & `lusid-sdk-1.0.98/lusid/models/equity_swap_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_vol_surface_data.py` & `lusid-sdk-1.0.98/lusid/models/equity_vol_surface_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/equity_vol_surface_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/equity_vol_surface_data_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/error_detail.py` & `lusid-sdk-1.0.98/lusid/models/error_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/event_date_range.py` & `lusid-sdk-1.0.98/lusid/models/event_date_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exchange_traded_option.py` & `lusid-sdk-1.0.98/lusid/models/exchange_traded_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exchange_traded_option_all_of.py` & `lusid-sdk-1.0.98/lusid/models/exchange_traded_option_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exchange_traded_option_contract_details.py` & `lusid-sdk-1.0.98/lusid/models/exchange_traded_option_contract_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/execution.py` & `lusid-sdk-1.0.98/lusid/models/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/execution_request.py` & `lusid-sdk-1.0.98/lusid/models/execution_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/execution_set_request.py` & `lusid-sdk-1.0.98/lusid/models/execution_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exercise_event.py` & `lusid-sdk-1.0.98/lusid/models/exercise_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exercise_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/exercise_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exotic_instrument.py` & `lusid-sdk-1.0.98/lusid/models/exotic_instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/exotic_instrument_all_of.py` & `lusid-sdk-1.0.98/lusid/models/exotic_instrument_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/expanded_group.py` & `lusid-sdk-1.0.98/lusid/models/expanded_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/field_definition.py` & `lusid-sdk-1.0.98/lusid/models/field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/field_schema.py` & `lusid-sdk-1.0.98/lusid/models/field_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/field_value.py` & `lusid-sdk-1.0.98/lusid/models/field_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/file_response.py` & `lusid-sdk-1.0.98/lusid/models/file_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fixed_leg.py` & `lusid-sdk-1.0.98/lusid/models/fixed_leg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fixed_leg_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fixed_leg_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fixed_leg_all_of_overrides.py` & `lusid-sdk-1.0.98/lusid/models/fixed_leg_all_of_overrides.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/floating_leg.py` & `lusid-sdk-1.0.98/lusid/models/floating_leg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/floating_leg_all_of.py` & `lusid-sdk-1.0.98/lusid/models/floating_leg_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/flow_convention_name.py` & `lusid-sdk-1.0.98/lusid/models/flow_convention_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/flow_conventions.py` & `lusid-sdk-1.0.98/lusid/models/flow_conventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/forward_rate_agreement.py` & `lusid-sdk-1.0.98/lusid/models/forward_rate_agreement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/forward_rate_agreement_all_of.py` & `lusid-sdk-1.0.98/lusid/models/forward_rate_agreement_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/funding_leg.py` & `lusid-sdk-1.0.98/lusid/models/funding_leg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/funding_leg_all_of.py` & `lusid-sdk-1.0.98/lusid/models/funding_leg_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/future.py` & `lusid-sdk-1.0.98/lusid/models/future.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/future_all_of.py` & `lusid-sdk-1.0.98/lusid/models/future_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/futures_contract_details.py` & `lusid-sdk-1.0.98/lusid/models/futures_contract_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_curve_by_quote_reference.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_curve_by_quote_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_curve_by_quote_reference_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_curve_by_quote_reference_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_curve_data_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_model_options.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_model_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_model_options_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_model_options_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_pips_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_pips_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_pips_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_pips_curve_data_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_curve_data_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_pips_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_pips_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_forward_tenor_pips_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_forward_tenor_pips_curve_data_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_option.py` & `lusid-sdk-1.0.98/lusid/models/fx_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_option_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_option_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_swap.py` & `lusid-sdk-1.0.98/lusid/models/fx_swap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_swap_all_of.py` & `lusid-sdk-1.0.98/lusid/models/fx_swap_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/fx_vol_surface_data.py` & `lusid-sdk-1.0.98/lusid/models/fx_vol_surface_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_complex_market_data_response.py` & `lusid-sdk-1.0.98/lusid/models/get_complex_market_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_counterparty_agreement_response.py` & `lusid-sdk-1.0.98/lusid/models/get_counterparty_agreement_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_credit_support_annex_response.py` & `lusid-sdk-1.0.98/lusid/models/get_credit_support_annex_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_instruments_response.py` & `lusid-sdk-1.0.98/lusid/models/get_instruments_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_quotes_response.py` & `lusid-sdk-1.0.98/lusid/models/get_quotes_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_recipe_response.py` & `lusid-sdk-1.0.98/lusid/models/get_recipe_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/get_reference_portfolio_constituents_response.py` & `lusid-sdk-1.0.98/lusid/models/get_reference_portfolio_constituents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/holding_adjustment.py` & `lusid-sdk-1.0.98/lusid/models/holding_adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/holding_adjustment_with_date.py` & `lusid-sdk-1.0.98/lusid/models/holding_adjustment_with_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/holding_context.py` & `lusid-sdk-1.0.98/lusid/models/holding_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/holdings_adjustment.py` & `lusid-sdk-1.0.98/lusid/models/holdings_adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/holdings_adjustment_header.py` & `lusid-sdk-1.0.98/lusid/models/holdings_adjustment_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/i_data_record.py` & `lusid-sdk-1.0.98/lusid/models/i_data_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/i_unit_definition_dto.py` & `lusid-sdk-1.0.98/lusid/models/i_unit_definition_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/id_selector_definition.py` & `lusid-sdk-1.0.98/lusid/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/identifier_part_schema.py` & `lusid-sdk-1.0.98/lusid/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/index_convention.py` & `lusid-sdk-1.0.98/lusid/models/index_convention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/index_model_options.py` & `lusid-sdk-1.0.98/lusid/models/index_model_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/index_model_options_all_of.py` & `lusid-sdk-1.0.98/lusid/models/index_model_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/industry_classifier.py` & `lusid-sdk-1.0.98/lusid/models/industry_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/inflation_linked_bond.py` & `lusid-sdk-1.0.98/lusid/models/inflation_linked_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/inflation_linked_bond_all_of.py` & `lusid-sdk-1.0.98/lusid/models/inflation_linked_bond_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/inflation_swap.py` & `lusid-sdk-1.0.98/lusid/models/inflation_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/inflation_swap_all_of.py` & `lusid-sdk-1.0.98/lusid/models/inflation_swap_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/informational_error_event.py` & `lusid-sdk-1.0.98/lusid/models/informational_error_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/informational_error_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/informational_error_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/informational_event.py` & `lusid-sdk-1.0.98/lusid/models/informational_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/informational_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/informational_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/inline_valuation_request.py` & `lusid-sdk-1.0.98/lusid/models/inline_valuation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/inline_valuations_reconciliation_request.py` & `lusid-sdk-1.0.98/lusid/models/inline_valuations_reconciliation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/input_transition.py` & `lusid-sdk-1.0.98/lusid/models/input_transition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument.py` & `lusid-sdk-1.0.98/lusid/models/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_definition.py` & `lusid-sdk-1.0.98/lusid/models/instrument_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_definition_format.py` & `lusid-sdk-1.0.98/lusid/models/instrument_definition_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_event.py` & `lusid-sdk-1.0.98/lusid/models/instrument_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_event_holder.py` & `lusid-sdk-1.0.98/lusid/models/instrument_event_holder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_id_type_descriptor.py` & `lusid-sdk-1.0.98/lusid/models/instrument_id_type_descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_id_value.py` & `lusid-sdk-1.0.98/lusid/models/instrument_id_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_leg.py` & `lusid-sdk-1.0.98/lusid/models/instrument_leg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_leg_all_of.py` & `lusid-sdk-1.0.98/lusid/models/instrument_leg_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_match.py` & `lusid-sdk-1.0.98/lusid/models/instrument_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_models.py` & `lusid-sdk-1.0.98/lusid/models/instrument_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_properties.py` & `lusid-sdk-1.0.98/lusid/models/instrument_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/instrument_search_property.py` & `lusid-sdk-1.0.98/lusid/models/instrument_search_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/interest_rate_swap.py` & `lusid-sdk-1.0.98/lusid/models/interest_rate_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/interest_rate_swap_all_of.py` & `lusid-sdk-1.0.98/lusid/models/interest_rate_swap_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/interest_rate_swaption.py` & `lusid-sdk-1.0.98/lusid/models/interest_rate_swaption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/interest_rate_swaption_all_of.py` & `lusid-sdk-1.0.98/lusid/models/interest_rate_swaption_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/ir_vol_cube_data.py` & `lusid-sdk-1.0.98/lusid/models/ir_vol_cube_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/ir_vol_cube_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/ir_vol_cube_data_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/is_business_day_response.py` & `lusid-sdk-1.0.98/lusid/models/is_business_day_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/label_value_set.py` & `lusid-sdk-1.0.98/lusid/models/label_value_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/leg_definition.py` & `lusid-sdk-1.0.98/lusid/models/leg_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/legal_entity.py` & `lusid-sdk-1.0.98/lusid/models/legal_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/level_step.py` & `lusid-sdk-1.0.98/lusid/models/level_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/life_cycle_event_lineage.py` & `lusid-sdk-1.0.98/lusid/models/life_cycle_event_lineage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/life_cycle_event_value.py` & `lusid-sdk-1.0.98/lusid/models/life_cycle_event_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/life_cycle_event_value_all_of.py` & `lusid-sdk-1.0.98/lusid/models/life_cycle_event_value_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/link.py` & `lusid-sdk-1.0.98/lusid/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/list_aggregation_reconciliation.py` & `lusid-sdk-1.0.98/lusid/models/list_aggregation_reconciliation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/list_aggregation_response.py` & `lusid-sdk-1.0.98/lusid/models/list_aggregation_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/loan_period.py` & `lusid-sdk-1.0.98/lusid/models/loan_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/lusid_instrument.py` & `lusid-sdk-1.0.98/lusid/models/lusid_instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/lusid_problem_details.py` & `lusid-sdk-1.0.98/lusid/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/lusid_unique_id.py` & `lusid-sdk-1.0.98/lusid/models/lusid_unique_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/lusid_validation_problem_details.py` & `lusid-sdk-1.0.98/lusid/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/mapped_string.py` & `lusid-sdk-1.0.98/lusid/models/mapped_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/mapping.py` & `lusid-sdk-1.0.98/lusid/models/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/mapping_rule.py` & `lusid-sdk-1.0.98/lusid/models/mapping_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_context.py` & `lusid-sdk-1.0.98/lusid/models/market_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_context_suppliers.py` & `lusid-sdk-1.0.98/lusid/models/market_context_suppliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_data_key_rule.py` & `lusid-sdk-1.0.98/lusid/models/market_data_key_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_data_options.py` & `lusid-sdk-1.0.98/lusid/models/market_data_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_data_overrides.py` & `lusid-sdk-1.0.98/lusid/models/market_data_overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_data_specific_rule.py` & `lusid-sdk-1.0.98/lusid/models/market_data_specific_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_options.py` & `lusid-sdk-1.0.98/lusid/models/market_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/market_quote.py` & `lusid-sdk-1.0.98/lusid/models/market_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/metric_value.py` & `lusid-sdk-1.0.98/lusid/models/metric_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/model_options.py` & `lusid-sdk-1.0.98/lusid/models/model_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/model_property.py` & `lusid-sdk-1.0.98/lusid/models/model_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/model_selection.py` & `lusid-sdk-1.0.98/lusid/models/model_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/next_value_in_sequence_response.py` & `lusid-sdk-1.0.98/lusid/models/next_value_in_sequence_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/opaque_market_data.py` & `lusid-sdk-1.0.98/lusid/models/opaque_market_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/opaque_market_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/opaque_market_data_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/opaque_model_options.py` & `lusid-sdk-1.0.98/lusid/models/opaque_model_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/opaque_model_options_all_of.py` & `lusid-sdk-1.0.98/lusid/models/opaque_model_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/open_event.py` & `lusid-sdk-1.0.98/lusid/models/open_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/open_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/open_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/operation.py` & `lusid-sdk-1.0.98/lusid/models/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/order.py` & `lusid-sdk-1.0.98/lusid/models/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/order_by_spec.py` & `lusid-sdk-1.0.98/lusid/models/order_by_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/order_request.py` & `lusid-sdk-1.0.98/lusid/models/order_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/order_set_request.py` & `lusid-sdk-1.0.98/lusid/models/order_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/otc_confirmation.py` & `lusid-sdk-1.0.98/lusid/models/otc_confirmation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/output_transaction.py` & `lusid-sdk-1.0.98/lusid/models/output_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/output_transition.py` & `lusid-sdk-1.0.98/lusid/models/output_transition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_allocation.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_block.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_calendar.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_corporate_action_source.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_corporate_action_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_custom_entity_definition.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_custom_entity_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_custom_entity_response.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_custom_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_cut_label_definition.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_cut_label_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_data_type_summary.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_data_type_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_execution.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_instrument.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_instrument_event_holder.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_instrument_event_holder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_legal_entity.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_legal_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_order.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_participation.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_participation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_person.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_person.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_placement.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_placement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_portfolio_group_search_result.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_portfolio_group_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_portfolio_search_result.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_portfolio_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_property_definition_search_result.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_property_definition_search_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_relationship_definition.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_relationship_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/paged_resource_list_of_sequence_definition.py` & `lusid-sdk-1.0.98/lusid/models/paged_resource_list_of_sequence_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/participation.py` & `lusid-sdk-1.0.98/lusid/models/participation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/participation_request.py` & `lusid-sdk-1.0.98/lusid/models/participation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/participation_set_request.py` & `lusid-sdk-1.0.98/lusid/models/participation_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/performance_return.py` & `lusid-sdk-1.0.98/lusid/models/performance_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/performance_returns_metric.py` & `lusid-sdk-1.0.98/lusid/models/performance_returns_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/perpetual_property.py` & `lusid-sdk-1.0.98/lusid/models/perpetual_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/person.py` & `lusid-sdk-1.0.98/lusid/models/person.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/placement.py` & `lusid-sdk-1.0.98/lusid/models/placement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/placement_request.py` & `lusid-sdk-1.0.98/lusid/models/placement_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/placement_set_request.py` & `lusid-sdk-1.0.98/lusid/models/placement_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio.py` & `lusid-sdk-1.0.98/lusid/models/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_cash_flow.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_cash_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_cash_ladder.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_cash_ladder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_details.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_entity_id.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_entity_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_group.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_group_properties.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_group_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_group_search_result.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_group_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_holding.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_properties.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_reconciliation_request.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_reconciliation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_result_data_key_rule.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_result_data_key_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_result_data_key_rule_all_of.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_result_data_key_rule_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolio_search_result.py` & `lusid-sdk-1.0.98/lusid/models/portfolio_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/portfolios_reconciliation_request.py` & `lusid-sdk-1.0.98/lusid/models/portfolios_reconciliation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/premium.py` & `lusid-sdk-1.0.98/lusid/models/premium.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/pricing_context.py` & `lusid-sdk-1.0.98/lusid/models/pricing_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/pricing_options.py` & `lusid-sdk-1.0.98/lusid/models/pricing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/processed_command.py` & `lusid-sdk-1.0.98/lusid/models/processed_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/property_definition.py` & `lusid-sdk-1.0.98/lusid/models/property_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/property_definition_search_result.py` & `lusid-sdk-1.0.98/lusid/models/property_definition_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/property_filter.py` & `lusid-sdk-1.0.98/lusid/models/property_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/property_interval.py` & `lusid-sdk-1.0.98/lusid/models/property_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/property_schema.py` & `lusid-sdk-1.0.98/lusid/models/property_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/property_value.py` & `lusid-sdk-1.0.98/lusid/models/property_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/quote.py` & `lusid-sdk-1.0.98/lusid/models/quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/quote_id.py` & `lusid-sdk-1.0.98/lusid/models/quote_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/quote_series_id.py` & `lusid-sdk-1.0.98/lusid/models/quote_series_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/raw_vendor_event.py` & `lusid-sdk-1.0.98/lusid/models/raw_vendor_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/raw_vendor_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/raw_vendor_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/realised_gain_loss.py` & `lusid-sdk-1.0.98/lusid/models/realised_gain_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconcile_date_time_rule.py` & `lusid-sdk-1.0.98/lusid/models/reconcile_date_time_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconcile_date_time_rule_all_of.py` & `lusid-sdk-1.0.98/lusid/models/reconcile_date_time_rule_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconcile_numeric_rule.py` & `lusid-sdk-1.0.98/lusid/models/reconcile_numeric_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconcile_numeric_rule_all_of.py` & `lusid-sdk-1.0.98/lusid/models/reconcile_numeric_rule_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconcile_string_rule.py` & `lusid-sdk-1.0.98/lusid/models/reconcile_string_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconcile_string_rule_all_of.py` & `lusid-sdk-1.0.98/lusid/models/reconcile_string_rule_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciled_transaction.py` & `lusid-sdk-1.0.98/lusid/models/reconciled_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciliation_break.py` & `lusid-sdk-1.0.98/lusid/models/reconciliation_break.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciliation_left_right_address_key_pair.py` & `lusid-sdk-1.0.98/lusid/models/reconciliation_left_right_address_key_pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciliation_line.py` & `lusid-sdk-1.0.98/lusid/models/reconciliation_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciliation_request.py` & `lusid-sdk-1.0.98/lusid/models/reconciliation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciliation_response.py` & `lusid-sdk-1.0.98/lusid/models/reconciliation_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reconciliation_rule.py` & `lusid-sdk-1.0.98/lusid/models/reconciliation_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reference_data.py` & `lusid-sdk-1.0.98/lusid/models/reference_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reference_instrument.py` & `lusid-sdk-1.0.98/lusid/models/reference_instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reference_instrument_all_of.py` & `lusid-sdk-1.0.98/lusid/models/reference_instrument_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reference_portfolio_constituent.py` & `lusid-sdk-1.0.98/lusid/models/reference_portfolio_constituent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reference_portfolio_constituent_request.py` & `lusid-sdk-1.0.98/lusid/models/reference_portfolio_constituent_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/related_entity.py` & `lusid-sdk-1.0.98/lusid/models/related_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/relation.py` & `lusid-sdk-1.0.98/lusid/models/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/relationship.py` & `lusid-sdk-1.0.98/lusid/models/relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/relationship_definition.py` & `lusid-sdk-1.0.98/lusid/models/relationship_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/repo.py` & `lusid-sdk-1.0.98/lusid/models/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/repo_all_of.py` & `lusid-sdk-1.0.98/lusid/models/repo_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reset_event.py` & `lusid-sdk-1.0.98/lusid/models/reset_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/reset_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/reset_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_id.py` & `lusid-sdk-1.0.98/lusid/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_access_controlled_resource.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_access_metadata_value_of.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_access_metadata_value_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_aggregation_query.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_aggregation_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_allocation.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_block.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_calendar_date.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_calendar_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_change.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_change_history.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_change_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_constituents_adjustment_header.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_constituents_adjustment_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_corporate_action.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_corporate_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_data_type.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_data_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_execution.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_get_counterparty_agreement_response.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_get_counterparty_agreement_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_get_credit_support_annex_response.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_get_credit_support_annex_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_get_recipe_response.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_get_recipe_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_holdings_adjustment_header.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_holdings_adjustment_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_i_unit_definition_dto.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_i_unit_definition_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_instrument_id_type_descriptor.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_instrument_id_type_descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_legal_entity.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_legal_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_mapping.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_order.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_participation.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_participation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_performance_return.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_performance_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_person.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_person.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_placement.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_placement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio_cash_flow.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio_cash_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio_cash_ladder.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio_cash_ladder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_portfolio_group.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_portfolio_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_processed_command.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_processed_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_property.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_property_definition.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_property_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_property_interval.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_property_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_quote.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_reconciliation_break.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_reconciliation_break.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_relation.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_relationship.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_relationship.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_scope_definition.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_scope_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_string.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/resource_list_of_value_type.py` & `lusid-sdk-1.0.98/lusid/models/resource_list_of_value_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/response_meta_data.py` & `lusid-sdk-1.0.98/lusid/models/response_meta_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_data_key_rule.py` & `lusid-sdk-1.0.98/lusid/models/result_data_key_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_data_key_rule_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_data_key_rule_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_data_schema.py` & `lusid-sdk-1.0.98/lusid/models/result_data_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_key_rule.py` & `lusid-sdk-1.0.98/lusid/models/result_key_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value.py` & `lusid-sdk-1.0.98/lusid/models/result_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value0_d.py` & `lusid-sdk-1.0.98/lusid/models/result_value0_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value0_d_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value0_d_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_bool.py` & `lusid-sdk-1.0.98/lusid/models/result_value_bool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_bool_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_bool_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_currency.py` & `lusid-sdk-1.0.98/lusid/models/result_value_currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_currency_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_currency_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_date_time_offset.py` & `lusid-sdk-1.0.98/lusid/models/result_value_date_time_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_date_time_offset_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_date_time_offset_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_decimal.py` & `lusid-sdk-1.0.98/lusid/models/result_value_decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_decimal_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_decimal_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_dictionary.py` & `lusid-sdk-1.0.98/lusid/models/result_value_dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_dictionary_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_dictionary_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_int.py` & `lusid-sdk-1.0.98/lusid/models/result_value_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_int_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_int_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_string.py` & `lusid-sdk-1.0.98/lusid/models/result_value_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/result_value_string_all_of.py` & `lusid-sdk-1.0.98/lusid/models/result_value_string_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/schedule.py` & `lusid-sdk-1.0.98/lusid/models/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/schema.py` & `lusid-sdk-1.0.98/lusid/models/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/scope_definition.py` & `lusid-sdk-1.0.98/lusid/models/scope_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/sequence_definition.py` & `lusid-sdk-1.0.98/lusid/models/sequence_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/set_legal_entity_identifiers_request.py` & `lusid-sdk-1.0.98/lusid/models/set_legal_entity_identifiers_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/set_legal_entity_properties_request.py` & `lusid-sdk-1.0.98/lusid/models/set_legal_entity_properties_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/set_person_identifiers_request.py` & `lusid-sdk-1.0.98/lusid/models/set_person_identifiers_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/set_person_properties_request.py` & `lusid-sdk-1.0.98/lusid/models/set_person_properties_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/side_configuration_data.py` & `lusid-sdk-1.0.98/lusid/models/side_configuration_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/simple_cash_flow_loan.py` & `lusid-sdk-1.0.98/lusid/models/simple_cash_flow_loan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/simple_cash_flow_loan_all_of.py` & `lusid-sdk-1.0.98/lusid/models/simple_cash_flow_loan_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/simple_instrument.py` & `lusid-sdk-1.0.98/lusid/models/simple_instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/simple_instrument_all_of.py` & `lusid-sdk-1.0.98/lusid/models/simple_instrument_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/step_schedule.py` & `lusid-sdk-1.0.98/lusid/models/step_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/step_schedule_all_of.py` & `lusid-sdk-1.0.98/lusid/models/step_schedule_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/stock_split_event.py` & `lusid-sdk-1.0.98/lusid/models/stock_split_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/stock_split_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/stock_split_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/stream.py` & `lusid-sdk-1.0.98/lusid/models/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/supported_analytics_internal_request.py` & `lusid-sdk-1.0.98/lusid/models/supported_analytics_internal_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/target_tax_lot.py` & `lusid-sdk-1.0.98/lusid/models/target_tax_lot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/target_tax_lot_request.py` & `lusid-sdk-1.0.98/lusid/models/target_tax_lot_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/term_deposit.py` & `lusid-sdk-1.0.98/lusid/models/term_deposit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/term_deposit_all_of.py` & `lusid-sdk-1.0.98/lusid/models/term_deposit_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/touch.py` & `lusid-sdk-1.0.98/lusid/models/touch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction.py` & `lusid-sdk-1.0.98/lusid/models/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_configuration_data.py` & `lusid-sdk-1.0.98/lusid/models/transaction_configuration_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_configuration_data_request.py` & `lusid-sdk-1.0.98/lusid/models/transaction_configuration_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_configuration_movement_data.py` & `lusid-sdk-1.0.98/lusid/models/transaction_configuration_movement_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_configuration_movement_data_request.py` & `lusid-sdk-1.0.98/lusid/models/transaction_configuration_movement_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_configuration_type_alias.py` & `lusid-sdk-1.0.98/lusid/models/transaction_configuration_type_alias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_price.py` & `lusid-sdk-1.0.98/lusid/models/transaction_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_property_mapping.py` & `lusid-sdk-1.0.98/lusid/models/transaction_property_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_property_mapping_request.py` & `lusid-sdk-1.0.98/lusid/models/transaction_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_query_parameters.py` & `lusid-sdk-1.0.98/lusid/models/transaction_query_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_reconciliation_request.py` & `lusid-sdk-1.0.98/lusid/models/transaction_reconciliation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_request.py` & `lusid-sdk-1.0.98/lusid/models/transaction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transaction_set_configuration_data.py` & `lusid-sdk-1.0.98/lusid/models/transaction_set_configuration_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transactions_reconciliations_response.py` & `lusid-sdk-1.0.98/lusid/models/transactions_reconciliations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transition_event.py` & `lusid-sdk-1.0.98/lusid/models/transition_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/transition_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/transition_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/trigger_event.py` & `lusid-sdk-1.0.98/lusid/models/trigger_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/trigger_event_all_of.py` & `lusid-sdk-1.0.98/lusid/models/trigger_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/typed_resource_id.py` & `lusid-sdk-1.0.98/lusid/models/typed_resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_calendar_request.py` & `lusid-sdk-1.0.98/lusid/models/update_calendar_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_custom_entity_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/update_custom_entity_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_cut_label_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/update_cut_label_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_data_type_request.py` & `lusid-sdk-1.0.98/lusid/models/update_data_type_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_derived_property_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/update_derived_property_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_instrument_identifier_request.py` & `lusid-sdk-1.0.98/lusid/models/update_instrument_identifier_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_portfolio_group_request.py` & `lusid-sdk-1.0.98/lusid/models/update_portfolio_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_portfolio_request.py` & `lusid-sdk-1.0.98/lusid/models/update_portfolio_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_property_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/update_property_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_relationship_definition_request.py` & `lusid-sdk-1.0.98/lusid/models/update_relationship_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/update_unit_request.py` & `lusid-sdk-1.0.98/lusid/models/update_unit_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_complex_market_data_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_complex_market_data_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_corporate_action_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_corporate_action_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_corporate_actions_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_corporate_actions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_counterparty_agreement_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_counterparty_agreement_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_credit_support_annex_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_credit_support_annex_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_custom_entities_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_custom_entities_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_custom_entity_access_metadata_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_custom_entity_access_metadata_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_instrument_event_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_instrument_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_instrument_events_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_instrument_events_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_instrument_properties_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_instrument_properties_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_instrument_property_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_instrument_property_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_instruments_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_instruments_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_legal_entities_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_legal_entities_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_legal_entity_access_metadata_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_legal_entity_access_metadata_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_legal_entity_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_legal_entity_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_person_access_metadata_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_person_access_metadata_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_person_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_person_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_portfolio_access_metadata_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_portfolio_access_metadata_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_portfolio_group_access_metadata_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_portfolio_group_access_metadata_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_portfolio_transactions_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_portfolio_transactions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_quote_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_quote_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_quotes_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_quotes_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_recipe_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_recipe_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_reference_portfolio_constituents_request.py` & `lusid-sdk-1.0.98/lusid/models/upsert_reference_portfolio_constituents_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_reference_portfolio_constituents_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_reference_portfolio_constituents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_returns_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_returns_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_single_structured_data_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_single_structured_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_structured_data_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_structured_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/upsert_transaction_properties_response.py` & `lusid-sdk-1.0.98/lusid/models/upsert_transaction_properties_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/user.py` & `lusid-sdk-1.0.98/lusid/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/valuation_request.py` & `lusid-sdk-1.0.98/lusid/models/valuation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/valuation_schedule.py` & `lusid-sdk-1.0.98/lusid/models/valuation_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/valuations_reconciliation_request.py` & `lusid-sdk-1.0.98/lusid/models/valuations_reconciliation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/value_type.py` & `lusid-sdk-1.0.98/lusid/models/value_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/vendor_model_rule.py` & `lusid-sdk-1.0.98/lusid/models/vendor_model_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/version.py` & `lusid-sdk-1.0.98/lusid/models/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/version_summary_dto.py` & `lusid-sdk-1.0.98/lusid/models/version_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_a2_b_data_record.py` & `lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_a2_b_data_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_a2_b_movement_record.py` & `lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_a2_b_movement_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_output_transaction.py` & `lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_output_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_portfolio_holding.py` & `lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_portfolio_holding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/versioned_resource_list_of_transaction.py` & `lusid-sdk-1.0.98/lusid/models/versioned_resource_list_of_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/weekend_mask.py` & `lusid-sdk-1.0.98/lusid/models/weekend_mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/weighted_instrument.py` & `lusid-sdk-1.0.98/lusid/models/weighted_instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/weighted_instruments.py` & `lusid-sdk-1.0.98/lusid/models/weighted_instruments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/yield_curve_data.py` & `lusid-sdk-1.0.98/lusid/models/yield_curve_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/models/yield_curve_data_all_of.py` & `lusid-sdk-1.0.98/lusid/models/yield_curve_data_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-sdk-1.0.91/lusid/rest.py` & `lusid-sdk-1.0.98/lusid/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     LUSID API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.91
+    The version of the OpenAPI document: 1.0.98
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-sdk-1.0.91/lusid/tcp/tcp_keep_alive_probes.py` & `lusid-sdk-1.0.98/lusid/tcp/tcp_keep_alive_probes.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/api_client_builder.py` & `lusid-sdk-1.0.98/lusid/utilities/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/api_client_factory.py` & `lusid-sdk-1.0.98/lusid/utilities/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/api_configuration.py` & `lusid-sdk-1.0.98/lusid/utilities/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/api_configuration_loader.py` & `lusid-sdk-1.0.98/lusid/utilities/api_configuration_loader.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/config_keys.json` & `lusid-sdk-1.0.98/lusid/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/lusid_retry.py` & `lusid-sdk-1.0.98/lusid/utilities/lusid_retry.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/proxy_config.py` & `lusid-sdk-1.0.98/lusid/utilities/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid/utilities/refreshing_token.py` & `lusid-sdk-1.0.98/lusid/utilities/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/lusid_sdk.egg-info/SOURCES.txt` & `lusid-sdk-1.0.98/lusid_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-sdk-1.0.91/setup.py` & `lusid-sdk-1.0.98/setup.py`

 * *Files identical despite different names*

