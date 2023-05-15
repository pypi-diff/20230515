# Comparing `tmp/st4sd-runtime-core-2.0.0a9.dev5.tar.gz` & `tmp/st4sd-runtime-core-2.0.0a9.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st4sd-runtime-core-2.0.0a9.dev5.tar", last modified: Thu May  4 09:10:29 2023, max compression
+gzip compressed data, was "dist/st4sd-runtime-core-2.0.0a9.dev7.tar", last modified: Mon May 15 07:57:42 2023, max compression
```

## Comparing `st4sd-runtime-core-2.0.0a9.dev5.tar` & `st4sd-runtime-core-2.0.0a9.dev7.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/.github/
--rw-rw-r--   0 root         (0) root         (0)      127 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/.github/dco.yml
--rw-rw-r--   0 root         (0) root         (0)     1799 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     8059 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/.travis.yml
--rw-rw-r--   0 root         (0) root         (0)       77 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/.whitesource
--rw-rw-r--   0 root         (0) root         (0)     3347 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/CODE_OF_CONDUCT.md
--rw-rw-r--   0 root         (0) root         (0)     2643 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/CONTRIBUTING.md
--rw-rw-r--   0 root         (0) root         (0)     2445 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)    10774 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/LICENSE.md
--rw-rw-r--   0 root         (0) root         (0)      439 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/MAINTAINERS.md
--rw-r--r--   0 root         (0) root         (0)     4097 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3334 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/
--rw-rw-r--   0 root         (0) root         (0)      180 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/creation_payload.json
--rwxrwxr-x   0 root         (0) root         (0)      292 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/skopeo_copy.sh
--rw-rw-r--   0 root         (0) root         (0)      635 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/st4sd-runtime-core-image.deploy
--rw-rw-r--   0 root         (0) root         (0)     1426 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/st4sd-runtime-core-multiarch.deploy
--rw-rw-r--   0 root         (0) root         (0)      291 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/st4sd-runtime-core-release-tag.deploy
--rwxrwxr-x   0 root         (0) root         (0)     2445 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/deploy/triggerExternalBuild.sh
--rw-rw-r--   0 root         (0) root         (0)     2442 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/py310.Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    35722 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/appenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/
--rw-rw-r--   0 root         (0) root         (0)      112 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2342 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/api.py
--rw-rw-r--   0 root         (0) root         (0)     2411 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     2891 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/context.py
--rw-rw-r--   0 root         (0) root         (0)      266 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/exit_codes.py
--rw-rw-r--   0 root         (0) root         (0)     1899 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/git.py
--rw-rw-r--   0 root         (0) root         (0)     5140 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/login.py
--rw-rw-r--   0 root         (0) root         (0)    18250 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/package.py
--rw-rw-r--   0 root         (0) root         (0)    31124 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/pvep_schema.jsonschema
--rw-rw-r--   0 root         (0) root         (0)     2300 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/stp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3003 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/codes.py
--rw-rw-r--   0 root         (0) root         (0)    82296 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/conf.py
--rw-rw-r--   0 root         (0) root         (0)   148053 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/data.py
--rw-rw-r--   0 root         (0) root         (0)    44154 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/errors.py
--rw-rw-r--   0 root         (0) root         (0)    57316 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   126138 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/cwl.py
--rw-rw-r--   0 root         (0) root         (0)    85741 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/dosini.py
--rw-rw-r--   0 root         (0) root         (0)   257676 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/flowir.py
--rw-rw-r--   0 root         (0) root         (0)   147639 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/
--rw-rw-r--   0 root         (0) root         (0)      683 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4236 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/hooks.py
--rw-rw-r--   0 root         (0) root         (0)    36110 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/interface.py
--rw-rw-r--   0 root         (0) root         (0)     2394 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/utils.py
--rw-rw-r--   0 root         (0) root         (0)     5562 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/interface.py
--rw-rw-r--   0 root         (0) root         (0)    67317 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package/
--rw-rw-r--   0 root         (0) root         (0)      544 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package/conf/
--rw-rw-r--   0 root         (0) root         (0)      376 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package/conf/flowir_package.yaml
--rw-rw-r--   0 root         (0) root         (0)     6144 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package.tar
--rw-rw-r--   0 root         (0) root         (0)      630 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/rewrite-rules.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      753 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/docker.py
--rw-rw-r--   0 root         (0) root         (0)   114992 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/k8s.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/localtask.py
--rw-rw-r--   0 root         (0) root         (0)   113107 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/lsf.py
--rwxrwxr-x   0 root         (0) root         (0)     1414 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/stage-out.sh
--rw-rw-r--   0 root         (0) root         (0)    13277 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/task_simulator.py
--rw-rw-r--   0 root         (0) root         (0)    34639 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backends.py
--rw-rw-r--   0 root         (0) root         (0)    23603 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backends_base.py
--rw-rw-r--   0 root         (0) root         (0)   118126 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/control.py
--rw-rw-r--   0 root         (0) root         (0)   104583 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/engine.py
--rw-rw-r--   0 root         (0) root         (0)     5429 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    26290 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/cwl.py
--rw-rw-r--   0 root         (0) root         (0)     9481 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/cwl_cmdline.py
--rw-rw-r--   0 root         (0) root         (0)     8089 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/js.py
--rw-rw-r--   0 root         (0) root         (0)    20080 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/monitor.py
--rw-rw-r--   0 root         (0) root         (0)    68147 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/optimizer.py
--rw-rw-r--   0 root         (0) root         (0)    34954 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/output.py
--rw-rw-r--   0 root         (0) root         (0)    45119 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/span.py
--rw-rw-r--   0 root         (0) root         (0)    35543 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/status.py
--rw-rw-r--   0 root         (0) root         (0)     5622 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3879 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/container_image_cache.py
--rw-rw-r--   0 root         (0) root         (0)     4089 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/rx.py
--rw-rw-r--   0 root         (0) root         (0)     5384 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/s3.py
--rw-rw-r--   0 root         (0) root         (0)    36584 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/service/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/service/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   259382 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/service/db.py
--rw-rw-r--   0 root         (0) root         (0)     8206 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/service/errors.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/settings.py
--rw-rw-r--   0 root         (0) root         (0)     6441 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/
--rw-rw-r--   0 root         (0) root         (0)      104 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/README
--rw-rw-r--   0 root         (0) root         (0)      317 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    58393 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/data.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/fsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4097 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4567 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/requirement_files/
--rw-rw-r--   0 root         (0) root         (0)      133 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/requirement_files/requirements_base_3.7.txt
--rw-rw-r--   0 root         (0) root         (0)      423 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/requirement_files/requirements_base_3.txt
--rw-rw-r--   0 root         (0) root         (0)       18 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/requirement_files/requirements_deploy.txt
--rw-rw-r--   0 root         (0) root         (0)       94 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/requirement_files/requirements_lsf.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/
--rwxrwxr-x   0 root         (0) root         (0)     7054 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/ccommand.py
--rwxrwxr-x   0 root         (0) root         (0)    11413 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/cexecute.py
--rwxrwxr-x   0 root         (0) root         (0)     1239 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/checkpackage.py
--rwxrwxr-x   0 root         (0) root         (0)     4286 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/ctest.py
--rwxrwxr-x   0 root         (0) root         (0)     2567 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/ecreate.py
--rwxrwxr-x   0 root         (0) root         (0)     4196 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/eflowir.py
--rwxrwxr-x   0 root         (0) root         (0)     8094 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/einputs.py
--rwxrwxr-x   0 root         (0) root         (0)     8246 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/einspect.py
--rwxrwxr-x   0 root         (0) root         (0)   106886 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/elaunch.py
--rwxrwxr-x   0 root         (0) root         (0)    17228 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/ememo.py
--rwxrwxr-x   0 root         (0) root         (0)    46741 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/epatch-apply.py
--rwxrwxr-x   0 root         (0) root         (0)    33324 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/epatch.py
--rwxrwxr-x   0 root         (0) root         (0)    17371 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/etest.py
--rwxrwxr-x   0 root         (0) root         (0)    10419 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/ewrap.py
--rwxrwxr-x   0 root         (0) root         (0)      821 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/expstatus.sh
--rw-rw-r--   0 root         (0) root         (0)     3840 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/k8srun.py
--rwxrwxr-x   0 root         (0) root         (0)   106886 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/launchexperiment.py
--rwxrwxr-x   0 root         (0) root         (0)    14013 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/lsfsub.py
--rwxrwxr-x   0 root         (0) root         (0)      262 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/scripts/stp
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     4693 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:10:29.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10844 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/conftest.py
--rw-rw-r--   0 root         (0) root         (0)    11290 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/dont_test_cwl.py
--rw-rw-r--   0 root         (0) root         (0)     4541 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/reactive_testutils.py
--rw-rw-r--   0 root         (0) root         (0)    14765 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/saltcurve_paragon.py
--rw-rw-r--   0 root         (0) root         (0)    11225 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_array_variables.py
--rw-rw-r--   0 root         (0) root         (0)     6643 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_command.py
--rw-rw-r--   0 root         (0) root         (0)     7643 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_component.py
--rw-rw-r--   0 root         (0) root         (0)     2432 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_container_image_uri_manipulation.py
--rw-rw-r--   0 root         (0) root         (0)    44829 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_control.py
--rw-rw-r--   0 root         (0) root         (0)     4840 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_data.py
--rw-rw-r--   0 root         (0) root         (0)     5588 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_db.py
--rw-rw-r--   0 root         (0) root         (0)    40697 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_dosini.py
--rw-rw-r--   0 root         (0) root         (0)    35269 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_dowhile.py
--rw-rw-r--   0 root         (0) root         (0)    30930 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_engines.py
--rw-rw-r--   0 root         (0) root         (0)    57435 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_flowir.py
--rw-rw-r--   0 root         (0) root         (0)    18304 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_graph.py
--rw-rw-r--   0 root         (0) root         (0)     3286 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_identifier.py
--rw-rw-r--   0 root         (0) root         (0)    22435 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_interface.py
--rw-rw-r--   0 root         (0) root         (0)     6059 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_k8s.py
--rw-rw-r--   0 root         (0) root         (0)     2467 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_memoization.py
--rw-rw-r--   0 root         (0) root         (0)    13525 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_package_load.py
--rw-rw-r--   0 root         (0) root         (0)     1673 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_service.py
--rw-rw-r--   0 root         (0) root         (0)     2085 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     5739 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tests/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3119 2023-05-04 09:06:38.000000 st4sd-runtime-core-2.0.0a9.dev5/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/.github/
+-rw-rw-r--   0 root         (0) root         (0)      127 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/.github/dco.yml
+-rw-rw-r--   0 root         (0) root         (0)     1799 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     8059 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)       77 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/.whitesource
+-rw-rw-r--   0 root         (0) root         (0)     3347 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 root         (0) root         (0)     2643 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/CONTRIBUTING.md
+-rw-rw-r--   0 root         (0) root         (0)     2445 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)    10774 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/LICENSE.md
+-rw-rw-r--   0 root         (0) root         (0)      439 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/MAINTAINERS.md
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3334 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/
+-rw-rw-r--   0 root         (0) root         (0)      180 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/creation_payload.json
+-rwxrwxr-x   0 root         (0) root         (0)      292 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/skopeo_copy.sh
+-rw-rw-r--   0 root         (0) root         (0)      635 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/st4sd-runtime-core-image.deploy
+-rw-rw-r--   0 root         (0) root         (0)     1426 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/st4sd-runtime-core-multiarch.deploy
+-rw-rw-r--   0 root         (0) root         (0)      291 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/st4sd-runtime-core-release-tag.deploy
+-rwxrwxr-x   0 root         (0) root         (0)     2445 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/deploy/triggerExternalBuild.sh
+-rw-rw-r--   0 root         (0) root         (0)     2442 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/py310.Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38111 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/appenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/
+-rw-rw-r--   0 root         (0) root         (0)      112 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2342 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2411 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     2891 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/context.py
+-rw-rw-r--   0 root         (0) root         (0)      266 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/exit_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     1899 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/git.py
+-rw-rw-r--   0 root         (0) root         (0)     5140 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/login.py
+-rw-rw-r--   0 root         (0) root         (0)    18498 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/package.py
+-rw-rw-r--   0 root         (0) root         (0)    31124 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/pvep_schema.jsonschema
+-rw-rw-r--   0 root         (0) root         (0)     2300 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/stp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3003 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/codes.py
+-rw-rw-r--   0 root         (0) root         (0)    82296 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/conf.py
+-rw-rw-r--   0 root         (0) root         (0)   148053 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/data.py
+-rw-rw-r--   0 root         (0) root         (0)    44154 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/errors.py
+-rw-rw-r--   0 root         (0) root         (0)    57645 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   126138 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)    85741 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/dosini.py
+-rw-rw-r--   0 root         (0) root         (0)   257676 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/flowir.py
+-rw-rw-r--   0 root         (0) root         (0)   147995 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/
+-rw-rw-r--   0 root         (0) root         (0)      683 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4236 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/hooks.py
+-rw-rw-r--   0 root         (0) root         (0)    36110 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/interface.py
+-rw-rw-r--   0 root         (0) root         (0)     2394 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5562 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    67317 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package/
+-rw-rw-r--   0 root         (0) root         (0)      544 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package/conf/
+-rw-rw-r--   0 root         (0) root         (0)      376 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package/conf/flowir_package.yaml
+-rw-rw-r--   0 root         (0) root         (0)     6144 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package.tar
+-rw-rw-r--   0 root         (0) root         (0)      630 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/rewrite-rules.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4169 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/docker.py
+-rw-rw-r--   0 root         (0) root         (0)   115031 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     5302 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/localtask.py
+-rw-rw-r--   0 root         (0) root         (0)   113107 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/lsf.py
+-rwxrwxr-x   0 root         (0) root         (0)     1414 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/stage-out.sh
+-rw-rw-r--   0 root         (0) root         (0)    13277 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/task_simulator.py
+-rw-rw-r--   0 root         (0) root         (0)    35956 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backends.py
+-rw-rw-r--   0 root         (0) root         (0)    31968 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backends_base.py
+-rw-rw-r--   0 root         (0) root         (0)   118126 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/control.py
+-rw-rw-r--   0 root         (0) root         (0)   104583 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/engine.py
+-rw-rw-r--   0 root         (0) root         (0)     5429 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    26290 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     9481 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/cwl_cmdline.py
+-rw-rw-r--   0 root         (0) root         (0)     8089 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/js.py
+-rw-rw-r--   0 root         (0) root         (0)    20080 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/monitor.py
+-rw-rw-r--   0 root         (0) root         (0)    68147 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/optimizer.py
+-rw-rw-r--   0 root         (0) root         (0)    34954 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/output.py
+-rw-rw-r--   0 root         (0) root         (0)    45119 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/span.py
+-rw-rw-r--   0 root         (0) root         (0)    35543 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/status.py
+-rw-rw-r--   0 root         (0) root         (0)     5622 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3878 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/container_image_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4089 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/rx.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/s3.py
+-rw-rw-r--   0 root         (0) root         (0)    36584 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/service/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/service/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   259382 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/service/db.py
+-rw-rw-r--   0 root         (0) root         (0)     8206 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/service/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     6441 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/
+-rw-rw-r--   0 root         (0) root         (0)      104 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/README
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    58393 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/data.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/fsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/requirement_files/
+-rw-rw-r--   0 root         (0) root         (0)      133 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/requirement_files/requirements_base_3.7.txt
+-rw-rw-r--   0 root         (0) root         (0)      423 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/requirement_files/requirements_base_3.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/requirement_files/requirements_deploy.txt
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/requirement_files/requirements_lsf.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     7054 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/ccommand.py
+-rwxrwxr-x   0 root         (0) root         (0)    11413 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/cexecute.py
+-rwxrwxr-x   0 root         (0) root         (0)     1239 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/checkpackage.py
+-rwxrwxr-x   0 root         (0) root         (0)     4286 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/ctest.py
+-rwxrwxr-x   0 root         (0) root         (0)     2567 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/ecreate.py
+-rwxrwxr-x   0 root         (0) root         (0)     4196 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/eflowir.py
+-rwxrwxr-x   0 root         (0) root         (0)     8094 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/einputs.py
+-rwxrwxr-x   0 root         (0) root         (0)     8246 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/einspect.py
+-rwxrwxr-x   0 root         (0) root         (0)   106990 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/elaunch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17228 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/ememo.py
+-rwxrwxr-x   0 root         (0) root         (0)    46741 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/epatch-apply.py
+-rwxrwxr-x   0 root         (0) root         (0)    33324 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/epatch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17371 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/etest.py
+-rwxrwxr-x   0 root         (0) root         (0)    10419 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/ewrap.py
+-rwxrwxr-x   0 root         (0) root         (0)      821 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/expstatus.sh
+-rw-rw-r--   0 root         (0) root         (0)     3840 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/k8srun.py
+-rwxrwxr-x   0 root         (0) root         (0)   106990 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/launchexperiment.py
+-rwxrwxr-x   0 root         (0) root         (0)    14013 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/lsfsub.py
+-rwxrwxr-x   0 root         (0) root         (0)      262 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/scripts/stp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     4693 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 07:57:42.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10844 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)    11290 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/dont_test_cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     4541 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/reactive_testutils.py
+-rw-rw-r--   0 root         (0) root         (0)    14765 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/saltcurve_paragon.py
+-rw-rw-r--   0 root         (0) root         (0)    11225 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_array_variables.py
+-rw-rw-r--   0 root         (0) root         (0)     6643 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_command.py
+-rw-rw-r--   0 root         (0) root         (0)     7643 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_component.py
+-rw-rw-r--   0 root         (0) root         (0)     2432 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_container_image_uri_manipulation.py
+-rw-rw-r--   0 root         (0) root         (0)    44829 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_control.py
+-rw-rw-r--   0 root         (0) root         (0)     4840 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5588 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_db.py
+-rw-rw-r--   0 root         (0) root         (0)    40697 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_dosini.py
+-rw-rw-r--   0 root         (0) root         (0)    35269 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_dowhile.py
+-rw-rw-r--   0 root         (0) root         (0)    30930 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_engines.py
+-rw-rw-r--   0 root         (0) root         (0)    57435 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_flowir.py
+-rw-rw-r--   0 root         (0) root         (0)    18304 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_graph.py
+-rw-rw-r--   0 root         (0) root         (0)     3286 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_identifier.py
+-rw-rw-r--   0 root         (0) root         (0)    22435 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_interface.py
+-rw-rw-r--   0 root         (0) root         (0)     6059 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     2467 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_memoization.py
+-rw-rw-r--   0 root         (0) root         (0)    13525 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_package_load.py
+-rw-rw-r--   0 root         (0) root         (0)     1673 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_service.py
+-rw-rw-r--   0 root         (0) root         (0)     2085 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/test_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     5739 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tests/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3119 2023-05-15 07:54:36.000000 st4sd-runtime-core-2.0.0a9.dev7/tox.ini
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/.gitignore` & `st4sd-runtime-core-2.0.0a9.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/.travis.yml` & `st4sd-runtime-core-2.0.0a9.dev7/.travis.yml`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/CODE_OF_CONDUCT.md` & `st4sd-runtime-core-2.0.0a9.dev7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/CONTRIBUTING.md` & `st4sd-runtime-core-2.0.0a9.dev7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/Dockerfile` & `st4sd-runtime-core-2.0.0a9.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/LICENSE.md` & `st4sd-runtime-core-2.0.0a9.dev7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/PKG-INFO` & `st4sd-runtime-core-2.0.0a9.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.0.0a9.dev5
+Version: 2.0.0a9.dev7
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/README.MD` & `st4sd-runtime-core-2.0.0a9.dev7/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/deploy/st4sd-runtime-core-image.deploy` & `st4sd-runtime-core-2.0.0a9.dev7/deploy/st4sd-runtime-core-image.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/deploy/st4sd-runtime-core-multiarch.deploy` & `st4sd-runtime-core-2.0.0a9.dev7/deploy/st4sd-runtime-core-multiarch.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/deploy/triggerExternalBuild.sh` & `st4sd-runtime-core-2.0.0a9.dev7/deploy/triggerExternalBuild.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/py310.Dockerfile` & `st4sd-runtime-core-2.0.0a9.dev7/py310.Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/appenv.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/appenv.py`

 * *Files 3% similar despite different names*

