# Comparing `tmp/quartodoc-0.3.0.tar.gz` & `tmp/quartodoc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.3.0.tar", last modified: Mon May  1 17:56:58 2023, max compression
+gzip compressed data, was "quartodoc-0.3.1.tar", last modified: Mon May 15 17:26:31 2023, max compression
```

## Comparing `quartodoc-0.3.0.tar` & `quartodoc-0.3.1.tar`

### file list

```diff
@@ -1,118 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.213488 quartodoc-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.217488 quartodoc-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-01 17:56:44.000000 quartodoc-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-01 17:56:44.000000 quartodoc-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 17:56:44.000000 quartodoc-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 17:56:44.000000 quartodoc-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-01 17:56:44.000000 quartodoc-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-01 17:56:58.229488 quartodoc-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-01 17:56:44.000000 quartodoc-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-01 17:56:44.000000 quartodoc-0.3.0/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.213488 quartodoc-0.3.0/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.217488 quartodoc-0.3.0/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/example.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/objects_siuba.json
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.inv
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.217488 quartodoc-0.3.0/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-01 17:56:44.000000 quartodoc-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-01 17:56:44.000000 quartodoc-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-01 17:56:58.229488 quartodoc-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.000081 quartodoc-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.012081 quartodoc-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-15 17:26:15.000000 quartodoc-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-15 17:26:15.000000 quartodoc-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 17:26:15.000000 quartodoc-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 17:26:15.000000 quartodoc-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 17:26:15.000000 quartodoc-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-15 17:26:31.040083 quartodoc-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-15 17:26:15.000000 quartodoc-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-15 17:26:15.000000 quartodoc-0.3.1/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.000081 quartodoc-0.3.1/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.012081 quartodoc-0.3.1/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/example.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/objects_siuba.json
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/objects_vetiver.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/objects_vetiver.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.012081 quartodoc-0.3.1/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.016082 quartodoc-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.016082 quartodoc-0.3.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.020082 quartodoc-0.3.1/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.020082 quartodoc-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.024082 quartodoc-0.3.1/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.024082 quartodoc-0.3.1/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.024082 quartodoc-0.3.1/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 17:26:15.000000 quartodoc-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.032082 quartodoc-0.3.1/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.036083 quartodoc-0.3.1/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.032082 quartodoc-0.3.1/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-15 17:26:15.000000 quartodoc-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 17:26:31.040083 quartodoc-0.3.1/setup.cfg
```

### Comparing `quartodoc-0.3.0/.github/workflows/ci.yml` & `quartodoc-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/.gitignore` & `quartodoc-0.3.1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -137,7 +137,9 @@
 
 # Pyre type checker
 .pyre/
 .Rproj.user
 
 # Local Netlify folder
 .netlify
+
+/.luarc.json
```

### Comparing `quartodoc-0.3.0/LICENSE` & `quartodoc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/Makefile` & `quartodoc-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/PKG-INFO` & `quartodoc-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: mc_al_github@fastmail.com
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `quartodoc-0.3.0/README.md` & `quartodoc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/README.qmd` & `quartodoc-0.3.1/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/_extensions/interlinks/README.md` & `quartodoc-0.3.1/_extensions/interlinks/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/_extensions/interlinks/example.qmd` & `quartodoc-0.3.1/_extensions/interlinks/example.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/_extensions/interlinks/interlinks.py` & `quartodoc-0.3.1/_extensions/interlinks/interlinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 import json
 import panflute as pf
 
-from quartodoc.inventory import Ref, RefSyntaxError
+from quartodoc.interlinks import Ref, RefSyntaxError
 from pathlib import Path
 from plum import dispatch
 
 
 # Hold all inventory items in a singleton -------------------------------------
 
 # TODO: make entries into dataclass
```

