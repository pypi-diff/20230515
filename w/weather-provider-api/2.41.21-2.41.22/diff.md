# Comparing `tmp/weather_provider_api-2.41.21.tar.gz` & `tmp/weather_provider_api-2.41.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_provider_api-2.41.21.tar", max compression
+gzip compressed data, was "weather_provider_api-2.41.22.tar", max compression
```

## Comparing `weather_provider_api-2.41.21.tar` & `weather_provider_api-2.41.22.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    17098 2023-04-25 06:11:11.020151 weather_provider_api-2.41.21/LICENSE
-drwxr-xr-x   0        0        0        0 2023-04-25 06:11:11.020151 weather_provider_api-2.41.21/LICENSES/
--rw-r--r--   0        0        0    11816 2023-04-25 06:11:11.024152 weather_provider_api-2.41.21/README.md
--rw-r--r--   0        0        0     1905 2023-04-25 06:11:39.924658 weather_provider_api-2.41.21/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/app_config.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/__init__.py
--rw-r--r--   0        0        0      280 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/base_model.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/__init__.py
--rw-r--r--   0        0        0      268 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/additional_responses.py
--rw-r--r--   0        0        0      278 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/api_models.py
--rw-r--r--   0        0        0      503 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/exceptions.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/__init__.py
--rw-r--r--   0        0        0      975 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/error_handling.py
--rw-r--r--   0        0        0     1375 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/headers.py
--rw-r--r--   0        0        0     2174 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/logging.py
--rw-r--r--   0        0        0      790 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/monitoring.py
--rw-r--r--   0        0        0      924 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/mounting.py
--rw-r--r--   0        0        0      303 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/rate_limiter.py
--rw-r--r--   0        0        0      988 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/validation.py
--rw-r--r--   0        0        0      274 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/views.py
--rw-r--r--   0        0        0     2815 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/main.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/__init__.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/__init__.py
--rw-r--r--   0        0        0     6492 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_models.py
--rw-r--r--   0        0        0     5806 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v1.py
--rw-r--r--   0        0        0     9693 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v2.py
--rw-r--r--   0        0        0       91 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/__init__.py
--rw-r--r--   0        0        0     5846 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/model.py
--rw-r--r--   0        0        0     1141 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/source.py
--rw-r--r--   0        0        0     6686 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/controller.py
--rw-r--r--   0        0        0      726 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/exceptions.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/repository/__init__.py
--rw-r--r--   0        0        0    14715 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/repository/repository.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/__init__.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/__init__.py
--rw-r--r--   0        0        0      656 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/cds.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/__init__.py
--rw-r--r--   0        0        0    13650 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/downloader.py
--rw-r--r--   0        0        0     6490 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
--rw-r--r--   0        0        0     6932 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
--rw-r--r--   0        0        0    15478 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
--rw-r--r--   0        0        0      591 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/factors.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/__init__.py
--rw-r--r--   0        0        0     8855 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5land.py
--rw-r--r--   0        0        0     7972 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/__init__.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
--rw-r--r--   0        0        0    24157 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
--rw-r--r--   0        0        0     9343 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
--rw-r--r--   0        0        0     1258 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/knmi.py
--rw-r--r--   0        0        0      415 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
--rw-r--r--   0        0        0    10462 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
--rw-r--r--   0        0        0    15043 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
--rw-r--r--   0        0        0     4265 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
--rw-r--r--   0        0        0    11316 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
--rw-r--r--   0        0        0    13406 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
--rw-r--r--   0        0        0    19917 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/stations.py
--rw-r--r--   0        0        0     2085 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/utils.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
--rw-r--r--   0        0        0     5148 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/__init__.py
--rw-r--r--   0        0        0     4240 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/date_helpers.py
--rw-r--r--   0        0        0     1472 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/file_helpers.py
--rw-r--r--   0        0        0     5742 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/geo_position.py
--rw-r--r--   0        0        0     1791 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/grid_helpers.py
--rw-r--r--   0        0        0      447 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/pandas_helpers.py
--rw-r--r--   0        0        0     5052 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/serializers.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/__init__.py
--rw-r--r--   0        0        0      393 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/erase_arome_repository.py
--rw-r--r--   0        0        0      413 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/erase_era5land_repository.py
--rw-r--r--   0        0        0      381 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/erase_era5sl_repository.py
--rw-r--r--   0        0        0      383 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/update_arome_repository.py
--rw-r--r--   0        0        0      401 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/update_era5land_repository.py
--rw-r--r--   0        0        0      371 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/update_era5sl_repository.py
--rw-r--r--   0        0        0      140 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/versions/__init__.py
--rw-r--r--   0        0        0      469 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/versions/v1.py
--rw-r--r--   0        0        0      469 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/versions/v2.py
--rw-r--r--   0        0        0    13036 1970-01-01 00:00:00.000000 weather_provider_api-2.41.21/PKG-INFO
+-rw-r--r--   0        0        0    17098 2023-05-15 06:40:40.447111 weather_provider_api-2.41.22/LICENSE
+drwxr-xr-x   0        0        0        0 2023-05-15 06:40:40.447111 weather_provider_api-2.41.22/LICENSES/
+-rw-r--r--   0        0        0    11816 2023-05-15 06:40:40.447111 weather_provider_api-2.41.22/README.md
+-rw-r--r--   0        0        0     1905 2023-05-15 06:41:10.791468 weather_provider_api-2.41.22/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/__init__.py
+-rw-r--r--   0        0        0     3704 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/app_config.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/__init__.py
+-rw-r--r--   0        0        0      280 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/base_model.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/errors/__init__.py
+-rw-r--r--   0        0        0      268 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/errors/additional_responses.py
+-rw-r--r--   0        0        0      278 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/errors/api_models.py
+-rw-r--r--   0        0        0      503 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/errors/exceptions.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/error_handling.py
+-rw-r--r--   0        0        0     1375 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/headers.py
+-rw-r--r--   0        0        0     2174 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/logging.py
+-rw-r--r--   0        0        0      790 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/monitoring.py
+-rw-r--r--   0        0        0      924 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/mounting.py
+-rw-r--r--   0        0        0      303 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/rate_limiter.py
+-rw-r--r--   0        0        0      988 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/initializers/validation.py
+-rw-r--r--   0        0        0      274 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/core/views.py
+-rw-r--r--   0        0        0     2815 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/main.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/__init__.py
+-rw-r--r--   0        0        0     6492 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/api_models.py
+-rw-r--r--   0        0        0     5806 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/api_view_v1.py
+-rw-r--r--   0        0        0     9781 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/api_view_v2.py
+-rw-r--r--   0        0        0       91 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/base_models/__init__.py
+-rw-r--r--   0        0        0     5846 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/base_models/model.py
+-rw-r--r--   0        0        0     1141 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/base_models/source.py
+-rw-r--r--   0        0        0     6686 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/controller.py
+-rw-r--r--   0        0        0      726 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/exceptions.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/repository/__init__.py
+-rw-r--r--   0        0        0    14715 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/repository/repository.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/__init__.py
+-rw-r--r--   0        0        0      656 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/cds.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/__init__.py
+-rw-r--r--   0        0        0    13650 2023-05-15 06:40:40.451111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/downloader.py
+-rw-r--r--   0        0        0     6490 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
+-rw-r--r--   0        0        0     6932 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
+-rw-r--r--   0        0        0    15478 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
+-rw-r--r--   0        0        0      591 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/factors.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/models/__init__.py
+-rw-r--r--   0        0        0     8855 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/models/era5land.py
+-rw-r--r--   0        0        0     7972 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
+-rw-r--r--   0        0        0    24157 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
+-rw-r--r--   0        0        0     9343 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
+-rw-r--r--   0        0        0     1258 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/knmi.py
+-rw-r--r--   0        0        0      415 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
+-rw-r--r--   0        0        0    10462 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
+-rw-r--r--   0        0        0    15043 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
+-rw-r--r--   0        0        0     4265 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
+-rw-r--r--   0        0        0    11316 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
+-rw-r--r--   0        0        0    13406 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
+-rw-r--r--   0        0        0    19917 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/stations.py
+-rw-r--r--   0        0        0     2085 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/utils.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
+-rw-r--r--   0        0        0     5148 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/__init__.py
+-rw-r--r--   0        0        0     4240 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/date_helpers.py
+-rw-r--r--   0        0        0     1472 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/file_helpers.py
+-rw-r--r--   0        0        0     5742 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/geo_position.py
+-rw-r--r--   0        0        0     1791 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/grid_helpers.py
+-rw-r--r--   0        0        0      447 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/pandas_helpers.py
+-rw-r--r--   0        0        0     5052 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/serializers.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/__init__.py
+-rw-r--r--   0        0        0      393 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/erase_arome_repository.py
+-rw-r--r--   0        0        0      413 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/erase_era5land_repository.py
+-rw-r--r--   0        0        0      381 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/erase_era5sl_repository.py
+-rw-r--r--   0        0        0      383 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/update_arome_repository.py
+-rw-r--r--   0        0        0      401 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/update_era5land_repository.py
+-rw-r--r--   0        0        0      371 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/scripts/update_era5sl_repository.py
+-rw-r--r--   0        0        0      140 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/versions/__init__.py
+-rw-r--r--   0        0        0      469 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/versions/v1.py
+-rw-r--r--   0        0        0      469 2023-05-15 06:40:40.455111 weather_provider_api-2.41.22/weather_provider_api/versions/v2.py
+-rw-r--r--   0        0        0    13036 1970-01-01 00:00:00.000000 weather_provider_api-2.41.22/PKG-INFO
```

### Comparing `weather_provider_api-2.41.21/LICENSE` & `weather_provider_api-2.41.22/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/README.md` & `weather_provider_api-2.41.22/README.md`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/pyproject.toml` & `weather_provider_api-2.41.22/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather_provider_api"
-version = "2.41.021"
+version = "2.41.022"
 description = "Weather Provider Libraries and API"
 authors = ["Verbindingsteam", "Raoul Linnenbank <58594297+rflinnenbank@users.noreply.github.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository="https://github.com/alliander-opensource/wpla/"
 include = [
     {path = "var_maps/*.json", format = "wheel"}
```

