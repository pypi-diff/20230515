# Comparing `tmp/orwynn-1.0.0b2.tar.gz` & `tmp/orwynn-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orwynn-1.0.0b2.tar", max compression
+gzip compressed data, was "orwynn-1.0.0b3.tar", max compression
```

## Comparing `orwynn-1.0.0b2.tar` & `orwynn-1.0.0b3.tar`

### file list

```diff
@@ -1,258 +1,258 @@
--rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0b2/LICENSE
--rw-r--r--   0        0        0        8 2022-12-09 11:58:05.154110 orwynn-1.0.0b2/README.md
--rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0b2/orwynn/__init__.py
--rw-r--r--   0        0        0       63 2022-12-11 09:09:39.933971 orwynn-1.0.0b2/orwynn/_di/Acceptor.py
--rw-r--r--   0        0        0      500 2023-03-06 12:12:57.645660 orwynn-1.0.0b2/orwynn/_di/BUILTIN_ACCEPTORS.py
--rw-r--r--   0        0        0      399 2023-02-28 05:48:16.657065 orwynn-1.0.0b2/orwynn/_di/BUILTIN_PROVIDERS.py
--rw-r--r--   0        0        0     4726 2023-04-03 14:59:49.701980 orwynn-1.0.0b2/orwynn/_di/Di.py
--rw-r--r--   0        0        0     6038 2023-04-03 14:59:49.636980 orwynn-1.0.0b2/orwynn/_di/DiContainer.py
--rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0b2/orwynn/_di/DiObject.py
--rw-r--r--   0        0        0      119 2023-03-06 11:23:49.043895 orwynn-1.0.0b2/orwynn/_di/DiObjectAlreadyInitializedInContainerError.py
--rw-r--r--   0        0        0      132 2023-03-06 11:23:49.043895 orwynn-1.0.0b2/orwynn/_di/FinalizedDiContainerError.py
--rw-r--r--   0        0        0       51 2023-03-06 11:23:49.043895 orwynn-1.0.0b2/orwynn/_di/MissingDiObjectError.py
--rw-r--r--   0        0        0       96 2023-03-06 11:23:49.043895 orwynn-1.0.0b2/orwynn/_di/NoAnnotationError.py
--rw-r--r--   0        0        0      291 2023-03-06 11:23:49.043895 orwynn-1.0.0b2/orwynn/_di/NotProviderError.py
--rw-r--r--   0        0        0       39 2022-12-11 09:09:05.931124 orwynn-1.0.0b2/orwynn/_di/Provider.py
--rw-r--r--   0        0        0      579 2023-03-06 11:30:55.552595 orwynn-1.0.0b2/orwynn/_di/ProviderAvailabilityError.py
--rw-r--r--   0        0        0      101 2023-03-06 14:58:11.412882 orwynn-1.0.0b2/orwynn/_di/__init__.py
--rw-r--r--   0        0        0     1733 2023-03-06 14:58:30.471950 orwynn-1.0.0b2/orwynn/_di/_collect_dependencies_for_acceptor.py
--rw-r--r--   0        0        0     3856 2023-02-28 05:48:16.658066 orwynn-1.0.0b2/orwynn/_di/check_availability.py
--rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0b2/orwynn/_di/collecting/ModuleCollector.py
--rw-r--r--   0        0        0      459 2023-03-06 11:30:55.551595 orwynn-1.0.0b2/orwynn/_di/collecting/ProviderAlreadyInitializedForMapError.py
--rw-r--r--   0        0        0     1086 2023-04-03 14:59:49.701980 orwynn-1.0.0b2/orwynn/_di/collecting/collect_modules_test.py
--rw-r--r--   0        0        0     3305 2023-04-03 14:59:49.702980 orwynn-1.0.0b2/orwynn/_di/collecting/collect_provider_dependencies.py
--rw-r--r--   0        0        0     1709 2023-02-28 06:25:30.262229 orwynn-1.0.0b2/orwynn/_di/collecting/collect_provider_dependencies_test.py
--rw-r--r--   0        0        0     3210 2023-02-28 05:48:16.648064 orwynn-1.0.0b2/orwynn/_di/collecting/get_parameters_for_provider.py
--rw-r--r--   0        0        0      324 2023-03-06 11:30:55.551595 orwynn-1.0.0b2/orwynn/_di/collecting/no_dependencies_for_given_provider_error.py
--rw-r--r--   0        0        0     2523 2023-02-27 12:30:57.696823 orwynn-1.0.0b2/orwynn/_di/collecting/provider_dependencies_map.py
--rw-r--r--   0        0        0      138 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/_di/collecting/provider_keyword_attribute_error.py
--rw-r--r--   0        0        0      376 2023-03-06 11:30:55.550595 orwynn-1.0.0b2/orwynn/_di/collecting/provider_not_found_in_map_error.py
--rw-r--r--   0        0        0      519 2023-02-28 05:48:16.651064 orwynn-1.0.0b2/orwynn/_di/di_test.py
--rw-r--r--   0        0        0     6771 2023-04-03 14:59:49.705980 orwynn-1.0.0b2/orwynn/_di/init/init_other_acceptors.py
--rw-r--r--   0        0        0     2907 2023-04-03 14:59:49.704980 orwynn-1.0.0b2/orwynn/_di/init/init_other_acceptors_test.py
--rw-r--r--   0        0        0     4157 2023-04-03 14:59:49.702980 orwynn-1.0.0b2/orwynn/_di/init/init_providers.py
--rw-r--r--   0        0        0      628 2023-02-28 05:48:16.657065 orwynn-1.0.0b2/orwynn/_di/init/init_providers_test.py
--rw-r--r--   0        0        0      336 2023-02-27 12:30:57.666822 orwynn-1.0.0b2/orwynn/_di/is_acceptor.py
--rw-r--r--   0        0        0      334 2023-02-27 12:30:57.666822 orwynn-1.0.0b2/orwynn/_di/is_provider.py
--rw-r--r--   0        0        0      836 2023-03-07 08:33:03.935262 orwynn-1.0.0b2/orwynn/_testingtools/__init__.py
--rw-r--r--   0        0        0     1920 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/apiversion/_ApiVersion.py
--rw-r--r--   0        0        0       36 2023-02-23 07:25:38.261308 orwynn-1.0.0b2/orwynn/apiversion/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/apiversion/api_version_test.py
--rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/apiversion/errors.py
--rw-r--r--   0        0        0      401 2023-03-07 07:20:52.198703 orwynn-1.0.0b2/orwynn/app/_ApiRouter.py
--rw-r--r--   0        0        0     1493 2023-03-07 07:21:08.188882 orwynn-1.0.0b2/orwynn/app/_ApiWebsocketRoute.py
--rw-r--r--   0        0        0     1689 2023-04-07 10:07:13.902717 orwynn-1.0.0b2/orwynn/app/_App.py
--rw-r--r--   0        0        0      120 2023-04-07 10:01:45.607493 orwynn-1.0.0b2/orwynn/app/_AppConfig.py
--rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0b2/orwynn/app/_AppMode.py
--rw-r--r--   0        0        0     1561 2023-03-07 07:20:52.199703 orwynn-1.0.0b2/orwynn/app/_CoreApp.py
--rw-r--r--   0        0        0       86 2023-04-07 10:06:55.137728 orwynn-1.0.0b2/orwynn/app/__init__.py
--rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0b2/orwynn/app/_get_dependant.py
--rw-r--r--   0        0        0     2207 2023-04-07 10:05:51.094748 orwynn-1.0.0b2/orwynn/app/app_test.py
--rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0b2/orwynn/apprc/_APP_RC_MODE_NESTING.py
--rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0b2/orwynn/apprc/_AppRc.py
--rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/apprc/_AppRcSearchError.py
--rw-r--r--   0        0        0       64 2023-02-27 06:16:07.584011 orwynn-1.0.0b2/orwynn/apprc/__init__.py
--rw-r--r--   0        0        0     3516 2023-04-07 09:56:47.710126 orwynn-1.0.0b2/orwynn/apprc/_parse_apprc.py
--rw-r--r--   0        0        0     2608 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/apprc/apprc_test.py
--rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0b2/orwynn/base/__init__.py
--rw-r--r--   0        0        0     1116 2023-04-03 14:59:49.383979 orwynn-1.0.0b2/orwynn/base/config/_Config.py
--rw-r--r--   0        0        0       28 2023-02-27 06:19:37.641319 orwynn-1.0.0b2/orwynn/base/config/__init__.py
--rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0b2/orwynn/base/config/config_test.py
--rw-r--r--   0        0        0     2201 2023-04-07 10:26:00.405258 orwynn-1.0.0b2/orwynn/base/controller/_Controller.py
--rw-r--r--   0        0        0       36 2023-02-27 09:39:20.802918 orwynn-1.0.0b2/orwynn/base/controller/__init__.py
--rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0b2/orwynn/base/controller/errors.py
--rw-r--r--   0        0        0      630 2023-02-27 07:44:54.968991 orwynn-1.0.0b2/orwynn/base/database/_Database.py
--rw-r--r--   0        0        0       32 2023-02-27 07:35:06.448928 orwynn-1.0.0b2/orwynn/base/database/__init__.py
--rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0b2/orwynn/base/database/errors.py
--rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0b2/orwynn/base/error/_ErrorValueSchema.py
--rw-r--r--   0        0        0      128 2023-03-06 11:23:49.035894 orwynn-1.0.0b2/orwynn/base/error/_ExceptionAlreadyHandledError.py
--rw-r--r--   0        0        0      157 2023-03-06 11:29:08.008168 orwynn-1.0.0b2/orwynn/base/error/_MalfunctionError.py
--rw-r--r--   0        0        0      403 2023-04-07 09:57:35.357451 orwynn-1.0.0b2/orwynn/base/error/__init__.py
--rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0b2/orwynn/base/error/_errcode.py
--rw-r--r--   0        0        0     1777 2023-02-20 12:03:03.462649 orwynn-1.0.0b2/orwynn/base/error/_find_detailed_class_for_exception.py
--rw-r--r--   0        0        0      227 2023-03-06 11:29:02.964195 orwynn-1.0.0b2/orwynn/base/error/_get_exception_direct_subclasses.py
--rw-r--r--   0        0        0      871 2023-04-07 09:57:35.360451 orwynn-1.0.0b2/orwynn/base/error/errcode_test.py
--rw-r--r--   0        0        0      340 2023-03-06 11:30:55.547595 orwynn-1.0.0b2/orwynn/base/error/error_test.py
--rw-r--r--   0        0        0      465 2023-03-06 11:30:05.054864 orwynn-1.0.0b2/orwynn/base/error/find_detailed_class_test.py
--rw-r--r--   0        0        0     1440 2023-04-03 15:25:55.605775 orwynn-1.0.0b2/orwynn/base/errorhandler/_ErrorHandler.py
--rw-r--r--   0        0        0       40 2023-03-06 12:10:21.521111 orwynn-1.0.0b2/orwynn/base/errorhandler/__init__.py
--rw-r--r--   0        0        0       95 2023-02-27 07:44:23.453495 orwynn-1.0.0b2/orwynn/base/middleware/_GlobalMiddlewareSetup.py
--rw-r--r--   0        0        0     2919 2023-04-03 14:59:49.527979 orwynn-1.0.0b2/orwynn/base/middleware/_Middleware.py
--rw-r--r--   0        0        0       94 2023-02-27 09:39:25.885954 orwynn-1.0.0b2/orwynn/base/middleware/__init__.py
--rw-r--r--   0        0        0     1188 2023-04-03 14:59:49.566980 orwynn-1.0.0b2/orwynn/base/middleware/global_middleware_test.py
--rw-r--r--   0        0        0     1437 2023-04-03 14:59:49.469979 orwynn-1.0.0b2/orwynn/base/model/_Model.py
--rw-r--r--   0        0        0       26 2023-02-27 07:44:01.168434 orwynn-1.0.0b2/orwynn/base/model/__init__.py
--rw-r--r--   0        0        0      805 2023-02-28 05:48:16.658066 orwynn-1.0.0b2/orwynn/base/model/model_test.py
--rw-r--r--   0        0        0     7191 2023-04-03 14:59:49.092978 orwynn-1.0.0b2/orwynn/base/module/_Module.py
--rw-r--r--   0        0        0       28 2023-02-27 08:27:08.818056 orwynn-1.0.0b2/orwynn/base/module/__init__.py
--rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0b2/orwynn/base/module/errors.py
--rw-r--r--   0        0        0      951 2023-04-03 14:59:49.134978 orwynn-1.0.0b2/orwynn/base/module/module_test.py
--rw-r--r--   0        0        0      397 2023-02-27 07:44:37.638169 orwynn-1.0.0b2/orwynn/base/service/_FrameworkService.py
--rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0b2/orwynn/base/service/_Service.py
--rw-r--r--   0        0        0       78 2023-02-28 05:48:16.655065 orwynn-1.0.0b2/orwynn/base/service/__init__.py
--rw-r--r--   0        0        0      213 2023-02-27 08:21:58.741307 orwynn-1.0.0b2/orwynn/base/worker/_Worker.py
--rw-r--r--   0        0        0       28 2023-02-27 08:22:18.356515 orwynn-1.0.0b2/orwynn/base/worker/__init__.py
--rw-r--r--   0        0        0    10692 2023-04-07 09:56:47.709126 orwynn-1.0.0b2/orwynn/boot/_Boot.py
--rw-r--r--   0        0        0      723 2023-02-28 05:48:16.655065 orwynn-1.0.0b2/orwynn/boot/_BootConfig.py
--rw-r--r--   0        0        0       50 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/boot/_UnknownBootModeError.py
--rw-r--r--   0        0        0       49 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/boot/_UnknownSourceError.py
--rw-r--r--   0        0        0       60 2023-02-27 12:41:46.281489 orwynn-1.0.0b2/orwynn/boot/__init__.py
--rw-r--r--   0        0        0     4765 2023-04-07 09:56:47.709126 orwynn-1.0.0b2/orwynn/boot/boot_test.py
--rw-r--r--   0        0        0      232 2023-03-06 14:58:11.414882 orwynn-1.0.0b2/orwynn/bootscript/_Bootscript.py
--rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0b2/orwynn/bootscript/_BootscriptCallable.py
--rw-r--r--   0        0        0     2309 2023-03-07 08:22:34.928871 orwynn-1.0.0b2/orwynn/bootscript/_BootscriptWorker.py
--rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0b2/orwynn/bootscript/_CallTime.py
--rw-r--r--   0        0        0      167 2023-03-06 14:58:11.415882 orwynn-1.0.0b2/orwynn/bootscript/__init__.py
--rw-r--r--   0        0        0      863 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/bootscript/bootscript_test.py
--rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0b2/orwynn/bootscript/errors.py
--rw-r--r--   0        0        0     2657 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/context/_ContextStorage.py
--rw-r--r--   0        0        0       90 2023-02-27 06:44:46.522437 orwynn-1.0.0b2/orwynn/context/__init__.py
--rw-r--r--   0        0        0      651 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/context/_context_manager.py
--rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/context/errors.py
--rw-r--r--   0        0        0      683 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/helpers/SUBCLASSABLES.py
--rw-r--r--   0        0        0     1140 2023-04-03 15:28:01.351294 orwynn-1.0.0b2/orwynn/helpers/web.py
--rw-r--r--   0        0        0      581 2023-03-06 12:13:17.936738 orwynn-1.0.0b2/orwynn/http/_BUILTIN_HTTP_MIDDLEWARE.py
--rw-r--r--   0        0        0      392 2023-03-06 12:14:21.405584 orwynn-1.0.0b2/orwynn/http/_DEFAULT_HTTP_ERROR_HANDLERS.py
--rw-r--r--   0        0        0     1240 2023-04-03 15:28:09.845148 orwynn-1.0.0b2/orwynn/http/__init__.py
--rw-r--r--   0        0        0      638 2023-02-27 13:18:48.601279 orwynn-1.0.0b2/orwynn/http/_context/ContextBuiltinMiddleware.py
--rw-r--r--   0        0        0      785 2023-02-27 13:17:45.453970 orwynn-1.0.0b2/orwynn/http/_context/HttpRequestContextBuiltinMiddleware.py
--rw-r--r--   0        0        0      959 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_context/HttpRequestContextId.py
--rw-r--r--   0        0        0      986 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_context/context_test.py
--rw-r--r--   0        0        0     5455 2023-04-03 15:31:36.939282 orwynn-1.0.0b2/orwynn/http/_controller/HttpController.py
--rw-r--r--   0        0        0     1239 2023-02-28 05:48:16.650064 orwynn-1.0.0b2/orwynn/http/_controller/endpoint/Endpoint.py
--rw-r--r--   0        0        0     1130 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_controller/endpoint/EndpointContainer.py
--rw-r--r--   0        0        0      218 2023-02-28 05:48:16.650064 orwynn-1.0.0b2/orwynn/http/_controller/endpoint/EndpointResponse.py
--rw-r--r--   0        0        0     2234 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_controller/endpoint/endpoint_test.py
--rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/http/_controller/errors.py
--rw-r--r--   0        0        0     6607 2023-04-03 15:40:19.722821 orwynn-1.0.0b2/orwynn/http/_controller/http_controller_test.py
--rw-r--r--   0        0        0      408 2023-02-27 07:44:23.427494 orwynn-1.0.0b2/orwynn/http/_cors/Cors.py
--rw-r--r--   0        0        0     1926 2023-02-28 05:48:16.656065 orwynn-1.0.0b2/orwynn/http/_cors/cors_test.py
--rw-r--r--   0        0        0     1107 2023-04-03 14:59:49.731980 orwynn-1.0.0b2/orwynn/http/_errorhandler/ErrorHandlerHttpMiddleware.py
--rw-r--r--   0        0        0     1211 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_errorhandler/default.py
--rw-r--r--   0        0        0     6159 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_errorhandler/error_handler_test.py
--rw-r--r--   0        0        0     4230 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/http/_log/HttpLogger.py
--rw-r--r--   0        0        0     1181 2023-02-28 05:54:49.627064 orwynn-1.0.0b2/orwynn/http/_log/LogMiddleware.py
--rw-r--r--   0        0        0      279 2023-02-27 12:24:09.544983 orwynn-1.0.0b2/orwynn/http/_middleware/BuiltinHttpMiddleware.py
--rw-r--r--   0        0        0      659 2023-02-28 05:48:16.646063 orwynn-1.0.0b2/orwynn/http/_middleware/HttpMiddleware.py
--rw-r--r--   0        0        0      329 2023-02-27 12:23:41.962432 orwynn-1.0.0b2/orwynn/http/_middleware/HttpNextCall.py
--rw-r--r--   0        0        0     2153 2023-02-28 05:48:16.654065 orwynn-1.0.0b2/orwynn/http/_middleware/http_middleware_test.py
--rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0b2/orwynn/http/_requests.py
--rw-r--r--   0        0        0      341 2023-02-21 09:58:36.577957 orwynn-1.0.0b2/orwynn/http/_responses.py
--rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0b2/orwynn/http/_schema/HttpExceptionValueSchema.py
--rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0b2/orwynn/http/_schema/RequestValidationExceptionValueSchema.py
--rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0b2/orwynn/http/errors.py
--rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0b2/orwynn/http/http_test.py
--rw-r--r--   0        0        0      187 2023-03-06 11:37:56.740371 orwynn-1.0.0b2/orwynn/indication/_Indicatable.py
--rw-r--r--   0        0        0    11525 2023-04-07 09:54:13.815708 orwynn-1.0.0b2/orwynn/indication/_Indication.py
--rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0b2/orwynn/indication/_IndicationType.py
--rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0b2/orwynn/indication/_Indicator.py
--rw-r--r--   0        0        0      174 2023-02-28 05:48:16.652064 orwynn-1.0.0b2/orwynn/indication/__init__.py
--rw-r--r--   0        0        0      233 2023-02-27 08:17:22.419985 orwynn-1.0.0b2/orwynn/indication/_default_api_indication.py
--rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/indication/errors.py
--rw-r--r--   0        0        0     2949 2023-04-07 08:57:48.011580 orwynn-1.0.0b2/orwynn/indication/indication_test.py
--rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0b2/orwynn/log/_LOG_EXTRA_RESERVED_FIELDS.py
--rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0b2/orwynn/log/_Log.py
--rw-r--r--   0        0        0      156 2023-02-27 09:57:55.608936 orwynn-1.0.0b2/orwynn/log/_LogConfig.py
--rw-r--r--   0        0        0      746 2023-02-27 07:44:23.427494 orwynn-1.0.0b2/orwynn/log/_LogHandler.py
--rw-r--r--   0        0        0      134 2023-02-27 08:12:14.243641 orwynn-1.0.0b2/orwynn/log/__init__.py
--rw-r--r--   0        0        0     1984 2023-02-27 12:51:28.284483 orwynn-1.0.0b2/orwynn/log/_configure_log.py
--rw-r--r--   0        0        0      423 2023-02-27 08:11:29.510555 orwynn-1.0.0b2/orwynn/log/_reraise_catch.py
--rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/log/errors.py
--rw-r--r--   0        0        0     3640 2023-03-06 12:04:13.972055 orwynn-1.0.0b2/orwynn/log/log_middleware_test.py
--rw-r--r--   0        0        0     1731 2023-02-28 05:48:16.662067 orwynn-1.0.0b2/orwynn/log/log_test.py
--rw-r--r--   0        0        0     1460 2023-02-28 05:48:16.662067 orwynn-1.0.0b2/orwynn/log/log_websocket_middleware_test.py
--rw-r--r--   0        0        0     1560 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/mapping/_Mapping.py
--rw-r--r--   0        0        0       30 2023-02-27 08:33:14.996815 orwynn-1.0.0b2/orwynn/mapping/__init__.py
--rw-r--r--   0        0        0      281 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/mapping/errors.py
--rw-r--r--   0        0        0      179 2023-02-27 08:32:55.043879 orwynn-1.0.0b2/orwynn/mapping/mapping_test.py
--rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0b2/orwynn/mongo/_ClientSession.py
--rw-r--r--   0        0        0     6048 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/mongo/_Document.py
--rw-r--r--   0        0        0     3579 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/mongo/_Mongo.py
--rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0b2/orwynn/mongo/_MongoConfig.py
--rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0b2/orwynn/mongo/_MongoEntity.py
--rw-r--r--   0        0        0      224 2023-02-28 05:48:16.650064 orwynn-1.0.0b2/orwynn/mongo/__init__.py
--rw-r--r--   0        0        0     3300 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/mongo/document_test.py
--rw-r--r--   0        0        0      445 2023-03-06 11:30:55.548595 orwynn-1.0.0b2/orwynn/mongo/errors.py
--rw-r--r--   0        0        0     1361 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/mongo/mongo_test.py
--rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0b2/orwynn/proxy/ApiIndicationOnlyProxy.py
--rw-r--r--   0        0        0     2763 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/proxy/BootProxy.py
--rw-r--r--   0        0        0    14623 2023-04-07 10:15:34.683787 orwynn-1.0.0b2/orwynn/router/_ControllerRegister.py
--rw-r--r--   0        0        0     3952 2023-04-03 14:59:49.711980 orwynn-1.0.0b2/orwynn/router/_ErrorHandlerManager.py
--rw-r--r--   0        0        0    10300 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/router/_MiddlewareRegister.py
--rw-r--r--   0        0        0     2697 2023-03-07 08:22:34.931871 orwynn-1.0.0b2/orwynn/router/_Router.py
--rw-r--r--   0        0        0       28 2023-02-27 13:24:49.469241 orwynn-1.0.0b2/orwynn/router/__init__.py
--rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/router/errors.py
--rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0b2/orwynn/router/global_http_route_test.py
--rw-r--r--   0        0        0     1306 2023-01-10 10:10:51.782079 orwynn-1.0.0b2/orwynn/singleton/_Singleton.py
--rw-r--r--   0        0        0       34 2023-02-27 08:21:14.680585 orwynn-1.0.0b2/orwynn/singleton/__init__.py
--rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0b2/orwynn/sql/_PoolclassStr.py
--rw-r--r--   0        0        0     3628 2023-04-03 14:59:49.742980 orwynn-1.0.0b2/orwynn/sql/_Sql.py
--rw-r--r--   0        0        0     1939 2023-02-28 06:53:42.496498 orwynn-1.0.0b2/orwynn/sql/_SqlConfig.py
--rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0b2/orwynn/sql/_SqlDatabaseKind.py
--rw-r--r--   0        0        0     2648 2023-04-03 14:59:49.734980 orwynn-1.0.0b2/orwynn/sql/_Table.py
--rw-r--r--   0        0        0      210 2023-02-28 05:15:28.490194 orwynn-1.0.0b2/orwynn/sql/__init__.py
--rw-r--r--   0        0        0     5865 2023-04-03 14:59:49.751980 orwynn-1.0.0b2/orwynn/sql/sql_test.py
--rw-r--r--   0        0        0    11258 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/testing/_Client.py
--rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0b2/orwynn/testing/_EmbeddedTestClient.py
--rw-r--r--   0        0        0      727 2023-02-28 05:48:16.655065 orwynn-1.0.0b2/orwynn/testing/__init__.py
--rw-r--r--   0        0        0     2057 2023-03-07 08:43:05.624039 orwynn-1.0.0b2/orwynn/testing/client_test.py
--rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0b2/orwynn/utils/BaseSubclassable.py
--rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0b2/orwynn/utils/Protocol.py
--rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/crypto/__init__.py
--rw-r--r--   0        0        0      448 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/dt/__init__.py
--rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0b2/orwynn/utils/fmt/__init__.py
--rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/fmt/fmt_test.py
--rw-r--r--   0        0        0     1974 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/klass/__init__.py
--rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0b2/orwynn/utils/klass/_errors.py
--rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0b2/orwynn/utils/klass/klass_test.py
--rw-r--r--   0        0        0     2545 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/mp/__init__.py
--rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0b2/orwynn/utils/mp/_dictpp.py
--rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0b2/orwynn/utils/mp/location.py
--rw-r--r--   0        0        0     1738 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/mp/mp_test.py
--rw-r--r--   0        0        0      131 2023-02-21 10:53:24.615257 orwynn-1.0.0b2/orwynn/utils/rnd/__init__.py
--rw-r--r--   0        0        0       90 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/rnd/rnd_test.py
--rw-r--r--   0        0        0      176 2023-02-17 07:26:21.447070 orwynn-1.0.0b2/orwynn/utils/types.py
--rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0b2/orwynn/utils/uio.py
--rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0b2/orwynn/utils/url/_Url.py
--rw-r--r--   0        0        0      254 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/url/_UrlVars.py
--rw-r--r--   0        0        0      697 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/url/__init__.py
--rw-r--r--   0        0        0     1934 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/url/_get_vars.py
--rw-r--r--   0        0        0      419 2023-03-06 13:33:43.023337 orwynn-1.0.0b2/orwynn/utils/url/_match_routes.py
--rw-r--r--   0        0        0     1412 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/url/get_vars_test.py
--rw-r--r--   0        0        0     9151 2023-04-03 15:00:11.231062 orwynn-1.0.0b2/orwynn/utils/validation/__init__.py
--rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0b2/orwynn/utils/validation/_validator.py
--rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0b2/orwynn/utils/validation/errors.py
--rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0b2/orwynn/utils/yml/__init__.py
--rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0b2/orwynn/utils/yml/errors.py
--rw-r--r--   0        0        0      864 2023-03-06 12:13:17.936738 orwynn-1.0.0b2/orwynn/websocket/_BUILTIN_WEBSOCKET_MIDDLEWARE.py
--rw-r--r--   0        0        0      248 2023-03-06 12:13:17.936738 orwynn-1.0.0b2/orwynn/websocket/_DEFAULT_WEBSOCKET_ERROR_HANDLERS.py
--rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0b2/orwynn/websocket/_Websocket.py
--rw-r--r--   0        0        0      836 2023-03-06 12:13:17.936738 orwynn-1.0.0b2/orwynn/websocket/__init__.py
--rw-r--r--   0        0        0      579 2023-02-28 05:55:07.500801 orwynn-1.0.0b2/orwynn/websocket/_context/ContextBuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0      824 2023-02-28 05:48:16.654065 orwynn-1.0.0b2/orwynn/websocket/_context/RequestContextBuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0     1028 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_context/WebsocketRequestContextId.py
--rw-r--r--   0        0        0     1291 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_context/websocket_context_test.py
--rw-r--r--   0        0        0     3977 2023-04-07 10:11:54.671319 orwynn-1.0.0b2/orwynn/websocket/_controller/WebsocketController.py
--rw-r--r--   0        0        0      902 2023-04-07 10:21:27.442702 orwynn-1.0.0b2/orwynn/websocket/_controller/WebsocketController_test.py
--rw-r--r--   0        0        0      147 2023-02-27 07:44:23.427494 orwynn-1.0.0b2/orwynn/websocket/_controller/WebsocketEventHandlerMethod.py
--rw-r--r--   0        0        0     2900 2023-02-28 05:48:16.658066 orwynn-1.0.0b2/orwynn/websocket/_controller/global_websocket_route_test.py
--rw-r--r--   0        0        0     3026 2023-03-06 13:33:04.085558 orwynn-1.0.0b2/orwynn/websocket/_controller/websocket_controller_test.py
--rw-r--r--   0        0        0      417 2023-03-06 12:12:57.645660 orwynn-1.0.0b2/orwynn/websocket/_errorhandler/DefaultWebsocketErrorHandler.py
--rw-r--r--   0        0        0     3620 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_errorhandler/ErrorHandlerWebsocketMiddleware.py
--rw-r--r--   0        0        0     1707 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_errorhandler/error_handler_websocket_test.py
--rw-r--r--   0        0        0      920 2023-02-28 05:48:16.653065 orwynn-1.0.0b2/orwynn/websocket/_log/LogWebsocketMiddleware.py
--rw-r--r--   0        0        0     1708 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_log/WebsocketLogger.py
--rw-r--r--   0        0        0      313 2023-02-28 05:48:16.648064 orwynn-1.0.0b2/orwynn/websocket/_middleware/BuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0      887 2023-02-28 05:48:16.653065 orwynn-1.0.0b2/orwynn/websocket/_middleware/ConnectionBuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0      748 2023-02-28 05:48:16.653065 orwynn-1.0.0b2/orwynn/websocket/_middleware/WebsocketMiddleware.py
--rw-r--r--   0        0        0      280 2023-02-27 13:14:10.637743 orwynn-1.0.0b2/orwynn/websocket/_middleware/WebsocketNextCall.py
--rw-r--r--   0        0        0     1056 2023-02-28 05:48:16.647063 orwynn-1.0.0b2/orwynn/websocket/_middleware/websocket_middleware_test.py
--rw-r--r--   0        0        0     1893 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_routing/NextCallHandler.py
--rw-r--r--   0        0        0     6084 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_routing/WebsocketStack.py
--rw-r--r--   0        0        0      231 2023-02-28 05:55:25.292122 orwynn-1.0.0b2/orwynn/websocket/_routing/_DispatchWebsocketFn.py
--rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0b2/orwynn/websocket/_routing/_GenericWebsocketFn.py
--rw-r--r--   0        0        0     5547 2023-04-03 14:59:49.717980 orwynn-1.0.0b2/orwynn/websocket/_routing/_get_handler_kwargs.py
--rw-r--r--   0        0        0      448 2023-02-28 05:48:16.646063 orwynn-1.0.0b2/orwynn/websocket/_routing/handlers.py
--rw-r--r--   0        0        0      823 2023-04-07 10:28:15.566495 orwynn-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 orwynn-1.0.0b2/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 orwynn-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0        8 2022-12-09 11:58:05.154110 orwynn-1.0.0b3/README.md
+-rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0b3/orwynn/__init__.py
+-rw-r--r--   0        0        0       63 2022-12-11 09:09:39.933971 orwynn-1.0.0b3/orwynn/_di/Acceptor.py
+-rw-r--r--   0        0        0      500 2023-03-06 12:12:57.645660 orwynn-1.0.0b3/orwynn/_di/BUILTIN_ACCEPTORS.py
+-rw-r--r--   0        0        0      399 2023-02-28 05:48:16.657065 orwynn-1.0.0b3/orwynn/_di/BUILTIN_PROVIDERS.py
+-rw-r--r--   0        0        0     4726 2023-04-03 14:59:49.701980 orwynn-1.0.0b3/orwynn/_di/Di.py
+-rw-r--r--   0        0        0     6038 2023-04-03 14:59:49.636980 orwynn-1.0.0b3/orwynn/_di/DiContainer.py
+-rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0b3/orwynn/_di/DiObject.py
+-rw-r--r--   0        0        0      119 2023-03-06 11:23:49.043895 orwynn-1.0.0b3/orwynn/_di/DiObjectAlreadyInitializedInContainerError.py
+-rw-r--r--   0        0        0      132 2023-03-06 11:23:49.043895 orwynn-1.0.0b3/orwynn/_di/FinalizedDiContainerError.py
+-rw-r--r--   0        0        0       51 2023-03-06 11:23:49.043895 orwynn-1.0.0b3/orwynn/_di/MissingDiObjectError.py
+-rw-r--r--   0        0        0       96 2023-03-06 11:23:49.043895 orwynn-1.0.0b3/orwynn/_di/NoAnnotationError.py
+-rw-r--r--   0        0        0      291 2023-03-06 11:23:49.043895 orwynn-1.0.0b3/orwynn/_di/NotProviderError.py
+-rw-r--r--   0        0        0       39 2022-12-11 09:09:05.931124 orwynn-1.0.0b3/orwynn/_di/Provider.py
+-rw-r--r--   0        0        0      579 2023-03-06 11:30:55.552595 orwynn-1.0.0b3/orwynn/_di/ProviderAvailabilityError.py
+-rw-r--r--   0        0        0      101 2023-03-06 14:58:11.412882 orwynn-1.0.0b3/orwynn/_di/__init__.py
+-rw-r--r--   0        0        0     1733 2023-03-06 14:58:30.471950 orwynn-1.0.0b3/orwynn/_di/_collect_dependencies_for_acceptor.py
+-rw-r--r--   0        0        0     3856 2023-02-28 05:48:16.658066 orwynn-1.0.0b3/orwynn/_di/check_availability.py
+-rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0b3/orwynn/_di/collecting/ModuleCollector.py
+-rw-r--r--   0        0        0      459 2023-03-06 11:30:55.551595 orwynn-1.0.0b3/orwynn/_di/collecting/ProviderAlreadyInitializedForMapError.py
+-rw-r--r--   0        0        0     1086 2023-04-03 14:59:49.701980 orwynn-1.0.0b3/orwynn/_di/collecting/collect_modules_test.py
+-rw-r--r--   0        0        0     3305 2023-04-03 14:59:49.702980 orwynn-1.0.0b3/orwynn/_di/collecting/collect_provider_dependencies.py
+-rw-r--r--   0        0        0     1709 2023-02-28 06:25:30.262229 orwynn-1.0.0b3/orwynn/_di/collecting/collect_provider_dependencies_test.py
+-rw-r--r--   0        0        0     3210 2023-02-28 05:48:16.648064 orwynn-1.0.0b3/orwynn/_di/collecting/get_parameters_for_provider.py
+-rw-r--r--   0        0        0      324 2023-03-06 11:30:55.551595 orwynn-1.0.0b3/orwynn/_di/collecting/no_dependencies_for_given_provider_error.py
+-rw-r--r--   0        0        0     2523 2023-02-27 12:30:57.696823 orwynn-1.0.0b3/orwynn/_di/collecting/provider_dependencies_map.py
+-rw-r--r--   0        0        0      138 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/_di/collecting/provider_keyword_attribute_error.py
+-rw-r--r--   0        0        0      376 2023-03-06 11:30:55.550595 orwynn-1.0.0b3/orwynn/_di/collecting/provider_not_found_in_map_error.py
+-rw-r--r--   0        0        0      519 2023-02-28 05:48:16.651064 orwynn-1.0.0b3/orwynn/_di/di_test.py
+-rw-r--r--   0        0        0     6771 2023-04-03 14:59:49.705980 orwynn-1.0.0b3/orwynn/_di/init/init_other_acceptors.py
+-rw-r--r--   0        0        0     2907 2023-04-03 14:59:49.704980 orwynn-1.0.0b3/orwynn/_di/init/init_other_acceptors_test.py
+-rw-r--r--   0        0        0     4157 2023-04-03 14:59:49.702980 orwynn-1.0.0b3/orwynn/_di/init/init_providers.py
+-rw-r--r--   0        0        0      628 2023-02-28 05:48:16.657065 orwynn-1.0.0b3/orwynn/_di/init/init_providers_test.py
+-rw-r--r--   0        0        0      336 2023-02-27 12:30:57.666822 orwynn-1.0.0b3/orwynn/_di/is_acceptor.py
+-rw-r--r--   0        0        0      334 2023-02-27 12:30:57.666822 orwynn-1.0.0b3/orwynn/_di/is_provider.py
+-rw-r--r--   0        0        0      836 2023-03-07 08:33:03.935262 orwynn-1.0.0b3/orwynn/_testingtools/__init__.py
+-rw-r--r--   0        0        0     1920 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/apiversion/_ApiVersion.py
+-rw-r--r--   0        0        0       36 2023-02-23 07:25:38.261308 orwynn-1.0.0b3/orwynn/apiversion/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/apiversion/api_version_test.py
+-rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/apiversion/errors.py
+-rw-r--r--   0        0        0      401 2023-03-07 07:20:52.198703 orwynn-1.0.0b3/orwynn/app/_ApiRouter.py
+-rw-r--r--   0        0        0     1493 2023-03-07 07:21:08.188882 orwynn-1.0.0b3/orwynn/app/_ApiWebsocketRoute.py
+-rw-r--r--   0        0        0     1689 2023-04-07 10:07:13.902717 orwynn-1.0.0b3/orwynn/app/_App.py
+-rw-r--r--   0        0        0      120 2023-04-07 10:01:45.607493 orwynn-1.0.0b3/orwynn/app/_AppConfig.py
+-rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0b3/orwynn/app/_AppMode.py
+-rw-r--r--   0        0        0     1561 2023-03-07 07:20:52.199703 orwynn-1.0.0b3/orwynn/app/_CoreApp.py
+-rw-r--r--   0        0        0       86 2023-04-07 10:06:55.137728 orwynn-1.0.0b3/orwynn/app/__init__.py
+-rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0b3/orwynn/app/_get_dependant.py
+-rw-r--r--   0        0        0     2207 2023-04-07 10:05:51.094748 orwynn-1.0.0b3/orwynn/app/app_test.py
+-rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0b3/orwynn/apprc/_APP_RC_MODE_NESTING.py
+-rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0b3/orwynn/apprc/_AppRc.py
+-rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/apprc/_AppRcSearchError.py
+-rw-r--r--   0        0        0       64 2023-02-27 06:16:07.584011 orwynn-1.0.0b3/orwynn/apprc/__init__.py
+-rw-r--r--   0        0        0     3516 2023-04-07 09:56:47.710126 orwynn-1.0.0b3/orwynn/apprc/_parse_apprc.py
+-rw-r--r--   0        0        0     2608 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/apprc/apprc_test.py
+-rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0b3/orwynn/base/__init__.py
+-rw-r--r--   0        0        0     1116 2023-04-03 14:59:49.383979 orwynn-1.0.0b3/orwynn/base/config/_Config.py
+-rw-r--r--   0        0        0       28 2023-02-27 06:19:37.641319 orwynn-1.0.0b3/orwynn/base/config/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0b3/orwynn/base/config/config_test.py
+-rw-r--r--   0        0        0     2201 2023-04-07 10:26:00.405258 orwynn-1.0.0b3/orwynn/base/controller/_Controller.py
+-rw-r--r--   0        0        0       36 2023-02-27 09:39:20.802918 orwynn-1.0.0b3/orwynn/base/controller/__init__.py
+-rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0b3/orwynn/base/controller/errors.py
+-rw-r--r--   0        0        0      630 2023-02-27 07:44:54.968991 orwynn-1.0.0b3/orwynn/base/database/_Database.py
+-rw-r--r--   0        0        0       32 2023-02-27 07:35:06.448928 orwynn-1.0.0b3/orwynn/base/database/__init__.py
+-rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0b3/orwynn/base/database/errors.py
+-rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0b3/orwynn/base/error/_ErrorValueSchema.py
+-rw-r--r--   0        0        0      128 2023-03-06 11:23:49.035894 orwynn-1.0.0b3/orwynn/base/error/_ExceptionAlreadyHandledError.py
+-rw-r--r--   0        0        0      157 2023-03-06 11:29:08.008168 orwynn-1.0.0b3/orwynn/base/error/_MalfunctionError.py
+-rw-r--r--   0        0        0      403 2023-04-07 09:57:35.357451 orwynn-1.0.0b3/orwynn/base/error/__init__.py
+-rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0b3/orwynn/base/error/_errcode.py
+-rw-r--r--   0        0        0     1777 2023-02-20 12:03:03.462649 orwynn-1.0.0b3/orwynn/base/error/_find_detailed_class_for_exception.py
+-rw-r--r--   0        0        0      227 2023-03-06 11:29:02.964195 orwynn-1.0.0b3/orwynn/base/error/_get_exception_direct_subclasses.py
+-rw-r--r--   0        0        0      871 2023-04-07 09:57:35.360451 orwynn-1.0.0b3/orwynn/base/error/errcode_test.py
+-rw-r--r--   0        0        0      340 2023-03-06 11:30:55.547595 orwynn-1.0.0b3/orwynn/base/error/error_test.py
+-rw-r--r--   0        0        0      465 2023-03-06 11:30:05.054864 orwynn-1.0.0b3/orwynn/base/error/find_detailed_class_test.py
+-rw-r--r--   0        0        0     1440 2023-04-03 15:25:55.605775 orwynn-1.0.0b3/orwynn/base/errorhandler/_ErrorHandler.py
+-rw-r--r--   0        0        0       40 2023-03-06 12:10:21.521111 orwynn-1.0.0b3/orwynn/base/errorhandler/__init__.py
+-rw-r--r--   0        0        0       95 2023-02-27 07:44:23.453495 orwynn-1.0.0b3/orwynn/base/middleware/_GlobalMiddlewareSetup.py
+-rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0b3/orwynn/base/middleware/_Middleware.py
+-rw-r--r--   0        0        0       94 2023-02-27 09:39:25.885954 orwynn-1.0.0b3/orwynn/base/middleware/__init__.py
+-rw-r--r--   0        0        0     1188 2023-04-03 14:59:49.566980 orwynn-1.0.0b3/orwynn/base/middleware/global_middleware_test.py
+-rw-r--r--   0        0        0     1437 2023-04-03 14:59:49.469979 orwynn-1.0.0b3/orwynn/base/model/_Model.py
+-rw-r--r--   0        0        0       26 2023-02-27 07:44:01.168434 orwynn-1.0.0b3/orwynn/base/model/__init__.py
+-rw-r--r--   0        0        0      805 2023-02-28 05:48:16.658066 orwynn-1.0.0b3/orwynn/base/model/model_test.py
+-rw-r--r--   0        0        0     7191 2023-04-03 14:59:49.092978 orwynn-1.0.0b3/orwynn/base/module/_Module.py
+-rw-r--r--   0        0        0       28 2023-02-27 08:27:08.818056 orwynn-1.0.0b3/orwynn/base/module/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0b3/orwynn/base/module/errors.py
+-rw-r--r--   0        0        0      951 2023-04-03 14:59:49.134978 orwynn-1.0.0b3/orwynn/base/module/module_test.py
+-rw-r--r--   0        0        0      397 2023-02-27 07:44:37.638169 orwynn-1.0.0b3/orwynn/base/service/_FrameworkService.py
+-rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0b3/orwynn/base/service/_Service.py
+-rw-r--r--   0        0        0       78 2023-02-28 05:48:16.655065 orwynn-1.0.0b3/orwynn/base/service/__init__.py
+-rw-r--r--   0        0        0      213 2023-02-27 08:21:58.741307 orwynn-1.0.0b3/orwynn/base/worker/_Worker.py
+-rw-r--r--   0        0        0       28 2023-02-27 08:22:18.356515 orwynn-1.0.0b3/orwynn/base/worker/__init__.py
+-rw-r--r--   0        0        0    10692 2023-04-07 09:56:47.709126 orwynn-1.0.0b3/orwynn/boot/_Boot.py
+-rw-r--r--   0        0        0      723 2023-02-28 05:48:16.655065 orwynn-1.0.0b3/orwynn/boot/_BootConfig.py
+-rw-r--r--   0        0        0       50 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/boot/_UnknownBootModeError.py
+-rw-r--r--   0        0        0       49 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/boot/_UnknownSourceError.py
+-rw-r--r--   0        0        0       60 2023-02-27 12:41:46.281489 orwynn-1.0.0b3/orwynn/boot/__init__.py
+-rw-r--r--   0        0        0     4765 2023-04-07 09:56:47.709126 orwynn-1.0.0b3/orwynn/boot/boot_test.py
+-rw-r--r--   0        0        0      232 2023-03-06 14:58:11.414882 orwynn-1.0.0b3/orwynn/bootscript/_Bootscript.py
+-rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0b3/orwynn/bootscript/_BootscriptCallable.py
+-rw-r--r--   0        0        0     2309 2023-03-07 08:22:34.928871 orwynn-1.0.0b3/orwynn/bootscript/_BootscriptWorker.py
+-rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0b3/orwynn/bootscript/_CallTime.py
+-rw-r--r--   0        0        0      167 2023-03-06 14:58:11.415882 orwynn-1.0.0b3/orwynn/bootscript/__init__.py
+-rw-r--r--   0        0        0      863 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/bootscript/bootscript_test.py
+-rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0b3/orwynn/bootscript/errors.py
+-rw-r--r--   0        0        0     2657 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/context/_ContextStorage.py
+-rw-r--r--   0        0        0       90 2023-02-27 06:44:46.522437 orwynn-1.0.0b3/orwynn/context/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/context/_context_manager.py
+-rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/context/errors.py
+-rw-r--r--   0        0        0      683 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/helpers/SUBCLASSABLES.py
+-rw-r--r--   0        0        0     1140 2023-04-03 15:28:01.351294 orwynn-1.0.0b3/orwynn/helpers/web.py
+-rw-r--r--   0        0        0      581 2023-03-06 12:13:17.936738 orwynn-1.0.0b3/orwynn/http/_BUILTIN_HTTP_MIDDLEWARE.py
+-rw-r--r--   0        0        0      392 2023-05-15 09:41:13.740171 orwynn-1.0.0b3/orwynn/http/_DEFAULT_HTTP_ERROR_HANDLERS.py
+-rw-r--r--   0        0        0     1262 2023-05-15 09:53:21.175789 orwynn-1.0.0b3/orwynn/http/__init__.py
+-rw-r--r--   0        0        0      638 2023-02-27 13:18:48.601279 orwynn-1.0.0b3/orwynn/http/_context/ContextBuiltinMiddleware.py
+-rw-r--r--   0        0        0      785 2023-04-21 10:02:27.264870 orwynn-1.0.0b3/orwynn/http/_context/HttpRequestContextBuiltinMiddleware.py
+-rw-r--r--   0        0        0      959 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/http/_context/HttpRequestContextId.py
+-rw-r--r--   0        0        0      986 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/http/_context/context_test.py
+-rw-r--r--   0        0        0     5455 2023-04-03 15:31:36.939282 orwynn-1.0.0b3/orwynn/http/_controller/HttpController.py
+-rw-r--r--   0        0        0     1239 2023-02-28 05:48:16.650064 orwynn-1.0.0b3/orwynn/http/_controller/endpoint/Endpoint.py
+-rw-r--r--   0        0        0     1130 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/http/_controller/endpoint/EndpointContainer.py
+-rw-r--r--   0        0        0      217 2023-05-15 09:51:42.051574 orwynn-1.0.0b3/orwynn/http/_controller/endpoint/EndpointResponse.py
+-rw-r--r--   0        0        0     2234 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/http/_controller/endpoint/endpoint_test.py
+-rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/http/_controller/errors.py
+-rw-r--r--   0        0        0     7269 2023-04-21 10:06:19.025210 orwynn-1.0.0b3/orwynn/http/_controller/http_controller_test.py
+-rw-r--r--   0        0        0      408 2023-02-27 07:44:23.427494 orwynn-1.0.0b3/orwynn/http/_cors/Cors.py
+-rw-r--r--   0        0        0     1926 2023-02-28 05:48:16.656065 orwynn-1.0.0b3/orwynn/http/_cors/cors_test.py
+-rw-r--r--   0        0        0     1107 2023-04-21 09:55:44.471980 orwynn-1.0.0b3/orwynn/http/_errorhandler/ErrorHandlerHttpMiddleware.py
+-rw-r--r--   0        0        0     1211 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/http/_errorhandler/default.py
+-rw-r--r--   0        0        0     6159 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/http/_errorhandler/error_handler_test.py
+-rw-r--r--   0        0        0     4513 2023-05-15 09:28:21.232649 orwynn-1.0.0b3/orwynn/http/_log/HttpLogger.py
+-rw-r--r--   0        0        0     1181 2023-02-28 05:54:49.627064 orwynn-1.0.0b3/orwynn/http/_log/LogMiddleware.py
+-rw-r--r--   0        0        0      279 2023-02-27 12:24:09.544983 orwynn-1.0.0b3/orwynn/http/_middleware/BuiltinHttpMiddleware.py
+-rw-r--r--   0        0        0      659 2023-04-21 09:58:22.708552 orwynn-1.0.0b3/orwynn/http/_middleware/HttpMiddleware.py
+-rw-r--r--   0        0        0      329 2023-02-27 12:23:41.962432 orwynn-1.0.0b3/orwynn/http/_middleware/HttpNextCall.py
+-rw-r--r--   0        0        0     2153 2023-02-28 05:48:16.654065 orwynn-1.0.0b3/orwynn/http/_middleware/http_middleware_test.py
+-rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0b3/orwynn/http/_requests.py
+-rw-r--r--   0        0        0      448 2023-05-15 09:53:21.181789 orwynn-1.0.0b3/orwynn/http/_responses.py
+-rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0b3/orwynn/http/_schema/HttpExceptionValueSchema.py
+-rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0b3/orwynn/http/_schema/RequestValidationExceptionValueSchema.py
+-rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0b3/orwynn/http/errors.py
+-rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0b3/orwynn/http/http_test.py
+-rw-r--r--   0        0        0      187 2023-03-06 11:37:56.740371 orwynn-1.0.0b3/orwynn/indication/_Indicatable.py
+-rw-r--r--   0        0        0    11582 2023-05-15 09:44:55.514487 orwynn-1.0.0b3/orwynn/indication/_Indication.py
+-rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0b3/orwynn/indication/_IndicationType.py
+-rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0b3/orwynn/indication/_Indicator.py
+-rw-r--r--   0        0        0      174 2023-02-28 05:48:16.652064 orwynn-1.0.0b3/orwynn/indication/__init__.py
+-rw-r--r--   0        0        0      233 2023-02-27 08:17:22.419985 orwynn-1.0.0b3/orwynn/indication/_default_api_indication.py
+-rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/indication/errors.py
+-rw-r--r--   0        0        0     3449 2023-05-15 09:48:05.804030 orwynn-1.0.0b3/orwynn/indication/indication_test.py
+-rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0b3/orwynn/log/_LOG_EXTRA_RESERVED_FIELDS.py
+-rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0b3/orwynn/log/_Log.py
+-rw-r--r--   0        0        0      156 2023-02-27 09:57:55.608936 orwynn-1.0.0b3/orwynn/log/_LogConfig.py
+-rw-r--r--   0        0        0      746 2023-02-27 07:44:23.427494 orwynn-1.0.0b3/orwynn/log/_LogHandler.py
+-rw-r--r--   0        0        0      134 2023-02-27 08:12:14.243641 orwynn-1.0.0b3/orwynn/log/__init__.py
+-rw-r--r--   0        0        0     1984 2023-02-27 12:51:28.284483 orwynn-1.0.0b3/orwynn/log/_configure_log.py
+-rw-r--r--   0        0        0      423 2023-02-27 08:11:29.510555 orwynn-1.0.0b3/orwynn/log/_reraise_catch.py
+-rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/log/errors.py
+-rw-r--r--   0        0        0     3640 2023-03-06 12:04:13.972055 orwynn-1.0.0b3/orwynn/log/log_middleware_test.py
+-rw-r--r--   0        0        0     1731 2023-02-28 05:48:16.662067 orwynn-1.0.0b3/orwynn/log/log_test.py
+-rw-r--r--   0        0        0     1460 2023-02-28 05:48:16.662067 orwynn-1.0.0b3/orwynn/log/log_websocket_middleware_test.py
+-rw-r--r--   0        0        0     1560 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/mapping/_Mapping.py
+-rw-r--r--   0        0        0       30 2023-02-27 08:33:14.996815 orwynn-1.0.0b3/orwynn/mapping/__init__.py
+-rw-r--r--   0        0        0      281 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/mapping/errors.py
+-rw-r--r--   0        0        0      179 2023-02-27 08:32:55.043879 orwynn-1.0.0b3/orwynn/mapping/mapping_test.py
+-rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0b3/orwynn/mongo/_ClientSession.py
+-rw-r--r--   0        0        0     6048 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/mongo/_Document.py
+-rw-r--r--   0        0        0     3579 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/mongo/_Mongo.py
+-rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0b3/orwynn/mongo/_MongoConfig.py
+-rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0b3/orwynn/mongo/_MongoEntity.py
+-rw-r--r--   0        0        0      224 2023-02-28 05:48:16.650064 orwynn-1.0.0b3/orwynn/mongo/__init__.py
+-rw-r--r--   0        0        0     3300 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/mongo/document_test.py
+-rw-r--r--   0        0        0      445 2023-03-06 11:30:55.548595 orwynn-1.0.0b3/orwynn/mongo/errors.py
+-rw-r--r--   0        0        0     1361 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/mongo/mongo_test.py
+-rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0b3/orwynn/proxy/ApiIndicationOnlyProxy.py
+-rw-r--r--   0        0        0     2841 2023-05-15 10:17:07.786310 orwynn-1.0.0b3/orwynn/proxy/BootProxy.py
+-rw-r--r--   0        0        0    14266 2023-05-15 09:53:21.180789 orwynn-1.0.0b3/orwynn/router/_ControllerRegister.py
+-rw-r--r--   0        0        0     3952 2023-04-03 14:59:49.711980 orwynn-1.0.0b3/orwynn/router/_ErrorHandlerManager.py
+-rw-r--r--   0        0        0    10300 2023-04-21 09:57:57.046622 orwynn-1.0.0b3/orwynn/router/_MiddlewareRegister.py
+-rw-r--r--   0        0        0     2697 2023-03-07 08:22:34.931871 orwynn-1.0.0b3/orwynn/router/_Router.py
+-rw-r--r--   0        0        0       28 2023-02-27 13:24:49.469241 orwynn-1.0.0b3/orwynn/router/__init__.py
+-rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/router/errors.py
+-rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0b3/orwynn/router/global_http_route_test.py
+-rw-r--r--   0        0        0     1306 2023-01-10 10:10:51.782079 orwynn-1.0.0b3/orwynn/singleton/_Singleton.py
+-rw-r--r--   0        0        0       34 2023-02-27 08:21:14.680585 orwynn-1.0.0b3/orwynn/singleton/__init__.py
+-rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0b3/orwynn/sql/_PoolclassStr.py
+-rw-r--r--   0        0        0     3888 2023-05-15 09:39:14.553897 orwynn-1.0.0b3/orwynn/sql/_Sql.py
+-rw-r--r--   0        0        0     1972 2023-05-15 09:35:55.577896 orwynn-1.0.0b3/orwynn/sql/_SqlConfig.py
+-rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0b3/orwynn/sql/_SqlDatabaseKind.py
+-rw-r--r--   0        0        0     2648 2023-04-03 14:59:49.734980 orwynn-1.0.0b3/orwynn/sql/_Table.py
+-rw-r--r--   0        0        0      210 2023-02-28 05:15:28.490194 orwynn-1.0.0b3/orwynn/sql/__init__.py
+-rw-r--r--   0        0        0     5865 2023-04-03 14:59:49.751980 orwynn-1.0.0b3/orwynn/sql/sql_test.py
+-rw-r--r--   0        0        0    11258 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/testing/_Client.py
+-rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0b3/orwynn/testing/_EmbeddedTestClient.py
+-rw-r--r--   0        0        0      727 2023-02-28 05:48:16.655065 orwynn-1.0.0b3/orwynn/testing/__init__.py
+-rw-r--r--   0        0        0     2057 2023-03-07 08:43:05.624039 orwynn-1.0.0b3/orwynn/testing/client_test.py
+-rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0b3/orwynn/utils/BaseSubclassable.py
+-rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0b3/orwynn/utils/Protocol.py
+-rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/crypto/__init__.py
+-rw-r--r--   0        0        0      448 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/dt/__init__.py
+-rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0b3/orwynn/utils/fmt/__init__.py
+-rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/fmt/fmt_test.py
+-rw-r--r--   0        0        0     1974 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/klass/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0b3/orwynn/utils/klass/_errors.py
+-rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0b3/orwynn/utils/klass/klass_test.py
+-rw-r--r--   0        0        0     2545 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/mp/__init__.py
+-rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0b3/orwynn/utils/mp/_dictpp.py
+-rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0b3/orwynn/utils/mp/location.py
+-rw-r--r--   0        0        0     1738 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/mp/mp_test.py
+-rw-r--r--   0        0        0      131 2023-02-21 10:53:24.615257 orwynn-1.0.0b3/orwynn/utils/rnd/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/rnd/rnd_test.py
+-rw-r--r--   0        0        0      176 2023-02-17 07:26:21.447070 orwynn-1.0.0b3/orwynn/utils/types.py
+-rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0b3/orwynn/utils/uio.py
+-rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0b3/orwynn/utils/url/_Url.py
+-rw-r--r--   0        0        0      254 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/url/_UrlVars.py
+-rw-r--r--   0        0        0      697 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/url/__init__.py
+-rw-r--r--   0        0        0     1934 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/url/_get_vars.py
+-rw-r--r--   0        0        0      419 2023-03-06 13:33:43.023337 orwynn-1.0.0b3/orwynn/utils/url/_match_routes.py
+-rw-r--r--   0        0        0     1412 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/url/get_vars_test.py
+-rw-r--r--   0        0        0     9151 2023-04-03 15:00:11.231062 orwynn-1.0.0b3/orwynn/utils/validation/__init__.py
+-rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0b3/orwynn/utils/validation/_validator.py
+-rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0b3/orwynn/utils/validation/errors.py
+-rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0b3/orwynn/utils/yml/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0b3/orwynn/utils/yml/errors.py
+-rw-r--r--   0        0        0      864 2023-03-06 12:13:17.936738 orwynn-1.0.0b3/orwynn/websocket/_BUILTIN_WEBSOCKET_MIDDLEWARE.py
+-rw-r--r--   0        0        0      248 2023-03-06 12:13:17.936738 orwynn-1.0.0b3/orwynn/websocket/_DEFAULT_WEBSOCKET_ERROR_HANDLERS.py
+-rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0b3/orwynn/websocket/_Websocket.py
+-rw-r--r--   0        0        0      836 2023-03-06 12:13:17.936738 orwynn-1.0.0b3/orwynn/websocket/__init__.py
+-rw-r--r--   0        0        0      579 2023-02-28 05:55:07.500801 orwynn-1.0.0b3/orwynn/websocket/_context/ContextBuiltinWebsocketMiddleware.py
+-rw-r--r--   0        0        0      824 2023-02-28 05:48:16.654065 orwynn-1.0.0b3/orwynn/websocket/_context/RequestContextBuiltinWebsocketMiddleware.py
+-rw-r--r--   0        0        0     1028 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_context/WebsocketRequestContextId.py
+-rw-r--r--   0        0        0     1291 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_context/websocket_context_test.py
+-rw-r--r--   0        0        0     3977 2023-04-07 10:11:54.671319 orwynn-1.0.0b3/orwynn/websocket/_controller/WebsocketController.py
+-rw-r--r--   0        0        0      902 2023-04-07 10:21:27.442702 orwynn-1.0.0b3/orwynn/websocket/_controller/WebsocketController_test.py
+-rw-r--r--   0        0        0      147 2023-02-27 07:44:23.427494 orwynn-1.0.0b3/orwynn/websocket/_controller/WebsocketEventHandlerMethod.py
+-rw-r--r--   0        0        0     2900 2023-02-28 05:48:16.658066 orwynn-1.0.0b3/orwynn/websocket/_controller/global_websocket_route_test.py
+-rw-r--r--   0        0        0     3026 2023-03-06 13:33:04.085558 orwynn-1.0.0b3/orwynn/websocket/_controller/websocket_controller_test.py
+-rw-r--r--   0        0        0      417 2023-03-06 12:12:57.645660 orwynn-1.0.0b3/orwynn/websocket/_errorhandler/DefaultWebsocketErrorHandler.py
+-rw-r--r--   0        0        0     3620 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_errorhandler/ErrorHandlerWebsocketMiddleware.py
+-rw-r--r--   0        0        0     1707 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_errorhandler/error_handler_websocket_test.py
+-rw-r--r--   0        0        0      920 2023-02-28 05:48:16.653065 orwynn-1.0.0b3/orwynn/websocket/_log/LogWebsocketMiddleware.py
+-rw-r--r--   0        0        0     1708 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_log/WebsocketLogger.py
+-rw-r--r--   0        0        0      313 2023-02-28 05:48:16.648064 orwynn-1.0.0b3/orwynn/websocket/_middleware/BuiltinWebsocketMiddleware.py
+-rw-r--r--   0        0        0      887 2023-02-28 05:48:16.653065 orwynn-1.0.0b3/orwynn/websocket/_middleware/ConnectionBuiltinWebsocketMiddleware.py
+-rw-r--r--   0        0        0      748 2023-02-28 05:48:16.653065 orwynn-1.0.0b3/orwynn/websocket/_middleware/WebsocketMiddleware.py
+-rw-r--r--   0        0        0      280 2023-02-27 13:14:10.637743 orwynn-1.0.0b3/orwynn/websocket/_middleware/WebsocketNextCall.py
+-rw-r--r--   0        0        0     1056 2023-02-28 05:48:16.647063 orwynn-1.0.0b3/orwynn/websocket/_middleware/websocket_middleware_test.py
+-rw-r--r--   0        0        0     1893 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_routing/NextCallHandler.py
+-rw-r--r--   0        0        0     6084 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_routing/WebsocketStack.py
+-rw-r--r--   0        0        0      231 2023-02-28 05:55:25.292122 orwynn-1.0.0b3/orwynn/websocket/_routing/_DispatchWebsocketFn.py
+-rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0b3/orwynn/websocket/_routing/_GenericWebsocketFn.py
+-rw-r--r--   0        0        0     5547 2023-04-03 14:59:49.717980 orwynn-1.0.0b3/orwynn/websocket/_routing/_get_handler_kwargs.py
+-rw-r--r--   0        0        0      448 2023-02-28 05:48:16.646063 orwynn-1.0.0b3/orwynn/websocket/_routing/handlers.py
+-rw-r--r--   0        0        0      823 2023-05-15 10:18:46.757980 orwynn-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 orwynn-1.0.0b3/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 orwynn-1.0.0b3/PKG-INFO
```

### Comparing `orwynn-1.0.0b2/LICENSE` & `orwynn-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/Di.py` & `orwynn-1.0.0b3/orwynn/_di/Di.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/DiContainer.py` & `orwynn-1.0.0b3/orwynn/_di/DiContainer.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/ProviderAvailabilityError.py` & `orwynn-1.0.0b3/orwynn/_di/ProviderAvailabilityError.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/_collect_dependencies_for_acceptor.py` & `orwynn-1.0.0b3/orwynn/_di/_collect_dependencies_for_acceptor.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/check_availability.py` & `orwynn-1.0.0b3/orwynn/_di/check_availability.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/collecting/ModuleCollector.py` & `orwynn-1.0.0b3/orwynn/_di/collecting/ModuleCollector.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/collecting/collect_modules_test.py` & `orwynn-1.0.0b3/orwynn/_di/collecting/collect_modules_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/collecting/collect_provider_dependencies.py` & `orwynn-1.0.0b3/orwynn/_di/collecting/collect_provider_dependencies.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/collecting/collect_provider_dependencies_test.py` & `orwynn-1.0.0b3/orwynn/_di/collecting/collect_provider_dependencies_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/collecting/get_parameters_for_provider.py` & `orwynn-1.0.0b3/orwynn/_di/collecting/get_parameters_for_provider.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/collecting/provider_dependencies_map.py` & `orwynn-1.0.0b3/orwynn/_di/collecting/provider_dependencies_map.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/di_test.py` & `orwynn-1.0.0b3/orwynn/_di/di_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/init/init_other_acceptors.py` & `orwynn-1.0.0b3/orwynn/_di/init/init_other_acceptors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/init/init_other_acceptors_test.py` & `orwynn-1.0.0b3/orwynn/_di/init/init_other_acceptors_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/init/init_providers.py` & `orwynn-1.0.0b3/orwynn/_di/init/init_providers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_di/init/init_providers_test.py` & `orwynn-1.0.0b3/orwynn/_di/init/init_providers_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/_testingtools/__init__.py` & `orwynn-1.0.0b3/orwynn/_testingtools/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/apiversion/_ApiVersion.py` & `orwynn-1.0.0b3/orwynn/apiversion/_ApiVersion.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/apiversion/api_version_test.py` & `orwynn-1.0.0b3/orwynn/apiversion/api_version_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/app/_ApiWebsocketRoute.py` & `orwynn-1.0.0b3/orwynn/app/_ApiWebsocketRoute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/app/_App.py` & `orwynn-1.0.0b3/orwynn/app/_App.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/app/_CoreApp.py` & `orwynn-1.0.0b3/orwynn/app/_CoreApp.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/app/_get_dependant.py` & `orwynn-1.0.0b3/orwynn/app/_get_dependant.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/app/app_test.py` & `orwynn-1.0.0b3/orwynn/app/app_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/apprc/_parse_apprc.py` & `orwynn-1.0.0b3/orwynn/apprc/_parse_apprc.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/apprc/apprc_test.py` & `orwynn-1.0.0b3/orwynn/apprc/apprc_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/config/_Config.py` & `orwynn-1.0.0b3/orwynn/base/config/_Config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/controller/_Controller.py` & `orwynn-1.0.0b3/orwynn/base/controller/_Controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/database/_Database.py` & `orwynn-1.0.0b3/orwynn/base/database/_Database.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/database/errors.py` & `orwynn-1.0.0b3/orwynn/base/database/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/error/_errcode.py` & `orwynn-1.0.0b3/orwynn/base/error/_errcode.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/error/_find_detailed_class_for_exception.py` & `orwynn-1.0.0b3/orwynn/base/error/_find_detailed_class_for_exception.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/error/errcode_test.py` & `orwynn-1.0.0b3/orwynn/base/error/errcode_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/errorhandler/_ErrorHandler.py` & `orwynn-1.0.0b3/orwynn/base/errorhandler/_ErrorHandler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/middleware/_Middleware.py` & `orwynn-1.0.0b3/orwynn/base/middleware/_Middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/middleware/global_middleware_test.py` & `orwynn-1.0.0b3/orwynn/base/middleware/global_middleware_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/model/_Model.py` & `orwynn-1.0.0b3/orwynn/base/model/_Model.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/model/model_test.py` & `orwynn-1.0.0b3/orwynn/base/model/model_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/module/_Module.py` & `orwynn-1.0.0b3/orwynn/base/module/_Module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/base/module/module_test.py` & `orwynn-1.0.0b3/orwynn/base/module/module_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/boot/_Boot.py` & `orwynn-1.0.0b3/orwynn/boot/_Boot.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/boot/_BootConfig.py` & `orwynn-1.0.0b3/orwynn/boot/_BootConfig.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/boot/boot_test.py` & `orwynn-1.0.0b3/orwynn/boot/boot_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/bootscript/_BootscriptWorker.py` & `orwynn-1.0.0b3/orwynn/bootscript/_BootscriptWorker.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/bootscript/bootscript_test.py` & `orwynn-1.0.0b3/orwynn/bootscript/bootscript_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/context/_ContextStorage.py` & `orwynn-1.0.0b3/orwynn/context/_ContextStorage.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/context/_context_manager.py` & `orwynn-1.0.0b3/orwynn/context/_context_manager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/helpers/SUBCLASSABLES.py` & `orwynn-1.0.0b3/orwynn/helpers/SUBCLASSABLES.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/helpers/web.py` & `orwynn-1.0.0b3/orwynn/helpers/web.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_BUILTIN_HTTP_MIDDLEWARE.py` & `orwynn-1.0.0b3/orwynn/http/_BUILTIN_HTTP_MIDDLEWARE.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/__init__.py` & `orwynn-1.0.0b3/orwynn/http/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from ._log.LogMiddleware import LogMiddleware
 from ._middleware.BuiltinHttpMiddleware import BuiltinHttpMiddleware
 from ._middleware.HttpMiddleware import HttpMiddleware
 from ._middleware.HttpNextCall import HttpNextCall
 from ._requests import HttpRequest
 from ._responses import (
+    FileHttpResponse,
     HtmlHttpResponse,
     HttpResponse,
     JsonHttpResponse,
     TestHttpResponse,
 )
 from ._schema.HttpExceptionValueSchema import HttpExceptionValueSchema
 from ._schema.RequestValidationExceptionValueSchema import (
```

### Comparing `orwynn-1.0.0b2/orwynn/http/_context/ContextBuiltinMiddleware.py` & `orwynn-1.0.0b3/orwynn/http/_context/ContextBuiltinMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_context/HttpRequestContextBuiltinMiddleware.py` & `orwynn-1.0.0b3/orwynn/http/_context/HttpRequestContextBuiltinMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_context/HttpRequestContextId.py` & `orwynn-1.0.0b3/orwynn/http/_context/HttpRequestContextId.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_context/context_test.py` & `orwynn-1.0.0b3/orwynn/http/_context/context_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_controller/HttpController.py` & `orwynn-1.0.0b3/orwynn/http/_controller/HttpController.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_controller/endpoint/Endpoint.py` & `orwynn-1.0.0b3/orwynn/http/_controller/endpoint/Endpoint.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_controller/endpoint/EndpointContainer.py` & `orwynn-1.0.0b3/orwynn/http/_controller/endpoint/EndpointContainer.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_controller/endpoint/endpoint_test.py` & `orwynn-1.0.0b3/orwynn/http/_controller/endpoint/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_controller/http_controller_test.py` & `orwynn-1.0.0b3/orwynn/http/_controller/http_controller_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+from fastapi import Query, Request
+
 from orwynn._di.Di import Di
 from orwynn.apiversion import ApiVersion
 from orwynn.base.controller.errors import (
     AlreadyRegisteredMethodError,
     MissingControllerClassAttributeError,
 )
 from orwynn.base.model import Model
@@ -246,7 +249,40 @@
     assert ctrl.is_matching_route("/api/v3/donuts/helloworld/tasty") is False
     ##
 
     assert ctrl.is_matching_route("/api/v2/donuts/e67840v/tasty/gogo") is False
     assert ctrl.is_matching_route("/api/v2/donuts/tasty") is False
     assert ctrl.is_matching_route("/api/donuts/eb00v/tasty") is False
     assert ctrl.is_matching_route("/donuts/eb00v/tasty") is False
+
+
+def test_multiple_query_params():
+    """
+    Should correctly parse list of query params.
+    """
+    class _Ctrl(HttpController):
+        ROUTE = "/items"
+        ENDPOINTS = [
+            Endpoint(method="get")
+        ]
+
+        def get(
+            self,
+            request: Request,
+            q: list[str] | None = Query(None)
+        ) -> dict:
+            return {
+                "q": q
+            }
+
+    boot: Boot = Boot(
+        Module("/", Controllers=[_Ctrl])
+    )
+
+    data: dict = boot.client.get_jsonify(
+        "/items?q=1&q=2",
+        200
+    )
+
+    assert data == {
+        "q": ["1", "2"]
+    }
```

### Comparing `orwynn-1.0.0b2/orwynn/http/_cors/cors_test.py` & `orwynn-1.0.0b3/orwynn/http/_cors/cors_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_errorhandler/ErrorHandlerHttpMiddleware.py` & `orwynn-1.0.0b3/orwynn/http/_errorhandler/ErrorHandlerHttpMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_errorhandler/default.py` & `orwynn-1.0.0b3/orwynn/http/_errorhandler/default.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_errorhandler/error_handler_test.py` & `orwynn-1.0.0b3/orwynn/http/_errorhandler/error_handler_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_log/HttpLogger.py` & `orwynn-1.0.0b3/orwynn/http/_log/HttpLogger.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,18 @@
     ) -> None:
         """Logs a response linking it to the according request.
         """
         # Fetch response body: for StreamingResponse it should apply special
         # logic.
         response_body: str
         if isinstance(response, StreamingResponse):
