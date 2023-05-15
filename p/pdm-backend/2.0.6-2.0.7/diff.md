# Comparing `tmp/pdm_backend-2.0.6.tar.gz` & `tmp/pdm_backend-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.0.6.tar", last modified: Mon Apr 10 11:46:53 2023, max compression
+gzip compressed data, was "pdm_backend-2.0.7.tar", last modified: Mon May 15 03:57:50 2023, max compression
```

## Comparing `pdm_backend-2.0.6.tar` & `pdm_backend-2.0.7.tar`

### file list

```diff
@@ -1,219 +1,180 @@
--rw-r--r--   0        0        0     1067 2023-04-10 11:46:39.233671 pdm_backend-2.0.6/LICENSE
--rw-r--r--   0        0        0     1725 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/README.md
--rw-r--r--   0        0        0     2271 2023-04-10 11:46:53.281793 pdm_backend-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     3282 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      661 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3265 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9606 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5115 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     7928 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    38937 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16469 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16315 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    19827 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0     1491 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/LICENSE
--rw-r--r--   0        0        0    15922 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/LICENSE.txt
--rw-r--r--   0        0        0      589 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/__init__.py
--rw-r--r--   0        0        0       30 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/__main__.py
--rw-r--r--   0        0        0        0 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/__init__.py
--rw-r--r--   0        0        0     1491 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/LICENSE
--rw-r--r--   0        0        0     8769 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__init__.py
--rw-r--r--   0        0        0      312 2023-04-10 11:46:39.237671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/__main__.py
--rw-r--r--   0        0        0    29451 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft04.py
--rw-r--r--   0        0        0     7661 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft06.py
--rw-r--r--   0        0        0     4222 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/draft07.py
--rw-r--r--   0        0        0     1612 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/exceptions.py
--rw-r--r--   0        0        0    12576 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/generator.py
--rw-r--r--   0        0        0      920 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/indent.py
--rw-r--r--   0        0        0     5527 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py
--rw-r--r--   0        0        0       19 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/fastjsonschema/version.py
--rw-r--r--   0        0        0     1812 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/_vendor/vendoring_instructions.rst
--rw-r--r--   0        0        0     8721 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/api.py
--rw-r--r--   0        0        0     8626 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/cli.py
--rw-r--r--   0        0        0    11263 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1634 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/errors.py
--rw-r--r--   0        0        0     1153 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     8756 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/formats.py
--rw-r--r--   0        0        0     4183 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/__init__.py
--rw-r--r--   0        0        0      807 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/distutils.schema.json
--rw-r--r--   0        0        0    11372 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/plugins/setuptools.schema.json
--rw-r--r--   0        0        0      997 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/NOTICE.template
--rw-r--r--   0        0        0     4718 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__init__.py
--rw-r--r--   0        0        0       61 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/__main__.py
--rw-r--r--   0        0        0      101 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/api-notice.template
--rw-r--r--   0        0        0      145 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli-notice.template
--rw-r--r--   0        0        0     2938 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/cli.py
--rw-r--r--   0        0        0     1038 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pre_compile/main_file.template
--rw-r--r--   0        0        0    11087 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/project_metadata.schema.json
--rw-r--r--   0        0        0       27 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/py.typed
--rw-r--r--   0        0        0     2124 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/pyproject_toml.schema.json
--rw-r--r--   0        0        0      821 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/types.py
--rw-r--r--   0        0        0      624 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/__init__.py
--rw-r--r--   0        0        0       61 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/__main__.py
--rw-r--r--   0        0        0      222 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/vendoring/cli.py
--rw-r--r--   0        0        0       97 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    11879 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9412 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/config.py
--rw-r--r--   0        0        0     4063 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      436 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4069 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6364 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     4894 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10064 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0      759 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14958 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3596 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     7080 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    10573 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/__init__.py
--rw-r--r--   0        0        0      747 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/conftest.py
--rw-r--r--   0        0        0      856 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-license/src/foo_module.py
-lrwxr-xr-x   0        0        0        0 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-04-10 11:46:39.241671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      555 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0    16264 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_api.py
--rw-r--r--   0        0        0     5324 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_metadata.py
--rw-r--r--   0        0        0      311 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_utils.py
--rw-r--r--   0        0        0     1176 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/test_wheel.py
--rw-r--r--   0        0        0      598 2023-04-10 11:46:39.245671 pdm_backend-2.0.6/tests/testutils.py
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/LICENSE
+-rw-r--r--   0        0        0     1725 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/README.md
+-rw-r--r--   0        0        0     2271 2023-05-15 03:57:50.543192 pdm_backend-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3282 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      661 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3265 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9606 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5115 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     7928 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    38937 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16469 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16315 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    19827 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0       70 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    11746 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9411 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     4063 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      452 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4069 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6364 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     4894 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0    10064 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0      759 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0    14958 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/macosx_platform.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3604 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     7080 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    10581 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      856 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-license/src/foo_module.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-version/README.md
+lrwxr-xr-x   0        0        0        0 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      555 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0    16264 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_metadata.py
+-rw-r--r--   0        0        0      311 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_wheel.py
+-rw-r--r--   0        0        0      598 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/testutils.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.0.7/PKG-INFO
```

### Comparing `pdm_backend-2.0.6/LICENSE` & `pdm_backend-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/README.md` & `pdm_backend-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/pyproject.toml` & `pdm_backend-2.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.0.6"
+version = "2.0.7"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/__init__.py` & `pdm_backend-2.0.7/src/pdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/__about__.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/requirements.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import pdm.backend._vendor.packaging.markers as pkg_markers
 import pdm.backend._vendor.packaging.requirements as pkg_requirements
 import pdm.backend._vendor.packaging.specifiers as pkg_specifiers
 import pdm.backend._vendor.packaging.version as pkg_version
 
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 
 class ConfigurationError(Exception):
     '''Error in the backend metadata.'''
     def __init__(self, msg: str, *, key: str | None = None):
         super().__init__(msg)
         self._key = key
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/api.py` & `pdm_backend-2.0.7/src/pdm/backend/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,250 +1,259 @@
-"""
-Retrieve JSON schemas for validating dicts representing a ``pyproject.toml`` file.
-"""
-import json
-import logging
+from __future__ import annotations
+
+import glob
+import os
 import sys
-from enum import Enum
-from functools import partial, reduce
-from itertools import chain
-from types import MappingProxyType, ModuleType
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Iterator,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
-
-from . import errors, formats
-from ._vendor import fastjsonschema as FJS
-from .error_reporting import detailed_errors
-from .extra_validations import EXTRA_VALIDATIONS
-from .types import FormatValidationFn, Schema, ValidationFn
-
-_logger = logging.getLogger(__name__)
-_chain_iter = chain.from_iterable
-
-if TYPE_CHECKING:  # pragma: no cover
-    from .plugins import PluginWrapper  # noqa
-
-
-try:  # pragma: no cover
-    if sys.version_info[:2] < (3, 7) or TYPE_CHECKING:  # See #22
-        from importlib_resources import files
-    else:
-        from importlib.resources import files
-
-    def read_text(package: Union[str, ModuleType], resource) -> str:
-        return files(package).joinpath(resource).read_text(encoding="utf-8")
-
-except ImportError:  # pragma: no cover
-    from importlib.resources import read_text
-
-
-T = TypeVar("T", bound=Mapping)
-AllPlugins = Enum("AllPlugins", "ALL_PLUGINS")
-ALL_PLUGINS = AllPlugins.ALL_PLUGINS
-
-TOP_LEVEL_SCHEMA = "pyproject_toml"
-PROJECT_TABLE_SCHEMA = "project_metadata"
-
-
-def _get_public_functions(module: ModuleType) -> Mapping[str, FormatValidationFn]:
-    return {
-        fn.__name__.replace("_", "-"): fn
-        for fn in module.__dict__.values()
-        if callable(fn) and not fn.__name__.startswith("_")
-    }
-
-
-FORMAT_FUNCTIONS = MappingProxyType(_get_public_functions(formats))
-
-
-def load(name: str, package: str = __package__, ext: str = ".schema.json") -> Schema:
-    """Load the schema from a JSON Schema file.
-    The returned dict-like object is immutable.
-    """
-    return Schema(json.loads(read_text(package, f"{name}{ext}")))
+from pathlib import Path
+from typing import Any, TypeVar
 
+from pdm.backend._vendor import tomli_w
+from pdm.backend._vendor.pyproject_metadata import ConfigurationError, StandardMetadata
+from pdm.backend.exceptions import ConfigError, ValidationError
+from pdm.backend.structures import Table
+from pdm.backend.utils import find_packages_iter
 
