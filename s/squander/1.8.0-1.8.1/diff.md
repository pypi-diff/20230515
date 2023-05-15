# Comparing `tmp/squander-1.8.0.tar.gz` & `tmp/squander-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squander-1.8.0.tar", last modified: Sat May 13 12:18:39 2023, max compression
+gzip compressed data, was "squander-1.8.1.tar", last modified: Mon May 15 09:26:12 2023, max compression
```

## Comparing `squander-1.8.0.tar` & `squander-1.8.1.tar`

### file list

```diff
@@ -1,188 +1,192 @@
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15910 2023-05-13 12:17:13.000000 squander-1.8.0/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    35149 2023-05-13 12:17:13.000000 squander-1.8.0/LICENSE
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      121 2023-05-13 12:17:13.000000 squander-1.8.0/MANIFEST.in
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    17824 2023-05-13 12:18:39.478572 squander-1.8.0/PKG-INFO
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    17284 2023-05-13 12:17:13.000000 squander-1.8.0/README.md
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.462572 squander-1.8.0/cmake/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4306 2023-05-13 12:17:13.000000 squander-1.8.0/cmake/check_AVX.cmake
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.466572 squander-1.8.0/common/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6776 2023-05-13 12:17:13.000000 squander-1.8.0/common/Adam.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8316 2023-05-13 12:17:13.000000 squander-1.8.0/common/common.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-13 12:17:13.000000 squander-1.8.0/common/common_DFE.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5524 2023-05-13 12:17:13.000000 squander-1.8.0/common/config_element.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14292 2023-05-13 12:17:13.000000 squander-1.8.0/common/dot.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.466572 squander-1.8.0/common/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3441 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/Adam.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      216 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/Config.h.in
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2109 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/QGDTypes.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/common.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3026 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/common_DFE.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3423 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/config_element.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7626 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/dot.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2443 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/logging.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3812 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/matrix.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13485 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/matrix_base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3746 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/matrix_real.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1393 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/mpi_base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1468 2023-05-13 12:17:13.000000 squander-1.8.0/common/include/numpy_interface.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2515 2023-05-13 12:17:13.000000 squander-1.8.0/common/logging.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5065 2023-05-13 12:17:13.000000 squander-1.8.0/common/matrix.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4491 2023-05-13 12:17:13.000000 squander-1.8.0/common/matrix_real.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1095 2023-05-13 12:17:13.000000 squander-1.8.0/common/mpi_base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4808 2023-05-13 12:17:13.000000 squander-1.8.0/common/numpy_interface.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.466572 squander-1.8.0/decomposition/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    57993 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    37081 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/N_Qubit_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   111147 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/N_Qubit_Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16714 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    77244 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/N_Qubit_Decomposition_adaptive.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    12741 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/N_Qubit_Decomposition_custom.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    24660 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/Sub_Matrix_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8536 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.466572 squander-1.8.0/decomposition/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16087 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7166 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/N_Qubit_Decomposition.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16028 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/N_Qubit_Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5077 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8301 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/N_Qubit_Decomposition_adaptive.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3393 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/N_Qubit_Decomposition_custom.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6860 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/Sub_Matrix_Decomposition.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3723 2023-05-13 12:17:13.000000 squander-1.8.0/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.470572 squander-1.8.0/gates/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5728 2023-05-13 12:17:13.000000 squander-1.8.0/gates/Adaptive.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4900 2023-05-13 12:17:13.000000 squander-1.8.0/gates/CH.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4937 2023-05-13 12:17:13.000000 squander-1.8.0/gates/CNOT.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5839 2023-05-13 12:17:13.000000 squander-1.8.0/gates/CRY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4841 2023-05-13 12:17:13.000000 squander-1.8.0/gates/CZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7781 2023-05-13 12:17:13.000000 squander-1.8.0/gates/Composite.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11545 2023-05-13 12:17:13.000000 squander-1.8.0/gates/Gate.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   120998 2023-05-13 12:17:13.000000 squander-1.8.0/gates/Gates_block.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8547 2023-05-13 12:17:13.000000 squander-1.8.0/gates/ON.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6819 2023-05-13 12:17:13.000000 squander-1.8.0/gates/RX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6815 2023-05-13 12:17:13.000000 squander-1.8.0/gates/RY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7110 2023-05-13 12:17:13.000000 squander-1.8.0/gates/RZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8697 2023-05-13 12:17:13.000000 squander-1.8.0/gates/SX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9587 2023-05-13 12:17:13.000000 squander-1.8.0/gates/SYC.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15472 2023-05-13 12:17:13.000000 squander-1.8.0/gates/U3.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8769 2023-05-13 12:17:13.000000 squander-1.8.0/gates/UN.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7950 2023-05-13 12:17:13.000000 squander-1.8.0/gates/X.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5671 2023-05-13 12:17:13.000000 squander-1.8.0/gates/Y.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5672 2023-05-13 12:17:13.000000 squander-1.8.0/gates/Z.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.470572 squander-1.8.0/gates/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3395 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/Adaptive.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2428 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/CH.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2504 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/CNOT.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3113 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/CRY.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2427 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/CZ.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3594 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/Composite.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5097 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/Gate.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15824 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/Gates_block.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/ON.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2812 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/RX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3088 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/RY.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2808 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/RZ.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2783 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/SX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2428 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/SYC.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6017 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/U3.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/UN.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2774 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/X.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2772 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/Y.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2772 2023-05-13 12:17:13.000000 squander-1.8.0/gates/include/Z.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.470572 squander-1.8.0/gates/kernels/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23561 2023-05-13 12:17:13.000000 squander-1.8.0/gates/kernels/apply_kernel_to_input_AVX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    32382 2023-05-13 12:17:13.000000 squander-1.8.0/gates/kernels/apply_kernel_to_state_vector_input.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.470572 squander-1.8.0/gates/kernels/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1786 2023-05-13 12:17:13.000000 squander-1.8.0/gates/kernels/include/apply_kernel_to_input_AVX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2099 2023-05-13 12:17:13.000000 squander-1.8.0/gates/kernels/include/apply_kernel_to_state_vector_input.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.470572 squander-1.8.0/nn/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    18464 2023-05-13 12:17:13.000000 squander-1.8.0/nn/NN.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.470572 squander-1.8.0/nn/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5274 2023-05-13 12:17:13.000000 squander-1.8.0/nn/include/NN.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.474572 squander-1.8.0/optimization_engines/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9698 2023-05-13 12:17:13.000000 squander-1.8.0/optimization_engines/RL_experience.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.474572 squander-1.8.0/optimization_engines/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3549 2023-05-13 12:17:13.000000 squander-1.8.0/optimization_engines/include/RL_experience.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      123 2023-05-13 12:17:13.000000 squander-1.8.0/pyproject.toml
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.474572 squander-1.8.0/qgd_python/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/__init__.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.474572 squander-1.8.0/qgd_python/decomposition/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4386 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7661 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    36730 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    24494 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    80282 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14278 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    41007 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3367 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.474572 squander-1.8.0/qgd_python/decomposition/test/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11024 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_Compression.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_Global_Phase.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7037 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_IBM.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1777 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_Project_Name.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5616 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_QX2.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4399 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_State_Preparation.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1656 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_Unitary.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4672 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_decomposition.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7190 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_fmo.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7018 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_heavy_hex.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5222 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_optmization_problem_combined.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4905 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/decomposition/test/test_parametric_circuit.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/qgd_python/gates/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13547 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8219 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_CH.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8160 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_CNOT.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8033 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_CZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    28536 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_Gates_Block.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8529 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_RX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8528 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_RY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8527 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_RZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7771 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_SX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7801 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_SYC.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9054 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_U3.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7489 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_X.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8367 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_Y.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8367 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/qgd_Z.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/qgd_python/gates/test/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3364 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_CH.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3409 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_CNOT.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3444 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_CZ.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3466 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_RX.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3348 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_RY.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3919 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_RZ.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3278 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_SX.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3676 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_U3.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3182 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_X.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3179 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_Y.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3232 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_Z.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6878 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/gates/test/test_gates.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/qgd_python/nn/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1304 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/nn/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/nn/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2387 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/nn/qgd_nn.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9635 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/nn/qgd_nn_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1573 2023-05-13 12:17:13.000000 squander-1.8.0/qgd_python/utils.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/random_unitary/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6628 2023-05-13 12:17:13.000000 squander-1.8.0/random_unitary/Random_Orthogonal.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11039 2023-05-13 12:17:13.000000 squander-1.8.0/random_unitary/Random_Unitary.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/random_unitary/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-13 12:17:13.000000 squander-1.8.0/random_unitary/include/Random_Orthogonal.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4476 2023-05-13 12:17:13.000000 squander-1.8.0/random_unitary/include/Random_Unitary.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       38 2023-05-13 12:18:39.478572 squander-1.8.0/setup.cfg
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1850 2023-05-13 12:17:13.000000 squander-1.8.0/setup.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/squander/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1442 2023-05-13 12:17:13.000000 squander-1.8.0/squander/__init__.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/squander.egg-info/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    17824 2023-05-13 12:18:39.000000 squander-1.8.0/squander.egg-info/PKG-INFO
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5051 2023-05-13 12:18:39.000000 squander-1.8.0/squander.egg-info/SOURCES.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        1 2023-05-13 12:18:39.000000 squander-1.8.0/squander.egg-info/dependency_links.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       50 2023-05-13 12:18:39.000000 squander-1.8.0/squander.egg-info/requires.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       20 2023-05-13 12:18:39.000000 squander-1.8.0/squander.egg-info/top_level.txt
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-13 12:18:39.478572 squander-1.8.0/test_standalone/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1996 2023-05-13 12:17:13.000000 squander-1.8.0/test_standalone/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6325 2023-05-13 12:17:13.000000 squander-1.8.0/test_standalone/custom_gate_structure_test.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4837 2023-05-13 12:17:13.000000 squander-1.8.0/test_standalone/decomposition_test.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14939 2023-05-15 09:25:56.000000 squander-1.8.1/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    35149 2023-05-15 09:25:56.000000 squander-1.8.1/LICENSE
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      121 2023-05-15 09:25:56.000000 squander-1.8.1/MANIFEST.in
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14953 2023-05-15 09:26:12.136824 squander-1.8.1/PKG-INFO
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14413 2023-05-15 09:25:56.000000 squander-1.8.1/README.md
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.116824 squander-1.8.1/cmake/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4306 2023-05-15 09:25:56.000000 squander-1.8.1/cmake/check_AVX.cmake
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.120824 squander-1.8.1/common/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6776 2023-05-15 09:25:56.000000 squander-1.8.1/common/Adam.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8316 2023-05-15 09:25:56.000000 squander-1.8.1/common/common.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-15 09:25:56.000000 squander-1.8.1/common/common_DFE.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5524 2023-05-15 09:25:56.000000 squander-1.8.1/common/config_element.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14292 2023-05-15 09:25:56.000000 squander-1.8.1/common/dot.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.120824 squander-1.8.1/common/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3441 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/Adam.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      216 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/Config.h.in
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2109 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/QGDTypes.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/common.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3026 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/common_DFE.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3423 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/config_element.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7626 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/dot.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9130 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/lbfgs.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2443 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/logging.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3812 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/matrix.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13485 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/matrix_base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3746 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/matrix_real.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1393 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/mpi_base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1468 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/numpy_interface.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9251 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/tolmin.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   156010 2023-05-15 09:25:56.000000 squander-1.8.1/common/lbfgs.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2515 2023-05-15 09:25:56.000000 squander-1.8.1/common/logging.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5065 2023-05-15 09:25:56.000000 squander-1.8.1/common/matrix.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4491 2023-05-15 09:25:56.000000 squander-1.8.1/common/matrix_real.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1095 2023-05-15 09:25:56.000000 squander-1.8.1/common/mpi_base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4808 2023-05-15 09:25:56.000000 squander-1.8.1/common/numpy_interface.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    58244 2023-05-15 09:25:56.000000 squander-1.8.1/common/tolmin.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.120824 squander-1.8.1/decomposition/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    57706 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    37081 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   100052 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16714 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    77317 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_adaptive.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    12741 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_custom.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23502 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/Sub_Matrix_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8536 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.124824 squander-1.8.1/decomposition/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16035 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7166 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15865 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5077 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8301 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_adaptive.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3393 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_custom.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6922 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3723 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.124824 squander-1.8.1/gates/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5728 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Adaptive.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4900 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CH.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4937 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CNOT.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5839 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CRY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4841 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7781 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Composite.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11545 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Gate.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   120998 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Gates_block.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8547 2023-05-15 09:25:56.000000 squander-1.8.1/gates/ON.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6819 2023-05-15 09:25:56.000000 squander-1.8.1/gates/RX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6815 2023-05-15 09:25:56.000000 squander-1.8.1/gates/RY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7110 2023-05-15 09:25:56.000000 squander-1.8.1/gates/RZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8697 2023-05-15 09:25:56.000000 squander-1.8.1/gates/SX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9587 2023-05-15 09:25:56.000000 squander-1.8.1/gates/SYC.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15472 2023-05-15 09:25:56.000000 squander-1.8.1/gates/U3.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8769 2023-05-15 09:25:56.000000 squander-1.8.1/gates/UN.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7950 2023-05-15 09:25:56.000000 squander-1.8.1/gates/X.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5671 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Y.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5672 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Z.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/gates/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3395 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Adaptive.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2428 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CH.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2504 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CNOT.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3113 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CRY.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2427 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CZ.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3594 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Composite.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5097 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Gate.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15824 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Gates_block.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/ON.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2812 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/RX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3088 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/RY.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2808 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/RZ.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2783 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/SX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2428 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/SYC.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6017 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/U3.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/UN.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2774 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/X.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2772 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Y.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2772 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Z.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/gates/kernels/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23561 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/apply_kernel_to_input_AVX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    32382 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/apply_kernel_to_state_vector_input.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/gates/kernels/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1786 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/include/apply_kernel_to_input_AVX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2099 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/include/apply_kernel_to_state_vector_input.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/nn/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    18464 2023-05-15 09:25:56.000000 squander-1.8.1/nn/NN.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/nn/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5274 2023-05-15 09:25:56.000000 squander-1.8.1/nn/include/NN.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/optimization_engines/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9698 2023-05-15 09:25:56.000000 squander-1.8.1/optimization_engines/RL_experience.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/optimization_engines/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3549 2023-05-15 09:25:56.000000 squander-1.8.1/optimization_engines/include/RL_experience.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      123 2023-05-15 09:25:56.000000 squander-1.8.1/pyproject.toml
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/qgd_python/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/__init__.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/qgd_python/decomposition/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4386 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7661 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    36730 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    24494 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    80626 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14278 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    41007 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3367 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.132824 squander-1.8.1/qgd_python/decomposition/test/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11024 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Compression.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Global_Phase.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7037 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_IBM.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1777 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Project_Name.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5616 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_QX2.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4399 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_State_Preparation.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1656 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Unitary.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4672 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_decomposition.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7190 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_fmo.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7018 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_heavy_hex.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5222 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_optmization_problem_combined.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4905 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_parametric_circuit.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.132824 squander-1.8.1/qgd_python/gates/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13547 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8219 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_CH.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8160 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_CNOT.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8033 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_CZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    28536 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_Gates_Block.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8529 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_RX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8528 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_RY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8527 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_RZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7771 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_SX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7801 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_SYC.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9054 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_U3.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7489 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_X.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8367 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_Y.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8367 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_Z.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/qgd_python/gates/test/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3364 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_CH.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3409 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_CNOT.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3444 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_CZ.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3466 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_RX.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3348 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_RY.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3919 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_RZ.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3278 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_SX.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3676 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_U3.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3182 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_X.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3179 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_Y.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3232 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_Z.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6878 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_gates.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/qgd_python/nn/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1304 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2387 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/qgd_nn.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9635 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/qgd_nn_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1573 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/utils.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/random_unitary/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6628 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/Random_Orthogonal.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11039 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/Random_Unitary.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/random_unitary/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/include/Random_Orthogonal.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4476 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/include/Random_Unitary.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       38 2023-05-15 09:26:12.136824 squander-1.8.1/setup.cfg
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1850 2023-05-15 09:25:56.000000 squander-1.8.1/setup.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/squander/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1442 2023-05-15 09:25:56.000000 squander-1.8.1/squander/__init__.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/squander.egg-info/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14953 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/PKG-INFO
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5133 2023-05-15 09:26:12.000000 squander-1.8.1/squander.egg-info/SOURCES.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        1 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/dependency_links.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       50 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/requires.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       20 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/top_level.txt
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/test_standalone/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1996 2023-05-15 09:25:56.000000 squander-1.8.1/test_standalone/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6325 2023-05-15 09:25:56.000000 squander-1.8.1/test_standalone/custom_gate_structure_test.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4837 2023-05-15 09:25:56.000000 squander-1.8.1/test_standalone/decomposition_test.cpp
```

### Comparing `squander-1.8.0/CMakeLists.txt` & `squander-1.8.1/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_minimum_required(VERSION 3.10.2)
 
 # CMAKE to create the shared library of the quantum gate decomposition project
 
 # set the project name and version