### Comparing `quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.inv` & `quartodoc-0.3.1/_extensions/interlinks/objects_vetiver.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.json` & `quartodoc-0.3.1/_extensions/interlinks/objects_vetiver.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/case_studies/objects_sqla.inv` & `quartodoc-0.3.1/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/case_studies/parsing.qmd` & `quartodoc-0.3.1/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/case_studies/some_package.py` & `quartodoc-0.3.1/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/case_studies/sphinx-inventory.md` & `quartodoc-0.3.1/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/case_studies/sphinx-inventory.qmd` & `quartodoc-0.3.1/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/_quarto.yml` & `quartodoc-0.3.1/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/examples/index.qmd` & `quartodoc-0.3.1/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/architecture.qmd` & `quartodoc-0.3.1/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/basic-building.qmd` & `quartodoc-0.3.1/docs/get-started/basic-building.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/basic-content.qmd` & `quartodoc-0.3.1/docs/get-started/basic-content.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/basic-docs.qmd` & `quartodoc-0.3.1/docs/get-started/basic-docs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/crossrefs.qmd` & `quartodoc-0.3.1/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.3.1/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.3.1/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/dev-prepare.qmd` & `quartodoc-0.3.1/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/dev-renderers.qmd` & `quartodoc-0.3.1/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/docstring-examples.qmd` & `quartodoc-0.3.1/docs/get-started/docstring-examples.qmd`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,16 @@
     markdown syntax:
     
     ```python
     1 + 1
     ```
     
     quarto syntax:
-    note that the "\" should be removed.
     
-    ```\{python}
+    ```{{python}}
     1 + 1
     ```
 ```
 
 
 ## Examples, etc..: the "s" matters
 