```diff
@@ -713,7 +713,71 @@
         try:
             kubernetes.config.load_incluster_config()
         except kubernetes.config.ConfigException:
             # VV: Assumes kubernetes v11.0.0
             kubernetes.config.load_kube_config()
 
         return kubernetes.client.CustomObjectsApi(kubernetes.client.ApiClient())
+
+
+class DockerConfiguration:
+    defaultConf: DockerConfiguration | None = None
+
+    @classmethod
+    def defaultConfiguration(
+            cls,
+            garbage_collect: str | None = None,
+    ) -> DockerConfiguration:
+        """Returns the default docker environment - required for st4sd Docker backend
+
+        Args:
+            garbage_collect: Controls how to delete Containers on task Completion.
+                Choices are "all", "failed", "successful", and (None|"none")
+
+        Exceptions:
+            Raises experiment.errors.ExperimentSetupError if the required environment cannot be configured for some
+            reason. The error object will contain further information on the underlying error
+        """
+        if cls.defaultConf is None:
+            return cls.newDefaultConfiguration(garbage_collect)
+
+        return cls.defaultConf
+
+    @classmethod
+    def newDefaultConfiguration(
+            cls,
+            garbage_collect: str | None = "none",
+    ) -> DockerConfiguration:
+        """Builds the default docker environment - required for st4sd Docker backend
+
+        Arguments:
+            garbage_collect: Controls how to delete Containers on task Completion.
+                Choices are "all", "failed", "successful", and (None|"none")
+
+        Returns
+            The default DockerConfiguration instance
+
+        Raises:
+            experiment.errors.ExperimentSetupError:  if the required environment cannot be configured for some
+                reason. The error object will contain further information on the underlying error
+        """
+        if garbage_collect is None:
+            garbage_collect = "none"
+
+        cls.defaultConf = cls(garbage_collect)
+        return cls.defaultConf
+
+    def __init__(self, garbage_collect: str | None = "none"):
+        valid_garbage_collect = ['successful', 'failed', 'all', 'none']
+        garbage_collect = garbage_collect or "none"
+
+        if garbage_collect not in valid_garbage_collect:
+            raise experiment.model.errors.ExperimentSetupError(
+                "Unable to configure Docker backend", underlyingError=KeyError(
+                    f"garbage_collect={garbage_collect} not one of {valid_garbage_collect}"),
+                instance_dir=None)
+
+        self._garbage_collect = garbage_collect
+
+    @property
+    def garbage_collect(self) -> str:
+        return self._garbage_collect
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/api.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/api.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/configuration.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/context.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/context.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/git.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/git.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/login.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/login.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/package.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,19 @@
         stderr.print(f"Failed to push experiment: {e}")
         raise typer.Exit(code=STPExitCodes.IO_ERROR)
     else:
         if config.settings.verbose:
             stdout.print("Experiment pushed successfully")
             stdout.print(json.dumps(result, indent=2))
 
+    active_context_name = config.settings.default_context
+    url = config.contexts.entries.get(active_context_name).url
+    stdout.print(f"Success! You can find the imported PVEP at:")
+    stdout.print(f"{url}/registry-ui/experiment/{exp_name}")
+
 
 @app.command()
 def update_definition(ctx: typer.Context,
                       path: Path = typer.Option(...,
                                                 help="Path to the file containing the experiment",
                                                 exists=True, readable=True, resolve_path=True, file_okay=True),
                       use_latest_commit: bool = typer.Option(False,
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/pvep_schema.jsonschema` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/pvep_schema.jsonschema`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/cli/stp.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/cli/stp.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/codes.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/codes.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/conf.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/conf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/data.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/errors.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/executors.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,22 @@
 
 import copy
 import sys
 import tempfile
 import threading
 import re
 from abc import ABCMeta, abstractmethod
-from typing import Dict, Optional, Tuple, Union
+from typing import (
+    Dict,
+    Optional,
+    Tuple,
+    Union,
+    Any
+)
+
 import six
 
 import experiment.model.errors
 import experiment.model.frontends.flowir
 import experiment.model.interface
 
 moduleLogger = logging.getLogger("monitor")
@@ -993,16 +1000,16 @@
             target: An instance of an executor.Command subclass
             options: A dictionary of key-value pairs.
                 Valid keys:values are subclass specific.'''
 
         return Executor(target, **options)
 
     def __init__(self,
-                    target,
-                    executable,
+                    target: experiment.model.interface.Command,
+                    executable: str,
                     arguments=None,
                     workingDir=None,
                     environment=None,
                     resolveShellSubstitutions=True,
                     useCommandEnvironment=True):
 
         #If we pass None to superclass it will be set to cwd which is not
@@ -1019,15 +1026,15 @@
         self._target = target
         #We have to resolve any pathless executables as when the chain is executed
         #they will no longer be looked up in the execution environment (as they are not the
         #first argument)
         self.target.updatePath()
 
     @property
-    def target(self):
+    def target(self) -> experiment.model.interface.Command:
 
         '''Returns the target of the executor'''
 
         return self._target
 
     @target.setter
     def target(self, obj):
@@ -1091,15 +1098,15 @@
          return retval
 
     @property
     def workingDir(self):
 
         '''Returns the first defined working dir in the chain'''
 
-        #I don't this can actually be None
+        #I don't think this can actually be None
         if self._workingDir is None:
             return self.target.workingDir
         else:
             return self._applyRewriteRule(self._workingDir)
 
     @property
     def endChain(self):
@@ -1121,15 +1128,19 @@
             self.target.setRewriteRule(rule)
 
 class DockerRun(Executor):
 
     '''Executor for docker'''
 
     @classmethod
-    def executorFromOptions(cls, target, options) -> DockerRun:
+    def executorFromOptions(
+            cls,
+            target: experiment.model.interface.Command,
+            options: Dict[str, Any],
+    ) -> DockerRun:
 
         '''Return an executor based on options
 
         Parameters:
             target: The executors target: A Command subclass instance
             options: A dictionary of key-value pairs.
                 Valid keys:values are subclass specific.'''
@@ -1139,114 +1150,104 @@
             dockerRunArgs = options['docker-args']
 
         executor = DockerRun(target=target,
                              image=options['docker-image'],
                              mounts=[(target.environment['INSTANCE_DIR'], target.environment['INSTANCE_DIR'])],
                              environment=target.environment,
                              resolveShellSubstitutions=False,
-                             runArguments=dockerRunArgs,
-                             shell=False)
-
-        moduleLogger.info("Dockerized command: %s" % executor.commandLine)
+                             use_entrypoint=options.get('docker-use-entrypoint', False),
+                             runArguments=dockerRunArgs)
 
         return executor
 
     def __init__(
-            self, target,
-                 image,
-                 executable="docker",
-                 arguments="",
-                 mounts=[],
-                 runArguments="",
-                 workingDir=None,
-                 shell = True,
-                 resolveShellSubstitutions=True,
-                 environment: Union[Dict[str, str], None] = None,
-                 useCommandEnvironment=True,
-                 addUser=True,
+        self,
+        target,
+        image,
+        executable="docker",
+        arguments="",
+        mounts=[],
+        runArguments="",
+        workingDir=None,
+        use_entrypoint = True,
+        resolveShellSubstitutions=True,
+        environment: Union[Dict[str, str], None] = None,
+        useCommandEnvironment=True,
+        addUser=True,
     ):
 
         '''
         Args:
-           executable: Docker executable to use - defaults to /usr/bin/docker
-           arguments: Docker arguments.
-           image: Docker image
-           mounts: A list of local directories to mount as local dir:container dir
-           workingDir: The working directory for the docker process
-           shell If True the target is executed in a bash shell:
-           runArguments - Extra args to docker run
+            target: the command to run inside the container
+            executable: Docker executable to use - defaults to docker
+            arguments: Docker arguments (i.e. docker <arguments> run)
+            image: Docker image
+            mounts: A list of local directories to mount as local dir:container dir
+            workingDir: The working directory for the docker process
+            use_entrypoint: if set to True will use executable as entrypoint of container
+            runArguments: Arguments to docker run (i.e. docker run <runArguments>)
         '''
 
         super(DockerRun, self).__init__(target,
                             executable=executable,
                             arguments=arguments,
                             workingDir=workingDir,
                             environment=environment,
                             resolveShellSubstitutions=resolveShellSubstitutions,
                             useCommandEnvironment=useCommandEnvironment)
 
         self.image = image
-        self.shell = shell
         self.mounts = mounts
+        self.use_entrypoint = use_entrypoint
 
         runArguments = [runArguments] if runArguments else []
 
         if addUser:
             uid = os.getuid()
             # VV: Set the user to the local user and the group to 0 so that containers do not run as root AND
             # those that follow OpenShift best practices just work out of the box
             #  https://docs.openshift.com/container-platform/4.12/openshift_images/create-images.html
             runArguments.append(f"--user {uid}:0")
 
         if environment:
             for name in environment:
                 runArguments.append(f"--env {name}")
 
+        if self.use_entrypoint:
+            runArguments.append(f'--entrypoint={self.target.executable}')
+
+        # VV: Ask <docker run> to allocate a pseudo-TTY
+        runArguments.append('-t')
+        runArguments.append(f'-w {self.workingDir}')
+
+        # VV: Contains arguments to `docker run` (e.g. --rm)
         self.runArguments = ' '.join(runArguments)
 
     @property
-    def arguments(self):
-
-        # dockerArgs, dockerShellArgs, dockerRunArgs, workingDir, image
-        boilerPlate = r"run " \
-                      r"%s " \
-                      r"%s " \
-                      r"%s " \
-                      r"-t " \
-                      r"-w %s "
-
-        dockerShellArgs = ""
-        if self.shell is True:
-            dockerShellArgs = '--entrypoint /bin/bash'
-
-        boilerPlate = boilerPlate % (
-            self._arguments,
-           dockerShellArgs,
-           self.runArguments,
-           self._workingDir
-        )
+    def arguments(self) -> str:
+        # VV: the format is "<dockerArguments> run <runArguments> <target command-line>"
+        args = [f"{self._arguments} run {self.runArguments}"]
 
         for mount in self.mounts:
-            boilerPlate += "-v %s:%s " % tuple(mount)
-
-        boilerPlate += self.image
-
-        return self._applyRewriteRule(boilerPlate)
-
-    @property
-    def commandLine(self):
-        args = self.arguments
+            args.append("-v %s:%s" % tuple(mount))
 
-        cl = "%s %s " % (self.executable, args)
+        args.append(self.image)
 
-        if self.shell is True:
-            cl += r'-c "%s"' % self.target.commandLine
+        if self.use_entrypoint:
+            # VV: The target executable is in --entrypoint - just use the target arguments here
+            args.append(self.target.arguments)
         else:
-            cl += self.target.commandLine
+            args.append(self.target.commandLine)
 
+        return self._applyRewriteRule(' '.join(args))
+
+    @property
+    def commandLine(self) -> str:
+        # VV: This is <docker> <run [--entrypoint] [--workdir] [-e ...]>
+        cl = f"{self.executable} {self.arguments}"
         return cl
 
 
 class OpenMPIRun(Executor):
 
     '''Executor for openmpi's mpirun'''
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/cwl.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/dosini.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/frontends/flowir.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/frontends/flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/graph.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1521,18 +1521,23 @@
 
         commandDetails = self.commandDetails
         executable = commandDetails['executable']
         rootStorage = self.workflowGraphRef().rootStorage  # type: ExperimentInstanceDirectory
         rootLocation = None if rootStorage is None else rootStorage.location
 
         #TODO: Possibly should be moved
-        if self.resourceManager['config']['backend'] != 'kubernetes':
+        backend_type = self.resourceManager['config']['backend']
+        if backend_type not in ['kubernetes', 'docker']:
             executableChecker = experiment.model.executors.LocalExecutableChecker()
+        elif backend_type == 'kubernetes':
+            executableChecker = experiment.runtime.backends_base.KubernetesExecutableChecker(
+                resourceManager=self.resourceManager)
         else:
-            executableChecker = experiment.runtime.backends_base.KubernetesExecutableChecker(resourceManager=self.resourceManager)
+            executableChecker = experiment.runtime.backends_base.DockerExecutableChecker(
+                resourceManager=self.resourceManager)
 
         #Do not attempt to find pathless executables here.
         #The default is to assuming pathless executable will be found in the environment and only check if explicitly asked
         #In this case it will happend if checkExecutable is called
         try:
             return experiment.model.executors.Command(executable,
                                                             arguments=self.resolveArguments(ignoreErrors=True),
@@ -1920,22 +1925,23 @@
                 command.updateAndCheckExecutable()
                 postCheck = command.executable
 
                 if updateSpecification and (preCheck != postCheck):
                     graphLogger.log(19, 'Updating executable of %s to %s' % (self.identification.identifier, postCheck))
                     self.setOption('#command.executable', postCheck)
 
-                if updateSpecification and (self.resourceManager['config']['backend'] == 'kubernetes'):
-                    img_original = self.resourceManager['kubernetes']['image']
+                if updateSpecification and (self.resourceManager['config']['backend'] in ['kubernetes', 'docker']):
+                    backend_type = self.resourceManager['config']['backend']
+                    img_original = self.resourceManager[backend_type]['image']
                     img_snapshot = experiment.runtime.utilities.container_image_cache.cache_lookup(img_original)
 
                     if img_original != img_snapshot:
-                        graphLogger.log(19, 'Updating kubernetes image of %s to %s' % (
-                            self.identification.identifier, img_snapshot))
-                        self.setOption('#resourceManager.kubernetes.image', img_snapshot)
+                        graphLogger.log(19, 'Updating %s image of %s to %s' % (
+                            backend_type, self.identification.identifier, img_snapshot))
+                        self.setOption(f'#resourceManager.{backend_type}.image', img_snapshot)
             except Exception as e:
                 if ignoreTestExecutablesError:
                     msg = "Check executable found an issue with executable %s, component: %s, environment id: %s=%s -" \
                           " have been instructed to ignore errors, will not raise an exception" % (
                         self.command.executable, self.identification.identifier,
                         self.commandDetails.get('environment', '*NoneDefined*'), self.environment)
                     graphLogger.info(msg)
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/__init__.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/hooks.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/interface.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/hooks/utils.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/interface.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/model/storage.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/model/storage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package/README.MD` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/resources/Template.package.tar` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/resources/Template.package.tar`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/rewrite-rules.json` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/rewrite-rules.json`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/k8s.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
                  postCommands=None,
                  options=None,
                  resourceRequest=None,
                  stdout=sys.stdout,
                  stderr=sys.stderr,
                  splitArgs=True,
                  cacheImage=True,
