# Comparing `tmp/pyikarus-0.3.0.dev202310000061.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000062.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000061.tar", last modified: Wed May 10 14:10:14 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000062.tar", last modified: Mon May 15 07:57:36 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000061.tar` & `pyikarus-0.3.0.dev202310000062.tar`

### file list

```diff
@@ -1,319 +1,324 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.902535 pyikarus-0.3.0.dev202310000061/
--rwxrwxrwx   0 root         (0) root         (0)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.bettercodehub.yml
--rwxrwxrwx   0 root         (0) root         (0)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.clang-format
--rwxrwxrwx   0 root         (0) root         (0)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:09.899658 pyikarus-0.3.0.dev202310000061/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.340819 pyikarus-0.3.0.dev202310000061/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 root         (0) root         (0)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.498914 pyikarus-0.3.0.dev202310000061/.github/workflows/
--rwxrwxrwx   0 root         (0) root         (0)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/codespell.yml
--rwxrwxrwx   0 root         (0) root         (0)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/createDockerContainer.yml
--rwxrwxrwx   0 root         (0) root         (0)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/createRelease.yml
--rwxrwxrwx   0 root         (0) root         (0)     1635 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/debian-coverage.yml
--rwxrwxrwx   0 root         (0) root         (0)     2108 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/debian.yml
--rwxrwxrwx   0 root         (0) root         (0)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/ghpages.yml
--rwxrwxrwx   0 root         (0) root         (0)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/reuseLint.yml
--rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/runExamples.yml
--rwxrwxrwx   0 root         (0) root         (0)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.github/workflows/style.yml
--rwxrwxrwx   0 root         (0) root         (0)      455 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.516358 pyikarus-0.3.0.dev202310000061/.reuse/
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/.reuse/dep5
--rwxrwxrwx   0 root         (0) root         (0)     3063 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1319 2023-05-10 12:56:29.000000 pyikarus-0.3.0.dev202310000061/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 root         (0) root         (0)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.570007 pyikarus-0.3.0.dev202310000061/LICENSES/
--rwxrwxrwx   0 root         (0) root         (0)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/LICENSES/CC-BY-SA-4.0.txt
--rwxrwxrwx   0 root         (0) root         (0)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/LICENSES/CC0-1.0.txt
--rwxrwxrwx   0 root         (0) root         (0)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/LICENSES/LGPL-3.0-or-later.txt
--rwxrwxrwx   0 root         (0) root         (0)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3638 2023-05-10 14:10:14.899533 pyikarus-0.3.0.dev202310000061/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.596047 pyikarus-0.3.0.dev202310000061/cmake/
--rwxrwxrwx   0 root         (0) root         (0)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.611464 pyikarus-0.3.0.dev202310000061/cmake/FormatTarget/
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.706738 pyikarus-0.3.0.dev202310000061/cmake/modules/
--rwxrwxrwx   0 root         (0) root         (0)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/modules/AddAutoDiffFlags.cmake
--rwxrwxrwx   0 root         (0) root         (0)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/modules/AddEigenFlags.cmake
--rwxrwxrwx   0 root         (0) root         (0)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/modules/AddMatplotppFlags.cmake
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/modules/AddSpdlogFlags.cmake
--rwxrwxrwx   0 root         (0) root         (0)      226 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/modules/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)      446 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/modules/IkarusMacros.cmake
--rwxrwxrwx   0 root         (0) root         (0)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/cmake/tools.cmake
--rwxrwxrwx   0 root         (0) root         (0)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/codecov.yml
--rwxrwxrwx   0 root         (0) root         (0)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/codespellignore
--rwxrwxrwx   0 root         (0) root         (0)     1588 2023-05-10 12:14:52.000000 pyikarus-0.3.0.dev202310000061/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.778592 pyikarus-0.3.0.dev202310000061/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.793890 pyikarus-0.3.0.dev202310000061/docs/BuildLocally/
--rwxrwxrwx   0 root         (0) root         (0)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/BuildLocally/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.825258 pyikarus-0.3.0.dev202310000061/docs/__pycache__/
--rwxrwxrwx   0 root         (0) root         (0)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000061/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rwxrwxrwx   0 root         (0) root         (0)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/literature.bib
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/literature.bib.license
--rwxrwxrwx   0 root         (0) root         (0)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/mkdocs-macros.py
--rwxrwxrwx   0 root         (0) root         (0)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/mkdocs.insiders.yml
--rwxrwxrwx   0 root         (0) root         (0)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:09.930780 pyikarus-0.3.0.dev202310000061/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.843273 pyikarus-0.3.0.dev202310000061/docs/overrides/partials/
--rwxrwxrwx   0 root         (0) root         (0)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:10.909862 pyikarus-0.3.0.dev202310000061/docs/website/
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.188846 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/
--rwxrwxrwx   0 root         (0) root         (0)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/assembler.md
--rwxrwxrwx   0 root         (0) root         (0)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/controlRoutines.md
--rwxrwxrwx   0 root         (0) root         (0)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/dirichletBCs.md
--rwxrwxrwx   0 root         (0) root         (0)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/feRequirements.md
--rwxrwxrwx   0 root         (0) root         (0)     8527 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/finiteElements.md
--rwxrwxrwx   0 root         (0) root         (0)     2745 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/grids.md
--rwxrwxrwx   0 root         (0) root         (0)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/index.md
--rwxrwxrwx   0 root         (0) root         (0)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/localBasis.md
--rwxrwxrwx   0 root         (0) root         (0)    44233 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/localFunctions.md
--rwxrwxrwx   0 root         (0) root         (0)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/manifolds.md
--rwxrwxrwx   0 root         (0) root         (0)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/nonlinearOperator.md
--rwxrwxrwx   0 root         (0) root         (0)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/observer.md
--rwxrwxrwx   0 root         (0) root         (0)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.397701 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/
--rwxrwxrwx   0 root         (0) root         (0)     6675 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/cantileverBeam.md
--rwxrwxrwx   0 root         (0) root         (0)     7271 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/computePi.md
--rwxrwxrwx   0 root         (0) root         (0)     5477 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/cooksMembrane.md
--rwxrwxrwx   0 root         (0) root         (0)     7051 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/incompressibleRubberBlock.md
--rwxrwxrwx   0 root         (0) root         (0)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/index.md
--rwxrwxrwx   0 root         (0) root         (0)     7719 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/kirchhoffPlate.md
--rwxrwxrwx   0 root         (0) root         (0)     5134 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/newtonRaphsonMethod.md
--rwxrwxrwx   0 root         (0) root         (0)     6149 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/nonLinearElasticity.md
--rwxrwxrwx   0 root         (0) root         (0)     4090 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.470831 pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/
--rwxrwxrwx   0 root         (0) root         (0)     2439 2023-05-10 12:50:55.000000 pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/buildDocumentationLocally.md
--rwxrwxrwx   0 root         (0) root         (0)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/codeStyle.md
--rwxrwxrwx   0 root         (0) root         (0)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/howToEdit.md
--rwxrwxrwx   0 root         (0) root         (0)     1762 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.514064 pyikarus-0.3.0.dev202310000061/docs/website/04_blog/
--rwxrwxrwx   0 root         (0) root         (0)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/04_blog/.authors.yml
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.534065 pyikarus-0.3.0.dev202310000061/docs/website/04_blog/posts/
--rwxrwxrwx   0 root         (0) root         (0)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.554012 pyikarus-0.3.0.dev202310000061/docs/website/05_cppReferences/
--rwxrwxrwx   0 root         (0) root         (0)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.570521 pyikarus-0.3.0.dev202310000061/docs/website/99_Literature/
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.645839 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:11.875628 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/
--rwxrwxrwx   0 root         (0) root         (0)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rwxrwxrwx   0 root         (0) root         (0)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rwxrwxrwx   0 root         (0) root         (0)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rwxrwxrwx   0 root         (0) root         (0)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rwxrwxrwx   0 root         (0) root         (0)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.125271 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/
--rwxrwxrwx   0 root         (0) root         (0)    35234 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rwxrwxrwx   0 root         (0) root         (0)    62184 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rwxrwxrwx   0 root         (0) root         (0)     2281 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rwxrwxrwx   0 root         (0) root         (0)    40033 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rwxrwxrwx   0 root         (0) root         (0)    25505 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rwxrwxrwx   0 root         (0) root         (0)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/logo_blue.svg
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/logo_blue.svg.license
--rwxrwxrwx   0 root         (0) root         (0)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/logo_white.svg
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/logo_white.svg.license
--rwxrwxrwx   0 root         (0) root         (0)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/download.md
--rwxrwxrwx   0 root         (0) root         (0)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/gallery.md
--rwxrwxrwx   0 root         (0) root         (0)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.145581 pyikarus-0.3.0.dev202310000061/docs/website/javascripts/
--rwxrwxrwx   0 root         (0) root         (0)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.165863 pyikarus-0.3.0.dev202310000061/docs/website/stylesheets/
--rwxrwxrwx   0 root         (0) root         (0)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/docs/website/stylesheets/extra.css
--rwxrwxrwx   0 root         (0) root         (0)      502 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.181086 pyikarus-0.3.0.dev202310000061/ikarus/
--rwxrwxrwx   0 root         (0) root         (0)      748 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.230954 pyikarus-0.3.0.dev202310000061/ikarus/assembler/
--rwxrwxrwx   0 root         (0) root         (0)      268 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)    11012 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/assembler/simpleAssemblers.hh
--rwxrwxrwx   0 root         (0) root         (0)    10681 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.285647 pyikarus-0.3.0.dev202310000061/ikarus/controlRoutines/
--rwxrwxrwx   0 root         (0) root         (0)      239 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/controlRoutines/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     2575 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/controlRoutines/loadControl.hh
--rwxrwxrwx   0 root         (0) root         (0)     2970 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.392149 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/
--rwxrwxrwx   0 root         (0) root         (0)      349 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)      185 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.476199 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/
--rwxrwxrwx   0 root         (0) root         (0)      282 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     2649 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/autodiffFE.hh
--rwxrwxrwx   0 root         (0) root         (0)     2151 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/powerBasisFE.hh
--rwxrwxrwx   0 root         (0) root         (0)     1701 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/scalarFE.hh
--rwxrwxrwx   0 root         (0) root         (0)     1041 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feRequirements.cpp
--rwxrwxrwx   0 root         (0) root         (0)     8419 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feRequirements.hh
--rwxrwxrwx   0 root         (0) root         (0)     1338 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.586151 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/
--rwxrwxrwx   0 root         (0) root         (0)      345 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)    20311 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rwxrwxrwx   0 root         (0) root         (0)    12753 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.769495 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/
--rwxrwxrwx   0 root         (0) root         (0)      397 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     5699 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/interface.hh
--rwxrwxrwx   0 root         (0) root         (0)     2718 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rwxrwxrwx   0 root         (0) root         (0)     4635 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rwxrwxrwx   0 root         (0) root         (0)     3809 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rwxrwxrwx   0 root         (0) root         (0)     5734 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/svk.hh
--rwxrwxrwx   0 root         (0) root         (0)      473 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/tags.hh
--rwxrwxrwx   0 root         (0) root         (0)     8010 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rwxrwxrwx   0 root         (0) root         (0)     1196 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials.hh
--rwxrwxrwx   0 root         (0) root         (0)     7966 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rwxrwxrwx   0 root         (0) root         (0)    12655 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.834622 pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/
--rwxrwxrwx   0 root         (0) root         (0)      301 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     6448 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/dirichletValues.hh
--rwxrwxrwx   0 root         (0) root         (0)     7791 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/nonLinearOperator.hh
--rwxrwxrwx   0 root         (0) root         (0)    12303 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.851279 pyikarus-0.3.0.dev202310000061/ikarus/python/
--rwxrwxrwx   0 root         (0) root         (0)      270 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.889770 pyikarus-0.3.0.dev202310000061/ikarus/python/assembler/
--rwxrwxrwx   0 root         (0) root         (0)      249 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/assembler/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     3115 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.932459 pyikarus-0.3.0.dev202310000061/ikarus/python/dirichletValues/
--rwxrwxrwx   0 root         (0) root         (0)      257 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/dirichletValues/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     4116 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:12.993089 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     5526 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.037011 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/materials/
--rwxrwxrwx   0 root         (0) root         (0)      259 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/materials/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     5107 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/materials/material.hh
--rwxrwxrwx   0 root         (0) root         (0)     5419 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.181844 pyikarus-0.3.0.dev202310000061/ikarus/python/test/
--rwxrwxrwx   0 root         (0) root         (0)      787 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     3808 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/linearElasticTest.py
--rwxrwxrwx   0 root         (0) root         (0)     1839 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/nameTest.vtu
--rwxrwxrwx   0 root         (0) root         (0)     4444 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/nonLinearElasticTest.py
--rwxrwxrwx   0 root         (0) root         (0)      862 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/setpath.py.in
--rwxrwxrwx   0 root         (0) root         (0)      321 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/test1.py
--rwxrwxrwx   0 root         (0) root         (0)      582 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/test/test2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.222700 pyikarus-0.3.0.dev202310000061/ikarus/python/utils/
--rwxrwxrwx   0 root         (0) root         (0)      245 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/utils/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     1434 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.241557 pyikarus-0.3.0.dev202310000061/ikarus/solver/
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.283606 pyikarus-0.3.0.dev202310000061/ikarus/solver/linearSolver/
--rwxrwxrwx   0 root         (0) root         (0)      244 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/linearSolver/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     8891 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.365942 pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/
--rwxrwxrwx   0 root         (0) root         (0)      272 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     5407 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rwxrwxrwx   0 root         (0) root         (0)     8297 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rwxrwxrwx   0 root         (0) root         (0)    18574 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.698827 pyikarus-0.3.0.dev202310000061/ikarus/utils/
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     1741 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/algorithms.hh
--rwxrwxrwx   0 root         (0) root         (0)      878 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/autodiffHelper.hh
--rwxrwxrwx   0 root         (0) root         (0)     6930 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/concepts.hh
--rwxrwxrwx   0 root         (0) root         (0)      503 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.776002 pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/
--rwxrwxrwx   0 root         (0) root         (0)      262 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     1654 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/griddrawer.hh
--rwxrwxrwx   0 root         (0) root         (0)      544 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/matplotHelper.cpp
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/matplotHelper.hh
--rwxrwxrwx   0 root         (0) root         (0)     2484 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/duneUtilities.hh
--rwxrwxrwx   0 root         (0) root         (0)     2347 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/eigenDuneTransformations.hh
--rwxrwxrwx   0 root         (0) root         (0)      682 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/eigenSparseAddon.hh
--rwxrwxrwx   0 root         (0) root         (0)     1367 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/findLineSegment.cpp
--rwxrwxrwx   0 root         (0) root         (0)      724 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/findLineSegment.hh
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/functionSanityChecks.cpp
--rwxrwxrwx   0 root         (0) root         (0)     6359 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/functionSanityChecks.hh
--rwxrwxrwx   0 root         (0) root         (0)     3152 2023-05-10 12:14:52.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/init.hh
--rwxrwxrwx   0 root         (0) root         (0)    15244 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/linearAlgebraHelper.hh
--rwxrwxrwx   0 root         (0) root         (0)     1711 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.952386 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/
--rwxrwxrwx   0 root         (0) root         (0)      450 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     1554 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/controlLogger.hh
--rwxrwxrwx   0 root         (0) root         (0)     2307 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/controlVTKWriter.hh
--rwxrwxrwx   0 root         (0) root         (0)      905 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/genericControlObserver.hh
--rwxrwxrwx   0 root         (0) root         (0)     1053 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/gridDrawerObserver.hh
--rwxrwxrwx   0 root         (0) root         (0)     1132 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/loadControlObserver.hh
--rwxrwxrwx   0 root         (0) root         (0)     1985 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/nonLinearSolverLogger.hh
--rwxrwxrwx   0 root         (0) root         (0)     5497 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/observer.hh
--rwxrwxrwx   0 root         (0) root         (0)      489 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/observerMessages.hh
--rwxrwxrwx   0 root         (0) root         (0)     4159 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/pathFollowingFunctions.hh
--rwxrwxrwx   0 root         (0) root         (0)     1131 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/polyfit.cpp
--rwxrwxrwx   0 root         (0) root         (0)      570 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/polyfit.hh
--rwxrwxrwx   0 root         (0) root         (0)    10054 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/tensorUtils.hh
--rwxrwxrwx   0 root         (0) root         (0)    15044 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus/utils/traits.hh
--rwxrwxrwx   0 root         (0) root         (0)      432 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/ikarus.pc.in
--rwxrwxrwx   0 root         (0) root         (0)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/iwyu.imp
--rwxrwxrwx   0 root         (0) root         (0)      305 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:13.978906 pyikarus-0.3.0.dev202310000061/python/
--rwxrwxrwx   0 root         (0) root         (0)      405 2023-05-10 14:08:02.000000 pyikarus-0.3.0.dev202310000061/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.071433 pyikarus-0.3.0.dev202310000061/python/ikarus/
--rwxrwxrwx   0 root         (0) root         (0)      511 2023-05-10 13:32:18.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5636 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.113354 pyikarus-0.3.0.dev202310000061/python/ikarus/assembler/
--rwxrwxrwx   0 root         (0) root         (0)      167 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     2300 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/assembler/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1408 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.155134 pyikarus-0.3.0.dev202310000061/python/ikarus/finite_elements/
--rwxrwxrwx   0 root         (0) root         (0)      173 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/finite_elements/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     3465 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/finite_elements/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1792 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.194636 pyikarus-0.3.0.dev202310000061/python/ikarus/utils/
--rwxrwxrwx   0 root         (0) root         (0)      163 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     1461 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.283977 pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3638 2023-05-10 14:10:08.000000 pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9785 2023-05-10 14:10:09.000000 pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 14:10:08.000000 pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-10 14:10:08.000000 pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-10 14:10:08.000000 pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      638 2023-05-10 14:08:02.000000 pyikarus-0.3.0.dev202310000061/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.298910 pyikarus-0.3.0.dev202310000061/sandbox/
--rwxrwxrwx   0 root         (0) root         (0)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.334645 pyikarus-0.3.0.dev202310000061/sandbox/src/
--rwxrwxrwx   0 root         (0) root         (0)     1220 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.356944 pyikarus-0.3.0.dev202310000061/sandbox/src/auxiliaryFiles/
--rwxrwxrwx   0 root         (0) root         (0)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/sandbox/src/auxiliaryFiles/circle.msh
--rwxrwxrwx   0 root         (0) root         (0)      320 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 14:10:14.903360 pyikarus-0.3.0.dev202310000061/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1864 2023-05-10 14:10:06.000000 pyikarus-0.3.0.dev202310000061/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.383175 pyikarus-0.3.0.dev202310000061/tests/
--rwxrwxrwx   0 root         (0) root         (0)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.785688 pyikarus-0.3.0.dev202310000061/tests/src/
--rwxrwxrwx   0 root         (0) root         (0)     1397 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/tests/src/CMakeLists.txt
--rwxrwxrwx   0 root         (0) root         (0)     3888 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/assemblerTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     9913 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/common.hh
--rwxrwxrwx   0 root         (0) root         (0)     2639 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/dependenciesTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     6409 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/dirichletValueTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3820 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/easTest.hh
--rwxrwxrwx   0 root         (0) root         (0)     1473 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/enhancedAssumedStrainsTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/tests/src/factories.hh
--rwxrwxrwx   0 root         (0) root         (0)     1870 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/functionTraitsTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     2221 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/linearElasticityTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     2378 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/manifoldsTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     7961 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/materialTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     6561 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/nonLinearElasticityTest.hh
--rwxrwxrwx   0 root         (0) root         (0)      724 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rwxrwxrwx   0 root         (0) root         (0)      729 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/tests/src/nonLinearElasticityTestSVK.cpp
--rwxrwxrwx   0 root         (0) root         (0)     9936 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/nonLinearOperatorTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     6327 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/pathFollowingTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1651 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/polyFitTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)      695 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/pythonConversionTest.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1292 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/testAutodiffHelper.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5702 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/testFEElement.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:10:14.882121 pyikarus-0.3.0.dev202310000061/tests/src/testFiles/
--rwxrwxrwx   0 root         (0) root         (0)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredQuadscoarse.msh
--rwxrwxrwx   0 root         (0) root         (0)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredTest.geo
--rwxrwxrwx   0 root         (0) root         (0)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredTest.msh
--rwxrwxrwx   0 root         (0) root         (0)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredTest2.geo
--rwxrwxrwx   0 root         (0) root         (0)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredTrianglesfine.msh
--rwxrwxrwx   0 root         (0) root         (0)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000061/tests/src/testHelpers.hh
--rwxrwxrwx   0 root         (0) root         (0)    17595 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000061/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.862806 pyikarus-0.3.0.dev202310000062/
+-rw-r--r--   0 user      (1001) user      (1001)      312 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/.bettercodehub.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1300 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/.clang-format
+-rw-r--r--   0 user      (1001) user      (1001)     1017 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/.cmake-format
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.754807 pyikarus-0.3.0.dev202310000062/.github/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.770806 pyikarus-0.3.0.dev202310000062/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 user      (1001) user      (1001)      460 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 user      (1001) user      (1001)      615 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.770806 pyikarus-0.3.0.dev202310000062/.github/workflows/
+-rw-r--r--   0 user      (1001) user      (1001)      476 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/codespell.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1034 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 user      (1001) user      (1001)     4900 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/createRelease.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1635 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 user      (1001) user      (1001)     2414 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/debian.yml
+-rw-r--r--   0 user      (1001) user      (1001)     2042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/ghpages.yml
+-rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/reuseLint.yml
+-rw-r--r--   0 user      (1001) user      (1001)     2854 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/runExamples.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1212 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/.github/workflows/style.yml
+-rw-r--r--   0 user      (1001) user      (1001)      457 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/.gitignore
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.770806 pyikarus-0.3.0.dev202310000062/.reuse/
+-rw-r--r--   0 user      (1001) user      (1001)      661 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/.reuse/dep5
+-rw-r--r--   0 user      (1001) user      (1001)     3274 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/CHANGELOG.md
+-rw-r--r--   0 user      (1001) user      (1001)     1318 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5335 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/CODE_OF_CONDUCT.md
+-rw-r--r--   0 user      (1001) user      (1001)      759 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/LICENSE.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.774807 pyikarus-0.3.0.dev202310000062/LICENSES/
+-rw-r--r--   0 user      (1001) user      (1001)    18375 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     7048 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)    42098 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1078 2023-03-24 20:46:08.000000 pyikarus-0.3.0.dev202310000062/LICENSES/MIT.txt
+-rw-r--r--   0 user      (1001) user      (1001)    16727 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-15 07:57:36.862806 pyikarus-0.3.0.dev202310000062/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     3229 2023-03-06 10:17:28.000000 pyikarus-0.3.0.dev202310000062/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.774807 pyikarus-0.3.0.dev202310000062/cmake/
+-rw-r--r--   0 user      (1001) user      (1001)      973 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/cmake/CPM.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.774807 pyikarus-0.3.0.dev202310000062/cmake/FormatTarget/
+-rw-r--r--   0 user      (1001) user      (1001)     1270 2023-03-10 08:15:25.000000 pyikarus-0.3.0.dev202310000062/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.778807 pyikarus-0.3.0.dev202310000062/cmake/modules/
+-rw-r--r--   0 user      (1001) user      (1001)      715 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      683 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      740 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      691 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      226 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      446 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 user      (1001) user      (1001)     2040 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/cmake/tools.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      148 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/codecov.yml
+-rw-r--r--   0 user      (1001) user      (1001)      121 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/codespellignore
+-rw-r--r--   0 user      (1001) user      (1001)     1588 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/config.h.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.778807 pyikarus-0.3.0.dev202310000062/docs/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.778807 pyikarus-0.3.0.dev202310000062/docs/BuildLocally/
+-rw-r--r--   0 user      (1001) user      (1001)      439 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      333 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.782806 pyikarus-0.3.0.dev202310000062/docs/__pycache__/
+-rw-r--r--   0 user      (1001) user      (1001)     1136 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 user      (1001) user      (1001)     6961 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/literature.bib
+-rw-r--r--   0 user      (1001) user      (1001)      117 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/literature.bib.license
+-rw-r--r--   0 user      (1001) user      (1001)     1245 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/mkdocs-macros.py
+-rw-r--r--   0 user      (1001) user      (1001)      394 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/mkdocs.insiders.yml
+-rw-r--r--   0 user      (1001) user      (1001)     5042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/docs/mkdocs.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.758807 pyikarus-0.3.0.dev202310000062/docs/overrides/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.782806 pyikarus-0.3.0.dev202310000062/docs/overrides/partials/
+-rw-r--r--   0 user      (1001) user      (1001)     1732 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/overrides/partials/comments.html
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.782806 pyikarus-0.3.0.dev202310000062/docs/website/
+-rw-r--r--   0 user      (1001) user      (1001)       24 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/.meta.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.786806 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/
+-rw-r--r--   0 user      (1001) user      (1001)     4710 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/assembler.md
+-rw-r--r--   0 user      (1001) user      (1001)     6387 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 user      (1001) user      (1001)     2024 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 user      (1001) user      (1001)     3237 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 user      (1001) user      (1001)     8524 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 user      (1001) user      (1001)     2745 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/grids.md
+-rw-r--r--   0 user      (1001) user      (1001)     4121 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/index.md
+-rw-r--r--   0 user      (1001) user      (1001)     4932 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 user      (1001) user      (1001)    44213 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 user      (1001) user      (1001)     3978 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 user      (1001) user      (1001)     2590 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 user      (1001) user      (1001)     3086 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/observer.md
+-rw-r--r--   0 user      (1001) user      (1001)     5211 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.790806 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/
+-rw-r--r--   0 user      (1001) user      (1001)     6655 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 user      (1001) user      (1001)     7251 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/computePi.md
+-rw-r--r--   0 user      (1001) user      (1001)     5439 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 user      (1001) user      (1001)     7055 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 user      (1001) user      (1001)     2164 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/index.md
+-rw-r--r--   0 user      (1001) user      (1001)     7702 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 user      (1001) user      (1001)     5114 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 user      (1001) user      (1001)     6200 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 user      (1001) user      (1001)     4071 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.790806 pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/
+-rw-r--r--   0 user      (1001) user      (1001)     2439 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 user      (1001) user      (1001)     1002 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 user      (1001) user      (1001)     2415 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 user      (1001) user      (1001)     1762 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.790806 pyikarus-0.3.0.dev202310000062/docs/website/04_blog/
+-rw-r--r--   0 user      (1001) user      (1001)      274 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/04_blog/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.790806 pyikarus-0.3.0.dev202310000062/docs/website/04_blog/posts/
+-rw-r--r--   0 user      (1001) user      (1001)     7731 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.790806 pyikarus-0.3.0.dev202310000062/docs/website/05_cppReferences/
+-rw-r--r--   0 user      (1001) user      (1001)     2324 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.790806 pyikarus-0.3.0.dev202310000062/docs/website/99_Literature/
+-rw-r--r--   0 user      (1001) user      (1001)      169 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.794807 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.794807 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 user      (1001) user      (1001)    52795 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    46250 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     2852 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    17924 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     9455 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.798807 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 user      (1001) user      (1001)    35234 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    62184 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     2281 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    40033 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    25505 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     8101 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/logo_blue.svg
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/logo_blue.svg.license
+-rw-r--r--   0 user      (1001) user      (1001)     8255 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/logo_white.svg
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/logo_white.svg.license
+-rw-r--r--   0 user      (1001) user      (1001)     4364 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000062/docs/website/download.md
+-rw-r--r--   0 user      (1001) user      (1001)      244 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/gallery.md
+-rw-r--r--   0 user      (1001) user      (1001)     1358 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.798807 pyikarus-0.3.0.dev202310000062/docs/website/javascripts/
+-rw-r--r--   0 user      (1001) user      (1001)      486 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.798807 pyikarus-0.3.0.dev202310000062/docs/website/stylesheets/
+-rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/docs/website/stylesheets/extra.css
+-rw-r--r--   0 user      (1001) user      (1001)      502 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/dune.module
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.798807 pyikarus-0.3.0.dev202310000062/ikarus/
+-rw-r--r--   0 user      (1001) user      (1001)      748 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/ikarus/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.802806 pyikarus-0.3.0.dev202310000062/ikarus/assembler/
+-rw-r--r--   0 user      (1001) user      (1001)      268 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)    11069 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 user      (1001) user      (1001)    10714 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.802806 pyikarus-0.3.0.dev202310000062/ikarus/controlRoutines/
+-rw-r--r--   0 user      (1001) user      (1001)      239 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     2575 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2970 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.802806 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/
+-rw-r--r--   0 user      (1001) user      (1001)      349 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      185 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.802806 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/
+-rw-r--r--   0 user      (1001) user      (1001)      282 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     2925 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2305 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1827 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1041 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feRequirements.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     8419 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1338 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.806806 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 user      (1001) user      (1001)      345 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)    19628 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 user      (1001) user      (1001)    12549 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.806806 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 user      (1001) user      (1001)      397 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5699 2023-05-08 12:58:29.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2718 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 user      (1001) user      (1001)     4635 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 user      (1001) user      (1001)     3809 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 user      (1001) user      (1001)     5734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 user      (1001) user      (1001)      473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 user      (1001) user      (1001)     8010 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1196 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 user      (1001) user      (1001)     7827 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 user      (1001) user      (1001)    12655 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.810807 pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/
+-rw-r--r--   0 user      (1001) user      (1001)      301 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     6734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 user      (1001) user      (1001)     7791 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 user      (1001) user      (1001)    12303 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.810807 pyikarus-0.3.0.dev202310000062/ikarus/python/
+-rw-r--r--   0 user      (1001) user      (1001)      294 2023-05-12 13:45:59.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.810807 pyikarus-0.3.0.dev202310000062/ikarus/python/assembler/
+-rw-r--r--   0 user      (1001) user      (1001)      249 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3149 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.810807 pyikarus-0.3.0.dev202310000062/ikarus/python/basis/
+-rw-r--r--   0 user      (1001) user      (1001)      237 2023-05-12 13:45:59.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     4559 2023-05-15 07:38:08.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.810807 pyikarus-0.3.0.dev202310000062/ikarus/python/dirichletValues/
+-rw-r--r--   0 user      (1001) user      (1001)      257 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     4116 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.814807 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/
+-rw-r--r--   0 user      (1001) user      (1001)      303 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5036 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.814807 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 user      (1001) user      (1001)      259 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5107 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 user      (1001) user      (1001)     5503 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.818807 pyikarus-0.3.0.dev202310000062/ikarus/python/test/
+-rw-r--r--   0 user      (1001) user      (1001)      564 2023-05-12 13:45:59.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3977 2023-05-12 13:45:59.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 user      (1001) user      (1001)  2704357 2023-05-15 07:48:32.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/test/nameTest.vtu
+-rw-r--r--   0 user      (1001) user      (1001)     4446 2023-05-15 07:38:08.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 user      (1001) user      (1001)      862 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.822806 pyikarus-0.3.0.dev202310000062/ikarus/python/utils/
+-rw-r--r--   0 user      (1001) user      (1001)      245 2023-05-12 13:45:59.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1181 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.822806 pyikarus-0.3.0.dev202310000062/ikarus/solver/
+-rw-r--r--   0 user      (1001) user      (1001)      211 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.822806 pyikarus-0.3.0.dev202310000062/ikarus/solver/linearSolver/
+-rw-r--r--   0 user      (1001) user      (1001)      244 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     8891 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.822806 pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 user      (1001) user      (1001)      272 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5407 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 user      (1001) user      (1001)     8297 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 user      (1001) user      (1001)    18574 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.830807 pyikarus-0.3.0.dev202310000062/ikarus/utils/
+-rw-r--r--   0 user      (1001) user      (1001)      712 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1741 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/algorithms.hh
+-rw-r--r--   0 user      (1001) user      (1001)      878 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1445 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/basis.hh
+-rw-r--r--   0 user      (1001) user      (1001)     6930 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/concepts.hh
+-rw-r--r--   0 user      (1001) user      (1001)      503 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.830807 pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/
+-rw-r--r--   0 user      (1001) user      (1001)      262 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1654 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 user      (1001) user      (1001)      544 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      703 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2484 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2347 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 user      (1001) user      (1001)      682 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1367 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      724 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 user      (1001) user      (1001)     3611 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2171 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6359 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 user      (1001) user      (1001)     3152 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/init.hh
+-rw-r--r--   0 user      (1001) user      (1001)    15244 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1711 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.834807 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/
+-rw-r--r--   0 user      (1001) user      (1001)      450 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1554 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2307 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 user      (1001) user      (1001)      905 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1053 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1132 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1985 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 user      (1001) user      (1001)     5497 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 user      (1001) user      (1001)      489 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 user      (1001) user      (1001)     4159 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1131 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      570 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/polyfit.hh
+-rw-r--r--   0 user      (1001) user      (1001)    10054 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 user      (1001) user      (1001)    15044 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/ikarus/utils/traits.hh
+-rw-r--r--   0 user      (1001) user      (1001)      432 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/ikarus.pc.in
+-rw-r--r--   0 user      (1001) user      (1001)      196 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/iwyu.imp
+-rw-r--r--   0 user      (1001) user      (1001)      422 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.834807 pyikarus-0.3.0.dev202310000062/python/
+-rw-r--r--   0 user      (1001) user      (1001)      403 2023-05-15 07:38:08.000000 pyikarus-0.3.0.dev202310000062/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.838806 pyikarus-0.3.0.dev202310000062/python/ikarus/
+-rw-r--r--   0 user      (1001) user      (1001)      517 2023-05-15 07:38:08.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      603 2023-05-12 13:45:59.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     5636 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.838806 pyikarus-0.3.0.dev202310000062/python/ikarus/assembler/
+-rw-r--r--   0 user      (1001) user      (1001)      167 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     2300 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     1491 2023-05-15 07:45:57.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/basis.py
+-rw-r--r--   0 user      (1001) user      (1001)     1408 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.838806 pyikarus-0.3.0.dev202310000062/python/ikarus/finite_elements/
+-rw-r--r--   0 user      (1001) user      (1001)      173 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3465 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     1792 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.842806 pyikarus-0.3.0.dev202310000062/python/ikarus/utils/
+-rw-r--r--   0 user      (1001) user      (1001)      163 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1496 2023-05-15 07:46:07.000000 pyikarus-0.3.0.dev202310000062/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.842806 pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-15 07:57:36.000000 pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     9884 2023-05-15 07:57:36.000000 pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-15 07:57:36.000000 pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-15 07:57:36.000000 pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-15 07:57:36.000000 pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) user      (1001)      636 2023-05-15 07:38:08.000000 pyikarus-0.3.0.dev202310000062/python/setup.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.842806 pyikarus-0.3.0.dev202310000062/sandbox/
+-rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/sandbox/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.846806 pyikarus-0.3.0.dev202310000062/sandbox/src/
+-rw-r--r--   0 user      (1001) user      (1001)     1220 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000062/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.846806 pyikarus-0.3.0.dev202310000062/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 user      (1001) user      (1001)   674469 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 user      (1001) user      (1001)      320 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/sandbox/src/sandbox.cpp
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-15 07:57:36.862806 pyikarus-0.3.0.dev202310000062/setup.cfg
+-rw-r--r--   0 user      (1001) user      (1001)     1864 2023-05-15 07:57:21.000000 pyikarus-0.3.0.dev202310000062/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.846806 pyikarus-0.3.0.dev202310000062/tests/
+-rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/tests/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.858806 pyikarus-0.3.0.dev202310000062/tests/src/
+-rw-r--r--   0 user      (1001) user      (1001)     1418 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3906 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/tests/src/assemblerTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     9913 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/common.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2639 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/dependenciesTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6520 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/dirichletValueTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     3820 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/easTest.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/enhancedAssumedStrainsTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      608 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/factories.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1870 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/functionTraitsTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     2661 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/linearElasticityTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     2378 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/manifoldsTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     7961 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/materialTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6770 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000062/tests/src/nonLinearElasticityTest.hh
+-rw-r--r--   0 user      (1001) user      (1001)      724 2023-05-08 13:07:10.000000 pyikarus-0.3.0.dev202310000062/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      729 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/nonLinearElasticityTestSVK.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     9936 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/nonLinearOperatorTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6327 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/pathFollowingTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     1651 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/polyFitTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      695 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/pythonConversionTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     1292 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     5805 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/testFEElement.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 07:57:36.858806 pyikarus-0.3.0.dev202310000062/tests/src/testFiles/
+-rw-r--r--   0 user      (1001) user      (1001)     9028 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 user      (1001) user      (1001)      395 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 user      (1001) user      (1001)      497 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 user      (1001) user      (1001)      546 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 user      (1001) user      (1001)    11431 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 user      (1001) user      (1001)     1114 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000062/tests/src/testHelpers.hh
+-rw-r--r--   0 user      (1001) user      (1001)    17595 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000062/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000061/.clang-format` & `pyikarus-0.3.0.dev202310000062/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.cmake-format` & `pyikarus-0.3.0.dev202310000062/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.0.dev202310000062/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/createRelease.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/debian.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/debian.yml`

 * *Files 13% similar despite different names*