-def load_builtin_plugin(name: str) -> Schema:
-    return load(name, f"{__package__}.plugins")
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import pdm.backend._vendor.tomli as tomllib
 
+T = TypeVar("T")
 
-class SchemaRegistry(Mapping[str, Schema]):
-    """Repository of parsed JSON Schemas used for validating a ``pyproject.toml``.
 
-    During instantiation the schemas equivalent to PEP 517, PEP 518 and PEP 621
-    will be combined with the schemas for the ``tool`` subtables provided by the
-    plugins.
+class Config:
+    """The project config object for pdm backend.
 
-    Since this object work as a mapping between each schema ``$id`` and the schema
-    itself, all schemas provided by plugins **MUST** have a top level ``$id``.
-    """
+    Parameters:
+        root: The root directory of the project
+        data: The parsed pyproject.toml data
 
-    def __init__(self, plugins: Sequence["PluginWrapper"] = ()):
-        self._schemas: Dict[str, Tuple[str, str, Schema]] = {}
-        # (which part of the TOML, who defines, schema)
-
-        top_level = cast(dict, load(TOP_LEVEL_SCHEMA))  # Make it mutable
-        self._spec_version = top_level["$schema"]
-        top_properties = top_level["properties"]
-        tool_properties = top_properties["tool"].setdefault("properties", {})
-
-        # Add PEP 621
-        project_table_schema = load(PROJECT_TABLE_SCHEMA)
-        self._ensure_compatibility(PROJECT_TABLE_SCHEMA, project_table_schema)
-        sid = project_table_schema["$id"]
-        top_level["project"] = {"$ref": sid}
-        origin = f"{__name__} - project metadata"
-        self._schemas = {sid: ("project", origin, project_table_schema)}
-
-        # Add tools using Plugins
-
-        for plugin in plugins:
-            pid, tool, schema = plugin.id, plugin.tool, plugin.schema
-            if plugin.tool in tool_properties:
-                _logger.warning(f"{plugin.id} overwrites `tool.{plugin.tool}` schema")
-            else:
-                _logger.info(f"{pid} defines `tool.{tool}` schema")
-            sid = self._ensure_compatibility(tool, schema)["$id"]
-            tool_properties[tool] = {"$ref": sid}
-            self._schemas[sid] = (f"tool.{tool}", pid, schema)
-
-        self._main_id = sid = top_level["$id"]
-        main_schema = Schema(top_level)
-        origin = f"{__name__} - build metadata"
-        self._schemas[sid] = ("<$ROOT>", origin, main_schema)
-
-    @property
-    def spec_version(self) -> str:
-        """Version of the JSON Schema spec in use"""
-        return self._spec_version
-
-    @property
-    def main(self) -> str:
-        """Top level schema for validating a ``pyproject.toml`` file"""
-        return self._main_id
-
-    def _ensure_compatibility(self, reference: str, schema: Schema) -> Schema:
-        if "$id" not in schema:
-            raise errors.SchemaMissingId(reference)
-        sid = schema["$id"]
-        if sid in self._schemas:
-            raise errors.SchemaWithDuplicatedId(sid)
-        version = schema.get("$schema")
-        if version and version != self.spec_version:
-            raise errors.InvalidSchemaVersion(reference, version, self.spec_version)
-        return schema
-
-    def __getitem__(self, key: str) -> Schema:
-        return self._schemas[key][-1]
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(self._schemas)
-
-    def __len__(self) -> int:
-        return len(self._schemas)
-
-
-class RefHandler(Mapping[str, Callable[[str], Schema]]):
-    """:mod:`fastjsonschema` allows passing a dict-like object to load external schema
-    ``$ref``s. Such objects map the URI schema (e.g. ``http``, ``https``, ``ftp``)
-    into a function that receives the schema URI and returns the schema (as parsed JSON)
-    (otherwise :mod:`urllib` is used and the URI is assumed to be a valid URL).
-    This class will ensure all the URIs are loaded from the local registry.
+    Attributes:
+        metadata (Metadata): The project metadata from the `project` table
+        build_config (BuildConfig): The build config from the `tool.pdm.build` table
     """
 
-    def __init__(self, registry: Mapping[str, Schema]):
-        self._uri_schemas = ["http", "https"]
-        self._registry = registry
-
-    def __contains__(self, key) -> bool:
-        return_val = isinstance(key, str)
-        if return_val and key not in self._uri_schemas:
-            self._uri_schemas.append(key)
-        return return_val
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(self._uri_schemas)
-
-    def __len__(self):
-        return len(self._uri_schemas)
-
-    def __getitem__(self, key: str) -> Callable[[str], Schema]:
-        """All the references should be retrieved from the registry"""
-        return self._registry.__getitem__
-
-
-class Validator:
-    def __init__(
-        self,
-        plugins: Union[Sequence["PluginWrapper"], AllPlugins] = ALL_PLUGINS,
-        format_validators: Mapping[str, FormatValidationFn] = FORMAT_FUNCTIONS,
-        extra_validations: Sequence[ValidationFn] = EXTRA_VALIDATIONS,
-    ):
-        self._code_cache: Optional[str] = None
-        self._cache: Optional[ValidationFn] = None
-        self._schema: Optional[Schema] = None
-
-        # Let's make the following options readonly
-        self._format_validators = MappingProxyType(format_validators)
-        self._extra_validations = tuple(extra_validations)
+    def __init__(self, root: Path, data: dict[str, Any]) -> None:
+        self.validate(data, root)
+        self.root = root
+        self.data = data
+        self.metadata = Metadata(data["project"])
+        self.build_config = BuildConfig(
+            root, data.setdefault("tool", {}).get("pdm", {}).get("build", {})
+        )
+
+    def to_coremetadata(self) -> str:
+        """Return the metadata as a Core Metadata string."""
+        metadata = StandardMetadata.from_pyproject(self.data, project_dir=self.root)
+        return str(metadata.as_rfc822())
+
+    @classmethod
+    def validate(cls, data: dict[str, Any], root: Path) -> None:
+        """Validate the pyproject.toml data."""
+        try:
+            StandardMetadata.from_pyproject(data, project_dir=root)
+        except ConfigurationError as e:
+            raise ValidationError(e.args[0], e.key) from e
+
+    @classmethod
+    def from_pyproject(cls, root: str | Path) -> Config:
+        """Load the pyproject.toml file from the given project root."""
+        root = Path(root)
+        pyproject = root / "pyproject.toml"
+        if not pyproject.exists():
+            raise ConfigError("pyproject.toml not found")
+        with pyproject.open("rb") as fp:
+            try:
+                data = tomllib.load(fp)
+            except tomllib.TOMLDecodeError as e:
+                raise ConfigError(f"Invalid pyproject.toml file: {e}") from e
+        return cls(root, data)
+
+    def write_to(self, path: str | Path) -> None:
+        """Write the pyproject.toml file to the given path."""
+        with open(path, "wb") as fp:
+            tomli_w.dump(self.data, fp)
+
+    def for_hook(self, name: str) -> dict[str, Any]:
+        """Return the config data for the given hook."""
+        return self.build_config.get("hooks", {}).get(name, {})
+
+    def convert_package_paths(self) -> dict[str, list | dict]:
+        """Return a {package_dir, packages, package_data, exclude_package_data} dict."""
+        packages = []
+        py_modules = []
+        package_data = {"": ["*"]}
+        exclude_package_data: dict[str, list[str]] = {}
+        package_dir = self.build_config.package_dir
+        includes = self.build_config.includes
+        excludes = self.build_config.excludes
+
+        src_dir = Path(package_dir or ".")
+        if not includes:
+            packages = list(
+                find_packages_iter(
+                    package_dir or ".",
+                    exclude=["tests", "tests.*"],
+                    src=str(src_dir),
+                )
+            )
+            if not packages:
+                py_modules = [path.name[:-3] for path in src_dir.glob("*.py")]
+        else:
+            packages_set = set()
+            includes = includes[:]
+            for include in includes[:]:
+                if include.replace("\\", "/").endswith("/*"):
+                    include = include[:-2]
+                if "*" not in include and os.path.isdir(include):
+                    dir_name = include.rstrip("/\\")
+                    temp = list(find_packages_iter(dir_name, src=package_dir or "."))
+                    if os.path.isfile(os.path.join(dir_name, "__init__.py")):
+                        temp.insert(0, dir_name)
+                    packages_set.update(temp)
+                    includes.remove(include)
+            packages[:] = list(packages_set)
+            for include in includes:
+                for path in glob.glob(include, recursive=True):
+                    if "/" not in path.lstrip("./") and path.endswith(".py"):
+                        # Only include top level py modules
+                        py_modules.append(path.lstrip("./")[:-3])
+                if include.endswith(".py"):
+                    continue
+                for package in packages:
+                    relpath = os.path.relpath(include, package)
+                    if not relpath.startswith(".."):
+                        package_data.setdefault(package, []).append(relpath)
+            for exclude in excludes:
+                for package in packages:
+                    relpath = os.path.relpath(exclude, package)
+                    if not relpath.startswith(".."):
+                        exclude_package_data.setdefault(package, []).append(relpath)
+        if packages and py_modules:
+            raise ConfigError("Can't specify packages and py_modules at the same time.")
+        return {
+            "package_dir": {"": package_dir} if package_dir else {},
+            "packages": packages,
+            "py_modules": py_modules,
+            "package_data": package_data,
+            "exclude_package_data": exclude_package_data,
+        }
 
-        if plugins is ALL_PLUGINS:
-            from .plugins import list_from_entry_points
 
-            self._plugins = tuple(list_from_entry_points())
-        else:
-            self._plugins = tuple(plugins)  # force immutability / read only
+class Metadata(Table):
+    """The project metadata table"""
+
+    @property
+    def readme_file(self) -> str | None:
+        """The readme file path, if not exists, returns None"""
+        readme = self.get("readme")
+        if not readme:
+            return None
+        if isinstance(readme, str):
+            return readme
+        if isinstance(readme, dict) and "file" in readme:
+            return readme["file"]
+        return None
 
-        self._schema_registry = SchemaRegistry(self._plugins)
-        self.handlers = RefHandler(self._schema_registry)
+    @property
+    def license_files(self) -> dict[str, list[str]]:
+        """The license files configuration"""
+        subtable_files = None
+        if (
+            "license" in self
+            and isinstance(self["license"], dict)
+            and "files" in self["license"]
+        ):
+            subtable_files = self["license"]["files"]
+        if "license-files" not in self:
+            if subtable_files is not None:
+                return {"paths": [self["license"]["file"]]}
+            return {
+                "globs": [
+                    "LICENSES/*",
+                    "LICEN[CS]E*",
+                    "COPYING*",
+                    "NOTICE*",
+                    "AUTHORS*",
+                ]
+            }
+        if subtable_files is not None:
+            raise ValidationError(
+                "license-files",
+                "Can't specify both 'license.files' and 'license-files' fields",
+            )
+        rv = self["license-files"]
+        valid_keys = {"globs", "paths"} & set(rv)
+        if len(valid_keys) == 2:
+            raise ValidationError(
+                "license-files", "Can't specify both 'paths' and 'globs'"
+            )
+        if not valid_keys:
+            raise ValidationError("license-files", "Must specify 'paths' or 'globs'")
+        return rv
 
     @property
-    def registry(self) -> SchemaRegistry:
-        return self._schema_registry
+    def entry_points(self) -> dict[str, dict[str, str]]:
+        """The entry points mapping"""
+        entry_points: dict[str, dict[str, str]] = self.get("entry-points", {})
+        if "scripts" in self:
+            entry_points["console_scripts"] = self["scripts"]
+        if "gui-scripts" in self:
+            entry_points["gui_scripts"] = self["gui-scripts"]
+        return entry_points
+
+
+class BuildConfig(Table):
+    """The `[tool.pdm.build]` table"""
+
+    def __init__(self, root: Path, data: dict[str, Any]) -> None:
+        self.root = root
+        super().__init__(data)
 
     @property
-    def schema(self) -> Schema:
-        """Top level ``pyproject.toml`` JSON Schema"""
-        return Schema({"$ref": self._schema_registry.main})
+    def custom_hook(self) -> str | None:
+        """The relative path to the custom hook or None if not exists"""
+        script = self.get("custom-hook", "pdm_build.py")
+        if (self.root / script).exists():
+            return script
+        return None
 
     @property
-    def extra_validations(self) -> Sequence[ValidationFn]:
-        """List of extra validation functions that run after the JSON Schema check"""
-        return self._extra_validations
+    def includes(self) -> list[str]:
+        """The includes setting"""
+        return self.get("includes", [])
 
     @property
-    def formats(self) -> Mapping[str, FormatValidationFn]:
-        """Mapping between JSON Schema formats and functions that validates them"""
-        return self._format_validators
+    def source_includes(self) -> list[str]:
+        """The source-includes setting"""
+        return self.get("source-includes", [])
 
     @property
-    def generated_code(self) -> str:
-        if self._code_cache is None:
-            fmts = dict(self.formats)
-            self._code_cache = FJS.compile_to_code(self.schema, self.handlers, fmts)
+    def excludes(self) -> list[str]:
+        """The excludes setting"""
+        return self.get("excludes", [])
 
-        return self._code_cache
+    @property
+    def run_setuptools(self) -> bool:
+        """Whether to run setuptools"""
+        return self.get("run-setuptools", False)
 
-    def __getitem__(self, schema_id: str) -> Schema:
-        """Retrieve a schema from registry"""
-        return self._schema_registry[schema_id]
+    @property
+    def package_dir(self) -> str:
+        """A directory that will be used to looking for packages."""
+        default = "src" if self.root.joinpath("src").exists() else ""
+        return self.get("package-dir", default)
 
-    def __call__(self, pyproject: T) -> T:
-        if self._cache is None:
-            compiled = FJS.compile(self.schema, self.handlers, dict(self.formats))
-            fn = partial(compiled, custom_formats=self._format_validators)
-            self._cache = cast(ValidationFn, fn)
+    @property
+    def is_purelib(self) -> bool:
+        """If not explicitly set, the project is considered to be non-pure
+        if `build` exists.
+        """
+        return self.get("is-purelib", not bool(self.run_setuptools))
 
-        with detailed_errors():
-            self._cache(pyproject)
-        return reduce(lambda acc, fn: fn(acc), self.extra_validations, pyproject)
+    @property
+    def editable_backend(self) -> str:
+        """Currently only two backends are supported:
+        - editables: Proxy modules via editables
+        - path: the legacy .pth file method(default)
+        """
+        return self.get("editable-backend", "path")
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/_vendor/validate_pyproject/error_reporting.py` & `pdm_backend-2.0.7/src/pdm/backend/wheel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,318 +1,281 @@
+from __future__ import annotations
+
+import csv
+import hashlib
 import io
-import json
-import logging
 import os
-import re
-from contextlib import contextmanager
-from textwrap import indent, wrap
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Union, cast
-
-from ._vendor.fastjsonschema import JsonSchemaValueException
-
-_logger = logging.getLogger(__name__)
-
-_MESSAGE_REPLACEMENTS = {
-    "must be named by propertyName definition": "keys must be named by",
-    "one of contains definition": "at least one item that matches",
-    " same as const definition:": "",
-    "only specified items": "only items matching the definition",
-}
-
-_SKIP_DETAILS = (
-    "must not be empty",
-    "is always invalid",
-    "must not be there",
+import shutil
+import stat
+import sys
+import tempfile
+import time
+import zipfile
+from base64 import urlsafe_b64encode
+from pathlib import Path
+from typing import IO, Any, Iterable, Mapping, NamedTuple, cast
+
+from pdm.backend._vendor.packaging import tags
+from pdm.backend._vendor.packaging.specifiers import SpecifierSet
+from pdm.backend._vendor.packaging.utils import canonicalize_name
+from pdm.backend.base import Builder
+from pdm.backend.hooks import Context
+from pdm.backend.hooks.setuptools import SetuptoolsBuildHook
+from pdm.backend.utils import (
+    expand_vars,
+    get_abi_tag,
+    get_platform,
+    safe_version,
+    to_filename,
 )
 
-_NEED_DETAILS = {"anyOf", "oneOf", "anyOf", "contains", "propertyNames", "not", "items"}
-
-_CAMEL_CASE_SPLITTER = re.compile(r"\W+|([A-Z][^A-Z\W]*)")
-_IDENTIFIER = re.compile(r"^[\w_]+$", re.I)
-
-_TOML_JARGON = {
-    "object": "table",
-    "property": "key",
-    "properties": "keys",
-    "property names": "keys",
-}
-
-
-class ValidationError(JsonSchemaValueException):
-    """Report violations of a given JSON schema.
-
-    This class extends :exc:`~fastjsonschema.JsonSchemaValueException`
-    by adding the following properties:
-
-    - ``summary``: an improved version of the ``JsonSchemaValueException`` error message
-      with only the necessary information)
-
-    - ``details``: more contextual information about the error like the failing schema
-      itself and the value that violates the schema.
-
-    Depending on the level of the verbosity of the ``logging`` configuration
-    the exception message will be only ``summary`` (default) or a combination of
-    ``summary`` and ``details`` (when the logging level is set to :obj:`logging.DEBUG`).
-    """
-
-    summary = ""
-    details = ""
-    _original_message = ""
-
-    @classmethod
-    def _from_jsonschema(cls, ex: JsonSchemaValueException):
-        formatter = _ErrorFormatting(ex)
-        obj = cls(str(formatter), ex.value, formatter.name, ex.definition, ex.rule)
-        debug_code = os.getenv("JSONSCHEMA_DEBUG_CODE_GENERATION", "false").lower()
-        if debug_code != "false":  # pragma: no cover
-            obj.__cause__, obj.__traceback__ = ex.__cause__, ex.__traceback__
-        obj._original_message = ex.message
-        obj.summary = formatter.summary
-        obj.details = formatter.details
-        return obj
-
-
-@contextmanager
-def detailed_errors():
-    try:
-        yield
-    except JsonSchemaValueException as ex:
-        raise ValidationError._from_jsonschema(ex) from None
-
-
-class _ErrorFormatting:
-    def __init__(self, ex: JsonSchemaValueException):
-        self.ex = ex
-        self.name = f"`{self._simplify_name(ex.name)}`"
-        self._original_message = self.ex.message.replace(ex.name, self.name)
-        self._summary = ""
-        self._details = ""
-
-    def __str__(self) -> str:
-        if _logger.getEffectiveLevel() <= logging.DEBUG and self.details:
-            return f"{self.summary}\n\n{self.details}"
-
-        return self.summary
+if sys.version_info < (3, 8):
+    from importlib_metadata import version as get_version
+else:
+    from importlib.metadata import version as get_version
+
+WHEEL_FILE_FORMAT = """\
+Wheel-Version: 1.0
+Generator: pdm-backend ({version})
+Root-Is-Purelib: {is_purelib}
+Tag: {tag}
+"""
+
+# Fix the date time for reproducible builds
+try:
+    _env_date = time.gmtime(int(os.environ["SOURCE_DATE_EPOCH"]))[:6]
+except (ValueError, KeyError):
+    ZIPINFO_DATE_TIME = (2016, 1, 1, 0, 0, 0)
+else:
+    if _env_date[0] < 1980:
+        raise ValueError("zipinfo date can't be earlier than 1980")
+    ZIPINFO_DATE_TIME = _env_date
+
+
+def _open_for_write(path: str | Path) -> IO[str]:
+    """A simple wrapper around open() that preserves the line ending styles"""
+    return open(path, "w", newline="", encoding="utf-8")
+
+
+class RecordEntry(NamedTuple):
+    relpath: str
+    hash_digest: str
+    size: str
+
+
+class WheelBuilder(Builder):
+    target = "wheel"
+    hooks = Builder.hooks + [SetuptoolsBuildHook()]
+
+    def __init__(
+        self, location: str | Path, config_settings: Mapping[str, Any] | None = None
+    ) -> None:
+        super().__init__(location, config_settings)
+        self.__tag: str | None = None
+
+    def _get_platform_tags(self) -> tuple[str | None, str | None, str | None]:
+        python_tag: str | None = None
+        py_limited_api: str | None = None
+        plat_name: str | None = None
+        if not self.config_settings:
+            return python_tag, py_limited_api, plat_name
+        if "--python-tag" in self.config_settings:
+            python_tag = self.config_settings["--python-tag"]
+        if "--py-limited-api" in self.config_settings:
+            py_limited_api = cast(str, self.config_settings["--py-limited-api"])
+        if "--plat-name" in self.config_settings:
+            plat_name = self.config_settings["--plat-name"]
+        return python_tag, py_limited_api, plat_name
+
+    def _fix_dependencies(self) -> None:
+        """Fix the dependencies and remove dynamic variables from the metadata"""
+        metadata = self.config.metadata
+        root = self.location.as_posix()
+        if metadata.get("dependencies"):
+            metadata["dependencies"] = [
+                expand_vars(dep, root) for dep in metadata["dependencies"]
+            ]
+        if metadata.get("optional-dependencies"):
+            for name, deps in metadata["optional-dependencies"].items():
+                metadata["optional-dependencies"][name] = [
+                    expand_vars(dep, root) for dep in deps
+                ]
+
+    def initialize(self, context: Context) -> None:
+        self._fix_dependencies()
+        return super().initialize(context)
+
+    def prepare_metadata(self, metadata_directory: str) -> Path:
+        """Write the dist-info files under the given directory"""
+        context = self.build_context(Path(metadata_directory))
+        self.initialize(context)
+        return self._write_dist_info(Path(metadata_directory))
+
+    def get_files(self, context: Context) -> Iterable[tuple[str, Path]]:
+        package_dir = self.config.build_config.package_dir
+        for relpath, path in super().get_files(context):
+            # remove the package-dir part from the relative paths
+            if package_dir and relpath.startswith(package_dir + "/"):
+                relpath = relpath[len(package_dir) + 1 :]
+            yield relpath, path
+        yield from self._get_metadata_files(context)
+
+    def build_artifact(
+        self, context: Context, files: Iterable[tuple[str, Path]]
+    ) -> Path:
+        records: list[RecordEntry] = []
+        with tempfile.NamedTemporaryFile(suffix=".whl", delete=False) as fp:
+            with zipfile.ZipFile(fp, "w", compression=zipfile.ZIP_DEFLATED) as zf:
+                for rel_path, full_path in files:
+                    records.append(self._add_file_to_zip(zf, rel_path, full_path))
+                self._write_record(zf, records)
+
+        target = context.dist_dir / f"{self.name_version}-{self.tag}.whl"
+        if target.exists():
+            target.unlink()
+        shutil.move(fp.name, target)
+        return target
 
     @property
-    def summary(self) -> str:
-        if not self._summary:
-            self._summary = self._expand_summary()
-
-        return self._summary
+    def name_version(self) -> str:
+        name = to_filename(canonicalize_name(self.config.metadata["name"]))
+        version = to_filename(safe_version(self.config.metadata["version"]))
+        return f"{name}-{version}"
 
     @property
-    def details(self) -> str:
-        if not self._details:
-            self._details = self._expand_details()
-
-        return self._details
-
-    def _simplify_name(self, name):
-        x = len("data.")
-        return name[x:] if name.startswith("data.") else name
-
-    def _expand_summary(self):
-        msg = self._original_message
-
-        for bad, repl in _MESSAGE_REPLACEMENTS.items():
-            msg = msg.replace(bad, repl)
-
-        if any(substring in msg for substring in _SKIP_DETAILS):
-            return msg
-
-        schema = self.ex.rule_definition
-        if self.ex.rule in _NEED_DETAILS and schema:
-            summary = _SummaryWriter(_TOML_JARGON)
-            return f"{msg}:\n\n{indent(summary(schema), '    ')}"
-
-        return msg
-
-    def _expand_details(self) -> str:
-        optional = []
-        desc_lines = self.ex.definition.pop("$$description", [])
-        desc = self.ex.definition.pop("description", None) or " ".join(desc_lines)
-        if desc:
-            description = "\n".join(
-                wrap(
-                    desc,
-                    width=80,
-                    initial_indent="    ",
-                    subsequent_indent="    ",
-                    break_long_words=False,
-                )
-            )
-            optional.append(f"DESCRIPTION:\n{description}")
-        schema = json.dumps(self.ex.definition, indent=4)
-        value = json.dumps(self.ex.value, indent=4)
-        defaults = [
-            f"GIVEN VALUE:\n{indent(value, '    ')}",
-            f"OFFENDING RULE: {self.ex.rule!r}",
-            f"DEFINITION:\n{indent(schema, '    ')}",
-        ]
-        return "\n\n".join(optional + defaults)
-
-
-class _SummaryWriter:
-    _IGNORE = {"description", "default", "title", "examples"}
-
-    def __init__(self, jargon: Optional[Dict[str, str]] = None):
-        self.jargon: Dict[str, str] = jargon or {}
-        # Clarify confusing terms
-        self._terms = {
-            "anyOf": "at least one of the following",
-            "oneOf": "exactly one of the following",
-            "allOf": "all of the following",
-            "not": "(*NOT* the following)",
-            "prefixItems": f"{self._jargon('items')} (in order)",
-            "items": "items",
-            "contains": "contains at least one of",
-            "propertyNames": (
-                f"non-predefined acceptable {self._jargon('property names')}"
-            ),
-            "patternProperties": f"{self._jargon('properties')} named via pattern",
-            "const": "predefined value",
-            "enum": "one of",
-        }
-        # Attributes that indicate that the definition is easy and can be done
-        # inline (e.g. string and number)
-        self._guess_inline_defs = [
-            "enum",
-            "const",
-            "maxLength",
-            "minLength",
-            "pattern",
-            "format",
-            "minimum",
-            "maximum",
-            "exclusiveMinimum",
-            "exclusiveMaximum",
-            "multipleOf",
-        ]
-
-    def _jargon(self, term: Union[str, List[str]]) -> Union[str, List[str]]:
-        if isinstance(term, list):
-            return [self.jargon.get(t, t) for t in term]
-        return self.jargon.get(term, term)
-
-    def __call__(
-        self,
-        schema: Union[dict, List[dict]],
-        prefix: str = "",
-        *,
-        _path: Sequence[str] = (),
-    ) -> str:
-        if isinstance(schema, list):
-            return self._handle_list(schema, prefix, _path)
+    def dist_info_name(self) -> str:
+        return f"{self.name_version}.dist-info"
 
-        filtered = self._filter_unecessary(schema, _path)
-        simple = self._handle_simple_dict(filtered, _path)
-        if simple:
-            return f"{prefix}{simple}"
-
-        child_prefix = self._child_prefix(prefix, "  ")
-        item_prefix = self._child_prefix(prefix, "- ")
-        indent = len(prefix) * " "
-        with io.StringIO() as buffer:
-            for i, (key, value) in enumerate(filtered.items()):
-                child_path = [*_path, key]
-                line_prefix = prefix if i == 0 else indent
-                buffer.write(f"{line_prefix}{self._label(child_path)}:")
-                # ^  just the first item should receive the complete prefix
-                if isinstance(value, dict):
-                    filtered = self._filter_unecessary(value, child_path)
-                    simple = self._handle_simple_dict(filtered, child_path)
-                    buffer.write(
-                        f" {simple}"
-                        if simple
-                        else f"\n{self(value, child_prefix, _path=child_path)}"
-                    )
-                elif isinstance(value, list) and (
-                    key != "type" or self._is_property(child_path)
-                ):
-                    children = self._handle_list(value, item_prefix, child_path)
-                    sep = " " if children.startswith("[") else "\n"
-                    buffer.write(f"{sep}{children}")
+    @property
+    def tag(self) -> str:
+        if self.__tag is None:
+            self.__tag = self._get_tag()
+        return self.__tag
+
+    def _get_tag(self) -> str:
+        impl, abi, platform = self._get_platform_tags()
+        is_purelib = self.config.build_config.is_purelib
+        if not is_purelib:
+            if not platform:
+                platform = get_platform(self.location / "build")
+            if not impl:
+                impl = tags.interpreter_name() + tags.interpreter_version()
+            if not abi:
+                abi = str(get_abi_tag()).lower()
+        else:
+            if not platform:
+                platform = "any"
+            abi = "none"
+            if not impl:
+                requires_python = self.config.metadata.get("requires-python", "")
+                if SpecifierSet(requires_python).contains("2.7"):
+                    impl = "py2.py3"
                 else:
-                    buffer.write(f" {self._value(value, child_path)}\n")
-            return buffer.getvalue()
-
-    def _is_unecessary(self, path: Sequence[str]) -> bool:
-        if self._is_property(path) or not path:  # empty path => instruction @ root
-            return False
-        key = path[-1]
-        return any(key.startswith(k) for k in "$_") or key in self._IGNORE
-
-    def _filter_unecessary(self, schema: dict, path: Sequence[str]):
-        return {
-            key: value
-            for key, value in schema.items()
-            if not self._is_unecessary([*path, key])
-        }
-
-    def _handle_simple_dict(self, value: dict, path: Sequence[str]) -> Optional[str]:
-        inline = any(p in value for p in self._guess_inline_defs)
-        simple = not any(isinstance(v, (list, dict)) for v in value.values())
-        if inline or simple:
-            return f"{{{', '.join(self._inline_attrs(value, path))}}}\n"
-        return None
+                    impl = "py3"
 
-    def _handle_list(
-        self, schemas: list, prefix: str = "", path: Sequence[str] = ()
+        platform = platform.lower().replace("-", "_").replace(".", "_")  # type: ignore
+        tag = (impl, abi, platform)
+        if not is_purelib:
+            supported_tags = [(t.interpreter, t.abi, platform) for t in tags.sys_tags()]
+            assert (
+                tag in supported_tags
+            ), f"would build wheel with unsupported tag {tag}"
+        return "-".join(tag)  # type: ignore[arg-type]
+
+    def _write_dist_info(self, parent: Path) -> Path:
+        """write the dist-info directory and return the path to it"""
+        dist_info = parent / self.dist_info_name
+        dist_info.mkdir(0o700, parents=True, exist_ok=True)
+        meta = self.config.metadata
+        entry_points = meta.entry_points
+        if entry_points:
+            with _open_for_write(dist_info / "entry_points.txt") as f:
+                self._write_entry_points(f, entry_points)
+
+        with _open_for_write(dist_info / "WHEEL") as f:
+            self._write_wheel_file(f, is_purelib=self.config.build_config.is_purelib)
+
+        with _open_for_write(dist_info / "METADATA") as f:
+            f.write(self.config.to_coremetadata())
+
+        for file in self.find_license_files():
+            target = dist_info / "licenses" / file
+            target.parent.mkdir(0o700, parents=True, exist_ok=True)
+            shutil.copy2(self.location / file, target)
+        return dist_info
+
+    def _add_file_to_zip(
+        self, zf: zipfile.ZipFile, rel_path: str, full_path: Path
+    ) -> RecordEntry:
+        self._show_add_file(rel_path, full_path)
+        zi = zipfile.ZipInfo(rel_path, ZIPINFO_DATE_TIME)
+        st_mode = os.stat(full_path).st_mode
+        zi.external_attr = (st_mode & 0xFFFF) << 16  # Unix attributes
+
+        if stat.S_ISDIR(st_mode):
+            zi.external_attr |= 0x10  # MS-DOS directory flag
+
+        with full_path.open("rb") as src:
+            hash_digest = self._write_zip_info(zf, zi, src)
+        size = zi.file_size
+        return RecordEntry(rel_path, f"sha256={hash_digest}", str(size))
+
+    @staticmethod
+    def _write_zip_info(
+        zf: zipfile.ZipFile, zi: zipfile.ZipInfo, src: IO[bytes]
     ) -> str:
-        if self._is_unecessary(path):
-            return ""
-
-        repr_ = repr(schemas)
-        if all(not isinstance(e, (dict, list)) for e in schemas) and len(repr_) < 60:
-            return f"{repr_}\n"
-
-        item_prefix = self._child_prefix(prefix, "- ")
-        return "".join(
-            self(v, item_prefix, _path=[*path, f"[{i}]"]) for i, v in enumerate(schemas)
-        )
-
-    def _is_property(self, path: Sequence[str]):
-        """Check if the given path can correspond to an arbitrarily named property"""
-        counter = 0
-        for key in path[-2::-1]:
-            if key not in {"properties", "patternProperties"}:
-                break
-            counter += 1
-
-        # If the counter if even, the path correspond to a JSON Schema keyword
-        # otherwise it can be any arbitrary string naming a property
-        return counter % 2 == 1
-
-    def _label(self, path: Sequence[str]) -> str:
-        *parents, key = path
-        if not self._is_property(path):
-            norm_key = _separate_terms(key)
-            return self._terms.get(key) or " ".join(self._jargon(norm_key))
-
-        if parents[-1] == "patternProperties":
-            return f"(regex {key!r})"
-        return repr(key)  # property name
-
-    def _value(self, value: Any, path: Sequence[str]) -> str:
-        if path[-1] == "type" and not self._is_property(path):
-            type_ = self._jargon(value)
-            return (
-                f"[{', '.join(type_)}]" if isinstance(value, list) else cast(str, type_)
+        hashsum = hashlib.sha256()
+        for buf in iter(lambda: src.read(2**16), b""):
+            hashsum.update(buf)
+
+        src.seek(0)
+        zf.writestr(zi, src.read(), compress_type=zipfile.ZIP_DEFLATED)
+        return urlsafe_b64encode(hashsum.digest()).decode("ascii").rstrip("=")
+
+    def _write_record(self, zf: zipfile.ZipFile, records: list[RecordEntry]) -> None:
+        zi = zipfile.ZipInfo(f"{self.dist_info_name}/RECORD", ZIPINFO_DATE_TIME)
+        buffer = io.BytesIO()
+        text_buffer = io.TextIOWrapper(buffer, encoding="utf-8", newline="")
+
+        writer = csv.writer(text_buffer, lineterminator="\n")
+        writer.writerows(records)
+        writer.writerow(RecordEntry(zi.filename, "", ""))
+        text_buffer.detach()
+        buffer.seek(0)
+        self._show_add_file(zi.filename, Path(zi.filename))
+        self._write_zip_info(zf, zi, buffer)
+
+    def _write_wheel_file(self, fp: IO[str], is_purelib: bool) -> None:
+        try:
+            version = get_version("pdm-backend")
+        except ModuleNotFoundError:
+            version = "0.0.0+local"
+
+        fp.write(
+            WHEEL_FILE_FORMAT.format(
+                is_purelib=str(is_purelib).lower(), tag=self.tag, version=version
             )
-        return repr(value)
+        )
 
-    def _inline_attrs(self, schema: dict, path: Sequence[str]) -> Iterator[str]:
-        for key, value in schema.items():
-            child_path = [*path, key]
-            yield f"{self._label(child_path)}: {self._value(value, child_path)}"
-
-    def _child_prefix(self, parent_prefix: str, child_prefix: str) -> str:
-        return len(parent_prefix) * " " + child_prefix
-
-
-def _separate_terms(word: str) -> List[str]:
-    """
-    >>> _separate_terms("FooBar-foo")
-    ['foo', 'bar', 'foo']
-    """
-    return [w.lower() for w in _CAMEL_CASE_SPLITTER.split(word) if w]
+    def _write_entry_points(
+        self, fp: IO[str], entry_points: dict[str, dict[str, str]]
+    ) -> None:
+        for group_name in sorted(entry_points):
+            fp.write(f"[{group_name}]\n")
+            for name, value in sorted(entry_points[group_name].items()):
+                fp.write(f"{name} = {value}\n")
+
+            fp.write("\n")
+
+    def _get_metadata_files(self, context: Context) -> Iterable[tuple[str, Path]]:
+        """Generate the metadata files for the wheel."""
+        if context.kwargs.get("metadata_directory"):
+            return self._iter_files_in_directory(context.kwargs["metadata_directory"])
+        else:
+            dist_info = self._write_dist_info(context.build_dir)
+            return self._iter_files_in_directory(str(dist_info))
+
+    def _iter_files_in_directory(self, path: str) -> Iterable[tuple[str, Path]]:
+        for root, _, files in os.walk(path):
+            relroot = os.path.relpath(root, os.path.dirname(path))
+            for file in files:
+                yield (Path(relroot, file).as_posix(), Path(root) / file)
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/base.py` & `pdm_backend-2.0.7/src/pdm/backend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         self.call_hook("pdm_build_finalize", context, artifact)
 
     def build(self, build_dir: str, **kwargs: Any) -> Path:
         """Build the package and return the path to the artifact."""
         context = self.build_context(Path(build_dir), **kwargs)
         if (
             not self.config_settings.get("no-clean-build")
-            or os.getenv("PDM_BUILD_NO_CLEAN", "false").lower() != "false"
+            or os.getenv("PDM_BUILD_NO_CLEAN", "false").lower() == "false"
         ):
             self.clean(context)
         self.initialize(context)
         files = sorted(self.get_files(context))
         artifact = self.build_artifact(context, files)
         self.finalize(context, artifact)
         return artifact
@@ -196,18 +196,14 @@
         self, context: Context, files: Iterable[tuple[str, Path]]
     ) -> Path:
         """Build the artifact from an iterable of (relpath, path) pairs
         and return the path to it.
         """
         raise NotImplementedError()
 
-    def format_pkginfo(self) -> str:
-        metadata = self.config.as_standard_metadata()
-        return str(metadata.as_rfc822())
-
     def _collect_files(self, context: Context) -> FileMap:
         """Collect files to add to the artifact under the given root."""
         root = self.location
         includes, excludes = self._get_include_and_exclude_paths()
         files = FileMap()
         for include_path in includes:
             path = root / include_path
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/config.py` & `pdm_backend-2.0.7/src/pdm/backend/hooks/version/scm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,260 +1,336 @@
+"""
+module to get version from tag of SCM repository.
+Adapted from setuptools-scm. Currently only support git and hg.
+"""
 from __future__ import annotations
 
-import glob
 import os
-import sys
+import re
+import shlex
+import shutil
+import subprocess
+import warnings
+from dataclasses import dataclass
+from datetime import datetime
 from pathlib import Path
-from typing import Any, TypeVar
+from typing import Any, Iterable, NamedTuple
 
-from pdm.backend._vendor import tomli_w
-from pdm.backend._vendor.pyproject_metadata import StandardMetadata
-from pdm.backend._vendor.validate_pyproject import api, errors
-from pdm.backend.exceptions import ConfigError, ValidationError
-from pdm.backend.structures import Table
-from pdm.backend.utils import find_packages_iter
-
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    import pdm.backend._vendor.tomli as tomllib
+from pdm.backend._vendor.packaging.version import Version
 
-T = TypeVar("T")
+DEFAULT_TAG_REGEX = re.compile(
+    r"^(?:[\w-]+-)?(?P<version>[vV]?\d+(?:\.\d+){0,2}[^\+]*)(?:\+.*)?$"
+)
 
 
+@dataclass(frozen=True)
 class Config:
-    """The project config object for pdm backend.
+    tag_regex: re.Pattern
 