-                 pollingInterval=30,
+                 pollingInterval: float = 30,
                  archive_path_prefix: str | None = None,
                  garbage_collect: str | None = "none",
                  archive_objects: str | None = "none",
                  template_pod_spec: Dict[str, Any] | None = None,
                  ):
         '''
 
@@ -366,15 +366,15 @@
             stdout: The stdout stream for the job
             stderr: The stderr stream for the job
             splitArgs: Parameter is not inspected, the args are created by splitting the executor.CommandLine using
                 shlex.split()
             cacheImage: If True if the task finishes successfully the image name so if a
                 subsequent Task uses the same image it will only be pulled 'IfNotPresent' regardless of label e.g.
                 'latest'
-            pollingInterval: In miliseconds
+            pollingInterval: Interval to poll status of task (in seconds)
             archive_path_prefix: If k8s is configured to archive objects
                 (appenv.KubernetesConfiguration.archive_objects)
                 it generates the objects "${archive_path_prefix}pods.yaml" and "${archive_path_prefix}job.yaml".
                 if archive_path_prefix is None then it defaults to "${executor.working_dir}/"
             garbage_collect: Controls how to delete Job and Pod objects on task Completion.
                 Choices are "all", "failed", "successful", and "none" (or None literal).
             archive_objects: Controls how to store the Job and Pod objects on task Completion.
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/localtask.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/localtask.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,32 +53,33 @@
                                   shell=shell, **kwargs)
         self._z_launched_date = datetime.datetime.now()
         epoch_submitted = self._z_launched_date.strftime("%d%m%y-%H%M%S")
         for key in ['epoch-submitted', 'epoch-started']:
             idx = self.schedulingData.indexOfColumnWithHeader(key)
             self.schedulingData.matrix[0][idx] = epoch_submitted
 
-        # VV: Ensure that epoch-finished is reflected to the caller of self.wait() after they wake-up
-        def measure_execution_time():
-            try:
-                subprocess.Popen.wait(self)
-            except:
-                self.log.critical("Failed to wait for termination of local task %s."
-                                  " EXCEPTION: %s\n" % (
-                    self.args, traceback.format_exc()
-                ))
-            self._z_finished_date = datetime.datetime.now()
+        threading.Thread(target=self._wait_task_and_set_epoch_finished).start()
+
+    def _wait_task_and_set_epoch_finished(self):
+        """Internal method that waits for task to finish and then sets epoch-finished
 
-            idx = self.schedulingData.indexOfColumnWithHeader('epoch-finished')
-            self.schedulingData.matrix[0][idx] = self._z_finished_date.strftime("%d%m%y-%H%M%S")
+        You inherit localTask and override this method to add your custom logic for waiting the task to complete
+        """
+        # VV: Ensure that epoch-finished is reflected to the caller of self.wait() after they wake-up
+        try:
+            subprocess.Popen.wait(self)
+        except Exception as e:
+            self.log.warning("Failed to wait for termination of local task %s due to %s" % (self.args, e))
+        self._z_finished_date = datetime.datetime.now()
 
-            # VV: Wake up whoever is blocked at .wait()
-            self._z_wait_event.set()
+        idx = self.schedulingData.indexOfColumnWithHeader('epoch-finished')
+        self.schedulingData.matrix[0][idx] = self._z_finished_date.strftime("%d%m%y-%H%M%S")
 
-        threading.Thread(target=measure_execution_time).start()
+        # VV: Wake up whoever is blocked at .wait()
+        self._z_wait_event.set()
 
     def isAlive(self):
 
         retval = True
         self.poll()
         if self.returncode is not None:
             retval = False
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/lsf.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/lsf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/stage-out.sh` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/stage-out.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backend_interfaces/task_simulator.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backend_interfaces/task_simulator.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backends.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,29 @@
 - Configuration management i.e. providing information on valid key/values.
 - Flow facing interfaces to exposed backend specific commands
 - Task Factory Functions (Launchers)'''
 
 from __future__ import print_function
 from __future__ import annotations
 
