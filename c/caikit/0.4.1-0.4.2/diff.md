# Comparing `tmp/caikit-0.4.1.tar.gz` & `tmp/caikit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.4.1.tar", last modified: Fri May 12 19:24:23 2023, max compression
+gzip compressed data, was "caikit-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.4.1.tar` & `caikit-0.4.2.tar`

### file list

```diff
@@ -1,312 +1,312 @@
--rw-r--r--   0        0        0       60 2023-05-12 19:24:15.177272 caikit-0.4.1/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-12 19:24:15.177272 caikit-0.4.1/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-05-12 19:24:15.177272 caikit-0.4.1/.gitignore
--rw-r--r--   0        0        0      324 2023-05-12 19:24:15.177272 caikit-0.4.1/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-12 19:24:15.177272 caikit-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-12 19:24:15.177272 caikit-0.4.1/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-12 19:24:15.177272 caikit-0.4.1/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-12 19:24:15.177272 caikit-0.4.1/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-12 19:24:15.177272 caikit-0.4.1/.whitesource
--rw-r--r--   0        0        0      336 2023-05-12 19:24:15.177272 caikit-0.4.1/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-12 19:24:15.177272 caikit-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-12 19:24:15.177272 caikit-0.4.1/LICENSE
--rw-r--r--   0        0        0     3626 2023-05-12 19:24:15.177272 caikit-0.4.1/README.md
--rw-r--r--   0        0        0      152 2023-05-12 19:24:15.177272 caikit-0.4.1/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit-overview.png
--rw-r--r--   0        0        0      419 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/config/__init__.py
--rw-r--r--   0        0        0     5392 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/config/config.py
--rw-r--r--   0        0        0     6488 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/config/config.yml
--rw-r--r--   0        0        0     1819 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1586 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1026 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    28672 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    12390 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4736 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40248 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21916 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/model_manager.py
--rw-r--r--   0        0        0    41505 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/module.py
--rw-r--r--   0        0        0     7074 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4716 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2769 2023-05-12 19:24:15.177272 caikit-0.4.1/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5715 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/module_meta.py
--rw-r--r--   0        0        0    14929 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/module_type.py
--rw-r--r--   0        0        0      709 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/resources/base.py
--rw-r--r--   0        0        0     5391 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9332 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16693 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5845 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13249 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12814 2023-05-12 19:24:15.181272 caikit-0.4.1/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0      666 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10744 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4794 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8232 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9473 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15316 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6797 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17900 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-12 19:24:15.185273 caikit-0.4.1/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-12 19:24:15.185273 caikit-0.4.1/code-of-conduct.md
--rw-r--r--   0        0        0     1610 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-12 19:24:15.185273 caikit-0.4.1/docs/architecture_club/README.md
--rw-r--r--   0        0        0      837 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1425 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      671 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      643 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3061 2023-05-12 19:24:15.185273 caikit-0.4.1/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
--rw-r--r--   0        0        0     1157 2023-05-12 19:24:18.557494 caikit-0.4.1/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-05-12 19:24:15.185273 caikit-0.4.1/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-12 19:24:15.185273 caikit-0.4.1/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     3572 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/config/__init__.py
--rw-r--r--   0        0        0     4345 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/config/test_configs.py
--rw-r--r--   0        0        0     9076 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    11661 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26454 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13147 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    19891 2023-05-12 19:24:15.185273 caikit-0.4.1/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     1104 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4291 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0      521 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_imports.py
--rw-r--r--   0        0        0    22165 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    13348 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_module.py
--rw-r--r--   0        0        0     7667 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8080 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     3773 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_module_type.py
--rw-r--r--   0        0        0     1038 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     2456 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    14659 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5542 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      337 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1875 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      646 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2456 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1306 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2713 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      410 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.189273 caikit-0.4.1/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14146 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10454 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17866 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8668 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3768 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1372 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7848 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15426 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30064 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11070 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26122 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-12 19:24:15.193273 caikit-0.4.1/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1115 2023-05-12 19:24:15.193273 caikit-0.4.1/tox.ini
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-15 18:00:15.868723 caikit-0.4.2/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-05-15 18:00:15.868723 caikit-0.4.2/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-15 18:00:15.868723 caikit-0.4.2/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-15 18:00:15.868723 caikit-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-15 18:00:15.868723 caikit-0.4.2/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-15 18:00:15.868723 caikit-0.4.2/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-15 18:00:15.868723 caikit-0.4.2/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-15 18:00:15.868723 caikit-0.4.2/.whitesource
+-rw-r--r--   0        0        0      336 2023-05-15 18:00:15.868723 caikit-0.4.2/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-15 18:00:15.868723 caikit-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-15 18:00:15.868723 caikit-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3626 2023-05-15 18:00:15.868723 caikit-0.4.2/README.md
+-rw-r--r--   0        0        0      152 2023-05-15 18:00:15.868723 caikit-0.4.2/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit-overview.png
+-rw-r--r--   0        0        0      419 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/config/__init__.py
+-rw-r--r--   0        0        0     5392 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/config/config.py
+-rw-r--r--   0        0        0     6488 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/config/config.yml
+-rw-r--r--   0        0        0     1819 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1026 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    28986 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    12390 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4736 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40248 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21916 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    41505 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module.py
+-rw-r--r--   0        0        0     7074 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4716 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2769 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5715 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_meta.py
+-rw-r--r--   0        0        0    14929 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_type.py
+-rw-r--r--   0        0        0      709 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     5391 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9332 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    16693 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5845 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13249 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    12814 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0      666 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10744 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4794 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8232 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9473 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15316 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6797 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17900 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-15 18:00:15.880723 caikit-0.4.2/code-of-conduct.md
+-rw-r--r--   0        0        0     1610 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      837 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1425 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      671 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      643 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3061 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
+-rw-r--r--   0        0        0     1157 2023-05-15 18:00:22.136702 caikit-0.4.2/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-05-15 18:00:15.880723 caikit-0.4.2/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-15 18:00:15.880723 caikit-0.4.2/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     3572 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/config/__init__.py
+-rw-r--r--   0        0        0     4345 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/config/test_configs.py
+-rw-r--r--   0        0        0     9076 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    11661 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26454 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13147 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    19621 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     1104 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4291 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0      521 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_imports.py
+-rw-r--r--   0        0        0    22165 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    13348 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_module.py
+-rw-r--r--   0        0        0     7667 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8080 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     3773 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_module_type.py
+-rw-r--r--   0        0        0     1038 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     2456 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    14659 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5542 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      337 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1875 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      646 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2456 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1306 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2713 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      410 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14146 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10454 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17866 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8668 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3768 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1372 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7848 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15426 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30064 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    11070 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26122 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1115 2023-05-15 18:00:15.888723 caikit-0.4.2/tox.ini
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.2/PKG-INFO
```

