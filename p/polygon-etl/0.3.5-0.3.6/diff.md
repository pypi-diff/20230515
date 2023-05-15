# Comparing `tmp/polygon-etl-0.3.5.tar.gz` & `tmp/polygon-etl-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon-etl-0.3.5.tar", last modified: Tue Mar 21 15:09:57 2023, max compression
+gzip compressed data, was "polygon-etl-0.3.6.tar", last modified: Mon May 15 10:01:58 2023, max compression
```

## Comparing `polygon-etl-0.3.5.tar` & `polygon-etl-0.3.6.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.860367 polygon-etl-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-21 15:09:57.860367 polygon-etl-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.824367 polygon-etl-0.3.5/polygon_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-21 15:09:57.000000 polygon-etl-0.3.5/polygon_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-21 15:09:57.000000 polygon-etl-0.3.5/polygon_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:09:57.000000 polygon-etl-0.3.5/polygon_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-21 15:09:57.000000 polygon-etl-0.3.5/polygon_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-21 15:09:57.000000 polygon-etl-0.3.5/polygon_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-21 15:09:57.000000 polygon-etl-0.3.5/polygon_etl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.828367 polygon-etl-0.3.5/polygonetl/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/atomic_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.832367 polygon-etl-0.3.5/polygonetl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_blocks_and_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_receipts_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/export_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/extract_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/extract_csv_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/extract_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/extract_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/extract_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/extract_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/filter_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/get_block_range_for_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/get_block_range_for_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/get_keccak_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/cli/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/csv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.836367 polygon-etl-0.3.5/polygonetl/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/geth_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/receipt_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/token_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/domain/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.836367 polygon-etl-0.3.5/polygonetl/enumeration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/enumeration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/enumeration/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/erc20_abi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.840367 polygon-etl-0.3.5/polygonetl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/executors/batch_work_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/executors/bounded_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/executors/fail_safe_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.844367 polygon-etl-0.3.5/polygonetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_all_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/export_traces_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.844367 polygon-etl-0.3.5/polygonetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/contracts_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/geth_traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/token_transfers_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/tokens_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/exporters/traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/jobs/extract_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/json_rpc_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mainnet_daofork_state_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mainnet_genesis_alloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.848367 polygon-etl-0.3.5/polygonetl/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/block_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/contract_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/geth_trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/receipt_log_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/receipt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/token_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/token_transfer_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/mappers/transaction_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.848367 polygon-etl-0.3.5/polygonetl/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/misc/retriable_value_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.852367 polygon-etl-0.3.5/polygonetl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/providers/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/providers/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/providers/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/providers/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.852367 polygon-etl-0.3.5/polygonetl/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/eth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/eth_special_trace_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/eth_token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/graph_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/trace_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/service/trace_status_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.856367 polygon-etl-0.3.5/polygonetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/eth_item_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/eth_item_timestamp_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/eth_streamer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/item_exporter_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/streaming/postgres_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/thread_local_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/polygonetl/web3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:09:57.860367 polygon-etl-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.824367 polygon-etl-0.3.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.856367 polygon-etl-0.3.5/tests/polygonetl/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.860367 polygon-etl-0.3.5/tests/polygonetl/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/mock_batch_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/mock_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_export_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/polygonetl/job/test_extract_tokens_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:09:57.860367 polygon-etl-0.3.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-21 15:09:48.000000 polygon-etl-0.3.5/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.494116 polygon-etl-0.3.6/polygon_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/atomic_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_blocks_and_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_receipts_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/filter_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/get_keccak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/csv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/geth_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/receipt_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/token_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/enumeration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/enumeration/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/erc20_abi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/batch_work_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/bounded_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/fail_safe_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_all_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_traces_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/contracts_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/geth_traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/token_transfers_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/tokens_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/json_rpc_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mainnet_daofork_state_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mainnet_genesis_alloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/block_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/contract_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/geth_trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/receipt_log_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/receipt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/token_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/token_transfer_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/transaction_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/misc/retriable_value_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/polygonetl/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_special_trace_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/trace_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/trace_status_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/polygonetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/eth_item_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/eth_item_timestamp_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/eth_streamer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/item_exporter_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/postgres_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/thread_local_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/web3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.494116 polygon-etl-0.3.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/tests/polygonetl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/tests/polygonetl/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/mock_batch_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/mock_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_tokens_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/resources/__init__.py
```

### Comparing `polygon-etl-0.3.5/PKG-INFO` & `polygon-etl-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-etl
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tools for exporting Polygon blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/polygon-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/polygon-etl/issues
 Project-URL: Source, https://github.com/blockchain-etl/polygon-etl