+import subprocess
 from typing import Optional, List, Dict, cast, TYPE_CHECKING, Any
 
 import experiment.model.errors
 
 if TYPE_CHECKING:
     from experiment.model.interface import InternalRepresentationAttributes
     from experiment.model.data import Job
 
 import logging
 import os
 import pprint
+
+import uuid
+
 from future.utils import raise_with_traceback
 
 import experiment.appenv
 
 import experiment.model.data
 import experiment.model.executors
 import experiment.model.frontends.flowir
@@ -147,29 +151,31 @@
         raise experiment.model.errors.FlowIRInconsistency(
             f"Component {job.identification.identifier} using the docker backend does not specify a "
             f"resourceManager.docker.image or a fallback resourceManager.kubernetes.image",
             flowir=job.configuration)
 
     # Step1. Build the DockerRun executor, it builds a commandline that includes mounts, environment, etc
     executor = experiment.model.executors.DockerRun.executorFromOptions(
-        job.command, options={'docker-image': image, 'docker-args': '--rm'})
+        job.command, options={'docker-image': image, 'docker-use-entrypoint': True})
 
     #Step 2. Create the task
     #The executor defines environment variables for all sub-executors and the task-manager (Global mode)
     #resources: Defines resource requests and backend-specific options
     outputFile = "out.stdout" if outputFile is None else outputFile
     errorFile = "out.stderr" if errorFile is None else errorFile
     outputFile = open(os.path.join(executor.workingDir, outputFile), 'wt')
     errorFile = open(os.path.join(executor.workingDir, errorFile), 'wt')
 