@@ -128,8 +127,44 @@
 
     See the [reference](/reference/index.qmd) page.
     """
 ```
 
 :::{.callout-note}
 Linking to functions documented outside your package must be configured in the [interlinks filter](./interlinks.qmd).
-:::
+:::
+
+
+## How do I document a class?
+
+See [this numpydoc page on documenting classes](https://numpydoc.readthedocs.io/en/latest/format.html#documenting-classes).
+
+Below is a simple example of a class docstring.
+
+```python
+class MyClass:
+    """A great class.
+
+    Parameters
+    ----------
+    a:
+        Some parameter.
+
+    Attributes
+    ----------
+    x:
+        An integer
+    """
+
+
+    x: int = 1
+
+
+    def __init__(self, a: str):
+        self.a = a
+```
+
+Note these two important pieces:
+
+* Document your `__init__` method parameters on the class docstring.
+* You can use an `Attributes` section in your docstring.
+
```

### Comparing `quartodoc-0.3.0/docs/get-started/extending.qmd` & `quartodoc-0.3.1/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.3.1/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/interlinks.qmd` & `quartodoc-0.3.1/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/get-started/overview.qmd` & `quartodoc-0.3.1/docs/get-started/overview.qmd`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 ```bash
 python -m pip install quartodoc
 
 # or from github
 python -m pip install git+https://github.com/machow/quartodoc.git
 ```
 
+:::{.callout-note}
+In order to install quarto, see the quarto [get started page](https://quarto.org/docs/get-started/).
+:::
+
+
 ## Basic use
 
 Getting started with quartodoc takes two steps: configuring a quarto website,
 and generating documentation pages for your library.
 
 First, create a `_quarto.yml` file with the following:
 
@@ -53,15 +58,15 @@
         - get_object
         - preview
 ```
 
 Next, run this command to generate your API pages:
 
 ```bash
-python -m quartodoc build
+quartodoc build
 ```
 
 This should create a `reference/` directory with an `index.qmd` and documentation
 pages for listed functions, like `get_object` and `preview`.
 
 Finally, preview your website with quarto:
 
@@ -70,25 +75,25 @@
 ```
 
 ## Rebuilding site
 
 As mentioned in the previous section, you can preview your quartodoc site using these commands:
 
 ```bash
-python -m quartodoc build
+quartodoc build
 quarto preview
 ```
 
 In order to rebuild your API documentation pages during a quarto preview, re-run
 the quartodoc build command:
 
 ```bash
 # with quarto preview running, you only need to re-run quartodoc build,
 # which will re-create the pages of your API documentation.
-python -m quartodoc build
+quartodoc build
 ```
 
 ## Looking up objects
 
 Finding python objects to document involves two pieces of configuration:
 
 * the package name.
@@ -137,8 +142,8 @@
 [pkgdown-code]: https://github.com/machow/quartodoc/tree/main/examples/pkgdown
 [single-page]: /examples/single-page/reference
 [sp-code]: https://github.com/machow/quartodoc/tree/main/examples/single-page
 [shiny]: https://shiny.rstudio.com/py/api/
 [vetiver]: https://rstudio.github.io/vetiver-python/stable/reference/
 [vt-code]: https://github.com/rstudio/vetiver-python
 [siuba]: https://siuba.org/api/
-[sb-code]: https://github.com/machow/siuba.org
+[sb-code]: https://github.com/machow/siuba.org
```

### Comparing `quartodoc-0.3.0/docs/get-started/sidebar.qmd` & `quartodoc-0.3.1/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/docs/styles.css` & `quartodoc-0.3.1/docs/styles.css`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/dascore/_quarto.yml` & `quartodoc-0.3.1/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/dascore/generate_api.py` & `quartodoc-0.3.1/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/pkgdown/_quarto.yml` & `quartodoc-0.3.1/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/pkgdown/objects.json` & `quartodoc-0.3.1/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.3.1/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.3.1/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/single-page/_quarto.yml` & `quartodoc-0.3.1/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/single-page/objects.json` & `quartodoc-0.3.1/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/examples/single-page/reference/index.qmd` & `quartodoc-0.3.1/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/__main__.py` & `quartodoc-0.3.1/quartodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/ast.py` & `quartodoc-0.3.1/quartodoc/ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/autosummary.py` & `quartodoc-0.3.1/quartodoc/autosummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,18 @@
         The renderer used to convert docstrings (e.g. to markdown).
     out_index:
         The output path of the index file, used to list all API functions.
     sidebar:
         The output path for a sidebar yaml config (by default no config generated).
     rewrite_all_pages:
         Whether to rewrite all rendered doc pages, or only those with changes.
+    source_dir:
+        A directory where source files to be documented live. This is only necessary
+        if you are not documenting a package, but collection of scripts. Use a "."
+        to refer to the current directory.
 
     """
 
     # builder dispatching ----
     style: str
     _registry: "dict[str, Builder]" = {}
 
@@ -373,14 +377,15 @@
         version: "str | None" = None,
         dir: str = "reference",
         title: str = "Function reference",
         renderer: "dict | Renderer | str" = "markdown",
         out_index: str = None,
         sidebar: "str | None" = None,
         rewrite_all_pages=False,
+        source_dir: "str | None" = None,
     ):
         self.layout = self.load_layout(sections=sections, package=package)
 
         self.package = package
         self.version = None
         self.dir = dir
         self.title = title
@@ -388,14 +393,15 @@
 
         self.renderer = Renderer.from_config(renderer)
 
         if out_index is not None:
             self.out_index = out_index
 
         self.rewrite_all_pages = rewrite_all_pages
+        self.source_dir = str(Path(source_dir).absolute()) if source_dir else None
 
     def load_layout(self, sections: dict, package: str):
         # TODO: currently returning the list of sections, to make work with
         # previous code. We should make Layout a first-class citizen of the
         # process.
         return layout.Layout(sections=sections, package=package)
 