```diff
@@ -35,32 +35,42 @@
 #            lib: "-stdlib=libc++",
 #           }
           - {
             name: "GCC-Debug",
             config: Debug,
             compilerC: gcc-12,
             compilerCxx: g++-12,
-            lib: ""
+            lib: "",
+            testRegex: "cpp"
           }
           - {
             name: "GCC-Release",
             config: Release,
             compilerC: gcc-12,
             compilerCxx: g++-12,
-            lib: ""
+            lib: "",
+            testRegex: "cpp"
+          }
+          - {
+            name: "GCC-Release-Python",
+            config: Release,
+            compilerC: gcc-12,
+            compilerCxx: g++-12,
+            lib: "",
+            testRegex: "python"
           }
     steps:
       - uses: actions/checkout@v2
         with:
          path: 'repo'
       - name: Build
         working-directory: ./repo
         run: |
           mkdir cmake-build-${{ matrix.config.config }}
           cd cmake-build-${{ matrix.config.config }}
           cmake ../  -DCMAKE_BUILD_TYPE=${{ matrix.config.config }} -G "Unix Makefiles" -DCMAKE_C_COMPILER=${{ matrix.config.compilerC }} -DCMAKE_CXX_COMPILER=${{ matrix.config.compilerCxx }}
           cmake --build . --parallel 2 --target ikarus
           cmake --build . --parallel 2 --target _ikarus
-          cmake --build . --parallel 2 --target build_tests
+          cmake --build . --parallel 2 --target build_${{ matrix.config.testRegex }}_tests
       - name: Tests
         working-directory: ./repo/cmake-build-${{ matrix.config.config }}
-        run: ctest --output-on-failure --parallel 2 -C ${{ matrix.config.config }}
+        run: ctest --output-on-failure --parallel 2 -L ${{ matrix.config.testRegex }}
```

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/ghpages.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/runExamples.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.github/workflows/style.yml` & `pyikarus-0.3.0.dev202310000062/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/.reuse/dep5` & `pyikarus-0.3.0.dev202310000062/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/CHANGELOG.md` & `pyikarus-0.3.0.dev202310000062/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: LGPL-3.0-or-later
 -->
 
 # Master (becomes Release v0.4)