### Comparing `weather_provider_api-2.41.21/weather_provider_api/app_config.py` & `weather_provider_api-2.41.22/weather_provider_api/app_config.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/core/initializers/error_handling.py` & `weather_provider_api-2.41.22/weather_provider_api/core/initializers/error_handling.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/core/initializers/headers.py` & `weather_provider_api-2.41.22/weather_provider_api/core/initializers/headers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/core/initializers/logging.py` & `weather_provider_api-2.41.22/weather_provider_api/core/initializers/logging.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/core/initializers/monitoring.py` & `weather_provider_api-2.41.22/weather_provider_api/core/initializers/monitoring.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/core/initializers/mounting.py` & `weather_provider_api-2.41.22/weather_provider_api/core/initializers/mounting.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/core/initializers/validation.py` & `weather_provider_api-2.41.22/weather_provider_api/core/initializers/validation.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/main.py` & `weather_provider_api-2.41.22/weather_provider_api/main.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_models.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/api_models.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v1.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/api_view_v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v2.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/api_view_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,21 +183,23 @@
     """
     weather_alert = WeatherAlert()
     return weather_alert.get_alarm()
 
 
 # Handler for requests with multiple locations:
 @app.get("/sources/{source_id}/models/{model_id}/multiple-locations/", tags=["sync"])
+@API_RATE_LIMITER.limit("5/minute")
 async def get_sync_weather_multi_loc(
-    source_id: str,
-    model_id: str,
-    cleanup_tasks: BackgroundTasks,
-    ret_args: WeatherContentRequestMultiLocationQuery = Depends(),
-    fmt_args: WeatherFormattingRequestQuery = Depends(),
-    accept: str = Depends(header_accept_type),
+        request: Request,
+        source_id: str,
+        model_id: str,
+        cleanup_tasks: BackgroundTasks,
+        ret_args: WeatherContentRequestMultiLocationQuery = Depends(),
+        fmt_args: WeatherFormattingRequestQuery = Depends(),
+        accept: str = Depends(header_accept_type),
 ):  # pragma: no cover
     starting_time = datetime.utcnow()
     logger.info(f"WeatherRequest({starting_time}): {request.url}", datetime=datetime.utcnow())
 
     source_id = source_id.lower()
     model_id = model_id.lower()
```

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/model.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/base_models/model.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/source.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/base_models/source.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/controller.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/controller.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/exceptions.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/repository/repository.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/repository/repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/cds.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/cds.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/downloader.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/factors.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/factors.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5land.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/models/era5land.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5sl.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/cds/models/era5sl.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/knmi.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/knmi.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/pluim.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/pluim.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/stations.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/stations.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/utils.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/knmi/utils.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/date_helpers.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/file_helpers.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/geo_position.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/geo_position.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/grid_helpers.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/grid_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/serializers.py` & `weather_provider_api-2.41.22/weather_provider_api/routers/weather/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.41.21/PKG-INFO` & `weather_provider_api-2.41.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-provider-api
-Version: 2.41.21
+Version: 2.41.22
 Summary: Weather Provider Libraries and API
 Home-page: https://github.com/alliander-opensource/wpla/
 License: MPL-2.0
 Author: Verbindingsteam
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

