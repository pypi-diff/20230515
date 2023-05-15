# Comparing `tmp/multipie-1.0.0.tar.gz` & `tmp/multipie-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipie-1.0.0.tar", last modified: Mon May 15 16:17:24 2023, max compression
+gzip compressed data, was "multipie-1.0.1.tar", last modified: Mon May 15 16:53:40 2023, max compression
```

## Comparing `multipie-1.0.0.tar` & `multipie-1.0.1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.190372 multipie-1.0.0/
--rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.0.0/LICENSE
--rw-------   0 hiro       (501) staff       (20)       99 2023-05-15 15:17:15.000000 multipie-1.0.0/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2086 2023-05-15 16:17:24.190472 multipie-1.0.0/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1591 2023-05-15 15:30:57.000000 multipie-1.0.0/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.149556 multipie-1.0.0/doc/
--rwxr-xr-x   0 hiro       (501) staff       (20)      599 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/Makefile
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.151995 multipie-1.0.0/doc/source/
--rw-r--r--   0 hiro       (501) staff       (20)      394 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/application.rst
--rw-r--r--   0 hiro       (501) staff       (20)      313 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/character.rst
--rw-------   0 hiro       (501) staff       (20)     5611 2023-05-15 15:20:56.000000 multipie-1.0.0/doc/source/conf.py
--rw-r--r--   0 hiro       (501) staff       (20)      511 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/developer.rst
--rw-r--r--   0 hiro       (501) staff       (20)      165 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/genindex.rst
--rw-r--r--   0 hiro       (501) staff       (20)      366 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/group.rst
--rw-r--r--   0 hiro       (501) staff       (20)      362 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/harmonics.rst
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-05-15 15:23:08.000000 multipie-1.0.0/doc/source/index.rst
--rw-r--r--   0 hiro       (501) staff       (20)      555 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/model.rst
--rw-r--r--   0 hiro       (501) staff       (20)      353 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/multipole.rst
--rw-r--r--   0 hiro       (501) staff       (20)      342 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/response_tensor.rst
--rw-r--r--   0 hiro       (501) staff       (20)      454 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/symmetry_operation.rst
--rw-r--r--   0 hiro       (501) staff       (20)      841 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/tag.rst
--rw-r--r--   0 hiro       (501) staff       (20)      335 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/virtual_cluster.rst
--rw-r--r--   0 hiro       (501) staff       (20)      287 2023-05-09 15:21:28.000000 multipie-1.0.0/doc/source/wyckoff.rst
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.152260 multipie-1.0.0/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-05-15 15:11:06.000000 multipie-1.0.0/multipie/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.165938 multipie-1.0.0/multipie/binary_data/
--rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.0.0/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.0.0/multipie/binary_data/CharacterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.0.0/multipie/binary_data/ClebschGordanPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.0.0/multipie/binary_data/HarmonicsPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.0.0/multipie/binary_data/ResponseTensorPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.0.0/multipie/binary_data/SymmetryOperationGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.0.0/multipie/binary_data/VirtualClusterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.0.0/multipie/binary_data/WyckoffGSet.pkl
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.166438 multipie-1.0.0/multipie/character/
--rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/character/character_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/character/character_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.166847 multipie-1.0.0/multipie/character/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)      838 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/character/tests/test_character_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      878 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/character/tests/test_character_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.167199 multipie-1.0.0/multipie/clebsch_gordan/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/clebsch_gordan/clebsch_gordan_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.167474 multipie-1.0.0/multipie/clebsch_gordan/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1142 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1165 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg_set.py
--rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.0.0/multipie/const.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.175679 multipie-1.0.0/multipie/data/
--rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_atomic_multipoles.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_cartesian_to_ch_harmoncis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_character_table.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_compatibility_relation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_harmonics_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_no_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_product_decomp.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_symmetry_operation_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_symmetry_operation_sg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_tag_harmonics_alias.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_tag_point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_tag_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_transform_matrix.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_virtual_cluster_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_wyckoff_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/data/data_wyckoff_sg.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.175897 multipie-1.0.0/multipie/examples/
--rwxr-xr-x   0 hiro       (501) staff       (20)      395 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/examples/ex_create_model.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.176533 multipie-1.0.0/multipie/examples/models/
--rwxr-xr-x   0 hiro       (501) staff       (20)      231 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/examples/models/cm.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      344 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/examples/models/graphene.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      519 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/examples/models/te.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.176828 multipie-1.0.0/multipie/group/
--rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/group/point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    22492 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/group/space_group.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.177113 multipie-1.0.0/multipie/group/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2579 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/group/tests/test_point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1377 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/group/tests/test_space_group.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.177734 multipie-1.0.0/multipie/harmonics/
--rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/harmonics/harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/harmonics_complex_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/harmonics_complex_pg_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/harmonics_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/harmonics_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.178255 multipie-1.0.0/multipie/harmonics/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)      528 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/tests/test_equivalent_operator.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1127 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/harmonics/tests/test_harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      441 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/tests/test_harmonics_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      439 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/harmonics/tests/test_harmonics_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.178395 multipie-1.0.0/multipie/harmonics/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/harmonics/util/equivalent_operator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.179192 multipie-1.0.0/multipie/model/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2149 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/construct_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/model/create_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    29773 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/material_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/multipie_manager.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    17710 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/symmetry_adapted_model.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.179865 multipie-1.0.0/multipie/model/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)     8278 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/model/tests/model_example.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2580 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/tests/test_construct_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      442 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/model/tests/test_material_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      542 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/model/tests/test_material_viewer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.180295 multipie-1.0.0/multipie/model/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/util/atomic_matrix_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    25780 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/util/create_pdf.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    24331 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/model/util/symmetry_adapted_model_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.146935 multipie-1.0.0/multipie/multipole/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.180586 multipie-1.0.0/multipie/multipole/base/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/multipole/base/base_atomic_multipole_dataset.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/multipole/base/base_atomic_multipole_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.180990 multipie-1.0.0/multipie/multipole/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2797 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/multipole/tests/test_atomic_orbital_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      447 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/multipole/tests/test_base_atomic_multipole_dataset.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      421 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/multipole/tests/test_base_atomic_multipole_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.182444 multipie-1.0.0/multipie/multipole/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    14659 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/multipole/util/atomic_orbital_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7216 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/multipole/util/atomic_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/multipole/util/multipole_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/multipole/util/pauli.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/multipole/util/spin_orbital_basis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/multipole/util/structure_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/multipole/util/z_samb_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.182845 multipie-1.0.0/multipie/response_tensor/
--rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/response_tensor/response_tensor_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/response_tensor/response_tensor_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.183181 multipie-1.0.0/multipie/response_tensor/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)      307 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/response_tensor/tests/test_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4692 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/response_tensor/tests/test_response_tensor_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.183337 multipie-1.0.0/multipie/response_tensor/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/response_tensor/util/response_tensor_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.183632 multipie-1.0.0/multipie/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.0.0/multipie/scripts/create_binary.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1541 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/scripts/create_samb.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.184039 multipie-1.0.0/multipie/symmetry_operation/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/symmetry_operation/symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/symmetry_operation/symmetry_operation_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/symmetry_operation/symmetry_operation_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.184574 multipie-1.0.0/multipie/symmetry_operation/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1548 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1607 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      531 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation_g_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1281 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.184701 multipie-1.0.0/multipie/symmetry_operation/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/symmetry_operation/util/symmetry_operation_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.185709 multipie-1.0.0/multipie/tag/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_list.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_multipole.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tag_wyckoff.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.186552 multipie-1.0.0/multipie/tag/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1108 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tests/test_tag_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      736 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tests/test_tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1441 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tests/test_tag_multipole.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1297 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tests/test_tag_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1797 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tests/test_tag_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      624 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/tag/tests/test_tag_wyckoff.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.186840 multipie-1.0.0/multipie/virtual_cluster/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.187145 multipie-1.0.0/multipie/virtual_cluster/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)      555 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/virtual_cluster/tests/test_virtual_cluster_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      480 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/virtual_cluster/tests/test_virtual_cluster_pg_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/virtual_cluster/virtual_cluster_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/virtual_cluster/virtual_cluster_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.187480 multipie-1.0.0/multipie/wyckoff/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.187824 multipie-1.0.0/multipie/wyckoff/tests/
--rwxr-xr-x   0 hiro       (501) staff       (20)      691 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/wyckoff/tests/test_wyckoff_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      500 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/wyckoff/tests/test_wyckoff_g_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.0.0/multipie/wyckoff/wyckoff_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.0.0/multipie/wyckoff/wyckoff_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.153067 multipie-1.0.0/multipie.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2086 2023-05-15 16:17:24.000000 multipie-1.0.0/multipie.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     5986 2023-05-15 16:17:24.000000 multipie-1.0.0/multipie.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-15 16:17:24.000000 multipie-1.0.0/multipie.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)      116 2023-05-15 16:17:24.000000 multipie-1.0.0/multipie.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       71 2023-05-15 16:17:24.000000 multipie-1.0.0/multipie.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        9 2023-05-15 16:17:24.000000 multipie-1.0.0/multipie.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      876 2023-05-15 16:17:24.190885 multipie-1.0.0/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.0.0/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.148599 multipie-1.0.0/tools/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.188330 multipie-1.0.0/tools/data/
--rw-r--r--   0 hiro       (501) staff       (20)     5398 2023-05-09 15:21:28.000000 multipie-1.0.0/tools/data/create_data_atomic_multipoles.py
--rw-r--r--   0 hiro       (501) staff       (20)     2794 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/data/create_data_real_harmonics.py
--rw-r--r--   0 hiro       (501) staff       (20)     1718 2023-05-09 15:21:28.000000 multipie-1.0.0/tools/data/create_data_virtual_cluster.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.188646 multipie-1.0.0/tools/data/util/
--rw-r--r--   0 hiro       (501) staff       (20)    13042 2023-05-09 15:21:28.000000 multipie-1.0.0/tools/data/util/atomic_multipole_matrix.py
--rw-r--r--   0 hiro       (501) staff       (20)      273 2023-05-09 15:21:28.000000 multipie-1.0.0/tools/data/util/output_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:17:24.190212 multipie-1.0.0/tools/pdf/
--rw-r--r--   0 hiro       (501) staff       (20)     3628 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_atomic_multipole.py
--rw-r--r--   0 hiro       (501) staff       (20)     3589 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_character.py
--rw-r--r--   0 hiro       (501) staff       (20)     2386 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_harmonics.py
--rw-r--r--   0 hiro       (501) staff       (20)     1861 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_response_tensor.py
--rw-r--r--   0 hiro       (501) staff       (20)     4578 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_symmetry_operation.py
--rw-r--r--   0 hiro       (501) staff       (20)     1572 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_virtual_cluster.py
--rw-r--r--   0 hiro       (501) staff       (20)     1989 2023-05-15 15:10:01.000000 multipie-1.0.0/tools/pdf/create_pdf_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.774211 multipie-1.0.1/
+-rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.0.1/LICENSE
+-rw-------   0 hiro       (501) staff       (20)       99 2023-05-15 15:17:15.000000 multipie-1.0.1/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2086 2023-05-15 16:53:40.774306 multipie-1.0.1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1591 2023-05-15 15:30:57.000000 multipie-1.0.1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.726388 multipie-1.0.1/doc/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      599 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/Makefile
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.729394 multipie-1.0.1/doc/source/
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/application.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      313 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/character.rst
+-rw-------   0 hiro       (501) staff       (20)     5611 2023-05-15 15:20:56.000000 multipie-1.0.1/doc/source/conf.py
+-rw-r--r--   0 hiro       (501) staff       (20)      511 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/developer.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      165 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/genindex.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      366 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/group.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      362 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/harmonics.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-05-15 15:23:08.000000 multipie-1.0.1/doc/source/index.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      555 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/model.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      353 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/multipole.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      342 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/response_tensor.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      454 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/symmetry_operation.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      841 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/tag.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      335 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/virtual_cluster.rst
+-rw-r--r--   0 hiro       (501) staff       (20)      287 2023-05-09 15:21:28.000000 multipie-1.0.1/doc/source/wyckoff.rst
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.729693 multipie-1.0.1/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-05-15 16:52:48.000000 multipie-1.0.1/multipie/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.743530 multipie-1.0.1/multipie/binary_data/
+-rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.0.1/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.0.1/multipie/binary_data/CharacterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.0.1/multipie/binary_data/ClebschGordanPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.0.1/multipie/binary_data/HarmonicsPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.0.1/multipie/binary_data/ResponseTensorPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.0.1/multipie/binary_data/SymmetryOperationGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.0.1/multipie/binary_data/VirtualClusterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.0.1/multipie/binary_data/WyckoffGSet.pkl
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.744100 multipie-1.0.1/multipie/character/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/character/character_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/character/character_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.744387 multipie-1.0.1/multipie/character/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      838 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/character/tests/test_character_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      878 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/character/tests/test_character_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.744660 multipie-1.0.1/multipie/clebsch_gordan/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/clebsch_gordan/clebsch_gordan_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.744957 multipie-1.0.1/multipie/clebsch_gordan/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1142 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1165 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg_set.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.0.1/multipie/const.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.753771 multipie-1.0.1/multipie/data/
+-rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_atomic_multipoles.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_cartesian_to_ch_harmoncis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_character_table.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_compatibility_relation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_harmonics_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_no_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_product_decomp.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_symmetry_operation_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_symmetry_operation_sg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_tag_harmonics_alias.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_tag_point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_tag_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_transform_matrix.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_virtual_cluster_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_wyckoff_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/data/data_wyckoff_sg.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.754094 multipie-1.0.1/multipie/examples/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      404 2023-05-15 16:47:35.000000 multipie-1.0.1/multipie/examples/ex_create_model.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.754595 multipie-1.0.1/multipie/examples/models/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      231 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/examples/models/cm.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      344 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/examples/models/graphene.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      519 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/examples/models/te.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.754927 multipie-1.0.1/multipie/group/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/group/point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22492 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/group/space_group.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.755222 multipie-1.0.1/multipie/group/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2579 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/group/tests/test_point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1377 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/group/tests/test_space_group.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.755897 multipie-1.0.1/multipie/harmonics/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/harmonics/harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/harmonics_complex_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/harmonics_complex_pg_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/harmonics_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/harmonics_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.762428 multipie-1.0.1/multipie/harmonics/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      528 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/tests/test_equivalent_operator.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1127 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/harmonics/tests/test_harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      441 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/tests/test_harmonics_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      439 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/harmonics/tests/test_harmonics_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.762782 multipie-1.0.1/multipie/harmonics/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/harmonics/util/equivalent_operator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.763842 multipie-1.0.1/multipie/model/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2149 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/construct_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/model/create_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    29773 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/material_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/multipie_manager.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    17710 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/symmetry_adapted_model.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.764481 multipie-1.0.1/multipie/model/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8278 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/model/tests/model_example.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2580 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/tests/test_construct_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      442 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/model/tests/test_material_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      542 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/model/tests/test_material_viewer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.764969 multipie-1.0.1/multipie/model/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/util/atomic_matrix_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    25780 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/util/create_pdf.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    24331 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/model/util/symmetry_adapted_model_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.723454 multipie-1.0.1/multipie/multipole/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.765399 multipie-1.0.1/multipie/multipole/base/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/multipole/base/base_atomic_multipole_dataset.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/multipole/base/base_atomic_multipole_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.765865 multipie-1.0.1/multipie/multipole/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2797 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/multipole/tests/test_atomic_orbital_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      447 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/multipole/tests/test_base_atomic_multipole_dataset.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      421 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/multipole/tests/test_base_atomic_multipole_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.766990 multipie-1.0.1/multipie/multipole/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14659 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/multipole/util/atomic_orbital_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7216 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/multipole/util/atomic_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/multipole/util/multipole_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/multipole/util/pauli.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/multipole/util/spin_orbital_basis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/multipole/util/structure_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/multipole/util/z_samb_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.767297 multipie-1.0.1/multipie/response_tensor/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/response_tensor/response_tensor_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/response_tensor/response_tensor_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.767608 multipie-1.0.1/multipie/response_tensor/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      307 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/response_tensor/tests/test_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4692 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/response_tensor/tests/test_response_tensor_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.767751 multipie-1.0.1/multipie/response_tensor/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/response_tensor/util/response_tensor_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.768059 multipie-1.0.1/multipie/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.0.1/multipie/scripts/create_binary.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1541 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/scripts/create_samb.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.768649 multipie-1.0.1/multipie/symmetry_operation/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/symmetry_operation/symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/symmetry_operation/symmetry_operation_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/symmetry_operation/symmetry_operation_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.769312 multipie-1.0.1/multipie/symmetry_operation/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1548 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1607 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      531 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation_g_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1281 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.769450 multipie-1.0.1/multipie/symmetry_operation/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/symmetry_operation/util/symmetry_operation_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.770531 multipie-1.0.1/multipie/tag/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_list.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_multipole.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tag_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.771352 multipie-1.0.1/multipie/tag/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1108 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tests/test_tag_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      736 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tests/test_tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1441 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tests/test_tag_multipole.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1297 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tests/test_tag_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1797 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tests/test_tag_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      624 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/tag/tests/test_tag_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.771652 multipie-1.0.1/multipie/virtual_cluster/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.772027 multipie-1.0.1/multipie/virtual_cluster/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      555 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/virtual_cluster/tests/test_virtual_cluster_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      480 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/virtual_cluster/tests/test_virtual_cluster_pg_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/virtual_cluster/virtual_cluster_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/virtual_cluster/virtual_cluster_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.772313 multipie-1.0.1/multipie/wyckoff/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.772595 multipie-1.0.1/multipie/wyckoff/tests/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      691 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/wyckoff/tests/test_wyckoff_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      500 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/wyckoff/tests/test_wyckoff_g_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.0.1/multipie/wyckoff/wyckoff_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.0.1/multipie/wyckoff/wyckoff_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.730718 multipie-1.0.1/multipie.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2086 2023-05-15 16:53:40.000000 multipie-1.0.1/multipie.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     5986 2023-05-15 16:53:40.000000 multipie-1.0.1/multipie.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-15 16:53:40.000000 multipie-1.0.1/multipie.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      116 2023-05-15 16:53:40.000000 multipie-1.0.1/multipie.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       71 2023-05-15 16:53:40.000000 multipie-1.0.1/multipie.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        9 2023-05-15 16:53:40.000000 multipie-1.0.1/multipie.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      876 2023-05-15 16:53:40.774728 multipie-1.0.1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.0.1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.725439 multipie-1.0.1/tools/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.772991 multipie-1.0.1/tools/data/
+-rw-r--r--   0 hiro       (501) staff       (20)     5398 2023-05-09 15:21:28.000000 multipie-1.0.1/tools/data/create_data_atomic_multipoles.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2794 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/data/create_data_real_harmonics.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1718 2023-05-09 15:21:28.000000 multipie-1.0.1/tools/data/create_data_virtual_cluster.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.773233 multipie-1.0.1/tools/data/util/
+-rw-r--r--   0 hiro       (501) staff       (20)    13042 2023-05-09 15:21:28.000000 multipie-1.0.1/tools/data/util/atomic_multipole_matrix.py
+-rw-r--r--   0 hiro       (501) staff       (20)      273 2023-05-09 15:21:28.000000 multipie-1.0.1/tools/data/util/output_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-15 16:53:40.774094 multipie-1.0.1/tools/pdf/
+-rw-r--r--   0 hiro       (501) staff       (20)     3628 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_atomic_multipole.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3589 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_character.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2386 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_harmonics.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1861 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_response_tensor.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4578 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_symmetry_operation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1572 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_virtual_cluster.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1989 2023-05-15 15:10:01.000000 multipie-1.0.1/tools/pdf/create_pdf_wyckoff.py
```

### Comparing `multipie-1.0.0/LICENSE` & `multipie-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/PKG-INFO` & `multipie-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.0.0/README.md` & `multipie-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/doc/Makefile` & `multipie-1.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/doc/source/conf.py` & `multipie-1.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/doc/source/model.rst` & `multipie-1.0.1/doc/source/model.rst`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/doc/source/tag.rst` & `multipie-1.0.1/doc/source/tag.rst`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/__init__.py` & `multipie-1.0.1/multipie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __top_dir__ = os.path.normpath(os.path.dirname(__file__) + "/../") + "/"
 __bin_dir__ = __top_dir__ + "multipie/binary_data/"
 
 
 # ==================================================
 from gcoreutils.string_util import class_name
 from gcoreutils.binary_manager import BinaryManager