+    label = job.identification.identifier.lower() + "-" + uuid.uuid4().hex[:8]
     return experiment.runtime.backend_interfaces.docker.DockerTask(
         executor=executor,
         stdout=outputFile,
         stderr=errorFile,
-        shell=True)
+        shell=True,
+        label=label)
 
 def KubernetesTaskGenerator(
         componentSpecification: experiment.model.interface.InternalRepresentationAttributes,
         outputFile: str | None = None, errorFile: str | None = None, archive_path_prefix: str | None = None):
 
     '''Creates a k8s task from component specification
 
@@ -375,32 +381,60 @@
         garbage_collect=k8s_garbage_collect, archive_objects=k8s_archive_objects)
 
     if k8s_store_path:
         # VV: Now store the dictionary under @k8s_store_path for use in the future (e.g cexecute.py)
         with open(k8s_store_path, 'w') as f:
             experiment.model.frontends.flowir.yaml_dump(default_k8s.raw_options, f)
 
+
+def DockerInitializer(
+        workflowGraph: experiment.model.graph.WorkflowGraph,
+        k8s_garbage_collect: str | None = None,
+        **kwargs):
+    """Initialises the docker backend
+
+    Args:
+        workflowGraph: a WorkflowGraph instance (currently not used but is part of initializer protocol)
+        k8s_garbage_collect: Controls how to delete Containers on task Completion.
+            Choices are "all", "failed", "successful", and (None|"none")
+
+    Raises:
+        experiment.model.errors.ExperimentSetupError: If unable to initialize Docker backend with appropriate
+          description
+    """
+    experiment.appenv.DockerConfiguration.defaultConfiguration(garbage_collect=k8s_garbage_collect)
+
+    exit_code = subprocess.Popen("docker", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).wait()
+
+    if exit_code != 0:
+        err = ValueError(f"docker command returned exit code {exit_code}")
+        raise experiment.model.errors.ExperimentSetupError(
+            "Docker backend is unavailable", underlyingError=err, instance_dir=None)
+
+
 backendGeneratorMap = {
     'simulator': SimulatorTaskGenerator,
     'lsf': LSFTaskGenerator,
     'local': LocalTaskGenerator,
     'kubernetes': KubernetesTaskGenerator,
     'docker': DockerTaskGenerator,
 }
 
 backendInitializerMap = {
     'lsf': LSFInitializer,
     'kubernetes': KubernetesInitializer,
+    'docker': DockerInitializer,
 }
 
 backendTaskMap = {
     'simulator': experiment.runtime.backend_interfaces.task_simulator.SimulatorTask,
     'lsf': experiment.runtime.backend_interfaces.lsf.Task,
     'local': experiment.runtime.backend_interfaces.localtask.LocalTask,
-    'kubernetes': experiment.runtime.backend_interfaces.k8s.NativeScheduledTask
+    'kubernetes': experiment.runtime.backend_interfaces.k8s.NativeScheduledTask,
+    'docker': experiment.runtime.backend_interfaces.docker.DockerTask,
 }
 
 
 def GenerateTaskFromSpecification(specification  # type: InternalRepresentationAttributes
                                   ):
 
     '''Creates and launches a last given a component specification
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/backends_base.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/backends_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 import experiment.appenv
 import experiment.model.codes
 import experiment.model.errors
 import experiment.model.executors
 import experiment.model.frontends.flowir
 import experiment.model.interface
 import experiment.runtime.backend_interfaces.k8s
+import experiment.runtime.backend_interfaces.docker
 import experiment.runtime.errors
+import experiment.runtime.task
 
 import experiment.runtime.utilities.container_image_cache
 
 if TYPE_CHECKING:
     pass
 
 
@@ -42,15 +44,15 @@
         resourceManager: experiment.model.frontends.flowir.DictFlowIRResourceManager,
         outputFile: str,
         pre: experiment.model.executors.Command | None = None,
         post: experiment.model.executors.Command | None = None,
         label: str | None = None,
         flowKubeEnvironment: Dict[str, Any] | None = None,
         splitArgs: bool = True,
-        pollingInterval: int = 30,
+        pollingInterval: float = 30,
         archive_path_prefix: str | None = None,
 ) -> experiment.runtime.backend_interfaces.k8s.NativeScheduledTask:
     # VV: Set resource requirements to very low, 100 Mebibytes for ram, and 1 CPU unit
 
     resourceManager = experiment.model.frontends.flowir.deep_copy(resourceManager)
 
     # VV: The expression `walltime*60.0` is treated as `active_deadline_seconds` in V1JobSpec, set it to a ludicrous
@@ -84,15 +86,15 @@
                             outputFile,  # type:  str
                             resourceRequest=None,  # type:  Dict[str, Any]
                             pre=None,  # type:  experiment.model.executors.Command
                             post=None,  # type:  experiment.model.executors.Command
                             label=None,  # type:  str
                             flowKubeEnvironment=None,  # type:  Dict[str, Any]
                             splitArgs=True,  # type:  bool,
-                            pollingInterval=30,  # type: int
+                            pollingInterval: float = 30,
                             archive_path_prefix: str | None = None,
                             ):
 
     '''Creates a k8s task from component specification
 
     Assumes the k8s options in component-spec are in DOSINI FORMAT
 
@@ -111,17 +113,21 @@
 
     Set by this function:
     k8s-name, no-default: Set to $COMPONENTNAME
     k8s-flow-id, no-default: Set to experiment FLOWID
     k8s-persistant-volume-claim: default: ....
 
     Args:
+        executor: Command to execute
+        resourceManager: The definition of the backend that will execute the Command
+        outputFile: The path to store the stdout under
         archive_path_prefix: If k8s is configured to archive objects (appenv.KubernetesConfiguration.archive_objects)
             it generates the objects "${archive_path_prefix}pods.yaml" and "${archive_path_prefix}job.yaml".
             if archive_path_prefix is None then it defaults to "${executor.working_dir}/"
+        pollingInterval: Interval to poll status of task (in seconds)
     '''
     #The Tasks name field - generated from the label param - cannot be more than 53 chars in length to meet k8s restrictions
     #This limit is 63 chars but the Task class adds up to 10
     #The prefix 'flow-' is 5 chars
     #The ident is 8 chars
     #This leaves 53-8-5 = 40 chars for the label
     if label is None:
@@ -211,16 +217,15 @@
             garbage_collect = appenv.garbage_collect,
             archive_objects = appenv.archive_objects,
             template_pod_spec=resourceManager.get('kubernetes', {}).get('podSpec')
         )
 
     return task
 
