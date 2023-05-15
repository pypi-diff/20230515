# Comparing `tmp/pdfservices-sdk-2.1.2b1.tar.gz` & `tmp/pdfservices-sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfservices-sdk-2.1.2b1.tar", last modified: Mon Jan 16 09:37:01 2023, max compression
+gzip compressed data, was "pdfservices-sdk-2.2.0.tar", last modified: Mon May 15 16:56:39 2023, max compression
```

## Comparing `pdfservices-sdk-2.1.2b1.tar` & `pdfservices-sdk-2.2.0.tar`

### file list

```diff
@@ -1,134 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.146357 pdfservices-sdk-2.1.2b1/
--rw-r--r--   0 runner    (1001) docker     (116)    11333 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1882 2023-01-16 09:37:01.146357 pdfservices-sdk-2.1.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-16 09:37:01.146357 pdfservices-sdk-2.1.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1293 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.134357 pdfservices-sdk-2.1.2b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.134357 pdfservices-sdk-2.1.2b1/src/adobe/
--rw-r--r--   0 runner    (1001) docker     (116)      684 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.134357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1313 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (116)     9410 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/service_account_credentials.py
--rw-r--r--   0 runner    (1001) docker     (116)     4833 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/exception/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5182 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/exception/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3182 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5100 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/cpf_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      850 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/document.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (116)      604 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1669 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output_files.py
--rw-r--r--   0 runner    (1001) docker     (116)     1502 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output_with_report.py
--rw-r--r--   0 runner    (1001) docker     (116)     1319 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output_without_report.py
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_params.py
--rw-r--r--   0 runner    (1001) docker     (116)     1828 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1519 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_outputs.py
--rw-r--r--   0 runner    (1001) docker     (116)     2781 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_params.py
--rw-r--r--   0 runner    (1001) docker     (116)     3137 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/cpf_content_analyzer_req.py
--rw-r--r--   0 runner    (1001) docker     (116)      915 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/cpf_params.py
--rw-r--r--   0 runner    (1001) docker     (116)      770 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/inline_params.py
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/inputs.py
--rw-r--r--   0 runner    (1001) docker     (116)      685 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/outputs.py
--rw-r--r--   0 runner    (1001) docker     (116)      697 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/extract_pdf_output_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)      774 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.138357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1606 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/cpf_content_analyzer_res.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/cpf_status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1447 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6159 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/platform_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5909 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/storage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/auth_factory.py
--rw-r--r--   0 runner    (1001) docker     (116)      857 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (116)     5948 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (116)      872 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/session_token.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/constants/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      836 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/constants/request_key.py
--rw-r--r--   0 runner    (1001) docker     (116)     3368 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/constants/service_constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1157 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1254 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5645 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (116)      690 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/http_method.py
--rw-r--r--   0 runner    (1001) docker     (116)     1475 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/http_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1099 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/request_header_const.py
--rw-r--r--   0 runner    (1001) docker     (116)     8723 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/response_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     2226 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/internal_client_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2142 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/internal_execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/io/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4269 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2846 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (116)      604 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2464 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotagpdf/autotag_data_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     3929 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotagpdf/autotag_pdf_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     7482 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/extract_data_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/extract_data_zipper.py
--rw-r--r--   0 runner    (1001) docker     (116)     3466 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/extract_pdf_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2450 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1057 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/rendition_output.py
--rw-r--r--   0 runner    (1001) docker     (116)     3396 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
--rw-r--r--   0 runner    (1001) docker     (116)     3010 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/path_util.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/io/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3248 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/io/file_ref.py
--rw-r--r--   0 runner    (1001) docker     (116)      959 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9227 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py
--rw-r--r--   0 runner    (1001) docker     (116)     7708 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2756 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.142357 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      784 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py
--rw-r--r--   0 runner    (1001) docker     (116)    10040 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py
--rw-r--r--   0 runner    (1001) docker     (116)      806 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py
--rw-r--r--   0 runner    (1001) docker     (116)      734 2023-01-16 09:36:49.000000 pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 09:37:01.146357 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1882 2023-01-16 09:37:01.000000 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6774 2023-01-16 09:37:01.000000 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-16 09:37:01.000000 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-16 09:37:01.000000 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      304 2023-01-16 09:37:01.000000 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2023-01-16 09:37:01.000000 pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.627454 pdfservices-sdk-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.627454 pdfservices-sdk-2.2.0/src/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.627454 pdfservices-sdk-2.2.0/src/adobe/pdfservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/service_account_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/client_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/platform_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/storage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/session_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/request_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/response_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/path_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/file_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/top_level.txt
```

### Comparing `pdfservices-sdk-2.1.2b1/LICENSE.md` & `pdfservices-sdk-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/PKG-INFO` & `pdfservices-sdk-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pdfservices-sdk
-Version: 2.1.2b1
+Version: 2.2.0
 Summary: Adobe PDFServices Client Library
 Home-page: https://www.adobe.com/go/pdftoolsapi_doc
 Author: Adobe Document Services
 Author-email: extractapi@adobe.com
 License: Apache2
 Description: PDFServices Python SDK
         =======================
         