@@ -410,14 +416,19 @@
             A simple pattern, that may include * as a wildcard. If specified,
             only doc paths for objects with matching names will be written.
             Path is the file's base name in the API dir (e.g. MdRenderer.render)
         """
 
         from quartodoc import blueprint, collect
 
+        if self.source_dir:
+            import sys
+
+            sys.path.append(self.source_dir)
+
         # shaping and collection ----
 
         _log.info("Generating blueprint.")
         blueprint = blueprint(self.layout)
 
         _log.info("Collecting pages and inventory items.")
         pages, items = collect(blueprint, base_dir=self.dir)
```

### Comparing `quartodoc-0.3.0/quartodoc/builder/blueprint.py` & `quartodoc-0.3.1/quartodoc/builder/blueprint.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/builder/collect.py` & `quartodoc-0.3.1/quartodoc/builder/collect.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/builder/utils.py` & `quartodoc-0.3.1/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/layout.py` & `quartodoc-0.3.1/quartodoc/layout.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/renderers/base.py` & `quartodoc-0.3.1/quartodoc/renderers/base.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/renderers/md_renderer.py` & `quartodoc-0.3.1/quartodoc/renderers/md_renderer.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/example_dynamic.py` & `quartodoc-0.3.1/quartodoc/tests/example_dynamic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/test_ast.py` & `quartodoc-0.3.1/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/test_basic.py` & `quartodoc-0.3.1/quartodoc/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/test_builder.py` & `quartodoc-0.3.1/quartodoc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.3.1/quartodoc/tests/test_builder_blueprint.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/test_layout.py` & `quartodoc-0.3.1/quartodoc/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc/tests/test_renderers.py` & `quartodoc-0.3.1/quartodoc/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.3.1/quartodoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: mc_al_github@fastmail.com
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `quartodoc-0.3.0/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.3.1/quartodoc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -57,18 +57,21 @@
 examples/pkgdown/reference/get_object.qmd
 examples/pkgdown/reference/index.qmd
 examples/pkgdown/reference/preview.qmd
 examples/single-page/.gitignore
 examples/single-page/_quarto.yml
 examples/single-page/objects.json
 examples/single-page/reference/index.qmd
+examples/weird-install/_quarto.yml
+examples/weird-install/src/some_module.py
 quartodoc/__init__.py
 quartodoc/__main__.py
 quartodoc/ast.py
 quartodoc/autosummary.py
+quartodoc/interlinks.py
 quartodoc/inventory.py
 quartodoc/layout.py
 quartodoc.egg-info/PKG-INFO
 quartodoc.egg-info/SOURCES.txt
 quartodoc.egg-info/dependency_links.txt
 quartodoc.egg-info/entry_points.txt
 quartodoc.egg-info/requires.txt
@@ -88,10 +91,15 @@
 quartodoc/tests/example_attribute.py
 quartodoc/tests/example_dynamic.py
 quartodoc/tests/example_signature.py
 quartodoc/tests/test_ast.py
 quartodoc/tests/test_basic.py
 quartodoc/tests/test_builder.py
 quartodoc/tests/test_builder_blueprint.py
-quartodoc/tests/test_inventory.py
+quartodoc/tests/test_interlinks.py
 quartodoc/tests/test_layout.py
-quartodoc/tests/test_renderers.py
+quartodoc/tests/test_renderers.py
+quartodoc/tests/example_interlinks/README.md
+quartodoc/tests/example_interlinks/_quarto.yml
+quartodoc/tests/example_interlinks/objects.json
+quartodoc/tests/example_interlinks/spec.yml
+quartodoc/tests/example_interlinks/_inv/other_objects.json
```

### Comparing `quartodoc-0.3.0/requirements-dev.txt` & `quartodoc-0.3.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.0/setup.cfg` & `quartodoc-0.3.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 install_requires = 
 	griffe==0.25
 	plum-dispatch<2.0.0;python_version<'3.10'
 	plum-dispatch;python_version>='3.10'
 	sphobjinv
 	tabulate
 	importlib-metadata
+	importlib-resources
 	panflute
 	pydantic
 	typing-extensions
 
 [options.extras_require]
 dev = 
 	pytest
```