```

### Comparing `multipie-1.0.0/multipie/binary_data/BaseAtomicMultipoleDataset.pkl` & `multipie-1.0.1/multipie/binary_data/BaseAtomicMultipoleDataset.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/CharacterPGSet.pkl` & `multipie-1.0.1/multipie/binary_data/CharacterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/ClebschGordanPGSet.pkl` & `multipie-1.0.1/multipie/binary_data/ClebschGordanPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/HarmonicsPGSet.pkl` & `multipie-1.0.1/multipie/binary_data/HarmonicsPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/ResponseTensorPGSet.pkl` & `multipie-1.0.1/multipie/binary_data/ResponseTensorPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/SymmetryOperationGSet.pkl` & `multipie-1.0.1/multipie/binary_data/SymmetryOperationGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/VirtualClusterPGSet.pkl` & `multipie-1.0.1/multipie/binary_data/VirtualClusterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/binary_data/WyckoffGSet.pkl` & `multipie-1.0.1/multipie/binary_data/WyckoffGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/character/character_pg.py` & `multipie-1.0.1/multipie/character/character_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/character/character_pg_set.py` & `multipie-1.0.1/multipie/character/character_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/character/tests/test_character_pg.py` & `multipie-1.0.1/multipie/character/tests/test_character_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/character/tests/test_character_pg_set.py` & `multipie-1.0.1/multipie/character/tests/test_character_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/clebsch_gordan/clebsch_gordan_pg.py` & `multipie-1.0.1/multipie/clebsch_gordan/clebsch_gordan_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/clebsch_gordan/clebsch_gordan_pg_set.py` & `multipie-1.0.1/multipie/clebsch_gordan/clebsch_gordan_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg.py` & `multipie-1.0.1/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg_set.py` & `multipie-1.0.1/multipie/clebsch_gordan/tests/test_clebsch_gordan_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/const.py` & `multipie-1.0.1/multipie/const.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_atomic_multipoles.py` & `multipie-1.0.1/multipie/data/data_atomic_multipoles.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_cartesian_to_ch_harmoncis.py` & `multipie-1.0.1/multipie/data/data_cartesian_to_ch_harmoncis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_character_table.py` & `multipie-1.0.1/multipie/data/data_character_table.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_compatibility_relation.py` & `multipie-1.0.1/multipie/data/data_compatibility_relation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_harmonics.py` & `multipie-1.0.1/multipie/data/data_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_harmonics_real.py` & `multipie-1.0.1/multipie/data/data_harmonics_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_no_space_group.py` & `multipie-1.0.1/multipie/data/data_no_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_product_decomp.py` & `multipie-1.0.1/multipie/data/data_product_decomp.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_symmetry_operation_pg.py` & `multipie-1.0.1/multipie/data/data_symmetry_operation_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_symmetry_operation_sg.py` & `multipie-1.0.1/multipie/data/data_symmetry_operation_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_tag_harmonics_alias.py` & `multipie-1.0.1/multipie/data/data_tag_harmonics_alias.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_tag_irrep.py` & `multipie-1.0.1/multipie/data/data_tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_tag_point_group.py` & `multipie-1.0.1/multipie/data/data_tag_point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_tag_space_group.py` & `multipie-1.0.1/multipie/data/data_tag_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_transform_matrix.py` & `multipie-1.0.1/multipie/data/data_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_virtual_cluster_real.py` & `multipie-1.0.1/multipie/data/data_virtual_cluster_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_wyckoff_pg.py` & `multipie-1.0.1/multipie/data/data_wyckoff_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/data/data_wyckoff_sg.py` & `multipie-1.0.1/multipie/data/data_wyckoff_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/examples/models/te.py` & `multipie-1.0.1/multipie/examples/models/te.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/group/point_group.py` & `multipie-1.0.1/multipie/group/point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/group/space_group.py` & `multipie-1.0.1/multipie/group/space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/group/tests/test_point_group.py` & `multipie-1.0.1/multipie/group/tests/test_point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/group/tests/test_space_group.py` & `multipie-1.0.1/multipie/group/tests/test_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/harmonics.py` & `multipie-1.0.1/multipie/harmonics/harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/harmonics_complex_pg.py` & `multipie-1.0.1/multipie/harmonics/harmonics_complex_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/harmonics_complex_pg_set.py` & `multipie-1.0.1/multipie/harmonics/harmonics_complex_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/harmonics_pg.py` & `multipie-1.0.1/multipie/harmonics/harmonics_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/harmonics_pg_set.py` & `multipie-1.0.1/multipie/harmonics/harmonics_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/tests/test_equivalent_operator.py` & `multipie-1.0.1/multipie/harmonics/tests/test_equivalent_operator.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/tests/test_harmonics.py` & `multipie-1.0.1/multipie/harmonics/tests/test_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/harmonics/util/equivalent_operator.py` & `multipie-1.0.1/multipie/harmonics/util/equivalent_operator.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/construct_model.py` & `multipie-1.0.1/multipie/model/construct_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/create_model.py` & `multipie-1.0.1/multipie/model/create_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/material_model.py` & `multipie-1.0.1/multipie/model/material_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/multipie_manager.py` & `multipie-1.0.1/multipie/model/multipie_manager.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/symmetry_adapted_model.py` & `multipie-1.0.1/multipie/model/symmetry_adapted_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/tests/model_example.py` & `multipie-1.0.1/multipie/model/tests/model_example.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/tests/test_construct_model.py` & `multipie-1.0.1/multipie/model/tests/test_construct_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/tests/test_material_viewer.py` & `multipie-1.0.1/multipie/model/tests/test_material_viewer.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/util/create_pdf.py` & `multipie-1.0.1/multipie/model/util/create_pdf.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/model/util/symmetry_adapted_model_util.py` & `multipie-1.0.1/multipie/model/util/symmetry_adapted_model_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/base/base_atomic_multipole_dataset.py` & `multipie-1.0.1/multipie/multipole/base/base_atomic_multipole_dataset.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/base/base_atomic_multipole_set.py` & `multipie-1.0.1/multipie/multipole/base/base_atomic_multipole_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/tests/test_atomic_orbital_util.py` & `multipie-1.0.1/multipie/multipole/tests/test_atomic_orbital_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/atomic_orbital_util.py` & `multipie-1.0.1/multipie/multipole/util/atomic_orbital_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/atomic_samb_util.py` & `multipie-1.0.1/multipie/multipole/util/atomic_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/multipole_util.py` & `multipie-1.0.1/multipie/multipole/util/multipole_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/pauli.py` & `multipie-1.0.1/multipie/multipole/util/pauli.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/spin_orbital_basis.py` & `multipie-1.0.1/multipie/multipole/util/spin_orbital_basis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/structure_samb_util.py` & `multipie-1.0.1/multipie/multipole/util/structure_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/multipole/util/z_samb_util.py` & `multipie-1.0.1/multipie/multipole/util/z_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/response_tensor/response_tensor_pg.py` & `multipie-1.0.1/multipie/response_tensor/response_tensor_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/response_tensor/response_tensor_pg_set.py` & `multipie-1.0.1/multipie/response_tensor/response_tensor_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/response_tensor/tests/test_response_tensor_util.py` & `multipie-1.0.1/multipie/response_tensor/tests/test_response_tensor_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/response_tensor/util/response_tensor_util.py` & `multipie-1.0.1/multipie/response_tensor/util/response_tensor_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/scripts/create_binary.py` & `multipie-1.0.1/multipie/scripts/create_binary.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/scripts/create_samb.py` & `multipie-1.0.1/multipie/scripts/create_samb.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/symmetry_operation.py` & `multipie-1.0.1/multipie/symmetry_operation/symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/symmetry_operation_g.py` & `multipie-1.0.1/multipie/symmetry_operation/symmetry_operation_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/symmetry_operation_g_set.py` & `multipie-1.0.1/multipie/symmetry_operation/symmetry_operation_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation.py` & `multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation_g.py` & `multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation_g_set.py` & `multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/tests/test_symmetry_operation_util.py` & `multipie-1.0.1/multipie/symmetry_operation/tests/test_symmetry_operation_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/symmetry_operation/util/symmetry_operation_util.py` & `multipie-1.0.1/multipie/symmetry_operation/util/symmetry_operation_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag.py` & `multipie-1.0.1/multipie/tag/tag.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_group.py` & `multipie-1.0.1/multipie/tag/tag_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_irrep.py` & `multipie-1.0.1/multipie/tag/tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_list.py` & `multipie-1.0.1/multipie/tag/tag_list.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_multipole.py` & `multipie-1.0.1/multipie/tag/tag_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_response_tensor.py` & `multipie-1.0.1/multipie/tag/tag_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_symmetry_operation.py` & `multipie-1.0.1/multipie/tag/tag_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tag_wyckoff.py` & `multipie-1.0.1/multipie/tag/tag_wyckoff.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tests/test_tag_group.py` & `multipie-1.0.1/multipie/tag/tests/test_tag_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tests/test_tag_irrep.py` & `multipie-1.0.1/multipie/tag/tests/test_tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tests/test_tag_multipole.py` & `multipie-1.0.1/multipie/tag/tests/test_tag_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tests/test_tag_response_tensor.py` & `multipie-1.0.1/multipie/tag/tests/test_tag_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tests/test_tag_symmetry_operation.py` & `multipie-1.0.1/multipie/tag/tests/test_tag_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/tag/tests/test_tag_wyckoff.py` & `multipie-1.0.1/multipie/tag/tests/test_tag_wyckoff.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/virtual_cluster/tests/test_virtual_cluster_pg.py` & `multipie-1.0.1/multipie/virtual_cluster/tests/test_virtual_cluster_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/virtual_cluster/virtual_cluster_pg.py` & `multipie-1.0.1/multipie/virtual_cluster/virtual_cluster_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/virtual_cluster/virtual_cluster_pg_set.py` & `multipie-1.0.1/multipie/virtual_cluster/virtual_cluster_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/wyckoff/tests/test_wyckoff_g.py` & `multipie-1.0.1/multipie/wyckoff/tests/test_wyckoff_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/wyckoff/wyckoff_g.py` & `multipie-1.0.1/multipie/wyckoff/wyckoff_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie/wyckoff/wyckoff_g_set.py` & `multipie-1.0.1/multipie/wyckoff/wyckoff_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/multipie.egg-info/PKG-INFO` & `multipie-1.0.1/multipie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.0.0/multipie.egg-info/SOURCES.txt` & `multipie-1.0.1/multipie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/setup.cfg` & `multipie-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/data/create_data_atomic_multipoles.py` & `multipie-1.0.1/tools/data/create_data_atomic_multipoles.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/data/create_data_real_harmonics.py` & `multipie-1.0.1/tools/data/create_data_real_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/data/create_data_virtual_cluster.py` & `multipie-1.0.1/tools/data/create_data_virtual_cluster.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/data/util/atomic_multipole_matrix.py` & `multipie-1.0.1/tools/data/util/atomic_multipole_matrix.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_atomic_multipole.py` & `multipie-1.0.1/tools/pdf/create_pdf_atomic_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_character.py` & `multipie-1.0.1/tools/pdf/create_pdf_character.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_harmonics.py` & `multipie-1.0.1/tools/pdf/create_pdf_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_response_tensor.py` & `multipie-1.0.1/tools/pdf/create_pdf_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_symmetry_operation.py` & `multipie-1.0.1/tools/pdf/create_pdf_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_virtual_cluster.py` & `multipie-1.0.1/tools/pdf/create_pdf_virtual_cluster.py`

 * *Files identical despite different names*

### Comparing `multipie-1.0.0/tools/pdf/create_pdf_wyckoff.py` & `multipie-1.0.1/tools/pdf/create_pdf_wyckoff.py`

 * *Files identical despite different names*