-- Added greeting and init function for reasonable default, e.g. log also to file ([#147](https://github.com/ikarus-project/ikarus/pull/147))
 - Add CODE_OF_CONDUCT.md file
 - Refactored Cmake and directory structure  ([#146](https://github.com/ikarus-project/ikarus/pull/146))
 - Added comment section to blog post ([511d83](https://github.com/ikarus-project/ikarus/commit/511d83f9e7c474c9b320db5bc9367114ebe2825d))
 - Updated license information ([#138](https://github.com/ikarus-project/ikarus/pull/138))
 - Added detailed documentation for ikarus-examples ([#140](https://github.com/ikarus-project/ikarus/pull/140))
 - Added computation of Cauchy stress in linear elasticity ([#137](https://github.com/ikarus-project/ikarus/pull/137))
+- Added greeting and init function for reasonable default, e.g. log also to file ([#147](https://github.com/ikarus-project/ikarus/pull/147))
+- Added an interface for the material library ([#154](https://github.com/ikarus-project/ikarus/pull/154))
+- Added a wrapper for flat and blocked basis ([#157](https://github.com/ikarus-project/ikarus/pull/157))
 
 ## Release v0.3 (Prometheus)
 
 - Added codespell workflow (CI checks now for grammar and typos in comments and variable names) [#70](https://github.com/ikarus-project/ikarus/pull/70)
 - Added `EnhancedAssumedStrains` to decorate a linear-elastic element with various EAS methods [#74](https://github.com/ikarus-project/ikarus/pull/74)
 - Added the ability for the linear solver to accept matrix-valued rhs [#76](https://github.com/ikarus-project/ikarus/pull/76)
 - Added a path-following technique, such that a scalar subsidiary equation, for example, for `Arc length method`,  can be implemented independently [#80](https://github.com/ikarus-project/ikarus/pull/80)
```

### Comparing `pyikarus-0.3.0.dev202310000061/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 project(
         ikarus
   VERSION 0.3
   LANGUAGES C CXX
 )
 
 add_definitions(-DDUNE_LOCALFEFUNCTIONS_USE_EIGEN=1)
-add_definitions(-DDCMAKE_DISABLE_FIND_PACKAGE_Vc=1)
+add_definitions(-DCMAKE_DISABLE_FIND_PACKAGE_Vc=1)
 add_definitions(-DCMAKE_DISABLE_FIND_PACKAGE_LATEX=1)
 add_definitions(-DBUILD_SHARED_LIBS=1)
 
 # find dune packages to make cmake modules available
 find_package(dune-common REQUIRED EXCLUDE_FROM_ALL)
 list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake/modules" ${dune-common_MODULE_PATH})
 include(DuneMacros)
```

### Comparing `pyikarus-0.3.0.dev202310000061/CODE_OF_CONDUCT.md` & `pyikarus-0.3.0.dev202310000062/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/LICENSE.md` & `pyikarus-0.3.0.dev202310000062/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.0.dev202310000062/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.0.dev202310000062/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.0.dev202310000062/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.0.dev202310000062/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/PKG-INFO` & `pyikarus-0.3.0.dev202310000062/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000061
+Version: 0.3.0.dev202310000062
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000061 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000062 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000061/README.md` & `pyikarus-0.3.0.dev202310000062/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/CPM.cmake` & `pyikarus-0.3.0.dev202310000062/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.0.dev202310000062/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.0.dev202310000062/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.0.dev202310000062/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.0.dev202310000062/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/cmake/tools.cmake` & `pyikarus-0.3.0.dev202310000062/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/config.h.cmake` & `pyikarus-0.3.0.dev202310000062/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.0.dev202310000062/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/literature.bib` & `pyikarus-0.3.0.dev202310000062/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/mkdocs-macros.py` & `pyikarus-0.3.0.dev202310000062/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/mkdocs.yml` & `pyikarus-0.3.0.dev202310000062/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/overrides/partials/comments.html` & `pyikarus-0.3.0.dev202310000062/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/assembler.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/finiteElements.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ```cpp
 ScalarType evaluateScalar(const FErequirements& req);
 void evaluateVector(const FErequirements& req, VectorType& b);
 void evaluateMatrix(const FErequirements& req, MatrixType& A);
 void calculateLocalSystem(const FErequirements& req, MatrixType& A, VectorType& b);
 void calculateAt(const Resultrequirements& req, const Eigen::Vector<double, Traits::mydim>& local,
                      ResultTypeMap<ScalarType>& result);
-void globalIndices(std::vector<GlobalIndex>& globalIndices);
+void globalFlatIndices(std::vector<GlobalIndex>& indices);
 ```
 
 Please refer to the [FE requirements](feRequirements.md) to learn more about the finite element requirements and result requirements. 
 The first four methods receive an object of type `FErequirements`. This object is responsible for passing different types of information needed for the local evaluation of the local linear algebra objects.
 The first method, `evaluateScalar`, simply returns by value because it is cheaper to return a `double`, for example when evaluating energy.
 The other methods, `evaluateVector`, `evaluateMatrix`, and `calculateLocalSystem`, receive one or two additional output arguments where the results are to be written.
 This interface is needed to circumvent the dynamic memory allocation, that is required if these methods return by value.
@@ -58,15 +58,15 @@
 }
 ```
 !!! note "`ResultTypeMap<double>::ResultArray`"
     `#!cpp ResultTypeMap<double>::ResultArray` is an object of type `#!cpp Eigen::Matrix<double,Eigen::Dynamic,Eigen::Dynamic,0,3,3>`.
     Thus, the maximum size of `result` is limited to a 3x3 matrix. This is used to circumvent dynamic memory allocations again.
 
 
-The last method is the `globalIndices`. It is used to write a finite element's global indices to the output parameter `globalIndices`.
+The last method is the `globalFlatIndices`. It is used to write a finite element's global indices to the output parameter `indices`.
 This information originates from a `basis` object. See existing implementations for details.
 
 ## Linear and Non-linear Elasticity
 * To be added
 
 ## Enhanced Assumed Strain Elements
 The Enhanced Assumed Strain (EAS) elements are a class of finite elements that helps to avoid the locking phenomenon.
@@ -168,8 +168,8 @@
       }
     }
   }
 ```
 
 If the number of EAS parameters is set to zero, the pure displacement formulation is then utilised for analysis.
 
-\bibliography
+\bibliography
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/grids.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/index.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/localFunctions.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Local functions
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/observer.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/01_framework/solvers.md` & `pyikarus-0.3.0.dev202310000062/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/cantileverBeam.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Cantilever beam with point load
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/computePi.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/computePi.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Compute the value of $\pi$
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/cooksMembrane.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Cook's membrane
 
@@ -47,28 +44,28 @@
 ```cpp
 Eigen::Vector<int, 4> easSet;
 easSet << 0, 4, 5, 7;
 ```
 The EAS elements are created then, as shown below:
 ```cpp
 auto numberOfEASParameters = easSet(nep); // (1)!
-std::vector<Ikarus::EnhancedAssumedStrains<Ikarus::LinearElastic<typename decltype(basis)::element_type>>> fes;
+std::vector<Ikarus::EnhancedAssumedStrains<Ikarus::LinearElastic<decltype(basis)>>> fes;
 for (auto &element : elements(gridView)) {
-  fes.emplace_back(*basis, element, E, nu, &volumeLoad, &neumannBoundary, &neumannBoundaryLoad);
+  fes.emplace_back(basis, element, E, nu, &volumeLoad, &neumannBoundary, &neumannBoundaryLoad);
   fes.back().setEASType(numberOfEASParameters);
 }
 ```
 
 1. `nep` is the index of the `for`-loop which runs from 0 to 4 here.
 
 The Dirichlet boundary conditions are defined for the left edge, and the Neumann boundary condition on the right edge is defined by the usage of the dune-python interface.
 A sparse assembler is used, and the linear system of equations is solved. The vertical displacement in the top right corner is computed as shown below and is later stored in a vector: 
 ```cpp
 auto dispGlobalFunc = Dune::Functions::makeDiscreteGlobalBasisFunction<Dune::FieldVector<double, 2>>(*basis, D_Glob);
-auto localView      = basis->localView();
+auto localView      = basis.flat().localView();
 auto localw         = localFunction(dispGlobalFunc);
 double uy_fe        = 0.0;
 Eigen::Vector2d req_pos;
 req_pos << 48.0, 60.0;
 for (auto &ele : elements(gridView)) {
   localView.bind(ele);
   localw.bind(ele);
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Deformation of an incompressible rubber block
 
@@ -15,19 +12,19 @@
 for such a system is defined in the `Solid struct` by the function
 `calculateScalarImpl(const FERequirementType &par, const Eigen::VectorX<ScalarType> &dx)`. 
 This function uses the principles of automatic differentiation to provide the stiffness matrix and
 other necessary quantities to perform a static structural analysis.
 
 ## Code highlights
 
-The `struct` named `Solid` is created as an object of `AutoDiffFE`. It is constructed as shown below:
+The `struct` named `Solid` is created such that it inherits from `AutoDiffFE`. It is constructed as shown below:
 ```cpp
 Solid(const Basis &basis, const typename LocalView::Element &element, double emod, double nu)
-    : BaseAD(basis, element), localView_{basis.localView()}, emod_{emod}, nu_{nu} {
-  localView_.bind(element);
+    : BaseAD(basis.flat(), element), emod_{emod}, nu_{nu} {
+  this->localView().bind(element);
   mu_       = emod_ / (2 * (1 + nu_));
   lambdaMat = convertLameConstants({.emodul = emod_, .nu = nu_}).toLamesFirstParameter();
 }
 ```
 It takes a reference to the basis function (`&basis`), the element (`&element`), and the material parameters, namely Young's modulus 
 (`emod`) and Poisson's ratio (`nu`), as arguments during construction. The function `convertLameConstants()` is a helper function
 to switch between the Lame parameters.
@@ -62,21 +59,22 @@
 std::array<int, 2> elementsPerDirection = {elex, eley};
 auto grid                               = std::make_shared<Grid>(bbox, elementsPerDirection);
 auto gridView                           = grid->leafGridView();
 ```
 A linear Lagrangian basis is opted for the displacements and a constant basis for the pressure degrees of freedom using the
 `composite` basis feature from Dune, as shown below:
 ```cpp
-auto basis = Ikarus::makeConstSharedBasis(
-gridView, composite(power<2>(lagrange<1>(), FlatInterleaved()), lagrange<0>(), FlatLexicographic()));
+auto basis = Ikarus::makeBasis(
+gridView, composite(power<2>(lagrange<1>()), lagrange<0>()));
 ```
 Here, `#!cpp power<2>` is used to approximate the displacement field in both $x$ and $y$ directions. 
 The displacement degrees of freedom at position $y=0$ are fixed using the following snippet:
 ```cpp
-Ikarus::DirichletValues dirichletValues(basis);
+auto basisP = std::make_shared<const decltype(basis)>(basis);
+Ikarus::DirichletValues dirichletValues(basisP->flat());
 dirichletValues.fixDOFs([](auto &basis_, auto &dirichletFlags) {
   Dune::Functions::forEachBoundaryDOF(subspaceBasis(basis_, _0),
                    [&](auto &&localIndex, auto &&localView, auto &&intersection) {
                        if (std::abs(intersection.geometry().center()[1]) < 1e-8)
                          dirichletFlags[localView.index(localIndex)] = true;
   });
 }); 
@@ -86,15 +84,15 @@
 degrees of freedom (obtained via `subspaceBasis(basis_, _0)`) are set to `true` and used by the assembler later.
 
 A `sparse` and a `dense` assembler are used to arrive at the stiffness matrix and the external load vector using the 
 finite element requirements as described [here](../01_framework/feRequirements.md#fe-requirements).  
 ```cpp
 auto sparseFlatAssembler = SparseFlatAssembler(fes, dirichletValues);
 auto denseFlatAssembler  = DenseFlatAssembler(fes, dirichletValues);
-  auto req = FErequirements().addAffordance(Ikarus::AffordanceCollections::elastoStatics);
+auto req = FErequirements().addAffordance(Ikarus::AffordanceCollections::elastoStatics);
 
 auto fextFunction = [&](auto &&lambdaLocal, auto &&dLocal) -> auto & {
   req.insertGlobalSolution(Ikarus::FESolutions::displacement, dLocal)
       .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
   return denseFlatAssembler.getReducedVector(req);
 };
 auto KFunction = [&](auto &&lambdaLocal, auto &&dLocal) -> auto & {
@@ -106,16 +104,16 @@
 The `SparseLU` package from the Eigen library is used to solve the linear system of equations. 
 
 For post-processing, the function `Dune::Functions::makeDiscreteGlobalBasisFunction()` is used to create a function for 
 the displacements and pressure using the basis functions and the nodal values. `Dune::VTKWriter` is used to write 
 the `*.vtu` files. The results can then be plotted, for example, using [Paraview](https://www.paraview.org/).
 ```cpp
 auto disp
-    = Dune::Functions::makeDiscreteGlobalBasisFunction<Dune::FieldVector<double, 2>>(subspaceBasis(*basis, _0), d);
-auto pressure = Dune::Functions::makeDiscreteGlobalBasisFunction<double>(subspaceBasis(*basis, _1), d);
+    = Dune::Functions::makeDiscreteGlobalBasisFunction<Dune::FieldVector<double, 2>>(subspaceBasis(basis.flat(), _0), d);
+auto pressure = Dune::Functions::makeDiscreteGlobalBasisFunction<double>(subspaceBasis(basis.flat(), _1), d);
 Dune::VTKWriter vtkWriter(gridView, Dune::VTK::nonconforming);
 vtkWriter.addVertexData(disp, Dune::VTK::FieldInfo("displacement", Dune::VTK::FieldInfo::Type::vector, 2));
 vtkWriter.addVertexData(pressure, Dune::VTK::FieldInfo("pressure", Dune::VTK::FieldInfo::Type::scalar, 1));
 vtkWriter.write("iks003_incompressibleLinearElasticity");
 ```
 
 ## Takeaways
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/index.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/kirchhoffPlate.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Plate subjected to a surface load
 
@@ -13,27 +10,26 @@
 Kirchhoff-type plate element is implemented in `iks004_kirchhoffPlate.cpp` using the automatic differentiation
 technique as commented before. The basis used for discretization is a NURBS basis from the `dune-iga` module.
 The problem is solved, and convergence plots are created by comparing the solutions to the available analytical solutions for the
 simply supported case.
 
 ## Code highlights
 
-Similar to the `struct` named `Solid` in `iks003_incompressible_LinearElasticity.cpp`, here a `struct` named `KirchhoffPlate` is created as an object 
-of `AutoDiffFE`. It is constructed as shown below:
+Similar to the `struct` named `Solid` in `iks003_incompressible_LinearElasticity.cpp`, here a `struct` named `KirchhoffPlate` 
+is created such that it inherits from `AutoDiffFE`. It is constructed as shown below:
 ```cpp
 KirchhoffPlate(const Basis &basis, const typename LocalView::Element &element, double p_Emodul, double p_nu,
                double p_thickness)
-    : BaseDisp(basis, element),
-      BaseAD(basis, element),
-      localView_{basis.localView()},
+    : BaseDisp(basis.flat(), element),
+      BaseAD(basis.flat(), element),
       Emodul{p_Emodul},
       nu{p_nu},
       thickness{p_thickness} {
-  localView_.bind(element);
-  geometry_.emplace(localView_.element().geometry());
+  this->localView().bind(element);
+  geometry_.emplace(this->localView().element().geometry());
 }
 ```
 It takes in the `p_thickness` parameter in addition to the ones in `Solid`. Here, the energy is calculated as:
 ```cpp
 energy += (0.5 * kappa.dot(D * kappa) - w * lambda) * geometry_->integrationElement(gp.position()) * gp.weight();
 ```
 with `kappa` being the vector of curvature containing $\kappa_{xx}, \kappa_{yy}$ and $\kappa_{xy}$. If the boundaries 
@@ -83,15 +79,15 @@
 13. Elevating the polynomial degree for the `patchData` in $y$-direction (`1`) by 1.
 14. Creating the grid object from the patch data
 
 In order to obtain the convergence plots, the system is solved five times, with the refinement level 
 increasing by 1 each time using the command `#!cpp grid.globalRefine(1);`. The NURBS basis can be obtained directly from the 
 NURBS grid using the `getPreBasis()` function, as shown below:
 ```cpp
-auto basis = Ikarus::makeConstSharedBasis(gridView, gridView.impl().getPreBasis());
+auto basis = Ikarus::makeBasis(gridView, gridView.impl().getPreBasis());
 ```
 This is followed by specifying the Dirichlet boundary conditions, creating the finite elements and the assembler, 
 solving the system of equations, and post-processing using Paraview as mentioned in the previous examples.
 The analytical solution for the simply supported case is adapted from 
 [Wikipedia](https://en.wikipedia.org/wiki/Bending_of_plates#Simply-supported_plate_with_uniformly-distributed_load) and is also mentioned below: 
 ```cpp
 auto wAna = [&](auto x) {
@@ -109,15 +105,15 @@
 };
 ```
 The `#!cpp Dune::Functions::makeDiscreteGlobalBasisFunction` is used to create a function from the nodal finite element 
 solution of the displacements and the NURBS basis whereas the `#!cpp Dune::Functions::makeAnalyticGridViewFunction` is 
 used to create a function by using the function to evaluate the analytical solutions and the `gridView` to get the position `x`.
 Local functions are then created that are used later to calculate the $L^2$-error.  
 ```cpp
-auto wGlobalFunction = Dune::Functions::makeDiscreteGlobalBasisFunction<Dune::FieldVector<double, 1>>(*basis, w);
+auto wGlobalFunction = Dune::Functions::makeDiscreteGlobalBasisFunction<Dune::FieldVector<double, 1>>(basis.flat(), w);
 auto wGlobalAnalyticFunction = Dune::Functions::makeAnalyticGridViewFunction(wAna, gridView);
 auto localw                  = localFunction(wGlobalFunction);
 auto localwAna               = localFunction(wGlobalAnalyticFunction);
 ```
 The $L^2$-error is calculated by using 
 $$
 L^2\textrm{-error} = \sqrt{\sum_{ele} \int_{\Omega_{ele}} \left( w_{analytical}-w_{FE} \right)^2}
@@ -143,15 +139,15 @@
 l2_error = std::sqrt(l2_error);
 ```
 The number of degrees of freedom for each refinement level and its corresponding $L^2$-error is pushed to a vector that 
 can be later used to create plots using the features from Matlab.    
 ```cpp
 std::vector<double> dofsVec;
 std::vector<double> l2Evcector;
-dofsVec.push_back(basis->size());
+dofsVec.push_back(basis.flat().size());
 l2Evcector.push_back(l2_error);
 ```
 
 ## Takeaways
 
 - NURBS grids can be created using the `dune-iga` module.
 - The basis for the corresponding NURBS grid can be obtained using the `getPreBasis()` function.
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Newton-Raphson method
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/nonLinearElasticity.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Non-linear Elasticity for 2D solids
 
@@ -56,25 +53,26 @@
   fext[1] = lamb / 40;
   return fext;
 };
 
 auto matParameter = Ikarus::toLamesFirstParameterAndShearModulus({.emodul = 1000, .nu = 0.3});
 
 Ikarus::StVenantKirchhoff matSVK(matParameter);
-auto reducedMat = plainStress(matSVK);
+auto reducedMat = planeStress(matSVK);
 
 std::vector<Ikarus::NonLinearElastic<typename decltype(basis)::element_type, decltype(reducedMat)>>> fes;
 for (auto &element : elements(gridView))
   fes.emplace_back(*basis, element, reducedMat, &neumannBoundary, neumannBoundaryLoad, volumeLoad);
 ```
 The functors `volumeLoad` and `neumannBoundaryLoad` are used to obtain the external volume and surface loads acting on a particular position.
 We use a Saint Venant–Kirchhoff material model, which we transform to a plane stress material law for our two-dimensional simulation.
 The line $y=0$ is clamped by applying the Dirichlet boundary condition expressed below:
 ```cpp
-Ikarus::DirichletValues dirichletValues(basis);
+auto basisP = std::make_shared<const decltype(basis)>(basis);
+Ikarus::DirichletValues dirichletValues(basisP->flat());
 
 dirichletValues.fixBoundaryDOFs([&](auto &dirichletFlags, auto &&localIndex, auto &&localView, auto &&intersection) {
   if (std::abs(intersection.geometry().center()[1]) < 1e-8) dirichletFlags[localView.index(localIndex)] = true;
 });
 ```
 The finite element requirements are defined by using the affordance `#!cpp Ikarus::AffordanceCollections::elastoStatics`.
 This is then used to create functors to get the stiffness matrix, residual vector, and energy value using a sparse assembler.
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.0.dev202310000062/docs/website/02_examples/vonMisesTruss.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
----
-status: new
----
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Von Mises truss calculation  
 
@@ -12,19 +9,19 @@
 
 `iks007_vonMisesTruss.cpp` utilizes the tools and features mentioned in the previous examples to solve the 
 standard Von-Mises truss example found in literature (refer to Section 2[@misesTruss1923]).
 
 
 ## Code highlights
 
-The struct named `Truss` is created as an object in `AutoDiffFE`. It is constructed as shown below:
+The struct named `Truss` is created such that it inherits from `AutoDiffFE`. It is constructed as shown below:
 ```cpp
 Truss(const Basis &basis, const typename LocalView::Element &element, double p_EA)
-    : BaseDisp(basis, element), BaseAD(basis, element), localView_{basis.localView()}, EA{p_EA} {
-  localView_.bind(element);
+    : BaseDisp(basis.flat(), element), BaseAD(basis.flat(), element), EA{p_EA} {
+  this->localView().bind(element);
 }
 ```
 It takes a reference to the basis function (`&basis`), the element (`&element`), and the axial stiffness of the 
 truss structure (`p_EA`) as arguments during construction.
 
 `ScalarType calculateScalarImpl(const FERequirementType &par, const Eigen::VectorX<ScalarType> &dx)` is
 then defined, returning a scalar value, in this case the energy.
```

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.0.dev202310000062/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.0.dev202310000062/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.0.dev202310000062/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.0.dev202310000062/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/download.md` & `pyikarus-0.3.0.dev202310000062/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/docs/website/index.md` & `pyikarus-0.3.0.dev202310000062/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/assembler/simpleAssemblers.hh`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 #include <ranges>
 #include <utility>
 
 #include <dune/common/math.hh>
+#include <dune/functions/backends/istlvectorbackend.hh>
 
 #include <Eigen/Core>
 #include <Eigen/Dense>
 #include <Eigen/Sparse>
 
 #include <ikarus/linearAlgebra/dirichletValues.hh>
 #include <ikarus/utils/concepts.hh>
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.0.dev202310000062/ikarus/assembler/simpleAssemblers.inl`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     vec.setZero(this->size());
     Eigen::VectorXd vecLocal;
     std::vector<GlobalIndex> dofs;
     for (auto &fe : this->finiteElements()) {
       vecLocal.setZero(fe.size());
       dofs.resize(0);
       fe.calculateVector(fErequirements, vecLocal);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       for (int i = 0; auto id : dofs) {
         vec(id[0]) += vecLocal(i);
         ++i;
       }
     }
     for (auto i = 0U; i < this->size(); ++i) {
       if (this->isConstrained(i)) vec[i] = 0;
@@ -49,18 +49,18 @@
     int reducedCounter = 0;
     Eigen::VectorXd vecLocal;
     std::vector<GlobalIndex> dofs;
     for (auto &fe : this->finiteElements()) {
       vecLocal.setZero(fe.size());
       dofs.resize(0);
       fe.calculateVector(fErequirements, vecLocal);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       assert(static_cast<long int>(dofs.size()) == vecLocal.size() && "The returned vector has wrong rowSize!");
       for (int i = 0; auto &&dofIndex : dofs) {
-        if (this->isConstrained(dofIndex[0])) {
+        if (this->isConstrained(dofIndex)) {
           ++reducedCounter;
           ++i;
           continue;
         } else
           vecRed(dofIndex[0] - this->constraintsBelow(dofIndex[0])) += vecLocal[i++];
       }
     }
@@ -102,15 +102,15 @@
     spMatReduced.coeffs().setZero();
     Eigen::MatrixXd A;
     std::vector<GlobalIndex> dofs;
     for (size_t elementIndex = 0; const auto &fe : this->finiteElements()) {
       A.setZero(fe.size(), fe.size());
       dofs.resize(0);
       fe.calculateMatrix(fErequirements, A);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       assert(dofs.size() == static_cast<unsigned>(A.rows()) && "The returned matrix has wrong rowSize!");
       assert(dofs.size() == static_cast<unsigned>(A.cols()) && "The returned matrix has wrong colSize!");
       Eigen::Index linearIndex = 0;
       for (auto r = 0U; r < dofs.size(); ++r) {
         if (this->isConstrained(dofs[r][0]))
           continue;
         else {
@@ -130,15 +130,15 @@
     spMat.resize(this->size(), this->size());
     std::vector<Eigen::Triplet<double>> vectorOfTriples;
 
     vectorOfTriples.reserve(this->estimateOfConnectivity());
     std::vector<GlobalIndex> dofs;
     for (auto &&fe : this->finiteElements()) {
       dofs.resize(0);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       for (auto idi : dofs)
         for (auto idj : dofs)
           vectorOfTriples.emplace_back(idi[0], idj[0], 0.0);
     }
 
     spMat.setFromTriplets(vectorOfTriples.begin(), vectorOfTriples.end());
     isOccupationPatternCreated = true;
@@ -150,15 +150,15 @@
     std::vector<Eigen::Triplet<double>> vectorOfTriples;
     using std::size;
 
     vectorOfTriples.reserve(this->estimateOfConnectivity());
     std::vector<GlobalIndex> dofs;
     for (auto &fe : this->finiteElements()) {
       dofs.resize(0);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       for (auto r = 0U; r < dofs.size(); ++r) {
         if (this->isConstrained(dofs[r][0]))
           continue;
         else {
           for (auto c = 0U; c < dofs.size(); ++c) {
             if (this->isConstrained(dofs[c][0])) continue;
             vectorOfTriples.emplace_back(dofs[r][0] - this->constraintsBelow(dofs[r][0]),
@@ -173,29 +173,29 @@
   }
 
   template <typename Basis, typename FEContainer>
   void SparseFlatAssembler<Basis, FEContainer>::createlinearDofsPerElement() {
     std::vector<GlobalIndex> dofs;
     for (auto &&fe : this->finiteElements()) {
       dofs.resize(0);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       elementLinearIndices.emplace_back(Dune::power(dofs.size(),2));
       for (Eigen::Index linearIndexOfElement = 0; auto &&c : dofs)
         for (auto &&r : dofs)
           elementLinearIndices.back()[linearIndexOfElement++] = spMat.getLinearIndex(r[0], c[0]);
     }
     arelinearDofsPerElementCreated = true;
   }
 
   template <typename Basis, typename FEContainer>
   void SparseFlatAssembler<Basis, FEContainer>::createlinearDofsPerElementReduced() {
     std::vector<GlobalIndex> dofs;
     for (auto &&fe : this->finiteElements()) {
       dofs.resize(0);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       elementLinearReducedIndices.emplace_back();
       for (auto r = 0U; r < dofs.size(); ++r) {
         if (this->isConstrained(dofs[r][0])) continue;
         for (auto c = 0U; c < dofs.size(); ++c) {
           if (this->isConstrained(dofs[c][0])) continue;
           elementLinearReducedIndices.back().push_back(spMatReduced.getLinearIndex(
               dofs[r][0] - this->constraintsBelow(dofs[r][0]), dofs[c][0] - this->constraintsBelow(dofs[c][0])));
@@ -210,15 +210,15 @@
     matRed.setZero(this->reducedSize(), this->reducedSize());
     Eigen::MatrixXd matLocal;
     std::vector<GlobalIndex> dofs;
     for (auto &fe : this->finiteElements()) {
       matLocal.setZero(fe.size(), fe.size());
       dofs.resize(0);
       fe.calculateMatrix(fErequirements, matLocal);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       assert(dofs.size() == static_cast<unsigned>(matLocal.rows()) && "The returned matrix has wrong rowSize!");
       assert(dofs.size() == static_cast<unsigned>(matLocal.cols()) && "The returned matrix has wrong colSize!");
       for (auto r = 0U; r < dofs.size(); ++r) {
         if (this->isConstrained(dofs[r][0])) {
           continue;
         } else {
           for (auto c = 0U; c < dofs.size(); ++c) {
@@ -239,15 +239,15 @@
     mat.setZero(this->size(), this->size());
     Eigen::MatrixXd matLocal;
     std::vector<GlobalIndex> dofs;
     for (auto &fe : this->finiteElements()) {
       matLocal.setZero(fe.size(), fe.size());
       dofs.resize(0);
       fe.calculateMatrix(fErequirements, matLocal);
-      fe.globalIndices(dofs);
+      fe.globalFlatIndices(dofs);
       for (auto i = 0; auto idi : dofs) {
         for (auto j = 0; auto idj : dofs) {
           mat(idi[0], idj[0]) += matLocal(i, j);
           ++j;
         }
         ++i;
       }
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files 16% similar despite different names*

```diff
@@ -14,60 +14,64 @@
   ////This element can not be used on its own but it should be inherited from
   //// The class constructor can only be called from the templated class.
   template <typename RealElement, typename Basis, typename FERequirementType_ = FErequirements<>, bool useEigenRef = false >
   class AutoDiffFE {
   public:
     using LocalView = typename Basis::LocalView;
     using Traits    = TraitsFromLocalView<LocalView,useEigenRef>;
+    using GridElement = typename LocalView::Element;
 
     using FERequirementType = FERequirementType_;
     void calculateMatrix(const FERequirementType& par, typename Traits::MatrixType h) const {
-      Eigen::VectorXdual2nd dx(localdofSize);
+      Eigen::VectorXdual2nd dx(localDofSize);
       Eigen::VectorXd g;
       autodiff::dual2nd e;
       dx.setZero();
       auto f = [&](auto& x) { return this->underlying().calculateScalarImpl(par, x); };
       hessian(f, autodiff::wrt(dx), at(dx), e, g, h);
     }
 
     void calculateVector(const FERequirementType& par, typename Traits::VectorType g) const {
-      Eigen::VectorXdual dx(localdofSize);
+      Eigen::VectorXdual dx(localDofSize);
       dx.setZero();
       autodiff::dual e;
       auto f = [&](auto& x) { return this->underlying().calculateScalarImpl(par, x); };
       gradient(f, autodiff::wrt(dx), at(dx), e, g);
     }
 
     void calculateLocalSystem(const FERequirementType& par, typename Traits::MatrixType h,
                               typename Traits::VectorType g) const {
-      Eigen::VectorXdual2nd dx(localdofSize);
+      Eigen::VectorXdual2nd dx(localDofSize);
       dx.setZero();
       auto f = [&](auto& x) { return this->underlying().calculateScalarImpl(par, x); };
       hessian(f, autodiff::wrt(dx), at(dx), g, h);
     }
 
     [[nodiscard]] typename Traits::ScalarType calculateScalar(const FERequirementType& par) const {
-      Eigen::VectorXd dx(localdofSize);
+      Eigen::VectorXd dx(localDofSize);
       dx.setZero();
 
       return this->underlying().calculateScalarImpl(par, dx);
     }
 
-    size_t size() const { return localdofSize; }
+    [[nodiscard]] size_t size() const { return localDofSize; }
+    const GridElement& getEntity() { return localView_.element(); }
+    const LocalView& localView() const { return localView_; }
+    LocalView& localView() { return localView_; }
 
   protected:
-    explicit AutoDiffFE(const Basis& basis, const typename LocalView::Element& element) {
-      auto localView = basis.localView();
-      localView.bind(element);
-      localdofSize = localView.size();
+    explicit AutoDiffFE(const Basis& basis, const typename LocalView::Element& element)
+        : localView_{basis.localView()} {
+      localView_.bind(element);
+      localDofSize = localView_.size();
     }
 
   private:
     RealElement const& underlying() const  // CRTP
     {
       return static_cast<RealElement const&>(*this);
     }
-
-    int localdofSize{};
+    LocalView localView_;
+    int localDofSize{};
   };
 
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files 8% similar despite different names*

```diff
@@ -14,43 +14,46 @@
   template <typename Basis>
   class PowerBasisFE {
   public:
     using RootBasis   = Basis;
     using LocalView   = typename Basis::LocalView;
     using GlobalIndex = typename LocalView::MultiIndex;
     explicit PowerBasisFE(const Basis& p_basis, const typename LocalView::Element& element)
-        : localView{p_basis.localView()} {
+        : localView_{p_basis.localView()} {
       static_assert(Ikarus::Concepts::PowerBasis<RootBasis>,
                     "You didn't pass a localview of a power basis to this method");
       static_assert(RootBasis::PreBasis::Node::degree() != 1,
                     "The basis has only one children. Maybe use scalarFE.hh. ");
 
-      localView.bind(element);
+      localView_.bind(element);
     }
 
     /** \brief Type of the Pairs of gridEntities and variable tags */
     using GridElementEntityType = typename LocalView::Element;
     using Traits                = FETraits<GridElementEntityType>;
 
     /** \brief Number of children in the powerBasis */
     static constexpr int num_children = RootBasis::PreBasis::Node::CHILDREN;
 
-    [[nodiscard]] constexpr int size() const { return localView.size(); }
+    [[nodiscard]] constexpr int size() const { return localView_.size(); }
 
-    void globalIndices(std::vector<GlobalIndex>& globalIndices) const {
+    void globalFlatIndices(std::vector<GlobalIndex>& globalIndices) const {
+      globalIndices.clear();
       static_assert(
-          requires { localView.tree().child(0); },
+          requires { localView_.tree().child(0); },
           "Your basis does not provide a child accessor. Maybe use scalarFE.hh.");
-      const auto& fe = localView.tree().child(0).finiteElement();
+      const auto& fe = localView_.tree().child(0).finiteElement();
       for (size_t i = 0; i < fe.size(); ++i) {
         for (int j = 0; j < num_children; ++j) {
-          globalIndices.push_back(localView.index((localView.tree().child(j).localIndex(i))));
+          globalIndices.push_back(localView_.index((localView_.tree().child(j).localIndex(i))));
         }
       }
     }
 
-    const GridElementEntityType& getEntity() { return localView.element(); }
+    const GridElementEntityType& getEntity() { return localView_.element(); }
+    const LocalView& localView() const { return localView_; }
+    LocalView& localView() { return localView_; }
 
   private:
-    LocalView localView;
+    LocalView localView_;
   };
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,35 @@
   template <typename Basis>
   class ScalarFieldFE {
   public:
     using RootBasis   = Basis;
     using LocalView   = typename Basis::LocalView;
     using GlobalIndex = typename LocalView::MultiIndex;
     explicit ScalarFieldFE(const Basis& basis, const typename LocalView::Element& element)
-        : localView{basis.localView()} {
+        : localView_{basis.localView()} {
       static_assert(RootBasis::PreBasis::Node::CHILDREN == 0, "This is no scalar basis!");
-      localView.bind(element);
+      localView_.bind(element);
     }
 
     /** \brief Type of the Pairs of gridEntities and variable tags */
     using GridElementEntityType = typename LocalView::Element;
     using Traits                = FETraits<GridElementEntityType>;
 
     /** \brief Dimension of the world space */
     static constexpr int worlddim = Traits::worlddim;
 
-    [[nodiscard]] int size() const { return localView.size(); }
+    [[nodiscard]] int size() const { return localView_.size(); }
 
-    void globalIndices(std::vector<GlobalIndex>& globalIndices) const {
-      const auto& fe = localView.tree().finiteElement();
+    void globalFlatIndices(std::vector<GlobalIndex>& globalIndices) const {
+      const auto& fe = localView_.tree().finiteElement();
       for (size_t i = 0; i < fe.size(); ++i)
-        globalIndices.push_back(localView.index(localView.tree().localIndex(i)));
+        globalIndices.push_back(localView_.index(localView_.tree().localIndex(i)));
     }
 
-    const GridElementEntityType& getEntity() { return localView.element(); }
+    const GridElementEntityType& getEntity() { return localView_.element(); }
+    const LocalView& localView() const { return localView_; }
+    LocalView& localView() { return localView_; }
 
   private:
-    LocalView localView;
+    LocalView localView_;
   };
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feRequirements.cpp` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feRequirements.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files 3% similar despite different names*

```diff
@@ -255,25 +255,17 @@
     using FERequirementType      = typename DisplacementBasedElement::FERequirementType;
     using ResultRequirementsType = typename DisplacementBasedElement::ResultRequirementsType;
     using LocalView              = typename DisplacementBasedElement::LocalView;
     using GridView               = typename DisplacementBasedElement::GridView;
     using Traits                 = typename DisplacementBasedElement::Traits;
     using DisplacementBasedElement::localView;
 
-    template <typename Basis, typename VolumeLoad = std::nullptr_t, typename NeumannBoundaryLoad = std::nullptr_t>
-    requires(Std::is_pointer<VolumeLoad>and Std::is_pointer<NeumannBoundaryLoad>)
-        EnhancedAssumedStrains(Basis& globalBasis, const typename LocalView::Element& element, double emod, double nu,
-                               VolumeLoad p_volumeLoad                          = nullptr,
-                               const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
-                               NeumannBoundaryLoad p_neumannBoundaryLoad        = nullptr)
-        : DisplacementBasedElement(globalBasis, element, emod, nu, p_volumeLoad, p_neumannBoundary,
-                                   p_neumannBoundaryLoad) {
-      if (Traits::mydim == 2)
-        setEASType(0);
-      else if (Traits::mydim == 3)
+    template <typename ...Args>
+        explicit EnhancedAssumedStrains(Args&& ...args)
+        : DisplacementBasedElement(std::forward<Args>(args)...) {
         setEASType(0);
     }
 
     double calculateScalar(const FERequirementType& par) const {
       if (onlyDisplacementBase) return DisplacementBasedElement::calculateScalar(par);
       DUNE_THROW(Dune::NotImplemented,
                  "EAS element do not support any scalar calculations, i.e. they are not derivable from a potential");
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files 12% similar despite different names*

```diff
@@ -27,70 +27,68 @@
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
 #include <ikarus/utils/defaultFunctions.hh>
 
 namespace Ikarus {
 
 
-  template <typename Basis, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
-  class LinearElastic : public PowerBasisFE<Basis> {
+  template <typename Basis_, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
+  class LinearElastic : public PowerBasisFE<typename Basis_::FlatBasis> {
   public:
-    using BaseDisp               = PowerBasisFE<Basis>;  // Handles globalIndices function
-    using GlobalIndex            = typename PowerBasisFE<Basis>::GlobalIndex;
+    using Basis = Basis_;
+    using FlatBasis = typename Basis::FlatBasis;
+    using BaseDisp               = PowerBasisFE<FlatBasis>;  // Handles globalIndices function
     using FERequirementType      = FErequirements_;
     using ResultRequirementsType = ResultRequirements<FERequirementType>;
-    using LocalView              = typename Basis::LocalView;
+    using LocalView              = typename FlatBasis::LocalView;
     using Element                = typename LocalView::Element;
-    using GridView               = typename Basis::GridView;
-    using GlobalBasis            = Basis;
+    using GridView               = typename FlatBasis::GridView;
 
     using Traits = TraitsFromLocalView<LocalView, useEigenRef>;
 
     static constexpr int mydim = Traits::mydim;
 
     template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
         LinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, double emod, double nu,
-                      VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* neumannBoundary = nullptr,
+                      VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
                       NeumannBoundaryLoad p_neumannBoundaryLoad = {})
-        : BaseDisp(globalBasis, element),
-          localView_{globalBasis.localView()},
-          neumannBoundary_{neumannBoundary},
+        : BaseDisp(globalBasis.flat(), element),
+          neumannBoundary{p_neumannBoundary},
           emod_{emod},
           nu_{nu} {
-            val=7;
-      localView_.bind(element);
-      auto& first_child = localView_.tree().child(0);
+      this->localView().bind(element);
+      auto& first_child = this->localView().tree().child(0);
       const auto& fe    = first_child.finiteElement();
       numberOfNodes     = fe.size();
       dispAtNodes.resize(fe.size());
-      const int order = 2 * (localView_.tree().child(0).finiteElement().localBasis().order());
-      localBasis      = Dune::CachedLocalBasis(localView_.tree().child(0).finiteElement().localBasis());
-      localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(localView_.element().type(), order),
+      const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
+      localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
+      localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(this->localView().element().type(), order),
                       Dune::bindDerivatives(0, 1));
 
       if constexpr (!std::is_same_v<VolumeLoad,LoadDefault>)
         volumeLoad =p_volumeLoad;
       if constexpr (!std::is_same_v<NeumannBoundaryLoad,LoadDefault>)
         neumannBoundaryLoad =p_neumannBoundaryLoad;
 
-      assert(((not neumannBoundary_ and not neumannBoundaryLoad) or (neumannBoundary_ and neumannBoundaryLoad))
+      assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
              && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
 
   public:
-    const auto& localView() const { return localView_; }
+    //    const auto& localView() const { return localView(); }
 
     auto getDisplacementFunction(const FERequirementType& par) const {
       const auto& d = par.getGlobalSolution(Ikarus::FESolutions::displacement);
 
       for (auto i = 0U; i < dispAtNodes.size(); ++i)
         for (auto k2 = 0U; k2 < mydim; ++k2)
-          dispAtNodes[i][k2] = d[localView_.index(localView_.tree().child(k2).localIndex(i))[0]];
+          dispAtNodes[i][k2] = d[this->localView().index(this->localView().tree().child(k2).localIndex(i))[0]];
       auto geo = std::make_shared<const typename GridView::GridView::template Codim<0>::Entity::Geometry>(
-          localView_.element().geometry());
+          this->localView().element().geometry());
       Dune::StandardLocalFunction uFunction(localBasis, dispAtNodes, geo);
 
       return uFunction;
     }
 
     auto getStrainFunction(const FERequirementType& par) const { return linearStrains(getDisplacementFunction(par)); }
 
@@ -109,72 +107,65 @@
       const auto u       = getDisplacementFunction(par);
       const auto eps     = getStrainFunction(par);
       const auto& lambda = par.getParameter(Ikarus::FEParameter::loadfactor);
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
       const auto C = getMaterialTangent();
 
-      const auto geo = localView_.element().geometry();
+      const auto geo = this->localView().element().geometry();
       double energy  = 0.0;
       for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
         const auto EVoigt = eps.evaluate(gpIndex, on(gridElement));
 
         energy += (0.5 * EVoigt.dot(C * EVoigt)) * geo.integrationElement(gp.position()) * gp.weight();
       }
       // External forces volume forces over the domain
       if (volumeLoad) {
         for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
           const auto uVal                              = u.evaluate(gpIndex);
-          Eigen::Vector<double, Traits::worlddim> fext = (*volumeLoad)(toEigen(gp.position()), lambda);
+          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(gp.position()), lambda);
           energy -= uVal.dot(fext) * geo.integrationElement(gp.position()) * gp.weight();
         }
       }
 
       // line or surface loads, i.e. neumann boundary
-      if (not neumannBoundary_ and not neumannBoundaryLoad) return energy;
+      if (not neumannBoundary) return energy;
 
-      auto element = localView_.element();
-      for (auto&& intersection : intersections(neumannBoundary_->gridView(), element)) {
-        if (not neumannBoundary_->contains(intersection)) continue;
+      auto element = this->localView().element();
+      for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
+        if (not neumannBoundary->contains(intersection)) continue;
 
         const auto& quadLine = Dune::QuadratureRules<double, mydim - 1>::rule(intersection.type(), u.order());
 
         for (const auto& curQuad : quadLine) {
           // Local position of the quadrature point
           const Dune::FieldVector<double, mydim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function
           const auto uVal = u.evaluate(quadPos);
 
           // Value of the Neumann data at the current position
           auto neumannValue
-              = (*neumannBoundaryLoad)(toEigen(intersection.geometry().global(curQuad.position())), lambda);
+              = neumannBoundaryLoad(toEigen(intersection.geometry().global(curQuad.position())), lambda);
 
           energy -= neumannValue.dot(uVal) * curQuad.weight() * integrationElement;
         }
       }
       return energy;
     }
 
-    double fac(int i) const
-    {
-      return i*val;
-    }
-
-    double val;
-
     void calculateMatrix(const FERequirementType& par, typename Traits::MatrixType K) const {
       const auto eps = getStrainFunction(par);
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
       const auto C   = getMaterialTangent();
-      const auto geo = localView_.element().geometry();
+      const auto geo = this->localView().element().geometry();
 
       for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
         const double intElement = geo.integrationElement(gp.position()) * gp.weight();
         for (size_t i = 0; i < numberOfNodes; ++i) {
           const auto bopI = eps.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
           for (size_t j = 0; j < numberOfNodes; ++j) {
             const auto bopJ = eps.evaluateDerivative(gpIndex, wrt(coeff(j)), on(gridElement));
@@ -208,15 +199,15 @@
     void calculateVector(const FERequirementType& par, typename Traits::VectorType force) const {
       const auto& lambda = par.getParameter(Ikarus::FEParameter::loadfactor);
       const auto eps     = getStrainFunction(par);
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
       const auto C   = getMaterialTangent();
-      const auto geo = localView_.element().geometry();
+      const auto geo = this->localView().element().geometry();
 
       // Internal forces
       for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
         const double intElement = geo.integrationElement(gp.position()) * gp.weight();
         auto stresses           = (C * eps.evaluate(gpIndex, on(gridElement))).eval();
         for (size_t i = 0; i < numberOfNodes; ++i) {
           const auto bopI = eps.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
@@ -224,30 +215,30 @@
         }
       }
 
       // External forces volume forces over the domain
       if (volumeLoad) {
         const auto u = getDisplacementFunction(par);
         for (const auto& [gpIndex, gp] : u.viewOverIntegrationPoints()) {
-          Eigen::Vector<double, Traits::worlddim> fext = (*volumeLoad)(toEigen(gp.position()), lambda);
+          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(gp.position()), lambda);
           for (size_t i = 0; i < numberOfNodes; ++i) {
             const auto udCi = u.evaluateDerivative(gpIndex, wrt(coeff(i)));
             force.template segment<mydim>(mydim * i)
                 -= udCi * fext * geo.integrationElement(gp.position()) * gp.weight();
           }
         }
       }
 
       // External forces, boundary forces, i.e. at the Neumann boundary
-      if (not neumannBoundary_ and not neumannBoundaryLoad) return;
+      if (not neumannBoundary) return;
 
       const auto u = getDisplacementFunction(par);
-      auto element = localView_.element();
-      for (auto&& intersection : intersections(neumannBoundary_->gridView(), element)) {
-        if (not neumannBoundary_->contains(intersection)) continue;
+      auto element = this->localView().element();
+      for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
+        if (not neumannBoundary->contains(intersection)) continue;
 
         // Integration rule along the boundary
         const auto& quadLine = Dune::QuadratureRules<double, mydim - 1>::rule(intersection.type(), u.order());
 
         for (const auto& curQuad : quadLine) {
           const Dune::FieldVector<double, mydim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
@@ -255,32 +246,31 @@
 
           // The value of the local function wrt the i-th coef
           for (size_t i = 0; i < numberOfNodes; ++i) {
             const auto udCi = u.evaluateDerivative(quadPos, wrt(coeff(i)));
 
             // Value of the Neumann data at the current position
             auto neumannValue
-                = (*neumannBoundaryLoad)(toEigen(intersection.geometry().global(curQuad.position())), lambda);
+                = neumannBoundaryLoad(toEigen(intersection.geometry().global(curQuad.position())), lambda);
             force.template segment<mydim>(mydim * i) -= udCi * neumannValue * curQuad.weight() * integrationElement;
           }
         }
       }
     }
 
-    LocalView localView_;
     Dune::CachedLocalBasis<
         std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
         localBasis;
-    std::optional<std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
-                                                                        const double&)>>
+    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
+                                                          const double&)>
         volumeLoad;
-    std::optional<std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
-                                                                        const double&)>>
+    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
+                                                          const double&)>
         neumannBoundaryLoad;
-    const BoundaryPatch<GridView>* neumannBoundary_;
+    const BoundaryPatch<GridView>* neumannBoundary;
     mutable Dune::BlockVector<Dune::RealTuple<double, Traits::dimension>> dispAtNodes;
     double emod_;
     double nu_;
     size_t numberOfNodes{0};
   };
 
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/materials.hh`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #include <ikarus/finiteElements/mechanics/materials/neohooke.hh>
 #include <ikarus/finiteElements/mechanics/materials/svk.hh>
 #include <ikarus/finiteElements/mechanics/materials/tags.hh>
 #include <ikarus/finiteElements/mechanics/materials/vanishingStress.hh>
 
 namespace Ikarus {
   template <typename MaterialImpl>
-  auto plainStress(const MaterialImpl& mat, typename MaterialImpl::ScalarType p_tol = 1e-8) {
+  auto planeStress(const MaterialImpl& mat, typename MaterialImpl::ScalarType p_tol = 1e-8) {
     return makeVanishingStress<{2, 1}, {2, 0}, {2, 2}>(mat, p_tol);
   }
 
   template <typename MaterialImpl>
   auto shellMaterial(const MaterialImpl& mat, typename MaterialImpl::ScalarType p_tol = 1e-8) {
     return makeVanishingStress<{2, 2}>(mat, p_tol);
   }
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files 12% similar despite different names*

```diff
@@ -20,137 +20,139 @@
 #include <ikarus/finiteElements/feBases/powerBasisFE.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/finiteElements/feTraits.hh>
 #include <ikarus/finiteElements/mechanics/materials.hh>
 #include <ikarus/finiteElements/physicsHelper.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
-#include <ikarus/utils/defaultFunctions.hh>
 
 namespace Ikarus {
 
-  template <typename Basis, typename Material_, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
-  class NonLinearElastic : public PowerBasisFE<Basis>,
-                                public Ikarus::AutoDiffFE<NonLinearElastic<Basis, Material_,FErequirements_,useEigenRef>, Basis,FErequirements_,useEigenRef> {
+  template <typename Basis_, typename Material_, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
+  class NonLinearElastic
+      : public PowerBasisFE<typename Basis_::FlatBasis>,
+        public Ikarus::AutoDiffFE<NonLinearElastic<Basis_, Material_,FErequirements_,useEigenRef>, typename Basis_::FlatBasis,FErequirements_,useEigenRef> {
   public:
-    using BaseDisp = PowerBasisFE<Basis>;  // Handles globalIndices function
-    using BaseAD   = Ikarus::AutoDiffFE<NonLinearElastic<Basis, Material_,FErequirements_,useEigenRef>, Basis,FErequirements_,useEigenRef>;
+    using Basis = Basis_;
+    using FlatBasis = typename Basis::FlatBasis;
+    using BaseDisp  = PowerBasisFE<FlatBasis>;  // Handles globalIndices function
+    using BaseAD    = Ikarus::AutoDiffFE<NonLinearElastic<Basis_, Material_,FErequirements_,useEigenRef>, typename Basis_::FlatBasis,FErequirements_,useEigenRef>;
+    using FERequirementType      = FErequirements_;
+
+    using ResultRequirementsType = ResultRequirements<FERequirementType>;
+
+    using BaseAD::localView;
     using BaseAD::size;
-    using GlobalIndex = typename PowerBasisFE<Basis>::GlobalIndex;
     friend BaseAD;
-    using FERequirementType = FErequirements_;
-    using LocalView         = typename Basis::LocalView;
-    using Element                = typename LocalView::Element;
+    using LocalView         = typename FlatBasis::LocalView;
+    using Element        = typename LocalView::Element;
     using Geometry          = typename Element::Geometry;
-    using GridView          = typename Basis::GridView;
+    using GridView          = typename FlatBasis::GridView;
     using Material          = Material_;
-    using GlobalBasis = Basis;
 
     template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
     NonLinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, const Material& p_mat,
-                     VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* neumannBoundary = nullptr,
+                     VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
                      NeumannBoundaryLoad p_neumannBoundaryLoad = {})
-        : BaseDisp(globalBasis, element),
-          BaseAD(globalBasis, element),
-          localView_{globalBasis.localView()},
-          neumannBoundary_{neumannBoundary},
+        : BaseDisp(globalBasis.flat(), element),
+          BaseAD(globalBasis.flat(), element),
+          neumannBoundary{p_neumannBoundary},
           mat{p_mat} {
-      localView_.bind(element);
-      const int order = 2 * (localView_.tree().child(0).finiteElement().localBasis().order());
-      localBasis      = Dune::CachedLocalBasis(localView_.tree().child(0).finiteElement().localBasis());
-      localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(localView_.element().type(), order),
+      this->localView().bind(element);
+      const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
+      localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
+      localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(this->localView().element().type(), order),
                       Dune::bindDerivatives(0, 1));
 
       if constexpr (!std::is_same_v<VolumeLoad,LoadDefault>)
         volumeLoad =p_volumeLoad;
       if constexpr (!std::is_same_v<NeumannBoundaryLoad,LoadDefault>)
         neumannBoundaryLoad =p_neumannBoundaryLoad;
 
-      assert(((not neumannBoundary_ and not neumannBoundaryLoad) or (neumannBoundary_ and neumannBoundaryLoad))
-             && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
+      assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
+                 && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
 
     using Traits = TraitsFromLocalView<LocalView,useEigenRef>;
-    const auto& localView() const { return localView_; }
+
   private:
     template <class ScalarType>
     ScalarType calculateScalarImpl(const FERequirementType& req, Eigen::VectorX<ScalarType>& dx) const {
       const auto& d      = req.getGlobalSolution(Ikarus::FESolutions::displacement);
       const auto& lambda = req.getParameter(Ikarus::FEParameter::loadfactor);
-
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
-      auto& first_child = localView_.tree().child(0);
+      auto& first_child = this->localView().tree().child(0);
       const auto& fe    = first_child.finiteElement();
       Dune::BlockVector<RealTuple<ScalarType, Traits::dimension>> disp(fe.size());
 
       for (auto i = 0U; i < fe.size(); ++i)
         for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
-          disp[i][k2] = dx[i * 2 + k2] + d[localView_.index(localView_.tree().child(k2).localIndex(i))[0]];
+          disp[i][k2]
+              = dx[i * 2 + k2] + d[this->localView().index(this->localView().tree().child(k2).localIndex(i))[0]];
 
       ScalarType energy = 0.0;
 
       decltype(auto) matAD = mat.template rebind<ScalarType>();
 
-      const auto geo = localView_.element().geometry();
+      const auto geo = this->localView().element().geometry();
       Dune::StandardLocalFunction uFunction(localBasis, disp, std::make_shared<const Geometry>(geo));
       for (const auto& [gpIndex, gp] : uFunction.viewOverIntegrationPoints()) {
-        const auto u        = uFunction.evaluate(gpIndex);
         const auto H        = uFunction.evaluateDerivative(gpIndex, Dune::wrt(spatialAll), Dune::on(gridElement));
         const auto E        = (0.5 * (H.transpose() + H + H.transpose() * H)).eval();
         const auto EVoigt   = toVoigt(E);
         auto internalEnergy = matAD.template storedEnergy<StrainTags::greenLagrangian>(EVoigt);
         energy += internalEnergy * geo.integrationElement(gp.position()) * gp.weight();
       }
-      // External forces volume forces over the domain
+
       if (volumeLoad) {
         for (const auto& [gpIndex, gp] : uFunction.viewOverIntegrationPoints()) {
-          const auto uVal                              = uFunction.evaluate(gpIndex);
-          Eigen::Vector<double, Traits::worlddim> fext = (*volumeLoad)(toEigen(gp.position()), lambda);
-          energy -= uVal.dot(fext) * geo.integrationElement(gp.position()) * gp.weight();
+          const auto u                              = uFunction.evaluate(gpIndex);
+          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(gp.position()), lambda);
+          energy -= u.dot(fext) * geo.integrationElement(gp.position()) * gp.weight();
         }
       }
-      const int order = 2 * (localView_.tree().child(0).finiteElement().localBasis().order());
+
+      const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
       // line or surface loads, i.e. neumann boundary
-      if (not neumannBoundary_ and not neumannBoundaryLoad) return energy;
+      if (not neumannBoundary) return energy;
 
-      auto element = localView_.element();
-      for (auto&& intersection : intersections(neumannBoundary_->gridView(), element)) {
-        if (not neumannBoundary_ or not neumannBoundary_->contains(intersection)) continue;
+      auto element = this->localView().element();
+      for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
+        if (not neumannBoundary or not neumannBoundary->contains(intersection)) continue;
 
         const auto& quadLine = Dune::QuadratureRules<double, Traits::mydim - 1>::rule(intersection.type(), order);
 
         for (const auto& curQuad : quadLine) {
           // Local position of the quadrature point
           const Dune::FieldVector<double, Traits::mydim>& quadPos
               = intersection.geometryInInside().global(curQuad.position());
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function
           const auto u = uFunction.evaluate(quadPos);
 
           // Value of the Neumann data at the current position
-          auto neumannValue = (*neumannBoundaryLoad)(toEigen(intersection.geometry().global(curQuad.position())), lambda);
+          auto neumannValue = neumannBoundaryLoad(toEigen(intersection.geometry().global(curQuad.position())), lambda);
 
           energy -= neumannValue.dot(u) * curQuad.weight() * integrationElement;
         }
       }
 
       return energy;
     }
 
-    LocalView localView_;
     Dune::CachedLocalBasis<
         std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
         localBasis;
-    std::optional<std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
-                                                                        const double&)>>
+    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
+                                                          const double&)>
         volumeLoad;
-    std::optional<std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
-                                                                        const double&)>>
+    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
+                                                          const double&)>
         neumannBoundaryLoad;
-    const BoundaryPatch<GridView>* neumannBoundary_;
+    const BoundaryPatch<GridView>* neumannBoundary;
     Material mat;
   };
 
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files 6% similar despite different names*

```diff
@@ -60,44 +60,50 @@
     void fixDOFs(F&& f) {
       f(basis_, dirichletFlagsBackend);
     }
 
     /* \brief Returns the local basis object */
     const auto& basis() const { return basis_; }
 
+    /* \brief Returns a boolean values, if the give multiIndex is constrained */
+    template <typename MultiIndex>
+    requires(not std::integral<MultiIndex>) [[nodiscard]] bool isConstrained(const MultiIndex& multiIndex) const {
+      return dirichletFlagsBackend[multiIndex];
+    }
+
     /* \brief Returns a boolean values, if the i-th degree of freedom is constrained */
     [[nodiscard]] bool isConstrained(std::size_t i) const { return dirichletFlags[i]; }
 
     /* \brief Returns how many degrees of freedoms are fixed */
     auto fixedDOFsize() const { return std::ranges::count(dirichletFlags, true); }
 
     /* \brief Returns how many degrees of freedom there are */
     auto size() const { return dirichletFlags.size(); }
 
     /* \brief Returns the underlying dof flag container */
     auto& container() const { return dirichletFlags; }
 
     /**
-     * \brief Function to insert a function of inhomogenious dirichlet boundary functions
+     * \brief Function to insert a function of inhomogeneous dirichlet boundary functions
      *
      * \param f A callback that will be called with the current coordinate vector and the scalar load factor
      * It creates internally the first derivative of the passed function and stores them simultaneously
      */
     template <typename F>
     void storeInhomogeneousBoundaryCondition(F&& f) {
       auto derivativeLambda = [&](const auto& globalCoord, const double& lambda) {
-        autodiff::real lambdadual = lambda;
-        lambdadual[1]             = 1;  // Setting the derivative in lambda direction to 1
-        return derivative(f(globalCoord, lambdadual));
+        autodiff::real lambdaDual = lambda;
+        lambdaDual[1]             = 1;  // Setting the derivative in lambda direction to 1
+        return derivative(f(globalCoord, lambdaDual));
       };
       dirichletFunctions.push_back({f, derivativeLambda});
     }
 
     /**
-     * \brief Function to evaluate all stored inhomogenious dirichlet boundary functions at all positions where the
+     * \brief Function to evaluate all stored inhomogeneous dirichlet boundary functions at all positions where the
      * corresponding degrees of freedom are true
      *
      * \param xIh The vector where the interpolated result should be stored
      * \param lambda the load factor
      */
     void evaluateInhomogeneousBoundaryCondition(Eigen::VectorXd& xIh, const double& lambda) {
       inhomogeneousBoundaryVectorDummy.setZero();
@@ -108,15 +114,15 @@
             basis_, inhomogeneousBoundaryVectorDummy,
             [&](const auto& globalCoord) { return f.value(globalCoord, lambda); }, dirichletFlagsBackend);
         xIh += inhomogeneousBoundaryVectorDummy;
       }
     }
 
     /**
-     * \brief Function to evaluate all stored inhomogenious dirichlet boundary DERIVATIVE functions at all positions
+     * \brief Function to evaluate all stored inhomogeneous dirichlet boundary DERIVATIVE functions at all positions
      * where the corresponding degrees of freedom are true
      *
      * \param xIh The vector where the interpolated result should be stored
      * \param lambda the load factor
      */
     void evaluateInhomogeneousBoundaryConditionDerivative(Eigen::VectorXd& xIh, const double& lambda) {
       inhomogeneousBoundaryVectorDummy.setZero();
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/python/assembler/flatAssembler.hh`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #include <dune/python/common/typeregistry.hh>
 //#include <dune/python/pybind11/numpy.h>
 #include <dune/python/pybind11/eigen.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
 
 #include <ikarus/finiteElements/feRequirements.hh>
+#include <ikarus/utils/basis.hh>
 
 namespace Ikarus::Python {
 
 #define MAKE_ASSEMBLER_REGISTERY_FUNCTION(name)         \
   template <class Assembler, class... options>  \
 void register##name(pybind11::handle scope, pybind11::class_<Assembler, options...> cls) {  \
   using pybind11::operator""_a;  \
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,105 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
+#include <ikarus/finiteElements/feRequirements.hh>
+
+#include <dune/fufem/boundarypatch.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/python/common/typeregistry.hh>
+#include <dune/python/functions/globalbasis.hh>
 #include <dune/python/pybind11/eigen.h>
+#include <dune/python/pybind11/functional.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
-#include <dune/python/pybind11/functional.h>
-#include <dune/fufem/boundarypatch.hh>
-
-#include <ikarus/finiteElements/feRequirements.hh>
-#include <dune/python/functions/globalbasis.hh>
+#include <ikarus/utils/basis.hh>
 
 namespace Ikarus::Python {
 
-  template <class LinearElastic, class... options>
-  void registerLinearElastic(pybind11::handle scope, pybind11::class_<LinearElastic, options...> cls) {
+  template <class NonLinearElastic, class... options>
+  void registerNonLinearElastic(pybind11::handle scope, pybind11::class_<NonLinearElastic, options...> cls) {
     using pybind11::operator""_a;
 
-    using GlobalBasis    = typename LinearElastic::GlobalBasis;
-    using GridView    = typename GlobalBasis::GridView;
-    using Element        = typename LinearElastic::Element;
-    using Traits        = typename LinearElastic::Traits;
-    using FErequirements = typename LinearElastic::FERequirementType;
+    using GlobalBasis    = typename NonLinearElastic::Basis;
+    using FlatBasis    = typename NonLinearElastic::FlatBasis;
+    using GridView       = typename GlobalBasis::GridView;
+    using Element        = typename NonLinearElastic::Element;
+    using Traits         = typename NonLinearElastic::Traits;
+    using FErequirements = typename NonLinearElastic::FERequirementType;
+    using Material       = typename NonLinearElastic::Material;
 
-    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu) {
-              return new LinearElastic(basis, element, emod, nu);
+    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat) {
+              return new NonLinearElastic(basis, element, mat);
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
 
-    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu,const std::function<Eigen::Vector<double, Traits::worlddim>(Eigen::Vector<double, Traits::worlddim>,
-                                                                                                                                                              const double&)> volumeLoad) {
-              return new LinearElastic(basis, element, emod, nu,volumeLoad);
-            }),
+    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat,
+                              const std::function<Eigen::Vector<double, Traits::worlddim>(
+                                  Eigen::Vector<double, Traits::worlddim>, const double&)>
+                                  volumeLoad) { return new NonLinearElastic(basis, element, mat, volumeLoad); }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
 
-    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, double emod, double nu,const std::function<Eigen::Vector<double, Traits::worlddim>(Eigen::Vector<double, Traits::worlddim>,
-                                                                                                                                                                    const double&)> volumeLoad,const BoundaryPatch<GridView>& bp
-                              ,const std::function<Eigen::Vector<double, Traits::worlddim>(Eigen::Vector<double, Traits::worlddim>,
-                                                                                          const double&)> neumannBoundaryLoad) {
-              return new LinearElastic(basis, element, emod, nu,volumeLoad,&bp,neumannBoundaryLoad);
+    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat,
+                              const std::function<Eigen::Vector<double, Traits::worlddim>(
+                                  Eigen::Vector<double, Traits::worlddim>, const double&)>
+                                  volumeLoad,
+                              const BoundaryPatch<GridView>& bp,
+                              const std::function<Eigen::Vector<double, Traits::worlddim>(
+                                  Eigen::Vector<double, Traits::worlddim>, const double&)>
+                                  neumannBoundaryLoad) {
+              return new NonLinearElastic(basis, element, mat, volumeLoad, &bp, neumannBoundaryLoad);
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>(), pybind11::keep_alive<1, 7>());
 
     pybind11::module scopedf = pybind11::module::import("dune.functions");
 
-    typedef Dune::Python::LocalViewWrapper< GlobalBasis > LocalViewWrapper;
+    typedef Dune::Python::LocalViewWrapper<FlatBasis> LocalViewWrapper;
     auto includes = Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"};
-    auto lv = Dune::Python::insertClass< LocalViewWrapper >( scopedf, "LocalViewWrapper",
-    Dune::Python::GenerateTypeName("Dune::Python::LocalViewWrapperWrapper", Dune::MetaType<GlobalBasis>()),
-        includes).first;
-    lv.def( "bind", &LocalViewWrapper::bind );
-    lv.def( "unbind", &LocalViewWrapper::unbind );
-    lv.def( "index", [] ( const LocalViewWrapper &localView, int index ) { return localView.index( index ); });
-    lv.def( "__len__", [] ( LocalViewWrapper &self ) -> int { return self.size(); } );
+    auto lv
+        = Dune::Python::insertClass<LocalViewWrapper>(
+              scopedf, "LocalViewWrapper",
+              Dune::Python::GenerateTypeName("Dune::Python::LocalViewWrapperWrapper", Dune::MetaType<FlatBasis>()),
+              includes)
+              .first;
+    lv.def("bind", &LocalViewWrapper::bind);
+    lv.def("unbind", &LocalViewWrapper::unbind);
+    lv.def("index", [](const LocalViewWrapper& localView, int index) { return localView.index(index); });
+    lv.def("__len__", [](LocalViewWrapper& self) -> int { return self.size(); });
 
     Dune::Python::Functions::registerTree<typename LocalViewWrapper::Tree>(lv);
     lv.def("tree", [](const LocalViewWrapper& view) { return view.tree(); });
 
-    auto basisName =Dune::className<GlobalBasis>();
-    auto entry = Dune::Python::insertClass<GlobalBasis>(scopedf, "DefaultGlobalBasis", pybind11::buffer_protocol(),
-                                                  Dune::Python::GenerateTypeName(basisName),Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"}
-    );
-    if (entry.second)
-      Dune::Python::registerGlobalBasis(scopedf,entry.first);
+    auto basisName = Dune::className<FlatBasis>();
+    auto entry     = Dune::Python::insertClass<FlatBasis>(
+        scopedf, "DefaultGlobalBasis", pybind11::buffer_protocol(), Dune::Python::GenerateTypeName(basisName),
+        Dune::Python::IncludeFiles{"dune/python/functions/globalbasis.hh"});
+    if (entry.second) Dune::Python::registerGlobalBasis(scopedf, entry.first);
 
     cls.def(
-        "localView", [](LinearElastic& self) -> LocalViewWrapper{
+        "localView",
+        [](NonLinearElastic& self) -> LocalViewWrapper {
           auto lvWrapped = LocalViewWrapper(self.localView().globalBasis());
-          //this can be simplified when https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418 becomes available
+          // this can be simplified when https://gitlab.dune-project.org/staging/dune-functions/-/merge_requests/418
+          // becomes available
           pybind11::object obj = pybind11::cast(self.localView().element());
           lvWrapped.bind(obj);
-          return lvWrapped; } , pybind11::keep_alive< 0, 1 >());
+          return lvWrapped;
+        },
+        pybind11::keep_alive<0, 1>());
     cls.def("calculateScalar",
-            [](LinearElastic& self, const FErequirements& req) { return self.calculateScalar(req); });
-    cls.def("calculateVector", [](LinearElastic& self, const FErequirements& req, Eigen::Ref<Eigen::VectorXd> vec) {
+            [](NonLinearElastic& self, const FErequirements& req) { return self.calculateScalar(req); });
+    cls.def("calculateVector", [](NonLinearElastic& self, const FErequirements& req, Eigen::Ref<Eigen::VectorXd> vec) {
       return self.calculateVector(req, vec);
     });
     cls.def(
         "calculateMatrix",
-        [](LinearElastic& self, const FErequirements& req, Eigen::Ref<Eigen::MatrixXd> mat) {
+        [](NonLinearElastic& self, const FErequirements& req, Eigen::Ref<Eigen::MatrixXd> mat) {
           return self.calculateMatrix(req, mat);
         },
         pybind11::arg("FErequirements"), pybind11::arg("elementMatrix").noconvert());
-
-    cls.def("getMaterialTangent", [](LinearElastic& self) { return self.getMaterialTangent(); });
-
   }
 
 }  // namespace Ikarus::Python
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/python/finiteElements/materials/material.hh`

 * *Files 18% similar despite different names*

```diff
@@ -39,26 +39,26 @@
             return new Materialname(matParameter);\
           })\
               ,"Young's modulus"_a, "Poisson's ratio"_a);\
 MAKE_MaterialFunction(cls##Materialname,Materialname,storedEnergy,vecSize);\
 MAKE_MaterialFunction(cls##Materialname,Materialname,stresses,vecSize);\
 MAKE_MaterialFunction(cls##Materialname,Materialname,tangentModuli,vecSize);     \
  \
-using PlainStressClass = decltype(plainStress(std::declval<Materialname>())); \
+using PlaneStressClass = decltype(planeStress(std::declval<Materialname>())); \
 auto includes = Dune::Python::IncludeFiles{"ikarus/finiteElements/mechanics/materials.hh"}; \
-auto pS = Dune::Python::insertClass< PlainStressClass >( scope, "PlainStressClass", \
+auto pS = Dune::Python::insertClass< PlaneStressClass >( scope, "PlaneStressClass", \
                                                 Dune::Python::GenerateTypeName("Ikarus::VanishingStress<std::array<Ikarus::Impl::StressIndexPair, 3ul>{{Ikarus::Impl::StressIndexPair{2ul, 1ul}, Ikarus::Impl::StressIndexPair{2ul,0ul}, Ikarus::Impl::StressIndexPair{2ul, 2ul}}},"+ Dune::className<Materialname>() +">"), \
                                                 includes).first; \
-    MAKE_MaterialFunction(pS,PlainStressClass,storedEnergy,3);\
-    MAKE_MaterialFunction(pS,PlainStressClass,stresses,3);\
-    MAKE_MaterialFunction(pS,PlainStressClass,tangentModuli,3);\
-    MAKE_MaterialFunction(pS,PlainStressClass,storedEnergy,6);\
-MAKE_MaterialFunction(pS,PlainStressClass,stresses,6);\
-MAKE_MaterialFunction(pS,PlainStressClass,tangentModuli,6);     \
-      cls##Materialname.def("asPlainStress", [](Materialname& self) { return plainStress(self);});    /* no keep_alive since plainStress copies the material */                                             \
+    MAKE_MaterialFunction(pS,PlaneStressClass,storedEnergy,3);\
+    MAKE_MaterialFunction(pS,PlaneStressClass,stresses,3);\
+    MAKE_MaterialFunction(pS,PlaneStressClass,tangentModuli,3);\
+    MAKE_MaterialFunction(pS,PlaneStressClass,storedEnergy,6);\
+MAKE_MaterialFunction(pS,PlaneStressClass,stresses,6);\
+MAKE_MaterialFunction(pS,PlaneStressClass,tangentModuli,6);     \
+      cls##Materialname.def("asPlaneStress", [](Materialname& self) { return planeStress(self);});    /* no keep_alive since planeStress copies the material */                                             \
       cls##Materialname.def("asShellMaterial", [](Materialname& self) { return shellMaterial(self);});    /* no keep_alive since shellMaterial copies the material */                                             \
       cls##Materialname.def("asbeamMaterial", [](Materialname& self) { return beamMaterial(self);});    /* no keep_alive since beamMaterial copies the material */                                             \
 }
 
 #define MAKE_MATERIAL_CLASS_IN_MODULE(Materialname,args) \
   auto includes##Materialname = Dune::Python::IncludeFiles{"ikarus/finiteElements/mechanics/materials.hh"}; \
 auto cls##Materialname       = Dune::Python::insertClass<Ikarus:: Materialname < args >>(\
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/ikarus/python/test/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 configure_file(setpath.py.in ${CMAKE_CURRENT_SOURCE_DIR}/setpath.py)
 
-# dune_python_add_test(NAME pytest1 SCRIPT test1.py WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR} LABELS quick)
-#dune_python_add_test(NAME pytest2 SCRIPT test2.py WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR} LABELS quick)
 dune_python_add_test(
   NAME
   pylinearElasticTest
   SCRIPT
         linearElasticTest.py
   WORKING_DIRECTORY
   ${CMAKE_CURRENT_SOURCE_DIR}
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.0.dev202310000062/ikarus/python/test/linearElasticTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,20 @@
         elements.append(3)
 
     req= ikarus.FErequirements()
     req.addAffordance(iks.ScalarAffordances.mechanicalPotentialEnergy)
 
     grid = dune.grid.structuredGrid(lowerLeft,upperRight,elements)
     grid. hierarchicalGrid . globalRefine(6)
-    basisLagrange1 = dune.functions.defaultGlobalBasis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    basisLagrange12 = dune.functions.defaultGlobalBasis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    dirichletValuesT = iks.dirichletValues(basisLagrange12)
 
-    d = np.zeros(len(basisLagrange1))
+    basisLagrange1 = iks.basis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    flatBasis = basisLagrange1.flat()
+    d = np.zeros(len(flatBasis))
     d[0]=0.0
 
     lambdaLoad = iks.ValueWrapper(3.0)
     req.insertParameter(iks.FEParameter.loadfactor,lambdaLoad)
 
     assert req.getParameter(iks.FEParameter.loadfactor) == lambdaLoad
     req.insertGlobalSolution(iks.FESolutions.displacement,d)
@@ -54,17 +57,17 @@
         return np.array([lambdaVal*x[0]*2, 2*lambdaVal*x[1]*0])
 
     def neumannLoad(x,lambdaVal) :
         return np.array([lambdaVal*0, lambdaVal])
 
 
     neumannVertices = np.zeros(grid.size(2)*2, dtype=bool)
-    assert len(neumannVertices)== len(basisLagrange1)
+    assert len(neumannVertices)== len(flatBasis)
 
-    basisLagrange1.interpolate(neumannVertices, lambda x :  True  if x[1]>0.9 else False)
+    flatBasis.interpolate(neumannVertices, lambda x :  True  if x[1]>0.9 else False)
 
     boundaryPatch = iks.utils.boundaryPatch(grid,neumannVertices)
 
     # the following should throw
     try:
         for e in grid.elements:
             iks.finite_elements.linearElasticElement(basisLagrange1,e,1000,0.2,volumeLoad,boundaryPatch)
@@ -75,15 +78,15 @@
     for e in grid.elements:
         fes.append(iks.finite_elements.linearElasticElement(basisLagrange1,e,1000,0.2,volumeLoad,boundaryPatch,neumannLoad))
 
     fes[0].calculateVector(req,forces)
     fes[0].calculateMatrix(req,stiffness)
     fes[0].localView()
 
-    dirichletValues = iks.dirichletValues(basisLagrange1)
+    dirichletValues = iks.dirichletValues(flatBasis)
 
     def fixFirstIndex(vec,globalIndex):
         vec[0]= True
 
     def fixAnotherVertex(vec,localIndex,localView):
         localView.index(localIndex)
         vec[1]= True
@@ -104,14 +107,14 @@
     # Mdense = assemblerDense.getMatrix(req)
     # assert (Msparse == Mdense).all()
     # print(Mdense)
     # print("F:",forces)
 
     x = sp.sparse.linalg.spsolve(Msparse,-forces)
     # print(x)
-    fx = basisLagrange1.asFunction(x)
+    fx = flatBasis.asFunction(x)
     grid.plot()
     # grid.writeVTK(pointdata={"fx":fx},name="nameTest",number=1)
     writer = vtkWriter( grid, "nameTest",
                     pointData   = {( "displacement",(0,1)):fx}
 
                     )
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.0.dev202310000062/ikarus/python/test/nonLinearElasticTest.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,42 +27,43 @@
         elements.append(3)
 
     req= ikarus.FErequirements()
     req.addAffordance(iks.ScalarAffordances.mechanicalPotentialEnergy)
 
     grid = dune.grid.structuredGrid(lowerLeft,upperRight,elements)
     grid. hierarchicalGrid.globalRefine(0)
-    basisLagrange1 = dune.functions.defaultGlobalBasis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    basisLagrange1 = ikarus.basis(grid, dune.functions.Power(dune.functions.Lagrange(order=1),2))
+    flatBasis = basisLagrange1.flat()
 
 
     forces = np.zeros(8)
     stiffness = np.zeros((8,8))
 
     def volumeLoad(x,lambdaVal) :
         return np.array([lambdaVal*x[0]*2, 2*lambdaVal*x[1]*0])
 
     def neumannLoad(x,lambdaVal) :
         return np.array([lambdaVal*0, lambdaVal])
 
 
     neumannVertices = np.zeros(grid.size(2)*2, dtype=bool)
-    assert len(neumannVertices)== len(basisLagrange1)
+    assert len(neumannVertices)== len(flatBasis)
 
-    basisLagrange1.interpolate(neumannVertices, lambda x :  True  if x[1]>0.9 else False)
+    flatBasis.interpolate(neumannVertices, lambda x :  True  if x[1]>0.9 else False)
 
     boundaryPatch = iks.utils.boundaryPatch(grid,neumannVertices)
 
     svk = iks.StVenantKirchhoff(emodul=1000,nu=0.3)
 
-    psNH = svk.asPlainStress()
+    psNH = svk.asPlaneStress()
     fes = []
     for e in grid.elements:
         fes.append(iks.finite_elements.nonLinearElasticElement(basisLagrange1,e,psNH,volumeLoad,boundaryPatch,neumannLoad))
 
-    dirichletValues = iks.dirichletValues(basisLagrange1)
+    dirichletValues = iks.dirichletValues(flatBasis)
 
     def fixFirstIndex(vec,globalIndex):
         vec[0]= True
 
     def fixAnotherVertex(vec,localIndex,localView):
         localView.index(localIndex)
         vec[1]= True
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.0.dev202310000062/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/python/utils/boundarypatch.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include <dune/functions/functionspacebases/lagrangebasis.hh>
-#include <dune/functions/functionspacebases/powerbasis.hh>
-#include <dune/grid/yaspgrid.hh>
-#include <dune/python/common/typeregistry.hh>
 #include <dune/python/pybind11/eigen.h>
 #include <dune/python/pybind11/pybind11.h>
 #include <dune/python/pybind11/stl.h>
 #include <dune/python/pybind11/functional.h>
 
 #include <ikarus/finiteElements/feRequirements.hh>
-#include <dune/python/functions/globalbasis.hh>
 
 namespace Ikarus::Python {
 
   // Python wrapper for the FVAssembler C++ class
   template <class BoundaryPatch, class... options>
   void registerBoundaryPatch(pybind11::handle scope, pybind11::class_<BoundaryPatch, options...> cls) {
     using pybind11::operator""_a;
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 # install headers
 install(
   FILES algorithms.hh
         autodiffHelper.hh
+        basis.hh
         concepts.hh
         defaultFunctions.hh
         duneUtilities.hh
         eigenDuneTransformations.hh
         eigenSparseAddon.hh
         findLineSegment.hh
+        flatPreBasis.hh
         functionSanityChecks.hh
         init.hh
         linearAlgebraHelper.hh
         makeEnum.hh
         pathFollowingFunctions.hh
         polyfit.hh
         tensorUtils.hh
```

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/algorithms.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/concepts.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/init.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/polyfit.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/ikarus/utils/traits.hh` & `pyikarus-0.3.0.dev202310000062/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/__init__.py` & `pyikarus-0.3.0.dev202310000062/python/ikarus/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,9 @@
     )
 
 except ImportError:
     pass
 
 from ._ikarus import *
 from .dirichletValues import dirichletValues
+from .basis import basis
 from .materials import *
```

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/_ikarus.cc` & `pyikarus-0.3.0.dev202310000062/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000062/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000062/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000062/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/materials.py` & `pyikarus-0.3.0.dev202310000062/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/python/ikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000062/python/ikarus/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     dune.generator.addToFlags(pre="-DCMAKE_PREFIX_PATH=$ENV{CMAKE_PREFIX_PATH}")
     generator = MySimpleGenerator("BoundaryPatch", "Ikarus::Python")
     element_type = f"BoundaryPatch<{gridView.cppTypeName}>"
 
     includes = []
     includes += ["dune/fufem/boundarypatch.hh"]
     includes += ["ikarus/python/utils/boundarypatch.hh"]
+    includes += gridView._includes
     moduleName = "boundaryPatch_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     return module.BoundaryPatch(gridView,booleanVector)
```

### Comparing `pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000061
+Version: 0.3.0.dev202310000062
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000061 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000062 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000061/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.0.dev202310000062/python/pyikarus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 .github/workflows/reuseLint.yml
 .github/workflows/runExamples.yml
 .github/workflows/style.yml
 .reuse/dep5
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/CC0-1.0.txt
 LICENSES/LGPL-3.0-or-later.txt
+LICENSES/MIT.txt
 LICENSES/MPL-2.0.txt
 cmake/CPM.cmake
 cmake/tools.cmake
 cmake/FormatTarget/CMakeLists.txt
 cmake/modules/AddAutoDiffFlags.cmake
 cmake/modules/AddEigenFlags.cmake
 cmake/modules/AddMatplotppFlags.cmake
@@ -144,47 +145,49 @@
 ikarus/linearAlgebra/CMakeLists.txt
 ikarus/linearAlgebra/dirichletValues.hh
 ikarus/linearAlgebra/nonLinearOperator.hh
 ikarus/linearAlgebra/truncatedConjugateGradient.hh
 ikarus/python/CMakeLists.txt
 ikarus/python/assembler/CMakeLists.txt
 ikarus/python/assembler/flatAssembler.hh
+ikarus/python/basis/CMakeLists.txt
+ikarus/python/basis/basis.hh
 ikarus/python/dirichletValues/CMakeLists.txt
 ikarus/python/dirichletValues/dirichletValues.hh
 ikarus/python/finiteElements/CMakeLists.txt
 ikarus/python/finiteElements/linearElastic.hh
 ikarus/python/finiteElements/nonLinearElastic.hh
 ikarus/python/finiteElements/materials/CMakeLists.txt
 ikarus/python/finiteElements/materials/material.hh
 ikarus/python/test/CMakeLists.txt
 ikarus/python/test/linearElasticTest.py
 ikarus/python/test/nameTest.vtu
 ikarus/python/test/nonLinearElasticTest.py
 ikarus/python/test/setpath.py.in
-ikarus/python/test/test1.py
-ikarus/python/test/test2.py
 ikarus/python/utils/CMakeLists.txt
 ikarus/python/utils/boundarypatch.hh
 ikarus/solver/CMakeLists.txt
 ikarus/solver/linearSolver/CMakeLists.txt
 ikarus/solver/linearSolver/linearSolver.hh
 ikarus/solver/nonLinearSolver/CMakeLists.txt
 ikarus/solver/nonLinearSolver/newtonRaphson.hh
 ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
 ikarus/solver/nonLinearSolver/trustRegion.hh
 ikarus/utils/CMakeLists.txt
 ikarus/utils/algorithms.hh
 ikarus/utils/autodiffHelper.hh
+ikarus/utils/basis.hh
 ikarus/utils/concepts.hh
 ikarus/utils/defaultFunctions.hh
 ikarus/utils/duneUtilities.hh
 ikarus/utils/eigenDuneTransformations.hh
 ikarus/utils/eigenSparseAddon.hh
 ikarus/utils/findLineSegment.cpp
 ikarus/utils/findLineSegment.hh
+ikarus/utils/flatPreBasis.hh
 ikarus/utils/functionSanityChecks.cpp
 ikarus/utils/functionSanityChecks.hh
 ikarus/utils/init.hh
 ikarus/utils/linearAlgebraHelper.hh
 ikarus/utils/makeEnum.hh
 ikarus/utils/pathFollowingFunctions.hh
 ikarus/utils/polyfit.cpp
@@ -205,14 +208,15 @@
 ikarus/utils/observer/observer.hh
 ikarus/utils/observer/observerMessages.hh
 python/CMakeLists.txt
 python/setup.py.in
 python/ikarus/CMakeLists.txt
 python/ikarus/__init__.py
 python/ikarus/_ikarus.cc
+python/ikarus/basis.py
 python/ikarus/dirichletValues.py
 python/ikarus/materials.py
 python/ikarus/assembler/CMakeLists.txt
 python/ikarus/assembler/__init__.py
 python/ikarus/finite_elements/CMakeLists.txt
 python/ikarus/finite_elements/__init__.py
 python/ikarus/utils/CMakeLists.txt
```

### Comparing `pyikarus-0.3.0.dev202310000061/python/setup.py.in` & `pyikarus-0.3.0.dev202310000062/python/setup.py.in`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
     name="${ProjectName}",
     description="${ProjectDescription}",
     version="${ProjectVersionString}",
     author="${ProjectAuthor}",
     author_email="${ProjectMaintainerEmail}",
     packages=find_packages(exclude=["docs/*"]),
     zip_safe=0,
-    package_data={"": ["*.so"], "pyikarus": ["data/*.cmake"]},
+    package_data={"": ["*.so"], "ikarus": ["data/*.cmake"]},
     install_requires=REQUIRED_PACKAGES,
     include_package_data=True,
 )
```

### Comparing `pyikarus-0.3.0.dev202310000061/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.0.dev202310000062/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/setup.py` & `pyikarus-0.3.0.dev202310000062/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # You are logged in as $(whoami)
 # EOF
 # nano ~/.pypirc
 # python -m venv /dune/dune-common/build-cmake/dune-env/
 # source /dune/dune-common/build-cmake/dune-env/bin/activate
 # pip install ikarus  --no-build-isolation
 
-ikarusVersion = "0.3.0.dev202310000061" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.0.dev202310000062" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor sicne ikarus pypi package already exists
 print(metadata)
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000062/tests/src/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 find_dependency(autodiff REQUIRED)
 find_dependency(Matplot++ REQUIRED)
 
 file(GLOB programSourceFiles CONFIGURE_DEPENDS *.cpp)
 
 foreach(programSourceFile ${programSourceFiles})
   get_filename_component(programName ${programSourceFile} NAME_WLE)
-  dune_add_test(SOURCES ${programSourceFile} LINK_LIBRARIES ikarus)
+  dune_add_test(SOURCES ${programSourceFile} LINK_LIBRARIES ikarus LABELS
+          cpp)
   target_compile_features(${programName} PUBLIC cxx_std_20)
   set_tests_properties(${programName} PROPERTIES TIMEOUT 1000)
   add_dune_pythonlibs_flags(${programName})
   find_package(PythonLibs REQUIRED)
   include_directories(${PYTHON_INCLUDE_DIRS})
   target_link_libraries(${programName} PUBLIC ${PYTHON_LIBRARIES})
   target_compile_options(${programName} PUBLIC -ftemplate-backtrace-limit=0)
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/assemblerTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/assemblerTest.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 
 using Dune::TestSuite;
 #include <ikarus/assembler/simpleAssemblers.hh>
 #include <ikarus/finiteElements/mechanics/nonLinearElastic.hh>
 #include <ikarus/linearAlgebra/dirichletValues.hh>
+#include <ikarus/utils/basis.hh>
 #include <ikarus/utils/init.hh>
 
 #include <Eigen/Core>
 
 auto SimpleAssemblersTest() {
   TestSuite t("SimpleAssemblersTest");
   using Grid = Dune::YaspGrid<2>;
@@ -30,41 +31,41 @@
   std::array<int, 2> elementsPerDirection = {2, 1};
   auto grid                               = std::make_shared<Grid>(bbox, elementsPerDirection);
 
   for (int i = 0; i < 4; ++i) {
     auto gridView = grid->leafGridView();
 
     using namespace Dune::Functions::BasisFactory;
-    auto basis        = makeBasis(gridView, power<2>(lagrange<1>(), FlatInterleaved()));
+    auto basis        = Ikarus::makeBasis(gridView, power<2>(lagrange<1>()));
     auto matParameter = Ikarus::toLamesFirstParameterAndShearModulus({.emodul = 1000, .nu = 0.3});
 
     Ikarus::StVenantKirchhoff matSVK(matParameter);
-    auto reducedMat = plainStress(matSVK, 1e-8);
+    auto reducedMat = planeStress(matSVK, 1e-8);
     std::vector<Ikarus::NonLinearElastic<decltype(basis), decltype(reducedMat)>> fes;
 
     auto volumeLoad = []([[maybe_unused]] const auto& globalCoord, const auto& lamb) {
       Eigen::Vector2d fext;
       fext.setZero();
       fext[1] = 2 * lamb;
       fext[0] = lamb;
       return fext;
     };
     for (auto&& ge : elements(gridView))
-      fes.emplace_back(basis, ge, reducedMat, nullptr, nullptr, volumeLoad);
+      fes.emplace_back(basis, ge, reducedMat,volumeLoad);
 
     auto basisP = std::make_shared<const decltype(basis)>(basis);
-    Ikarus::DirichletValues dirichletValues(basisP);
+    Ikarus::DirichletValues dirichletValues(basisP->flat());
     dirichletValues.fixDOFs([](auto& basis_, auto& dirichletFlags) {
       Dune::Functions::forEachBoundaryDOF(basis_, [&](auto&& indexGlobal) { dirichletFlags[indexGlobal] = true; });
     });
 
     Ikarus::SparseFlatAssembler sparseFlatAssembler(fes, dirichletValues);
     Ikarus::DenseFlatAssembler denseFlatAssembler(fes, dirichletValues);
 
-    Eigen::VectorXd d(basis.size());
+    Eigen::VectorXd d(basis.flat().size());
     d.setRandom();
     double load = 0.0;
 
     Ikarus::FErequirements req = Ikarus::FErequirements()
                                      .insertGlobalSolution(Ikarus::FESolutions::displacement, d)
                                      .insertParameter(Ikarus::FEParameter::loadfactor, load)
                                      .addAffordance(Ikarus::MatrixAffordances::stiffness);
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/common.hh` & `pyikarus-0.3.0.dev202310000062/tests/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/dirichletValueTest.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #include <dune/functions/functionspacebases/powerbasis.hh>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/localfefunctions/eigenDuneTransformations.hh>
 
 #include <Eigen/Core>
 
 #include <ikarus/linearAlgebra/dirichletValues.hh>
+#include <ikarus/utils/basis.hh>
 #include <ikarus/utils/duneUtilities.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/init.hh>
 
 using Dune::TestSuite;
 
 auto dirichletBCTest() {
@@ -33,25 +34,27 @@
   Dune::FieldVector<double, 2> bbox       = {4, 2};
   std::array<int, 2> elementsPerDirection = {2, 1};
   auto grid                               = std::make_shared<Grid>(bbox, elementsPerDirection);
 
   auto gridView = grid->leafGridView();
 
   using namespace Dune::Functions::BasisFactory;
-  auto basis = Ikarus::makeConstSharedBasis(gridView, power<2>(lagrange<1>(), FlatInterleaved()));
+  auto basis = Ikarus::makeBasis(gridView, power<2>(lagrange<1>()));
 
-  Ikarus::DirichletValues dirichletValues1(basis);
+  auto basisP = std::make_shared<const decltype(basis)>(basis);
+
+  Ikarus::DirichletValues dirichletValues1(basisP->flat());
   dirichletValues1.fixDOFs([](auto& basis_, auto& dirichFlags) {
     Dune::Functions::forEachBoundaryDOF(basis_, [&](auto&& indexGlobal) { dirichFlags[indexGlobal] = true; });
   });
 
-  Ikarus::DirichletValues dirichletValues2(basis);
+  Ikarus::DirichletValues dirichletValues2(basisP->flat());
   dirichletValues2.fixBoundaryDOFs([](auto& dirichFlags, auto&& indexGlobal) { dirichFlags[indexGlobal] = true; });
 
-  for (std::size_t i = 0; i < basis->size(); ++i)
+  for (std::size_t i = 0; i < basisP->flat().size(); ++i)
     t.check(dirichletValues1.isConstrained(i) == dirichletValues2.isConstrained(i))
         << "Different dirichlet value creations didn't provide the same result. Index: i=" << i;
 
   auto inhomogeneousDisplacement = []<typename T>(const auto& globalCoord, const T& lambda) {
     Eigen::Vector<T, 2> localInhomogeneous;
     if (globalCoord[0] > 4 - 1e-8) {
       localInhomogeneous[0] = 4 * lambda;
@@ -85,15 +88,15 @@
           << "Values differ dispDerivs[i]: " << dispDerivs[globalIndex[0]];
     } else if (intersection.geometry().center()[0] < 1e-8) {
       t.check(Dune::FloatCmp::eq(disps[globalIndex[0]], 14.0)) << "Values differ disps[i]: " << disps[globalIndex[0]];
       t.check(Dune::FloatCmp::eq(dispDerivs[globalIndex[0]], 7.0))
           << "Values differ dispDerivs[i]: " << dispDerivs[globalIndex[0]];
     }
   };
-  Dune::Functions::forEachBoundaryDOF(*basis, lambdaCheck);
+  Dune::Functions::forEachBoundaryDOF(basisP->flat(), lambdaCheck);
 
   // Check that we can store lambda from python
   std::string inhomogeneousDisplacementFunction
       = std::string("lambda globalCoord,lam: ( numpy.array([1*lam*globalCoord[0], 2*lam*globalCoord[1]]) )");
 
   Python::start();
   Python::Reference main = Python::import("__main__");
@@ -120,15 +123,15 @@
   auto inhomogeneousDisplacementFromPython = [&]<typename T>(const auto& globalCoord, const T& lambda_) {
     auto pythonFunc
         = Python::make_function<Dune::FieldVector<T, 2>>(Python::evaluate(inhomogeneousDisplacementFunction));
 
     return Dune::toEigen(pythonFunc(globalCoord, lambda_));
   };
   //
-  Ikarus::DirichletValues dirichletValues3(basis);
+  Ikarus::DirichletValues dirichletValues3(basisP->flat());
   dirichletValues3.fixBoundaryDOFs([](auto& dirichFlags, auto&& indexGlobal) { dirichFlags[indexGlobal] = true; });
 
   Eigen::VectorXd disps2, dispDerivs2;
   dirichletValues3.storeInhomogeneousBoundaryCondition(inhomogeneousDisplacementFromPython);
   double lambda3 = 6;
   dirichletValues3.evaluateInhomogeneousBoundaryCondition(disps2, lambda3);
   dirichletValues3.evaluateInhomogeneousBoundaryConditionDerivative(dispDerivs2, lambda3);
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/easTest.hh` & `pyikarus-0.3.0.dev202310000062/tests/src/easTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/factories.hh` & `pyikarus-0.3.0.dev202310000062/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/linearElasticityTest.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -3,40 +3,45 @@
 
 #include <config.h>
 
 #include "testFEElement.hh"
 
 #include <dune/common/test/testsuite.hh>
 #include <dune/functions/functionspacebases/basistags.hh>
+#include <dune/functions/functionspacebases/compositebasis.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 
 #include <ikarus/finiteElements/mechanics/linearElastic.hh>
+#include <ikarus/utils/flatPreBasis.hh>
 #include <ikarus/utils/init.hh>
 
 using Dune::TestSuite;
 
 template <typename Basis>
 using LinearElasticElement = Ikarus::LinearElastic<Basis>;
 
 int main(int argc, char** argv) {
   Ikarus::init(argc, argv);
   Dune::TestSuite t("LinearElasticity");
 
   using namespace Dune::Functions::BasisFactory;
-  auto firstOrderLagrangePrePower2Basis  = power<2>(lagrange<1>(), FlatInterleaved());
-  auto secondOrderLagrangePrePower2Basis = power<2>(lagrange<2>(), FlatInterleaved());
-  auto firstOrderLagrangePrePower3Basis  = power<3>(lagrange<1>(), FlatInterleaved());
-  auto secondOrderLagrangePrePower3Basis = power<3>(lagrange<2>(), FlatInterleaved());
+  auto firstOrderLagrangePrePower2Basis         = power<2>(lagrange<1>(), FlatInterleaved());
+  auto secondOrderLagrangePrePower2Basis        = power<2>(lagrange<2>(), FlatInterleaved());
+  auto firstOrderLagrangePrePower3Basis         = power<3>(lagrange<1>(), FlatInterleaved());
+  auto secondOrderLagrangePrePower3Basis        = power<3>(lagrange<2>(), FlatInterleaved());
+  auto secondOrderLagrangePrePower3BasisBlocked = power<3>(lagrange<2>());
 
   t.subTest(testFEElement<LinearElasticElement, 2>(firstOrderLagrangePrePower2Basis, "LinearElastic", true,
                                                    checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
   t.subTest(testFEElement<LinearElasticElement, 2>(secondOrderLagrangePrePower2Basis, "LinearElastic", true,
                                                    checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
   t.subTest(testFEElement<LinearElasticElement, 3>(firstOrderLagrangePrePower3Basis, "LinearElastic", true,
                                                    checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
   t.subTest(testFEElement<LinearElasticElement, 3>(secondOrderLagrangePrePower3Basis, "LinearElastic", true,
                                                    checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
+  t.subTest(testFEElement<LinearElasticElement, 3>(secondOrderLagrangePrePower3BasisBlocked, "LinearElastic", true,
+                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
   t.subTest(testFEElement<LinearElasticElement, 2>(firstOrderLagrangePrePower2Basis, "LinearElastic", false,
                                                    checkCauchyStressFunctor));
   return t.exit();
 }
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/materialTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/materialTest.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -169,12 +169,12 @@
 
   auto nhRed4 = shellMaterial(nh, 1e-12);
   t.subTest(testMaterial(nhRed4));
 
   auto nhRed5 = beamMaterial(nh, 1e-12);
   t.subTest(testMaterial(nhRed5));
 
-  auto nhRed6 = plainStress(nh, 1e-12);
+  auto nhRed6 = planeStress(nh, 1e-12);
   t.subTest(testMaterial(nhRed6));
 
   return t.exit();
 }
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/nonLinearElasticityTest.hh` & `pyikarus-0.3.0.dev202310000062/tests/src/nonLinearElasticityTest.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,156 @@
-// SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
-// SPDX-License-Identifier: LGPL-3.0-or-later
-
-//
-#include <config.h>
-
-#include "common.hh"
-#include "testHelpers.hh"
-
-#include <ikarus/assembler/simpleAssemblers.hh>
-#include <ikarus/controlRoutines/loadControl.hh>
-#include <ikarus/finiteElements/mechanics/nonLinearElastic.hh>
-#include <ikarus/linearAlgebra/dirichletValues.hh>
-#include <ikarus/linearAlgebra/nonLinearOperator.hh>
-#include <ikarus/solver/nonLinearSolver/newtonRaphson.hh>
-#include <ikarus/solver/nonLinearSolver/trustRegion.hh>
-#include <ikarus/utils/algorithms.hh>
-#include <ikarus/utils/drawing/griddrawer.hh>
-#include <ikarus/utils/init.hh>
-#include <ikarus/utils/observer/controlVTKWriter.hh>
-
-#include <dune/common/test/testsuite.hh>
-#include <dune/functions/functionspacebases/basistags.hh>
-#include <dune/functions/functionspacebases/boundarydofs.hh>
-#include <dune/functions/functionspacebases/lagrangebasis.hh>
-#include <dune/functions/functionspacebases/powerbasis.hh>
-
-#include "spdlog/spdlog.h"
-
-#include <Eigen/Core>
-
-using Dune::TestSuite;
-
-template <typename Grid, typename Material>
-auto NonLinearElasticityLoadControlNRandTR(const Material& mat) {
-  TestSuite t("NonLinearElasticityLoadControlNRandTR" + Dune::className(Grid{}));
-  auto grid     = createGrid<Grid>();
-  auto gridView = grid->leafGridView();
-
-  using namespace Ikarus;
-
-  using namespace Dune::Functions::BasisFactory;
-  auto basis = makeBasis(gridView, power<2>(lagrange<1>(), FlatInterleaved()));
-
-  auto g          = basis.localView();
-  auto volumeLoad = []([[maybe_unused]] auto& globalCoord, auto& lamb) {
-    Eigen::Vector2d fext;
-    fext.setZero();
-    fext[1] = 2 * lamb;
-    fext[0] = lamb;
-    return fext;
-  };
-
-  auto reducedMat = plainStress(mat, 1e-8);
-
-  std::vector<Ikarus::NonLinearElastic<decltype(basis), decltype(reducedMat)>> fes;
-
-  for (auto& element : elements(gridView))
-    fes.emplace_back(basis, element, reducedMat, nullptr, nullptr, volumeLoad);
-  auto basisP = std::make_shared<const decltype(basis)>(basis);
-  Ikarus::DirichletValues dirichletValues(basisP);
-  dirichletValues.fixBoundaryDOFs([&](auto& dirichletFlags, auto&& localIndex, auto&& localView, auto&& intersection) {
-    if (std::abs(intersection.geometry().center()[1]) < 1e-8) dirichletFlags[localView.index(localIndex)] = true;
-  });
-
-  auto sparseAssembler = SparseFlatAssembler(fes, dirichletValues);
-
-  Eigen::VectorXd d;
-  d.setZero(basis.size());
-  double lambda = 0.0;
-
-  auto req = FErequirements().addAffordance(Ikarus::AffordanceCollections::elastoStatics);
-
-  auto residualFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
-    req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
-        .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
-    return sparseAssembler.getVector(req);
-  };
-
-  auto KFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
-    req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
-        .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
-    return sparseAssembler.getMatrix(req);
-  };
-
-  auto energyFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
-    req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
-        .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
-    return sparseAssembler.getScalar(req);
-  };
-
-  auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(energyFunction, residualFunction, KFunction),
-                                            parameter(d, lambda));
-  //  t.check(checkGradient(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkGradient Failed";
-  //  t.check(checkHessian(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkHessian Failed";
-
-  const double gradTol = 1e-8;
-
-  auto tr = Ikarus::makeTrustRegion(nonLinOp);
-  tr->setup({.verbosity = 1,
-             .maxiter   = 1000,
-             .grad_tol  = gradTol,
-             .corr_tol  = 1e-16,  // everything should converge to the gradient tolerance
-             .useRand   = false,
-             .rho_reg   = 1e8,
-             .Delta0    = 1});
-
-  auto vtkWriter = std::make_shared<ControlSubsamplingVertexVTKWriter<decltype(basis)>>(basis, d, 2);
-  vtkWriter->setFileNamePrefix("Test2Dsolid");
-  vtkWriter->setFieldInfo("Displacement", Dune::VTK::FieldInfo::Type::vector, 2);
-
-  auto lc = Ikarus::LoadControl(tr, 1, {0, 50});
-  lc.subscribeAll(vtkWriter);
-  const auto controlInfo = lc.run();
-  nonLinOp.template update<0>();
-  const auto maxDisp = std::ranges::max(d);
-  const double energyExpected
-      = (std::is_same_v<Grid, Grids::Yasp>)
-            ? -2.9593431593780032962
-            : ((std::is_same_v<Grid, Grids::Alu>) ? -2.9530594665063669702
-                                                  : /* std::is_same_v<Grid, Grids::Iga> */ -1.4533281398929942529);
-  const double maxDispExpected
-      = (std::is_same_v<Grid, Grids::Yasp>)
-            ? 0.11291304159624337977
-            : ((std::is_same_v<Grid, Grids::Alu>) ? 0.1123397197762363714
-                                                  : /* std::is_same_v<Grid, Grids::Iga> */ 0.061647849558021668159);
-  std::cout << std::setprecision(20) << nonLinOp.value() << std::endl;
-  std::cout << "Maxdisp: " << maxDisp << std::endl;
-  if constexpr (std::is_same_v<Material, Ikarus::StVenantKirchhoff<>>) {
-    t.check(Dune::FloatCmp::eq(energyExpected, nonLinOp.value()), "energyExpected == nonLinOp.value()")
-        << "energyExpected: " << energyExpected << "\nnonLinOp.value(): " << nonLinOp.value();
-
-    t.check(std::abs(maxDispExpected - maxDisp) < 1e-12, "maxDispExpected-maxDisp")
-        << "maxDispExpected: \n"
-        << maxDispExpected << "\nmaxDisp: \n"
-        << maxDisp;
-  } else {  // using a Neohooke material yields a lower energy and larger displacements
-    t.check(Dune::FloatCmp::gt(energyExpected, nonLinOp.value()), "energyExpected > nonLinOp.value()")
-        << "energyExpected: " << energyExpected << "\nnonLinOp.value(): " << nonLinOp.value();
-
-    t.check(maxDispExpected < maxDisp, "maxDispExpected<maxDisp") << "maxDispExpected: \n"
-                                                                  << maxDispExpected << "\nmaxDisp: \n"
-                                                                  << maxDisp;
-  }
-
-  nonLinOp.template update<1>();
-  t.check(controlInfo.success, "Successful result");
-  t.check(gradTol >= nonLinOp.derivative().norm(), "Gradient Tolerance should be larger than actual tolerance");
-  return t;
-}
+// SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
+// SPDX-License-Identifier: LGPL-3.0-or-later
+
+#include <config.h>
+
+#include "common.hh"
+#include "testHelpers.hh"
+
+#include <ikarus/assembler/simpleAssemblers.hh>
+#include <ikarus/controlRoutines/loadControl.hh>
+#include <ikarus/finiteElements/mechanics/nonLinearElastic.hh>
+#include <ikarus/linearAlgebra/dirichletValues.hh>
+#include <ikarus/linearAlgebra/nonLinearOperator.hh>
+#include <ikarus/solver/nonLinearSolver/newtonRaphson.hh>
+#include <ikarus/solver/nonLinearSolver/trustRegion.hh>
+#include <ikarus/utils/algorithms.hh>
+#include <ikarus/utils/drawing/griddrawer.hh>
+#include <ikarus/utils/init.hh>
+#include <ikarus/utils/observer/controlVTKWriter.hh>
+
+#include <dune/common/test/testsuite.hh>
+#include <dune/functions/functionspacebases/basistags.hh>
+#include <dune/functions/functionspacebases/boundarydofs.hh>
+#include <dune/functions/functionspacebases/lagrangebasis.hh>
+#include <dune/functions/functionspacebases/powerbasis.hh>
+
+#include <spdlog/spdlog.h>
+#include <ikarus/utils/basis.hh>
+
+#include <Eigen/Core>
+
+using Dune::TestSuite;
+
+template <typename Grid, typename Material>
+auto NonLinearElasticityLoadControlNRandTR(const Material& mat) {
+  TestSuite t("NonLinearElasticityLoadControlNRandTR " + Dune::className(Grid{}) + " "+ Dune::className(mat));
+  auto grid     = createGrid<Grid>();
+  auto gridView = grid->leafGridView();
+
+  using namespace Ikarus;
+
+  using namespace Dune::Functions::BasisFactory;
+  auto basis = Ikarus::makeBasis(gridView, power<2>(lagrange<1>(), FlatInterleaved()));
+//  auto g          = basis.flat().localView();
+  auto volumeLoad = []([[maybe_unused]] auto& globalCoord, auto& lamb) {
+    Eigen::Vector2d fext;
+    fext.setZero();
+    fext[1] = 2 * lamb;
+    fext[0] = lamb;
+    return fext;
+  };
+
+  auto reducedMat = planeStress(mat, 1e-8);
+
+  std::vector<Ikarus::NonLinearElastic<decltype(basis), decltype(reducedMat)>> fes;
+
+  for (auto& element : elements(gridView))
+    fes.emplace_back(basis, element, reducedMat,volumeLoad);
+
+  Ikarus::DirichletValues dirichletValues(basis.flat());
+  dirichletValues.fixBoundaryDOFs([&](auto& dirichletFlags, auto&& localIndex, auto&& localView, auto&& intersection) {
+    if (std::abs(intersection.geometry().center()[1]) < 1e-8) dirichletFlags[localView.index(localIndex)] = true;
+  });
+
+  auto sparseAssembler = SparseFlatAssembler(fes, dirichletValues);
+
+  Eigen::VectorXd d;
+  d.setZero(basis.flat().size());
+  double lambda = 0.0;
+
+  auto req = FErequirements().addAffordance(Ikarus::AffordanceCollections::elastoStatics);
+
+  auto residualFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
+    req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
+        .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
+    return sparseAssembler.getVector(req);
+  };
+
+  auto KFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
+    req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
+        .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
+    return sparseAssembler.getMatrix(req);
+  };
+
+  auto energyFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
+    req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
+        .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
+    return sparseAssembler.getScalar(req);
+  };
+
+  auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(energyFunction, residualFunction, KFunction),
+                                            parameter(d, lambda));
+  //  t.check(checkGradient(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkGradient Failed";
+  //  t.check(checkHessian(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkHessian Failed";
+
+  const double gradTol = 1e-8;
+
+  auto tr = Ikarus::makeTrustRegion(nonLinOp);
+  tr->setup({.verbosity = 1,
+             .maxiter   = 1000,
+             .grad_tol  = gradTol,
+             .corr_tol  = 1e-16,  // everything should converge to the gradient tolerance
+             .useRand   = false,
+             .rho_reg   = 1e8,
+             .Delta0    = 1});
+
+  using FlatBasis = decltype(basis)::FlatBasis;
+  auto vtkWriter = std::make_shared<ControlSubsamplingVertexVTKWriter<FlatBasis>>(basis.flat(), d, 2);
+  vtkWriter->setFileNamePrefix("Test2Dsolid");
+  vtkWriter->setFieldInfo("Displacement", Dune::VTK::FieldInfo::Type::vector, 2);
+
+  auto lc = Ikarus::LoadControl(tr, 1, {0, 50});
+  lc.subscribeAll(vtkWriter);
+  const auto controlInfo = lc.run();
+  nonLinOp.template update<0>();
+  const auto maxDisp = std::ranges::max(d);
+  double energyExpected;
+  if (std::is_same_v<Grid, Grids::Yasp>)
+    energyExpected =-2.9593431593780032962;
+        else if (std::is_same_v<Grid, Grids::Alu>)
+    energyExpected =-2.9530594665063669702;
+        else  /* std::is_same_v<Grid, Grids::Iga> */
+    energyExpected = -1.4533281398929942529;
+
+  double maxDispExpected;
+  if (std::is_same_v<Grid, Grids::Yasp>)
+    maxDispExpected =0.11291304159624337977;
+  else if (std::is_same_v<Grid, Grids::Alu>)
+    maxDispExpected =0.1123397197762363714;
+  else  /* std::is_same_v<Grid, Grids::Iga> */
+    maxDispExpected =  0.061647849558021668159;
+
+  std::cout << std::setprecision(20) << nonLinOp.value() << std::endl;
+  std::cout << "Maxdisp: " << maxDisp << std::endl;
+  if constexpr (std::is_same_v<Material, Ikarus::StVenantKirchhoff<>>) {
+    t.check(Dune::FloatCmp::eq(energyExpected, nonLinOp.value()), "energyExpected == nonLinOp.value()")
+        << "energyExpected: " << energyExpected << "\nnonLinOp.value(): " << nonLinOp.value();
+
+    t.check(std::abs(maxDispExpected - maxDisp) < 1e-12, "maxDispExpected-maxDisp")
+        << "\nmaxDispExpected: \n"
+        << maxDispExpected << "\nmaxDisp: \n"
+        << maxDisp;
+  } else {  // using a Neohooke material yields a lower energy and larger displacements
+    t.check(Dune::FloatCmp::gt(energyExpected, nonLinOp.value()), "energyExpected > nonLinOp.value()")
+        << "energyExpected: " << energyExpected << "\nnonLinOp.value(): " << nonLinOp.value();
+
+    t.check(maxDispExpected < maxDisp, "maxDispExpected<maxDisp") << "maxDispExpected: \n"
+                                                                  << maxDispExpected << "\nmaxDisp: \n"
+                                                                  << maxDisp;
+  }
+
+  nonLinOp.template update<1>();
+  t.check(controlInfo.success, "Successful result");
+  t.check(gradTol >= nonLinOp.derivative().norm(), "Gradient Tolerance should be larger than actual tolerance");
+  return t;
+}
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/polyFitTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/testFEElement.hh` & `pyikarus-0.3.0.dev202310000062/tests/src/testFEElement.hh`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #include <dune/fufem/boundarypatch.hh>
 #include <dune/grid/uggrid.hh>
 
 #include <ikarus/assembler/simpleAssemblers.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/linearAlgebra/dirichletValues.hh>
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
+#include <ikarus/utils/basis.hh>
 
 /** These tests test your element on some gridElement with some basis
  *
  * @tparam FEElementTemplate The element as template template parameter. The template needs to be the globalBasis
  * @tparam gridDim The dimension of the grid element the finite element should be tested
  * @tparam PreBasis The preBasis you want to test the element with
  * @tparam F A variadic number of the test functor you want to be checked, they need to accept a non-linear operator and
@@ -49,17 +50,18 @@
 
   std::unique_ptr<Grid> grid = gridFactory.createGrid();
 
   auto gridView = grid->leafGridView();
   using namespace Ikarus;
 
   using namespace Dune::Functions::BasisFactory;
-  auto basis = makeBasis(gridView, preBasis);
+  auto basis     = Ikarus::makeBasis(gridView, preBasis);
+  auto flatBasis = basis.flat();
 
-  auto localView = basis.localView();
+  auto localView = flatBasis.localView();
 
   auto volumeLoad = []<typename VectorType>([[maybe_unused]] const VectorType& globalCoord, auto& lamb) {
     VectorType fext;
     fext.setZero();
     fext[1] = 2 * lamb;
     fext[0] = lamb;
     return fext;
@@ -80,40 +82,40 @@
 
   const double youngsModulus = 1000;
   const double poissonsRatio = 0.3;
   auto element               = gridView.template begin<0>();
 
   using FEElementType = FEElementTemplate<decltype(basis)>;
   std::vector<FEElementType> fes;
-  fes.emplace_back(basis, *element, youngsModulus, poissonsRatio, &volumeLoad, &neumannBoundary, &neumannBoundaryLoad);
+  fes.emplace_back(basis, *element, youngsModulus, poissonsRatio, volumeLoad, &neumannBoundary, neumannBoundaryLoad);
   auto basisP = std::make_shared<const decltype(basis)>(basis);
 
-  Ikarus::DirichletValues dirichletValues(basisP);
+  Ikarus::DirichletValues dirichletValues(basisP->flat());
   auto& fe             = fes[0];
   auto sparseAssembler = SparseFlatAssembler(fes, dirichletValues);
 
   typename FEElementType::FERequirementType::SolutionVectorTypeRaw d;
-  d.setRandom(basis.size());
+  d.setRandom(basis.flat().size());
 
   double lambda = 7.3;
 
   auto requirements = FErequirements()
                           .insertParameter(Ikarus::FEParameter::loadfactor, lambda)
                           .addAffordance(Ikarus::AffordanceCollections::elastoStatics);
   Eigen::VectorXd forces;
   Eigen::MatrixXd stiffnessmatrix;
 
   auto fvLambda = [&](auto&& d_) -> auto {
-    forces.setZero(basis.localView().maxSize());
+    forces.setZero(flatBasis.localView().maxSize());
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getScalar(requirements);
   };
 
   auto dfvLambda = [&](auto&& d_) -> auto& {
-    forces.setZero(basis.localView().maxSize());
+    forces.setZero(flatBasis.localView().maxSize());
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getVector(requirements);
   };
   auto ddfvLambda = [&](auto&& d_) -> auto& {
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getMatrix(requirements);
   };
```

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.0.dev202310000062/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/testHelpers.hh` & `pyikarus-0.3.0.dev202310000062/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000061/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.0.dev202310000062/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