-
-class KubernetesExecutableChecker(experiment.model.interface.ExecutableChecker):
+class ContainerBasedExecutableChecker(experiment.model.interface.ExecutableChecker):
     cache = {}
     # VV: Maps expanded container URIs to the fully resolved, and expanded, image URI which is returned by
     # kubernetes, in the form of pod.status.containerStatuses.imageID. In this context, expanded means that the
     # image URI includes a tag (the default tag is `:latest`).
     image_cache = {}
 
     @classmethod
@@ -255,51 +260,134 @@
         return cls.hash_command(environment, executable, image) in cls.cache
 
     @classmethod
     def get_hashed_command(cls, environment, executable, image):
         # type: (Dict[str, str], str, str) -> str
         return cls.cache[cls.hash_command(environment, executable, image)]
 
-    def __init__(self,  resourceManager: experiment.model.frontends.flowir.DictFlowIRResourceManager):
+    def _create_task_that_checks_executable(
+            self,
+            command: experiment.model.executors.Command,
+            output_path: str,
+            stderr_path: Union[str, None] = None,
+    ) -> experiment.runtime.task.Task:
+        """Creates a task which resolves the executable and writes it to a file
+
+        Override this method
+
+        Arguments:
+            command: The command to run which will check and resolve the executable path
+            output_path: the file in which to store the stdout of task (e.g. resolved path of executable)
+            output_path: the file in which to store the stderr of task (e.g. error messages explaining the failure)
+        Return:
+             a Task
+        """
+        raise NotImplementedError("Must override this method in classes that inherit this class")
+
+    def _get_target_image(self) -> str:
+        """Returns the image that this checkExecutable will target
+
+        Override this method
+
+        Returns:
+            The image that this checkExecutable will target
+        """
+
+        raise NotImplementedError("Must override this method in classes that inherit this class")
+
+    def _set_target_image(self, img: str):
+        """Sets the image that this checkExecutable will target
+
+        Override this method
+
+        Arguments:
+            img: The container image that this executableCheck will target
+        """
+
+        raise NotImplementedError("Must override this method in classes that inherit this class")
+
+    def _explain_executable_check_failure(
+            self,
+            task: experiment.runtime.task.Task,
+            command: experiment.model.executors.Command,
+            remaining_attempts: int,
+            stdout_path: str,
+            stderr_path: Union[str, None] = None,
+    ) -> Tuple[Exception, bool]:
+        """Inspects a task to explain why it was unable to check the executable
+
+        Override this method
+
+        Arguments:
+            task: The task to inspect
+            command: The check executable command that the task ran
+            remaining_attempts: How many times this task may be retried
+            stdout_path: the path to the file that the task stored its stdout in (may not exist)
+            stderr_path: the path to the file that the task stored its stderr in (may not exist)
+
+        Returns:
+            A tuple of an exception explaining the problem and a bool for whether there should be another
+            resubmission (True) or if there is no reason to retry this task again (False)
+        """
+
+        raise NotImplementedError("Must implement this method in classes that inherit this class")
+
+    def _extract_referenced_image_ids(self, task: experiment.runtime.task.Task) -> Dict[str, str]:
+        """Maps the container images that the task used to the full container image url including a digest
+
+        Override this method
+        """
+        raise NotImplementedError("Must override this method in classes that inherit this class")
+
+
+    def __init__(
+            self,
+            resourceManager: experiment.model.frontends.flowir.DictFlowIRResourceManager
+    ):
         '''Initializes the KubernetesExecutableChecker using metadata in component.resourceManager
 
         Args
             resourceManager:
                     Contains the following key-paths
                         - ['kubernetes']['image']
                         - ['kubernetes']['image-pull-secret']
          '''
 
-        self.log = logging.getLogger('backends.k8scheckexe')
+        self.log = logging.getLogger('backends.containerCheckExe')
         self.resourceManager = resourceManager
+        self.resolve_image()
 
+    def resolve_image(self):
         # VV: If a previous executable check involved the referenced image, make sure to use the exact same image id
-        img = self.resourceManager['kubernetes']['image']
-        self.resourceManager['kubernetes']['image'] = experiment.runtime.utilities.container_image_cache.cache_lookup(img)
+        img = self._get_target_image()
+        img = experiment.runtime.utilities.container_image_cache.cache_lookup(img)
+        self._set_target_image(img)
 
     def _findCommand(self, command):
 
-        return experiment.model.executors.Command(executable='which',
-                                                        arguments=command._executable,
-                                                        environment=command._environment,
-                                                        resolveShellSubstitutions=False,
-                                                        resolvePath=False)
+        return experiment.model.executors.Command(
+            executable='which',
+            arguments=command._executable,
+            environment=command._environment,
+            resolveShellSubstitutions=False,
+            resolvePath=False)
 
     def _findAndResolveCommand(self, command):
 
 
         #FIXME:Set environment
 
-        return experiment.model.executors.Command(executable='sh',
-                                                        arguments='-c "readlink -f $(which %s)"' % command._executable,
-                                                        environment=command._environment,
-                                                        resolveShellSubstitutions=False,
-                                                        resolvePath=False)
+        return experiment.model.executors.Command(
+            executable='sh',
+            arguments='-c "readlink -f $(which %s)"' % command._executable,
+            environment=command._environment,
+            resolveShellSubstitutions=False,
+            resolvePath=False)
 
-    def findExecutable(self, command, resolvePath):
+    def findExecutable(self, command: experiment.model.executors.Command, resolvePath: bool) -> Union[str, None]:
 
         '''Finds the Commands executable
 
         A search is performed if
         - The Commands executable is pathless
         - resolvePath is True
 
@@ -312,23 +400,20 @@
 
         Raises:
             ValueError if the executable is:
             - relative
 
         Returns:
             The updated executable path
-                '''
+        '''
 
         findCommand = self._findCommand(command) if not resolvePath else self._findAndResolveCommand(command)
 
         fd, filename = tempfile.mkstemp(dir=command.workingDir)
-        archive_path_prefix = os.path.join(command.workingDir, f"executable-check-{os.path.basename(filename)}-")
-        task = LightWeightKubernetesTaskGenerator(findCommand, resourceManager=self.resourceManager,
-                                       outputFile=filename, label='executable-check',
-                                       splitArgs=False, archive_path_prefix=archive_path_prefix)
+        task = self._create_task_that_checks_executable(findCommand, filename)
         task.wait()
 
         if task.returncode == 0:
             with open(filename) as f:
                 executableWithPath = f.read().strip("\n") or None
         else:
             executableWithPath = None
@@ -341,16 +426,15 @@
                 "Unable to find location of executable %s using command environment %s" % (
                     command._executable, command._environment
                 ))
 
         return executableWithPath
 
 
-    def checkExecutable(self, command):
-        # type: ("Command") -> "experiment.runtime.backend_interfaces.k8s.NativeScheduledTask"
+    def checkExecutable(self, command: experiment.model.executors.Command) -> experiment.runtime.task.Task:
         '''Checks if the executable defined by command exists
 
         Params:
             command: An executors.Command instance
 
         Raise:
             ValueError if the executable is
@@ -360,26 +444,21 @@
             - cannot be executed
         '''
         checkCommand = experiment.model.executors.Command(executable='test',
                                                                 arguments='-x %s' % command._executable,
                                                                 resolveShellSubstitutions=False,
                                                                 resolvePath=False)
         fd, filename = tempfile.mkstemp(dir=command.workingDir)
-        archive_path_prefix = os.path.join(command.workingDir, f"executable-check-{os.path.basename(filename)}-")
-        task = LightWeightKubernetesTaskGenerator(
-            checkCommand, resourceManager=self.resourceManager,
-            outputFile=filename, label='executable-check', splitArgs=False,
-            archive_path_prefix=archive_path_prefix)
+        task = self._create_task_that_checks_executable(checkCommand, filename)
         task.wait()
         os.remove(filename)
 
         if task.returncode != 0:
             msg = "Specified executable at '%s' does not exist or is not executable by user (using environment %s)" % (
-                command._executable,
-                command._environment)
+                command._executable, command._environment)
             self.log.warning(msg)
             raise ValueError(msg)
 
         return task
 
     def findAndCheckExecutable(self, command, resolvePath=False):
 
@@ -402,17 +481,17 @@
             TaskSubmissionError if unable to submit Kubernetes Job that resolves executable path
 
         Returns:
             The updated executable path
         '''
         # VV: If the image has been already used before, opt for the exact same hash, else use the task that is about
         # to be spawned to cache the container image url that was used, including its hash
-        image = experiment.runtime.utilities.container_image_cache.cache_lookup(self.resourceManager['kubernetes']['image'])  # type: str
+        image = experiment.runtime.utilities.container_image_cache.cache_lookup(self._get_target_image())  # type: str
 
-        task = None  # type: Optional[experiment.runtime.backend_interfaces.k8s.NativeScheduledTask]
+        task = None  # type: Optional[experiment.runtime.task.Task]
 
         # VV: Freeze the environment and executable; use this tuple to communicate with the cache
         orig_environment = (command._environment or {}).copy()
         orig_executable = command._executable
 
         if KubernetesExecutableChecker.is_command_hashed(orig_environment, orig_executable, image):
             return KubernetesExecutableChecker.get_hashed_command(orig_environment, orig_executable, image)