```

### Comparing `polygon-etl-0.3.5/README.md` & `polygon-etl-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygon_etl.egg-info/PKG-INFO` & `polygon-etl-0.3.6/polygon_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-etl
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tools for exporting Polygon blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/polygon-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/polygon-etl/issues
 Project-URL: Source, https://github.com/blockchain-etl/polygon-etl
```

### Comparing `polygon-etl-0.3.5/polygon_etl.egg-info/SOURCES.txt` & `polygon-etl-0.3.6/polygon_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/__init__.py` & `polygon-etl-0.3.6/polygonetl/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/__main__.py` & `polygon-etl-0.3.6/polygonetl/__main__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/atomic_counter.py` & `polygon-etl-0.3.6/polygonetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/__init__.py` & `polygon-etl-0.3.6/polygonetl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_all.py` & `polygon-etl-0.3.6/polygonetl/cli/export_all.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_blocks_and_transactions.py` & `polygon-etl-0.3.6/polygonetl/cli/export_blocks_and_transactions.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_contracts.py` & `polygon-etl-0.3.6/polygonetl/cli/export_contracts.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_geth_traces.py` & `polygon-etl-0.3.6/polygonetl/cli/export_geth_traces.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_receipts_and_logs.py` & `polygon-etl-0.3.6/polygonetl/cli/export_receipts_and_logs.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_token_transfers.py` & `polygon-etl-0.3.6/polygonetl/cli/export_token_transfers.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_tokens.py` & `polygon-etl-0.3.6/polygonetl/cli/export_tokens.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/export_traces.py` & `polygon-etl-0.3.6/polygonetl/cli/export_traces.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/extract_contracts.py` & `polygon-etl-0.3.6/polygonetl/cli/extract_contracts.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/extract_csv_column.py` & `polygon-etl-0.3.6/polygonetl/cli/extract_csv_column.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/extract_field.py` & `polygon-etl-0.3.6/polygonetl/cli/extract_field.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/extract_geth_traces.py` & `polygon-etl-0.3.6/polygonetl/cli/extract_geth_traces.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/extract_token_transfers.py` & `polygon-etl-0.3.6/polygonetl/cli/extract_token_transfers.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/extract_tokens.py` & `polygon-etl-0.3.6/polygonetl/cli/extract_tokens.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/filter_items.py` & `polygon-etl-0.3.6/polygonetl/cli/filter_items.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/get_block_range_for_date.py` & `polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_date.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/get_block_range_for_timestamps.py` & `polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_timestamps.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/get_keccak_hash.py` & `polygon-etl-0.3.6/polygonetl/cli/get_keccak_hash.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/cli/stream.py` & `polygon-etl-0.3.6/polygonetl/cli/stream.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/csv_utils.py` & `polygon-etl-0.3.6/polygonetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/__init__.py` & `polygon-etl-0.3.6/polygonetl/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/block.py` & `polygon-etl-0.3.6/polygonetl/domain/block.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/contract.py` & `polygon-etl-0.3.6/polygonetl/domain/contract.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/geth_trace.py` & `polygon-etl-0.3.6/polygonetl/domain/geth_trace.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/receipt.py` & `polygon-etl-0.3.6/polygonetl/domain/receipt.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/receipt_log.py` & `polygon-etl-0.3.6/polygonetl/domain/receipt_log.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/token.py` & `polygon-etl-0.3.6/polygonetl/domain/token.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/token_transfer.py` & `polygon-etl-0.3.6/polygonetl/domain/token_transfer.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/trace.py` & `polygon-etl-0.3.6/polygonetl/domain/trace.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/domain/transaction.py` & `polygon-etl-0.3.6/polygonetl/domain/transaction.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/erc20_abi.py` & `polygon-etl-0.3.6/polygonetl/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/executors/__init__.py` & `polygon-etl-0.3.6/polygonetl/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/executors/batch_work_executor.py` & `polygon-etl-0.3.6/polygonetl/executors/batch_work_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 import logging
 import time
 from json.decoder import JSONDecodeError
 
 from requests.exceptions import Timeout as RequestsTimeout, HTTPError, TooManyRedirects, ConnectionError as RequestsConnectionError
-from web3.utils.threads import Timeout as Web3Timeout
+from web3._utils.threads import Timeout as Web3Timeout
 
 from polygonetl.executors.bounded_executor import BoundedExecutor
 from polygonetl.executors.fail_safe_executor import FailSafeExecutor
 from polygonetl.misc.retriable_value_error import RetriableValueError
 from polygonetl.progress_logger import ProgressLogger
 from polygonetl.utils import dynamic_batch_iterator