-        The Adobe PDFServices Python SDK provides APIs for various operations on a PDF. Currently, it contains 
-        * Extract API for extracting elements and renditions from PDFs 
-        * Autotag API for improving accessibility of the PDF document. This generates the tagged PDF, along with an optional XLSX report providing detailed information about the added and already existing tags.
+        The Adobe PDFServices Python SDK provides ML APIs. Currently, it contains 
+        - Extract API for extracting elements and renditions from PDFs
+        - Autotag API for improving accessibility of the PDF document. This generates the tagged PDF, along with an optional XLSX report providing detailed information about the added and already existing tags.
         
         Adobe Document Cloud’s simple cloud-based APIs help you get up and running quickly. Once you’ve received your developer credential, download and set up the sample project. After you’re familiar with the APIs, leverage the samples in your own server-side code.
         
         Installation
         ------------
         
         * Install [Python](https://www.python.org/) 3.6 or higher. 
         * pip install pdfservices-sdk
         
         Resources
         ------------
         
         * [QuickStart](https://www.adobe.com/go/pdftoolsapi_doc)
         * [Samples](https://www.adobe.com/go/pdfservices_python_samples)
-        * [API Reference](https://www.adobe.com/go/pdfservices_python_docs) 
+        * [API Reference](https://www.adobe.com/go/pdfservices_python_docs)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pdfservices-sdk-2.1.2b1/README.md` & `pdfservices-sdk-2.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 PDFServices Python SDK
 =======================
 
-The Adobe PDFServices Python SDK provides APIs for various operations on a PDF. Currently, it contains 
-* Extract API for extracting elements and renditions from PDFs 
-* Autotag API for improving accessibility of the PDF document. This generates the tagged PDF, along with an optional XLSX report providing detailed information about the added and already existing tags.
+The Adobe PDFServices Python SDK provides ML APIs. Currently, it contains 
+- Extract API for extracting elements and renditions from PDFs
+- Autotag API for improving accessibility of the PDF document. This generates the tagged PDF, along with an optional XLSX report providing detailed information about the added and already existing tags.
 
 Adobe Document Cloud’s simple cloud-based APIs help you get up and running quickly. Once you’ve received your developer credential, download and set up the sample project. After you’re familiar with the APIs, leverage the samples in your own server-side code.
 
 Installation
 ------------
 
 * Install [Python](https://www.python.org/) 3.6 or higher. 
 * pip install pdfservices-sdk
 
 Resources
 ------------
 
 * [QuickStart](https://www.adobe.com/go/pdftoolsapi_doc)
 * [Samples](https://www.adobe.com/go/pdfservices_python_samples)
-* [API Reference](https://www.adobe.com/go/pdfservices_python_docs) 
+* [API Reference](https://www.adobe.com/go/pdfservices_python_docs)
```

### Comparing `pdfservices-sdk-2.1.2b1/setup.py` & `pdfservices-sdk-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdfservices-sdk",
-    version="2.1.2b1",
+    version="2.2.0",
     author='Adobe Document Services',
     author_email='extractapi@adobe.com',
     license='Apache2',
     description="Adobe PDFServices Client Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.adobe.com/go/pdftoolsapi_doc",
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/credentials.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/auth/service_account_credentials.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/service_account_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,30 +27,20 @@
     """
     Service Account credentials allow your application to call PDF Tools Extract API on behalf of the application itself,
     or on behalf of an enterprise organization. For getting the credentials,
     `Click Here <https://www.adobe.com/go/pdfextractapi_requestform>`_.
     """
 
     # TODO Can this constructor be excluded from documentation
-    def __init__(self, client_id, client_secret, private_key, organization_id, account_id,
-                 ims_base_uri=ServiceConstants.JWT_BASE_URI, claim=None):
-
+    def __init__(self, client_id, client_secret, private_key, organization_id, account_id):
         self._client_id = _is_valid(client_id, "client_id")
         self._client_secret = _is_valid(client_secret, "client_secret")
         self._private_key = _is_valid(private_key, "private_key")
         self._organization_id = _is_valid(organization_id, "organization_id")
         self._account_id = _is_valid(account_id, "account_id")
-        self.ims_base_uri = ServiceConstants.JWT_BASE_URI if not ims_base_uri else ims_base_uri
-        if not claim:
-            format_str = "{base}{claim}" if self.ims_base_uri.endswith("/") else "{base}/{claim}"
-            claim = format_str.format(
-                base=self.ims_base_uri,
-                claim=ServiceConstants.JWT_CLAIM
-            )
-        self._claim = _is_valid(claim, "claim")
 
     @property
     def client_id(self):
         """ Client Id (API Key) """
         return self._client_id
 
     @property
@@ -60,19 +50,14 @@
 
     @property
     def private_key(self):
         """  Content of the Private Key (PEM format) """
         return self._private_key
 
     @property
-    def claim(self):
-        """ Identifies the Service for which Authorization(Access) Token will be issued"""
-        return self._claim
-
-    @property
     def organization_id(self):
         """Identifies the organization(format: org_ident@AdobeOrg) that has been configured for access to PDF Tools API."""
         return self._organization_id
 
     @property
     def account_id(self):
         """Account ID(format: id@techacct.adobe.com)"""
@@ -87,23 +72,26 @@
         _CLIENT_SECRET = "client_secret"
         _SERVICE_ACCOUNT_CREDENTIALS = "service_account_credentials"
         _PRIVATE_KEY_FILE = "private_key_file"
         _CLAIM = "claim"
         _ORGANIZATION_ID = "organization_id"
         _TECHNICAL_ACCOUNT_ID = "account_id"
         _IMS_BASE_URI = "ims_base_uri"
+        _PDF_SERVICES = "pdf_services"
+        _PDF_SERVICES_URI = "pdf_services_uri"
 
         def __init__(self):
             self._client_id = None
             self._client_secret = None
             self._private_key = None
             self._account_id = None
             self._organization_id = None
             self._ims_base_uri = ServiceConstants.JWT_BASE_URI
             self._claim = None
+            self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI
             return
 
         def with_client_id(self, client_id: str):
             """ Set Client ID (API Key)
 
             :param client_id: Client Id (API Key)
             :type client_id: str
@@ -197,17 +185,21 @@
             if private_key_file_path:
                 # if its not relative to current working directory,
                 # create file path with credentials file directory as working directory
                 if not os.path.exists(path_util.get_file_path(private_key_file_path)):
                     credentials_file_directory = os.path.dirname(path_util.conf_file_abs_path(credentials_file_path))
                     private_key_file_path = os.path.join(credentials_file_directory, private_key_file_path)
                 self._private_key = file_utils.read_conf_file_content(private_key_file_path)
+            pdf_services = config_dict.get(self._PDF_SERVICES, {})
+            self._pdf_services_uri = pdf_services.get(self._PDF_SERVICES_URI, self._pdf_services_uri)
             return self
 
         def build(self):
             """ Returns a new :class:`ServiceAccountCredentials` instance built from the current state of this builder.
 
             :return: A ServiceAccountCredentials instance.
             :rtype: ServiceAccountCredentials
             """
-            return ServiceAccountCredentials(self._client_id, self._client_secret, self._private_key, self._organization_id,
-                                             self._account_id, self._ims_base_uri, self._claim)
+
+            from adobe.pdfservices.operation.internal.auth.service_account_credentials_with_uri import ServiceAccountCredentialsWithUri
+            return ServiceAccountCredentialsWithUri(self._client_id, self._client_secret, self._private_key, self._organization_id, self._account_id,
+                                             self._pdf_services_uri, self._ims_base_uri, self._claim)
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/client_config.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/client_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 import json
 
 from adobe.pdfservices.operation.internal.constants.service_constants import ServiceConstants
 from adobe.pdfservices.operation.internal.util import file_utils
+from adobe.pdfservices.operation.region import Region
 
 
 class ClientConfig(object):
     """
     Encapsulates the API request configurations
     """
     _CONNECT_TIMEOUT_KEY = "connectTimeout"
     _READ_TIMEOUT_KEY = "readTimeout"
     _PDF_SERVICES = "pdf_services"
     _PDF_SERVICES_URI = "pdf_services_uri"
+    _REGION = "region"
 
     @staticmethod
     def builder():
         """Creates a new :class:`ClientConfig` builder.
 
         :return: A ClientConfig.Builder instance.
         :rtype: ClientConfig.Builder
@@ -39,14 +41,48 @@
         Builds a :class:`ClientConfig` instance.
         """
         def __init__(self):
             self._connect_timeout = ServiceConstants.HTTP_CONNECT_TIMEOUT
             self._read_timeout = ServiceConstants.HTTP_READ_TIMEOUT
             self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI
 
+        def with_pdf_services_uri(self, pdf_services_uri: str):
+            """Sets the pdf service uri.
+
+            :param pdf_services_uri: PDF service URI.
+            :type pdf_services_uri: str
+            :return: This Builder instance to add any additional parameters.
+            :rtype: ClientConfig.Builder
+            """
+            self._pdf_services_uri = pdf_services_uri
+            return self
+
+        def with_region(self, region: Region):
+            """Updates the relevant value for the region.
+
+            :param region: Service region(US or EU). Default value is US.
+            :type region: Region
+            :return: This Builder instance to add any additional parameters.
+            :rtype: ClientConfig.Builder
+            """
+            self._set_pdf_services_uri_for_region(region)
+            return self
+
+        def _set_pdf_services_uri_for_region(self, region: Region):
+            """Sets the pdf service uri based on the region.
+
+            :param region: Service region(US or EU).Default value is US.
+            :type region: Region
+            :return: Region specific pdf_services_uri
+            :rtype: str
+            """
+            if region == 'us':
+                self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI_US
+            elif region == 'eu':
+                self._pdf_services_uri = ServiceConstants.PDF_SERVICES_URI_EU
 
         # the time it allows for the client to establish a connection to the server
         def with_connect_timeout(self, connect_timeout: int):
             """Sets the connect timeout. It should be greater than zero.
 
             :param connect_timeout: determines the timeout in milliseconds until a connection is established in the \
                 API calls. Default value is 4000 milliseconds
@@ -83,21 +119,24 @@
 
             JSON structure:
 
             .. code-block:: JSON
 
                 {
                     "connectTimeout": "4000",
-                    "readTimeout": "20000"
+                    "readTimeout": "20000",
+                    "region": "eu"
                 }
             """
             config_json_str = file_utils.read_conf_file_content(client_config_file_path)
             config_dict = json.loads(config_json_str)
             self._connect_timeout = int(config_dict.get(ClientConfig._CONNECT_TIMEOUT_KEY, self._connect_timeout))
             self._read_timeout = int(config_dict.get(ClientConfig._READ_TIMEOUT_KEY, self._read_timeout))
+            region_node = config_dict.get(ClientConfig._REGION)
+            self.with_region(region_node)
             pdf_services_config = config_dict.get(ClientConfig._PDF_SERVICES)
             if pdf_services_config:
                 pdf_services_uri_node = pdf_services_config.get(ClientConfig._PDF_SERVICES_URI)
                 if pdf_services_uri_node:
                     self._pdf_services_uri = pdf_services_uri_node
             return self
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/exception/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/exception/exceptions.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/execution_context.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/execution_context.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/cpf_api.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/platform_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,98 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
+import json
 import logging
-import mimetypes
 from datetime import datetime
 from http import HTTPStatus
-from typing import List
-
 import polling2
+from polling2 import TimeoutException
 import requests
 
-from adobe.pdfservices.operation.exception.exceptions import ServiceApiException, SdkException
-from adobe.pdfservices.operation.internal.api.dto.request.platform.cpf_content_analyzer_req import \
-    CPFContentAnalyzerRequests
+from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
+from adobe.pdfservices.operation.internal.api.dto.response.job_status import JobStatus
+from adobe.pdfservices.operation.internal.constants.request_key import RequestKey
+from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
+from adobe.pdfservices.operation.exception.exceptions import ServiceApiException
+from adobe.pdfservices.operation.internal.api.dto.response.platform.platform_api_response import PlatformApiResponse
 from adobe.pdfservices.operation.internal.exceptions import OperationException
-from adobe.pdfservices.operation.internal.http import http_client
-from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
+from adobe.pdfservices.operation.internal.extension_media_type_mapping import ExtensionMediaTypeMapping
 from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
+from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
-from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
-from adobe.pdfservices.operation.internal.service_constants import ServiceConstants
+from adobe.pdfservices.operation.internal.http import http_client
 from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
-from adobe.pdfservices.operation.internal.io.file_ref_impl import FileRefImpl
-from adobe.pdfservices.operation.internal.service.extract_data_parser import ExtractDataParser
+from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
 
 
-class CPFApi:
-    logger = logging.getLogger(__name__)
+class PlatformApi:
+    operation = '/operation/'
+    POLLING_TIMEOUT_STATUS_CODE = 0
 
     @staticmethod
-    def cpf_create_ops_api(context: InternalExecutionContext, analyzer_request: CPFContentAnalyzerRequests,
-                           source_files: List[FileRefImpl], operation):
-        start_time = datetime.now()
-        multipart_dict: dict = {
-            ServiceConstants.CONTENT_ANALYZER_REQUESTS_STRING:
-                (
-                    ServiceConstants.CONTENT_ANALYZER_REQUESTS_STRING,
-                    analyzer_request.to_json(),
-                    mimetypes.types_map['.json']
-                )
-        }
-        for index, source_file_ref in enumerate(source_files):
-            file_name = 'fileInput' + str(index + 1)
-            multipart_dict[file_name] = (file_name, source_file_ref.get_as_stream())
-
-        if logging.getLogger().isEnabledFor(logging.DEBUG):
-            logging.debug("Upload req: url; %s", context.client_config.get_cpf_ops_create_uri())
-
+    def submit_job(context: InternalExecutionContext, platform_api_request: PlatformApiRequest, operation_endpoint: str,
+                   x_request_id: str, operation_header_info: str):
         http_request = HttpRequest(http_method=HttpMethod.POST,
-                                   url=context.client_config.get_cpf_ops_create_uri(),
-                                   files=multipart_dict,
-                                   headers={DefaultHeaders.X_DCSDK_OPS_INFO_HEADER_NAME: operation},
+                                   request_key=RequestKey.PLATFORM,
+                                   url=context.client_config.get_pdf_services_uri() + PlatformApi.operation +
+                                       operation_endpoint, data=platform_api_request.to_json(),
+                                   headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id,
+                                            DefaultHeaders.X_DCSDK_OPS_INFO_HEADER_NAME: operation_header_info,
+                                            DefaultHeaders.CONTENT_TYPE_HEADER_NAME: ExtensionMediaTypeMapping.JSON.mime_type},
+
                                    authenticator=context.authenticator,
                                    connect_timeout=context.client_config.get_connect_timeout(),
                                    read_timeout=context.client_config.get_read_timeout())
         response = http_client.process_request(http_request=http_request,
-                                               success_status_codes=[HTTPStatus.ACCEPTED],
-                                               error_response_handler=CPFApi.handle_error_response)
-        logging.debug("Upload Operation Latency(ms): %d", (datetime.now() - start_time).microseconds / 1000)
-        return response.headers['location']
-
-    @staticmethod
-    def handle_error_response(response: requests.Response):
-        pass
+                                               success_status_codes=[HTTPStatus.CREATED],
+                                               error_response_handler=PlatformApi.handle_error_response)
+        return response.headers.get('location')
 
     @staticmethod
-    def cpf_status_api(location, context: InternalExecutionContext):
+    def status_poll(context: InternalExecutionContext, location: str, x_request_id: str):
         def is_correct_response(response):
-            return response.status_code == HTTPStatus.OK
+            content = json.loads(response.content)
+            status = content.get('status')
+            if status == JobStatus.FAILED:
+                job_error_response = PlatformApiResponse(status,content.get('error')).get_error_response()
+                raise ServiceApiException(job_error_response.get('message'), ResponseUtil.
+                                          get_request_tracking_id_from_response(response, False), job_error_response
+                                          .get('status'), job_error_response.get('code'))
+            return status == JobStatus.DONE
 
         start_time = datetime.now()
         http_request = HttpRequest(http_method=HttpMethod.GET,
+                                   request_key=RequestKey.STATUS,
                                    url=location,
-                                   headers={},
+                                   headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id},
                                    authenticator=context.authenticator,
                                    connect_timeout=context.client_config.get_connect_timeout(),
                                    read_timeout=context.client_config.get_read_timeout(),
                                    retryable=True)
-        response = polling2.poll(
-            lambda: http_client.process_request(http_request=http_request,
-                                                success_status_codes=[HTTPStatus.OK, HTTPStatus.ACCEPTED],
-                                                error_response_handler=CPFApi.handle_error_response),
-            check_success=is_correct_response,
-            step=0.5,
-            timeout=10 * 60
-        )
-        logging.debug("Upload Operation Latency(ms): %d", (datetime.now() - start_time).microseconds / 1000)
-        return response
+
+        try:
+            response = polling2.poll(
+                lambda: http_client.process_request(http_request=http_request,
+                                                    success_status_codes=[HTTPStatus.OK, HTTPStatus.ACCEPTED],
+                                                    error_response_handler=PlatformApi.handle_error_response),
+                check_success=is_correct_response,
+                step=0.5,
+                timeout=10 * 60
+            )
+            logging.debug(f'Total polling time, Latency(ms): {(datetime.now() - start_time).microseconds / 1000}')
+            return response
+        except TimeoutException:
+            logging.error("Polling Timeout reached. Something's wrong, file operation took too long")
+            raise OperationException(message="Operation execution has timed out!", error_message="Polling Timeout reached", request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(response, True)
+                                     ,status_code=PlatformApi.POLLING_TIMEOUT_STATUS_CODE)
+
+
+    @staticmethod
+    def handle_error_response(response: requests.Response):
+        pass
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/document.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/document.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# governing permissions and limitations under the License.
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_params.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# Copyright 2022 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
+import json
+from adobe.pdfservices.operation.internal.util.json_hint_encoder import JSONHintEncoder
 
-from adobe.pdfservices.operation.internal.api.dto.request.platform.inline_params import InlineParams
 from adobe.pdfservices.operation.pdfops.options.autotagpdf.autotag_pdf_options import AutotagPDFOptions
+from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
 
 
-class AutotagPDFParams(InlineParams):
+class AutotagPDFRequest(PlatformApiRequest):
     json_hint = {
+        'asset_id': 'assetID',
         'generate_report': 'generateReport',
         'shift_headings': 'shiftHeadings'
     }
 
-    def __init__(self, generate_report: bool = None, shift_headings: bool = None):
+    def __init__(self, asset_id: str= None, generate_report: bool = None, shift_headings: bool = None):
         super().__init__()
+        self.asset_id = asset_id
         self.generate_report = generate_report
         self.shift_headings = shift_headings
 
     @classmethod
-    def from_autotag_pdf_options(cls, autotag_pdf_options: AutotagPDFOptions = None):
+    def from_autotag_pdf_options(cls, asset_id, autotag_pdf_options: AutotagPDFOptions = None):
         if autotag_pdf_options is None:
-            return cls
-        return cls(generate_report=autotag_pdf_options.generate_report,
+            return cls(asset_id=asset_id)
+        return cls(asset_id=asset_id,generate_report=autotag_pdf_options.generate_report,
                    shift_headings=autotag_pdf_options.shift_headings)
 
     def to_json(self):
-        raise NotImplementedError("The Function to_json is not implemented")
+        return json.dumps(self, cls=JSONHintEncoder, indent=1, sort_keys=True)
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# Copyright 2022 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-import json
-from adobe.pdfservices.operation.internal.util.json_hint_encoder import JSONHintEncoder
+from logging import getLogger
 
-from adobe.pdfservices.operation.pdfops.options.autotagpdf.autotag_pdf_options import AutotagPDFOptions
-from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
+from adobe.pdfservices.operation.io.file_ref import FileRef
 
+logger = getLogger(__name__)
 
-class AutotagPDFRequest(PlatformApiRequest):
-    json_hint = {
-        'asset_id': 'assetID',
-        'generate_report': 'generateReport',
-        'shift_headings': 'shiftHeadings'
-    }
-
-    def __init__(self, asset_id: str= None, generate_report: bool = None, shift_headings: bool = None):
-        super().__init__()
-        self.asset_id = asset_id
-        self.generate_report = generate_report
-        self.shift_headings = shift_headings
-
-    @classmethod
-    def from_autotag_pdf_options(cls, asset_id, autotag_pdf_options: AutotagPDFOptions = None):
-        if autotag_pdf_options is None:
-            return cls(asset_id=asset_id)
-        return cls(asset_id=asset_id,generate_report=autotag_pdf_options.generate_report,
-                   shift_headings=autotag_pdf_options.shift_headings)
 
-    def to_json(self):
-        return json.dumps(self, cls=JSONHintEncoder, indent=1, sort_keys=True)
+class AutotagPDFOutput:
+    """
+    Class for providing support for output files namely tagged PDF and XLSX report file for AutotagPDFOperation
+    """
+
+    def __init__(self, tagged_pdf: FileRef = None, report: FileRef = None):
+        self._tagged_pdf = tagged_pdf
+        self._report = report
+
+    @property
+    def tagged_pdf(self):
+        return self._tagged_pdf
+
+    @property
+    def report(self):
+        return self._report
+
+    def get_tagged_pdf(self):
+        return self._tagged_pdf
+
+    def get_report(self):
+        return self._report
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_params.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,49 +3,55 @@
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 # 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
+import json
 from typing import List
 
-from adobe.pdfservices.operation.internal.api.dto.request.platform.inline_params import InlineParams
+from adobe.pdfservices.operation.internal.util.json_hint_encoder import JSONHintEncoder
+
+from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
 from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_element_type import ExtractElementType
 from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_renditions_element_type import \
     ExtractRenditionsElementType
 from adobe.pdfservices.operation.pdfops.options.extractpdf.table_structure_type import TableStructureType
 from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_pdf_options import ExtractPDFOptions
 
 
-class ExtractPDFParams(InlineParams):
+class ExtractPDFRequest(PlatformApiRequest):
     json_hint = {
+        'asset_id': 'assetID',
         'elements_to_extract': 'elementsToExtract',
         'renditions_to_extract': 'renditionsToExtract',
         'table_output_format': 'tableOutputFormat',
         'extract_char_info': 'getCharBounds',
         'include_styling_info': 'includeStyling'
     }
 
-    def __init__(self, elements_to_extract: List[ExtractElementType] = None,
+    def __init__(self, asset_id: str = None, elements_to_extract: List[ExtractElementType] = None,
                  renditions_to_extract: List[ExtractRenditionsElementType] = None, table_output_format: TableStructureType = None,
                  extract_char_info: bool = None, include_styling_info: bool = None):
         super().__init__()
+        self.asset_id = asset_id
         self.elements_to_extract = elements_to_extract
         self.renditions_to_extract = renditions_to_extract
         self.table_output_format = table_output_format
         self.extract_char_info = extract_char_info
         self.include_styling_info = include_styling_info
 
     @classmethod
-    def from_extract_pdf_options(cls, extract_pdf_options: ExtractPDFOptions = None):
+    def from_extract_pdf_options(cls, asset_id: str = None, extract_pdf_options: ExtractPDFOptions = None):
         if extract_pdf_options:
-            return cls(elements_to_extract=extract_pdf_options.elements_to_extract,
+            return cls(asset_id=asset_id,
+                       elements_to_extract=extract_pdf_options.elements_to_extract,
                        renditions_to_extract=extract_pdf_options.elements_to_extract_renditions,
                        table_output_format=extract_pdf_options.table_output_format,
                        extract_char_info=extract_pdf_options.get_char_info,
                        include_styling_info=extract_pdf_options.include_styling_info)
         else:
-            return cls(elements_to_extract=[ExtractElementType.TEXT])
+            return cls(asset_id=asset_id, elements_to_extract=[ExtractElementType.TEXT])
 
     def to_json(self):
-        pass
+        return json.dumps(self, cls=JSONHintEncoder, indent=1, sort_keys=True)
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/cpf_content_analyzer_req.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,30 +4,20 @@
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 # 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-import json
+from adobe.pdfservices.operation.auth.credentials import Credentials
+from adobe.pdfservices.operation.auth.service_account_credentials import ServiceAccountCredentials
+from adobe.pdfservices.operation.internal.auth.jwt_authenticator import JwtAuthenticator
 
-from adobe.pdfservices.operation.internal.api.dto.request.platform.engine import Engine
-from adobe.pdfservices.operation.internal.api.dto.request.platform.inputs import Inputs
-from adobe.pdfservices.operation.internal.api.dto.request.platform.outputs import Outputs
-from adobe.pdfservices.operation.internal.util.json_hint_encoder import JSONHintEncoder
 
-
-class CPFContentAnalyzerRequests:
-
-    json_hint = {
-        'engine' : 'cpf:engine',
-        'inputs' : 'cpf:inputs',
-        'outputs' : 'cpf:outputs'
-    }
-
-    def __init__(self, service_id, inputs: Inputs, outputs : Outputs):
-        self.engine = Engine(service_id)
-        self.inputs = inputs
-        self.outputs = outputs
-
-    def to_json(self):
-        return json.dumps(self, cls=JSONHintEncoder, indent=4, sort_keys=True)
+class AuthenticatorFactory:
+
+    @staticmethod
+    def get_authenticator(credential: Credentials):
+        if isinstance(credential, ServiceAccountCredentials):
+            return JwtAuthenticator(credential)
+        else:
+            raise ValueError("Invalid Credentials provided as argument")
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/cpf_params.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-from adobe.pdfservices.operation.internal.api.dto.request.platform.inline_params import InlineParams
+from abc import ABC
 
+class PlatformApiRequest(ABC):
 
-class CPFParams:
-    json_hint = {
-        'inline_params': 'cpf:inline',
-    }
-    inline_params: InlineParams
 
-    def __init__(self, inline_params: InlineParams):
-        self.inline_params = inline_params
+    def __init__(self):
+        return
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/inline_params.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_method.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-from abc import ABC
+import enum
 
-#TODO checck if python has interface instead of just abstract class. if astract can it bbe extended by mutliple classes
-class InlineParams(ABC):
 
-
-    def __init__(self):
-        return
+class HttpMethod(enum.Enum):
+    GET="GET"
+    PUT="PUT"
+    POST="POST"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/inputs.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-from adobe.pdfservices.operation.internal.api.dto.document import Document
-from adobe.pdfservices.operation.internal.api.dto.request.platform.cpf_params import CPFParams
+import enum
 
 
-
-class Inputs:
-
-    json_hint = {
-        'document_in' : 'documentIn',
-        'params' : 'params',
-    }
-
-    def __init__(self, input_file_format, params: CPFParams):
-        self.document_in = Document(input_file_format, 'fileInput1')
-        self.params = params
-
-    def to_json(self):
-        pass
+class JobStatus(str, enum.Enum):
+    """
+    enum of status of the response
+    """
+    IN_PROGRESS = "in_progress"
+    FAILED = "failed"
+    DONE = "done"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/outputs.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/session_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Copyright 2021 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
+# 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-from abc import ABC
 
+from datetime import datetime, timedelta
 
-class Outputs(ABC):
 
-    def __init__(self):
-        return
+class SessionToken:
+
+    expired_at: datetime
+
+    def __init__(self, access_token, expired_in_ms):
+        self.access_token = access_token
+        self.expired_at = datetime.now() + timedelta(milliseconds=expired_in_ms)
+
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/request_key.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-from abc import ABC
+import enum
 
-class PlatformApiRequest(ABC):
 
-
-    def __init__(self):
-        return
+class RequestKey(str, enum.Enum):
+    """
+    enum of RequestKeys in the requests
+    """
+    STATUS = "status"
+    PLATFORM = "platform"
+    UPLOAD = "upload"
+    DOWNLOAD = "download"
+    AUTHN = "ims.session_token"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright 2021 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
+# 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-import enum
 
 
-class JobStatus(str, enum.Enum):
-    """
-    enum of status of the response
-    """
-    IN_PROGRESS = "in_progress"
-    FAILED = "failed"
-    DONE = "done"
+from abc import ABC, abstractmethod
+
+from adobe.pdfservices.operation.execution_context import ExecutionContext
+
+
+class Operation(ABC):
+
+    # Add documentation of exceptions thrown by this method i.e. ServiceApiException, IOException, ServiceUsageException
+    @abstractmethod
+    def execute(self, execution_context : ExecutionContext):
+        pass
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/cpf_content_analyzer_res.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-
 import json
 
-from adobe.pdfservices.operation.internal.api.dto.response.extract_pdf_output_metadata import ExtractPDFOutputMetadata
-from adobe.pdfservices.operation.internal.api.dto.response.platform.cpf_status import CPFStatus
 from adobe.pdfservices.operation.internal.util.json_hint_encoder import JSONHintEncoder, JSONHintDecoder
+from adobe.pdfservices.operation.internal.api.dto.response.platform.job_error_response import JobErrorResponse
 
 
-class ExtractContentAnalyzerResponse(json.JSONDecoder):
+class PlatformApiResponse:
 
     json_hint = {
-        'status': {'name' : 'cpf:status', 'type' : CPFStatus },
-        'outputs': { 'name' : 'cpf:outputs', 'type' : ExtractPDFOutputMetadata}
+        'status': 'status',
+        'error': 'error'
     }
 
-    def __init__(self, outputs : ExtractPDFOutputMetadata = None, status : CPFStatus = None):
-        self.outputs = outputs
+    def __init__(self, status: int, error: JobErrorResponse):
+        self.error = error
         self.status = status
 
+    def get_error_response(self):
+        return self.error
+
+    def get_status(self):
+        return self.status
+
     def to_json(self):
         return json.dumps(self, cls=JSONHintEncoder, indent=4, sort_keys=True)
 
     @staticmethod
-    def from_json( json_str):
-        JSONHintDecoder.current_class = ExtractContentAnalyzerResponse
+    def from_json(json_str):
+        JSONHintDecoder.current_class = PlatformApiResponse
         return JSONHintDecoder.as_class(json.loads(json_str))
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/dto/response/platform/cpf_status.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-import json
-
-
-class CPFStatus(json.JSONDecoder):
+class JobErrorResponse:
 
     json_hint = {
-        'completed' : 'completed',
-        'type' : 'type',
-        'status' : 'status',
-        'report' : 'report',
-        'title' : 'title'
+        'code': 'code',
+        'status': 'status',
+        'message': 'message'
     }
 
-    def __init__(self, completed = None, type= None, status= None, report= None, title= None):
-        self.completed = completed
-        self.type = type
+    def __init__(self, code: str, message : str, status: int):
+        self.code = code
+        self.message = message
         self.status = status
-        self.report = report
-        self.title = title
 
+    def get_code(self):
+        return self.code
+
+    def get_message(self):
+        return self.message
+
+    def get_status(self):
+        return self.status
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/api/platform_api.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/storage_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,97 +3,107 @@
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-import json
+
 import logging
 from datetime import datetime
 from http import HTTPStatus
-import polling2
-from polling2 import TimeoutException
-import requests
 
-from adobe.pdfservices.operation.internal.api.dto.response.job_status import JobStatus
+import requests
 from adobe.pdfservices.operation.internal.constants.request_key import RequestKey
-from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
-from adobe.pdfservices.operation.exception.exceptions import ServiceApiException
-from adobe.pdfservices.operation.internal.api.dto.response.platform.platform_api_response import PlatformApiResponse
 from adobe.pdfservices.operation.internal.exceptions import OperationException
+from adobe.pdfservices.operation.exception.exceptions import ServiceApiException, SdkException
+from adobe.pdfservices.operation.io.file_ref import FileRef
+from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
 from adobe.pdfservices.operation.internal.extension_media_type_mapping import ExtensionMediaTypeMapping
-from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
-from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
 from adobe.pdfservices.operation.internal.http import http_client
-from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
-from adobe.pdfservices.operation.internal.api.dto.request.platform.platform_api_request import PlatformApiRequest
+from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
+from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
+from adobe.pdfservices.operation.internal.api.dto.request.asset_upload_uri_request import AssetUploadURIRequest
+
 
+class StorageApi:
 
-class PlatformApi:
-    operation = '/operation/'
-    POLLING_TIMEOUT_STATUS_CODE = 0
+    assets = "/assets"
 
     @staticmethod
-    def submit_job(context: InternalExecutionContext, platform_api_request: PlatformApiRequest, operation_endpoint: str,
-                   x_request_id: str, operation_header_info: str):
-        http_request = HttpRequest(http_method=HttpMethod.POST,
-                                   request_key=RequestKey.PLATFORM,
-                                   url=context.client_config.get_pdf_services_uri() + PlatformApi.operation +
-                                       operation_endpoint, data=platform_api_request.to_json(),
-                                   headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id,
-                                            DefaultHeaders.X_DCSDK_OPS_INFO_HEADER_NAME: operation_header_info,
-                                            DefaultHeaders.CONTENT_TYPE_HEADER_NAME: ExtensionMediaTypeMapping.JSON.mime_type},
+    def upload_to_cloud(context: InternalExecutionContext, uri: str, source_file_ref: FileRef):
+        try:
+            http_request = HttpRequest(http_method=HttpMethod.PUT,
+                                       request_key=RequestKey.UPLOAD,
+                                       url=uri,
+                                       data=source_file_ref.get_as_stream(),
+                                       headers={DefaultHeaders.CONTENT_TYPE_HEADER_NAME: source_file_ref.get_media_type(
+                                       )},
+                                       connect_timeout=context.client_config.get_connect_timeout(),
+                                       read_timeout=context.client_config.get_read_timeout())
+            response = http_client.process_request(http_request=http_request,
+                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
+                                                   error_response_handler=StorageApi.handle_error_response)
 
-                                   authenticator=context.authenticator,
-                                   connect_timeout=context.client_config.get_connect_timeout(),
-                                   read_timeout=context.client_config.get_read_timeout())
-        response = http_client.process_request(http_request=http_request,
-                                               success_status_codes=[HTTPStatus.CREATED],
-                                               error_response_handler=PlatformApi.handle_error_response)
-        return response.headers.get('location')
+            logging.debug(f'Asset upload response {response}')
+
+            return response
+        except FileNotFoundError as fe:
+            raise fe
+        except IOError as io:
+            raise SdkException(f'Unexpected error while uploading file {io}')
 
     @staticmethod
-    def status_poll(context: InternalExecutionContext, location: str, x_request_id: str):
-        def is_correct_response(response):
-            content = json.loads(response.content)
-            status = content.get('status')
-            if status == JobStatus.FAILED:
-                job_error_response = PlatformApiResponse(status, content.get('error')).get_error_response()
-                raise ServiceApiException(job_error_response.get('message'), ResponseUtil.
-                                          get_request_tracking_id_from_response(response, False), job_error_response
-                                          .get('status'), job_error_response.get('code'))
-            return status == JobStatus.DONE
+    def get_upload_uri(context: InternalExecutionContext, media_type: str, x_request_id: str):
 
-        start_time = datetime.now()
-        http_request = HttpRequest(http_method=HttpMethod.GET,
-                                   request_key=RequestKey.STATUS,
-                                   url=location,
-                                   headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id},
-                                   authenticator=context.authenticator,
-                                   connect_timeout=context.client_config.get_connect_timeout(),
-                                   read_timeout=context.client_config.get_read_timeout(),
-                                   retryable=True)
         try:
+            assetUploadURIRequest = AssetUploadURIRequest(media_type)
 
-            response = polling2.poll(
-                lambda: http_client.process_request(http_request=http_request,
-                                                    success_status_codes=[HTTPStatus.OK, HTTPStatus.ACCEPTED],
-                                                    error_response_handler=PlatformApi.handle_error_response),
-                check_success=is_correct_response,
-                step=0.5,
-                timeout=10 * 60
-            )
-            logging.debug(f'Total polling time, Latency(ms): {(datetime.now() - start_time).microseconds / 1000}')
+            http_request = HttpRequest(http_method=HttpMethod.POST,
+                                       request_key=RequestKey.PLATFORM,
+                                       url=context.client_config.get_pdf_services_uri() + StorageApi.assets,
+                                       data=assetUploadURIRequest.to_json(),
+                                       headers={DefaultHeaders.DC_REQUEST_ID_HEADER_KEY: x_request_id,
+                                                DefaultHeaders.CONTENT_TYPE_HEADER_NAME: ExtensionMediaTypeMapping.JSON.mime_type}
+                                       , authenticator=context.authenticator,
+                                       connect_timeout=context.client_config.get_connect_timeout(),
+                                       read_timeout=context.client_config.get_read_timeout())
+
+            response = http_client.process_request(http_request=http_request,
+                                                   success_status_codes=[HTTPStatus.ACCEPTED, HTTPStatus.OK],
+                                                   error_response_handler=StorageApi.handle_error_response)
             return response
-        except TimeoutException:
-            logging.error("Polling Timeout reached. Something's wrong, file operation took too long")
-            raise OperationException(message="Operation execution has timed out!",
-                                     error_message="Polling Timeout reached",
-                                     request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(response,
-                                                                                                            True)
-                                     , status_code=PlatformApi.POLLING_TIMEOUT_STATUS_CODE)
+
+        except OperationException as oex:
+            raise ServiceApiException(message=oex.error_message, error_code=oex.error_code,
+                                      request_tracking_id=oex.request_tracking_id, status_code=oex.status_code)
 
     @staticmethod
     def handle_error_response(response: requests.Response):
         pass
+
+    @staticmethod
+    def download_and_save_file(context: InternalExecutionContext, uri: str,
+                               destination_path: str):
+
+        start_time = datetime.now()
+        http_request = HttpRequest(http_method=HttpMethod.GET,
+                                   request_key=RequestKey.DOWNLOAD,
+                                   headers={},
+                                   url=uri,
+                                   connect_timeout=context.client_config.get_connect_timeout(),
+                                   read_timeout=context.client_config.get_read_timeout())
+
+        response = http_client.process_request(http_request=http_request,
+                                               success_status_codes=[HTTPStatus.OK, HTTPStatus.ACCEPTED],
+                                               error_response_handler=StorageApi.handle_error_response)
+        logging.debug(f'Upload Operation Latency(ms): {(datetime.now() - start_time).microseconds / 1000}')
+
+        logging.info(f'Downloading file to {destination_path}')
+
+        file = FileRef.create_from_local_file(destination_path)
+        with open(destination_path, 'wb') as f:
+            f.write(response.content)
+        return file
+
+
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/authenticator.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 import sys
 from datetime import datetime, timedelta
 from http import HTTPStatus
 
 import jwt
 
 from adobe.pdfservices.operation.auth.service_account_credentials import ServiceAccountCredentials
+from adobe.pdfservices.operation.internal.auth.service_account_credentials_with_uri import ServiceAccountCredentialsWithUri
 from adobe.pdfservices.operation.exception.exceptions import SdkException
 from adobe.pdfservices.operation.internal.auth.authenticator import Authenticator
 from adobe.pdfservices.operation.internal.auth.session_token import SessionToken
 from adobe.pdfservices.operation.internal.constants.request_key import RequestKey
 from adobe.pdfservices.operation.internal.exceptions import OperationException
 from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
 from adobe.pdfservices.operation.internal.constants.service_constants import ServiceConstants, custom_error_messages
 from adobe.pdfservices.operation.internal.http import http_client
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
 
 
 class JwtAuthenticator(Authenticator):
     token: SessionToken = None
-    service_account_configuration: ServiceAccountCredentials
+    service_account_configuration: ServiceAccountCredentialsWithUri
     jwt_endpoint = ''
 
     def __init__(self, service_account_configuration):
         self.service_account_configuration = service_account_configuration
         self._logger = logging.getLogger(__name__)
         pass
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/auth/session_token.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Copyright 2021 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from datetime import datetime, timedelta
+import enum
 
 
-class SessionToken:
-
-    expired_at: datetime
-
-    def __init__(self, access_token, expired_in_ms):
-        self.access_token = access_token
-        self.expired_at = datetime.now() + timedelta(milliseconds=expired_in_ms)
-
+class TableStructureType(str, enum.Enum):
+    """
+    enum of TableStructureType in a PDF.
+    """
+    CSV = "csv"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/constants/request_key.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/validation_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-import enum
+from typing import Set
 
 
-class RequestKey(str, enum.Enum):
-    """
-    enum of RequestKeys in the requests
-    """
-    STATUS = "status"
-    PLATFORM = "platform"
-    UPLOAD = "upload"
-    DOWNLOAD = "download"
-    AUTHN = "ims.session_token"
+def validate_media_type(allowed_media_types: Set, media_type: str):
+    if not media_type or media_type not in allowed_media_types:
+        raise ValueError("Operation cannot be performed on the specified input media type : {media_type}".format(
+            media_type=media_type))
+
+
+def is_empty(value: str):
+    return not value or value.isspace()
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/constants/service_constants.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,17 +43,20 @@
     HTTP_RETRIABLE_RESPONSE_CODE = 401
     APACHE_CLIENT_MAX_CONNECTION = 200
     APACHE_CLIENT_MAX_CONNECTION_PER_ROUTE = 20
     JWT_BASE_URI = 'https://ims-na1.adobelogin.com'
     JWT_URI_SUFFIX = 'ims/exchange/jwt/'
     JWT_AUDIENCE_SUFFIX = 'c/'
     JWT_CLAIM = 's/ent_documentcloud_sdk'
-    OPERATION_RESULT_TEMP_DIRECTORY = 'sdkResult'
+    OPERATION_RESULT_TEMP_DIRECTORY = 'sdk_result'
+    CPF_OPS_CREATE_URI = 'https://cpf-ue1.adobe.io/ops/:create'
     EXTRACT_OPERATION_ENDPOINT = 'extractpdf'
     AUTOTAG_OPERATION_ENDPOINT = 'autotag'
     TEXT_MIME_TYPE = "text/directory"
     EXTRACT_OPERATION_NAME = "EXTRACT_PDF"
     AUTOTAG_OPERATION_NAME = "AUTOTAG_PDF"
     CONTENT_ANALYZER_REQUESTS_STRING = "contentAnalyzerRequests"
     CONTENT_ANALYZER_RESPONSE_STRING = "contentAnalyzerResponse"
     ASSET_UPLOAD_URI_REQUESTS_STRING = "assetUploadURIRequests"
     PDF_SERVICES_URI = "https://pdf-services.adobe.io"
+    PDF_SERVICES_URI_US = "https://pdf-services-ue1.adobe.io"
+    PDF_SERVICES_URI_EU = "https://pdf-services-ew1.adobe.io"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/exceptions.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import enum
 
 
 class ExtensionMediaTypeMapping(str, enum.Enum):
     PDF = "application/pdf"
     ZIP = "application/zip"
-    XLSX = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
     JSON = "application/json"
+    XLSX = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
 
     @property
     def mime_type(self):
         return self.value
 
     @property
     def extension(self):
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/http_client.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import requests
 
 from adobe.pdfservices.operation.exception.exceptions import SdkException
 from adobe.pdfservices.operation.internal.http.request_header_const import DefaultHeaders
 from adobe.pdfservices.operation.internal.http.response_util import ResponseUtil
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
-from adobe.pdfservices.operation.internal.exceptions import OperationException
 
 _logger = logging.getLogger(__name__)
 
 
 def process_request(http_request: HttpRequest, success_status_codes: List,
                     error_response_handler: Callable[[requests.Response], None]):
     _append_default_headers(http_request.headers)
@@ -38,29 +37,22 @@
         response = _execute_request(http_request)
         if _handle_response_and_retry(response, success_status_codes,
                                       error_response_handler, not http_request.authenticator, http_request.request_key) and http_request.retryable:
             _force_authenticate(http_request)
             # Only single retry is required in case of token expiry
             http_request.retryable = False
         else:
-            if response.status_code not in (200, 201, 202):
-                raise OperationException(message=response.text,
-                                         status_code=response.status_code,
-                                         error_code=response.reason,
-                                         error_message=response.text,
-                                         request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(
-                                             response, False))
             return response
 
 
 def _append_default_headers(headers: dict):
     # Set SDK Info header
     headers[DefaultHeaders.DC_APP_INFO_HEADER_KEY] = "{lang}-{name}-{version}".format(lang="python",
                                                                                       name='pdfservices-sdk',
-                                                                                      version='2.1.2b1')
+                                                                                      version='2.2.0')
     headers[DefaultHeaders.ACCEPT_HEADER_NAME] = DefaultHeaders.JSON_TXT_CONTENT_TYPE
 
 
 def _execute_request(http_request: HttpRequest):
     response = None
     timeout = (http_request.connect_timeout, http_request.read_timeout)
     try:
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/http_method.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright 2021 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
+# 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
+
 import enum
 
 
-class HttpMethod(enum.Enum):
-    GET="GET"
-    PUT="PUT"
-    POST="POST"
+class ExtractElementType(str, enum.Enum):
+    """
+    enum of ElementTypes in a PDF which can be extracted as json.
+    """
+    TEXT = "text"
+    TABLES = "tables"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/http_request.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/request_header_const.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/http/response_util.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/response_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def get_request_tracking_id_from_response(response: requests.Response, is_ims_api_call):
         if is_ims_api_call:
             return response.headers.get("X-DEBUG-ID", None)
         else:
             return response.headers.get("x-request-id", None)
 
     @staticmethod
-    def handle_service_usage_failure(response):
+    def handle_service_usage_failure(response: requests.Response):
         response_content = json.loads(response.content)
         error_code = None
         if response_content.get(CPF_STATUS, None):
             if response_content.get(CPF_STATUS, {}).get(REPORT, None):
                 error_code = ResponseUtil._get_report_error_code(response_content)
             response_content[MESSAGE] = ResponseUtil.QUOTA_ERROR_MESSAGE
         else:
@@ -100,30 +100,29 @@
         raise ServiceUsageException(message=response_content.get('error').get('message'),
                                     request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(response,
                                                                                                            False),
                                     error_code=error_code,
                                     status_code=response.status_code)
 
     @staticmethod
-    def handle_upload_asset_failure(response, request_key):
+    def handle_upload_asset_failure(response: requests.Response, request_key: str):
         if request_key == RequestKey.UPLOAD:
             try:
                     response_content = fromstring(response.content)
                     error_code = response_content.find('Code').text
                     request_id = response_content.find('RequestId').text
                     error_message = response_content.find('Message').text
                     status_code = response.status_code
             except SAXParseException:
                 raise ServiceApiException("Error in uploading file")
             raise OperationException(message="Error response received for request", status_code=status_code,
                                      request_tracking_id=request_id,error_message=error_message,error_code=error_code)
 
     @staticmethod
     def handle_cpf_error_response(response):
-
         response_content = json.loads(response.content)
         error_code = response_content.get(ERROR_CODE, None)
         error_message = response_content.get(MESSAGE, None)
         report_error_code = None
         if response_content.get(STATUS, None):
             error_code = response_content.get(STATUS, None)
             if response_content.get(TITLE, None):
@@ -135,16 +134,14 @@
             if response_content.get(CPF_STATUS, {}).get(REPORT, None):
                 report_error_code = ResponseUtil._get_report_error_code(response_content)
             error_code = response_content.get(CPF_STATUS, {}).get(STATUS, None)
             error_message = response_content.get(CPF_STATUS, {}).get(TITLE, None)
         elif response_content.get(ERROR, None):
             error_code = response.status_code
             error_message = response_content.get(ERROR, {}).get(MESSAGE, None)
-        if response.status_code == 401 and error_code != "401013":
-            return True
         raise OperationException(message="Error response received for request",
                                  request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(response,
                                                                                                         False),
                                  error_code=error_code,
                                  status_code=response.status_code,
                                  error_message=error_message,
                                  report_error_code=report_error_code)
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/internal_client_config.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_client_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,14 @@
         self._connect_timeout = connect_timeout
         self._read_timeout = read_timeout
         self._pdf_services_uri = pdf_services_uri
 
     def get_pdf_services_uri(self):
         return self._pdf_services_uri
 
-    def get_cpf_autotag_service_id(self):
-        return ServiceConstants.CPF_OPS_AUTOTAG_ANALYZER_ID
-
     def get_connect_timeout(self):
         return self._connect_timeout/1000 if self._connect_timeout else None
 
     def get_read_timeout(self):
         return self._read_timeout/1000 if self._read_timeout else None
 
     def validate(self):
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/internal_execution_context.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_execution_context.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/io/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/autotagpdf/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2022 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
+# 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/extract_data_parser.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,177 +4,162 @@
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 # 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-import json
-import os
-import mimetypes
-
-from requests_toolbelt import MultipartDecoder
-
-from adobe.pdfservices.operation.internal.api.dto.response.extract_pdf_output_metadata import ExtractPDFOutputMetadata
-from adobe.pdfservices.operation.internal.api.dto.response.platform.cpf_content_analyzer_res import \
-    ExtractContentAnalyzerResponse
-from adobe.pdfservices.operation.internal.service_constants import ServiceConstants
-from adobe.pdfservices.operation.internal.service.extract_data_zipper import ExtractDataZipper
-from adobe.pdfservices.operation.internal.service.rendition_output import ExtractRenditionOutput
-
-
-class StructuredData:
-    file_format: str
-    data: str
-    elementContentNameToType: dict = {}
-    renditionToPathMapping = {"TABLES": "table",
-                              "FIGURES": "figure"}
-
-    def __init__(self, file_format, data):
-        self.file_format = file_format
-        self.data = data
-        self.parse_data()
-
-    def get_pdfelement_type(self, filename):
-        if filename.find(":") >= 0:
-            filename = filename.split(":")[1]
-        return self.elementContentNameToType.get(filename, "renditions")
-
-    def parse_data(self):
-        if "elements" in self.data:
-            self.update_elements_path_for_tables_and_renditions(self.data["elements"])
-
-    def update_elements_path_for_tables_and_renditions(self, elements):
-        for element in elements:
-            rendition_type = self.pdf_rendition_identifier(element)
-            if rendition_type:
-                fileNames = element["filePaths"]
-                for idx, fileName in enumerate(fileNames):
-                    self.elementContentNameToType[fileName] = rendition_type
-                    fileNames[idx] = "{dir}{path_sep}{file_name}".format(dir=rendition_type.lower(),
-                                                                         path_sep=os.path.sep,
-                                                                         file_name=fileName)
-            # Kids is a list of elements which is present if styling info is included
-            Kids = element.get("Kids", [])
-            if len(Kids) > 0:
-                self.update_elements_path_for_tables_and_renditions(Kids)
-
-
-    def pdf_rendition_identifier(self, pdf_element):
-        if self.is_rendition_element(pdf_element):
-            identifier = pdf_element["Path"].rsplit("/", 1)[1]
-            for key, value in self.renditionToPathMapping.items():
-                if identifier.lower().startswith(value.lower()):
-                    return key
-        return None
-
-    def is_rendition_element(self, pdf_element):
-        if pdf_element and "filePaths" in pdf_element and "Path" in pdf_element:
-            return len(pdf_element["filePaths"]) > 0 and pdf_element["Path"]
-        return False
-
-    def get_file_name(self):
-        return "structuredData" + self.file_format
-
-
-class MultiPartKey:
-    contentAnalyzerResponse: str
-    jsonoutput: str
-    rendition: []
-
-    def __init__(self):
-        self.contentAnalyzerResponse = ''
-        self.jsonoutput = ''
-        self.rendition = []
-
-
-class ExtractDataParser:
-    content: str = None
-    content_type_header: str = None
-    zip_file_path = ''
-    ed_zipper: ExtractDataZipper
-
-    def __init__(self, content, content_type_header, file_path):
-        self.content = content
-        self.content_type_header = content_type_header
-        self.zip_file_path = file_path
-        self.ed_zipper = ExtractDataZipper(file_path)
-
-    @staticmethod
-    def get_key_dstring(cds):
-        if cds.startswith(b'form-data'):
-            cds = cds.decode()
-            return cds.replace("form-data; name=\"", "").replace("\"", "")
-
-    @staticmethod
-    def filename_with_extension(file_name, extension):
-        if extension:
-            file_name += extension
-        return file_name
-
-    @staticmethod
-    def get_extension(file_format):
-        return mimetypes.guess_extension(file_format)
-
-    def frame_extract_rendition_output(self,
-                                       extract_output_metadata: ExtractPDFOutputMetadata,
-                                       structured_data: StructuredData,
-                                       body_part,
-                                       file_name
-                                       ):
-        ero: ExtractRenditionOutput = ExtractRenditionOutput()
-        ero.file_name = file_name
-        ero.body = body_part
-        file_format = extract_output_metadata.indexed_meta_info[file_name].dc_format
-        ero.rendition_extension = ExtractDataParser.get_extension(file_format)
-        ero.pdf_element_type = structured_data.get_pdfelement_type(
-            ExtractDataParser.filename_with_extension(file_name, ero.rendition_extension))
-        return ero
-
-    def get_output_metadata(self, analyzer_str):
-        pass
-
-    @staticmethod
-    def get_keys(key_to_content_map: map):
-        multipart_key = MultiPartKey()
-        for key in key_to_content_map.keys():
-            if ServiceConstants.CONTENT_ANALYZER_RESPONSE_STRING in key:
-                multipart_key.contentAnalyzerResponse = key
-            elif 'jsonoutput' in key:
-                multipart_key.jsonoutput = key
-            else:
-                multipart_key.rendition.append(key)
-        return multipart_key
-
-    def parse(self):
-
-        decoded_content = MultipartDecoder(self.content,
-                                           self.content_type_header)
-        key_to_content_map = {}
-        for part in decoded_content.parts:
-            cds = part.headers[b'Content-Disposition']
-            key = ExtractDataParser.get_key_dstring(cds)
-            key_to_content_map[key] = part.content
-
-        # For Json Response
-        keys: MultiPartKey = ExtractDataParser.get_keys(key_to_content_map)
-        extract_json = key_to_content_map[keys.contentAnalyzerResponse].decode()
-        extract_content_analyzer_res = ExtractContentAnalyzerResponse.from_json(extract_json)
-        extract_output_metadata: ExtractPDFOutputMetadata = extract_content_analyzer_res.outputs
-
-        # For ElementsInfo
-        structured_output = key_to_content_map[keys.jsonoutput].decode()
-        mt = mimetypes.MimeTypes()
-        extension = mt.guess_extension(extract_output_metadata.indexed_meta_info[keys.jsonoutput].dc_format)
-        structure_output: StructuredData = StructuredData(
-            extension,
-            json.loads(structured_output))
-        self.ed_zipper.add_structured_data(structure_output)
-
-        # For Elements Renditions
-        for rendition_key in keys.rendition:
-            rendition_output: ExtractRenditionOutput = self.frame_extract_rendition_output(
-                extract_output_metadata,
-                structure_output,
-                key_to_content_map[rendition_key],
-                rendition_key)
-            self.ed_zipper.add_rendition_data(rendition_output)
+import logging
+import uuid
+
+from adobe.pdfservices.operation.execution_context import ExecutionContext
+from adobe.pdfservices.operation.internal.api.storage_api import StorageApi
+from adobe.pdfservices.operation.internal.extension_media_type_mapping import ExtensionMediaTypeMapping
+from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
+from adobe.pdfservices.operation.internal.service.extract_pdf_service import ExtractPDFService
+from adobe.pdfservices.operation.internal.util.file_utils import get_transaction_id
+from adobe.pdfservices.operation.internal.util.path_util import get_temporary_destination_path
+from adobe.pdfservices.operation.internal.util.validation_util import validate_media_type
+from adobe.pdfservices.operation.io.file_ref import FileRef
+from adobe.pdfservices.operation.operation import Operation
+from adobe.pdfservices.operation.exception.exceptions import ServiceApiException
+from adobe.pdfservices.operation.pdfops.options.extractpdf.extract_pdf_options import ExtractPDFOptions
+
+
+class ExtractPDFOperation(Operation):
+    """An Operation that extracts pdf elements such as text and tables in a structured format from a PDF, along
+    with renditions for tables and figures.
+
+    Sample usage.
+
+    .. code-block:: python
+
+        try:
+            base_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+
+            credentials = Credentials.service_account_credentials_builder() \\
+                .from_file(base_path + "/pdfservices-api-credentials.json") \\
+                .build()
+
+            execution_context = ExecutionContext.create(credentials)
+            extract_pdf_operation = ExtractPDFOperation.create_new()
+
+            source = FileRef.create_from_local_file(base_path + "/resources/extractPdfInput.pdf")
+            extract_pdf_operation.set_input(source)
+
+            extract_pdf_options: ExtractPDFOptions = ExtractPDFOptions.builder() \\
+                .with_elements_to_extract([ExtractElementType.TEXT, ExtractElementType.TABLES]) \\
+                .with_elements_to_extract_renditions([ExtractRenditionsElementType.TABLES, ExtractRenditionsElementType.FIGURES]) \\
+                .with_get_char_info(True) \\
+                .with_include_styling_info(True) \\
+                .build()
+            extract_pdf_operation.set_options(extract_pdf_options)
+
+            result: FileRef = extract_pdf_operation.execute(execution_context)
+
+            result.save_as(base_path + "/output/ExtractTextTableWithFigureTableRendition.zip")
+        except (ServiceApiException, ServiceUsageException, SdkException):
+            logging.exception("Exception encountered while executing operation")
+
+    """
+
+    SUPPORTED_SOURCE_MEDIA_TYPES = {ExtensionMediaTypeMapping.PDF.mime_type}
+    """ Supported source file formats for :class:`ExtractPdfOperation` is .pdf."""
+
+    __create_key = object()
+
+    def __init__(self, create_key):
+        assert (create_key == ExtractPDFOperation.__create_key), \
+            "Operation objects must be created using create_new"
+        self._source_file_ref = None
+        self._is_invoked = False
+        self._extract_pdf_options = None
+        self._logger = logging.getLogger(__name__)
+
+    @classmethod
+    def create_new(cls):
+        """ creates a new instance of `ExtractPDFOperation`.
+
+        :return: A new instance of ExtractPDFOperation
+        :rtype: ExtractPDFOperation
+        """
+        return ExtractPDFOperation(cls.__create_key)
+
+    def get_options(self):
+        """gets the ExtractPDFOptions.
+
+        :return: The options parameter of the operation
+        :rtype: ExtractPDFOptions
+        """
+
+        return self._extract_pdf_options
+
+    def set_options(self, extract_pdf_options: ExtractPDFOptions):
+        """ sets the ExtractPDFOptions.
+
+        :param extract_pdf_options: ExtractPDFOptions to set.
+        :type extract_pdf_options: ExtractPDFOptions
+        :return: This instance to add any additional parameters.
+        :rtype: ExtractPDFOperation
+        """
+        if not isinstance(extract_pdf_options, ExtractPDFOptions):
+            raise ValueError("Only ExtractPDFOptions type instance is accepted")
+        self._extract_pdf_options = extract_pdf_options
+        return self
+
+    def set_input(self, source_file_ref: FileRef):
+        """
+        Sets an input file.
+
+        :param source_file_ref: An input file.
+        :type source_file_ref: FileRef
+        :return: This instance to add any additional parameters.
+        :rtype: ExtractPDFOperation
+        """
+        if not isinstance(source_file_ref, FileRef):
+            raise ValueError("Only FileRef type instance is accepted")
+        self._source_file_ref = source_file_ref
+        return self
+
+    def execute(self, execution_context: ExecutionContext):
+        """
+        Executes this operation synchronously using the supplied context and returns a new FileRef instance for the resulting Zip file.
+        The resulting file may be stored in the system temporary directory. See :class:`adobe.pdfservices.operation.io.file_ref.FileRef` for how temporary resources are cleaned up.
+
+        :param execution_context: The context in which the operation will be executed.
+        :type execution_context: ExecutionContext
+        :return: The FileRef to the result.
+        :rtype: FileRef
+        :raises ServiceApiException: if an API call results in an error response.
+        """
+        try:
+            self._validate_invocation_count()
+            self._validate(execution_context=execution_context)
+            self._logger.info("All validations successfully done. Beginning ExtractPDF operation execution")
+
+            x_request_id = str(uuid.uuid4())
+            download_uri = ExtractPDFService.extract_pdf(execution_context, self._source_file_ref, self.get_options(),
+                                                         x_request_id)
+
+            file_location = get_temporary_destination_path(target_extension=ExtensionMediaTypeMapping.ZIP.extension)
+            file = StorageApi.download_and_save_file(execution_context, download_uri, file_location)
+            self._logger.info(f'Extract Operation Successful - Transaction ID: {get_transaction_id(x_request_id)}')
+
+            return file
+
+        except ServiceApiException as se:
+            raise se
+        except Exception as ex:
+            raise ex
+
+    def _validate_invocation_count(self):
+        if self._is_invoked:
+            self._logger.error("Operation instance must only be invoked once")
+            raise ValueError("Operation instance must not be reused, can only be invoked once")
+
+    def _validate(self, execution_context: InternalExecutionContext):
+        if not execution_context:
+            raise ValueError("Client Context not initialized before invoking the operation")
+        execution_context.validate()
+        if not self._source_file_ref:
+            raise ValueError("No input was set for operation")
+        validate_media_type(self.SUPPORTED_SOURCE_MEDIA_TYPES, self._source_file_ref.get_media_type())
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/file_utils.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/internal/util/path_util.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/path_util.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/io/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/io/file_ref.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/file_ref.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright 2022 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 import logging
 import uuid
 
 from adobe.pdfservices.operation.exception.exceptions import ServiceApiException
 from adobe.pdfservices.operation.execution_context import ExecutionContext
-from adobe.pdfservices.operation.internal.api.dto.request.autotagpdf.autotag_pdf_output_files import \
-    AutotagPDFOutputFiles
+from adobe.pdfservices.operation.internal.api.dto.request.autotagpdf.autotag_pdf_output import \
+    AutotagPDFOutput
 from adobe.pdfservices.operation.internal.exceptions import OperationException
 from adobe.pdfservices.operation.internal.extension_media_type_mapping import ExtensionMediaTypeMapping
 from adobe.pdfservices.operation.internal.internal_execution_context import InternalExecutionContext
 from adobe.pdfservices.operation.internal.api.storage_api import StorageApi
 from adobe.pdfservices.operation.internal.util.file_utils import get_transaction_id
 from adobe.pdfservices.operation.internal.util.path_util import get_temporary_destination_path
 from adobe.pdfservices.operation.internal.util.validation_util import validate_media_type
@@ -54,25 +54,25 @@
 
             autotag_pdf_options: AutotagPDFOptions = AutotagPDFOptions.builder() \\
                 .with_shift_headings() \\
                 .with_generate_report() \\
                 .build()
             autotag_pdf_operation.set_options(autotag_pdf_options)
 
-            autotag_output_files: AutotagPDFOutputFiles = autotag_pdf_operation.execute(execution_context)
+            autotag_pdf_output: AutotagPDFOutput = autotag_pdf_operation.execute(execution_context)
 
             input_file_name = Path(input_file_path).stem
             base_output_path = base_path + "/output/AutotagPDFWithOptions/"
 
             Path(base_output_path).mkdir(parents=True, exist_ok=True)
             tagged_pdf_path = f'{base_output_path}{input_file_name}-tagged.pdf'
             report_path = f'{base_output_path}{input_file_name}-report.xlsx'
 
-            autotag_output_files.save_pdf_file(tagged_pdf_path)
-            autotag_output_files.save_xls_file(report_path)
+            autotag_pdf_output.get_tagged_pdf().save_as(tagged_pdf_path)
+            autotag_pdf_output.get_report().save_as(report_path)
 
         except (ServiceApiException, ServiceUsageException, SdkException) as e:
             logging.exception(f'Exception encountered while executing operation: {e}')
 
     """
 
     SUPPORTED_SOURCE_MEDIA_TYPES = {ExtensionMediaTypeMapping.PDF.mime_type}
@@ -130,49 +130,48 @@
         if not isinstance(source_file_ref, FileRef):
             raise ValueError("Invalid input file type. Only FileRef type instance is accepted")
         self._source_file_ref = source_file_ref
         return self
 
     def execute(self, execution_context: ExecutionContext):
         """
-        Executes this operation synchronously using the supplied context and returns a new AutotagPDFOutputFiles
+        Executes this operation synchronously using the supplied context and returns a new AutotagPDFOutput
         instance for the generated tagged pdf file and XLSX report file. The resulting file may be stored in the system
         temporary directory.
         See :class:`adobe.pdfservices.operation.io.file_ref.FileRef` for how temporary resources are cleaned up.
 
         :param execution_context: The context in which the operation will be executed.
         :type execution_context: ExecutionContext
-        :return: The instance of AutotagPDFOutputFiles.
-        :rtype: AutotagPDFOutputFiles
+        :return: The instance of AutotagPDFOutput.
+        :rtype: AutotagPDFOutput
         :raises ServiceApiException: if an API call results in an error response.
         """
         try:
             self._validate(execution_context=execution_context)
             self._logger.info("All validations successfully done. Beginning AutotagPDF operation execution")
 
             x_request_id = str(uuid.uuid1())
             download_uri_list = AutotagPDFService.autotag_pdf(execution_context, self._source_file_ref, self.get_options(),
                                                          x_request_id)
             self._is_invoked = True
             temporary_tagged_pdf_destination_path = get_temporary_destination_path(target_extension=ExtensionMediaTypeMapping.PDF.extension)
             temporary_report_destination_path = get_temporary_destination_path(
                 target_extension=ExtensionMediaTypeMapping.XLSX.extension)
             StorageApi.download_and_save_file(execution_context, download_uri_list[0],
-                                           temporary_tagged_pdf_destination_path)
-
-            autotag_pdf_output_files = AutotagPDFOutputFiles()
-            autotag_pdf_output_files.pdf_file = FileRef.create_from_local_file(temporary_tagged_pdf_destination_path)
-
+                                              temporary_tagged_pdf_destination_path)
             if self.get_options() is not None and self.get_options().generate_report == True:
                 StorageApi.download_and_save_file(execution_context, download_uri_list[1],
-                                            temporary_report_destination_path)
-                autotag_pdf_output_files.xls_file = FileRef.create_from_local_file(temporary_report_destination_path)
+                                                  temporary_report_destination_path)
+                autotag_pdf_output = AutotagPDFOutput(FileRef.create_from_local_file(temporary_tagged_pdf_destination_path),
+                                                                        FileRef.create_from_local_file(temporary_report_destination_path))
+            else:
+                autotag_pdf_output = AutotagPDFOutput(FileRef.create_from_local_file(temporary_tagged_pdf_destination_path))
 
             self._logger.info("Autotag Operation Successful - Request ID: %s", x_request_id)
-            return autotag_pdf_output_files
+            return autotag_pdf_output
 
         except ServiceApiException as se:
             raise se
 
         except Exception as ex:
             raise ex
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2022 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# governing permissions and limitations under the License.
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2021 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
+# governing permissions and limitations under the License.
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 import enum
 
 
-class ExtractElementType(str, enum.Enum):
+class ExtractRenditionsElementType(str, enum.Enum):
     """
-    enum of ElementTypes in a PDF which can be extracted as json.
+    enum of ElementTypes in a PDF which can be extracted as renditions.
     """
-    TEXT = "text"
     TABLES = "tables"
+    FIGURES = "figures"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.1.2b1/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py` & `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,9 @@
-# Copyright 2021 Adobe. All rights reserved.
+# Copyright 2023 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-
-import enum
-
-
-class TableStructureType(str, enum.Enum):
-    """
-    enum of TableStructureType in a PDF.
-    """
-    CSV = "csv"
```

### Comparing `pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/PKG-INFO` & `pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pdfservices-sdk
-Version: 2.1.2b1
+Version: 2.2.0
 Summary: Adobe PDFServices Client Library
 Home-page: https://www.adobe.com/go/pdftoolsapi_doc
 Author: Adobe Document Services
 Author-email: extractapi@adobe.com
 License: Apache2
 Description: PDFServices Python SDK
         =======================
         
-        The Adobe PDFServices Python SDK provides APIs for various operations on a PDF. Currently, it contains 
-        * Extract API for extracting elements and renditions from PDFs 
-        * Autotag API for improving accessibility of the PDF document. This generates the tagged PDF, along with an optional XLSX report providing detailed information about the added and already existing tags.
+        The Adobe PDFServices Python SDK provides ML APIs. Currently, it contains 
+        - Extract API for extracting elements and renditions from PDFs
+        - Autotag API for improving accessibility of the PDF document. This generates the tagged PDF, along with an optional XLSX report providing detailed information about the added and already existing tags.
         
         Adobe Document Cloud’s simple cloud-based APIs help you get up and running quickly. Once you’ve received your developer credential, download and set up the sample project. After you’re familiar with the APIs, leverage the samples in your own server-side code.
         
         Installation
         ------------
         
         * Install [Python](https://www.python.org/) 3.6 or higher. 
         * pip install pdfservices-sdk
         
         Resources
         ------------
         
         * [QuickStart](https://www.adobe.com/go/pdftoolsapi_doc)
         * [Samples](https://www.adobe.com/go/pdfservices_python_samples)
-        * [API Reference](https://www.adobe.com/go/pdfservices_python_docs) 
+        * [API Reference](https://www.adobe.com/go/pdfservices_python_docs)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pdfservices-sdk-2.1.2b1/src/pdfservices_sdk.egg-info/SOURCES.txt` & `pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,84 +5,64 @@
 setup.py
 src/adobe/__init__.py
 src/adobe/pdfservices/__init__.py
 src/adobe/pdfservices/operation/__init__.py
 src/adobe/pdfservices/operation/client_config.py
 src/adobe/pdfservices/operation/execution_context.py
 src/adobe/pdfservices/operation/operation.py
+src/adobe/pdfservices/operation/region.py
 src/adobe/pdfservices/operation/auth/__init__.py
 src/adobe/pdfservices/operation/auth/credentials.py
 src/adobe/pdfservices/operation/auth/service_account_credentials.py
 src/adobe/pdfservices/operation/exception/__init__.py
 src/adobe/pdfservices/operation/exception/exceptions.py
 src/adobe/pdfservices/operation/internal/__init__.py
 src/adobe/pdfservices/operation/internal/exceptions.py
 src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
 src/adobe/pdfservices/operation/internal/internal_client_config.py
 src/adobe/pdfservices/operation/internal/internal_execution_context.py
-src/adobe/pdfservices/operation/internal/service_constants.py
 src/adobe/pdfservices/operation/internal/api/__init__.py
-src/adobe/pdfservices/operation/internal/api/cpf_api.py
 src/adobe/pdfservices/operation/internal/api/platform_api.py
 src/adobe/pdfservices/operation/internal/api/storage_api.py
 src/adobe/pdfservices/operation/internal/api/dto/__init__.py
 src/adobe/pdfservices/operation/internal/api/dto/document.py
 src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
 src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
-src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_outputs.py
-src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_params.py
 src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py
 src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
-src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output_files.py
-src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output_with_report.py
-src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output_without_report.py
-src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_params.py
+src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py
 src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py
 src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py
-src/adobe/pdfservices/operation/internal/api/dto/request/platform/cpf_content_analyzer_req.py
-src/adobe/pdfservices/operation/internal/api/dto/request/platform/cpf_params.py
 src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py
-src/adobe/pdfservices/operation/internal/api/dto/request/platform/inline_params.py
-src/adobe/pdfservices/operation/internal/api/dto/request/platform/inputs.py
-src/adobe/pdfservices/operation/internal/api/dto/request/platform/outputs.py
 src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py
 src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
-src/adobe/pdfservices/operation/internal/api/dto/response/extract_pdf_output_metadata.py
 src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
 src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py
-src/adobe/pdfservices/operation/internal/api/dto/response/platform/cpf_content_analyzer_res.py
-src/adobe/pdfservices/operation/internal/api/dto/response/platform/cpf_status.py
 src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
 src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
 src/adobe/pdfservices/operation/internal/auth/__init__.py
 src/adobe/pdfservices/operation/internal/auth/auth_factory.py
 src/adobe/pdfservices/operation/internal/auth/authenticator.py
 src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
+src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py
 src/adobe/pdfservices/operation/internal/auth/session_token.py
 src/adobe/pdfservices/operation/internal/constants/__init__.py
 src/adobe/pdfservices/operation/internal/constants/request_key.py
 src/adobe/pdfservices/operation/internal/constants/service_constants.py
 src/adobe/pdfservices/operation/internal/http/__init__.py
 src/adobe/pdfservices/operation/internal/http/http_client.py
 src/adobe/pdfservices/operation/internal/http/http_method.py
 src/adobe/pdfservices/operation/internal/http/http_request.py
 src/adobe/pdfservices/operation/internal/http/request_header_const.py
 src/adobe/pdfservices/operation/internal/http/response_util.py
 src/adobe/pdfservices/operation/internal/io/__init__.py
 src/adobe/pdfservices/operation/internal/io/file_ref_impl.py
 src/adobe/pdfservices/operation/internal/service/__init__.py
 src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py
-src/adobe/pdfservices/operation/internal/service/extract_data_parser.py
-src/adobe/pdfservices/operation/internal/service/extract_data_zipper.py
-src/adobe/pdfservices/operation/internal/service/extract_pdf_api.py
 src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py
-src/adobe/pdfservices/operation/internal/service/rendition_output.py
-src/adobe/pdfservices/operation/internal/service/autotagpdf/__init__.py
-src/adobe/pdfservices/operation/internal/service/autotagpdf/autotag_data_parser.py
-src/adobe/pdfservices/operation/internal/service/autotagpdf/autotag_pdf_api.py
 src/adobe/pdfservices/operation/internal/util/__init__.py
 src/adobe/pdfservices/operation/internal/util/file_utils.py
 src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
 src/adobe/pdfservices/operation/internal/util/path_util.py
 src/adobe/pdfservices/operation/internal/util/validation_util.py
 src/adobe/pdfservices/operation/io/__init__.py
 src/adobe/pdfservices/operation/io/file_ref.py
```