-    Parameters:
-        root: The root directory of the project
-        data: The parsed pyproject.toml data
-
-    Attributes:
-        metadata (Metadata): The project metadata from the `project` table
-        build_config (BuildConfig): The build config from the `tool.pdm.build` table
-    """
 
-    def __init__(self, root: Path, data: dict[str, Any]) -> None:
-        self.validate(data)
-        self.root = root
-        self.data = data
-        self.metadata = Metadata(data["project"])
-        self.build_config = BuildConfig(
-            root, data.setdefault("tool", {}).get("pdm", {}).get("build", {})
+def _subprocess_call(
+    cmd: str | list[str],
+    cwd: os.PathLike | None = None,
+    extra_env: dict[str, str] | None = None,
+) -> tuple[int, str, str]:
+    # adapted from pre-commit
+    # Too many bugs dealing with environment variables and GIT:
+    # https://github.com/pre-commit/pre-commit/issues/300
+    env = {
+        k: v
+        for k, v in os.environ.items()
+        if not k.startswith("GIT_")
+        or k in ("GIT_EXEC_PATH", "GIT_SSH", "GIT_SSH_COMMAND")
+    }
+    env.update({"LC_ALL": "C", "LANG": "", "HGPLAIN": "1"})
+    if extra_env:
+        env.update(extra_env)
+    if isinstance(cmd, str):
+        cmd = shlex.split(cmd)
+    proc = subprocess.Popen(
+        cmd, cwd=cwd, env=env, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    )
+    out, err = proc.communicate()
+    return (
+        proc.returncode,
+        out.decode("utf-8", "surrogateescape").strip(),
+        err.decode("utf-8", "surrogateescape").strip(),
+    )
+
+
+class VersionInfo(NamedTuple):
+    version: Version
+    distance: int | None
+    dirty: bool
+    node: str | None
+    branch: str | None
+
+
+def meta(
+    config: Config,
+    tag: str | Version,
+    distance: int | None = None,
+    dirty: bool = False,
+    node: str | None = None,
+    branch: str | None = None,
+) -> VersionInfo:
+    if isinstance(tag, str):
+        tag = tag_to_version(config, tag)
+    return VersionInfo(tag, distance, dirty, node, branch)
+
+
+def _git_get_branch(root: os.PathLike[Any]) -> str | None:
+    ret, out, _ = _subprocess_call("git rev-parse --abbrev-ref HEAD", root)
+    if not ret:
+        return out
+    return None
+
+
+def _git_is_dirty(root: os.PathLike[Any]) -> bool:
+    _, out, _ = _subprocess_call("git status --porcelain --untracked-files=no", root)
+    return bool(out)
+
+
+def _git_get_node(root: os.PathLike[Any]) -> str | None:
+    ret, out, _ = _subprocess_call("git rev-parse --verify --quiet HEAD", root)
+    if not ret:
+        return out[:7]
+    return None
+
+
+def _git_count_all_nodes(root: os.PathLike[Any]) -> int:
+    _, out, _ = _subprocess_call("git rev-list HEAD", root)
+    return out.count("\n") + 1
+
+
+def _git_parse_describe(describe_output: str) -> tuple[str, int, str, bool]:
+    # 'describe_output' looks e.g. like 'v1.5.0-0-g4060507' or
+    # 'v1.15.1rc1-37-g9bd1298-dirty'.
+
+    if describe_output.endswith("-dirty"):
+        dirty = True
+        describe_output = describe_output[:-6]
+    else:
+        dirty = False
+
+    tag, number, node = describe_output.rsplit("-", 2)
+    return tag, int(number), node, dirty
+
+
+class _ParseResult(NamedTuple):
+    version: str
+    prefix: str
+    suffix: str
+
+
+def _parse_version_tag(config: Config, tag: str) -> _ParseResult | None:
+    tagstring = tag if not isinstance(tag, str) else str(tag)
+    match = config.tag_regex.match(tagstring)
+
+    result = None
+    if match:
+        if len(match.groups()) == 1:
+            key: int | str = 1
+        else:
+            key = "version"
+
+        result = _ParseResult(
+            match.group(key),
+            match.group(0)[: match.start(key)],
+            match.group(0)[match.end(key) :],
         )
 
-    def as_standard_metadata(self) -> StandardMetadata:
-        """Return the metadata as a StandardMetadata object."""
-        return StandardMetadata.from_pyproject(self.data, project_dir=self.root)
-
-    @staticmethod
-    def validate(data: dict[str, Any]) -> None:
-        """Validate the pyproject.toml data."""
-        validator = api.Validator()
-        try:
-            validator(data)
-        except errors.ValidationError as e:
-            raise ValidationError(e.summary, e.details) from e
-
-    @classmethod
-    def from_pyproject(cls, root: str | Path) -> Config:
-        """Load the pyproject.toml file from the given project root."""
-        root = Path(root)
-        pyproject = root / "pyproject.toml"
-        if not pyproject.exists():
-            raise ConfigError("pyproject.toml not found")
-        with pyproject.open("rb") as fp:
-            try:
-                data = tomllib.load(fp)
-            except tomllib.TOMLDecodeError as e:
-                raise ConfigError(f"Invalid pyproject.toml file: {e}") from e
-        return cls(root, data)
-
-    def write_to(self, path: str | Path) -> None:
-        """Write the pyproject.toml file to the given path."""
-        with open(path, "wb") as fp:
-            tomli_w.dump(self.data, fp)
-
-    def for_hook(self, name: str) -> dict[str, Any]:
-        """Return the config data for the given hook."""
-        return self.build_config.get("hooks", {}).get(name, {})
-
-    def convert_package_paths(self) -> dict[str, list | dict]:
-        """Return a {package_dir, packages, package_data, exclude_package_data} dict."""
-        packages = []
-        py_modules = []
-        package_data = {"": ["*"]}
-        exclude_package_data: dict[str, list[str]] = {}
-        package_dir = self.build_config.package_dir
-        includes = self.build_config.includes
-        excludes = self.build_config.excludes
-
-        src_dir = Path(package_dir or ".")
-        if not includes:
-            packages = list(
-                find_packages_iter(
-                    package_dir or ".",
-                    exclude=["tests", "tests.*"],
-                    src=str(src_dir),
-                )
-            )
-            if not packages:
-                py_modules = [path.name[:-3] for path in src_dir.glob("*.py")]
-        else:
-            packages_set = set()
-            includes = includes[:]
-            for include in includes[:]:
-                if include.replace("\\", "/").endswith("/*"):
-                    include = include[:-2]
-                if "*" not in include and os.path.isdir(include):
-                    dir_name = include.rstrip("/\\")
-                    temp = list(find_packages_iter(dir_name, src=package_dir or "."))
-                    if os.path.isfile(os.path.join(dir_name, "__init__.py")):
-                        temp.insert(0, dir_name)
-                    packages_set.update(temp)
-                    includes.remove(include)
-            packages[:] = list(packages_set)
-            for include in includes:
-                for path in glob.glob(include, recursive=True):
-                    if "/" not in path.lstrip("./") and path.endswith(".py"):
-                        # Only include top level py modules
-                        py_modules.append(path.lstrip("./")[:-3])
-                if include.endswith(".py"):
-                    continue
-                for package in packages:
-                    relpath = os.path.relpath(include, package)
-                    if not relpath.startswith(".."):
-                        package_data.setdefault(package, []).append(relpath)
-            for exclude in excludes:
-                for package in packages:
-                    relpath = os.path.relpath(exclude, package)
-                    if not relpath.startswith(".."):
-                        exclude_package_data.setdefault(package, []).append(relpath)
-        if packages and py_modules:
-            raise ConfigError("Can't specify packages and py_modules at the same time.")
-        return {
-            "package_dir": {"": package_dir} if package_dir else {},
-            "packages": packages,
-            "py_modules": py_modules,
-            "package_data": package_data,
-            "exclude_package_data": exclude_package_data,
-        }
-
-
-class Metadata(Table):
-    """The project metadata table"""
-
-    @property
-    def readme_file(self) -> str | None:
-        """The readme file path, if not exists, returns None"""
-        readme = self.get("readme")
-        if not readme:
-            return None
-        if isinstance(readme, str):
-            return readme
-        if isinstance(readme, dict) and "file" in readme:
-            return readme["file"]
+    return result
+
+
+def tag_to_version(config: Config, tag: str) -> Version:
+    """
+    take a tag that might be prefixed with a keyword and return only the version part
+    :param config: optional configuration object
+    """
+    tagdict = _parse_version_tag(config, tag)
+    if not tagdict or not tagdict.version:
+        warnings.warn(f"tag {tag!r} no version found")
+        return Version("0.0.0")
+
+    version = tagdict.version
+
+    if tagdict.suffix:
+        warnings.warn(f"tag {tag!r} will be stripped of its suffix {tagdict.suffix!r}")
+
+    return Version(version)
+
+
+def tags_to_versions(config: Config, tags: Iterable[str]) -> list[Version]:
+    """
+    take tags that might be prefixed with a keyword and return only the version part
+    :param tags: an iterable of tags
+    :param config: optional configuration object
+    """
+    return [tag_to_version(config, tag) for tag in tags if tag]
+
+
+def git_parse_version(root: os.PathLike[Any], config: Config) -> VersionInfo | None:
+    GIT = shutil.which("git")
+    if not GIT:
         return None
 
-    @property
-    def license_files(self) -> dict[str, list[str]]:
-        """The license files configuration"""
-        subtable_files = None
-        if (
-            "license" in self
-            and isinstance(self["license"], dict)
-            and "files" in self["license"]
-        ):
-            subtable_files = self["license"]["files"]
-        if "license-files" not in self:
-            if subtable_files is not None:
-                return {"paths": [self["license"]["file"]]}
-            return {
-                "globs": [
-                    "LICENSES/*",
-                    "LICEN[CS]E*",
-                    "COPYING*",
-                    "NOTICE*",
-                    "AUTHORS*",
-                ]
-            }
-        if subtable_files is not None:
-            raise ValidationError(
-                "license-files",
-                "Can't specify both 'license.files' and 'license-files' fields",
-            )
-        rv = self["license-files"]
-        valid_keys = {"globs", "paths"} & set(rv)
-        if len(valid_keys) == 2:
-            raise ValidationError(
-                "license-files", "Can't specify both 'paths' and 'globs'"
-            )
-        if not valid_keys:
-            raise ValidationError("license-files", "Must specify 'paths' or 'globs'")
-        return rv
-
-    @property
-    def entry_points(self) -> dict[str, dict[str, str]]:
-        """The entry points mapping"""
-        entry_points: dict[str, dict[str, str]] = self.get("entry-points", {})
-        if "scripts" in self:
-            entry_points["console_scripts"] = self["scripts"]
-        if "gui-scripts" in self:
-            entry_points["gui_scripts"] = self["gui-scripts"]
-        return entry_points
-
-
-class BuildConfig(Table):
-    """The `[tool.pdm.build]` table"""
-
-    def __init__(self, root: Path, data: dict[str, Any]) -> None:
-        self.root = root
-        super().__init__(data)
-
-    @property
-    def custom_hook(self) -> str | None:
-        """The relative path to the custom hook or None if not exists"""
-        script = self.get("custom-hook", "pdm_build.py")
-        if (self.root / script).exists():
-            return script
+    ret, repo, _ = _subprocess_call([GIT, "rev-parse", "--show-toplevel"], root)
+    if ret or not os.path.samefile(root, repo):
         return None
 
-    @property
-    def includes(self) -> list[str]:
-        """The includes setting"""
-        return self.get("includes", [])
-
-    @property
-    def source_includes(self) -> list[str]:
-        """The source-includes setting"""
-        return self.get("source-includes", [])
-
-    @property
-    def excludes(self) -> list[str]:
-        """The excludes setting"""
-        return self.get("excludes", [])
-
-    @property
-    def run_setuptools(self) -> bool:
-        """Whether to run setuptools"""
-        return self.get("run-setuptools", False)
-
-    @property
-    def package_dir(self) -> str:
-        """A directory that will be used to looking for packages."""
-        default = "src" if self.root.joinpath("src").exists() else ""
-        return self.get("package-dir", default)
-
-    @property
-    def is_purelib(self) -> bool:
-        """If not explicitly set, the project is considered to be non-pure
-        if `build` exists.
-        """
-        return self.get("is-purelib", not bool(self.run_setuptools))
-
-    @property
-    def editable_backend(self) -> str:
-        """Currently only two backends are supported:
-        - editables: Proxy modules via editables
-        - path: the legacy .pth file method(default)
-        """
-        return self.get("editable-backend", "path")
+    if os.path.isfile(os.path.join(root, ".git/shallow")):
+        warnings.warn(f"{root!r} is shallow and may cause errors")
+    describe_cmd = [GIT, "describe", "--dirty", "--tags", "--long", "--match", "*.*"]
+    ret, output, err = _subprocess_call(describe_cmd, root)
+    branch = _git_get_branch(root)
+
+    if ret:
+        rev_node = _git_get_node(root)
+        dirty = _git_is_dirty(root)
+        if rev_node is None:
+            return meta(config, "0.0", 0, dirty)
+        return meta(
+            config, "0.0", _git_count_all_nodes(root), dirty, f"g{rev_node}", branch
+        )
+    else:
+        tag, number, node, dirty = _git_parse_describe(output)
+        return meta(config, tag, number or None, dirty, node, branch)
+
+
+def get_latest_normalizable_tag(root: os.PathLike[Any]) -> str:
+    # Gets all tags containing a '.' from oldest to newest
+    cmd = [
+        "hg",
+        "log",
+        "-r",
+        "ancestors(.) and tag('re:\\.')",
+        "--template",
+        "{tags}\n",
+    ]
+    _, output, _ = _subprocess_call(cmd, root)
+    outlines = output.split()
+    if not outlines:
+        return "null"
+    tag = outlines[-1].split()[-1]
+    return tag
+
+
+def hg_get_graph_distance(root: os.PathLike[Any], rev1: str, rev2: str = ".") -> int:
+    cmd = ["hg", "log", "-q", "-r", f"{rev1}::{rev2}"]
+    _, out, _ = _subprocess_call(cmd, root)
+    return len(out.strip().splitlines()) - 1
+
+
+def _hg_tagdist_normalize_tagcommit(
+    config: Config, root: os.PathLike[Any], tag: str, dist: int, node: str, branch: str
+) -> VersionInfo:
+    dirty = node.endswith("+")
+    node = "h" + node.strip("+")
+
+    # Detect changes since the specified tag
+    revset = (
+        "(branch(.)"  # look for revisions in this branch only
+        " and tag({tag!r})::."  # after the last tag
+        # ignore commits that only modify .hgtags and nothing else:
+        " and (merge() or file('re:^(?!\\.hgtags).*$'))"
+        " and not tag({tag!r}))"  # ignore the tagged commit itself
+    ).format(tag=tag)
+    if tag != "0.0":
+        _, commits, _ = _subprocess_call(
+            ["hg", "log", "-r", revset, "--template", "{node|short}"],
+            root,
+        )
+    else:
+        commits = "True"
+
+    if commits or dirty:
+        return meta(config, tag, distance=dist, node=node, dirty=dirty, branch=branch)
+    else:
+        return meta(config, tag)
+
+
+def guess_next_version(tag_version: Version) -> str:
+    version = _strip_local(str(tag_version))
+    return _bump_dev(version) or _bump_regex(version)
+
+
+def _strip_local(version_string: str) -> str:
+    public, _, _ = version_string.partition("+")
+    return public
+
+
+def _bump_dev(version: str) -> str:
+    if ".dev" not in version:
+        return ""
+
+    prefix, tail = version.rsplit(".dev", 1)
+    assert tail == "0", "own dev numbers are unsupported"
+    return prefix
+
+
+def _bump_regex(version: str) -> str:
+    match = re.match(r"(.*?)(\d+)$", version)
+    assert match is not None
+    prefix, tail = match.groups()
+    return "%s%d" % (prefix, int(tail) + 1)
+
+
+def hg_parse_version(root: os.PathLike[Any], config: Config) -> VersionInfo | None:
+    if not shutil.which("hg"):
+        return None
+    _, output, _ = _subprocess_call("hg id -i -b -t", root)
+    identity_data = output.split()
+    if not identity_data:
+        return None
+    node = identity_data.pop(0)
+    branch = identity_data.pop(0)
+    if "tip" in identity_data:
+        # tip is not a real tag
+        identity_data.remove("tip")
+    tags = tags_to_versions(config, identity_data)
+    dirty = node[-1] == "+"
+    if tags:
+        return meta(config, tags[0], dirty=dirty, branch=branch)
+
+    if node.strip("+") == "0" * 12:
+        return meta(config, "0.0", dirty=dirty, branch=branch)
+
+    try:
+        tag = get_latest_normalizable_tag(root)
+        dist = hg_get_graph_distance(root, tag)
+        if tag == "null":
+            tag = "0.0"
+            dist = int(dist) + 1
+        return _hg_tagdist_normalize_tagcommit(config, root, tag, dist, node, branch)
+    except ValueError:
+        return None  # unpacking failed, old hg
+
+
+def format_version(version: VersionInfo) -> str:
+    if version.distance is None:
+        main_version = str(version.version)
+    else:
+        guessed = guess_next_version(version.version)
+        main_version = f"{guessed}.dev{version.distance}"
+
+    if version.distance is None or version.node is None:
+        clean_format = ""
+        dirty_format = "+d{time:%Y%m%d}"
+    else:
+        clean_format = "+{node}"
+        dirty_format = "+{node}.d{time:%Y%m%d}"
+    fmt = dirty_format if version.dirty else clean_format
+    local_version = fmt.format(node=version.node, time=datetime.utcnow())
+    return main_version + local_version
+
+
+def get_version_from_scm(root: str | Path, *, tag_regex: str | None = None) -> str:
+    config = Config(tag_regex=re.compile(tag_regex) if tag_regex else DEFAULT_TAG_REGEX)
+    for func in (git_parse_version, hg_parse_version):
+        version = func(root, config)  # type: ignore
+        if version:
+            break
+    else:
+        version = meta(config, "0.0.0")
+    assert version is not None
+    return format_version(version)
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/editable.py` & `pdm_backend-2.0.7/src/pdm/backend/editable.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/hooks/base.py` & `pdm_backend-2.0.7/src/pdm/backend/hooks/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.0.7/src/pdm/backend/hooks/setuptools.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/hooks/version/__init__.py` & `pdm_backend-2.0.7/src/pdm/backend/hooks/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/intree.py` & `pdm_backend-2.0.7/src/pdm/backend/intree.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/macosx_platform.py` & `pdm_backend-2.0.7/src/pdm/backend/macosx_platform.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/sdist.py` & `pdm_backend-2.0.7/src/pdm/backend/sdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 if tar_info.isreg():
                     with path.open("rb") as f:
                         tar.addfile(tar_info, f)
                 else:
                     tar.addfile(tar_info)
                 self._show_add_file(relpath, path)
 
-            pkg_info = self.format_pkginfo().encode("utf-8")
+            pkg_info = self.config.to_coremetadata().encode("utf-8")
             tar_info = tarfile.TarInfo(pjoin(dist_info, "PKG-INFO"))
             tar_info.size = len(pkg_info)
             tar_info = clean_tarinfo(tar_info)
             tar.addfile(tar_info, BytesIO(pkg_info))
             self._show_add_file("PKG-INFO", Path("PKG-INFO"))
 
         return target
```

### Comparing `pdm_backend-2.0.6/src/pdm/backend/structures.py` & `pdm_backend-2.0.7/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/src/pdm/backend/utils.py` & `pdm_backend-2.0.7/src/pdm/backend/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/conftest.py` & `pdm_backend-2.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.0.7/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.0.7/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.0.7/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/test_api.py` & `pdm_backend-2.0.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/test_file_finder.py` & `pdm_backend-2.0.7/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/test_hooks.py` & `pdm_backend-2.0.7/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/test_metadata.py` & `pdm_backend-2.0.7/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/test_wheel.py` & `pdm_backend-2.0.7/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/tests/testutils.py` & `pdm_backend-2.0.7/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.6/PKG-INFO` & `pdm_backend-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.0.6
+Version: 2.0.7
 Summary: The build backend used by PDM that supports latest packaging standards
 Keywords: packaging PEP 517 build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.0.6 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.0.7 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
 packaging PEP 517 build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