### Comparing `caikit-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.4.2/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/.github/workflows/build-library.yml` & `caikit-0.4.2/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/.github/workflows/lint-code.yml` & `caikit-0.4.2/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/.github/workflows/publish-library.yml` & `caikit-0.4.2/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/.pylintrc` & `caikit-0.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/CONTRIBUTING.md` & `caikit-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/LICENSE` & `caikit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/README.md` & `caikit-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit-overview.png` & `caikit-0.4.2/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/config/__init__.py` & `caikit-0.4.2/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/config/config.py` & `caikit-0.4.2/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/config/config.yml` & `caikit-0.4.2/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/__init__.py` & `caikit-0.4.2/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/__init__.py` & `caikit-0.4.2/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/base.py` & `caikit-0.4.2/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.4.2/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.4.2/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/schemes/base.py` & `caikit-0.4.2/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.4.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.4.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/blocks/__init__.py` & `caikit-0.4.2/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/blocks/base.py` & `caikit-0.4.2/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/__init__.py` & `caikit-0.4.2/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/base.py` & `caikit-0.4.2/caikit/core/data_model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,17 @@
         initialization
         """
 
         # use the fully qualified protobuf name to avoid conflicts with
         # nested messages that have matching names
         cls.full_name = cls._proto_class.DESCRIPTOR.full_name
 
-        # all fields
+        # preserve old fields for _make_property_getter later
+        old_fields = cls.fields
+        # overwrite to only have proto-specific fields present
         cls.fields = tuple(cls._proto_class.DESCRIPTOR.fields_by_name)
 
         # map from all enum fields to their enum classes
         # note: enums are also primitives, these overlap
         cls.fields_enum_map = {
             field.name: getattr(enums, field.enum_type.name)
             for field in cls._proto_class.DESCRIPTOR.fields
@@ -231,15 +233,18 @@
 
         # Update the global class and proto registries
         # NOTE: Explicitly not respecting metaclass inheritance so single
         #   registry shared for all
         _DataBaseMetaClass.class_registry[cls.full_name] = cls
 
         # Add properties that use the underlying backend
-        for field in cls.fields:
+        # also add fields that existed in old_fields
+        # for supporting oneofs
+        # see https://github.com/caikit/caikit/pull/107 for details
+        for field in set(cls.fields + tuple(old_fields)):
             setattr(cls, field, mcs._make_property_getter(field))
 
         # If there is not already an __init__ function defined, make one
         current_init = cls.__init__
         if current_init is None or current_init is DataBase.__init__:
             setattr(cls, "__init__", mcs._make_init(cls.fields))
```

### Comparing `caikit-0.4.1/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.4.2/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/data_backends/base.py` & `caikit-0.4.2/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.4.2/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/dataobject.py` & `caikit-0.4.2/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/enums.py` & `caikit-0.4.2/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/producer.py` & `caikit-0.4.2/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.4.2/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/streams/__init__.py` & `caikit-0.4.2/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/streams/converter.py` & `caikit-0.4.2/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.4.2/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/streams/data_stream.py` & `caikit-0.4.2/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/streams/resolver.py` & `caikit-0.4.2/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/data_model/streams/validator.py` & `caikit-0.4.2/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/model_manager.py` & `caikit-0.4.2/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module.py` & `caikit-0.4.2/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_backend_config.py` & `caikit-0.4.2/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_backends/__init__.py` & `caikit-0.4.2/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_backends/backend_types.py` & `caikit-0.4.2/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_backends/base.py` & `caikit-0.4.2/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_backends/local_backend.py` & `caikit-0.4.2/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_config.py` & `caikit-0.4.2/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_meta.py` & `caikit-0.4.2/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/module_type.py` & `caikit-0.4.2/caikit/core/module_type.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/resources/__init__.py` & `caikit-0.4.2/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/resources/base.py` & `caikit-0.4.2/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/task.py` & `caikit-0.4.2/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/__init__.py` & `caikit-0.4.2/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/compatibility.py` & `caikit-0.4.2/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/errors/__init__.py` & `caikit-0.4.2/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.4.2/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.4.2/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/fileio.py` & `caikit-0.4.2/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/isa.py` & `caikit-0.4.2/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/logging.py` & `caikit-0.4.2/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.4.2/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/serializers.py` & `caikit-0.4.2/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/toolkit/wip_decorator.py` & `caikit-0.4.2/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/workflows/__init__.py` & `caikit-0.4.2/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/core/workflows/base.py` & `caikit-0.4.2/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/__init__.py` & `caikit-0.4.2/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/common/__init__.py` & `caikit-0.4.2/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.4.2/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/common/data_model/producer.py` & `caikit-0.4.2/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/runtime/__init__.py` & `caikit-0.4.2/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.4.2/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.4.2/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/__init__.py` & `caikit-0.4.2/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/dump_services.py` & `caikit-0.4.2/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/grpc_server.py` & `caikit-0.4.2/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/interceptors/__init__.py` & `caikit-0.4.2/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.4.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/metrics/__init__.py` & `caikit-0.4.2/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.4.2/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/__init__.py` & `caikit-0.4.2/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/batcher.py` & `caikit-0.4.2/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/loaded_model.py` & `caikit-0.4.2/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/model_loader.py` & `caikit-0.4.2/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/model_manager.py` & `caikit-0.4.2/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/model_sizer.py` & `caikit-0.4.2/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/model_management/training_manager.py` & `caikit-0.4.2/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/__init__.py` & `caikit-0.4.2/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.4.2/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.4.2/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.4.2/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.4.2/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.4.2/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_factory.py` & `caikit-0.4.2/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.4.2/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.4.2/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/create_service.py` & `caikit-0.4.2/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.4.2/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/primitives.py` & `caikit-0.4.2/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/rpcs.py` & `caikit-0.4.2/caikit/runtime/service_generation/rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.4.2/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/servicers/__init__.py` & `caikit-0.4.2/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.4.2/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.4.2/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.4.2/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.4.2/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.4.2/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/types/__init__.py` & `caikit-0.4.2/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/types/aborted_exception.py` & `caikit-0.4.2/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.4.2/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.4.2/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/utils/__init__.py` & `caikit-0.4.2/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/utils/import_util.py` & `caikit-0.4.2/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/utils/servicer_util.py` & `caikit-0.4.2/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/work_management/__init__.py` & `caikit-0.4.2/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/work_management/abortable_action.py` & `caikit-0.4.2/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/work_management/call_aborter.py` & `caikit-0.4.2/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.4.2/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/docs/adrs/010-data-model-definition.md` & `caikit-0.4.2/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/docs/adrs/015-runtime-service-generation.md` & `caikit-0.4.2/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/docs/adrs/018-shared-backends.md` & `caikit-0.4.2/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/docs/adrs/019-loader-stack.md` & `caikit-0.4.2/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/docs/architecture_club/04-25-23.md` & `caikit-0.4.2/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/start_runtime_with_sample_lib.py` & `caikit-0.4.2/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/README.md` & `caikit-0.4.2/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/client.py` & `caikit-0.4.2/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.4.2/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/start_runtime.py` & `caikit-0.4.2/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.4.2/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.4.2/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py` & `caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/pyproject.toml` & `caikit-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.4.1"
+version = "0.4.2"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.4.1/scripts/fmt.sh` & `caikit-0.4.2/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/__init__.py` & `caikit-0.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/base.py` & `caikit-0.4.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/config/test_configs.py` & `caikit-0.4.2/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/conftest.py` & `caikit-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.4.2/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.4.2/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/blocks/__init__.py` & `caikit-0.4.2/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/blocks/test_base.py` & `caikit-0.4.2/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.4.2/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/streams/test_converter.py` & `caikit-0.4.2/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.4.2/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.4.2/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/streams/test_resolver.py` & `caikit-0.4.2/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/streams/test_validator.py` & `caikit-0.4.2/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/test_base.py` & `caikit-0.4.2/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/data_model/test_dataobject.py` & `caikit-0.4.2/tests/core/data_model/test_dataobject.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import tempfile
 
 # Third Party
 from google.protobuf import descriptor_pool, message
 import pytest
 
 # First Party
-from py_to_proto.dataclass_to_proto import Annotated, OneofField
+from py_to_proto.dataclass_to_proto import Annotated, FieldNumber, OneofField
 
 # Local
 from caikit.core import (  # NOTE: Imported from the top to validate
     DataObjectBase,
     dataobject,
 )
 from caikit.core.data_model import enums
@@ -430,79 +430,75 @@
         "foo": {"data": ["hello"]},
         "bar": None,
         "baz": None,
         "bat": None,
     }
 
 
-# TODO --- This test is currently broken
-#
-# The reason this test is broken is because of the difference between how proto
-# and dataclass treat oneofs. In proto, the name of the oneof is just a label
-# and the elements of the oneof are concrete fields, only one of which may be
-# set at a given time. In a dataclass, a Union field holds the name of the field
-# as the property and the various definitions of that field are all accessed via
-# the name of the Union field.
-#
-# To fix this, we need to figure out the fully-supported oneof semantics for
-# caikit. My gut is that we should support the union of the two where accessing
-# the union/oneof by name gets you whichever of the individual fields is set and
-# accessing any of the individual fields gets you the value iff that is the
-# field within the oneof that's set. The catch is that this would require proper
-# "which oneof" semantics to handle the case where the type of the field does
-# not uniquely identify the sub-field (i.e. oneof delineated by name, not type)
-##
-# def test_dataobject_with_oneof():
-#     """Make sure that using a Union to create a oneof works as expected"""
-
-#     @dataobject
-#     class BazObj:
-#         @dataobject
-#         class Foo:
-#             data: List[str]
-
-#         @dataobject
-#         class Bar:
-#             data: str
-
-#         @dataobject
-#         class Baz:
-#             data: List[str]
-
-#         @dataobject
-#         class Bat:
-#             data1: str
-#             data2: str
-
-#         data_stream: Union[
-#             Annotated[Foo, OneofField("foo")],
-#             Annotated[Bar, OneofField("bar")],
-#             Annotated[Baz, OneofField("baz")],
-#             Annotated[Bat, OneofField("bat")],
-#         ]
-
-#     # proto tests
-#     foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
-#     proto_repr_foo = foo1.to_proto()
-#     assert proto_repr_foo.foo.data == ["hello"]
-#     assert BazObj.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
-
-#     bar1 = BazObj(foo=BazObj.Foo(data=["hello"]), bar=BazObj.Bar(data="world"))
-#     proto_repr_bar = bar1.to_proto()
-#     assert proto_repr_bar.bar.data == "world"
-
-#     # json tests
-#     foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
-#     json_repr_foo = foo1.to_json()
-#     assert json.loads(json_repr_foo) == {
-#         "foo": {"data": ["hello"]},
-#         "bar": None,
-#         "baz": None,
-#         "bat": None,
-#     }
+def test_dataobject_with_oneof():
+    """Make sure that using a Union to create a oneof works as expected"""
+
+    @dataobject
+    class BazObj(DataObjectBase):
+        _private_slots = ("_which_oneof_datastream",)
+
+        @dataobject
+        class Foo(DataObjectBase):
+            data: List[str]
+
+        @dataobject
+        class Bar(DataObjectBase):
+            data: str
+
+        data_stream: Union[
+            Annotated[Foo, FieldNumber(1), OneofField("foo")],
+            Annotated[Bar, FieldNumber(2), OneofField("bar")],
+        ]
+
+        def __getattr__(self, name):
+            if name == "data_stream":
+                if self._which_oneof_datastream == "foo":
+                    return self.foo
+                elif self._which_oneof_datastream == "bar":
+                    return self.bar
+                return None
+            if name == "_foo":
+                if self._which_oneof_datastream == "foo":
+                    return self._data_stream
+            if name == "_bar":
+                if self._which_oneof_datastream == "bar":
+                    return self._data_stream
+
+        def __init__(self, *args, **kwargs):
+            if "foo" in kwargs:
+                self._which_oneof_datastream = "foo"
+                self._data_stream = kwargs["foo"]
+            if "bar" in kwargs:
+                self._which_oneof_datastream = "bar"
+                self._data_stream = kwargs["bar"]
+
+    # proto tests
+    foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
+    assert isinstance(foo1.data_stream, BazObj.Foo)
+    proto_repr_foo = foo1.to_proto()
+    assert proto_repr_foo.foo.data == ["hello"]
+    assert BazObj.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
+
+    bar1 = BazObj(foo=BazObj.Foo(data=["hello"]), bar=BazObj.Bar(data="world"))
+    assert isinstance(bar1.data_stream, BazObj.Bar)
+    proto_repr_bar = bar1.to_proto()
+    assert proto_repr_bar.bar.data == "world"
+
+    # json tests
+    foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
+    json_repr_foo = foo1.to_json()
+    assert json.loads(json_repr_foo) == {
+        "foo": {"data": ["hello"]},
+        "bar": None,
+    }
 
 
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
 
     @dataobject
     class BazObj(DataObjectBase):
```

### Comparing `caikit-0.4.1/tests/core/data_model/test_producer.py` & `caikit-0.4.2/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/helpers.py` & `caikit-0.4.2/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/module_backends/test_backend_types.py` & `caikit-0.4.2/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_imports.py` & `caikit-0.4.2/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_model_manager.py` & `caikit-0.4.2/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_module.py` & `caikit-0.4.2/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_module_backend_config.py` & `caikit-0.4.2/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_module_metadata.py` & `caikit-0.4.2/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_module_type.py` & `caikit-0.4.2/tests/core/test_module_type.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_no_write_permissions.py` & `caikit-0.4.2/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/test_task.py` & `caikit-0.4.2/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/toolkit/test_compatibility.py` & `caikit-0.4.2/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/toolkit/test_error_handler.py` & `caikit-0.4.2/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/toolkit/test_fileio.py` & `caikit-0.4.2/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.4.2/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/toolkit/test_serializers.py` & `caikit-0.4.2/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.4.2/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/workflows/__init__.py` & `caikit-0.4.2/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/core/workflows/test_base.py` & `caikit-0.4.2/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/data_model_helpers.py` & `caikit-0.4.2/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/config/config.yml` & `caikit-0.4.2/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/dummy_block.zip` & `caikit-0.4.2/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/dummy_block/config.yml` & `caikit-0.4.2/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.4.2/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/dummy_resource.zip` & `caikit-0.4.2/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/dummy_workflow.zip` & `caikit-0.4.2/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/fixtures.py` & `caikit-0.4.2/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/invalid.zip` & `caikit-0.4.2/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/linux.txt` & `caikit-0.4.2/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/primitive_party.proto` & `caikit-0.4.2/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.4.2/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.4.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.4.2/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.4.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/generated/__init__.py` & `caikit-0.4.2/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/metrics/__init__.py` & `caikit-0.4.2/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.4.2/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/model_management/__init__.py` & `caikit-0.4.2/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/model_management/test_batcher.py` & `caikit-0.4.2/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/model_management/test_model_loader.py` & `caikit-0.4.2/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/model_management/test_model_manager.py` & `caikit-0.4.2/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.4.2/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/model_management/test_training_manager.py` & `caikit-0.4.2/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.4.2/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/test_create_service.py` & `caikit-0.4.2/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.4.2/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/test_primitives.py` & `caikit-0.4.2/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.4.2/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/servicers/__init__.py` & `caikit-0.4.2/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.4.2/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.4.2/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.4.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.4.2/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.4.2/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/test_grpc_server.py` & `caikit-0.4.2/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/test_service_factory.py` & `caikit-0.4.2/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/utils/__init__.py` & `caikit-0.4.2/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/utils/test_import_util.py` & `caikit-0.4.2/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/utils/test_servicer_util.py` & `caikit-0.4.2/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/work_management/__init__.py` & `caikit-0.4.2/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.4.2/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.4.2/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.4.2/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/tox.ini` & `caikit-0.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.4.1/PKG-INFO` & `caikit-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.4.1
+Version: 0.4.2
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
```