-            response_body: str = await self.__get_response_body(response)
+            try:
+                response_body: str = await self.__get_response_body(response)
+            except UnicodeDecodeError:
+                response_body = ""
         else:
             # Interestingly, even returned explicitly JSONResponse handled here
             # as StreamingResponse, so maybe there is not need to handle
             # "else:" branch here.
             raise MalfunctionError(
                 f"unexpected branch entering for response {response}"
             )
@@ -91,21 +94,26 @@
             # get the MalfunctionError:
 
         plain_message: str = \
             f"response {response.status_code}" \
             f" {request.url.path}{request.url.query}:" \
             f" {response_body}"
         json_: dict | None
-        json_ = validation.apply(
-            json.loads(
-                response_body
-            ),
-            dict
-        )
-        if not json_:
+
+        content_type: str = response.headers.get("content-type", "")
+        if "application/json" in content_type:
+            json_ = validation.apply(
+                json.loads(
+                    response_body
+                ),
+                dict
+            )
+            if not json_:
+                json_ = None
+        else:
             json_ = None
 
         extra: dict = {
             "http.response": {
                 "status_code": response.status_code,
                 "request_id": request_id,
                 "media_type": response.media_type,
```

### Comparing `orwynn-1.0.0b2/orwynn/http/_log/LogMiddleware.py` & `orwynn-1.0.0b3/orwynn/http/_log/LogMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_middleware/HttpMiddleware.py` & `orwynn-1.0.0b3/orwynn/http/_middleware/HttpMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/http/_middleware/http_middleware_test.py` & `orwynn-1.0.0b3/orwynn/http/_middleware/http_middleware_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/indication/_Indication.py` & `orwynn-1.0.0b3/orwynn/indication/_Indication.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,18 @@
                     f" type: {type(enum_value)}, only str or int are"
                     " supported"
                 )
 
             final_error_code = enum_value
 
         else:
-            if not type(error_code) is int or not type(error_code) is str:
+            if (
+                not isinstance(error_code, int)
+                and not isinstance(error_code, str)
+            ):
                 raise validation.ValidationError(
                     "error code should be int, str or enum,"
                     f" got {type(error_code)}"
                 )
             final_error_code = error_code
 
         return final_error_code
```

### Comparing `orwynn-1.0.0b2/orwynn/indication/indication_test.py` & `orwynn-1.0.0b3/orwynn/indication/indication_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -99,18 +99,34 @@
 
     class SimpleError(Exception):
         CODE = ErrorCode.SIMPLE_CASE
 
     class AdvancedError(Exception):
         CODE = ErrorCode.ADVANCED_CASE
 
+    class IntError(Exception):
+        CODE = 5
+
+    class StrError(Exception):
+        CODE = "hello"
+
     data: dict
 
     data = default_indication.digest(SimpleError("hello world"))
     assert data["type"] == "error"
     assert data["value"]["message"] == "hello world"
     assert data["value"]["error_code"] == ErrorCode.SIMPLE_CASE.value
 
     data = default_indication.digest(AdvancedError("hello world"))
     assert data["type"] == "error"
     assert data["value"]["message"] == "hello world"
     assert data["value"]["error_code"] == ErrorCode.ADVANCED_CASE.value
+
+    data = default_indication.digest(IntError("hello world"))
+    assert data["type"] == "error"
+    assert data["value"]["message"] == "hello world"
+    assert data["value"]["error_code"] == 5
+
+    data = default_indication.digest(StrError("hello world"))
+    assert data["type"] == "error"
+    assert data["value"]["message"] == "hello world"
+    assert data["value"]["error_code"] == "hello"
```

### Comparing `orwynn-1.0.0b2/orwynn/log/_LogHandler.py` & `orwynn-1.0.0b3/orwynn/log/_LogHandler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/log/_configure_log.py` & `orwynn-1.0.0b3/orwynn/log/_configure_log.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/log/log_middleware_test.py` & `orwynn-1.0.0b3/orwynn/log/log_middleware_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/log/log_test.py` & `orwynn-1.0.0b3/orwynn/log/log_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/log/log_websocket_middleware_test.py` & `orwynn-1.0.0b3/orwynn/log/log_websocket_middleware_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/mapping/_Mapping.py` & `orwynn-1.0.0b3/orwynn/mapping/_Mapping.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/mongo/_Document.py` & `orwynn-1.0.0b3/orwynn/mongo/_Document.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/mongo/_Mongo.py` & `orwynn-1.0.0b3/orwynn/mongo/_Mongo.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/mongo/document_test.py` & `orwynn-1.0.0b3/orwynn/mongo/document_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/mongo/mongo_test.py` & `orwynn-1.0.0b3/orwynn/mongo/mongo_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/proxy/BootProxy.py` & `orwynn-1.0.0b3/orwynn/proxy/BootProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         self.__ErrorHandlers: set[type["ErrorHandler"]] = \
             ErrorHandlers
         self.__global_http_route: str = global_http_route
         self.__global_websocket_route: str = global_websocket_route
         self.__api_version: ApiVersion = api_version
 
     @property
+    def root_dir(self) -> Path:
+        return self.__root_dir
+
+    @property
     def mode(self) -> "AppMode":
         return self.__mode
 
     @property
     def api_indication(self) -> "Indication":
         return self.__api_indication
```

### Comparing `orwynn-1.0.0b2/orwynn/router/_ControllerRegister.py` & `orwynn-1.0.0b3/orwynn/router/_ControllerRegister.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     EndpointNotFoundError,
     UnsupportedHttpMethodError,
 )
 from orwynn.indication._Indication import Indication
 from orwynn.proxy.BootProxy import BootProxy
 from orwynn.router.errors import (
     UnmatchedEndpointEntityError,
-    WrongHandlerReturnTypeError,
 )
 from orwynn.utils import validation
 from orwynn.utils.Protocol import Protocol
 from orwynn.utils.url import join_routes
 from orwynn.websocket import (
     WebsocketController,
     WebsocketStack,
@@ -323,20 +322,14 @@
                     and issubclass(fn_return_typehint, Model)
                 ):
                     final_responses[spec.default_status_code] = {
                         "model": api_indication.gen_schema(
                             fn_return_typehint
                         )
                     }