```

### Comparing `polygon-etl-0.3.5/polygonetl/executors/bounded_executor.py` & `polygon-etl-0.3.6/polygonetl/executors/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/executors/fail_safe_executor.py` & `polygon-etl-0.3.6/polygonetl/executors/fail_safe_executor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/exporters.py` & `polygon-etl-0.3.6/polygonetl/exporters.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/__init__.py` & `polygon-etl-0.3.6/polygonetl/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_all_common.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_all_common.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_blocks_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_contracts_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_geth_traces_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_receipts_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_token_transfers_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_token_transfers_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,12 +78,12 @@
         events = event_filter.get_all_entries()
         for event in events:
             log = self.receipt_log_mapper.web3_dict_to_receipt_log(event)
             token_transfer = self.token_transfer_extractor.extract_transfer_from_log(log)
             if token_transfer is not None:
                 self.item_exporter.export_item(self.token_transfer_mapper.token_transfer_to_dict(token_transfer))
 
-        self.web3.eth.uninstallFilter(event_filter.filter_id)
+        self.web3.eth.uninstall_filter(event_filter.filter_id)
 
     def _end(self):
         self.batch_work_executor.shutdown()
         self.item_exporter.close()
```

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_tokens_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/export_traces_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/export_traces_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         if self.include_daofork_traces and DAOFORK_BLOCK_NUMBER in block_number_batch:
             daofork_traces = self.special_trace_service.get_daofork_traces()
             all_traces.extend(daofork_traces)
 
         # TODO: Change to traceFilter when this issue is fixed
         # https://github.com/paritytech/parity-ethereum/issues/9822
-        json_traces = self.web3.parity.traceBlock(block_number)
+        json_traces = self.web3.parity.trace_block(block_number)
 
         if json_traces is None:
             raise ValueError(
                 "Response from the node is None. Is the node fully synced?"
             )
 
         traces = [
```

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/__init__.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/contracts_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/contracts_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/geth_traces_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/geth_traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/token_transfers_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/token_transfers_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/tokens_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/tokens_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/exporters/traces_item_exporter.py` & `polygon-etl-0.3.6/polygonetl/jobs/exporters/traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/extract_contracts_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/extract_geth_traces_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/extract_token_transfers_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/jobs/extract_tokens_job.py` & `polygon-etl-0.3.6/polygonetl/jobs/extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/json_rpc_requests.py` & `polygon-etl-0.3.6/polygonetl/json_rpc_requests.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mainnet_daofork_state_changes.py` & `polygon-etl-0.3.6/polygonetl/mainnet_daofork_state_changes.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mainnet_genesis_alloc.py` & `polygon-etl-0.3.6/polygonetl/mainnet_genesis_alloc.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/__init__.py` & `polygon-etl-0.3.6/polygonetl/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/block_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/block_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/contract_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/contract_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/geth_trace_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/geth_trace_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/receipt_log_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/receipt_log_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/receipt_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/receipt_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/token_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/token_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/token_transfer_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/token_transfer_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/trace_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/trace_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/mappers/transaction_mapper.py` & `polygon-etl-0.3.6/polygonetl/mappers/transaction_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/misc/__init__.py` & `polygon-etl-0.3.6/polygonetl/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/misc_utils.py` & `polygon-etl-0.3.6/polygonetl/misc_utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/progress_logger.py` & `polygon-etl-0.3.6/polygonetl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/providers/__init__.py` & `polygon-etl-0.3.6/polygonetl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/providers/auto.py` & `polygon-etl-0.3.6/polygonetl/providers/auto.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/providers/ipc.py` & `polygon-etl-0.3.6/polygonetl/providers/ipc.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 import json
 import socket
 
+from web3._utils.threads import Timeout
 from web3.providers.ipc import IPCProvider
-from web3.utils.threads import (
-    Timeout,
-)
 
 try:
     from json import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
```

### Comparing `polygon-etl-0.3.5/polygonetl/providers/request.py` & `polygon-etl-0.3.6/polygonetl/providers/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import logging
 
 import lru
 import requests
 from requests.adapters import HTTPAdapter
-
-from web3.utils.caching import (
-    generate_cache_key,
-)
+from web3._utils.caching import generate_cache_key
 
 
 def _remove_session(key, session):
     session.close()
 
 
 _session_cache = lru.LRU(8, callback=_remove_session)