@@ -444,71 +523,215 @@
                     executable='sh',
                     arguments="-c 'export CMD_PATH=`readlink -f %s`; echo ${CMD_PATH}; "
                               "test -x ${CMD_PATH} -a -e ${CMD_PATH}'" % command._executable,
                     environment=command.environment,
                     resolveShellSubstitutions=False,
                     resolvePath=False)
 
-            # VV: Sometimes k8s is quirky and drops submitted jobs. Retry up to 2 times
+            # VV: Sometimes backends can be quirky causing tasks to be dropped. Retry up to 2 times
             max_resubmission_attempts = 2
-            resubmission_attempts = max_resubmission_attempts
-
-            k8s_last_reason_failed = None
-            while resubmission_attempts > 0:
+            last_reason_failed = None
+            for resubmission_attempts in range(max_resubmission_attempts):
+                task = None
                 fd, filename = tempfile.mkstemp(dir=command.workingDir)
-                archive_path_prefix = os.path.join(command.workingDir,
-                                                   f"executable-check-{os.path.basename(filename)}-")
-                task = LightWeightKubernetesTaskGenerator(
-                    checkCommand, resourceManager=self.resourceManager,
-                    outputFile=filename, label='executable-check', splitArgs=False,
-                    pollingInterval=2.5, archive_path_prefix=archive_path_prefix,
-                )
-
-                task.wait()
-
-                if task.returncode == 0:
-                    with open(filename) as f:
-                        executablePath = f.read().strip("\n")
-                else:
-                    executablePath = None
-                os.remove(filename)
-
-                if task.returncode == 0:
-                    self.log.info("Found executable in command environment - using %s" % executablePath)
-                    break
-                elif task.exitReason == experiment.model.codes.exitReasons['SubmissionFailed']:
-                    resubmission_attempts -= 1
-                    this_image = self.resourceManager.get('kubernetes', {}).get('image')
-                    try:
-                        why_failed = '. '.join(task.explain_job_failure())
-                    except Exception:
-                        why_failed = 'SubmissionFailed'
-
-                    self.log.info("Job to resolve executable %s using image %s failed to Submit due to "
-                                  "%s, will retry up to %d times" % (
-                        command._executable, this_image, why_failed, resubmission_attempts))
-
-                    k8s_last_reason_failed = ValueError(why_failed)
-                else:
-                    msg = "No executable file exists at '%s' (resolved path: %s) (using command environment %s)" % (
-                        command._executable,  executablePath, command._environment)
-                    self.log.warning(msg)
-                    raise ValueError(msg)
+                fd, filename_stderr = tempfile.mkstemp(dir=command.workingDir)
+                try:
+                    task = self._create_task_that_checks_executable(checkCommand, filename)
+                    task.wait()
+
+                    if task.returncode == 0:
+                        with open(filename) as f:
+                            executablePath = f.read().strip("\n")
+                    else:
+                        executablePath = None
+
+                    if task.returncode == 0 and executablePath:
+                        self.log.info("Found executable in command environment - using %s" % executablePath)
+                        last_reason_failed = None
+                        break
+
+                    last_reason_failed, try_again = self._explain_executable_check_failure(
+                        task, checkCommand, max_resubmission_attempts - resubmission_attempts -1,
+                        filename, filename_stderr)
+
+                    if not try_again:
+                        break
+                except Exception as e:
+                    last_reason_failed = e
+                    continue
+                finally:
+                    os.remove(filename)
+                    os.remove(filename_stderr)
 
             if executablePath in ["", None]:
-                msg = "Job to resolve executable \"%s\" using image \"%s\" failed to Submit %d times" % (
-                      command._executable, self.resourceManager.get('kubernetes', {}).get('image'),
-                      max_resubmission_attempts)
-                raise experiment.runtime.errors.TaskSubmissionError(msg, k8s_last_reason_failed)
+                msg = "Unable to resolve executable \"%s\" using image \"%s\" failed to Submit %d times" % (
+                    command._executable, self._get_target_image(), max_resubmission_attempts)
+                raise experiment.runtime.errors.TaskSubmissionError(msg, last_reason_failed)
 
-        if task:
+        if task is not None:
             # VV: Update the image cache to include the fully-resolved-image-ids that the task used
-            referenced = task.get_referenced_image_ids()
+            referenced = self._extract_referenced_image_ids(task)
             for img in referenced:
                 experiment.runtime.utilities.container_image_cache.cache_register(img, referenced[img])
 
         # VV: Use the fully resolved image id when caching the executable path
         resolved_image = experiment.runtime.utilities.container_image_cache.cache_lookup(image)
-        KubernetesExecutableChecker.cache_command(orig_environment, orig_executable,
-                                                  image, executablePath, resolved_image)
+        self.cache_command(orig_environment, orig_executable, image, executablePath, resolved_image)
 
         return executablePath