-                elif fn_return_typehint not in [dict, None]:
-                    raise WrongHandlerReturnTypeError(
-                        f"route handler {fn} should have either Model, dict"
-                        f" or None return type, got {fn_return_typehint}"
-                        " instead"
-                    )
                 else:
                     result["response_model"] = None
 
             # Add default pydantic validation error
             if (
                 422 not in final_responses
                 and self.__is_pydantic_validation_error_can_occur_in_fn(fn)
```

### Comparing `orwynn-1.0.0b2/orwynn/router/_ErrorHandlerManager.py` & `orwynn-1.0.0b3/orwynn/router/_ErrorHandlerManager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/router/_MiddlewareRegister.py` & `orwynn-1.0.0b3/orwynn/router/_MiddlewareRegister.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/router/_Router.py` & `orwynn-1.0.0b3/orwynn/router/_Router.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/router/global_http_route_test.py` & `orwynn-1.0.0b3/orwynn/router/global_http_route_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/singleton/_Singleton.py` & `orwynn-1.0.0b3/orwynn/singleton/_Singleton.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/sql/_Sql.py` & `orwynn-1.0.0b3/orwynn/sql/_Sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 class Sql(Database):
     def __init__(
         self,
         config: SqlConfig
     ) -> None:
         super().__init__()
         self.__config = config
-        self.__engine: Engine = self.__create_engine()
+        self.__engine: Engine = self._create_engine()
+
+    @property
+    def engine(self) -> Engine:
+        return self.__engine
 
     @property
     def session(self) -> Session:
         """Returns a new session."""
         return Session(self.__engine)
 
     def create_tables(self, *tables: type[Table]) -> None:
@@ -33,44 +37,46 @@
         Args:
             *tables:
                 Tables to create. If no tables are given (or None), all
                 reachable tables are created.
         """
         Table.metadata.create_all(
             self.__engine,
-            tables=self.__collect_sqla_tables(*tables)
+            tables=self._collect_sqla_tables(*tables)
         )
 
     def drop_tables(self, *tables: type[Table]) -> None:
         """Drops tables.
 
         Args:
             *tables:
                 Tables to drop. If no tables are given (or None), all
                 reachable tables are dropped.
         """
         Table.metadata.drop_all(
             self.__engine,
-            tables=self.__collect_sqla_tables(*tables)
+            tables=self._collect_sqla_tables(*tables)
         )
 
-    def __collect_sqla_tables(
+    def _collect_sqla_tables(
         self,
         *tables: type[Table]
     ) -> Optional[Sequence[SQLAlchemyTable]]:
         sqla_tables: Optional[Sequence[SQLAlchemyTable]] = None
         if tables:
             sqla_tables = []
             for table in tables:
                 sqla_tables.append(table.__table__)  # type: ignore
         return sqla_tables
 
-    def __create_engine(self) -> Engine:
+    def _create_engine(self) -> Engine:
         url: str
         connect_args: dict = {}
+        final_kwargs: dict = {}
+
         match self.__config.database_kind:
             case SQLDatabaseKind.POSTGRESQL:
                 url = \
                     f"postgresql://{self.__config.database_user}" \
                     + f":{self.__config.database_password}" \
                     + f"@{self.__config.database_host}" \
                     + f":{self.__config.database_port}" \
@@ -95,12 +101,17 @@
                 # with the database for the same request.
                 # See https://fastapi.tiangolo.com/tutorial/sql-databases/#note
                 connect_args.update({"check_same_thread": False})
             case _:
                 raise TypeError(
                     f"unknown database {self.__config.database_kind}"
                 )
+
+        final_kwargs["connect_args"] = connect_args
+        final_kwargs["poolclass"] = self.__config.real_poolclass
+        if self.__config.pool_size:
+            final_kwargs["pool_size"] = self.__config.pool_size
+
         return create_engine(
             url,
-            connect_args=connect_args,
-            poolclass=self.__config.real_poolclass
+            **final_kwargs
         )
```

### Comparing `orwynn-1.0.0b2/orwynn/sql/_SqlConfig.py` & `orwynn-1.0.0b3/orwynn/sql/_SqlConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     database_name: str | None = None
     database_user: str | None = None
     database_password: str | None = None
     database_path: str | None = None
     database_host: str | None = None
     database_port: int | None = None
     poolclass: PoolclassStr | None = None
+    pool_size: int | None = None
 
     def __init__(self, **data: Any) -> None:
         try:
             db_kind: SQLDatabaseKind = SQLDatabaseKind(data["database_kind"])
         except KeyError as err:
             raise KeyError(
                 "define key \"database_kind\" in your apprc config"
```

### Comparing `orwynn-1.0.0b2/orwynn/sql/_Table.py` & `orwynn-1.0.0b3/orwynn/sql/_Table.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/sql/sql_test.py` & `orwynn-1.0.0b3/orwynn/sql/sql_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/testing/_Client.py` & `orwynn-1.0.0b3/orwynn/testing/_Client.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/testing/__init__.py` & `orwynn-1.0.0b3/orwynn/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/testing/client_test.py` & `orwynn-1.0.0b3/orwynn/testing/client_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/crypto/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/fmt/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/fmt/fmt_test.py` & `orwynn-1.0.0b3/orwynn/utils/fmt/fmt_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/klass/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/klass/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/klass/klass_test.py` & `orwynn-1.0.0b3/orwynn/utils/klass/klass_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/mp/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/mp/location.py` & `orwynn-1.0.0b3/orwynn/utils/mp/location.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/mp/mp_test.py` & `orwynn-1.0.0b3/orwynn/utils/mp/mp_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/url/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/url/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/url/_get_vars.py` & `orwynn-1.0.0b3/orwynn/utils/url/_get_vars.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/url/get_vars_test.py` & `orwynn-1.0.0b3/orwynn/utils/url/get_vars_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/validation/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/validation/errors.py` & `orwynn-1.0.0b3/orwynn/utils/validation/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/utils/yml/__init__.py` & `orwynn-1.0.0b3/orwynn/utils/yml/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_BUILTIN_WEBSOCKET_MIDDLEWARE.py` & `orwynn-1.0.0b3/orwynn/websocket/_BUILTIN_WEBSOCKET_MIDDLEWARE.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/__init__.py` & `orwynn-1.0.0b3/orwynn/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_context/ContextBuiltinWebsocketMiddleware.py` & `orwynn-1.0.0b3/orwynn/websocket/_context/ContextBuiltinWebsocketMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_context/RequestContextBuiltinWebsocketMiddleware.py` & `orwynn-1.0.0b3/orwynn/websocket/_context/RequestContextBuiltinWebsocketMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_context/WebsocketRequestContextId.py` & `orwynn-1.0.0b3/orwynn/websocket/_context/WebsocketRequestContextId.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_context/websocket_context_test.py` & `orwynn-1.0.0b3/orwynn/websocket/_context/websocket_context_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_controller/WebsocketController.py` & `orwynn-1.0.0b3/orwynn/websocket/_controller/WebsocketController.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_controller/WebsocketController_test.py` & `orwynn-1.0.0b3/orwynn/websocket/_controller/WebsocketController_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_controller/global_websocket_route_test.py` & `orwynn-1.0.0b3/orwynn/websocket/_controller/global_websocket_route_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_controller/websocket_controller_test.py` & `orwynn-1.0.0b3/orwynn/websocket/_controller/websocket_controller_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_errorhandler/ErrorHandlerWebsocketMiddleware.py` & `orwynn-1.0.0b3/orwynn/websocket/_errorhandler/ErrorHandlerWebsocketMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_errorhandler/error_handler_websocket_test.py` & `orwynn-1.0.0b3/orwynn/websocket/_errorhandler/error_handler_websocket_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_log/LogWebsocketMiddleware.py` & `orwynn-1.0.0b3/orwynn/websocket/_log/LogWebsocketMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_log/WebsocketLogger.py` & `orwynn-1.0.0b3/orwynn/websocket/_log/WebsocketLogger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_middleware/ConnectionBuiltinWebsocketMiddleware.py` & `orwynn-1.0.0b3/orwynn/websocket/_middleware/ConnectionBuiltinWebsocketMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_middleware/WebsocketMiddleware.py` & `orwynn-1.0.0b3/orwynn/websocket/_middleware/WebsocketMiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_middleware/websocket_middleware_test.py` & `orwynn-1.0.0b3/orwynn/websocket/_middleware/websocket_middleware_test.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_routing/NextCallHandler.py` & `orwynn-1.0.0b3/orwynn/websocket/_routing/NextCallHandler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_routing/WebsocketStack.py` & `orwynn-1.0.0b3/orwynn/websocket/_routing/WebsocketStack.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/orwynn/websocket/_routing/_get_handler_kwargs.py` & `orwynn-1.0.0b3/orwynn/websocket/_routing/_get_handler_kwargs.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b2/pyproject.toml` & `orwynn-1.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orwynn"
-version = "1.0.0b2"
+version = "1.0.0b3"
 description = "Scalable web-framework with out-of-the-box architecture"
 authors = ["ryzhovalex <thed4rkof@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.88.0"
```

### Comparing `orwynn-1.0.0b2/setup.py` & `orwynn-1.0.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
  'pyyaml>=6.0,<7.0',
  'sqlalchemy>=2.0.3,<3.0.0',
  'uvicorn[standard]>=0.20.0,<0.21.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'orwynn',
-    'version': '1.0.0b2',
+    'version': '1.0.0b3',
     'description': 'Scalable web-framework with out-of-the-box architecture',
     'long_description': '# Orwynn',
     'author': 'ryzhovalex',
     'author_email': 'thed4rkof@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `orwynn-1.0.0b2/PKG-INFO` & `orwynn-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orwynn
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Scalable web-framework with out-of-the-box architecture
 Author: ryzhovalex
 Author-email: thed4rkof@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