```

### Comparing `polygon-etl-0.3.5/polygonetl/providers/rpc.py` & `polygon-etl-0.3.6/polygonetl/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/__init__.py` & `polygon-etl-0.3.6/polygonetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/eth_contract_service.py` & `polygon-etl-0.3.6/polygonetl/service/eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/eth_service.py` & `polygon-etl-0.3.6/polygonetl/service/eth_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 
 
 from datetime import datetime, timezone
 
 from polygonetl.service.graph_operations import GraphOperations, OutOfBoundsError, Point
 from web3.middleware import geth_poa_middleware
 
+
 class EthService(object):
     def __init__(self, web3):
-        web3.middleware_stack.inject(geth_poa_middleware, layer=0)
+        web3.middleware_onion.inject(geth_poa_middleware, layer=0)
         graph = BlockTimestampGraph(web3)
         self._graph_operations = GraphOperations(graph)
 
     def get_block_range_for_date(self, date):
         start_datetime = datetime.combine(date, datetime.min.time().replace(tzinfo=timezone.utc))
         end_datetime = datetime.combine(date, datetime.max.time().replace(tzinfo=timezone.utc))
         return self.get_block_range_for_timestamps(start_datetime.timestamp(), end_datetime.timestamp())
@@ -68,15 +69,15 @@
 
 class BlockTimestampGraph(object):
     def __init__(self, web3):
         self._web3 = web3
 
     def get_first_point(self):
         # Ignore the genesis block as its timestamp is 0
-        return block_to_point(self._web3.eth.getBlock(1))
+        return block_to_point(self._web3.eth.get_block(1))
 
     def get_last_point(self):
         return block_to_point(self._web3.eth.getBlock('latest'))
 
     def get_point(self, x):
         return block_to_point(self._web3.eth.getBlock(x))
```

### Comparing `polygon-etl-0.3.5/polygonetl/service/eth_special_trace_service.py` & `polygon-etl-0.3.6/polygonetl/service/eth_special_trace_service.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/eth_token_service.py` & `polygon-etl-0.3.6/polygonetl/service/eth_token_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import logging
 
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import BadFunctionCallOutput, ContractLogicError
 
 from polygonetl.domain.token import EthToken
 from polygonetl.erc20_abi import ERC20_ABI
 
 logger = logging.getLogger('eth_token_service')
 
 
@@ -61,15 +61,15 @@
 
     def _call_contract_function(self, func):
         # BadFunctionCallOutput exception happens if the token doesn't implement a particular function
         # or was self-destructed
         # OverflowError exception happens if the return type of the function doesn't match the expected type
         result = call_contract_function(
             func=func,
-            ignore_errors=(BadFunctionCallOutput, OverflowError, ValueError),
+            ignore_errors=(BadFunctionCallOutput, ContractLogicError, OverflowError, ValueError),
             default_value=None)
 
         if self._function_call_result_transformer is not None:
             return self._function_call_result_transformer(result)
         else:
             return result
```

### Comparing `polygon-etl-0.3.5/polygonetl/service/graph_operations.py` & `polygon-etl-0.3.6/polygonetl/service/graph_operations.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/token_transfer_extractor.py` & `polygon-etl-0.3.6/polygonetl/service/token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/trace_id_calculator.py` & `polygon-etl-0.3.6/polygonetl/service/trace_id_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/service/trace_status_calculator.py` & `polygon-etl-0.3.6/polygonetl/service/trace_status_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/__init__.py` & `polygon-etl-0.3.6/polygonetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/enrich.py` & `polygon-etl-0.3.6/polygonetl/streaming/enrich.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/eth_item_id_calculator.py` & `polygon-etl-0.3.6/polygonetl/streaming/eth_item_id_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/eth_item_timestamp_calculator.py` & `polygon-etl-0.3.6/polygonetl/streaming/eth_item_timestamp_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/eth_streamer_adapter.py` & `polygon-etl-0.3.6/polygonetl/streaming/eth_streamer_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,21 @@
         self.item_exporter = item_exporter
         self.batch_size = batch_size
         self.max_workers = max_workers
         self.entity_types = entity_types
         self.item_id_calculator = EthItemIdCalculator()
         self.item_timestamp_calculator = EthItemTimestampCalculator()
         self.web3 = Web3(self.batch_web3_provider)
-        self.web3.middleware_stack.inject(geth_poa_middleware, layer=0)
+        self.web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
     def open(self):
         self.item_exporter.open()
 
     def get_current_block_number(self):