-project(CQGD VERSION 1.7)
+project(CQGD VERSION 1.8.1)
 
 # reuse compilation time linking for use runtime linking 
 SET(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
 
 # specify the C++ standard
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
@@ -221,60 +221,14 @@
   elseif (${HAVE_AVX_EXTENSIONS})
     list(APPEND CXX_FLAGS_RELEASE "/arch:AVX" "-DUSE_AVX")
   endif()
 
 endif()
 
 
-############################################################
-# checking GNU Scientific libraries and headers
-
-# adding GSL library dir if given
-if(DEFINED ENV{GSL_LIB_DIR})
-
-  find_library(GSL_LIB gsl 
-               PATHS $ENV{GSL_LIB_DIR} 
-               NO_DEFAULT_PATH
-               REQUIRED)
-else()
-
-  find_library(GSL_LIB gsl
-               PATHS ${PYTHON_SYS_PATH}
-               REQUIRED)
-
-endif()
-
-
-# adding GSL include dir
-if(DEFINED ENV{GSL_INC_DIR})
-
-  set(CMAKE_REQUIRED_FLAGS "-c")
-  check_include_file_cxx(gsl/gsl_multimin.h GSL_HEADER "-I$ENV{GSL_INC_DIR}")
-
-  if(NOT GSL_HEADER)
-    message(FATAL_ERROR "GSL header gsl_multimin.h not found")
-  endif()
-
-  message("-- Adding include directory $ENV{GSL_INC_DIR}")
-  list(APPEND EXTRA_INCLUDES "$ENV{GSL_INC_DIR}")
-
-else()
-
-  set(CMAKE_REQUIRED_FLAGS "-c")
-  check_include_file_cxx(gsl/gsl_multimin.h GSL_HEADER)
-  list(APPEND EXTRA_INCLUDES "${CMAKE_REQUIRED_INCLUDES}") 
-
-  if(NOT GSL_HEADER)
-    message(FATAL_ERROR "GSL header gsl_multimin.h not found")
-  endif()
-
-
-endif()
-
-
 
 
 ############################################################xx
 # checking TBB libraries and headers
 
 # adding TBB library dir if given by environment variable
 if(DEFINED ENV{TBB_LIB_DIR})
@@ -345,14 +299,16 @@
     ${PROJECT_SOURCE_DIR}/common/common.cpp
     ${PROJECT_SOURCE_DIR}/common/config_element.cpp
     ${PROJECT_SOURCE_DIR}/common/dot.cpp
     ${PROJECT_SOURCE_DIR}/common/matrix.cpp
     ${PROJECT_SOURCE_DIR}/common/matrix_real.cpp
     ${PROJECT_SOURCE_DIR}/common/logging.cpp
     ${PROJECT_SOURCE_DIR}/common/Adam.cpp
+    ${PROJECT_SOURCE_DIR}/common/tolmin.cpp
+    ${PROJECT_SOURCE_DIR}/common/lbfgs.cpp
     ${PROJECT_SOURCE_DIR}/optimization_engines/RL_experience.cpp
     ${PROJECT_SOURCE_DIR}/gates/CNOT.cpp
     ${PROJECT_SOURCE_DIR}/gates/SYC.cpp
     ${PROJECT_SOURCE_DIR}/gates/CZ.cpp
     ${PROJECT_SOURCE_DIR}/gates/CH.cpp
     ${PROJECT_SOURCE_DIR}/gates/Gate.cpp
     ${PROJECT_SOURCE_DIR}/gates/UN.cpp
@@ -422,15 +378,14 @@
 target_link_libraries( qgd PRIVATE
     ${BLAS_LIBRARIES}
     ${LAPACK_LIBRARIES}
     ${LAPACKE_LIBRARIES}
     ${TBBMALLOC_LIB}
     ${TBBMALLOC_PROXY_LIB}
     ${TBB_LIB}
-    ${GSL_LIB}
     ${MPI_C_LIBRARIES}
     )
 
 
 target_include_directories(qgd PRIVATE
                             .
                             ./common/include
```

### Comparing `squander-1.8.0/LICENSE` & `squander-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/PKG-INFO` & `squander-1.8.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: squander
-Version: 1.8.0
-Summary: The C++ binding for the SQUANDER package
-Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
-Maintainer: Peter Rakyta
-Maintainer-email: peter.rakyta@ttk.elte.hu
-License: GNU General Public License v3.0
-Keywords: test,cmake,extension
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: C
-Classifier: Programming Language :: C++
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)](https://doi.org/10.5281/zenodo.4508680)
  <a href="https://trackgit.com">
 <img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/l0sfey1m19at85951dwl" alt="trackgit-views" />
 </a>
 
 # Sequential Quantum Gate Decomposer (SQUANDER)
 
@@ -48,20 +32,17 @@
 * Zoltán Zimborás (researcher): zimboras.zoltan@wigner.hu
 * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
 
 
 
 ### Dependencies
 
-The optimization algorithm of SQUANDER relies on the [multimin](https://www.gnu.org/software/gsl/doc/html/multimin.html) component of the [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/index.html). 
-We developed and tested the SQUANDER package with GNU Scientific Library of version 2.5, 2.6 and 2.7.
 The dependencies necessary to compile and build the SQUANDER package are the followings:
 
 * [CMake](https://cmake.org/) (>=3.10.2)
-* [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/index.html) (>=2.5, shipped with the gsl python package)
 * C++/C [Intel](https://software.intel.com/content/www/us/en/develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler
 * [TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel Python package)
 * [Intel MKL](https://software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html) (optional)
 * [OpenBlas](https://www.openblas.net/) (optional, recommended)
 * [LAPACKE](https://www.netlib.org/lapack/lapacke.html)
 * [Doxygen](https://www.doxygen.nl/index.html) (optional)
 
@@ -69,78 +50,36 @@
 The SQUANDER Python interface needs the following packages to be installed on the system:
 
 * [Qiskit](https://qiskit.org/documentation/install.html)
 * [Numpy](https://numpy.org/install/)
 * [scipy](https://www.scipy.org/install.html)
 * [scikit-build](https://scikit-build.readthedocs.io/en/latest/)
 * [tbb-devel](https://pypi.org/project/tbb-devel/) (containing the TBB Library)
-* [gsl](https://anaconda.org/conda-forge/gsl) (containing the GNU Scientific Library)
-
-
-
-
-### How to obtain GNU Scientific Library
-
-In order to build and use the SQUANDER we recommend the Anaconda virtual python environment providing all the required dependencies for SQUANDER.
-One can easily install the GNU Scientific Library for local users by the command
-
-$ conda install -c conda-forge gsl
-
-Alternatively, a python binding project alongside the GNU GSL library is accessible via pypi repository:
-
-$ pip install numpy swig
 
-$ pip install pygsl
 
-Here we describe an alternative way to deploy GNU Scientific Library from source by the end user without administrative privileges. 
-The GNU Scientific Library can be downloaded from the site [https://www.gnu.org/software/gsl/](https://www.gnu.org/software/gsl/).
-After the downloaded package is extracted somewhere in the home directory of the user (**path/to/gsl/source**), one should configure the building environment using the **configure** tool.
-Depending on the individual settings the default compiler to be invoked might be different from HPC to HPC. 
-To ensure the usage of the GNU compiler, the following shell command should be executed inside the directory **path/to/gsl/source**:
 
-$ ./configure --prefix=path/to/gsl FC=gfortran CC=gcc CXX=g++
-
-(Similarly, Intel compiler can be forced by setting FC=ifort CC=icc and CXX=icpc.)
-The installation directory of the compiled GNU Scientific Library is given by **--prefix=path/to/gsl** (which is different from the directory path of 
-the source files given by **path/to/gslsource**).
-To install GNU Scientific Library the user should have read and write permissions on the path **path/to/gsl** (which might be for example /home/username/gsl).
-After the successful configuration the GNU Scientific Library can be compiled by the shell command
-
-$ make
-
-The compilation of the GNU Scientific Library takes some time. When the compilation is done, the package (including the C header files and the static and shared libraries) is installed into the directory **path/to/gsl** by the shell command:
-
-$ make install
 
 ### Install SQUANDER from Python Package Index (PyPI)
 
 Since version 1.7.1 the SQUANDER package is accessible at Python Package Index (PyPI). The package can be installed on linux systems following the steps outlined below:
 
 $ pip install numpy swig tbb-devel wheel scikit-build ninja qiskit
 
-$ pip install pygsl
-
 $ pip install squander
 
 
 
 ### Download the SQUANDER package
 
 The developer version of the Quantum Gate Decomposer package can be downloaded from github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/tree/master).
 After the package is downloaded into the directory **path/to/SQUANDER/package** (which would be the path to the source code of the SQUANDER package), one can proceed to the compilation steps described in the next section.
 
 ### How to build the SQUANDER package
 
 The SQUANDER package is equipped with a Python build script and CMake tools to ease the compilation and the deployment of the package.
-To ensure that SQUANDER package would find the necessary libraries and header files during compilation time it is advised to define the following environment variables:
-
-$ export GSL_LIB_DIR=path/to/gsl/lib(64)
-
-$ export GSL_INC_DIR=path/to/gsl/include
-
 The SQUANDER package is parallelized via Threading Building Block (TBB) libraries. If TBB is not present in the system, it can be easily installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
 Alternatively the TBB libraries can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB)   and built from source. 
 In this case one should supply the necessary environment variables pointing to the header and library files of the TBB package. For newer
 Intel compilers the TBB package is part of the Intel compiler package, similarly to the MKL package. If the TBB library is located at non-standrad path or the SQUANDER package is compiled with GNU compiler, then setting the
 
 $ export TBB_LIB_DIR=path/to/TBB/lib(64)
 
@@ -167,16 +106,14 @@
 
 $ conda activate qgd
 
 Install dependencies:
 
 $ conda install numpy scipy pip pytest scikit-build tbb-devel
 
-$ conda install -c conda-forge gsl
-
 $ pip install qiskit matplotlib 
 
 After the basic environment variables are set and the dependencies are installed, the compilation of the package can be started by the Python command:
 
 $ python3 setup.py build_ext
 
 The command above starts the compilation of the SQUANDER C++ library and builds the necessary C++ Python interface extensions of the SQUANDER package in place.
```

#### html2text {}

```diff
@@ -1,185 +1,141 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.0 Summary: The C++ binding
-for the SQUANDER package Home-page: https://github.com/rakytap/sequential-
-quantum-gate-decomposer Maintainer: Peter Rakyta Maintainer-email:
-peter.rakyta@ttk.elte.hu License: GNU General Public License v3.0 Keywords:
-test,cmake,extension Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: Programming Language :: C Classifier:
-Programming Language :: C++ Description-Content-Type: text/markdown License-
-File: LICENSE [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)]
-(https://doi.org/10.5281/zenodo.4508680) [trackgit-views] # Sequential Quantum
-Gate Decomposer (SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER)
-package provides a novel solution to decompose any n-qubit unitaries into a
-sequence of one-qubit rotations and two-qubit controlled gates (such as
-controlled NOT or controlled phase gate). SQUANDER utilizes two novel gate
-synthesis techniques reported in Refereces [1] and [2]. (i) To synthesize
-general unitaries SQUANDER applies periodic layers of two-qubit and parametric
-one-qubit gates to an n-qubit unitary such that the resulting unitary is 1-
-qubit decoupled, i.e., is a tensor product of an (n-1)-qubit and a 1-qubit
-unitary. Continuing the decoupling procedure sequentially one arrives at the
-end to a full decomposition of the original unitary into 1- and 2-qubit gates.
-SQUANDER provides lower CNOT counts for generic n-qubit unitaries (up to n=6)
-than the previously provided lower bounds. (ii) An adaptive circuit compression
-is used to optimize quantum circuit by the application of parametric two-qubit
-gates in the synthesis process. The utilization of these parametric two-qubit
-gates in the circuit design allows one to transform the discrete combinatorial
-problem of circuit synthesis into an optimization problem over continuous
-variables. The circuit is then compressed by a sequential removal of two-qubit
-gates from the design, while the remaining building blocks are continuously
-adapted to the reduced gate structure by iterated learning cycles. The SQUANDER
-library is written in C/C++ providing a Python interface via [C++ extensions]
-(https://docs.python.org/3/library/ctypes.html). The present package is
-supplied with Python building script and CMake tools to ease its deployment.
-The SQUANDER package can be built with both Intel and GNU compilers, and can be
-link against various CBLAS libraries installed on the system. (So far the CLBAS
-libraries of the GNU Scientific Library, OpenBLAS and the Intel MKL packages
-were tested.) In the following we briefly summarize the steps to build, install
-and use the SQUANDER package. The project was supported by grant OTKA PD123927
-and by the Ministry of Innovation and Technology and the National Research,
-Development and Innovation Office within the Quantum Information National
-Laboratory of Hungary. Find the documantation of the SQUANDER package at
-[CodeDocs[xyz]](https://codedocs.xyz/rakytap/sequential-quantum-gate-
-decomposer/) ### Contact Us Have a question about the SQUANDER package? Don't
-hesitate to contact us at the following e-mails: * ZoltÃ¡n ZimborÃ¡s
-(researcher): zimboras.zoltan@wigner.hu * Peter Rakyta (developer):
-peter.rakyta@ttk.elte.hu ### Dependencies The optimization algorithm of
-SQUANDER relies on the [multimin](https://www.gnu.org/software/gsl/doc/html/
-multimin.html) component of the [GNU Scientific Library](https://www.gnu.org/
-software/gsl/doc/html/index.html). We developed and tested the SQUANDER package
-with GNU Scientific Library of version 2.5, 2.6 and 2.7. The dependencies
-necessary to compile and build the SQUANDER package are the followings: *
-[CMake](https://cmake.org/) (>=3.10.2) * [GNU Scientific Library](https://
-www.gnu.org/software/gsl/doc/html/index.html) (>=2.5, shipped with the gsl
-python package) * C++/C [Intel](https://software.intel.com/content/www/us/en/
-develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://
-gcc.gnu.org/) (>=v4.8.1) compiler * [TBB](https://github.com/oneapi-src/oneTBB)
-library (shipped with tbb-devel Python package) * [Intel MKL](https://
-software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html)
-(optional) * [OpenBlas](https://www.openblas.net/) (optional, recommended) *
-[LAPACKE](https://www.netlib.org/lapack/lapacke.html) * [Doxygen](https://
-www.doxygen.nl/index.html) (optional) The Python interface of SQUANDER was
-developed and tested with Python 3.6-3.9. The SQUANDER Python interface needs
-the following packages to be installed on the system: * [Qiskit](https://
-qiskit.org/documentation/install.html) * [Numpy](https://numpy.org/install/) *
-[scipy](https://www.scipy.org/install.html) * [scikit-build](https://scikit-
-build.readthedocs.io/en/latest/) * [tbb-devel](https://pypi.org/project/tbb-
-devel/) (containing the TBB Library) * [gsl](https://anaconda.org/conda-forge/
-gsl) (containing the GNU Scientific Library) ### How to obtain GNU Scientific
-Library In order to build and use the SQUANDER we recommend the Anaconda
-virtual python environment providing all the required dependencies for
-SQUANDER. One can easily install the GNU Scientific Library for local users by
-the command $ conda install -c conda-forge gsl Alternatively, a python binding
-project alongside the GNU GSL library is accessible via pypi repository: $ pip
-install numpy swig $ pip install pygsl Here we describe an alternative way to
-deploy GNU Scientific Library from source by the end user without
-administrative privileges. The GNU Scientific Library can be downloaded from
-the site [https://www.gnu.org/software/gsl/](https://www.gnu.org/software/gsl/
-). After the downloaded package is extracted somewhere in the home directory of
-the user (**path/to/gsl/source**), one should configure the building
-environment using the **configure** tool. Depending on the individual settings
-the default compiler to be invoked might be different from HPC to HPC. To
-ensure the usage of the GNU compiler, the following shell command should be
-executed inside the directory **path/to/gsl/source**: $ ./configure --
-prefix=path/to/gsl FC=gfortran CC=gcc CXX=g++ (Similarly, Intel compiler can be
-forced by setting FC=ifort CC=icc and CXX=icpc.) The installation directory of
-the compiled GNU Scientific Library is given by **--prefix=path/to/gsl** (which
-is different from the directory path of the source files given by **path/to/
-gslsource**). To install GNU Scientific Library the user should have read and
-write permissions on the path **path/to/gsl** (which might be for example /
-home/username/gsl). After the successful configuration the GNU Scientific
-Library can be compiled by the shell command $ make The compilation of the GNU
-Scientific Library takes some time. When the compilation is done, the package
-(including the C header files and the static and shared libraries) is installed
-into the directory **path/to/gsl** by the shell command: $ make install ###
-Install SQUANDER from Python Package Index (PyPI) Since version 1.7.1 the
-SQUANDER package is accessible at Python Package Index (PyPI). The package can
-be installed on linux systems following the steps outlined below: $ pip install
-numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install pygsl $ pip
-install squander ### Download the SQUANDER package The developer version of the
-Quantum Gate Decomposer package can be downloaded from github repository
-[https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://
-github.com/rakytap/quantum-gate-decomposer/tree/master). After the package is
-downloaded into the directory **path/to/SQUANDER/package** (which would be the
-path to the source code of the SQUANDER package), one can proceed to the
-compilation steps described in the next section. ### How to build the SQUANDER
-package The SQUANDER package is equipped with a Python build script and CMake
-tools to ease the compilation and the deployment of the package. To ensure that
-SQUANDER package would find the necessary libraries and header files during
-compilation time it is advised to define the following environment variables: $
-export GSL_LIB_DIR=path/to/gsl/lib(64) $ export GSL_INC_DIR=path/to/gsl/include
-The SQUANDER package is parallelized via Threading Building Block (TBB)
-libraries. If TBB is not present in the system, it can be easily installed via
-python package [tbb-devel](https://pypi.org/project/tbb-devel/). Alternatively
-the TBB libraries can be installed via apt or yum utility (sudo apt install
-libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB]
-(https://github.com/oneapi-src/oneTBB) and built from source. In this case one
-should supply the necessary environment variables pointing to the header and
-library files of the TBB package. For newer Intel compilers the TBB package is
-part of the Intel compiler package, similarly to the MKL package. If the TBB
-library is located at non-standrad path or the SQUANDER package is compiled
-with GNU compiler, then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $
-export TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)](https://
+doi.org/10.5281/zenodo.4508680) [trackgit-views] # Sequential Quantum Gate
+Decomposer (SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER) package
+provides a novel solution to decompose any n-qubit unitaries into a sequence of
+one-qubit rotations and two-qubit controlled gates (such as controlled NOT or
+controlled phase gate). SQUANDER utilizes two novel gate synthesis techniques
+reported in Refereces [1] and [2]. (i) To synthesize general unitaries SQUANDER
+applies periodic layers of two-qubit and parametric one-qubit gates to an n-
+qubit unitary such that the resulting unitary is 1-qubit decoupled, i.e., is a
+tensor product of an (n-1)-qubit and a 1-qubit unitary. Continuing the
+decoupling procedure sequentially one arrives at the end to a full
+decomposition of the original unitary into 1- and 2-qubit gates. SQUANDER
+provides lower CNOT counts for generic n-qubit unitaries (up to n=6) than the
+previously provided lower bounds. (ii) An adaptive circuit compression is used
+to optimize quantum circuit by the application of parametric two-qubit gates in
+the synthesis process. The utilization of these parametric two-qubit gates in
+the circuit design allows one to transform the discrete combinatorial problem
+of circuit synthesis into an optimization problem over continuous variables.
+The circuit is then compressed by a sequential removal of two-qubit gates from
+the design, while the remaining building blocks are continuously adapted to the
+reduced gate structure by iterated learning cycles. The SQUANDER library is
+written in C/C++ providing a Python interface via [C++ extensions](https://
+docs.python.org/3/library/ctypes.html). The present package is supplied with
+Python building script and CMake tools to ease its deployment. The SQUANDER
+package can be built with both Intel and GNU compilers, and can be link against
+various CBLAS libraries installed on the system. (So far the CLBAS libraries of
+the GNU Scientific Library, OpenBLAS and the Intel MKL packages were tested.)
+In the following we briefly summarize the steps to build, install and use the
+SQUANDER package. The project was supported by grant OTKA PD123927 and by the
+Ministry of Innovation and Technology and the National Research, Development
+and Innovation Office within the Quantum Information National Laboratory of
+Hungary. Find the documantation of the SQUANDER package at [CodeDocs[xyz]]
+(https://codedocs.xyz/rakytap/sequential-quantum-gate-decomposer/) ### Contact
+Us Have a question about the SQUANDER package? Don't hesitate to contact us at
+the following e-mails: * ZoltÃ¡n ZimborÃ¡s (researcher):
+zimboras.zoltan@wigner.hu * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
+### Dependencies The dependencies necessary to compile and build the SQUANDER
+package are the followings: * [CMake](https://cmake.org/) (>=3.10.2) * C++/C
+[Intel](https://software.intel.com/content/www/us/en/develop/tools/compilers/c-
+compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler *
+[TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel
+Python package) * [Intel MKL](https://software.intel.com/content/www/us/en/
+develop/tools/math-kernel-library.html) (optional) * [OpenBlas](https://
+www.openblas.net/) (optional, recommended) * [LAPACKE](https://www.netlib.org/
+lapack/lapacke.html) * [Doxygen](https://www.doxygen.nl/index.html) (optional)
+The Python interface of SQUANDER was developed and tested with Python 3.6-3.9.
+The SQUANDER Python interface needs the following packages to be installed on
+the system: * [Qiskit](https://qiskit.org/documentation/install.html) * [Numpy]
+(https://numpy.org/install/) * [scipy](https://www.scipy.org/install.html) *
+[scikit-build](https://scikit-build.readthedocs.io/en/latest/) * [tbb-devel]
+(https://pypi.org/project/tbb-devel/) (containing the TBB Library) ### Install
+SQUANDER from Python Package Index (PyPI) Since version 1.7.1 the SQUANDER
+package is accessible at Python Package Index (PyPI). The package can be
+installed on linux systems following the steps outlined below: $ pip install
+numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install squander ###
+Download the SQUANDER package The developer version of the Quantum Gate
+Decomposer package can be downloaded from github repository [https://
+github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/
+rakytap/quantum-gate-decomposer/tree/master). After the package is downloaded
+into the directory **path/to/SQUANDER/package** (which would be the path to the
+source code of the SQUANDER package), one can proceed to the compilation steps
+described in the next section. ### How to build the SQUANDER package The
+SQUANDER package is equipped with a Python build script and CMake tools to ease
+the compilation and the deployment of the package. The SQUANDER package is
+parallelized via Threading Building Block (TBB) libraries. If TBB is not
+present in the system, it can be easily installed via python package [tbb-
+devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
+can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
+be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
+oneapi-src/oneTBB) and built from source. In this case one should supply the
+necessary environment variables pointing to the header and library files of the
+TBB package. For newer Intel compilers the TBB package is part of the Intel
+compiler package, similarly to the MKL package. If the TBB library is located
+at non-standrad path or the SQUANDER package is compiled with GNU compiler,
+then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
+TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
 SQUANDER package by making the appropriate CMake calls. ### Developer build We
 recommend to install the SQUANDER package in the Anaconda environment. In order
 to install the necessary requirements, follow the steps below: Creating new
 python environment: $ conda create -n qgd Activate the new anaconda environment
 $ conda activate qgd Install dependencies: $ conda install numpy scipy pip
-pytest scikit-build tbb-devel $ conda install -c conda-forge gsl $ pip install
-qiskit matplotlib After the basic environment variables are set and the
-dependencies are installed, the compilation of the package can be started by
-the Python command: $ python3 setup.py build_ext The command above starts the
-compilation of the SQUANDER C++ library and builds the necessary C++ Python
-interface extensions of the SQUANDER package in place. After a successful
-build, one can register the SQUANDER package in the Python distribution in
-developer (i.e. editable) mode by command: $ python -m pip install -e . ###
-Binary distribution After the environment variables are set it is possible to
-build wheel binaries of the SQUANDER package. In order to launch the
-compilation process from python, **[scikit-build](https://scikit-
-build.readthedocs.io/en/latest/)** package is necessary. (It is optional to
-install the ninja package which speeds up the building process by parallel
-compilation.) The binary wheel can be constructed by command $ python3 setup.py
-bdist_wheel in the root directory of the SQUADER package. The created SQUANDER
-wheel can be installed on the local machine by issuing the command from the
-directory **path/to/SQUANDER/package/dist** $ pip3 install qgd-*.whl We notice,
-that the created wheel is not portable, since it contains hard coded link to
-external libraries (TBB and CBLAS). ### Source distribution A portable source
-distribution of the SQUANDER package can be created by a command launched from
-the root directory of the SQUANDER package: $ python3 setup.py sdist In order
-to create a source distribution it is not necessary to set the environment
-variables, since this script only collects the necessary files and pack them
-into a tar ball located in the directory **path/to/SQUANDER/package/dist**. In
-order to install the SQUANDER package from source tar ball, see the previous
-section discussing the initialization of the environment variables. The package
-can be compiled and installed by the command $ pip3 install qgd-*.tar.gz issued
-from directory **path/to/SQUANDER/package/dist** (It is optional to install the
-ninja package which speeds up the building process by parallel compilation.)
-### How to use The algorithm implemented in the SQUANDER package intends to
-transform the given unitary into an identity matrix via a sequence of two-qubit
-and one-qubit gate operations applied on the unitary. Thus, in order to get the
-decomposition of a unitary, one should rather provide the complex transpose of
-this unitary as the input for the SQUANDER decomposing process, as can be seen
-in the examples. ## Python Interface The SQUANDER package contains a Python
-interface allowing the access of the functionalities of the SQUANDER package
-from Python. The usage of the SQUANDER Python interface is demonstrated in the
-example files in the directory **examples** located in the directory **path/to/
-SQUANDER/package**, or in test files located in sub-directories of **path/to/
-SQUANDER/package/qgd_python/*/test**. ### Example code snippet Here we provide
-an example to use the SQUANDER package. The following python interface is
-accessible from version 1.8.0. In this example we use two optimization engines
-for the decomposition: 1. An evolutionary engine called AGENTS 2. Second order
-gradient descend algorithm (BFGS) Firstly we construct a Python map to set
-hyper-parameters during the gate synthesis. #Python map containing hyper-
-parameters config = { 'max_outer_iterations': 1, 'max_inner_iterations_agent':
-25000, 'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
+pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+environment variables are set and the dependencies are installed, the
+compilation of the package can be started by the Python command: $ python3
+setup.py build_ext The command above starts the compilation of the SQUANDER C++
+library and builds the necessary C++ Python interface extensions of the
+SQUANDER package in place. After a successful build, one can register the
+SQUANDER package in the Python distribution in developer (i.e. editable) mode
+by command: $ python -m pip install -e . ### Binary distribution After the
+environment variables are set it is possible to build wheel binaries of the
+SQUANDER package. In order to launch the compilation process from python, **
+[scikit-build](https://scikit-build.readthedocs.io/en/latest/)** package is
+necessary. (It is optional to install the ninja package which speeds up the
+building process by parallel compilation.) The binary wheel can be constructed
+by command $ python3 setup.py bdist_wheel in the root directory of the SQUADER
+package. The created SQUANDER wheel can be installed on the local machine by
+issuing the command from the directory **path/to/SQUANDER/package/dist** $ pip3
+install qgd-*.whl We notice, that the created wheel is not portable, since it
+contains hard coded link to external libraries (TBB and CBLAS). ### Source
+distribution A portable source distribution of the SQUANDER package can be
+created by a command launched from the root directory of the SQUANDER package:
+$ python3 setup.py sdist In order to create a source distribution it is not
+necessary to set the environment variables, since this script only collects the
+necessary files and pack them into a tar ball located in the directory **path/
+to/SQUANDER/package/dist**. In order to install the SQUANDER package from
+source tar ball, see the previous section discussing the initialization of the
+environment variables. The package can be compiled and installed by the command
+$ pip3 install qgd-*.tar.gz issued from directory **path/to/SQUANDER/package/
+dist** (It is optional to install the ninja package which speeds up the
+building process by parallel compilation.) ### How to use The algorithm
+implemented in the SQUANDER package intends to transform the given unitary into
+an identity matrix via a sequence of two-qubit and one-qubit gate operations
+applied on the unitary. Thus, in order to get the decomposition of a unitary,
+one should rather provide the complex transpose of this unitary as the input
+for the SQUANDER decomposing process, as can be seen in the examples. ## Python
+Interface The SQUANDER package contains a Python interface allowing the access
+of the functionalities of the SQUANDER package from Python. The usage of the
+SQUANDER Python interface is demonstrated in the example files in the directory
+**examples** located in the directory **path/to/SQUANDER/package**, or in test
+files located in sub-directories of **path/to/SQUANDER/package/qgd_python/*/
+test**. ### Example code snippet Here we provide an example to use the SQUANDER
+package. The following python interface is accessible from version 1.8.0. In
+this example we use two optimization engines for the decomposition: 1. An
+evolutionary engine called AGENTS 2. Second order gradient descend algorithm
+(BFGS) Firstly we construct a Python map to set hyper-parameters during the
+gate synthesis. #Python map containing hyper-parameters config =
+{ 'max_outer_iterations': 1, 'max_inner_iterations_agent': 25000,
+'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
 'max_inner_iterations_final': 5000, 'Randomized_Radius': 0.3,
 'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-4,
 'optimization_tolerance': 1e-8, 'agent_num': 10} Next we initialize the
 decomposition class with the unitary Umtx to be decomposed. # creating a class
 to decompose the unitary from squander import N_Qubit_Decomposition_adaptive
 cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config ) The
 verbosity of the execution output can be controlled by the function call #
```

### Comparing `squander-1.8.0/README.md` & `squander-1.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: squander
+Version: 1.8.1
+Summary: The C++ binding for the SQUANDER package
+Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
+Maintainer: Peter Rakyta
+Maintainer-email: peter.rakyta@ttk.elte.hu
+License: GNU General Public License v3.0
+Keywords: test,cmake,extension
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)](https://doi.org/10.5281/zenodo.4508680)
  <a href="https://trackgit.com">
 <img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/l0sfey1m19at85951dwl" alt="trackgit-views" />
 </a>
 
 # Sequential Quantum Gate Decomposer (SQUANDER)
 
@@ -32,20 +48,17 @@
 * Zoltán Zimborás (researcher): zimboras.zoltan@wigner.hu
 * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
 
 
 
 ### Dependencies
 
-The optimization algorithm of SQUANDER relies on the [multimin](https://www.gnu.org/software/gsl/doc/html/multimin.html) component of the [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/index.html). 
-We developed and tested the SQUANDER package with GNU Scientific Library of version 2.5, 2.6 and 2.7.
 The dependencies necessary to compile and build the SQUANDER package are the followings:
 
 * [CMake](https://cmake.org/) (>=3.10.2)
-* [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/index.html) (>=2.5, shipped with the gsl python package)
 * C++/C [Intel](https://software.intel.com/content/www/us/en/develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler
 * [TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel Python package)
 * [Intel MKL](https://software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html) (optional)
 * [OpenBlas](https://www.openblas.net/) (optional, recommended)
 * [LAPACKE](https://www.netlib.org/lapack/lapacke.html)
 * [Doxygen](https://www.doxygen.nl/index.html) (optional)
 
@@ -53,78 +66,36 @@
 The SQUANDER Python interface needs the following packages to be installed on the system:
 
 * [Qiskit](https://qiskit.org/documentation/install.html)
 * [Numpy](https://numpy.org/install/)
 * [scipy](https://www.scipy.org/install.html)
 * [scikit-build](https://scikit-build.readthedocs.io/en/latest/)
 * [tbb-devel](https://pypi.org/project/tbb-devel/) (containing the TBB Library)
-* [gsl](https://anaconda.org/conda-forge/gsl) (containing the GNU Scientific Library)
-
-
-
-
-### How to obtain GNU Scientific Library
-
-In order to build and use the SQUANDER we recommend the Anaconda virtual python environment providing all the required dependencies for SQUANDER.
-One can easily install the GNU Scientific Library for local users by the command
-
-$ conda install -c conda-forge gsl
-
-Alternatively, a python binding project alongside the GNU GSL library is accessible via pypi repository:
-
-$ pip install numpy swig
 
-$ pip install pygsl
 
-Here we describe an alternative way to deploy GNU Scientific Library from source by the end user without administrative privileges. 
-The GNU Scientific Library can be downloaded from the site [https://www.gnu.org/software/gsl/](https://www.gnu.org/software/gsl/).
-After the downloaded package is extracted somewhere in the home directory of the user (**path/to/gsl/source**), one should configure the building environment using the **configure** tool.
-Depending on the individual settings the default compiler to be invoked might be different from HPC to HPC. 
-To ensure the usage of the GNU compiler, the following shell command should be executed inside the directory **path/to/gsl/source**:
 
-$ ./configure --prefix=path/to/gsl FC=gfortran CC=gcc CXX=g++
-
-(Similarly, Intel compiler can be forced by setting FC=ifort CC=icc and CXX=icpc.)
-The installation directory of the compiled GNU Scientific Library is given by **--prefix=path/to/gsl** (which is different from the directory path of 
-the source files given by **path/to/gslsource**).
-To install GNU Scientific Library the user should have read and write permissions on the path **path/to/gsl** (which might be for example /home/username/gsl).
-After the successful configuration the GNU Scientific Library can be compiled by the shell command
-
-$ make
-
-The compilation of the GNU Scientific Library takes some time. When the compilation is done, the package (including the C header files and the static and shared libraries) is installed into the directory **path/to/gsl** by the shell command:
-
-$ make install
 
 ### Install SQUANDER from Python Package Index (PyPI)
 
 Since version 1.7.1 the SQUANDER package is accessible at Python Package Index (PyPI). The package can be installed on linux systems following the steps outlined below:
 
 $ pip install numpy swig tbb-devel wheel scikit-build ninja qiskit
 
-$ pip install pygsl
-
 $ pip install squander
 
 
 
 ### Download the SQUANDER package
 
 The developer version of the Quantum Gate Decomposer package can be downloaded from github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/tree/master).
 After the package is downloaded into the directory **path/to/SQUANDER/package** (which would be the path to the source code of the SQUANDER package), one can proceed to the compilation steps described in the next section.
 
 ### How to build the SQUANDER package
 
 The SQUANDER package is equipped with a Python build script and CMake tools to ease the compilation and the deployment of the package.
-To ensure that SQUANDER package would find the necessary libraries and header files during compilation time it is advised to define the following environment variables:
-
-$ export GSL_LIB_DIR=path/to/gsl/lib(64)
-
-$ export GSL_INC_DIR=path/to/gsl/include
-
 The SQUANDER package is parallelized via Threading Building Block (TBB) libraries. If TBB is not present in the system, it can be easily installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
 Alternatively the TBB libraries can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB)   and built from source. 
 In this case one should supply the necessary environment variables pointing to the header and library files of the TBB package. For newer
 Intel compilers the TBB package is part of the Intel compiler package, similarly to the MKL package. If the TBB library is located at non-standrad path or the SQUANDER package is compiled with GNU compiler, then setting the
 
 $ export TBB_LIB_DIR=path/to/TBB/lib(64)
 
@@ -151,16 +122,14 @@
 
 $ conda activate qgd
 
 Install dependencies:
 
 $ conda install numpy scipy pip pytest scikit-build tbb-devel
 
-$ conda install -c conda-forge gsl
-
 $ pip install qiskit matplotlib 
 
 After the basic environment variables are set and the dependencies are installed, the compilation of the package can be started by the Python command:
 
 $ python3 setup.py build_ext
 
 The command above starts the compilation of the SQUANDER C++ library and builds the necessary C++ Python interface extensions of the SQUANDER package in place.
```

#### html2text {}

```diff
@@ -1,178 +1,149 @@
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)](https://
-doi.org/10.5281/zenodo.4508680) [trackgit-views] # Sequential Quantum Gate
-Decomposer (SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER) package
-provides a novel solution to decompose any n-qubit unitaries into a sequence of
-one-qubit rotations and two-qubit controlled gates (such as controlled NOT or
-controlled phase gate). SQUANDER utilizes two novel gate synthesis techniques
-reported in Refereces [1] and [2]. (i) To synthesize general unitaries SQUANDER
-applies periodic layers of two-qubit and parametric one-qubit gates to an n-
-qubit unitary such that the resulting unitary is 1-qubit decoupled, i.e., is a
-tensor product of an (n-1)-qubit and a 1-qubit unitary. Continuing the
-decoupling procedure sequentially one arrives at the end to a full
-decomposition of the original unitary into 1- and 2-qubit gates. SQUANDER
-provides lower CNOT counts for generic n-qubit unitaries (up to n=6) than the
-previously provided lower bounds. (ii) An adaptive circuit compression is used
-to optimize quantum circuit by the application of parametric two-qubit gates in
-the synthesis process. The utilization of these parametric two-qubit gates in
-the circuit design allows one to transform the discrete combinatorial problem
-of circuit synthesis into an optimization problem over continuous variables.
-The circuit is then compressed by a sequential removal of two-qubit gates from
-the design, while the remaining building blocks are continuously adapted to the
-reduced gate structure by iterated learning cycles. The SQUANDER library is
-written in C/C++ providing a Python interface via [C++ extensions](https://
-docs.python.org/3/library/ctypes.html). The present package is supplied with
-Python building script and CMake tools to ease its deployment. The SQUANDER
-package can be built with both Intel and GNU compilers, and can be link against
-various CBLAS libraries installed on the system. (So far the CLBAS libraries of
-the GNU Scientific Library, OpenBLAS and the Intel MKL packages were tested.)
-In the following we briefly summarize the steps to build, install and use the
-SQUANDER package. The project was supported by grant OTKA PD123927 and by the
-Ministry of Innovation and Technology and the National Research, Development
-and Innovation Office within the Quantum Information National Laboratory of
-Hungary. Find the documantation of the SQUANDER package at [CodeDocs[xyz]]
-(https://codedocs.xyz/rakytap/sequential-quantum-gate-decomposer/) ### Contact
-Us Have a question about the SQUANDER package? Don't hesitate to contact us at
-the following e-mails: * ZoltÃ¡n ZimborÃ¡s (researcher):
-zimboras.zoltan@wigner.hu * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
-### Dependencies The optimization algorithm of SQUANDER relies on the
-[multimin](https://www.gnu.org/software/gsl/doc/html/multimin.html) component
-of the [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/
-index.html). We developed and tested the SQUANDER package with GNU Scientific
-Library of version 2.5, 2.6 and 2.7. The dependencies necessary to compile and
-build the SQUANDER package are the followings: * [CMake](https://cmake.org/)
-(>=3.10.2) * [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/
-html/index.html) (>=2.5, shipped with the gsl python package) * C++/C [Intel]
-(https://software.intel.com/content/www/us/en/develop/tools/compilers/c-
-compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler *
-[TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel
-Python package) * [Intel MKL](https://software.intel.com/content/www/us/en/
-develop/tools/math-kernel-library.html) (optional) * [OpenBlas](https://
-www.openblas.net/) (optional, recommended) * [LAPACKE](https://www.netlib.org/
-lapack/lapacke.html) * [Doxygen](https://www.doxygen.nl/index.html) (optional)
-The Python interface of SQUANDER was developed and tested with Python 3.6-3.9.
-The SQUANDER Python interface needs the following packages to be installed on
-the system: * [Qiskit](https://qiskit.org/documentation/install.html) * [Numpy]
-(https://numpy.org/install/) * [scipy](https://www.scipy.org/install.html) *
-[scikit-build](https://scikit-build.readthedocs.io/en/latest/) * [tbb-devel]
-(https://pypi.org/project/tbb-devel/) (containing the TBB Library) * [gsl]
-(https://anaconda.org/conda-forge/gsl) (containing the GNU Scientific Library)
-### How to obtain GNU Scientific Library In order to build and use the SQUANDER
-we recommend the Anaconda virtual python environment providing all the required
-dependencies for SQUANDER. One can easily install the GNU Scientific Library
-for local users by the command $ conda install -c conda-forge gsl
-Alternatively, a python binding project alongside the GNU GSL library is
-accessible via pypi repository: $ pip install numpy swig $ pip install pygsl
-Here we describe an alternative way to deploy GNU Scientific Library from
-source by the end user without administrative privileges. The GNU Scientific
-Library can be downloaded from the site [https://www.gnu.org/software/gsl/]
-(https://www.gnu.org/software/gsl/). After the downloaded package is extracted
-somewhere in the home directory of the user (**path/to/gsl/source**), one
-should configure the building environment using the **configure** tool.
-Depending on the individual settings the default compiler to be invoked might
-be different from HPC to HPC. To ensure the usage of the GNU compiler, the
-following shell command should be executed inside the directory **path/to/gsl/
-source**: $ ./configure --prefix=path/to/gsl FC=gfortran CC=gcc CXX=g++
-(Similarly, Intel compiler can be forced by setting FC=ifort CC=icc and
-CXX=icpc.) The installation directory of the compiled GNU Scientific Library is
-given by **--prefix=path/to/gsl** (which is different from the directory path
-of the source files given by **path/to/gslsource**). To install GNU Scientific
-Library the user should have read and write permissions on the path **path/to/
-gsl** (which might be for example /home/username/gsl). After the successful
-configuration the GNU Scientific Library can be compiled by the shell command $
-make The compilation of the GNU Scientific Library takes some time. When the
-compilation is done, the package (including the C header files and the static
-and shared libraries) is installed into the directory **path/to/gsl** by the
-shell command: $ make install ### Install SQUANDER from Python Package Index
-(PyPI) Since version 1.7.1 the SQUANDER package is accessible at Python Package
-Index (PyPI). The package can be installed on linux systems following the steps
-outlined below: $ pip install numpy swig tbb-devel wheel scikit-build ninja
-qiskit $ pip install pygsl $ pip install squander ### Download the SQUANDER
-package The developer version of the Quantum Gate Decomposer package can be
-downloaded from github repository [https://github.com/rakytap/quantum-gate-
-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/
-tree/master). After the package is downloaded into the directory **path/to/
-SQUANDER/package** (which would be the path to the source code of the SQUANDER
-package), one can proceed to the compilation steps described in the next
-section. ### How to build the SQUANDER package The SQUANDER package is equipped
-with a Python build script and CMake tools to ease the compilation and the
-deployment of the package. To ensure that SQUANDER package would find the
-necessary libraries and header files during compilation time it is advised to
-define the following environment variables: $ export GSL_LIB_DIR=path/to/gsl/
-lib(64) $ export GSL_INC_DIR=path/to/gsl/include The SQUANDER package is
-parallelized via Threading Building Block (TBB) libraries. If TBB is not
-present in the system, it can be easily installed via python package [tbb-
-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
-can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
-be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
-oneapi-src/oneTBB) and built from source. In this case one should supply the
-necessary environment variables pointing to the header and library files of the
-TBB package. For newer Intel compilers the TBB package is part of the Intel
-compiler package, similarly to the MKL package. If the TBB library is located
-at non-standrad path or the SQUANDER package is compiled with GNU compiler,
-then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
-TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
-successful compilation. When the TBB library is installed via a python package,
-setting the environment variables above is not necessary. The SQUANDER package
-with C++ Python extensions can be compiled via the Python script **setup.py**
-located in the root directory of the SQUANDER package. The script automatically
-finds out the CBLAS library working behind the numpy package and uses it in
-further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Developer build We
-recommend to install the SQUANDER package in the Anaconda environment. In order
-to install the necessary requirements, follow the steps below: Creating new
-python environment: $ conda create -n qgd Activate the new anaconda environment
-$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
-pytest scikit-build tbb-devel $ conda install -c conda-forge gsl $ pip install
-qiskit matplotlib After the basic environment variables are set and the
-dependencies are installed, the compilation of the package can be started by
-the Python command: $ python3 setup.py build_ext The command above starts the
-compilation of the SQUANDER C++ library and builds the necessary C++ Python
-interface extensions of the SQUANDER package in place. After a successful
-build, one can register the SQUANDER package in the Python distribution in
-developer (i.e. editable) mode by command: $ python -m pip install -e . ###
-Binary distribution After the environment variables are set it is possible to
-build wheel binaries of the SQUANDER package. In order to launch the
-compilation process from python, **[scikit-build](https://scikit-
-build.readthedocs.io/en/latest/)** package is necessary. (It is optional to
-install the ninja package which speeds up the building process by parallel
-compilation.) The binary wheel can be constructed by command $ python3 setup.py
-bdist_wheel in the root directory of the SQUADER package. The created SQUANDER
-wheel can be installed on the local machine by issuing the command from the
-directory **path/to/SQUANDER/package/dist** $ pip3 install qgd-*.whl We notice,
-that the created wheel is not portable, since it contains hard coded link to
-external libraries (TBB and CBLAS). ### Source distribution A portable source
-distribution of the SQUANDER package can be created by a command launched from
-the root directory of the SQUANDER package: $ python3 setup.py sdist In order
-to create a source distribution it is not necessary to set the environment
-variables, since this script only collects the necessary files and pack them
-into a tar ball located in the directory **path/to/SQUANDER/package/dist**. In
-order to install the SQUANDER package from source tar ball, see the previous
-section discussing the initialization of the environment variables. The package
-can be compiled and installed by the command $ pip3 install qgd-*.tar.gz issued
-from directory **path/to/SQUANDER/package/dist** (It is optional to install the
-ninja package which speeds up the building process by parallel compilation.)
-### How to use The algorithm implemented in the SQUANDER package intends to
-transform the given unitary into an identity matrix via a sequence of two-qubit
-and one-qubit gate operations applied on the unitary. Thus, in order to get the
-decomposition of a unitary, one should rather provide the complex transpose of
-this unitary as the input for the SQUANDER decomposing process, as can be seen
-in the examples. ## Python Interface The SQUANDER package contains a Python
-interface allowing the access of the functionalities of the SQUANDER package
-from Python. The usage of the SQUANDER Python interface is demonstrated in the
-example files in the directory **examples** located in the directory **path/to/
-SQUANDER/package**, or in test files located in sub-directories of **path/to/
-SQUANDER/package/qgd_python/*/test**. ### Example code snippet Here we provide
-an example to use the SQUANDER package. The following python interface is
-accessible from version 1.8.0. In this example we use two optimization engines
-for the decomposition: 1. An evolutionary engine called AGENTS 2. Second order
-gradient descend algorithm (BFGS) Firstly we construct a Python map to set
-hyper-parameters during the gate synthesis. #Python map containing hyper-
-parameters config = { 'max_outer_iterations': 1, 'max_inner_iterations_agent':
-25000, 'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
+Metadata-Version: 2.1 Name: squander Version: 1.8.1 Summary: The C++ binding
+for the SQUANDER package Home-page: https://github.com/rakytap/sequential-
+quantum-gate-decomposer Maintainer: Peter Rakyta Maintainer-email:
+peter.rakyta@ttk.elte.hu License: GNU General Public License v3.0 Keywords:
+test,cmake,extension Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: Programming Language :: C Classifier:
+Programming Language :: C++ Description-Content-Type: text/markdown License-
+File: LICENSE [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)]
+(https://doi.org/10.5281/zenodo.4508680) [trackgit-views] # Sequential Quantum
+Gate Decomposer (SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER)
+package provides a novel solution to decompose any n-qubit unitaries into a
+sequence of one-qubit rotations and two-qubit controlled gates (such as
+controlled NOT or controlled phase gate). SQUANDER utilizes two novel gate
+synthesis techniques reported in Refereces [1] and [2]. (i) To synthesize
+general unitaries SQUANDER applies periodic layers of two-qubit and parametric
+one-qubit gates to an n-qubit unitary such that the resulting unitary is 1-
+qubit decoupled, i.e., is a tensor product of an (n-1)-qubit and a 1-qubit
+unitary. Continuing the decoupling procedure sequentially one arrives at the
+end to a full decomposition of the original unitary into 1- and 2-qubit gates.
+SQUANDER provides lower CNOT counts for generic n-qubit unitaries (up to n=6)
+than the previously provided lower bounds. (ii) An adaptive circuit compression
+is used to optimize quantum circuit by the application of parametric two-qubit
+gates in the synthesis process. The utilization of these parametric two-qubit
+gates in the circuit design allows one to transform the discrete combinatorial
+problem of circuit synthesis into an optimization problem over continuous
+variables. The circuit is then compressed by a sequential removal of two-qubit
+gates from the design, while the remaining building blocks are continuously
+adapted to the reduced gate structure by iterated learning cycles. The SQUANDER
+library is written in C/C++ providing a Python interface via [C++ extensions]
+(https://docs.python.org/3/library/ctypes.html). The present package is
+supplied with Python building script and CMake tools to ease its deployment.
+The SQUANDER package can be built with both Intel and GNU compilers, and can be
+link against various CBLAS libraries installed on the system. (So far the CLBAS
+libraries of the GNU Scientific Library, OpenBLAS and the Intel MKL packages
+were tested.) In the following we briefly summarize the steps to build, install
+and use the SQUANDER package. The project was supported by grant OTKA PD123927
+and by the Ministry of Innovation and Technology and the National Research,
+Development and Innovation Office within the Quantum Information National
+Laboratory of Hungary. Find the documantation of the SQUANDER package at
+[CodeDocs[xyz]](https://codedocs.xyz/rakytap/sequential-quantum-gate-
+decomposer/) ### Contact Us Have a question about the SQUANDER package? Don't
+hesitate to contact us at the following e-mails: * ZoltÃ¡n ZimborÃ¡s
+(researcher): zimboras.zoltan@wigner.hu * Peter Rakyta (developer):
+peter.rakyta@ttk.elte.hu ### Dependencies The dependencies necessary to compile
+and build the SQUANDER package are the followings: * [CMake](https://cmake.org/
+) (>=3.10.2) * C++/C [Intel](https://software.intel.com/content/www/us/en/
+develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://
+gcc.gnu.org/) (>=v4.8.1) compiler * [TBB](https://github.com/oneapi-src/oneTBB)
+library (shipped with tbb-devel Python package) * [Intel MKL](https://
+software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html)
+(optional) * [OpenBlas](https://www.openblas.net/) (optional, recommended) *
+[LAPACKE](https://www.netlib.org/lapack/lapacke.html) * [Doxygen](https://
+www.doxygen.nl/index.html) (optional) The Python interface of SQUANDER was
+developed and tested with Python 3.6-3.9. The SQUANDER Python interface needs
+the following packages to be installed on the system: * [Qiskit](https://
+qiskit.org/documentation/install.html) * [Numpy](https://numpy.org/install/) *
+[scipy](https://www.scipy.org/install.html) * [scikit-build](https://scikit-
+build.readthedocs.io/en/latest/) * [tbb-devel](https://pypi.org/project/tbb-
+devel/) (containing the TBB Library) ### Install SQUANDER from Python Package
+Index (PyPI) Since version 1.7.1 the SQUANDER package is accessible at Python
+Package Index (PyPI). The package can be installed on linux systems following
+the steps outlined below: $ pip install numpy swig tbb-devel wheel scikit-build
+ninja qiskit $ pip install squander ### Download the SQUANDER package The
+developer version of the Quantum Gate Decomposer package can be downloaded from
+github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/
+master](https://github.com/rakytap/quantum-gate-decomposer/tree/master). After
+the package is downloaded into the directory **path/to/SQUANDER/package**
+(which would be the path to the source code of the SQUANDER package), one can
+proceed to the compilation steps described in the next section. ### How to
+build the SQUANDER package The SQUANDER package is equipped with a Python build
+script and CMake tools to ease the compilation and the deployment of the
+package. The SQUANDER package is parallelized via Threading Building Block
+(TBB) libraries. If TBB is not present in the system, it can be easily
+installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
+Alternatively the TBB libraries can be installed via apt or yum utility (sudo
+apt install libtbb-dev) or it can be downloaded from [https://github.com/
+oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB) and built from source.
+In this case one should supply the necessary environment variables pointing to
+the header and library files of the TBB package. For newer Intel compilers the
+TBB package is part of the Intel compiler package, similarly to the MKL
+package. If the TBB library is located at non-standrad path or the SQUANDER
+package is compiled with GNU compiler, then setting the $ export
+TBB_LIB_DIR=path/to/TBB/lib(64) $ export TBB_INC_DIR=path/to/TBB/include
+environment variables are sufficient for successful compilation. When the TBB
+library is installed via a python package, setting the environment variables
+above is not necessary. The SQUANDER package with C++ Python extensions can be
+compiled via the Python script **setup.py** located in the root directory of
+the SQUANDER package. The script automatically finds out the CBLAS library
+working behind the numpy package and uses it in further linking. The
+**setup.py** script also build the C++ library of the SQUANDER package by
+making the appropriate CMake calls. ### Developer build We recommend to install
+the SQUANDER package in the Anaconda environment. In order to install the
+necessary requirements, follow the steps below: Creating new python
+environment: $ conda create -n qgd Activate the new anaconda environment $
+conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
+scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+environment variables are set and the dependencies are installed, the
+compilation of the package can be started by the Python command: $ python3
+setup.py build_ext The command above starts the compilation of the SQUANDER C++
+library and builds the necessary C++ Python interface extensions of the
+SQUANDER package in place. After a successful build, one can register the
+SQUANDER package in the Python distribution in developer (i.e. editable) mode
+by command: $ python -m pip install -e . ### Binary distribution After the
+environment variables are set it is possible to build wheel binaries of the
+SQUANDER package. In order to launch the compilation process from python, **
+[scikit-build](https://scikit-build.readthedocs.io/en/latest/)** package is
+necessary. (It is optional to install the ninja package which speeds up the
+building process by parallel compilation.) The binary wheel can be constructed
+by command $ python3 setup.py bdist_wheel in the root directory of the SQUADER
+package. The created SQUANDER wheel can be installed on the local machine by
+issuing the command from the directory **path/to/SQUANDER/package/dist** $ pip3
+install qgd-*.whl We notice, that the created wheel is not portable, since it
+contains hard coded link to external libraries (TBB and CBLAS). ### Source
+distribution A portable source distribution of the SQUANDER package can be
+created by a command launched from the root directory of the SQUANDER package:
+$ python3 setup.py sdist In order to create a source distribution it is not
+necessary to set the environment variables, since this script only collects the
+necessary files and pack them into a tar ball located in the directory **path/
+to/SQUANDER/package/dist**. In order to install the SQUANDER package from
+source tar ball, see the previous section discussing the initialization of the
+environment variables. The package can be compiled and installed by the command
+$ pip3 install qgd-*.tar.gz issued from directory **path/to/SQUANDER/package/
+dist** (It is optional to install the ninja package which speeds up the
+building process by parallel compilation.) ### How to use The algorithm
+implemented in the SQUANDER package intends to transform the given unitary into
+an identity matrix via a sequence of two-qubit and one-qubit gate operations
+applied on the unitary. Thus, in order to get the decomposition of a unitary,
+one should rather provide the complex transpose of this unitary as the input
+for the SQUANDER decomposing process, as can be seen in the examples. ## Python
+Interface The SQUANDER package contains a Python interface allowing the access
+of the functionalities of the SQUANDER package from Python. The usage of the
+SQUANDER Python interface is demonstrated in the example files in the directory
+**examples** located in the directory **path/to/SQUANDER/package**, or in test
+files located in sub-directories of **path/to/SQUANDER/package/qgd_python/*/
+test**. ### Example code snippet Here we provide an example to use the SQUANDER
+package. The following python interface is accessible from version 1.8.0. In
+this example we use two optimization engines for the decomposition: 1. An
+evolutionary engine called AGENTS 2. Second order gradient descend algorithm
+(BFGS) Firstly we construct a Python map to set hyper-parameters during the
+gate synthesis. #Python map containing hyper-parameters config =
+{ 'max_outer_iterations': 1, 'max_inner_iterations_agent': 25000,
+'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
 'max_inner_iterations_final': 5000, 'Randomized_Radius': 0.3,
 'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-4,
 'optimization_tolerance': 1e-8, 'agent_num': 10} Next we initialize the
 decomposition class with the unitary Umtx to be decomposed. # creating a class
 to decompose the unitary from squander import N_Qubit_Decomposition_adaptive
 cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config ) The
 verbosity of the execution output can be controlled by the function call #
```

### Comparing `squander-1.8.0/cmake/check_AVX.cmake` & `squander-1.8.1/cmake/check_AVX.cmake`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/Adam.cpp` & `squander-1.8.1/common/Adam.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/common.cpp` & `squander-1.8.1/common/common.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/common_DFE.cpp` & `squander-1.8.1/common/common_DFE.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/config_element.cpp` & `squander-1.8.1/common/config_element.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/dot.cpp` & `squander-1.8.1/common/dot.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/Adam.h` & `squander-1.8.1/common/include/Adam.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/QGDTypes.h` & `squander-1.8.1/common/include/QGDTypes.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/common.h` & `squander-1.8.1/common/include/common.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/common_DFE.h` & `squander-1.8.1/common/include/common_DFE.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/config_element.h` & `squander-1.8.1/common/include/config_element.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/dot.h` & `squander-1.8.1/common/include/dot.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/logging.h` & `squander-1.8.1/common/include/logging.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/matrix.h` & `squander-1.8.1/common/include/matrix.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/matrix_base.h` & `squander-1.8.1/common/include/matrix_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/matrix_real.h` & `squander-1.8.1/common/include/matrix_real.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/mpi_base.h` & `squander-1.8.1/common/include/mpi_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/include/numpy_interface.h` & `squander-1.8.1/common/include/numpy_interface.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/logging.cpp` & `squander-1.8.1/common/logging.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/matrix.cpp` & `squander-1.8.1/common/matrix.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/matrix_real.cpp` & `squander-1.8.1/common/matrix_real.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/mpi_base.cpp` & `squander-1.8.1/common/mpi_base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/common/numpy_interface.cpp` & `squander-1.8.1/common/numpy_interface.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/Decomposition_Base.cpp` & `squander-1.8.1/decomposition/Decomposition_Base.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -419,52 +419,52 @@
             optimization_block = gates.size();
         }
 
         // random generator of real numbers   
         std::uniform_real_distribution<> distrib_real(0.0, 2*M_PI);
 
         // the array storing the optimized parameters
-        gsl_vector* optimized_parameters_gsl = gsl_vector_alloc (parameter_num_loc);
+        Matrix_real optimized_parameters(1, parameter_num_loc);
 
         // preparing solution guess for the iterations
         if ( initial_guess == ZEROS ) {
             for(int idx = 0; idx < parameter_num-solution_guess_num; idx++) {
-                optimized_parameters_gsl->data[idx] = 0;
+                optimized_parameters[idx] = 0;
             }
         }
         else if ( initial_guess == RANDOM ) {
             for(int idx = 0; idx < parameter_num-solution_guess_num; idx++) {
-                optimized_parameters_gsl->data[idx] = distrib_real(gen);
+                optimized_parameters[idx] = distrib_real(gen);
             }
 
 #ifdef __MPI__        
-            MPI_Bcast( (void*)optimized_parameters_gsl->data, parameter_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+            MPI_Bcast( (void*)optimized_parameters.get_data(), parameter_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif
 
 
         }
         else if ( initial_guess == CLOSE_TO_ZERO ) {
             for(int idx = 0; idx < parameter_num-solution_guess_num; idx++) {
-                optimized_parameters_gsl->data[idx] = distrib_real(gen)/100;
+                optimized_parameters[idx] = distrib_real(gen)/100;
             }
 
 #ifdef __MPI__        
-            MPI_Bcast( (void*)optimized_parameters_gsl->data, parameter_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+            MPI_Bcast( (void*)optimized_parameters.get_data(), parameter_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif
 
         }
         else {
 	     std::stringstream sstream;
 	     sstream << "bad value for initial guess" << std::endl;
 	     print(sstream, 0);  	
 	     exit(-1);
         }
 
         if ( solution_guess_num > 0) {
-            memcpy(optimized_parameters_gsl->data + parameter_num-solution_guess_num, solution_guess, solution_guess_num*sizeof(double));
+            memcpy(optimized_parameters.get_data() + parameter_num-solution_guess_num, solution_guess, solution_guess_num*sizeof(double));
         }
 
         // starting number of gate block applied prior to the optimalized gate blocks
         int pre_gate_parameter_num = 0;
 
         // defining temporary variables for iteration cycles
         int block_idx_end;
@@ -474,15 +474,15 @@
         Gate* fixed_gate_post = new Gate( qbit_num );
         std::vector<Matrix, tbb::cache_aligned_allocator<Matrix>> gates_mtxs_post;
 
         // the identity matrix used in the calculations
         Matrix Identity =  create_identity( matrix_size );
 
 
-        gsl_vector *solution_guess_gsl = NULL;
+        Matrix_real solution_guess_tmp;
 
 
         // maximal number of outer iterations overriden by config
         long long max_outer_iterations_loc;
         if ( config.count("max_outer_iterations") > 0 ) {
             config["max_outer_iterations"].get_property( max_outer_iterations_loc );
          
@@ -533,15 +533,15 @@
             }
 
 
             // ***** get the fixed gates applied after the optimized gates *****
             // create a list of post gates matrices
             if (block_idx_start == (int)gates_loc.size() ) {
                 // matrix of the fixed gates aplied after the gates to be varied
-                double* fixed_parameters_post = optimized_parameters_gsl->data;
+                double* fixed_parameters_post = optimized_parameters.get_data();
                 std::vector<Gate*>::iterator fixed_gates_post_it = gates_loc.begin();
 
                 gates_mtxs_post = get_gate_products(fixed_parameters_post, fixed_gates_post_it, block_idx_end);
             }
 
             // Create a general gate describing the cumulative effect of gates following the optimized gates
             if (block_idx_end > 0) {
@@ -558,38 +558,37 @@
             for ( int idx=block_idx_end; idx<block_idx_start; idx++ ) {
                 gates.push_back( gates_loc[idx] );
             }
 
 
             // constructing solution guess for the optimization
             parameter_num = block_parameter_num;
-            if ( solution_guess_gsl == NULL ) {
-                solution_guess_gsl = gsl_vector_alloc (parameter_num);
+            if ( solution_guess_tmp.size() == 0 ) {
+                solution_guess_tmp = Matrix_real(1, parameter_num);
             }
-            else if ( parameter_num != (int)solution_guess_gsl->size ) {
-                gsl_vector_free(solution_guess_gsl);
-                solution_guess_gsl = gsl_vector_alloc (parameter_num);
+            else if ( parameter_num != (int)solution_guess_tmp.size() ) {
+                solution_guess_tmp = Matrix_real(1, parameter_num);
             }
-            memcpy( solution_guess_gsl->data, optimized_parameters_gsl->data+parameter_num_loc - pre_gate_parameter_num - block_parameter_num, parameter_num*sizeof(double) );
+            memcpy( solution_guess_tmp.get_data(), optimized_parameters.get_data()+parameter_num_loc - pre_gate_parameter_num - block_parameter_num, parameter_num*sizeof(double) );
 
             // solve the optimization problem of the block
-            solve_layer_optimization_problem( parameter_num, solution_guess_gsl  );
+            solve_layer_optimization_problem( parameter_num, solution_guess_tmp );
 
             // add the current minimum to the array of minimums and calculate the mean
             double minvec_mean = 0;
             for (int idx=min_vec_num-1; idx>0; idx--) {
                 minimum_vec[idx] = minimum_vec[idx-1];
                 minvec_mean = minvec_mean + minimum_vec[idx-1];
             }
             minimum_vec[0] = current_minimum;
             minvec_mean = minvec_mean + current_minimum;
             minvec_mean = minvec_mean/min_vec_num;
 
             // store the obtained optimalized parameters for the block
-            memcpy( optimized_parameters_gsl->data+parameter_num_loc - pre_gate_parameter_num-block_parameter_num, optimized_parameters_mtx.get_data(), parameter_num*sizeof(double) );
+            memcpy( optimized_parameters.get_data()+parameter_num_loc - pre_gate_parameter_num-block_parameter_num, optimized_parameters_mtx.get_data(), parameter_num*sizeof(double) );
 
             if (block_idx_end == 0) {
                 block_idx_start = gates_loc.size();
                 pre_gate_parameter_num = 0;
             }
             else {
                 block_idx_start = block_idx_start - optimization_block;
@@ -604,15 +603,20 @@
 		sstream << "The minimum with " << layer_num << " layers after " << iter_idx << " outer iterations is " << current_minimum << " calculated in " << (current_time - start_time).seconds() << " seconds" << std::endl;
 		print(sstream, 2);            
                 start_time = tbb::tick_count::now();
             }
 
 
             // calculate the variance of the last 10 minimums
-            double minvec_std = sqrt(gsl_stats_variance_m( minimum_vec, 1, min_vec_num, minvec_mean));
+            double minvec_std = 0.0;
+            for ( int kdx=0; kdx<min_vec_num; kdx++ ) {
+                double tmp = minimum_vec[kdx] - minvec_mean;
+                minvec_std += tmp*tmp;
+            }
+            minvec_std = sqrt(minvec_std/(min_vec_num-1));
 
             // conditions to break the iteration cycles
             if (std::abs(minvec_std/minimum_vec[min_vec_num-1]) < convergence_threshold ) {              
 		std::stringstream sstream;
 	        sstream << "The iterations converged to minimum " << current_minimum << " after " << iter_idx << " outer iterations with " << layer_num << " layers" << std::endl;
 		print(sstream, 1);             
                 break;
@@ -638,45 +642,38 @@
         optimization_block = optimization_block_loc;
 
         // store the result of the optimization
         gates.clear();
         gates = gates_loc;
 
         parameter_num = parameter_num_loc;
-/*
-        if (optimized_parameters != NULL ) {
-            qgd_free( optimized_parameters );
-        }
-*/
+
+
         optimized_parameters_mtx = Matrix_real( 1, parameter_num );
-        memcpy( optimized_parameters_mtx.get_data(), optimized_parameters_gsl->data, parameter_num*sizeof(double) );
+        memcpy( optimized_parameters_mtx.get_data(), optimized_parameters.get_data(), parameter_num*sizeof(double) );
 
 
-        // free unnecessary resources
-        gsl_vector_free(optimized_parameters_gsl);
-        gsl_vector_free(solution_guess_gsl);
-        optimized_parameters_gsl = NULL;
-        solution_guess_gsl = NULL;
 
         delete(fixed_gate_post);
 
         // restore the original unitary
         Umtx = Umtx_loc; // copy?
 
 
 }
 
 
 
+
 /**
 @brief Abstarct function to be used to solve a single sub-layer optimization problem. The optimalized parameters are stored in attribute optimized_parameters.
 @param 'num_of_parameters' The number of free parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Libarary vector containing the free parameters to be optimized.
+@param solution_guess Array containing the free parameters to be optimized.
 */
-void Decomposition_Base::solve_layer_optimization_problem( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void Decomposition_Base::solve_layer_optimization_problem( int num_of_parameters, Matrix_real solution_guess) {
     return;
 }
 
 
 
 
 /**
```

### Comparing `squander-1.8.0/decomposition/N_Qubit_Decomposition.cpp` & `squander-1.8.1/decomposition/N_Qubit_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/N_Qubit_Decomposition_Base.cpp` & `squander-1.8.1/decomposition/N_Qubit_Decomposition_Base.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     \brief Base class to determine the decomposition of a unitary into a sequence of two-qubit and one-qubit gate gates.
     This class contains the non-template implementation of the decomposition class
 */
 
 #include "N_Qubit_Decomposition_Base.h"
 #include "N_Qubit_Decomposition_Cost_Function.h"
 #include "Adam.h"
+#include "tolmin.h"
+#include "lbfgs.h"
 
 #include "RL_experience.h"
 
 #include <fstream>
 
 
 #ifdef __DFE__
@@ -325,59 +327,62 @@
             if ( check_optimization_solution() ) return;
 
             solve_optimization_problem(optimized_parameters_mtx.get_data(), parameter_num);
         }
 }
 
 
+
+
 /**
 @brief Call to solve layer by layer the optimization problem via calling one of the implemented algorithms. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem( int num_of_parameters, Matrix_real solution_guess) {
+
 
     switch ( alg ) {
         case ADAM:
-            solve_layer_optimization_problem_ADAM( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_ADAM( num_of_parameters, solution_guess);
             return;
         case ADAM_BATCHED:
-            solve_layer_optimization_problem_ADAM_BATCHED( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_ADAM_BATCHED( num_of_parameters, solution_guess);
             return;
         case AGENTS:
-            solve_layer_optimization_problem_AGENTS( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_AGENTS( num_of_parameters, solution_guess);
             return;
         case COSINE:
-            solve_layer_optimization_problem_COSINE( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_COSINE( num_of_parameters, solution_guess);
             return;
         case AGENTS_COMBINED:
-            solve_layer_optimization_problem_AGENTS_COMBINED( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_AGENTS_COMBINED( num_of_parameters, solution_guess);
             return;
         case BFGS:
-            solve_layer_optimization_problem_BFGS( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_BFGS( num_of_parameters, solution_guess);
             return;
         case BFGS2:
-            solve_layer_optimization_problem_BFGS2( num_of_parameters, solution_guess_gsl);
+            solve_layer_optimization_problem_BFGS2( num_of_parameters, solution_guess);
             return;
         default:
             std::string error("N_Qubit_Decomposition_Base::solve_layer_optimization_problem: unimplemented optimization algorithm");
             throw error;
     }
 
 
 }
 
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the COSINE algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_COSINE( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_COSINE( int num_of_parameters, Matrix_real& solution_guess) {
 
 #ifdef __DFE__
         if ( qbit_num >= 5 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
@@ -387,29 +392,28 @@
             return;
         }
 
 
         double M_PI_half = M_PI/2;
         double M_PI_double = M_PI*2;
 
-
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
             std::uniform_real_distribution<> distrib_real(0, M_PI_double); 
             for ( int idx=0; idx<num_of_parameters; idx++) {
-                solution_guess_gsl->data[idx] = distrib_real(gen);
+                solution_guess[idx] = distrib_real(gen);
             }
+
         }
 
 
 
-//memset( solution_guess_gsl->data, 0.0, solution_guess_gsl->size*sizeof(double) );
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
 
 
 
         std::stringstream sstream;
         double optimization_time = 0.0;
@@ -716,17 +720,17 @@
 
 }
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the AGENT algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_AGENTS( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_AGENTS( int num_of_parameters, Matrix_real& solution_guess) {
 
 
 #ifdef __DFE__
         if ( qbit_num >= 5 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
@@ -737,34 +741,35 @@
             return;
         }
 
 
         double M_PI_half = M_PI/2;
         double M_PI_double = M_PI*2;
 
-
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
             std::uniform_real_distribution<> distrib_real(0, M_PI_double); 
             for ( int idx=0; idx<num_of_parameters; idx++) {
-                solution_guess_gsl->data[idx] = distrib_real(gen);
+                solution_guess[idx] = distrib_real(gen);
             }
+
         }
 
 
+
 #ifdef __MPI__        
-        MPI_Bcast( (void*)solution_guess_gsl->data, num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+        MPI_Bcast( (void*)solution_guess.get_data(), num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif
 
 
 
-//memset( solution_guess_gsl->data, 0.0, solution_guess_gsl->size*sizeof(double) );
+
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
 
         long long sub_iter_idx = 0;
         double current_minimum_hold = current_minimum;
     
 
@@ -888,15 +893,15 @@
             memset( solution_guess_mtx_agent.get_data(), 0.0, solution_guess_mtx_agent.size()*sizeof(double) );              
 
 #ifdef __MPI__        
             if ( current_rank == 0 ) {
 #endif
 
                 if ( agent_idx == 0 ) {
-                    memcpy( solution_guess_mtx_agent.get_data(), solution_guess_gsl->data, solution_guess_gsl->size*sizeof(double) );
+                    memcpy( solution_guess_mtx_agent.get_data(), solution_guess.get_data(), solution_guess.size()*sizeof(double) );
                 }
                 else {
                     randomize_parameters( optimized_parameters_mtx, solution_guess_mtx_agent, current_minimum  ); 
                 }
 
 
 #ifdef __MPI__        
@@ -1223,46 +1228,46 @@
 }
 
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the AGENT COMBINED algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_AGENTS_COMBINED( int num_of_parameters, gsl_vector *solution_guess_gsl)  {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_AGENTS_COMBINED( int num_of_parameters, Matrix_real& solution_guess)  {
 
 
 
-    optimized_parameters_mtx = Matrix_real(solution_guess_gsl->data, solution_guess_gsl->size, 1);
+    optimized_parameters_mtx = Matrix_real(solution_guess.get_data(), solution_guess.size(), 1);
 
     for( int loop_idx=0; loop_idx<1; loop_idx++ ) {
 
-        gsl_vector *solution_guess_gsl_AGENTS = gsl_vector_alloc(num_of_parameters);
-        memcpy( solution_guess_gsl_AGENTS->data, optimized_parameters_mtx.get_data(), optimized_parameters_mtx.size()*sizeof(double) );
+        Matrix_real solution_guess_AGENTS(num_of_parameters ,1);
+        memcpy( solution_guess_AGENTS.get_data(), optimized_parameters_mtx.get_data(), optimized_parameters_mtx.size()*sizeof(double) );
 
-        solve_layer_optimization_problem_AGENTS( num_of_parameters, solution_guess_gsl_AGENTS );
+        solve_layer_optimization_problem_AGENTS( num_of_parameters, solution_guess_AGENTS );
 
 
-        gsl_vector *solution_guess_gsl_COSINE = gsl_vector_alloc(num_of_parameters);
-        memcpy( solution_guess_gsl_COSINE->data, optimized_parameters_mtx.get_data(), optimized_parameters_mtx.size()*sizeof(double) );
+        Matrix_real solution_guess_COSINE(num_of_parameters, 1);
+        memcpy( solution_guess_COSINE.get_data(), optimized_parameters_mtx.get_data(), optimized_parameters_mtx.size()*sizeof(double) );
 
-        solve_layer_optimization_problem_BFGS( num_of_parameters, solution_guess_gsl_COSINE );
+        solve_layer_optimization_problem_BFGS( num_of_parameters, solution_guess_COSINE );
 
     }
         
 
 }
 
 /**
 @brief Call to solve layer by layer the optimization problem via batched ADAM algorithm. (optimal for larger problems) The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_ADAM_BATCHED( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_ADAM_BATCHED( int num_of_parameters, Matrix_real& solution_guess) {
 
 
 #ifdef __DFE__
         if ( qbit_num >= 2 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
@@ -1270,22 +1275,21 @@
 
 
         if (gates.size() == 0 ) {
             return;
         }
 
 
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
         }
-//memset( solution_guess_gsl->data, 0.0, solution_guess_gsl->size*sizeof(double) );
 
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
 
         int random_shift_count = 0;
         int sub_iter_idx = 0;
         double current_minimum_hold = current_minimum;
     
@@ -1295,20 +1299,18 @@
 pure_DFE_time = 0.0;
         Adam optimizer;
         optimizer.initialize_moment_and_variance( num_of_parameters );
 
 
 
         // the array storing the optimized parameters
-        gsl_vector* grad_gsl = gsl_vector_alloc(num_of_parameters);
-        gsl_vector* solution_guess_tmp = gsl_vector_alloc(num_of_parameters);
-        memcpy(solution_guess_tmp->data, solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+        Matrix_real solution_guess_tmp = Matrix_real( num_of_parameters, 1 );
+        memcpy(solution_guess_tmp.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
 
-        Matrix_real solution_guess_tmp_mtx = Matrix_real( solution_guess_tmp->data, num_of_parameters, 1 );
-        Matrix_real grad_mtx = Matrix_real( grad_gsl->data, num_of_parameters, 1 );
+        Matrix_real grad_mtx = Matrix_real( num_of_parameters, 1 );
         //solution_guess_tmp_mtx.print_matrix();
 
 
         long long max_inner_iterations_loc;
         if ( config.count("max_inner_iterations_agent") > 0 ) {
              config["max_inner_iterations_agent"].get_property( max_inner_iterations_loc );  
         }
@@ -1347,15 +1349,15 @@
             Umtx = Umtx_slice;
 
             for ( long long iter_idx=0; iter_idx<max_inner_iterations_loc; iter_idx++ ) {
 
             
 
 
-                optimization_problem_combined( solution_guess_tmp, (void*)(this), &f0, grad_gsl );
+                optimization_problem_combined( solution_guess_tmp, (void*)(this), &f0, grad_mtx );
 
                 prev_cost_fnv_val = f0;
   
                 if (sub_iter_idx == 1 ) {
                     current_minimum_hold = f0;   
                
                     if ( adaptive_eta )  { 
@@ -1370,15 +1372,15 @@
                     sub_iter_idx = 0;
                     current_minimum_hold = f0;        
                 }
     
     
                 if (current_minimum > f0 ) {
                     current_minimum = f0;
-                    memcpy( optimized_parameters_mtx.get_data(),  solution_guess_tmp->data, num_of_parameters*sizeof(double) );
+                    memcpy( optimized_parameters_mtx.get_data(),  solution_guess.get_data(), num_of_parameters*sizeof(double) );
                     //double new_eta = 1e-3 * f0 * f0;
                 
                     if ( adaptive_eta )  {
                         double new_eta = 1e-3 * f0;
                         optimizer.eta = new_eta > 1e-6 ? new_eta : 1e-6;
                         optimizer.eta = new_eta < 1e-1 ? new_eta : 1e-1;
                     }
@@ -1405,15 +1407,15 @@
                 }
 
 
 
                 // calculate the gradient norm
                 double norm = 0.0;
                 for ( int grad_idx=0; grad_idx<num_of_parameters; grad_idx++ ) {
-                    norm += grad_gsl->data[grad_idx]*grad_gsl->data[grad_idx];
+                    norm += grad_mtx[grad_idx]*grad_mtx[grad_idx];
                 }
                 norm = std::sqrt(norm);
                     
 
                 if ( sub_iter_idx> iteration_threshold_of_randomization || ADAM_status != 0 ) {
 
                     //random_shift_count++;
@@ -1428,28 +1430,28 @@
                         sstream << "ADAM: initiate randomization at " << f0 << ", gradient norm " << norm << std::endl;
                     }
                     else {
                         sstream << "ADAM: leaving local minimum " << f0 << ", gradient norm " << norm << " eta: " << optimizer.eta << std::endl;
                     }
                     print(sstream, 0);   
                     
-                    Matrix_real solution_guess_tmp_mtx( solution_guess_tmp->data, solution_guess_tmp->size, 1);
-                    randomize_parameters(optimized_parameters_mtx, solution_guess_tmp_mtx, f0 );
+
+                    randomize_parameters(optimized_parameters_mtx, solution_guess_tmp, f0 );
         
                     optimizer.reset();
                     optimizer.initialize_moment_and_variance( num_of_parameters );   
 
                     ADAM_status = 0;   
 
                     //optimizer.eta = 1e-3;
         
                 }
 
                 else {
-                    ADAM_status = optimizer.update(solution_guess_tmp_mtx, grad_mtx, f0);
+                    ADAM_status = optimizer.update(solution_guess_tmp, grad_mtx, f0);
                 }
 
                 sub_iter_idx++;
 
             }
 
 
@@ -1457,31 +1459,29 @@
 
         }
 
         sstream.str("");
         sstream << "obtained minimum: " << current_minimum << std::endl;
 
 
-        gsl_vector_free(grad_gsl);
-        gsl_vector_free(solution_guess_tmp);
         tbb::tick_count adam_end = tbb::tick_count::now();
         adam_time  = adam_time + (adam_end-adam_start).seconds();
         sstream << "adam time: " << adam_time << ", pure DFE time:  " << pure_DFE_time << " " << f0 << std::endl;
         
         print(sstream, 0); 
         
 
 }
 
 /**
 @brief Call to solve layer by layer the optimization problem via ADAM algorithm. (optimal for larger problems) The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_ADAM( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_ADAM( int num_of_parameters, Matrix_real& solution_guess) {
 
 #ifdef __DFE__
         if ( qbit_num >= 2 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
@@ -1489,22 +1489,22 @@
 
         if (gates.size() == 0 ) {
             return;
         }
 
 
 
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
         }
-//memset( solution_guess_gsl->data, 0.0, solution_guess_gsl->size*sizeof(double) );
+
 
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
         int random_shift_count = 0;
         long long sub_iter_idx = 0;
         double current_minimum_hold = current_minimum;
     
 
@@ -1513,21 +1513,18 @@
 pure_DFE_time = 0.0;
         Adam optimizer;
         optimizer.initialize_moment_and_variance( num_of_parameters );
 
 
 
         // the array storing the optimized parameters
-        gsl_vector* grad_gsl = gsl_vector_alloc(num_of_parameters);
-        gsl_vector* solution_guess_tmp = gsl_vector_alloc(num_of_parameters);
-        memcpy(solution_guess_tmp->data, solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+        Matrix_real solution_guess_tmp = Matrix_real( num_of_parameters, 1 );
+        memcpy(solution_guess_tmp.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
 
-        Matrix_real solution_guess_tmp_mtx = Matrix_real( solution_guess_tmp->data, num_of_parameters, 1 );
-        Matrix_real grad_mtx = Matrix_real( grad_gsl->data, num_of_parameters, 1 );
-        //solution_guess_tmp_mtx.print_matrix();
+        Matrix_real grad_mtx = Matrix_real( num_of_parameters, 1 );
 
 
 
 
 
 
         int ADAM_status = 0;
@@ -1568,15 +1565,15 @@
         
 
         for ( long long iter_idx=0; iter_idx<max_inner_iterations_loc; iter_idx++ ) {
 
             number_of_iters++;
 
 
-            optimization_problem_combined( solution_guess_tmp, (void*)(this), &f0, grad_gsl );
+            optimization_problem_combined( solution_guess_tmp, (void*)(this), &f0, grad_mtx );
 
             prev_cost_fnv_val = f0;
   
             if (sub_iter_idx == 1 ) {
                 current_minimum_hold = f0;   
                
                 if ( adaptive_eta )  { 
@@ -1591,31 +1588,30 @@
                 sub_iter_idx = 0;
                 current_minimum_hold = f0;        
             }
     
     
             if (current_minimum > f0 ) {
                 current_minimum = f0;
-                memcpy( optimized_parameters_mtx.get_data(),  solution_guess_tmp->data, num_of_parameters*sizeof(double) );
+                memcpy( optimized_parameters_mtx.get_data(),  solution_guess_tmp.get_data(), num_of_parameters*sizeof(double) );
                 //double new_eta = 1e-3 * f0 * f0;
                 
                 if ( adaptive_eta )  {
                     double new_eta = 1e-3 * f0;
                     optimizer.eta = new_eta > 1e-6 ? new_eta : 1e-6;
                     optimizer.eta = new_eta < 1e-1 ? new_eta : 1e-1;
                 }
                 
                 randomization_successful = 1;
             }
     
 
             if ( iter_idx % 5000 == 0 ) {
 
-                Matrix_real solution_guess_tmp_mtx( solution_guess_tmp->data, solution_guess_tmp->size, 1 );
-                Matrix matrix_new = get_transformed_matrix( solution_guess_tmp_mtx, gates.begin(), gates.size(), Umtx );
+                Matrix matrix_new = get_transformed_matrix( solution_guess_tmp, gates.begin(), gates.size(), Umtx );
 
                 std::stringstream sstream;
                 sstream << "ADAM: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100 << "\%, current minimum:" << current_minimum << ", current cost function:" << get_cost_function(matrix_new, trace_offset) << ", sub_iter_idx:" << sub_iter_idx <<std::endl;
                 print(sstream, 0);   
                 std::string filename("initial_circuit_iteration.binary");
                 export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
             }
@@ -1626,15 +1622,15 @@
             }
 
 
 
                 // calculate the gradient norm
                 double norm = 0.0;
                 for ( int grad_idx=0; grad_idx<num_of_parameters; grad_idx++ ) {
-                    norm += grad_gsl->data[grad_idx]*grad_gsl->data[grad_idx];
+                    norm += grad_mtx[grad_idx]*grad_mtx[grad_idx];
                 }
                 norm = std::sqrt(norm);
                 
 //grad_mtx.print_matrix();
 /*
             if ( ADAM_status == 0 && norm > 0.01 && optimizer.eta < 1e-4) {
 
@@ -1670,77 +1666,74 @@
                     sstream << "ADAM: initiate randomization at " << f0 << ", gradient norm " << norm << std::endl;
                 }
                 else {
                     sstream << "ADAM: leaving local minimum " << f0 << ", gradient norm " << norm << " eta: " << optimizer.eta << std::endl;
                 }
                 print(sstream, 0);   
                     
-                 Matrix_real solution_guess_gsl_mtx( solution_guess_gsl->data, solution_guess_gsl->size, 1 );
-                randomize_parameters(optimized_parameters_mtx, solution_guess_tmp_mtx, f0 );
+                randomize_parameters(optimized_parameters_mtx, solution_guess_tmp, f0 );
                 randomization_successful = 0;
         
                 optimizer.reset();
                 optimizer.initialize_moment_and_variance( num_of_parameters );   
 
                 ADAM_status = 0;   
 
                 //optimizer.eta = 1e-3;
         
             }
 
             else {
-                ADAM_status = optimizer.update(solution_guess_tmp_mtx, grad_mtx, f0);
+                ADAM_status = optimizer.update(solution_guess_tmp, grad_mtx, f0);
             }
 
             sub_iter_idx++;
 
         }
         sstream.str("");
         sstream << "obtained minimum: " << current_minimum << std::endl;
 
 
-        gsl_vector_free(grad_gsl);
-        gsl_vector_free(solution_guess_tmp);
         tbb::tick_count adam_end = tbb::tick_count::now();
         adam_time  = adam_time + (adam_end-adam_start).seconds();
         sstream << "adam time: " << adam_time << ", pure DFE time:  " << pure_DFE_time << " " << f0 << std::endl;
 
         print(sstream, 0); 
 
 }
 
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via BBFG algorithm. (optimal for smaller problems) The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_BFGS( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_BFGS( int num_of_parameters, Matrix_real& solution_guess) {
 
 
 #ifdef __DFE__
         if ( qbit_num >= 2 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
         if (gates.size() == 0 ) {
             return;
         }
 
 
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
         }
 
 
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
         // maximal number of iteration loops
         int iteration_loops_max;
         try {
             iteration_loops_max = std::max(iteration_loops[qbit_num], 1);
         }
@@ -1758,72 +1751,45 @@
         }
         else {
             max_inner_iterations_loc =max_inner_iterations;
         }
 
 
         // do the optimization loops
-        for (int idx=0; idx<iteration_loops_max; idx++) {
+        for (long long idx=0; idx<iteration_loops_max; idx++) {
 	    
-            long long iter = 0;
-            int status;
-
-            const gsl_multimin_fdfminimizer_type *T;
-            gsl_multimin_fdfminimizer *s;
 
-            N_Qubit_Decomposition_Base* par = this;
 
+            Problem p(num_of_parameters, 0, 2*M_PI, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
 
-            gsl_multimin_function_fdf my_func;
-
-
-            my_func.n = num_of_parameters;
-            my_func.f = optimization_problem;
-            my_func.df = optimization_problem_grad;
-            my_func.fdf = optimization_problem_combined;
-            my_func.params = par;
-
-
-            T = gsl_multimin_fdfminimizer_vector_bfgs2;
-            s = gsl_multimin_fdfminimizer_alloc (T, num_of_parameters);
-
-            gsl_multimin_fdfminimizer_set(s, &my_func, solution_guess_gsl, 0.01, 0.1);
-
-            do {
-                iter++;
-                number_of_iters++;
-                gsl_set_error_handler_off();
-                status = gsl_multimin_fdfminimizer_iterate (s);
-
-                if (status) {
-                  break;
-                }
-
-                status = gsl_multimin_test_gradient (s->gradient, gradient_threshold);
-
-            } while (status == GSL_CONTINUE && iter < max_inner_iterations_loc);
+            double f; 
+            if (num_of_parameters > 250) {
+                Lbfgs lbfgs(&p);
+                f = lbfgs.Solve(solution_guess);
+            } else {
+                Tolmin tolmin(&p);
+                f = tolmin.Solve(solution_guess, false, max_inner_iterations);
+            }
 
-            if (current_minimum > s->f) {
-                current_minimum = s->f;
-                memcpy( optimized_parameters_mtx.get_data(), s->x->data, num_of_parameters*sizeof(double) );
-                gsl_multimin_fdfminimizer_free (s);
 
+            if (current_minimum > f) {
+                current_minimum = f;
+                memcpy( optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
                 for ( int jdx=0; jdx<num_of_parameters; jdx++) {
-                    solution_guess_gsl->data[jdx] = solution_guess_gsl->data[jdx] + distrib_real(gen)/100;
+                    solution_guess[jdx] = solution_guess[jdx] + distrib_real(gen)/100;
                 }
             }
             else {
                 for ( int jdx=0; jdx<num_of_parameters; jdx++) {
-                    solution_guess_gsl->data[jdx] = solution_guess_gsl->data[jdx] + distrib_real(gen);
+                    solution_guess[jdx] = solution_guess[jdx] + distrib_real(gen);
                 }
-                gsl_multimin_fdfminimizer_free (s);
             }
 
 #ifdef __MPI__        
-            MPI_Bcast( (void*)solution_guess_gsl->data, num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+            MPI_Bcast( (void*)solution_guess.get_data(), num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif
 
 
 
         }
 
 }
@@ -1831,37 +1797,37 @@
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via BFGS algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_BFGS2( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void N_Qubit_Decomposition_Base::solve_layer_optimization_problem_BFGS2( int num_of_parameters, Matrix_real solution_guess) {
 
 
 #ifdef __DFE__
         if ( qbit_num >= 2 && get_accelerator_num() > 0 ) {
             upload_Umtx_to_DFE();
         }
 #endif
 
 
         if (gates.size() == 0 ) {
             return;
         }
 
 
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
         }
 
 
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
         // maximal number of iteration loops
         int iteration_loops_max;
         try {
             iteration_loops_max = std::max(iteration_loops[qbit_num], 1);
         }
@@ -1907,148 +1873,79 @@
         }
 
         std::stringstream sstream;
         sstream << "max_inner_iterations: " << max_inner_iterations_loc << ", randomization threshold: " << iteration_threshold_of_randomization_loc << std::endl;
         print(sstream, 2); 
 
         // do the optimization loops
-        for (long long idx=0; idx<iteration_loops_max; idx++) {
-
-            long long iter_idx = 0;
-            int status = GSL_CONTINUE;
-
-            const gsl_multimin_fdfminimizer_type *T;
-            gsl_multimin_fdfminimizer *s;
-
-            N_Qubit_Decomposition_Base* par = this;
-
-
-            gsl_multimin_function_fdf my_func;
-
-
-            my_func.n = num_of_parameters;
-            my_func.f = optimization_problem;
-            my_func.df = optimization_problem_grad;
-            my_func.fdf = optimization_problem_combined;
-            my_func.params = par;
-
+        double f = DBL_MAX;
+        for (long long iter_idx=0; iter_idx<iteration_loops_max; iter_idx++) {
 
-            T = gsl_multimin_fdfminimizer_vector_bfgs2;
-            s = gsl_multimin_fdfminimizer_alloc (T, num_of_parameters);
-
-            gsl_multimin_fdfminimizer_set(s, &my_func, solution_guess_gsl, 0.01, 0.1);
-
-            do {
-                gsl_set_error_handler_off();
-                
-                if ( sub_iter_idx > iteration_threshold_of_randomization_loc || status != GSL_CONTINUE ) {
-
-                    
-                    sub_iter_idx = 0;
-                    random_shift_count++;
-                    current_minimum_hold = current_minimum;  
-
-                    // calculate the gradient norm
-                    gsl_vector* grad_gsl = gsl_vector_alloc(num_of_parameters);
-                    optimization_problem_grad( solution_guess_gsl, this, grad_gsl );
-                    double norm = 0.0;
-                    for ( int grad_idx=0; grad_idx<num_of_parameters; grad_idx++ ) {
-                        norm += grad_gsl->data[grad_idx]*grad_gsl->data[grad_idx];
-                    }
-                    norm = std::sqrt(norm);  
-                    gsl_vector_free( grad_gsl );
-
-
-                    std::stringstream sstream;
-                    sstream << "BFGS2: leaving local minimum " << s->f << ", gradient norm " << norm  << std::endl;                    
-                    print(sstream, 0);   
-                    
-                    Matrix_real solution_guess_gsl_mtx( solution_guess_gsl->data, solution_guess_gsl->size, 1 );
-                    randomize_parameters(optimized_parameters_mtx, solution_guess_gsl_mtx, s->f );    
+            
+                Problem p(num_of_parameters, 0, 2*M_PI, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
+                Tolmin tolmin(&p);
 
-#ifdef __MPI__        
-                    MPI_Bcast( (void*)solution_guess_gsl->data, num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
-#endif
-                    
-                    status = 0;    
-                    
-                    gsl_multimin_fdfminimizer_free (s);                     
-                    s = gsl_multimin_fdfminimizer_alloc (T, num_of_parameters);  
-                    gsl_multimin_fdfminimizer_set(s, &my_func, solution_guess_gsl, 0.01, 0.1);                             
-        
-                }
-                else {
-                    status = gsl_multimin_fdfminimizer_iterate (s);
-                }
-                                
-/*
-                if (status) {
-                  break;
-                }
-*/
-                status = gsl_multimin_test_gradient (s->gradient, gradient_threshold);
-                
+                f = tolmin.Solve(solution_guess, false, max_inner_iterations);             
                 
                 if (sub_iter_idx == 1 ) {
-                     current_minimum_hold = s->f;    
+                     current_minimum_hold = f;    
                 }
 
 
-                if (current_minimum_hold*0.95 > s->f || (current_minimum_hold*0.97 > s->f && s->f < 1e-3) ||  (current_minimum_hold*0.99 > s->f && s->f < 1e-4) ) {
+                if (current_minimum_hold*0.95 > f || (current_minimum_hold*0.97 > f && f < 1e-3) ||  (current_minimum_hold*0.99 > f && f < 1e-4) ) {
                      sub_iter_idx = 0;
-                     current_minimum_hold = s->f;        
+                     current_minimum_hold = f;        
                 }
     
     
-                if (current_minimum > s->f ) {
-                     current_minimum = s->f;
-                     memcpy( optimized_parameters_mtx.get_data(),  s->x->data, num_of_parameters*sizeof(double) );
+                if (current_minimum > f ) {
+                     current_minimum = f;
+                     memcpy( optimized_parameters_mtx.get_data(),  solution_guess.get_data(), num_of_parameters*sizeof(double) );
                 }
     
 
                 if ( iter_idx % 5000 == 0 ) {
                      std::stringstream sstream;
                      sstream << "BFGS2: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100 << "\%, current minimum:" << current_minimum << std::endl;
                      print(sstream, 2);  
 
                      std::string filename("initial_circuit_iteration.binary");
                      export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
                 }
 
 
-                if (s->f < optimization_tolerance || random_shift_count > random_shift_count_max ) {
+                if (f < optimization_tolerance || random_shift_count > random_shift_count_max ) {
                     break;
                 }
 
 
                 sub_iter_idx++;
                 iter_idx++;
                 number_of_iters++;
 
-            } while (iter_idx < max_inner_iterations_loc && s->f > optimization_tolerance);
+        
 
-            if (current_minimum > s->f) {
-                current_minimum = s->f;
-                memcpy( optimized_parameters_mtx.get_data(), s->x->data, num_of_parameters*sizeof(double) );                
+            if (current_minimum > f) {
+                current_minimum = f;
+                memcpy( optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );                
 
                 for ( int jdx=0; jdx<num_of_parameters; jdx++) {
-                    solution_guess_gsl->data[jdx] = optimized_parameters_mtx[jdx] + distrib_real(gen)*2*M_PI/100;
+                    solution_guess[jdx] = optimized_parameters_mtx[jdx] + distrib_real(gen)*2*M_PI/100;
                 }
             }
             else {
                 for ( int jdx=0; jdx<num_of_parameters; jdx++) {
-                    solution_guess_gsl->data[jdx] = optimized_parameters_mtx[jdx] + distrib_real(gen)*2*M_PI;
+                    solution_guess[jdx] = optimized_parameters_mtx[jdx] + distrib_real(gen)*2*M_PI;
                 }
             }
 
 #ifdef __MPI__        
-            MPI_Bcast( (void*)solution_guess_gsl->data, num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+            MPI_Bcast( (void*)solution_guess.get_data(), num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif
             
-            gsl_multimin_fdfminimizer_free (s);
             
             if (current_minimum < optimization_tolerance ) {
                 break;
             }
 
 
 
@@ -2214,17 +2111,36 @@
         calcqgdKernelDFE( Umtx.rows, Umtx.cols, DFEgates, gatesNum, gateSetNum, trace_offset, trace_DFE_mtx.get_data() );
         unlock_lib();    
                                                                       
 #endif  
 pure_DFE_time += (tbb::tick_count::now() - t0_DFE_pure).seconds();       
 
         // calculate the cost function
-        for ( int idx=0; idx<parameters_vec.size(); idx++ ) {
-            cost_fnc_mtx[idx] = 1-trace_DFE_mtx[idx*3]/Umtx.cols;
+        if ( cost_fnc == FROBENIUS_NORM ) {
+            for ( int idx=0; idx<parameters_vec.size(); idx++ ) {
+                cost_fnc_mtx[idx] = 1-trace_DFE_mtx[idx*3]/Umtx.cols;
+            }
         }
+        else if ( cost_fnc == FROBENIUS_NORM_CORRECTION1 ) {
+            for ( int idx=0; idx<parameters_vec.size(); idx++ ) {
+                cost_fnc_mtx[idx] = 1-(trace_DFE_mtx[idx*3] + std::sqrt(prev_cost_fnv_val)*trace_DFE_mtx[idx*3+1]*correction1_scale)/Umtx.cols;
+            }
+        }
+        else if ( cost_fnc == FROBENIUS_NORM_CORRECTION2 ) {
+            for ( int idx=0; idx<parameters_vec.size(); idx++ ) {
+                cost_fnc_mtx[idx] = 1-(trace_DFE_mtx[idx*3] + std::sqrt(prev_cost_fnv_val)*(trace_DFE_mtx[idx*3+1]*correction1_scale + trace_DFE_mtx[idx*3+2]*correction2_scale))/Umtx.cols;
+            }
+        }
+        else {
+            std::string err("N_Qubit_Decomposition_Base::optimization_problem_batched: Cost function variant not implmented.");
+            throw err;
+        }
+
+
+       
 
 
         delete[] DFEgates;
 
     }
     else{
 
@@ -2244,30 +2160,32 @@
 
 DFE_time += (tbb::tick_count::now() - t0_DFE).seconds();       
     return cost_fnc_mtx;
         
 }
 
 
+
+
+
 /**
 // @brief The optimization problem of the final optimization
-@param parameters A GNU Scientific Library containing the parameters to be optimized.
+@param parameters Array containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param ret_temp A matrix to store trace in for gradient for HS test 
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
-double N_Qubit_Decomposition_Base::optimization_problem( const gsl_vector* parameters, void* void_instance, Matrix ret_temp) {
+double N_Qubit_Decomposition_Base::optimization_problem( Matrix_real parameters, void* void_instance, Matrix ret_temp) {
 
     N_Qubit_Decomposition_Base* instance = reinterpret_cast<N_Qubit_Decomposition_Base*>(void_instance);
     std::vector<Gate*> gates_loc = instance->get_gates();
 
     // get the transformed matrix with the gates in the list
     Matrix Umtx_loc = instance->get_Umtx();
-    Matrix_real parameters_mtx(parameters->data, 1, instance->get_parameter_num() );
-    Matrix matrix_new = instance->get_transformed_matrix( parameters_mtx, gates_loc.begin(), gates_loc.size(), Umtx_loc );
+    Matrix matrix_new = instance->get_transformed_matrix( parameters, gates_loc.begin(), gates_loc.size(), Umtx_loc );
 
   
     cost_function_type cost_fnc = instance->get_cost_function_variant();
 
     if ( cost_fnc == FROBENIUS_NORM ) {
         return get_cost_function(matrix_new, instance->get_trace_offset());
     }
@@ -2311,105 +2229,66 @@
         std::string err("N_Qubit_Decomposition_Base::optimization_problem: Cost function variant not implmented.");
         throw err;
     }
 
 
 }
 
+
+
 /**
 // @brief The optimization problem of the final optimization
-@param parameters A GNU Scientific Library containing the parameters to be optimized.
+@param parameters Array containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
-double N_Qubit_Decomposition_Base::optimization_problem( const gsl_vector* parameters, void* void_instance) {
+double N_Qubit_Decomposition_Base::optimization_problem( Matrix_real parameters, void* void_instance) {
+
     N_Qubit_Decomposition_Base* instance = reinterpret_cast<N_Qubit_Decomposition_Base*>(void_instance);
     Matrix ret(1,3);
     double cost_func = instance->optimization_problem(parameters, void_instance, ret);
     return cost_func;
 }
 
-Matrix_real N_Qubit_Decomposition_Base::optimization_problem_batch( int batchsize, const gsl_vector* parameters, void* void_instance) {
-    N_Qubit_Decomposition_Base* instance = reinterpret_cast<N_Qubit_Decomposition_Base*>(void_instance);
-    Matrix_real costs(batchsize,1);
-    // the number of free parameters
-    int parameter_num_loc = instance->get_parameter_num();
-#ifdef __DFE__
-    if ( instance->qbit_num >= 2 && instance->get_accelerator_num() > 0 ) {
-        int trace_offset_loc = instance->get_trace_offset();
-        // the variant of the cost function
-        cost_function_type cost_fnc = instance->get_cost_function_variant();
-    
-        // value of the cost function from the previous iteration to weigth the correction to the trace
-        double prev_cost_fnv_val = instance->get_previous_cost_function_value();
-        double correction1_scale    = instance->get_correction1_scale();
-        double correction2_scale    = instance->get_correction2_scale();    
-        Matrix&& Umtx_loc = instance->get_Umtx();
-        Matrix_real trace_DFE_mtx(batchsize, 3);
-        int gatesNum;
-        Matrix_real parameters_mtx(parameters->data, 1, parameters->size);
-        DFEgate_kernel_type* DFEgates = instance->convert_to_DFE_gates( parameters_mtx, gatesNum);
-        lock_lib();
-        calcqgdKernelDFE( Umtx_loc.rows, Umtx_loc.cols, DFEgates, parameter_num_loc, batchsize, trace_offset_loc, trace_DFE_mtx.get_data() );
-        unlock_lib();
-        for (int idx=0; idx<batchsize; idx++) {
-            if ( cost_fnc == FROBENIUS_NORM ) {
-                costs[idx] = 1-trace_DFE_mtx[3*idx]/Umtx_loc.cols;
-            } else if ( cost_fnc == FROBENIUS_NORM_CORRECTION1 ) {
-                costs[idx] = 1 - (trace_DFE_mtx[3*idx] + 0*std::sqrt(prev_cost_fnv_val)*trace_DFE_mtx[3*idx+1]*correction1_scale)/Umtx_loc.cols;
-            }
-            else if ( cost_fnc == FROBENIUS_NORM_CORRECTION2 ) {
-                costs[idx] = 1 - (trace_DFE_mtx[3*idx] + std::sqrt(prev_cost_fnv_val)*(trace_DFE_mtx[3*idx+1]*correction1_scale + trace_DFE_mtx[3*idx+2]*correction2_scale))/Umtx_loc.cols;
-            }
-            else {
-                std::string err("N_Qubit_Decomposition_Base::optimization_problem_batch: Cost function variant not implmented.");
-                throw err;
-            }
-        }
-    } else {
-#else
-    tbb::parallel_for( tbb::blocked_range<int>(0,batchsize,2), [&](tbb::blocked_range<int> r) {
-        Matrix ret(batchsize,3);
-        for (int idx=r.begin(); idx<r.end(); ++idx) {
-            gsl_vector_view view = gsl_vector_subvector(parameters, parameter_num_loc * idx, parameter_num_loc);
-            costs[idx] = instance->optimization_problem(&view.vector, void_instance, ret);
-        }
-    });
-#endif
-#ifdef __DFE__
-    }
-#endif
-    return costs;
-}
+
+
+
+
+
+
+
 
 /**
 @brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
-@param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
+@param parameters Array containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
-@param grad A GNU Scientific Library vector containing the calculated gradient components.
+@param grad Array containing the calculated gradient components.
 */
-void N_Qubit_Decomposition_Base::optimization_problem_grad( const gsl_vector* parameters, void* void_instance, gsl_vector* grad ) {
+void N_Qubit_Decomposition_Base::optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real& grad ) {
 
     // The function value at x0
     double f0;
 
     // calculate the approximate gradient
     optimization_problem_combined( parameters, void_instance, &f0, grad);
 
 }
 
 
+
+
+
 /**
 @brief Call to calculate both the cost function and the its gradient components.
-@param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
+@param parameters Array containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
-@param grad A GNU Scientific Library vector containing the calculated gradient components.
+@param grad Array containing the calculated gradient components.
 */
-void N_Qubit_Decomposition_Base::optimization_problem_combined( const gsl_vector* parameters, void* void_instance, double* f0, gsl_vector* grad ) {
+void N_Qubit_Decomposition_Base::optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad ) {
 
     N_Qubit_Decomposition_Base* instance = reinterpret_cast<N_Qubit_Decomposition_Base*>(void_instance);
 
     // the number of free parameters
     int parameter_num_loc = instance->get_parameter_num();
 
     // the variant of the cost function
@@ -2425,18 +2304,17 @@
 
 #ifdef __DFE__
 
 ///////////////////////////////////////
 //std::cout << "number of qubits: " << instance->qbit_num << std::endl;
 //tbb::tick_count t0_DFE = tbb::tick_count::now();/////////////////////////////////    
 if ( instance->qbit_num >= 5 && instance->get_accelerator_num() > 0 ) {
-    Matrix_real parameters_mtx(parameters->data, 1, parameters->size);
 
     int gatesNum, redundantGateSets, gateSetNum;
-    DFEgate_kernel_type* DFEgates = instance->convert_to_DFE_gates_with_derivates( parameters_mtx, gatesNum, gateSetNum, redundantGateSets );
+    DFEgate_kernel_type* DFEgates = instance->convert_to_DFE_gates_with_derivates( parameters, gatesNum, gateSetNum, redundantGateSets );
 
     Matrix&& Umtx_loc = instance->get_Umtx();   
     Matrix_real trace_DFE_mtx(gateSetNum, 3);
 
 
 #ifdef __MPI__
     // the number of decomposing layers are divided between the MPI processes
@@ -2466,15 +2344,15 @@
     instance->print(sstream, 5);	
     
   
     if ( cost_fnc == FROBENIUS_NORM ) {
         *f0 = 1-trace_DFE_mtx[0]/Umtx_loc.cols;
     }
     else if ( cost_fnc == FROBENIUS_NORM_CORRECTION1 ) {
-        *f0 = 1 - (trace_DFE_mtx[0] + 0*std::sqrt(prev_cost_fnv_val)*trace_DFE_mtx[1]*correction1_scale)/Umtx_loc.cols;
+        *f0 = 1 - (trace_DFE_mtx[0] + std::sqrt(prev_cost_fnv_val)*trace_DFE_mtx[1]*correction1_scale)/Umtx_loc.cols;
     }
     else if ( cost_fnc == FROBENIUS_NORM_CORRECTION2 ) {
         *f0 = 1 - (trace_DFE_mtx[0] + std::sqrt(prev_cost_fnv_val)*(trace_DFE_mtx[1]*correction1_scale + trace_DFE_mtx[2]*correction2_scale))/Umtx_loc.cols;
     }
     else {
         std::string err("N_Qubit_Decomposition_Base::optimization_problem_combined: Cost function variant not implmented.");
         throw err;
@@ -2528,16 +2406,15 @@
 
     tbb::parallel_invoke(
         [&]{
             *f0 = instance->optimization_problem(parameters, reinterpret_cast<void*>(instance), trace_tmp); 
         },
         [&]{
             Matrix&& Umtx_loc = instance->get_Umtx();   
-            Matrix_real parameters_mtx(parameters->data, 1, parameters->size);
-            Umtx_deriv = instance->apply_derivate_to( parameters_mtx, Umtx_loc );
+            Umtx_deriv = instance->apply_derivate_to( parameters, Umtx_loc );
         });
 
 
 
 
     tbb::parallel_for( tbb::blocked_range<int>(0,parameter_num_loc,2), [&](tbb::blocked_range<int> r) {
         for (int idx=r.begin(); idx<r.end(); ++idx) { 
@@ -2573,168 +2450,76 @@
                 grad_comp = get_cost_function_sum_of_squares(Umtx_deriv[idx]);
             }
             else {
                 std::string err("N_Qubit_Decomposition_Base::optimization_problem_combined: Cost function variant not implmented.");
                 throw err;
             }
             
-//            grad->data[idx] = grad_comp;
-            gsl_vector_set(grad, idx, grad_comp);
+            grad[idx] = grad_comp;
 
 
 
         }
     });
 
     std::stringstream sstream;
     sstream << *f0 << std::endl;
     instance->print(sstream, 5);	
 
 #ifdef __DFE__
 }
+#endif
 
-/*
-tbb::tick_count t1_CPU = tbb::tick_count::now();/////////////////////////////////
-std::cout << "time elapsed CPU: " << (t1_CPU-t0_CPU).seconds() << " number of parameters: " << parameter_num_loc << std::endl;
-std::cout << "cost function CPU: " << *f0 << " and DFE: " << f0_DFE << std::endl;
-
-for ( int idx=0; idx<parameter_num_loc; idx++ ) {
-
-    double diff = std::sqrt((grad_components_DFE_mtx[idx]-gsl_vector_get(grad, idx))*(grad_components_DFE_mtx[idx]-gsl_vector_get(grad, idx)));
-    if ( diff > 1e-5 ) {
-        std::cout << "DFE and CPU cost functions differs at index " << idx << " " <<  grad_components_DFE_mtx[idx] << " and " <<  gsl_vector_get(grad, idx) << std::endl;
-        
-    }   
 
 }
 
 
 
-std::cout << "N_Qubit_Decomposition_Base::optimization_problem_combined" << std::endl;
-std::string error("N_Qubit_Decomposition_Base::optimization_problem_combined");
-        throw error;
+/**
+@brief Call to calculate both the cost function and the its gradient components.
+@param parameters Array containing the free parameters to be optimized.
+@param void_instance A void pointer pointing to the instance of the current class.
+@param f0 The value of the cost function at x0.
+@param grad Array containing the calculated gradient components.
 */
-#endif
+void N_Qubit_Decomposition_Base::optimization_problem_combined( Matrix_real parameters, double* f0, Matrix_real grad ) {
 
-/*
+    optimization_problem_combined( parameters, this, f0, grad );
+    return;
+}
 
-    // adjust gradient components corresponding to adaptive gates
-    for (int idx=3*qbit_num; idx<parameter_num_loc; idx=idx+7 ) {
-        double grad_comp = gsl_vector_get(grad, idx);
-        grad_comp = grad_comp * std::sin( parameters->data[idx])*0.5*M_PI;
-        gsl_vector_set(grad, idx, grad_comp);
-    }
-*/
 
-}
 
-void N_Qubit_Decomposition_Base::optimization_problem_combined_unitary( const gsl_vector* parameters, void* void_instance, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv ) {
+/**
+@brief ?????????????
+*/
+void N_Qubit_Decomposition_Base::optimization_problem_combined_unitary( Matrix_real parameters, void* void_instance, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv ) {
     // vector containing gradients of the transformed matrix
     N_Qubit_Decomposition_Base* instance = reinterpret_cast<N_Qubit_Decomposition_Base*>(void_instance);
 
     tbb::parallel_invoke(
         [&]{
             Matrix Umtx_loc = instance->get_Umtx();
-            Matrix_real parameters_mtx(parameters->data, 1, parameters->size);
-            Umtx = instance->get_transformed_matrix( parameters_mtx, instance->gates.begin(), instance->gates.size(), Umtx_loc );
+            Umtx = instance->get_transformed_matrix( parameters, instance->gates.begin(), instance->gates.size(), Umtx_loc );
         },
         [&]{
             Matrix Umtx_loc = instance->get_Umtx();
-            Matrix_real parameters_mtx(parameters->data, 1, parameters->size);
-            Umtx_deriv = instance->apply_derivate_to( parameters_mtx, Umtx_loc );
+            Umtx_deriv = instance->apply_derivate_to( parameters, Umtx_loc );
         });
 }
 
+
 /**
-@brief Call to calculate both the cost function and the its gradient components.
-@param parameters The parameters for which the cost fuction shoule be calculated
-@param f0 The value of the cost function at x0.
-@param grad An array storing the calculated gradient components
+@brief ?????????????
 */
-void N_Qubit_Decomposition_Base::optimization_problem_combined( const Matrix_real& parameters, double* f0, Matrix_real& grad ) {
-
-#ifdef __DFE__
-
-    lock_lib();
-
-    if ( get_accelerator_num() > 0 && get_initialize_id() != id ) {
-        std::string err("The uploaded unitary to the DFE might not be identical to the unitary stored by this specific class instance. Please upload the unitary to DFE by the Upload_Umtx_to_DFE() method.");
-        throw err;
-    }
+void N_Qubit_Decomposition_Base::optimization_problem_combined_unitary( Matrix_real parameters, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv ) {
 
-#endif
-
-    // create GSL wrappers around the pointers
-    gsl_block block_tmp;
-    block_tmp.data = parameters.get_data();
-    block_tmp.size = parameters.size(); 
-
-    gsl_vector parameters_gsl;
-    parameters_gsl.data = parameters.get_data();
-    parameters_gsl.size = parameters.size();
-    parameters_gsl.stride = 1;   
-    parameters_gsl.block = &block_tmp; 
-    parameters_gsl.owner = 0; 
-    
-    
-    gsl_block block_tmp2;
-    block_tmp.data = grad.get_data();
-    block_tmp.size = grad.size();        
-
-    gsl_vector grad_gsl;
-    grad_gsl.data = grad.get_data();
-    grad_gsl.size = grad.size();
-    grad_gsl.stride = 1;   
-    grad_gsl.block = &block_tmp2; 
-    grad_gsl.owner = 0;    
-
-    // call the method to calculate the cost function and the gradients
-    optimization_problem_combined( &parameters_gsl, this, f0, &grad_gsl );
-
-#ifdef __DFE__
-    unlock_lib();
-#endif
-
-}
-
-void N_Qubit_Decomposition_Base::optimization_problem_combined_unitary( const Matrix_real& parameters, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv ) {
-
-    // create GSL wrappers around the pointers
-    gsl_block block_tmp;
-    block_tmp.data = parameters.get_data();
-    block_tmp.size = parameters.size(); 
-
-    gsl_vector parameters_gsl;
-    parameters_gsl.data = parameters.get_data();
-    parameters_gsl.size = parameters.size();
-    parameters_gsl.stride = 1;   
-    parameters_gsl.block = &block_tmp; 
-    parameters_gsl.owner = 0; 
-
-    // call the method to calculate the cost function and the gradients
-    optimization_problem_combined_unitary( &parameters_gsl, this, Umtx, Umtx_deriv );
-
-}
-
-Matrix_real N_Qubit_Decomposition_Base::optimization_problem_batch( Matrix_real parameters )
-{
-    // create GSL wrappers around the pointers
-    gsl_block block_tmp;
-    block_tmp.data = parameters.get_data();
-    block_tmp.size = parameters.size(); 
-
-    gsl_vector parameters_gsl;
-    parameters_gsl.data = parameters.get_data();
-    parameters_gsl.size = parameters.size();
-    parameters_gsl.stride = 1; //assert parameters.cols == parameters.stride == get_num_parameters()...   
-    parameters_gsl.block = &block_tmp; 
-    parameters_gsl.owner = 0; 
+    optimization_problem_combined_unitary( parameters, this, Umtx, Umtx_deriv);
+    return;
     
-    Matrix_real result = optimization_problem_batch(parameters.rows, &parameters_gsl, this);
-    return result;
 }
 
 
 /**
 @brief Call to get the variant of the cost function used in the calculations
 */
 cost_function_type 
@@ -2824,16 +2609,16 @@
             max_inner_iterations = 2.5e3;
             random_shift_count_max = 3;
             gradient_threshold = 1e-8;
             max_outer_iterations = 1;
             return;
 
         case BFGS:
-            max_inner_iterations = 100;
-            gradient_threshold = 1e-1;
+            max_inner_iterations = 10000;
+            gradient_threshold = 1e-8;
             random_shift_count_max = 1;  
             max_outer_iterations = 1e8; 
             return;
 
         case BFGS2:
             max_inner_iterations = 1e5;
             random_shift_count_max = 100;
```

### Comparing `squander-1.8.0/decomposition/N_Qubit_Decomposition_Cost_Function.cpp` & `squander-1.8.1/decomposition/N_Qubit_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/N_Qubit_Decomposition_adaptive.cpp` & `squander-1.8.1/decomposition/N_Qubit_Decomposition_adaptive.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
     // BFGS is better for smaller problems, while ADAM for larger ones
     if ( qbit_num <= 5 ) {
         set_optimizer( BFGS );
 
         // Maximal number of iteartions in the optimization process
         max_outer_iterations = 4;
+        max_inner_iterations = 10000;
     }
     else {
         set_optimizer( ADAM );
 
         // Maximal number of iteartions in the optimization process
         max_outer_iterations = 1;
     }
@@ -148,29 +149,28 @@
 
     // BFGS is better for smaller problems, while ADAM for larger ones
     if ( qbit_num <= 5 ) {
         alg = BFGS;
 
         // Maximal number of iteartions in the optimization process
         max_outer_iterations = 4;
+        max_inner_iterations = 10000;
     }
     else {
         alg = ADAM;
 
         // Maximal number of iteartions in the optimization process
         max_outer_iterations = 1;
     }
 
     // Boolean variable to determine whether randomized adaptive layers are used or not
     randomized_adaptive_layers = false;
 
 }
 
-
-
 /**
 @brief Destructor of the class
 */
 N_Qubit_Decomposition_adaptive::~N_Qubit_Decomposition_adaptive() {
 
 }
 
@@ -2045,8 +2045,7 @@
 
 
 
 
 
 
 
-
```

### Comparing `squander-1.8.0/decomposition/N_Qubit_Decomposition_custom.cpp` & `squander-1.8.1/decomposition/N_Qubit_Decomposition_custom.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/Sub_Matrix_Decomposition.cpp` & `squander-1.8.1/decomposition/Sub_Matrix_Decomposition.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 /*! \file Sub_Matrix_Decomposition.cpp
     \brief Class responsible for the disentanglement of one qubit from the others.
 */
 
 #include "Sub_Matrix_Decomposition.h"
 #include "Sub_Matrix_Decomposition_Cost_Function.h"
 
+#include "tolmin.h"
+
 
 #ifdef __MPI__
 #include <mpi.h>
 #endif // MPI
 
 //tbb::spin_mutex my_mutex;
 
@@ -48,14 +50,16 @@
 
     // logical value indicating whether the quasi-unitarization of the submatrices was done or not
     subdisentaglement_done = false;
 
     // custom gate structure used in the decomposition
     unit_gate_structure = NULL;
 
+    max_inner_iterations = 100;
+
 }
 
 
 /**
 @brief Constructor of the class.
 @param Umtx_in The unitary matrix to be decomposed
 @param qbit_num_in The number of qubits spanning the unitary Umtx
@@ -86,14 +90,16 @@
             max_layer_num.insert( std::pair<int, int>(it->first,  it->second) );
         }
     }
 
     // custom gate structure used in the decomposition
     unit_gate_structure = NULL;
 
+    max_inner_iterations = 100;
+
 
 }
 
 
 /**
 @brief Destructor of the class
 */
@@ -177,15 +183,14 @@
                     qgd_free(optimized_parameters);
                     optimized_parameters = NULL;
                 }
 */
                 // solve the optimization problem to find the correct minimum
                 solve_optimization_problem( NULL, 0);
 
-
                 if (check_optimization_solution()) {
                     break;
                 }
             }
 
         }
 
@@ -400,112 +405,79 @@
 
 
 /**
 @brief Call to solve layer by layer the optimization problem. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void Sub_Matrix_Decomposition::solve_layer_optimization_problem( int num_of_parameters, gsl_vector *solution_guess_gsl) {
+void Sub_Matrix_Decomposition::solve_layer_optimization_problem( int num_of_parameters, Matrix_real solution_guess) {
 
 
         if (gates.size() == 0 ) {
             return;
         }
 
 
-        if (solution_guess_gsl == NULL) {
-            solution_guess_gsl = gsl_vector_alloc(num_of_parameters);
+        if (solution_guess.size() == 0 ) {
+            solution_guess = Matrix_real(num_of_parameters,1);
         }
-/*
-        if (optimized_parameters == NULL) {
-            optimized_parameters = (double*)qgd_calloc(num_of_parameters,sizeof(double), 64);
-            memcpy(optimized_parameters, solution_guess_gsl->data, num_of_parameters*sizeof(double) );
-        }
-*/
+
+
         if (optimized_parameters_mtx.size() == 0) {
             optimized_parameters_mtx = Matrix_real(1, num_of_parameters);
-            memcpy(optimized_parameters_mtx.get_data(), solution_guess_gsl->data, num_of_parameters*sizeof(double) );
+            memcpy(optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
         }
 
 
         // maximal number of iteration loops
         int iteration_loops_max;
         try {
             iteration_loops_max = std::max(iteration_loops[qbit_num], 1);
         }
         catch (...) {
             iteration_loops_max = 1;
         }
 
+        // maximal number of inner iterations overriden by config
+        long long max_inner_iterations_loc;
+        if ( config.count("max_inner_iterations") > 0 ) {
+            config["max_inner_iterations"].get_property( max_inner_iterations_loc );         
+        }
+        else {
+            max_inner_iterations_loc =max_inner_iterations;
+        }
+
         // random generator of real numbers   
         std::uniform_real_distribution<> distrib_real(0.0, 2*M_PI);
 
         // do the optimization loops
-        for (int idx=0; idx<iteration_loops_max; idx++) {
-
-            int iter = 0;
-            int status;
+        for (long long idx=0; idx<iteration_loops_max; idx++) {
 
-            const gsl_multimin_fdfminimizer_type *T;
-            gsl_multimin_fdfminimizer *s;
+            Problem p(num_of_parameters, 0, 2*M_PI, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
+            Tolmin tolmin(&p);
 
-            Sub_Matrix_Decomposition* par = this;
+            Matrix_real x(solution_guess.get_data(), num_of_parameters, 1); 
 
+            double f = tolmin.Solve(x, false, max_inner_iterations);
 
-            gsl_multimin_function_fdf my_func;
-
-
-            my_func.n = num_of_parameters;
-            my_func.f = optimization_problem;
-            my_func.df = optimization_problem_grad;
-            my_func.fdf = optimization_problem_combined;
-            my_func.params = par;
-
-
-            T = gsl_multimin_fdfminimizer_vector_bfgs2;
-            s = gsl_multimin_fdfminimizer_alloc (T, num_of_parameters);
-
-
-            gsl_multimin_fdfminimizer_set (s, &my_func, solution_guess_gsl, 0.1, 0.1);
-
-            do {
-                iter++;
-
-                status = gsl_multimin_fdfminimizer_iterate (s);
-
-                if (status) {
-                  break;
-                }
-
-                status = gsl_multimin_test_gradient (s->gradient, 1e-1);
-                /*if (status == GSL_SUCCESS) {
-                    printf ("Minimum found\n");
-                }*/
-
-            } while (status == GSL_CONTINUE && iter < 100);
-
-            if (current_minimum > s->f) {
-                current_minimum = s->f;
-                memcpy( optimized_parameters_mtx.get_data(), s->x->data, num_of_parameters*sizeof(double) );
-                gsl_multimin_fdfminimizer_free (s);
-
+            if (current_minimum > f) {
+                current_minimum = f;
+                memcpy( optimized_parameters_mtx.get_data(), solution_guess.get_data(), num_of_parameters*sizeof(double) );
                 for ( int jdx=0; jdx<num_of_parameters; jdx++) {
-                    solution_guess_gsl->data[jdx] = solution_guess_gsl->data[jdx] + distrib_real(gen)/100;
+                    solution_guess[jdx] = solution_guess[jdx] + distrib_real(gen)/100;
                 }
             }
             else {
                 for ( int jdx=0; jdx<num_of_parameters; jdx++) {
-                    solution_guess_gsl->data[jdx] = solution_guess_gsl->data[jdx] + distrib_real(gen);
+                    solution_guess[jdx] = solution_guess[jdx] + distrib_real(gen);
                 }
-
-                gsl_multimin_fdfminimizer_free (s);
             }
 
 #ifdef __MPI__        
-            MPI_Bcast( (void*)solution_guess_gsl->data, num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+            MPI_Bcast( (void*)solution_guess.get_data(), num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif
 
 
 
         }
 
 
@@ -542,27 +514,26 @@
 
 /**
 @brief The optimization problem of the final optimization
 @param parameters A GNU Scientific Library containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @return Returns with the cost function. (zero if the qubits are disentangled.)
 */
-double Sub_Matrix_Decomposition::optimization_problem( const gsl_vector* parameters, void* void_instance ) {
+double Sub_Matrix_Decomposition::optimization_problem( Matrix_real parameters, void* void_instance ) {
 
     Sub_Matrix_Decomposition* instance = reinterpret_cast<Sub_Matrix_Decomposition*>(void_instance);
     std::vector<Gate*> gates_loc = instance->get_gates();
 
     Matrix Umtx_loc, matrix_new;
 
 //{
 //tbb::spin_mutex::scoped_lock my_lock{my_mutex};
 
     Umtx_loc = instance->get_Umtx();
-    Matrix_real parameters_mtx(parameters->data, 1, instance->get_parameter_num() );
-    matrix_new = instance->get_transformed_matrix( parameters_mtx, gates_loc.begin(), gates_loc.size(), Umtx_loc );
+    matrix_new = instance->get_transformed_matrix( parameters, gates_loc.begin(), gates_loc.size(), Umtx_loc );
 
 #ifdef DEBUG
         if (matrix_new.isnan()) {
            std::stringstream sstream;
 	   sstream << "Sub_Matrix_Decomposition::optimization_problem matrix_new contains NaN b." << std::endl;
 	   print(sstream, 1);	 
         }
@@ -583,15 +554,15 @@
 
 /**
 @brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-void Sub_Matrix_Decomposition::optimization_problem_grad( const gsl_vector* parameters, void* void_instance, gsl_vector* grad ) {
+void Sub_Matrix_Decomposition::optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real grad ) {
 
     // The function value at x0
     double f0;
 
     // calculate the approximate gradient
     optimization_problem_combined( parameters, void_instance, &f0, grad);
 
@@ -602,45 +573,40 @@
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-void Sub_Matrix_Decomposition::optimization_problem_combined( const gsl_vector* parameters, void* void_instance, double* f0, gsl_vector* grad ) {
+void Sub_Matrix_Decomposition::optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad ) {
 
     Sub_Matrix_Decomposition* instance = reinterpret_cast<Sub_Matrix_Decomposition*>(void_instance);
 
     int parameter_num_loc = instance->get_parameter_num();
 
     // storage for the function values calculated at the displaced points x
-    gsl_vector* f = gsl_vector_alloc(grad->size);
+    Matrix_real f(1, grad.size());
 
     // the difference in one direction in the parameter for the gradient calculation
     double dparam = 1e-8;
 
     // calculate the function values at displaced x and the central x0 points through TBB parallel for
     tbb::parallel_for(0, parameter_num_loc+1, 1, [&](int i) {
 
-        if (i == (int)parameters->size) {
+        if (i == (int)parameters.size()) {
             // calculate function value at x0
             *f0 = instance->optimization_problem(parameters, reinterpret_cast<void*>(instance));
         }
         else {
 
-            gsl_vector* parameters_d = gsl_vector_calloc(parameters->size);
-            memcpy( parameters_d->data, parameters->data, parameters->size*sizeof(double) );
-            parameters_d->data[i] = parameters_d->data[i] + dparam;
+            Matrix_real parameters_d = parameters.copy();
+            parameters_d[i] = parameters_d[i] + dparam;
 
             // calculate the cost function at the displaced point
-            f->data[i] = instance->optimization_problem(parameters_d, reinterpret_cast<void*>(instance));
-
-            // release vectors
-            gsl_vector_free(parameters_d);
-            parameters_d = NULL;
+            f[i] = instance->optimization_problem(parameters_d, reinterpret_cast<void*>(instance));
 
         }
     });
 
 
 /*
     // sequential version
@@ -657,19 +623,18 @@
 #ifdef DEBUG
         if (isnan(f->data[idx])) {
 	  sstream << "Sub_Matrix_Decomposition::optimization_problem_combined: f->data[i] is NaN " << std::endl;
 	  print(sstream, 0);	  
           exit(-1);
         }
 #endif // DEBUG
-        gsl_vector_set(grad, idx, (f->data[idx]-(*f0))/dparam);
+        grad[idx] = (f[idx]-(*f0))/dparam;
     }
 
 
-    gsl_vector_free(f);
 
 }
```

### Comparing `squander-1.8.0/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp` & `squander-1.8.1/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/include/Decomposition_Base.h` & `squander-1.8.1/decomposition/include/Decomposition_Base.h`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 #include "ON.h"
 #include "Adaptive.h"
 #include "Composite.h"
 #include <map>
 #include <cstdlib>
 #include <time.h>
 #include <ctime>
-#include "gsl/gsl_multimin.h"
-#include "gsl/gsl_statistics.h"
+#include <cfloat>
+#include <limits>
 #include <tbb/cache_aligned_allocator.h>
 
 #include "config_element.h"
 
 #include <random>
 
 /// @brief Type definition of the types of the initial guess
@@ -202,20 +202,21 @@
 /**
 @brief This method can be used to solve the main optimization problem which is devidid into sub-layer optimization processes. (The aim of the optimization problem is to disentangle one or more qubits) The optimalized parameters are stored in attribute optimized_parameters.
 @param solution_guess An array of the guessed parameters
 @param solution_guess_num The number of guessed parameters. (not necessarily equal to the number of free parameters)
 */
 void solve_optimization_problem( double* solution_guess, int solution_guess_num );
 
+
 /**
 @brief Abstarct function to be used to solve a single sub-layer optimization problem. The optimalized parameters are stored in attribute optimized_parameters.
 @param 'num_of_parameters' The number of free parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Libarary vector containing the free parameters to be optimized.
+@param solution_guess_gsl Array containing the free parameters to be optimized.
 */
-virtual void solve_layer_optimization_problem( int num_of_parameters, gsl_vector *solution_guess_gsl);
+virtual void solve_layer_optimization_problem( int num_of_parameters, Matrix_real solution_guess_gsl);
 
 
 
 /**
 @brief This is an abstact definition of function giving the cost functions measuring the entaglement of the qubits. When the qubits are indepent, teh cost function should be zero.
 @param parameters An array of the free parameters to be optimized. (The number of the free paramaters should be equal to the number of parameters in one sub-layer)
 */
```

### Comparing `squander-1.8.0/decomposition/include/N_Qubit_Decomposition.h` & `squander-1.8.1/decomposition/include/N_Qubit_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/include/N_Qubit_Decomposition_Base.h` & `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Base.h`

 * *Files 3% similar despite different names*

```diff
@@ -168,76 +168,78 @@
 
 
 /**
 @brief final optimization procedure improving the accuracy of the decompositin when all the qubits were already disentangled.
 */
 void final_optimization();
 
+
+
 /**
 @brief Call to solve layer by layer the optimization problem via calling one of the implemented algorithms. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
-@param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
+@param solution_guess Array containing the solution guess.
 */
-void solve_layer_optimization_problem( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem( int num_of_parameters, Matrix_real solution_guess);
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the COSINE algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_COSINE( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_COSINE( int num_of_parameters, Matrix_real& solution_guess_gsl);
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the AGENT algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_AGENTS( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_AGENTS( int num_of_parameters, Matrix_real& solution_guess_gsl);
 
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via the AGENT COMBINED algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_AGENTS_COMBINED( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_AGENTS_COMBINED( int num_of_parameters, Matrix_real& solution_guess_gsl);
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via BBFG algorithm. (optimal for smaller problems) The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_BFGS( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_BFGS( int num_of_parameters, Matrix_real& solution_guess_gsl);
 
 
 
 /**
 @brief Call to solve layer by layer the optimization problem via BBFG algorithm. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_BFGS2( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_BFGS2( int num_of_parameters, Matrix_real solution_guess);
 
 /**
 @brief Call to solve layer by layer the optimization problem via batched ADAM algorithm. (optimal for larger problems) The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_ADAM_BATCHED( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_ADAM_BATCHED( int num_of_parameters, Matrix_real& solution_guess_gsl);
 
 /**
 @brief Call to solve layer by layer the optimization problem via ADAM algorithm. (optimal for larger problems) The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem_ADAM( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem_ADAM( int num_of_parameters, Matrix_real& solution_guess_gsl);
 
 /**
 @brief ?????????????
 */
 void randomize_parameters( Matrix_real& input, Matrix_real& output, const double& f0 );
 
 /**
@@ -260,75 +262,80 @@
 @brief The optimization problem of the final optimization with batched input (implemented only for the Frobenius norm cost function)
 @param parameters An array of the free parameters to be optimized. (The number of teh free paramaters should be equal to the number of parameters in one sub-layer)
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
 Matrix_real optimization_problem_batched( std::vector<Matrix_real>& parameters_vec);
 
 
+
 /**
-@brief The optimization problem of the final optimization useful for gradient
-@param parameters A GNU Scientific Library containing the parameters to be optimized.
+// @brief The optimization problem of the final optimization
+@param parameters Array containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
-@param ret_temp A matrix to store trace in for gradient
+@param ret_temp A matrix to store trace in for gradient for HS test 
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
-double optimization_problem( const gsl_vector* parameters, void* void_instance, Matrix ret_temp );
+double optimization_problem( Matrix_real parameters, void* void_instance, Matrix ret_temp);
 
 
 /**
-@brief The optimization problem of the final optimization
-@param parameters A GNU Scientific Library containing the parameters to be optimized.
+// @brief The optimization problem of the final optimization
+@param parameters Array containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
-static double optimization_problem( const gsl_vector* parameters, void* void_instance );
+static double optimization_problem( Matrix_real parameters, void* void_instance);
 
 
 /**
-@brief The optimization problem of the final optimization
-@param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
+@brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
+@param parameters Array containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
-@param grad A GNU Scientific Library vector containing the calculated gradient components.
+@param grad Array containing the calculated gradient components.
 */
-static Matrix_real optimization_problem_batch( int batchsize, const gsl_vector* parameters, void* void_instance );
+static void N_Qubit_Decomposition_Base::optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real& grad );
+
 
 
 /**
-@brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
+@brief Call to calculate both the cost function and the its gradient components.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
+@param f0 The value of the cost function at x0.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-static void optimization_problem_grad( const gsl_vector* parameters, void* void_instance, gsl_vector* grad );
-
+//static void optimization_problem_combined( const gsl_vector* parameters, void* void_instance, double* f0, gsl_vector* grad );
 
 
 /**
 @brief Call to calculate both the cost function and the its gradient components.
-@param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
+@param parameters Array containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
-@param grad A GNU Scientific Library vector containing the calculated gradient components.
+@param grad Array containing the calculated gradient components.
 */
-static void optimization_problem_combined( const gsl_vector* parameters, void* void_instance, double* f0, gsl_vector* grad );
+static void optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad );
+
+
 
-static void optimization_problem_combined_unitary( const gsl_vector* parameters, void* void_instance, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv );
 
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters The parameters for which the cost fuction shoule be calculated
 @param f0 The value of the cost function at x0.
 @param grad An array storing the calculated gradient components
 @param onlyCPU Set true to use only CPU in the calculations (has effect if compiled to use accelerator devices)
 */
-void optimization_problem_combined( const Matrix_real& parameters, double* f0, Matrix_real& grad );
+void optimization_problem_combined( Matrix_real parameters, double* f0, Matrix_real grad );
+
+
 
-void optimization_problem_combined_unitary( const Matrix_real& parameters, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv );
+static void optimization_problem_combined_unitary( Matrix_real parameters, void* void_instance, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv );
+void optimization_problem_combined_unitary( Matrix_real parameters, Matrix& Umtx, std::vector<Matrix>& Umtx_deriv );
 
-Matrix_real optimization_problem_batch( Matrix_real batch );
 
 /**
 // @brief The optimization problem of the final optimization
 @param parameters A GNU Scientific Library containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
```

### Comparing `squander-1.8.0/decomposition/include/N_Qubit_Decomposition_Cost_Function.h` & `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/include/N_Qubit_Decomposition_adaptive.h` & `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/include/N_Qubit_Decomposition_custom.h` & `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_custom.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/decomposition/include/Sub_Matrix_Decomposition.h` & `squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition.h`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 
     /// A map of <int n: int num> indicating that how many identical succesive blocks should be used in the disentanglement of the nth qubit from the others
     std::map<int,int> identical_blocks;
 
     /// Custom gate structure describing the gate structure used in the decomposition. The gate structure is repeated periodically in the decomposing gate structure
     Gates_block* unit_gate_structure;
 
+    /// maximal number of inner iterations
+    long long max_inner_iterations;
+
 
 public:
 
 /**
 @brief Nullary constructor of the class.
 @return An instance of the class
 */
@@ -102,15 +105,15 @@
 
 
 /**
 @brief Call to solve layer by layer the optimization problem. The optimalized parameters are stored in attribute optimized_parameters.
 @param num_of_parameters Number of parameters to be optimized
 @param solution_guess_gsl A GNU Scientific Library vector containing the solution guess.
 */
-void solve_layer_optimization_problem( int num_of_parameters, gsl_vector *solution_guess_gsl);
+void solve_layer_optimization_problem( int num_of_parameters, Matrix_real solution_guess_gsl);
 
 
 
 
 /**
 @brief The optimization problem of the final optimization
 @param parameters An array of the free parameters to be optimized. (The number of teh free paramaters should be equal to the number of parameters in one sub-layer)
@@ -122,34 +125,34 @@
 
 /**
 @brief The optimization problem of the final optimization
 @param parameters A GNU Scientific Library containing the parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @return Returns with the cost function. (zero if the qubits are desintangled.)
 */
-static double optimization_problem( const gsl_vector* parameters, void* void_instance );
+static double optimization_problem( Matrix_real parameters, void* void_instance );
 
 
 /**
 @brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-static void optimization_problem_grad( const gsl_vector* parameters, void* void_instance, gsl_vector* grad  );
+static void optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real grad  );
 
 
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-static void optimization_problem_combined( const gsl_vector* parameters, void* void_instance, double* f0, gsl_vector* grad );
+static void optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad );
 
 /**
 @brief Set the number of identical successive blocks during the subdecomposition of the qbit-th qubit.
 @param qbit The number of qubits for which the maximal number of layers should be used in the subdecomposition.
 @param identical_blocks_in The number of successive identical layers used in the subdecomposition.
 @return Returns with zero in case of success.
 */
```

### Comparing `squander-1.8.0/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h` & `squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/Adaptive.cpp` & `squander-1.8.1/gates/Adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/CH.cpp` & `squander-1.8.1/gates/CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/CNOT.cpp` & `squander-1.8.1/gates/CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/CRY.cpp` & `squander-1.8.1/gates/CRY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/CZ.cpp` & `squander-1.8.1/gates/CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/Composite.cpp` & `squander-1.8.1/gates/Composite.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/Gate.cpp` & `squander-1.8.1/gates/Gate.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/Gates_block.cpp` & `squander-1.8.1/gates/Gates_block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/ON.cpp` & `squander-1.8.1/gates/ON.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/RX.cpp` & `squander-1.8.1/gates/RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/RY.cpp` & `squander-1.8.1/gates/RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/RZ.cpp` & `squander-1.8.1/gates/RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/SX.cpp` & `squander-1.8.1/gates/SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/SYC.cpp` & `squander-1.8.1/gates/SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/U3.cpp` & `squander-1.8.1/gates/U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/UN.cpp` & `squander-1.8.1/gates/UN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/X.cpp` & `squander-1.8.1/gates/X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/Y.cpp` & `squander-1.8.1/gates/Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/Z.cpp` & `squander-1.8.1/gates/Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/Adaptive.h` & `squander-1.8.1/gates/include/Adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/CH.h` & `squander-1.8.1/gates/include/CH.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/CNOT.h` & `squander-1.8.1/gates/include/CNOT.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/CRY.h` & `squander-1.8.1/gates/include/CRY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/CZ.h` & `squander-1.8.1/gates/include/CZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/Composite.h` & `squander-1.8.1/gates/include/Composite.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/Gate.h` & `squander-1.8.1/gates/include/Gate.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/Gates_block.h` & `squander-1.8.1/gates/include/Gates_block.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/ON.h` & `squander-1.8.1/gates/include/ON.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/RX.h` & `squander-1.8.1/gates/include/RX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/RY.h` & `squander-1.8.1/gates/include/RY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/RZ.h` & `squander-1.8.1/gates/include/RZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/SX.h` & `squander-1.8.1/gates/include/SX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/SYC.h` & `squander-1.8.1/gates/include/SYC.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/U3.h` & `squander-1.8.1/gates/include/U3.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/UN.h` & `squander-1.8.1/gates/include/UN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/X.h` & `squander-1.8.1/gates/include/X.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/Y.h` & `squander-1.8.1/gates/include/Y.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/include/Z.h` & `squander-1.8.1/gates/include/Z.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/kernels/apply_kernel_to_input_AVX.cpp` & `squander-1.8.1/gates/kernels/apply_kernel_to_input_AVX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/kernels/apply_kernel_to_state_vector_input.cpp` & `squander-1.8.1/gates/kernels/apply_kernel_to_state_vector_input.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/kernels/include/apply_kernel_to_input_AVX.h` & `squander-1.8.1/gates/kernels/include/apply_kernel_to_input_AVX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/gates/kernels/include/apply_kernel_to_state_vector_input.h` & `squander-1.8.1/gates/kernels/include/apply_kernel_to_state_vector_input.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/nn/NN.cpp` & `squander-1.8.1/nn/NN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/nn/include/NN.h` & `squander-1.8.1/nn/include/NN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/optimization_engines/RL_experience.cpp` & `squander-1.8.1/optimization_engines/RL_experience.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/optimization_engines/include/RL_experience.h` & `squander-1.8.1/optimization_engines/include/RL_experience.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/CMakeLists.txt` & `squander-1.8.1/qgd_python/decomposition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1677,15 +1677,20 @@
     }
 
 
     Matrix_real parameters_mtx = numpy2matrix_real( parameters_arg );
     Matrix_real result_mtx;
 
     try {
-        result_mtx = self->decomp->optimization_problem_batch(parameters_mtx );
+        std::vector<Matrix_real> parameters_vec;
+        parameters_vec.resize(parameters_mtx.rows);
+        for( int row_idx=0; row_idx<parameters_mtx.rows; row_idx++ ) {
+            parameters_vec[row_idx] = Matrix_real( parameters_mtx.get_data() + row_idx*parameters_mtx.stride, 1, parameters_mtx.cols, parameters_mtx.stride );
+        }
+        result_mtx = self->decomp->optimization_problem_batched( parameters_vec );
     }
     catch (std::string err ) {
         PyErr_SetString(PyExc_Exception, err.c_str());
         return NULL;
     }
     catch (...) {
         std::string err( "Invalid pointer to decomposition class");
```

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py` & `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_Compression.py` & `squander-1.8.1/qgd_python/decomposition/test/test_Compression.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_Global_Phase.py` & `squander-1.8.1/qgd_python/decomposition/test/test_Global_Phase.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_IBM.py` & `squander-1.8.1/qgd_python/decomposition/test/test_IBM.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_Project_Name.py` & `squander-1.8.1/qgd_python/decomposition/test/test_Project_Name.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_QX2.py` & `squander-1.8.1/qgd_python/decomposition/test/test_QX2.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_State_Preparation.py` & `squander-1.8.1/qgd_python/decomposition/test/test_State_Preparation.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_Unitary.py` & `squander-1.8.1/qgd_python/decomposition/test/test_Unitary.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_decomposition.py` & `squander-1.8.1/qgd_python/decomposition/test/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_fmo.py` & `squander-1.8.1/qgd_python/decomposition/test/test_fmo.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_heavy_hex.py` & `squander-1.8.1/qgd_python/decomposition/test/test_heavy_hex.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_optmization_problem_combined.py` & `squander-1.8.1/qgd_python/decomposition/test/test_optmization_problem_combined.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/decomposition/test/test_parametric_circuit.py` & `squander-1.8.1/qgd_python/decomposition/test/test_parametric_circuit.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/CMakeLists.txt` & `squander-1.8.1/qgd_python/gates/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_CH.cpp` & `squander-1.8.1/qgd_python/gates/qgd_CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_CNOT.cpp` & `squander-1.8.1/qgd_python/gates/qgd_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_CZ.cpp` & `squander-1.8.1/qgd_python/gates/qgd_CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_Gates_Block.cpp` & `squander-1.8.1/qgd_python/gates/qgd_Gates_Block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_RX.cpp` & `squander-1.8.1/qgd_python/gates/qgd_RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_RY.cpp` & `squander-1.8.1/qgd_python/gates/qgd_RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_RZ.cpp` & `squander-1.8.1/qgd_python/gates/qgd_RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_SX.cpp` & `squander-1.8.1/qgd_python/gates/qgd_SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_SYC.cpp` & `squander-1.8.1/qgd_python/gates/qgd_SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_U3.cpp` & `squander-1.8.1/qgd_python/gates/qgd_U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_X.cpp` & `squander-1.8.1/qgd_python/gates/qgd_X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_Y.cpp` & `squander-1.8.1/qgd_python/gates/qgd_Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/qgd_Z.cpp` & `squander-1.8.1/qgd_python/gates/qgd_Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_CH.py` & `squander-1.8.1/qgd_python/gates/test/test_CH.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_CNOT.py` & `squander-1.8.1/qgd_python/gates/test/test_CNOT.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_CZ.py` & `squander-1.8.1/qgd_python/gates/test/test_CZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_RX.py` & `squander-1.8.1/qgd_python/gates/test/test_RX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_RY.py` & `squander-1.8.1/qgd_python/gates/test/test_RY.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_RZ.py` & `squander-1.8.1/qgd_python/gates/test/test_RZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_SX.py` & `squander-1.8.1/qgd_python/gates/test/test_SX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_U3.py` & `squander-1.8.1/qgd_python/gates/test/test_U3.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_X.py` & `squander-1.8.1/qgd_python/gates/test/test_X.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_Y.py` & `squander-1.8.1/qgd_python/gates/test/test_Y.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_Z.py` & `squander-1.8.1/qgd_python/gates/test/test_Z.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/gates/test/test_gates.py` & `squander-1.8.1/qgd_python/gates/test/test_gates.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/nn/CMakeLists.txt` & `squander-1.8.1/qgd_python/nn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/nn/qgd_nn.py` & `squander-1.8.1/qgd_python/nn/qgd_nn.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/nn/qgd_nn_Wrapper.cpp` & `squander-1.8.1/qgd_python/nn/qgd_nn_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/qgd_python/utils.py` & `squander-1.8.1/qgd_python/utils.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/random_unitary/Random_Orthogonal.cpp` & `squander-1.8.1/random_unitary/Random_Orthogonal.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/random_unitary/Random_Unitary.cpp` & `squander-1.8.1/random_unitary/Random_Unitary.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/random_unitary/include/Random_Orthogonal.h` & `squander-1.8.1/random_unitary/include/Random_Orthogonal.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/random_unitary/include/Random_Unitary.h` & `squander-1.8.1/random_unitary/include/Random_Unitary.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/setup.py` & `squander-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 setup(
     name="squander",
     packages=find_packages(
         exclude=(
             "test_standalone", "test_standalone.*",
         )
     ),
-    version='1.8.0',
+    version='1.8.1',
     url="https://github.com/rakytap/sequential-quantum-gate-decomposer", 
     maintainer="Peter Rakyta",
     maintainer_email="peter.rakyta@ttk.elte.hu",
     include_package_data=True,
     install_requires=[
         "setuptools>=40.8.0",
         "wheel",
```

### Comparing `squander-1.8.0/squander/__init__.py` & `squander-1.8.1/squander/__init__.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/squander.egg-info/PKG-INFO` & `squander-1.8.1/squander.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.0
+Version: 1.8.1
 Summary: The C++ binding for the SQUANDER package
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
@@ -48,20 +48,17 @@
 * Zoltán Zimborás (researcher): zimboras.zoltan@wigner.hu
 * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
 
 
 
 ### Dependencies
 
-The optimization algorithm of SQUANDER relies on the [multimin](https://www.gnu.org/software/gsl/doc/html/multimin.html) component of the [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/index.html). 
-We developed and tested the SQUANDER package with GNU Scientific Library of version 2.5, 2.6 and 2.7.
 The dependencies necessary to compile and build the SQUANDER package are the followings:
 
 * [CMake](https://cmake.org/) (>=3.10.2)
-* [GNU Scientific Library](https://www.gnu.org/software/gsl/doc/html/index.html) (>=2.5, shipped with the gsl python package)
 * C++/C [Intel](https://software.intel.com/content/www/us/en/develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler
 * [TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel Python package)
 * [Intel MKL](https://software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html) (optional)
 * [OpenBlas](https://www.openblas.net/) (optional, recommended)
 * [LAPACKE](https://www.netlib.org/lapack/lapacke.html)
 * [Doxygen](https://www.doxygen.nl/index.html) (optional)
 
@@ -69,78 +66,36 @@
 The SQUANDER Python interface needs the following packages to be installed on the system:
 
 * [Qiskit](https://qiskit.org/documentation/install.html)
 * [Numpy](https://numpy.org/install/)
 * [scipy](https://www.scipy.org/install.html)
 * [scikit-build](https://scikit-build.readthedocs.io/en/latest/)
 * [tbb-devel](https://pypi.org/project/tbb-devel/) (containing the TBB Library)
-* [gsl](https://anaconda.org/conda-forge/gsl) (containing the GNU Scientific Library)
 
 
 
 
-### How to obtain GNU Scientific Library
-
-In order to build and use the SQUANDER we recommend the Anaconda virtual python environment providing all the required dependencies for SQUANDER.
-One can easily install the GNU Scientific Library for local users by the command
-
-$ conda install -c conda-forge gsl
-
-Alternatively, a python binding project alongside the GNU GSL library is accessible via pypi repository:
-
-$ pip install numpy swig
-
-$ pip install pygsl
-
-Here we describe an alternative way to deploy GNU Scientific Library from source by the end user without administrative privileges. 
-The GNU Scientific Library can be downloaded from the site [https://www.gnu.org/software/gsl/](https://www.gnu.org/software/gsl/).
-After the downloaded package is extracted somewhere in the home directory of the user (**path/to/gsl/source**), one should configure the building environment using the **configure** tool.
-Depending on the individual settings the default compiler to be invoked might be different from HPC to HPC. 
-To ensure the usage of the GNU compiler, the following shell command should be executed inside the directory **path/to/gsl/source**:
-
-$ ./configure --prefix=path/to/gsl FC=gfortran CC=gcc CXX=g++
-
-(Similarly, Intel compiler can be forced by setting FC=ifort CC=icc and CXX=icpc.)
-The installation directory of the compiled GNU Scientific Library is given by **--prefix=path/to/gsl** (which is different from the directory path of 
-the source files given by **path/to/gslsource**).
-To install GNU Scientific Library the user should have read and write permissions on the path **path/to/gsl** (which might be for example /home/username/gsl).
-After the successful configuration the GNU Scientific Library can be compiled by the shell command
-
-$ make
-
-The compilation of the GNU Scientific Library takes some time. When the compilation is done, the package (including the C header files and the static and shared libraries) is installed into the directory **path/to/gsl** by the shell command:
-
-$ make install
-
 ### Install SQUANDER from Python Package Index (PyPI)
 
 Since version 1.7.1 the SQUANDER package is accessible at Python Package Index (PyPI). The package can be installed on linux systems following the steps outlined below:
 
 $ pip install numpy swig tbb-devel wheel scikit-build ninja qiskit
 
-$ pip install pygsl
-
 $ pip install squander
 
 
 
 ### Download the SQUANDER package
 
 The developer version of the Quantum Gate Decomposer package can be downloaded from github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/tree/master).
 After the package is downloaded into the directory **path/to/SQUANDER/package** (which would be the path to the source code of the SQUANDER package), one can proceed to the compilation steps described in the next section.
 
 ### How to build the SQUANDER package
 
 The SQUANDER package is equipped with a Python build script and CMake tools to ease the compilation and the deployment of the package.
-To ensure that SQUANDER package would find the necessary libraries and header files during compilation time it is advised to define the following environment variables:
-
-$ export GSL_LIB_DIR=path/to/gsl/lib(64)
-
-$ export GSL_INC_DIR=path/to/gsl/include
-
 The SQUANDER package is parallelized via Threading Building Block (TBB) libraries. If TBB is not present in the system, it can be easily installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
 Alternatively the TBB libraries can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB)   and built from source. 
 In this case one should supply the necessary environment variables pointing to the header and library files of the TBB package. For newer
 Intel compilers the TBB package is part of the Intel compiler package, similarly to the MKL package. If the TBB library is located at non-standrad path or the SQUANDER package is compiled with GNU compiler, then setting the
 
 $ export TBB_LIB_DIR=path/to/TBB/lib(64)
 
@@ -167,16 +122,14 @@
 
 $ conda activate qgd
 
 Install dependencies:
 
 $ conda install numpy scipy pip pytest scikit-build tbb-devel
 
-$ conda install -c conda-forge gsl
-
 $ pip install qiskit matplotlib 
 
 After the basic environment variables are set and the dependencies are installed, the compilation of the package can be started by the Python command:
 
 $ python3 setup.py build_ext
 
 The command above starts the compilation of the SQUANDER C++ library and builds the necessary C++ Python interface extensions of the SQUANDER package in place.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.0 Summary: The C++ binding
+Metadata-Version: 2.1 Name: squander Version: 1.8.1 Summary: The C++ binding
 for the SQUANDER package Home-page: https://github.com/rakytap/sequential-
 quantum-gate-decomposer Maintainer: Peter Rakyta Maintainer-email:
 peter.rakyta@ttk.elte.hu License: GNU General Public License v3.0 Keywords:
 test,cmake,extension Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Programming Language :: C Classifier:
 Programming Language :: C++ Description-Content-Type: text/markdown License-
 File: LICENSE [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)]
@@ -37,149 +37,113 @@
 and by the Ministry of Innovation and Technology and the National Research,
 Development and Innovation Office within the Quantum Information National
 Laboratory of Hungary. Find the documantation of the SQUANDER package at
 [CodeDocs[xyz]](https://codedocs.xyz/rakytap/sequential-quantum-gate-
 decomposer/) ### Contact Us Have a question about the SQUANDER package? Don't
 hesitate to contact us at the following e-mails: * ZoltÃ¡n ZimborÃ¡s
 (researcher): zimboras.zoltan@wigner.hu * Peter Rakyta (developer):
-peter.rakyta@ttk.elte.hu ### Dependencies The optimization algorithm of
-SQUANDER relies on the [multimin](https://www.gnu.org/software/gsl/doc/html/
-multimin.html) component of the [GNU Scientific Library](https://www.gnu.org/
-software/gsl/doc/html/index.html). We developed and tested the SQUANDER package
-with GNU Scientific Library of version 2.5, 2.6 and 2.7. The dependencies
-necessary to compile and build the SQUANDER package are the followings: *
-[CMake](https://cmake.org/) (>=3.10.2) * [GNU Scientific Library](https://
-www.gnu.org/software/gsl/doc/html/index.html) (>=2.5, shipped with the gsl
-python package) * C++/C [Intel](https://software.intel.com/content/www/us/en/
+peter.rakyta@ttk.elte.hu ### Dependencies The dependencies necessary to compile
+and build the SQUANDER package are the followings: * [CMake](https://cmake.org/
+) (>=3.10.2) * C++/C [Intel](https://software.intel.com/content/www/us/en/
 develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://
 gcc.gnu.org/) (>=v4.8.1) compiler * [TBB](https://github.com/oneapi-src/oneTBB)
 library (shipped with tbb-devel Python package) * [Intel MKL](https://
 software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html)
 (optional) * [OpenBlas](https://www.openblas.net/) (optional, recommended) *
 [LAPACKE](https://www.netlib.org/lapack/lapacke.html) * [Doxygen](https://
 www.doxygen.nl/index.html) (optional) The Python interface of SQUANDER was
 developed and tested with Python 3.6-3.9. The SQUANDER Python interface needs
 the following packages to be installed on the system: * [Qiskit](https://
 qiskit.org/documentation/install.html) * [Numpy](https://numpy.org/install/) *
 [scipy](https://www.scipy.org/install.html) * [scikit-build](https://scikit-
 build.readthedocs.io/en/latest/) * [tbb-devel](https://pypi.org/project/tbb-
-devel/) (containing the TBB Library) * [gsl](https://anaconda.org/conda-forge/
-gsl) (containing the GNU Scientific Library) ### How to obtain GNU Scientific
-Library In order to build and use the SQUANDER we recommend the Anaconda
-virtual python environment providing all the required dependencies for
-SQUANDER. One can easily install the GNU Scientific Library for local users by
-the command $ conda install -c conda-forge gsl Alternatively, a python binding
-project alongside the GNU GSL library is accessible via pypi repository: $ pip
-install numpy swig $ pip install pygsl Here we describe an alternative way to
-deploy GNU Scientific Library from source by the end user without
-administrative privileges. The GNU Scientific Library can be downloaded from
-the site [https://www.gnu.org/software/gsl/](https://www.gnu.org/software/gsl/
-). After the downloaded package is extracted somewhere in the home directory of
-the user (**path/to/gsl/source**), one should configure the building
-environment using the **configure** tool. Depending on the individual settings
-the default compiler to be invoked might be different from HPC to HPC. To
-ensure the usage of the GNU compiler, the following shell command should be
-executed inside the directory **path/to/gsl/source**: $ ./configure --
-prefix=path/to/gsl FC=gfortran CC=gcc CXX=g++ (Similarly, Intel compiler can be
-forced by setting FC=ifort CC=icc and CXX=icpc.) The installation directory of
-the compiled GNU Scientific Library is given by **--prefix=path/to/gsl** (which
-is different from the directory path of the source files given by **path/to/
-gslsource**). To install GNU Scientific Library the user should have read and
-write permissions on the path **path/to/gsl** (which might be for example /
-home/username/gsl). After the successful configuration the GNU Scientific
-Library can be compiled by the shell command $ make The compilation of the GNU
-Scientific Library takes some time. When the compilation is done, the package
-(including the C header files and the static and shared libraries) is installed
-into the directory **path/to/gsl** by the shell command: $ make install ###
-Install SQUANDER from Python Package Index (PyPI) Since version 1.7.1 the
-SQUANDER package is accessible at Python Package Index (PyPI). The package can
-be installed on linux systems following the steps outlined below: $ pip install
-numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install pygsl $ pip
-install squander ### Download the SQUANDER package The developer version of the
-Quantum Gate Decomposer package can be downloaded from github repository
-[https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://
-github.com/rakytap/quantum-gate-decomposer/tree/master). After the package is
-downloaded into the directory **path/to/SQUANDER/package** (which would be the
-path to the source code of the SQUANDER package), one can proceed to the
-compilation steps described in the next section. ### How to build the SQUANDER
-package The SQUANDER package is equipped with a Python build script and CMake
-tools to ease the compilation and the deployment of the package. To ensure that
-SQUANDER package would find the necessary libraries and header files during
-compilation time it is advised to define the following environment variables: $
-export GSL_LIB_DIR=path/to/gsl/lib(64) $ export GSL_INC_DIR=path/to/gsl/include
-The SQUANDER package is parallelized via Threading Building Block (TBB)
-libraries. If TBB is not present in the system, it can be easily installed via
-python package [tbb-devel](https://pypi.org/project/tbb-devel/). Alternatively
-the TBB libraries can be installed via apt or yum utility (sudo apt install
-libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB]
-(https://github.com/oneapi-src/oneTBB) and built from source. In this case one
-should supply the necessary environment variables pointing to the header and
-library files of the TBB package. For newer Intel compilers the TBB package is
-part of the Intel compiler package, similarly to the MKL package. If the TBB
-library is located at non-standrad path or the SQUANDER package is compiled
-with GNU compiler, then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $
-export TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
-successful compilation. When the TBB library is installed via a python package,
-setting the environment variables above is not necessary. The SQUANDER package
-with C++ Python extensions can be compiled via the Python script **setup.py**
-located in the root directory of the SQUANDER package. The script automatically
-finds out the CBLAS library working behind the numpy package and uses it in
-further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Developer build We
-recommend to install the SQUANDER package in the Anaconda environment. In order
-to install the necessary requirements, follow the steps below: Creating new
-python environment: $ conda create -n qgd Activate the new anaconda environment
-$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
-pytest scikit-build tbb-devel $ conda install -c conda-forge gsl $ pip install
-qiskit matplotlib After the basic environment variables are set and the
-dependencies are installed, the compilation of the package can be started by
-the Python command: $ python3 setup.py build_ext The command above starts the
-compilation of the SQUANDER C++ library and builds the necessary C++ Python
-interface extensions of the SQUANDER package in place. After a successful
-build, one can register the SQUANDER package in the Python distribution in
-developer (i.e. editable) mode by command: $ python -m pip install -e . ###
-Binary distribution After the environment variables are set it is possible to
-build wheel binaries of the SQUANDER package. In order to launch the
-compilation process from python, **[scikit-build](https://scikit-
-build.readthedocs.io/en/latest/)** package is necessary. (It is optional to
-install the ninja package which speeds up the building process by parallel
-compilation.) The binary wheel can be constructed by command $ python3 setup.py
-bdist_wheel in the root directory of the SQUADER package. The created SQUANDER
-wheel can be installed on the local machine by issuing the command from the
-directory **path/to/SQUANDER/package/dist** $ pip3 install qgd-*.whl We notice,
-that the created wheel is not portable, since it contains hard coded link to
-external libraries (TBB and CBLAS). ### Source distribution A portable source
-distribution of the SQUANDER package can be created by a command launched from
-the root directory of the SQUANDER package: $ python3 setup.py sdist In order
-to create a source distribution it is not necessary to set the environment
-variables, since this script only collects the necessary files and pack them
-into a tar ball located in the directory **path/to/SQUANDER/package/dist**. In
-order to install the SQUANDER package from source tar ball, see the previous
-section discussing the initialization of the environment variables. The package
-can be compiled and installed by the command $ pip3 install qgd-*.tar.gz issued
-from directory **path/to/SQUANDER/package/dist** (It is optional to install the
-ninja package which speeds up the building process by parallel compilation.)
-### How to use The algorithm implemented in the SQUANDER package intends to
-transform the given unitary into an identity matrix via a sequence of two-qubit
-and one-qubit gate operations applied on the unitary. Thus, in order to get the
-decomposition of a unitary, one should rather provide the complex transpose of
-this unitary as the input for the SQUANDER decomposing process, as can be seen
-in the examples. ## Python Interface The SQUANDER package contains a Python
-interface allowing the access of the functionalities of the SQUANDER package
-from Python. The usage of the SQUANDER Python interface is demonstrated in the
-example files in the directory **examples** located in the directory **path/to/
-SQUANDER/package**, or in test files located in sub-directories of **path/to/
-SQUANDER/package/qgd_python/*/test**. ### Example code snippet Here we provide
-an example to use the SQUANDER package. The following python interface is
-accessible from version 1.8.0. In this example we use two optimization engines
-for the decomposition: 1. An evolutionary engine called AGENTS 2. Second order
-gradient descend algorithm (BFGS) Firstly we construct a Python map to set
-hyper-parameters during the gate synthesis. #Python map containing hyper-
-parameters config = { 'max_outer_iterations': 1, 'max_inner_iterations_agent':
-25000, 'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
+devel/) (containing the TBB Library) ### Install SQUANDER from Python Package
+Index (PyPI) Since version 1.7.1 the SQUANDER package is accessible at Python
+Package Index (PyPI). The package can be installed on linux systems following
+the steps outlined below: $ pip install numpy swig tbb-devel wheel scikit-build
+ninja qiskit $ pip install squander ### Download the SQUANDER package The
+developer version of the Quantum Gate Decomposer package can be downloaded from
+github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/
+master](https://github.com/rakytap/quantum-gate-decomposer/tree/master). After
+the package is downloaded into the directory **path/to/SQUANDER/package**
+(which would be the path to the source code of the SQUANDER package), one can
+proceed to the compilation steps described in the next section. ### How to
+build the SQUANDER package The SQUANDER package is equipped with a Python build
+script and CMake tools to ease the compilation and the deployment of the
+package. The SQUANDER package is parallelized via Threading Building Block
+(TBB) libraries. If TBB is not present in the system, it can be easily
+installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
+Alternatively the TBB libraries can be installed via apt or yum utility (sudo
+apt install libtbb-dev) or it can be downloaded from [https://github.com/
+oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB) and built from source.
+In this case one should supply the necessary environment variables pointing to
+the header and library files of the TBB package. For newer Intel compilers the
+TBB package is part of the Intel compiler package, similarly to the MKL
+package. If the TBB library is located at non-standrad path or the SQUANDER
+package is compiled with GNU compiler, then setting the $ export
+TBB_LIB_DIR=path/to/TBB/lib(64) $ export TBB_INC_DIR=path/to/TBB/include
+environment variables are sufficient for successful compilation. When the TBB
+library is installed via a python package, setting the environment variables
+above is not necessary. The SQUANDER package with C++ Python extensions can be
+compiled via the Python script **setup.py** located in the root directory of
+the SQUANDER package. The script automatically finds out the CBLAS library
+working behind the numpy package and uses it in further linking. The
+**setup.py** script also build the C++ library of the SQUANDER package by
+making the appropriate CMake calls. ### Developer build We recommend to install
+the SQUANDER package in the Anaconda environment. In order to install the
+necessary requirements, follow the steps below: Creating new python
+environment: $ conda create -n qgd Activate the new anaconda environment $
+conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
+scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+environment variables are set and the dependencies are installed, the
+compilation of the package can be started by the Python command: $ python3
+setup.py build_ext The command above starts the compilation of the SQUANDER C++
+library and builds the necessary C++ Python interface extensions of the
+SQUANDER package in place. After a successful build, one can register the
+SQUANDER package in the Python distribution in developer (i.e. editable) mode
+by command: $ python -m pip install -e . ### Binary distribution After the
+environment variables are set it is possible to build wheel binaries of the
+SQUANDER package. In order to launch the compilation process from python, **
+[scikit-build](https://scikit-build.readthedocs.io/en/latest/)** package is
+necessary. (It is optional to install the ninja package which speeds up the
+building process by parallel compilation.) The binary wheel can be constructed
+by command $ python3 setup.py bdist_wheel in the root directory of the SQUADER
+package. The created SQUANDER wheel can be installed on the local machine by
+issuing the command from the directory **path/to/SQUANDER/package/dist** $ pip3
+install qgd-*.whl We notice, that the created wheel is not portable, since it
+contains hard coded link to external libraries (TBB and CBLAS). ### Source
+distribution A portable source distribution of the SQUANDER package can be
+created by a command launched from the root directory of the SQUANDER package:
+$ python3 setup.py sdist In order to create a source distribution it is not
+necessary to set the environment variables, since this script only collects the
+necessary files and pack them into a tar ball located in the directory **path/
+to/SQUANDER/package/dist**. In order to install the SQUANDER package from
+source tar ball, see the previous section discussing the initialization of the
+environment variables. The package can be compiled and installed by the command
+$ pip3 install qgd-*.tar.gz issued from directory **path/to/SQUANDER/package/
+dist** (It is optional to install the ninja package which speeds up the
+building process by parallel compilation.) ### How to use The algorithm
+implemented in the SQUANDER package intends to transform the given unitary into
+an identity matrix via a sequence of two-qubit and one-qubit gate operations
+applied on the unitary. Thus, in order to get the decomposition of a unitary,
+one should rather provide the complex transpose of this unitary as the input
+for the SQUANDER decomposing process, as can be seen in the examples. ## Python
+Interface The SQUANDER package contains a Python interface allowing the access
+of the functionalities of the SQUANDER package from Python. The usage of the
+SQUANDER Python interface is demonstrated in the example files in the directory
+**examples** located in the directory **path/to/SQUANDER/package**, or in test
+files located in sub-directories of **path/to/SQUANDER/package/qgd_python/*/
+test**. ### Example code snippet Here we provide an example to use the SQUANDER
+package. The following python interface is accessible from version 1.8.0. In
+this example we use two optimization engines for the decomposition: 1. An
+evolutionary engine called AGENTS 2. Second order gradient descend algorithm
+(BFGS) Firstly we construct a Python map to set hyper-parameters during the
+gate synthesis. #Python map containing hyper-parameters config =
+{ 'max_outer_iterations': 1, 'max_inner_iterations_agent': 25000,
+'max_inner_iterations_compression': 10000, 'max_inner_iterations' : 500,
 'max_inner_iterations_final': 5000, 'Randomized_Radius': 0.3,
 'randomized_adaptive_layers': 1, 'optimization_tolerance_agent': 1e-4,
 'optimization_tolerance': 1e-8, 'agent_num': 10} Next we initialize the
 decomposition class with the unitary Umtx to be decomposed. # creating a class
 to decompose the unitary from squander import N_Qubit_Decomposition_adaptive
 cDecompose = N_Qubit_Decomposition_adaptive( Umtx.conj().T, config=config ) The
 verbosity of the execution output can be controlled by the function call #
```

### Comparing `squander-1.8.0/squander.egg-info/SOURCES.txt` & `squander-1.8.1/squander.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,36 @@
 setup.py
 cmake/check_AVX.cmake
 common/Adam.cpp
 common/common.cpp
 common/common_DFE.cpp
 common/config_element.cpp
 common/dot.cpp
+common/lbfgs.cpp
 common/logging.cpp
 common/matrix.cpp
 common/matrix_real.cpp
 common/mpi_base.cpp
 common/numpy_interface.cpp
+common/tolmin.cpp
 common/include/Adam.h
 common/include/Config.h.in
 common/include/QGDTypes.h
 common/include/common.h
 common/include/common_DFE.h
 common/include/config_element.h
 common/include/dot.h
+common/include/lbfgs.h
 common/include/logging.h
 common/include/matrix.h
 common/include/matrix_base.h
 common/include/matrix_real.h
 common/include/mpi_base.h
 common/include/numpy_interface.h
+common/include/tolmin.h
 decomposition/Decomposition_Base.cpp
 decomposition/N_Qubit_Decomposition.cpp
 decomposition/N_Qubit_Decomposition_Base.cpp
 decomposition/N_Qubit_Decomposition_Cost_Function.cpp
 decomposition/N_Qubit_Decomposition_adaptive.cpp
 decomposition/N_Qubit_Decomposition_custom.cpp
 decomposition/Sub_Matrix_Decomposition.cpp
```

### Comparing `squander-1.8.0/test_standalone/CMakeLists.txt` & `squander-1.8.1/test_standalone/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/test_standalone/custom_gate_structure_test.cpp` & `squander-1.8.1/test_standalone/custom_gate_structure_test.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.0/test_standalone/decomposition_test.cpp` & `squander-1.8.1/test_standalone/decomposition_test.cpp`

 * *Files identical despite different names*