+
+
+class KubernetesExecutableChecker(ContainerBasedExecutableChecker):
+    def _create_task_that_checks_executable(
+            self,
+            command: experiment.model.executors.Command,
+            stdout_path: str,
+            stderr_path: Union[str, None] = None,
+    ) -> experiment.runtime.backend_interfaces.k8s.NativeScheduledTask:
+        archive_path_prefix = os.path.join(command.workingDir, f"executable-check-{os.path.basename(stdout_path)}-")
+
+        return LightWeightKubernetesTaskGenerator(
+            command, resourceManager=self.resourceManager,
+            outputFile=stdout_path, label='executable-check', splitArgs=False,
+            pollingInterval=2.5, archive_path_prefix=archive_path_prefix)
+
+    def _get_target_image(self) -> str:
+        return self.resourceManager['kubernetes']['image']
+
+    def _set_target_image(self, img: str):
+        self.resourceManager['kubernetes']['image'] = img
+
+    def _explain_executable_check_failure(
+            self,
+            task: experiment.runtime.backend_interfaces.k8s.NativeScheduledTask,
+            command: experiment.model.executors.Command,
+            remaining_attempts: int,
+            stdout_path: str,
+            stderr_path: Union[str, None] = None,
+    ) -> Tuple[Exception, bool]:
+        if task.exitReason == experiment.model.codes.exitReasons['SubmissionFailed']:
+            this_image = self._get_target_image()
+            try:
+                why_failed = '. '.join(task.explain_job_failure())
+            except Exception:
+                why_failed = 'SubmissionFailed'
+
+            self.log.info("Job to resolve executable %s using image %s failed to Submit due to %s, "
+                          "will retry up to %d times" % (
+                              command._executable, this_image, why_failed, remaining_attempts))
+
+            return  ValueError(why_failed), True
+        elif task.returncode != 0:
+            msg = "Unable to check whether executable '%s' exists (using command environment %s), check executable " \
+                  "task exited with %s. Will not retry" % (
+                command._executable, command._environment, task.returncode)
+            self.log.warning(msg)
+            return ValueError(msg), False
+
+        msg = "Unable to check whether executable '%s' exists (using command environment %s), check executable " \
+              "task exited with reason %s. Will retry up to %d times" % (
+            command._executable, command._environment, task.exitReason, remaining_attempts)
+        self.log.warning(msg)
+        return ValueError(msg), True
+
+    def _extract_referenced_image_ids(
+            self,
+            task: experiment.runtime.backend_interfaces.k8s.NativeScheduledTask
+    ) -> Dict[str, str]:
+        return task.get_referenced_image_ids()
+
+
+class DockerExecutableChecker(ContainerBasedExecutableChecker):
+    def _create_task_that_checks_executable(
+            self,
+            command: experiment.model.executors.Command,
+            stdout_path: str,
+            stderr_path: Union[str, None] = None,
+    ) -> experiment.runtime.backend_interfaces.docker.DockerTask:
+        docker_opts={'docker-image': self._get_target_image(), "docker-args": "--rm", "docker-use-entrypoint": True}
+        executor = experiment.model.executors.DockerRun.executorFromOptions(command, options=docker_opts)
+
+        stderr = open(stderr_path, 'wt') if stderr_path else None
+
+        return experiment.runtime.backend_interfaces.docker.DockerTask(
+            executor, stdout=open(stdout_path, 'wt'), stderr=stderr, shell=True)
+
+    def _get_target_image(self) -> str:
+        return self.resourceManager['docker']['image']
+
+    def _set_target_image(self, img: str):
+        self.resourceManager['docker']['image'] = img
+
+    def _explain_executable_check_failure(
+            self,
+            task: experiment.runtime.backend_interfaces.docker.DockerTask,
+            command: experiment.model.executors.Command,
+            remaining_attempts: int,
+            stdout_path: str,
+            stderr_path: Union[str, None] = None,
+    ) -> Tuple[Exception, bool]:
+        stdout_contents = ""
+        stderr_contents = ""
+
+        try:
+            if os.path.exists(stderr_path):
+                with open(stderr_path, 'rt') as f:
+                    stderr_contents = f.read()
+        except Exception as e:
+            self.log.info(f"Could not get read stderr from {stderr_path} due to {e} - ignoring error")
+
+
+        try:
+            if os.path.exists(stdout_path):
+                with open(stdout_path, 'rt') as f:
+                    stdout_contents = f.read()
+        except Exception as e:
+            self.log.info(f"Could not get read stderr from {stdout_path} due to {e} - ignoring error")
+
+
+        if task.exitReason == experiment.model.codes.exitReasons['SubmissionFailed']:
+            this_image = self._get_target_image()
+            why_failed = 'SubmissionFailed'
+
+            msg = "Container to resolve executable %s using image %s failed to Submit due to %s, " \
+                  "will retry up to %d times" % (command._executable, this_image, why_failed, remaining_attempts)
+
+            if stderr_contents:
+                msg += ". Stderr contents: " + stderr_contents
+            if stdout_contents:
+                msg += ". Stdout contents: " + stdout_contents
+
+
+            self.log.info(msg)
+            return ValueError(msg), True
+        elif task.returncode != 0:
+            msg = "Unable to check whether executable '%s' exists (using command environment %s), check executable " \
+                  "task exited with %s" % (
+                      command._executable, command._environment, task.returncode)
+
+            if stderr_contents:
+                msg += ". Stderr contents: " + stderr_contents
+            if stdout_contents:
+                msg += ". Stdout contents: " + stdout_contents
+
+            msg += " - will not retry"
+
+            self.log.warning(msg)
+            return ValueError(msg), False
+
+        msg = "Unable to check whether executable '%s' exists (using command environment %s), check executable " \
+              "task exited with reason %s. Will retry up to %d times" % (
+                  command._executable, command._environment, task.exitReason, remaining_attempts)
+        if stderr_contents:
+            msg += ". Stderr contents: " + stderr_contents
+        if stdout_contents:
+            msg += ". Stdout contents: " + stdout_contents
+
+        msg += f" - will retry up to {remaining_attempts} times"
+        self.log.warning(msg)
+        return ValueError(msg), True
+
+    def _extract_referenced_image_ids(
+            self,
+            task: experiment.runtime.backend_interfaces.docker.DockerTask
+    ) -> Dict[str, str]:
+        return task.get_referenced_image_ids()
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/control.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/engine.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/engine.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/errors.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/cwl.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/cwl_cmdline.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/cwl_cmdline.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/interpreters/js.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/interpreters/js.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/monitor.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/monitor.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/optimizer.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/optimizer.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/output.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/output.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/span.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/span.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/status.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/status.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/task.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/task.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/container_image_cache.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/container_image_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     """
     image_uri = expand_image_uri(image_uri)
     return _image_cache.get(image_uri, image_uri)
 
 
 def cache_register(image_uri, resolved_image_uri):
     # type: (str, str) -> None
-    """Registers an image_uri with its fully resolved image URI, both areguments are fully expanded
+    """Registers an image_uri with its fully resolved image URI, both arguments are fully expanded
     (see expand_image_uri())
     """
 
     image_uri = expand_image_uri(image_uri)
     resolved_image_uri= expand_image_uri(resolved_image_uri)
 
     _image_cache[image_uri] = resolved_image_uri
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/rx.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/rx.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/utilities/s3.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/utilities/s3.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/runtime/workflow.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/runtime/workflow.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/service/db.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/service/db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/service/errors.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/service/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/settings.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/test.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/test.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/data.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/experiment/utilities/fsearch.py` & `st4sd-runtime-core-2.0.0a9.dev7/python/experiment/utilities/fsearch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/PKG-INFO` & `st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.0.0a9.dev5
+Version: 2.0.0a9.dev7
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/python/st4sd_runtime_core.egg-info/SOURCES.txt` & `st4sd-runtime-core-2.0.0a9.dev7/python/st4sd_runtime_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/ccommand.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/ccommand.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/cexecute.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/cexecute.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/checkpackage.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/checkpackage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/ctest.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/ctest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/ecreate.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/ecreate.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/eflowir.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/eflowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/einputs.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/einputs.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/einspect.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/einspect.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/elaunch.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/elaunch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1261,29 +1261,30 @@
     launchOptions.add_option('--useMemoization', dest='useMemoization', metavar="YES/NO",
                              action="callback", default=False, callback=cb_parse_bool, type=str,
                              help='Enable/disable memoization of the workflow using other cached workflow instances '
                                   'which have been injected into the CDB in the past. '
                                   'also required a valid --mongoEndPoint value. Default is No')
     launchOptions.add_option('--kubernetesGarbageCollect', dest='kubernetesGarbageCollect',
                              choices=["all", "failed", "successful", "none"], default=None, type="choice",
-                             help='Controls how to delete Job and Pod objects after Kubernetes task Completion.')
+                             help='Controls how to delete Job and Pod objects after Kubernetes task Completion. '
+                                  'The Docker backend also uses this option to garbage collect containers.')
     launchOptions.add_option('--kubernetesArchiveObjects', dest='kubernetesArchiveObjects',
                              choices=["all", "failed", "successful", "none"], default=None, type="choice",
                              help=' Controls how to store the Job and Pod objects after Kubernetes task Completion.')
     # VV: Overriding means that we can detect whether the user provided a commandline or not, for the time being
     # we can configure --executionMode to just set --kubernetesGarbageCollect and --kubernetesArchiveObjects
     # and then only use --kubernetesArchiveObjects if it's not `None`
     launchOptions.add_option('--executionMode', dest='executionMode',
-                             choices=['production', 'development', 'debug'], type="choice", default="debug",
+                             choices=['production', 'development', 'debug'], type="choice", default="development",
                              help="Configures default options based on intended execution mode. For example, "
-                                  "'debug' configures flow to never garbage collect Kubernetes objects and always"
-                                  " archive them. "
-                                  "'development' only garbage collects kubernetes objects for successful k8s tasks and"
+                                  "'debug' never garbage collects Kubernetes/docker objects and always"
+                                  " archives them. "
+                                  "'development' garbage collects Kubernetes/docker objects of successful tasks and"
                                   " always archives them. "
-                                  "'production' garbage collects all kubernetes objects for k8s tasks and always "
+                                  "'production' garbage collects all Kubernetes/docker objects of tasks and always "
                                   "archives them. "
                                   "Any command-line options you provide override the settings configured by "
                                   "--executionMode.")
 
     restartGroup.add_option("-r", "--restart", dest="restart",
                             help="Restart at given stage"
                                  "Note this option requires an existing instance is passed to the experiment NOT a package. "
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/ememo.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/ememo.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/epatch-apply.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/epatch-apply.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/epatch.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/epatch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/etest.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/etest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/ewrap.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/ewrap.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/expstatus.sh` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/expstatus.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/k8srun.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/k8srun.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/launchexperiment.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/launchexperiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1261,29 +1261,30 @@
     launchOptions.add_option('--useMemoization', dest='useMemoization', metavar="YES/NO",
                              action="callback", default=False, callback=cb_parse_bool, type=str,
                              help='Enable/disable memoization of the workflow using other cached workflow instances '
                                   'which have been injected into the CDB in the past. '
                                   'also required a valid --mongoEndPoint value. Default is No')
     launchOptions.add_option('--kubernetesGarbageCollect', dest='kubernetesGarbageCollect',
                              choices=["all", "failed", "successful", "none"], default=None, type="choice",
-                             help='Controls how to delete Job and Pod objects after Kubernetes task Completion.')
+                             help='Controls how to delete Job and Pod objects after Kubernetes task Completion. '
+                                  'The Docker backend also uses this option to garbage collect containers.')
     launchOptions.add_option('--kubernetesArchiveObjects', dest='kubernetesArchiveObjects',
                              choices=["all", "failed", "successful", "none"], default=None, type="choice",
                              help=' Controls how to store the Job and Pod objects after Kubernetes task Completion.')
     # VV: Overriding means that we can detect whether the user provided a commandline or not, for the time being
     # we can configure --executionMode to just set --kubernetesGarbageCollect and --kubernetesArchiveObjects
     # and then only use --kubernetesArchiveObjects if it's not `None`
     launchOptions.add_option('--executionMode', dest='executionMode',
-                             choices=['production', 'development', 'debug'], type="choice", default="debug",
+                             choices=['production', 'development', 'debug'], type="choice", default="development",
                              help="Configures default options based on intended execution mode. For example, "
-                                  "'debug' configures flow to never garbage collect Kubernetes objects and always"
-                                  " archive them. "
-                                  "'development' only garbage collects kubernetes objects for successful k8s tasks and"
+                                  "'debug' never garbage collects Kubernetes/docker objects and always"
+                                  " archives them. "
+                                  "'development' garbage collects Kubernetes/docker objects of successful tasks and"
                                   " always archives them. "
-                                  "'production' garbage collects all kubernetes objects for k8s tasks and always "
+                                  "'production' garbage collects all Kubernetes/docker objects of tasks and always "
                                   "archives them. "
                                   "Any command-line options you provide override the settings configured by "
                                   "--executionMode.")
 
     restartGroup.add_option("-r", "--restart", dest="restart",
                             help="Restart at given stage"
                                  "Note this option requires an existing instance is passed to the experiment NOT a package. "
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/scripts/lsfsub.py` & `st4sd-runtime-core-2.0.0a9.dev7/scripts/lsfsub.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/setup.py` & `st4sd-runtime-core-2.0.0a9.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/conftest.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/dont_test_cwl.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/dont_test_cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/reactive_testutils.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/reactive_testutils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/saltcurve_paragon.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/saltcurve_paragon.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_array_variables.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_array_variables.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_command.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_component.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_container_image_uri_manipulation.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_container_image_uri_manipulation.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_control.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_data.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_db.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_dosini.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_dowhile.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_dowhile.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_engines.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_flowir.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_graph.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_identifier.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_interface.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_k8s.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_memoization.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_memoization.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_package_load.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_package_load.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_service.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/test_settings.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tests/utils.py` & `st4sd-runtime-core-2.0.0a9.dev7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev5/tox.ini` & `st4sd-runtime-core-2.0.0a9.dev7/tox.ini`

 * *Files identical despite different names*