-        return int(self.web3.eth.getBlock("latest").number)
+        return int(self.web3.eth.get_block("latest").number)
 
     def export_all(self, start_block, end_block):
         # Export blocks and transactions
         blocks, transactions = [], []
         if self._should_export(EntityType.BLOCK) or self._should_export(EntityType.TRANSACTION):
             blocks, transactions = self._export_blocks_and_transactions(start_block, end_block)
```

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/item_exporter_creator.py` & `polygon-etl-0.3.6/polygonetl/streaming/item_exporter_creator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/streaming/postgres_tables.py` & `polygon-etl-0.3.6/polygonetl/streaming/postgres_tables.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/thread_local_proxy.py` & `polygon-etl-0.3.6/polygonetl/thread_local_proxy.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/utils.py` & `polygon-etl-0.3.6/polygonetl/utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/polygonetl/web3_utils.py` & `polygon-etl-0.3.6/polygonetl/web3_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 
 
 def build_web3(provider):
     w3 = Web3(provider)
-    w3.middleware_stack.inject(geth_poa_middleware, layer=0)
+    w3.middleware_onion.inject(geth_poa_middleware, layer=0)
     return w3
```

### Comparing `polygon-etl-0.3.5/setup.py` & `polygon-etl-0.3.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 long_description = read("README.md") if os.path.isfile("README.md") else ""
 
 setup(
     name="polygon-etl",
-    version="0.3.5",
+    version="0.3.6",
     author="Evgeny Medvedev",
     author_email="evge.medvedev@gmail.com",
     description="Tools for exporting Polygon blockchain data to CSV or JSON",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blockchain-etl/polygon-etl",
     packages=find_packages(exclude=["schemas", "tests"]),
@@ -25,37 +25,33 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     keywords="polygon",
-    # web3.py doesn't work on 3.5.2 and less (https://github.com/ethereum/web3.py/issues/1012)
-    # google-cloud-pubsub==2.1.0 requires >=3.6 (https://pypi.org/project/google-cloud-pubsub/2.1.0/)
-    # collections.Mapping unsupported in 3.10 (https://bugs.python.org/issue44737)
     python_requires=">=3.7,<3.10",
     install_requires=[
         "base58==2.1.1",
         "blockchain-etl-common==1.6.1",
-        "click>=7.0",
-        "eth-abi==1.3.0",
-        "eth-utils==1.8.4",
-        "ethereum-dasm==0.1.4",
+        "click>=8.0,<9",
+        "eth-abi==2.2.0",  # web3 5.28.0 depends on eth-abi<3.0.0
+        "eth-utils==1.10",  # eth-abi 2.2.0 depends on eth-utils<2.0.0
+        "ethereum-dasm==0.1.5",
         "requests>=2.23",
-        "web3==4.7.2",
+        "six==1.16.0",  # REVIEW: Missing dependency for blockchain-etl-common
+        "web3>=5.29,<6",
     ],
     extras_require={
         "streaming": [
-            "google-cloud-pubsub==2.1.0",
-            "pytz",  # See https://github.com/googleapis/python-pubsub/issues/468
-            "google-cloud-storage==1.33.0",
-            "pg8000==1.13.2",
-            "pytz==2022.1",
-            "sqlalchemy==1.3.13",
-            "timeout-decorator==0.4.1",
+            "google-cloud-pubsub==2.13.5",
+            "google-cloud-storage==2.7.0",
+            "pg8000>=1.16.6",  # SQLAlchemy 1.4.46 requires pg8000>=1.16.6
+            "SQLAlchemy==1.4.46",
+            "timeout-decorator==0.5.0",
         ],
     },
     entry_points={
         "console_scripts": [
             "polygonetl=polygonetl.cli:cli",
         ],
     },
```

### Comparing `polygon-etl-0.3.5/tests/polygonetl/__init__.py` & `polygon-etl-0.3.6/tests/polygonetl/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/__init__.py` & `polygon-etl-0.3.6/tests/polygonetl/job/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/helpers.py` & `polygon-etl-0.3.6/tests/polygonetl/job/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/mock_batch_web3_provider.py` & `polygon-etl-0.3.6/tests/polygonetl/job/mock_batch_web3_provider.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/mock_web3_provider.py` & `polygon-etl-0.3.6/tests/polygonetl/job/mock_web3_provider.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_blocks_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_contracts_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_geth_traces_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_receipts_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_token_transfers_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_tokens_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_export_traces_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_export_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_extract_contracts_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_extract_geth_traces_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_extract_token_transfers_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/polygonetl/job/test_extract_tokens_job.py` & `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.5/tests/resources/__init__.py` & `polygon-etl-0.3.6/tests/resources/__init__.py`

 * *Files identical despite different names*

