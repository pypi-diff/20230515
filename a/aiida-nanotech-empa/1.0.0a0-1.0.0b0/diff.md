# Comparing `tmp/aiida-nanotech-empa-1.0.0a0.tar.gz` & `tmp/aiida_nanotech_empa-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-nanotech-empa-1.0.0a0.tar", last modified: Sat Jan 14 11:26:59 2023, max compression
+gzip compressed data, was "aiida_nanotech_empa-1.0.0b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-nanotech-empa-1.0.0a0.tar` & `aiida_nanotech_empa-1.0.0b0.tar`

### file list

```diff
@@ -1,90 +1,121 @@
--rw-r--r--   0        0        0       13 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.codecov.yml
--rw-r--r--   0        0        0       33 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.coveragerc
--rw-r--r--   0        0        0       52 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.flake8
--rw-r--r--   0        0        0      200 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.github/install_cp2k.sh
--rw-r--r--   0        0        0      289 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.github/install_qe.sh
--rw-r--r--   0        0        0     1721 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      795 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      135 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.gitignore
--rw-r--r--   0        0        0     1629 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     2125 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/README.md
--rw-r--r--   0        0        0      189 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/__init__.py
--rw-r--r--   0        0        0        0 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/__init__.py
--rw-r--r--   0        0        0     9880 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
--rw-r--r--   0        0        0     2545 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
--rw-r--r--   0        0        0     1679 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
--rw-r--r--   0        0        0     1490 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/pp_parser.py
--rw-r--r--   0        0        0        0 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/schedulers/__init__.py
--rw-r--r--   0        0        0     1520 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
--rw-r--r--   0        0        0        0 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/__init__.py
--rw-r--r--   0        0        0    15838 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/analyze_structure.py
--rw-r--r--   0        0        0     1126 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/common_utils.py
--rw-r--r--   0        0        0     2779 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/cube_utils.py
--rw-r--r--   0        0        0    10004 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
--rw-r--r--   0        0        0    10035 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/igor.py
--rw-r--r--   0        0        0     5432 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/pymol_render.py
--rw-r--r--   0        0        0     8574 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/stm_tools.py
--rw-r--r--   0        0        0      103 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/version.py
--rw-r--r--   0        0        0        0 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/__init__.py
--rw-r--r--   0        0        0    12136 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
--rw-r--r--   0        0        0     6986 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/bulk_opt_workchain.py
--rw-r--r--   0        0        0     6593 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
--rw-r--r--   0        0        0     2627 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
--rw-r--r--   0        0        0     2333 2023-01-14 11:26:56.167808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
--rw-r--r--   0        0        0   135679 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
--rw-r--r--   0        0        0   114564 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
--rw-r--r--   0        0        0   172445 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
--rw-r--r--   0        0        0   135561 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
--rw-r--r--   0        0        0      378 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
--rw-r--r--   0        0        0   154582 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
--rw-r--r--   0        0        0     8385 2023-01-14 11:26:56.171808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
--rw-r--r--   0        0        0  1959318 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
--rw-r--r--   0        0        0    13544 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
--rw-r--r--   0        0        0    12255 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
--rw-r--r--   0        0        0     6422 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
--rw-r--r--   0        0        0     6175 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_workchain.py
--rw-r--r--   0        0        0     7790 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/bulk_opt_protocol.yml
--rw-r--r--   0        0        0     8126 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
--rw-r--r--   0        0        0    11446 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
--rw-r--r--   0        0        0     7860 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/molecule_opt_protocol.yml
--rw-r--r--   0        0        0     7790 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/slab_opt_protocol.yml
--rw-r--r--   0        0        0     6877 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/slab_opt_workchain.py
--rw-r--r--   0        0        0      812 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/__init__.py
--rw-r--r--   0        0        0     9657 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
--rw-r--r--   0        0        0     9008 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
--rw-r--r--   0        0        0     6185 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/common.py
--rw-r--r--   0        0        0     6594 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
--rw-r--r--   0        0        0     8362 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
--rw-r--r--   0        0        0     5560 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
--rw-r--r--   0        0        0    11300 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
--rw-r--r--   0        0        0    12090 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
--rw-r--r--   0        0        0    12036 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
--rw-r--r--   0        0        0    11853 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
--rw-r--r--   0        0        0        0 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/qe/__init__.py
--rw-r--r--   0        0        0    24245 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/qe/nanoribbon.py
--rw-r--r--   0        0        0     3370 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/conftest.py
--rw-r--r--   0        0        0       96 2023-01-14 11:26:56.179808 aiida-nanotech-empa-1.0.0a0/examples/__init__.py
--rw-r--r--   0        0        0   921233 2023-01-14 11:26:56.183809 aiida-nanotech-empa-1.0.0a0/examples/data/sssp_minimal/C.upf
--rw-r--r--   0        0        0   366195 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/data/sssp_minimal/H.upf
--rw-r--r--   0        0        0       13 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/.gitignore
--rw-r--r--   0        0        0      558 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/benzene-diradical.xyz
--rw-r--r--   0        0        0      422 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/c2h2_no_spin.xyz
--rw-r--r--   0        0        0      467 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/c2h2_spin.xyz
--rw-r--r--   0        0        0     2621 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_ads_gw_ic.py
--rw-r--r--   0        0        0     2085 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_bulkopt.py
--rw-r--r--   0        0        0     2661 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_fragment_separation.py
--rw-r--r--   0        0        0     3179 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_gw.py
--rw-r--r--   0        0        0     1935 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_mol_opt_gw.py
--rw-r--r--   0        0        0     1656 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_molopt.py
--rw-r--r--   0        0        0     1727 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_slabopt.py
--rw-r--r--   0        0        0     2146 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_gaussian_casscf.py
--rw-r--r--   0        0        0     1394 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_gaussian_spin.py
--rw-r--r--   0        0        0     2777 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/example_nanoribbon.py
--rw-r--r--   0        0        0     2530 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/h2_on_au111.xyz
--rw-r--r--   0        0        0     1568 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/h2_on_hbn.xyz
--rw-r--r--   0        0        0      679 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/examples/workflows/si_bulk.xyz
--rw-r--r--   0        0        0     4003 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      253 2023-01-14 11:26:56.187809 aiida-nanotech-empa-1.0.0a0/pytest.ini
--rw-r--r--   0        0        0     3471 1970-01-01 00:00:00.000000 aiida-nanotech-empa-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.codecov.yml
+-rw-r--r--   0        0        0       33 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.coveragerc
+-rw-r--r--   0        0        0       52 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.flake8
+-rw-r--r--   0        0        0      200 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.github/install_cp2k.sh
+-rw-r--r--   0        0        0      289 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.github/install_qe.sh
+-rw-r--r--   0        0        0     1737 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      795 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      135 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.gitignore
+-rw-r--r--   0        0        0     1628 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0     2125 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/README.md
+-rw-r--r--   0        0        0      189 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/helpers.py
+-rw-r--r--   0        0        0      273 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/__init__.py
+-rw-r--r--   0        0        0     9867 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
+-rw-r--r--   0        0        0     4706 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
+-rw-r--r--   0        0        0     2542 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
+-rw-r--r--   0        0        0     1678 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
+-rw-r--r--   0        0        0     1379 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/pp_parser.py
+-rw-r--r--   0        0        0      230 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/afm.py
+-rw-r--r--   0        0        0     2951 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/hrstm.py
+-rw-r--r--   0        0        0     3542 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/overlap.py
+-rw-r--r--   0        0        0     2863 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/stm.py
+-rw-r--r--   0        0        0      168 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/__init__.py
+-rw-r--r--   0        0        0     1523 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
+-rw-r--r--   0        0        0     1599 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/__init__.py
+-rw-r--r--   0        0        0    15829 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/analyze_structure.py
+-rw-r--r--   0        0        0     1375 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/common_utils.py
+-rw-r--r--   0        0        0     2736 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/cube_utils.py
+-rw-r--r--   0        0        0     9994 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
+-rw-r--r--   0        0        0    10034 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/igor.py
+-rw-r--r--   0        0        0     5427 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/pymol_render.py
+-rw-r--r--   0        0        0     8560 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/stm_tools.py
+-rw-r--r--   0        0        0      103 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/version.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/__init__.py
+-rw-r--r--   0        0        0    12242 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
+-rw-r--r--   0        0        0     5908 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
+-rw-r--r--   0        0        0    30468 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
+-rw-r--r--   0        0        0     2627 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
+-rw-r--r--   0        0        0     2333 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
+-rw-r--r--   0        0        0   135679 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
+-rw-r--r--   0        0        0   114564 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
+-rw-r--r--   0        0        0   172445 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
+-rw-r--r--   0        0        0   135561 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
+-rw-r--r--   0        0        0      378 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
+-rw-r--r--   0        0        0   154582 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
+-rw-r--r--   0        0        0     8385 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
+-rw-r--r--   0        0        0    10869 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
+-rw-r--r--   0        0        0    10601 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
+-rw-r--r--   0        0        0  1959318 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
+-rw-r--r--   0        0        0    10100 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
+-rw-r--r--   0        0        0    13286 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
+-rw-r--r--   0        0        0     8261 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
+-rw-r--r--   0        0        0     5417 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
+-rw-r--r--   0        0        0    12131 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
+-rw-r--r--   0        0        0     6432 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
+-rw-r--r--   0        0        0     9959 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
+-rw-r--r--   0        0        0     3893 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
+-rw-r--r--   0        0        0     6771 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
+-rw-r--r--   0        0        0     5579 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
+-rw-r--r--   0        0        0     1252 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
+-rw-r--r--   0        0        0    12253 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
+-rw-r--r--   0        0        0    11446 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
+-rw-r--r--   0        0        0     7983 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
+-rw-r--r--   0        0        0     9918 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
+-rw-r--r--   0        0        0     1966 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
+-rw-r--r--   0        0        0     7603 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
+-rw-r--r--   0        0        0    14363 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
+-rw-r--r--   0        0        0     4085 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
+-rw-r--r--   0        0        0      812 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/__init__.py
+-rw-r--r--   0        0        0     9185 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
+-rw-r--r--   0        0        0     8919 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
+-rw-r--r--   0        0        0     6083 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/common.py
+-rw-r--r--   0        0        0     6708 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
+-rw-r--r--   0        0        0     7953 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
+-rw-r--r--   0        0        0     5234 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
+-rw-r--r--   0        0        0    11073 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
+-rw-r--r--   0        0        0    12134 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
+-rw-r--r--   0        0        0    11760 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
+-rw-r--r--   0        0        0    11519 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
+-rw-r--r--   0        0        0       80 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/qe/__init__.py
+-rw-r--r--   0        0        0    22418 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/qe/nanoribbon.py
+-rw-r--r--   0        0        0     3369 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/conftest.py
+-rw-r--r--   0        0        0       96 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/examples/__init__.py
+-rw-r--r--   0        0        0   921233 2023-05-15 10:57:57.009751 aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/C.upf
+-rw-r--r--   0        0        0   366195 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/H.upf
+-rw-r--r--   0        0        0       13 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/.gitignore
+-rwxr-xr-x   0        0        0     9833 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/aa
+-rw-r--r--   0        0        0      558 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/benzene-diradical.xyz
+-rw-r--r--   0        0        0      402 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2.xyz
+-rw-r--r--   0        0        0      422 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_no_spin.xyz
+-rw-r--r--   0        0        0     2959 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_on_au111.xyz
+-rw-r--r--   0        0        0      467 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_spin.xyz
+-rw-r--r--   0        0        0      572 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h4.xyz
+-rw-r--r--   0        0        0     2533 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_ads_gw_ic.py
+-rw-r--r--   0        0        0     4739 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_afm.py
+-rw-r--r--   0        0        0     2725 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_diag.py
+-rw-r--r--   0        0        0     3169 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_fragment_separation.py
+-rw-r--r--   0        0        0     4118 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_geo_opt.py
+-rw-r--r--   0        0        0     3177 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_gw.py
+-rw-r--r--   0        0        0     5394 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_hrstm.py
+-rw-r--r--   0        0        0     1934 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_mol_opt_gw.py
+-rw-r--r--   0        0        0     5582 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_neb.py
+-rw-r--r--   0        0        0     3513 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_orb.py
+-rw-r--r--   0        0        0     4089 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_pdos.py
+-rw-r--r--   0        0        0     2742 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_phonons.py
+-rw-r--r--   0        0        0     2622 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_replica_chain.py
+-rw-r--r--   0        0        0     3446 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_stm.py
+-rw-r--r--   0        0        0     2145 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_casscf.py
+-rw-r--r--   0        0        0     1393 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_spin.py
+-rw-r--r--   0        0        0     2776 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_nanoribbon.py
+-rw-r--r--   0        0        0      251 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/h2.xyz
+-rw-r--r--   0        0        0     2483 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_au111.xyz
+-rw-r--r--   0        0        0     1568 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_hbn.xyz
+-rw-r--r--   0        0        0      679 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/si_bulk.xyz
+-rw-r--r--   0        0        0     4743 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0      253 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/pytest.ini
+-rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b0/PKG-INFO
```

### Comparing `aiida-nanotech-empa-1.0.0a0/.github/workflows/ci.yml` & `aiida_nanotech_empa-1.0.0b0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           - 5432:5432
       rabbitmq:
         image: rabbitmq:latest
         ports:
           - 5672:5672
     strategy:
       matrix:
-        python-version: ['3.8', '3.9']
+        python-version: ['3.8', '3.9', '3.10']
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
@@ -52,15 +52,15 @@
         file: ./coverage.xml
 
   pre-commit:
     runs-on: ubuntu-latest
     timeout-minutes: 15
     strategy:
       matrix:
-        python-version: ['3.8', '3.9']
+        python-version: ['3.8', '3.9', '3.10']
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `aiida-nanotech-empa-1.0.0a0/.github/workflows/publish.yml` & `aiida_nanotech_empa-1.0.0b0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/.pre-commit-config.yaml` & `aiida_nanotech_empa-1.0.0b0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -9,29 +9,29 @@
           - id: end-of-file-fixer
             exclude: ^.*data/
           - id: trailing-whitespace
             exclude: ^.*.upf
           - id: check-yaml
           - id: check-added-large-files
     - repo: https://github.com/pycqa/isort
-      rev: 5.11.4
+      rev: 5.12.0
       hooks:
           - id: isort
             args: [--profile, black, --filter-files]
     - repo: https://github.com/PyCQA/autoflake
-      rev: v2.0.0
+      rev: v2.0.2
       hooks:
           - id: autoflake
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.2.2
+      rev: v3.3.1
       hooks:
           - id: pyupgrade
-            args: [--py37-plus]
+            args: [--py38-plus]
     - repo: https://github.com/psf/black
-      rev: 22.12.0
+      rev: 23.3.0
       hooks:
           - id: black
             language_version: python3
     - repo: https://github.com/PyCQA/flake8
       rev: 6.0.0
       hooks:
           - id: flake8
@@ -42,15 +42,15 @@
                 - flake8-comprehensions
                 - flake8-debugger
                 - flake8-logging-format
                 - pep8-naming
                 - pyflakes
                 - tryceratops
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v0.961
+      rev: v1.1.1
       hooks:
           - id: mypy
             additional_dependencies:
                 - types-click-spinner
                 - types-requests
                 - types-tabulate
                 - types-toml
```

### Comparing `aiida-nanotech-empa-1.0.0a0/LICENSE` & `aiida_nanotech_empa-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/README.md` & `aiida_nanotech_empa-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/cp2k_gw_parser.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_gw_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """AiiDA-CP2K output parser for GW calculations."""
 
-from aiida.common import OutputParsingError
-from aiida.orm import Dict
+
+from aiida import common, orm
 from aiida_cp2k.parsers import Cp2kBaseParser
 from aiida_cp2k.utils import parse_cp2k_output_advanced
 
-HART_2_EV = 27.21138602
+from ..helpers import HART_2_EV
 
 
-class Cp2kNoOutputFileError(OutputParsingError):
+class Cp2kNoOutputFileError(common.OutputParsingError):
     def __init__(self):
         super().__init__("CP2K output file  not retrieved")
 
 
-class Cp2kDidNotFinishProperlyError(OutputParsingError):
+class Cp2kDidNotFinishProperlyError(common.OutputParsingError):
     def __init__(self):
         super().__init__("CP2K did not finish properly")
 
 
 def is_number(s):
     try:
         float(s)
     except ValueError:
         return False
     return True
 
 
-class Cp2kGWParser(Cp2kBaseParser):
+class Cp2kGwParser(Cp2kBaseParser):
     """AiiDA parser class for the output of CP2K GW calculations."""
 
     def _parse_stdout(self):
-
         fname = self.node.process_class._DEFAULT_OUTPUT_FILE
         if fname not in self.retrieved.base.repository.list_object_names():
             raise Cp2kNoOutputFileError()
 
         try:
             output_string = self.retrieved.base.repository.get_object_content(fname)
         except OSError:
@@ -48,19 +47,19 @@
         if "nwarnings" not in result_dict:
             raise Cp2kDidNotFinishProperlyError()
 
         if "aborted" in result_dict:
             return self.exit_codes.ERROR_OUTPUT_CONTAINS_ABORT
 
         # Standard output parameters
-        self.out("std_output_parameters", Dict(dict=result_dict))
+        self.out("std_output_parameters", orm.Dict(dict=result_dict))
 
         # Custom GW parsing
         gw_output_parameters = self._parse_cp2k_gw_output(output_string)
-        self.out("gw_output_parameters", Dict(dict=gw_output_parameters))
+        self.out("gw_output_parameters", orm.Dict(dict=gw_output_parameters))
 
         return None
 
     def _parse_cp2k_gw_output(self, output_string):  # noqa
         lines = output_string.splitlines()
 
         results = {}
@@ -136,15 +135,14 @@
                 gw_occ = []
                 gw_e_scf = []
                 gw_eval = []
 
                 while True:
                     line_loc = lines[i_line]
                     if "GW HOMO-LUMO gap" in line_loc:
-
                         spin = 1 if "Beta" in line_loc else 0
 
                         if len(results["mo"]) > spin:
                             # we already have a set, overwrite with later iteration
                             results["mo"][spin] = gw_mo
                             results["occ"][spin] = gw_occ
                             results["gw_eval"][spin] = gw_eval
@@ -181,15 +179,14 @@
                 ic_occ = []
                 ic_en = []
                 ic_delta = []
 
                 while True:
                     line_loc = lines[i_line]
                     if "IC HOMO-LUMO gap" in line_loc:
-
                         spin = 1 if "Beta" in line_loc else 0
 
                         if len(results["mo"]) > spin:
                             # we already have a set, overwrite with later iteration
                             results["mo"][spin] = ic_mo
                             results["occ"][spin] = ic_occ
                             results["ic_en"][spin] = ic_en
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,31 @@
 import aiida_nanotech_empa.utils.pymol_render as pr
 
 
 class CubegenPymolParser(CubegenBaseParser):
     """Cubegen parser based on pymol."""
 
     def _parse_folders(self, retrieved_folders, parser_params):
-
         # Parse constant-height planes based on the base parser
         super()._parse_folders(retrieved_folders, parser_params)
 
         # By default, don't re-orient cube
         orient_cube = False
         if "orient_cube" in parser_params:
             orient_cube = parser_params["orient_cube"]
 
         if "isovalues" in parser_params:
             isovalues = parser_params["isovalues"]
         else:
             isovalues = [0.01]
 
         with tempfile.TemporaryDirectory() as image_folder:
-
             for retrieved_fd in retrieved_folders:
                 for filename in retrieved_fd.list_object_names():
                     if filename.endswith(".cube"):
-
                         # AiiDA retrieved folder provides handles to retrieved files
                         # pymol rendering, however, requires the path to the cube file
                         # therefore, we need to write the contents to a temporary file
 
                         with retrieved_fd.open(filename) as handle:
                             cube = Cube.from_file_handle(handle)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-from aiida.orm import Dict, Float
+from aiida import orm
 from aiida_gaussian.parsers.gaussian import GaussianBaseParser
 
-HART_2_EV = 27.21138602
+from ..helpers import HART_2_EV
 
 
 class GaussianCasscfParser(GaussianBaseParser):
-    """
-    CASSCF AiiDA parser for the output of Gaussian
-    """
+    """AiiDA parser for Gaussian CASSCF calculations."""
 
     def _parse_log(self, log_file_string, _inputs):
-        """Overwrite the basic log parser"""
+        """Overwrite the basic log parser."""
 
-        # parse with cclib
+        # Parse with cclib.
         property_dict = self._parse_log_cclib(log_file_string)
 
         if property_dict is None:
             return self.exit_codes.ERROR_OUTPUT_PARSING
 
         property_dict.update(self._parse_electron_numbers(log_file_string))
 
         property_dict.update(self._parse_casscf(log_file_string))
 
-        self.out("output_parameters", Dict(dict=property_dict))
+        self.out("output_parameters", orm.Dict(dict=property_dict))
 
         if "casscf_energy_ev" in property_dict:
-            self.out("casscf_energy_ev", Float(property_dict["casscf_energy_ev"]))
+            self.out("casscf_energy_ev", orm.Float(property_dict["casscf_energy_ev"]))
         if "casmp2_energy_ev" in property_dict:
-            self.out("casmp2_energy_ev", Float(property_dict["casmp2_energy_ev"]))
+            self.out("casmp2_energy_ev", orm.Float(property_dict["casmp2_energy_ev"]))
 
         exit_code = self._final_checks_on_log(log_file_string, property_dict)
         if exit_code is not None:
             return exit_code
 
         return None
 
     def _parse_casscf(self, log_file_string):
-
         parsed_data = {}
 
         for line in log_file_string.splitlines():
             if "     eigenvalue " in line.lower():
                 parsed_data["casscf_energy_ev"] = (
                     float(line.split()[-1].replace("D", "E")) * HART_2_EV
                 )
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/parsers/pp_parser.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/pp_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-"""Parsers provided by aiida_nanotech_empa.
-
-Register parsers via the "aiida.parsers" entry point in setup.json.
-"""
 import io
 
 import numpy as np
 from aiida import orm
 from aiida_gaussian.utils.cube import Cube
 from aiida_quantumespresso.parsers.pp import PpParser as BasePpParser
 
 from aiida_nanotech_empa.utils.cube_utils import crop_cube
 
-ANG_TO_BOHR = 1.8897259886
+from ..helpers import ANG_TO_BOHR
 
 
 class PpParser(BasePpParser):
     """Reduce and parse Gaussian Cube formatted output.
     :param data_file_str: the data file read in as a single string
     """
 
     def parse_gaussian(self, data_file_str):
-
         with io.StringIO(data_file_str) as data_file_handle:
             cube = Cube.from_file_handle(data_file_handle)
 
         crop_cube(cube, x_crop=None, y_crop=1.8, z_crop=3.1)
 
         # Create the arraydata object
         coordinates_units = "bohr"
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,23 @@
             num_mpiprocs = job_tmpl.job_resource.get_tot_num_mpiprocs()
             mem_per_proc_mb = physical_memory_kb // (1024 * num_mpiprocs)
 
             rusage_added = False
             new_lines = []
             for line in lsf_script_lines:
                 if line.startswith("#BSUB -M"):
-                    # Skip the BSUB -M line
+                    # Skip the BSUB -M line.
                     continue
                 if not line.startswith("#") and not rusage_added:
-                    # Add the rusage line after the other #BSUB commands
+                    # Add the rusage line after the other #BSUB commands.
                     rusage_line = '#BSUB -R "rusage[mem={},scratch={}]"'.format(
                         mem_per_proc_mb, 2 * mem_per_proc_mb
                     )
                     new_lines.append(rusage_line)
                     rusage_added = True
 
                 new_lines.append(line)
 
             return "\n".join(new_lines)
 
-        # If memory is not specified, just use the default LSF script
+        # If memory is not specified, just use the default LSF script.
         return super()._get_submit_script_header(job_tmpl)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/analyze_structure.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/analyze_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import copy
 import itertools
-from copy import deepcopy
 
 import more_itertools as mit
 import numpy as np
 from ase import Atoms, neighborlist
 from scipy import sparse
 from scipy.signal import find_peaks
 from scipy.spatial import ConvexHull
@@ -224,15 +224,15 @@
         possible_mol_atoms += [i for i in range(nat) if atype[i] == 5]
         # identify separate molecules
         # all_molecules=self.molecules(mol_atoms,atoms)
         all_molecules = []
         if len(possible_mol_atoms) > 0:
             # conne = conne_matrix(frame[possible_mol_atoms])
             fragments = molecules(possible_mol_atoms, frame)
-            all_molecules = deepcopy(fragments)
+            all_molecules = copy.deepcopy(fragments)
             # remove isolated atoms
             for frag in fragments:
                 if len(frag) == 1:
                     all_molecules.remove(frag)
                 else:
                     for atom in frag:
                         if lbls[atom] in metalatingtypes:
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/cube_utils.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/cube_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-"""
-Routines regarding gaussian cube files
-"""
-
 import collections
 
 import ase
 import numpy as np
 from aiida_gaussian.utils.cube import Cube
 
-ANG_TO_BOHR = 1.8897259886
+from ..helpers import ANG_TO_BOHR
 
 
 def crop_cube(cube, x_crop=None, y_crop=None, z_crop=None):
     """
     Crops the extent of the cube file
 
     x_crop, y_crop, z_crop can be
@@ -36,15 +32,14 @@
     c_p1 = np.copy(i_p1)
 
     for i, i_crop in enumerate([x_crop, y_crop, z_crop]):
         pmax = np.max(cube.ase_atoms.positions[:, i])
         pmin = np.min(cube.ase_atoms.positions[:, i])
 
         if i_crop:
-
             if isinstance(i_crop, collections.abc.Iterable):
                 i_crop_ = i_crop
             else:
                 i_crop_ = [i_crop, i_crop]
 
             c_p0[i] = pmin - i_crop_[0]
             c_p1[i] = pmax + i_crop_[1]
@@ -71,15 +66,14 @@
 
     cube.origin = c_p0
     cube.cell = (np.atleast_2d(cube.data.shape).T * np.diag(dv)) * ANG_TO_BOHR
     cube.ase_atoms.positions = cube.ase_atoms.positions - cube.origin
 
 
 def cube_from_qe_pp_arraydata(ad):
-
     data_units = str(ad.get_array("data_units"))
     coord_units = str(ad.get_array("coordinates_units"))
     data = ad.get_array("data")
 
     coords = ad.get_array("coordinates")
     dv = ad.get_array("voxel")
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,36 +6,33 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image
 
 
 def select_frontier_orbital_energies(out_params, n_orb=4):
-
     nspin = len(out_params["homos"])
     mo_e = np.array(out_params["moenergies"])
 
     indexes = []
     energies = [[]]
     occs = [[]]
 
     if nspin == 1:
-
         homo_s0 = out_params["homos"][0]
 
         i_start = max(homo_s0 - n_orb, -1)
         i_end = min(homo_s0 + n_orb, len(mo_e[0]) - 1)
 
         for i_orb in range(i_end, i_start, -1):
             indexes.append(i_orb + 1)
             energies[0].append(mo_e[0][i_orb])
             occs[0].append(2 if i_orb <= homo_s0 else 0)
 
     elif nspin == 2:
-
         energies.append([])
         occs.append([])
 
         homo_s0 = out_params["homos"][0]
         homo_s1 = out_params["homos"][1]
 
         central_i = int(np.round((homo_s0 + homo_s1) / 2))
@@ -50,15 +47,14 @@
             occs[0].append(1 if i_orb <= homo_s0 else 0)
             occs[1].append(1 if i_orb <= homo_s1 else 0)
 
     return {"indexes": indexes, "energies": energies, "occs": occs}
 
 
 def _get_orb_energies_str(out_params, n_orb=4):
-
     orb_dict = select_frontier_orbital_energies(out_params, n_orb)
 
     inds = orb_dict["indexes"]
     ens = orb_dict["energies"]
     occs = orb_dict["occs"]
 
     nspin = len(orb_dict["energies"])
@@ -67,15 +63,14 @@
         header = "{:>10} {:>16} {:>6}".format("i_orb", "E (eV)", "occ")
         lines = [header]
 
         for z in zip(inds, ens[0], occs[0]):
             lines.append("{:>10} {:>16.4f} {:>6}".format(*z))
 
     elif nspin == 2:
-
         header = "{:>10} {:>16} {:>9} {:>16} {:>9}".format(
             "i_orb", "E(up) (eV)", "occ(up)", "E(down) (eV)", "occ(down)"
         )
         lines = [header]
 
         for z in zip(inds, ens[0], occs[0], ens[1], occs[1]):
             lines.append("{:>10} {:>16.4f} {:>9} {:>16.4f} {:>9}".format(*z))
@@ -117,15 +112,14 @@
     if "gap_a" in dict(out_params):
         s += "GAP alpha: {:.4f} eV\n".format(out_params["gap_a"])
         s += "GAP beta:  {:.4f} eV\n".format(out_params["gap_b"])
     return s
 
 
 def _get_natorb_analysis_str(natorb_params, out_params, n_orb=4):
-
     no_occs = natorb_params["no_occs"]
     no_occs_sp = natorb_params["no_occs_sp"]
 
     i_start = out_params["homos"][0] - n_orb
     i_end = out_params["homos"][0] + n_orb
 
     lines = ["{:>20} {:>16} {:>16}".format("i_no", "occ", "sp. proj. occ")]
@@ -158,22 +152,20 @@
 def plot_cube_images(
     cube_image_folder,
     name_contains=None,
     show=True,
     save_image_loc=None,
     save_prefix="",
 ):
-
     if name_contains is None:
         name_contains = ["z+"]
 
     rows = {}
     image_names = cube_image_folder.list_object_names()
     for imag_name in image_names:
-
         if not all(e in imag_name for e in name_contains):
             continue
 
         label = imag_name.split("_")[0]
         if label not in rows:
             rows[label] = []
         pil_image = get_pil_image(cube_image_folder, imag_name)
@@ -257,15 +249,14 @@
             _get_natorb_analysis_str(
                 dict(wc_node.outputs.gs_natorb_params), gs_out_params
             )
         )
     print()
 
     if "gs_hf_out_params" in wc_node.outputs:
-
         gs_hf_out_params = dict(wc_node.outputs.gs_hf_out_params)
 
         print("##############################################################")
         print("#### GROUND STATE HF")
         print("##############################################################")
 
         if "gs_hf_cube_images" in wc_node.outputs:
@@ -286,15 +277,14 @@
                 _get_natorb_analysis_str(
                     dict(wc_node.outputs.gs_hf_natorb_params), gs_hf_out_params
                 )
             )
         print()
 
     for mult in list(wc_node.inputs.multiplicity_list):
-
         if mult == gs_multiplicity:
             continue
 
         print("##############################################################")
         print(f"#### MULTIPLICITY {mult}")
         print("##############################################################")
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/igor.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/igor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 class MissingBeginError(OSError):
     def __init__(self, fname):
         super().__init__(f"Missing 'BEGIN' statement in {fname}.")
 
 
 def read_wave(lines, fname=None):
-
     line = lines.pop(0)
     while not re.match("WAVES", line):
         if len(lines) == 0:
             return None
         line = lines.pop(0)
     # 1d or 2d?
     d2 = False
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/pymol_render.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/pymol_render.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 
 _stdouterr = sys.stdout, sys.stderr
 pymol.finish_launching(["pymol", "-qc"])
 sys.stdout, sys.stderr = _stdouterr
 
 
 def _crop_image_bbox(filename):
-
     image = Image.open(filename)
 
     try:
         image = image.convert("RGBa")
         image = image.crop(image.getbbox())
     except ValueError:
         inv_image = ImageOps.invert(image)
         image = image.crop(inv_image.getbbox())
 
     image = image.convert("RGBA")
     image.save(filename)
 
 
 def _save_and_crop(fname, max_w, view):
-
     for _try in range(4):
         # Pymol sometimes creates the png with a delay
         # and sometimes even after a long delay, the image is not created
         # in this case, try to create the image again (loop over _try)
         pymol.cmd.png(fname, width=f"{max_w + 1}cm", dpi=500, ray=1)
         # Wait for a bit
         for _i in range(200):
@@ -61,15 +59,14 @@
     input_file,
     isov=0.05,
     colors=("brightorange", "marine"),
     output_folder=".",
     output_name=None,
     orientations=("z", "y", "x"),
 ):
-
     pymol.cmd.delete("all")
 
     # ------------------------------------
     # General PYMOL settings
 
     # Transparency settings
     pymol.cmd.set(name="transparency_mode", value=1)
@@ -83,15 +80,14 @@
 
     pymol.cmd.set("specular", 0.3)
 
     filepath, ext = os.path.splitext(input_file)
     filename = os.path.basename(filepath)
 
     if ext == ".cube":
-
         # Geometry from cube.
         ase_geom = Cube.from_file(input_file, read_data=False).ase_atoms
         with tempfile.NamedTemporaryFile(delete=False, mode="w") as tempf:
             ase_geom.write(tempf.name, format="xyz")
             tempf.close()
             pymol.cmd.load(tempf.name, format="xyz")
 
@@ -103,15 +99,14 @@
         pymol.cmd.set(name="transparency", value=0.0, selection="%pos_1")
 
         pymol.cmd.isosurface("neg_1", "cube", -isov)
         pymol.cmd.set(name="surface_color", value=colors[1], selection="%neg_1")
         pymol.cmd.set(name="transparency", value=0.0, selection="%neg_1")
 
     elif ext == ".xyz":
-
         ase_geom = ase.io.read(input_file)
         pymol.cmd.load(input_file)
 
     x_w = np.ptp(ase_geom.positions[:, 0])
     y_w = np.ptp(ase_geom.positions[:, 1])
     z_w = np.ptp(ase_geom.positions[:, 2])
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/utils/stm_tools.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/stm_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from . import igor
-
-ang_2_bohr = 1.0 / 0.52917721067
-hart_2_ev = 27.21138602
+from .helpers import ANG_TO_BOHR, HART_2_EV
 
 
 def process_cube_planes_array(cpa):
     x_arr = cpa.get_array("x_arr")
     y_arr = cpa.get_array("y_arr")
     h_arr = cpa.get_array("h_arr")
 
@@ -58,19 +56,19 @@
 def extrapolate_morb(orb_plane, dx, dy, energy_wrt_vacuum, delta_h):
     """
     dx, dy, delta_h - in ang
     energy_wrt_vacuum - in eV
     """
 
     # Convert everything to a.u.
-    dx = dx * ang_2_bohr
-    dy = dy * ang_2_bohr
-    delta_h = delta_h * ang_2_bohr
+    dx = dx * ANG_TO_BOHR
+    dy = dy * ANG_TO_BOHR
+    delta_h = delta_h * ANG_TO_BOHR
 
-    energy_wrt_vacuum = energy_wrt_vacuum / hart_2_ev
+    energy_wrt_vacuum = energy_wrt_vacuum / HART_2_EV
 
     if energy_wrt_vacuum >= 0.0:
         print("Warning: unbound state, can't extrapolate! Constant extrapolation.")
         energy_wrt_vacuum = 0.0
 
     fourier = np.fft.rfft2(orb_plane)
     # NB: rfft2 takes REAL fourier transform over last (y) axis and COMPLEX over other (x) axes
@@ -124,17 +122,15 @@
     energies = sop["moenergies"]
     nspin = len(sop["moenergies"])
 
     final_map = None
 
     for i_spin in range(nspin):
         for i_mo, e in enumerate(energies[i_spin]):
-
             if np.abs(e - energy) <= 1.5 * fwhm:
-
                 broad_coef = gaussian(e - energy, fwhm)
 
                 if i_mo not in cpa_dict["mo_planes"]:
                     print(
                         f"Missing MO{i_mo}, that potentially contributes to sts at E={energy}"
                     )
                     continue
@@ -145,15 +141,14 @@
                     final_map = broad_coef * orb_map**2
                 else:
                     final_map += broad_coef * orb_map**2
     return final_map
 
 
 def save_figure_and_igor(data_2d, filename, title, **imshow_args):
-
     plt.figure(figsize=(5, 5))
     plt.imshow(data_2d.T, **imshow_args)
     plt.title(title)
     plt.savefig(filename + ".png", dpi=250, bbox_inches="tight")
     plt.close()
 
     extent = imshow_args["extent"]
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
-from aiida.engine import ExitCode, ToContext, WorkChain, calcfunction, if_
-from aiida.orm import Bool, Code, Dict, Float, Int, List, Str, StructureData
+from aiida import engine, orm
 
+from .geo_opt_workchain import Cp2kGeoOptWorkChain
 from .molecule_gw_workchain import Cp2kMoleculeGwWorkChain
-from .molecule_opt_workchain import Cp2kMoleculeOptWorkChain
 
 IC_PLANE_HEIGHTS = {
     "Au(111)": 1.42,  # Kharche J. Phys. Chem. Lett. 7, 1526–1533 (2016).
 }
 
 
 def geometrical_analysis(ase_geo, substr_elem):
@@ -27,25 +26,26 @@
     surf_z = np.mean(substr_top_layer.positions[:, 2])
 
     mol_atoms = non_s_atoms[non_s_atoms.positions[:, 2] > surf_z]
 
     return mol_atoms, surf_z
 
 
-@calcfunction
+@engine.calcfunction
 def analyze_structure(structure, substrate, mag_per_site, ads_h=None):
-
     ase_geo = structure.get_ase()
     substr_elem = substrate.value.split("(")[0]
 
     mol_atoms, surf_z = geometrical_analysis(ase_geo, substr_elem)
 
     if surf_z is None:
         if ads_h is None:
-            return ExitCode(300, "Ads. height not specified for isolated molecule.")
+            return engine.ExitCode(
+                300, "Ads. height not specified for isolated molecule."
+            )
         # Adsorption height is defined from the geometrical center of the molecule
         surf_z = np.mean(mol_atoms.positions[:, 2]) - ads_h.value
 
     else:
         # If you manually specify adsorption height, it will override the
         # height extracted from the geometry
         if ads_h is not None:
@@ -62,23 +62,22 @@
         mps = [
             m
             for at, m in zip(ase_geo, list(mag_per_site))
             if (at.symbol, *np.round(at.position, 2)) in mol_at_tuples
         ]
 
     return {
-        "mol_struct": StructureData(ase=mol_atoms),
-        "image_plane_z": Float(imag_plane_z),
-        "mol_mag_per_site": List(mps),
+        "mol_struct": orm.StructureData(ase=mol_atoms),
+        "image_plane_z": orm.Float(imag_plane_z),
+        "mol_mag_per_site": orm.List(mps),
     }
 
 
-@calcfunction
+@engine.calcfunction
 def calc_gw_ic_parameters(gw_params, ic_params):
-
     gw_evals = gw_params["gw_eval"]
     ic_deltas = ic_params["ic_delta"]
     homo_inds = gw_params["homo"]
 
     homo_ens = []
     lumo_ens = []
     gw_ic_levels = []
@@ -104,65 +103,68 @@
         "homo": gw_params["homo"],
         "mo": gw_params["mo"],
         "gw_levels": gw_params["gw_eval"],
         "ic_deltas": ic_params["ic_delta"],
         "scf_levels": gw_params["g0w0_e_scf"],
     }
 
-    return Dict(gw_ic_params)
+    return orm.Dict(gw_ic_params)
 
 
-class Cp2kAdsorbedGwIcWorkChain(WorkChain):
+class Cp2kAdsorbedGwIcWorkChain(engine.WorkChain):
     """
     WorkChain to run GW and IC for an adsorbed system
 
     Two different ways to run:
     1) geometry of a molecule adsorbed on a substrate
     2) isolated molecule & adsorption height
     """
 
     @classmethod
     def define(cls, spec):
         super().define(spec)
-        spec.input("code", valid_type=Code)
+        spec.input("code", valid_type=orm.Code)
 
         spec.input(
             "structure",
-            valid_type=StructureData,
+            valid_type=orm.StructureData,
             help="A molecule on a substrate or an isolated molecule.",
         )
         spec.input(
             "ads_height",
-            valid_type=Float,
+            valid_type=orm.Float,
             required=False,
             help=(
-                "Ads. height from the molecular geometrical center."
+                "Adsoprtion height from the molecular geometrical center."
                 "Required if an isolated molecule is specified."
             ),
         )
         spec.input(
             "substrate",
-            valid_type=Str,
-            default=lambda: Str("Au(111)"),
+            valid_type=orm.Str,
+            default=lambda: orm.Str("Au(111)"),
             help="Substrate type, determines the image charge plane.",
         )
         spec.input(
             "protocol",
-            valid_type=Str,
-            default=lambda: Str("gpw_std"),
+            valid_type=orm.Str,
+            default=lambda: orm.Str("gpw_std"),
             required=False,
             help="Protocol supported by the GW workchain.",
         )
         spec.input(
-            "multiplicity", valid_type=Int, default=lambda: Int(0), required=False
+            "multiplicity",
+            valid_type=orm.Int,
+            default=lambda: orm.Int(0),
+            required=False,
         )
         spec.input(
             "magnetization_per_site",
-            valid_type=List,
-            default=lambda: List(list=[]),
+            valid_type=orm.List,
+            default=lambda: orm.List(list=[]),
             required=False,
         )
         spec.input_namespace(
             "options",
             valid_type=dict,
             non_db=True,
             required=False,
@@ -187,31 +189,31 @@
             valid_type=dict,
             non_db=True,
             required=False,
             help="Define options for the GW cacluation: walltime, memory, CPUs, etc.",
         )
         spec.input(
             "debug",
-            valid_type=Bool,
-            default=lambda: Bool(False),
+            valid_type=orm.Bool,
+            default=lambda: orm.Bool(False),
             required=False,
             help="Run with fast parameters for debugging.",
         )
 
         spec.input(
             "geometry_mode",
-            valid_type=Str,
-            default=lambda: Str("ads_geo"),
+            valid_type=orm.Str,
+            default=lambda: orm.Str("ads_geo"),
             required=False,
             help="Possibilities: ads_geo, gas_opt",
         )
 
         spec.outline(
             cls.setup,
-            if_(cls.gas_opt_selected)(cls.gas_opt, cls.check_gas_opt),
+            engine.if_(cls.gas_opt_selected)(cls.gas_opt, cls.check_gas_opt),
             cls.ic,
             cls.gw,
             cls.finalize,
         )
         spec.outputs.dynamic = True
 
         spec.exit_code(
@@ -253,68 +255,67 @@
             self.report("Structure analyis failed.")
             return self.exit_codes.ERROR_STRUCTURE_ANALYSIS
 
         self.ctx.mol_struct = an_out["mol_struct"]
         self.ctx.image_plane_z = an_out["image_plane_z"]
         self.ctx.mol_mag_per_site = an_out["mol_mag_per_site"]
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
 
     def gas_opt_selected(self):
         return self.inputs.geometry_mode.value == "gas_opt"
 
     def gas_opt(self):
-        builder = Cp2kMoleculeOptWorkChain.get_builder()
+        builder = Cp2kGeoOptWorkChain.get_builder()
         builder.code = self.inputs.code
         builder.structure = self.ctx.mol_struct
         builder.multiplicity = self.inputs.multiplicity
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
-        builder.vdw = Bool(True)
-        builder.protocol = Str("standard")
+        builder.vdw = orm.Bool(True)
+        builder.protocol = orm.Str("standard")
         if self.inputs.debug.value:
-            builder.protocol = Str("debug")
+            builder.protocol = orm.Str("debug")
         builder.options = self.inputs.options.scf
         builder.metadata.description = "gas_opt"
         submitted_node = self.submit(builder)
-        return ToContext(gas_opt=submitted_node)
+        return engine.ToContext(gas_opt=submitted_node)
 
     def check_gas_opt(self):
         if not self.ctx.gas_opt.is_finished_ok:
             return self.exit_codes.ERROR_TERMINATION
         # set the optimized geometrical center to the adsorbed conf geometrical center
         ads_mol_ase = self.ctx.mol_struct.get_ase()
         ads_mol_geo_center = np.mean(ads_mol_ase.positions, axis=0)
         gas_opt_ase = self.ctx.gas_opt.outputs.output_structure.get_ase()
         gas_opt_geo_center = np.mean(gas_opt_ase.positions, axis=0)
         gas_opt_ase.positions += ads_mol_geo_center - gas_opt_geo_center
-        self.ctx.mol_struct = StructureData(ase=gas_opt_ase)
-        return ExitCode(0)
+        self.ctx.mol_struct = orm.StructureData(ase=gas_opt_ase)
+        return engine.ExitCode(0)
 
     def ic(self):
         self.report("Submitting IC.")
 
         # Run IC first, because it has a higher chance of failure
 
         builder = Cp2kMoleculeGwWorkChain.get_builder()
         builder.code = self.inputs.code
         builder.protocol = self.inputs.protocol
         builder.structure = self.ctx.mol_struct
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
         builder.multiplicity = self.inputs.multiplicity
         builder.debug = self.inputs.debug
-        builder.run_image_charge = Bool(True)
+        builder.run_image_charge = orm.Bool(True)
         builder.z_ic_plane = self.ctx.image_plane_z
         builder.options.scf = self.inputs.options.scf
         builder.options.gw = self.inputs.options.ic
         builder.metadata.description = "ic"
         submitted_node = self.submit(builder)
-        return ToContext(ic=submitted_node)
+        return engine.ToContext(ic=submitted_node)
 
     def gw(self):
-
         if not self.ctx.ic.is_finished_ok:
             return self.exit_codes.ERROR_TERMINATION
 
         self.report("Submitting GW.")
 
         builder = Cp2kMoleculeGwWorkChain.get_builder()
         builder.code = self.inputs.code
@@ -323,15 +324,15 @@
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
         builder.multiplicity = self.inputs.multiplicity
         builder.debug = self.inputs.debug
         builder.options.scf = self.inputs.options.scf
         builder.options.gw = self.inputs.options.gw
         builder.metadata.description = "gw"
         submitted_node = self.submit(builder)
-        return ToContext(gw=submitted_node)
+        return engine.ToContext(gw=submitted_node)
 
     def finalize(self):
         self.report("Finalizing...")
         if not self.ctx.gw.is_finished_ok:
             return self.exit_codes.ERROR_TERMINATION
 
         gw_out_params = self.ctx.gw.outputs.gw_output_parameters
@@ -350,8 +351,8 @@
         if extras_label not in self.inputs.structure.base.extras.all:
             extras_list = []
         else:
             extras_list = self.inputs.structure.base.extras.all[extras_label]
         extras_list.append(self.node.pk)
         self.inputs.structure.base.extras.set(extras_label, extras_list)
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/bulk_opt_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,220 +1,198 @@
-import copy
-import os
-import pathlib
-
-import yaml
-from aiida.engine import ExitCode, ToContext, WorkChain
-from aiida.orm import Bool, Code, Dict, Int, List, SinglefileData, Str, StructureData
-from aiida.plugins import WorkflowFactory
-
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.cp2k.cp2k_utils import (
-    determine_kinds,
-    dict_merge,
-    get_cutoff,
-    get_kinds_section,
-)
+import numpy as np
+from aiida import engine, orm
 
-Cp2kBaseWorkChain = WorkflowFactory("cp2k.base")
+from .geo_opt_workchain import Cp2kGeoOptWorkChain
+from .molecule_gw_workchain import Cp2kMoleculeGwWorkChain
 
 
-class Cp2kBulkOptWorkChain(WorkChain):
+@engine.calcfunction
+def analyze_structure(structure, mag_per_site):
+    mol_atoms = structure.get_ase()
+
+    mps = []
+    if list(mag_per_site):
+        mol_at_tuples = [
+            (e, *np.round(p, 2))
+            for e, p in zip(mol_atoms.get_chemical_symbols(), mol_atoms.positions)
+        ]
+        mps = [
+            m
+            for at, m in zip(mol_atoms, list(mag_per_site))
+            if (at.symbol, *np.round(at.position, 2)) in mol_at_tuples
+        ]
+
+    return {
+        "mol_struct": orm.StructureData(ase=mol_atoms),
+        "mol_mag_per_site": orm.List(mps),
+    }
+
+
+class Cp2kMoleculeOptGwWorkChain(engine.WorkChain):
+    """WorkChain to  optimize molecule and run GW:
+
+    Two different ways to run:
+    1) optimize geo and run gw
+    2) run gw
+    """
+
     @classmethod
     def define(cls, spec):
         super().define(spec)
-        spec.input("code", valid_type=Code)
-        spec.input("structure", valid_type=StructureData)
+        spec.input("code", valid_type=orm.Code)
 
         spec.input(
-            "charge",  # +1 means one electron removed
-            valid_type=Int,
-            default=lambda: Int(0),
-            required=False,
+            "structure", valid_type=orm.StructureData, help="An isolated molecule."
         )
         spec.input(
-            "fixed_atoms", valid_type=Str, default=lambda: Str(""), required=False
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("gpw_std"),
+            required=False,
+            help="Protocol supported by the GW workchain.",
         )
         spec.input(
-            "cell_opt", valid_type=Bool, default=lambda: Bool(False), required=False
+            "multiplicity",
+            valid_type=orm.Int,
+            default=lambda: orm.Int(0),
+            required=False,
         )
         spec.input(
-            "symmetry",
-            valid_type=Str,
-            default=lambda: Str("ORTHORHOMBIC"),
+            "magnetization_per_site",
+            valid_type=orm.List,
+            default=lambda: orm.List(list=[]),
             required=False,
         )
-        spec.input(
-            "cell_freedom",
-            valid_type=Str,
-            default=lambda: Str("KEEP_SYMMETRY"),
+        spec.input_namespace(
+            "options",
+            valid_type=dict,
+            non_db=True,
             required=False,
+            help="Define options for the cacluations: walltime, memory, CPUs, etc.",
         )
+
         spec.input(
-            "multiplicity", valid_type=Int, default=lambda: Int(0), required=False
+            "options.geo_opt",
+            valid_type=dict,
+            non_db=True,
+            required=False,
+            help="Define options for the GEO_OPT cacluation: walltime, memory, CPUs, etc.",
         )
+
         spec.input(
-            "magnetization_per_site",
-            valid_type=List,
-            default=lambda: List(list=[]),
+            "options.gw",
+            valid_type=dict,
+            non_db=True,
             required=False,
+            help="Define options for the GW cacluation: walltime, memory, CPUs, etc.",
         )
-        spec.input("vdw", valid_type=Bool, default=lambda: Bool(False), required=False)
         spec.input(
-            "protocol",
-            valid_type=Str,
-            default=lambda: Str("standard"),
+            "debug",
+            valid_type=orm.Bool,
+            default=lambda: orm.Bool(False),
             required=False,
-            help="Settings to run simulations with.",
+            help="Run with fast parameters for debugging.",
         )
         spec.input(
-            "options",
-            valid_type=dict,
-            non_db=True,
+            "geo_opt",
+            valid_type=orm.Bool,
+            default=lambda: orm.Bool(True),
             required=False,
-            help="Define options for the cacluations: walltime, memory, CPUs, etc.",
+            help="Perform geo opt step.",
         )
 
-        # workchain outline
-        spec.outline(cls.setup, cls.submit_calc, cls.finalize)
+        spec.outline(
+            cls.setup,
+            engine.if_(cls.gas_opt_selected)(cls.gas_opt, cls.check_gas_opt),
+            cls.gw,
+            cls.finalize,
+        )
         spec.outputs.dynamic = True
 
         spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
     def setup(self):
-        self.report("Inspecting input and setting up things")
-
-        # --------------------------------------------------
-
-    def submit_calc(self):
-
-        # load input template
-        the_protocol = "./protocols/bulk_opt_protocol.yml"
-        if self.inputs.cell_opt.value:
-            the_protocol = "./protocols/cell_opt_protocol.yml"
-        with open(
-            pathlib.Path(__file__).parent / the_protocol, encoding="utf-8"
-        ) as handle:
-            protocols = yaml.safe_load(handle)
-            input_dict = copy.deepcopy(protocols[self.inputs.protocol.value])
-
-        structure = self.inputs.structure
-        # cutoff
-        self.ctx.cutoff = get_cutoff(structure=structure)
-
-        # get initial magnetization
-        magnetization_per_site = copy.deepcopy(self.inputs.magnetization_per_site)
-        structure_with_tags, kinds_dict = determine_kinds(
-            structure, magnetization_per_site
-        )
-
-        ase_atoms = structure_with_tags.get_ase()
-
-        builder = Cp2kBaseWorkChain.get_builder()
-        builder.cp2k.code = self.inputs.code
-        builder.cp2k.structure = StructureData(ase=ase_atoms)
-        builder.cp2k.file = {
-            "basis": SinglefileData(
-                file=os.path.join(
-                    os.path.dirname(os.path.realpath(__file__)),
-                    ".",
-                    "data",
-                    "BASIS_MOLOPT",
-                )
-            ),
-            "pseudo": SinglefileData(
-                file=os.path.join(
-                    os.path.dirname(os.path.realpath(__file__)),
-                    ".",
-                    "data",
-                    "POTENTIAL",
-                )
-            ),
-        }
-
-        # charge
-        input_dict["FORCE_EVAL"]["DFT"]["CHARGE"] = self.inputs.charge.value
-        # vdw
-        if not self.inputs.vdw.value:
-            input_dict["FORCE_EVAL"]["DFT"]["XC"].pop("VDW_POTENTIAL")
-
-        # UKS
-        if self.inputs.multiplicity.value > 0:
-            input_dict["FORCE_EVAL"]["DFT"]["UKS"] = ".TRUE."
-            input_dict["FORCE_EVAL"]["DFT"][
-                "MULTIPLICITY"
-            ] = self.inputs.multiplicity.value
-
-        # only bulk opt
-        if not self.inputs.cell_opt.value:
-            # fixed atoms
-            input_dict["MOTION"]["CONSTRAINT"]["FIXED_ATOMS"][
-                "LIST"
-            ] = self.inputs.fixed_atoms.value
-
-        # cell opt
-        else:
-            # cell symmetry
-            input_dict["FORCE_EVAL"]["SUBSYS"]["CELL"][
-                "SYMMETRY"
-            ] = self.inputs.symmetry.value
+        self.report("Inspecting input and setting up things.")
 
-            # cell do free
-            if self.inputs.cell_freedom.value == "KEEP_SYMMETRY":
-                input_dict["MOTION"]["CELL_OPT"]["KEEP_SYMMETRY"] = ""
-            elif self.inputs.cell_freedom.value == "KEEP_ANGLES":
-                input_dict["MOTION"]["CELL_OPT"]["KEEP_ANGLES"] = ""
-
-        # cutoff
-        input_dict["FORCE_EVAL"]["DFT"]["MGRID"]["CUTOFF"] = self.ctx.cutoff
-
-        # KINDS section
-        self.ctx.kinds_section = get_kinds_section(kinds_dict, protocol="gpw")
-        dict_merge(input_dict, self.ctx.kinds_section)
-
-        # Setup options.
-        if "options" in self.inputs:
-            builder.cp2k.metadata.options = self.inputs.options
+        n_atoms = len(self.inputs.structure.get_ase())
+        n_mags = len(list(self.inputs.magnetization_per_site))
+        if n_mags not in (0, n_atoms):
+            self.report("If set, magnetization_per_site needs a value for every atom.")
+            return self.exit_codes.ERROR_TERMINATION
 
-        # Setup walltime.
-        if "max_wallclock_seconds" in self.inputs.options:
-            input_dict["GLOBAL"]["WALLTIME"] = max(
-                self.inputs.options["max_wallclock_seconds"] - 600, 600
-            )
+        an_out = analyze_structure(
+            self.inputs.structure, self.inputs.magnetization_per_site
+        )
 
-        # parser
-        builder.cp2k.metadata.options.parser_name = "cp2k_advanced_parser"
+        self.ctx.mol_struct = an_out["mol_struct"]
+        self.ctx.mol_mag_per_site = an_out["mol_mag_per_site"]
 
-        # handlers
+        return engine.ExitCode(0)
 
-        builder.handler_overrides = Dict(
-            {"restart_incomplete_calculation": {"enabled": True}}
-        )
+    def gas_opt_selected(self):
+        return self.inputs.geo_opt.value
+
+    def gas_opt(self):
+        builder = Cp2kGeoOptWorkChain.get_builder()
+        builder.code = self.inputs.code
+        builder.structure = self.ctx.mol_struct
+        builder.multiplicity = self.inputs.multiplicity
+        builder.magnetization_per_site = self.ctx.mol_mag_per_site
+        builder.vdw = orm.Bool(True)
+        builder.protocol = orm.Str("standard")
+        if self.inputs.debug.value:
+            builder.protocol = orm.Str("debug")
+        builder.options = self.inputs.options.geo_opt
+        builder.metadata.description = "Submitted by Cp2kMoleculeOptGwWorkChain."
+        builder.metadata.label = "Cp2kGeoOptWorkChain"
+        return engine.ToContext(gas_opt=self.submit(builder))
 
-        # cp2k input dictionary
-        builder.cp2k.parameters = Dict(input_dict)
+    def check_gas_opt(self):
+        if not self.ctx.gas_opt.is_finished_ok:
+            return self.exit_codes.ERROR_TERMINATION
 
+        # Set the optimized geometry as ctx geometry.
+        self.ctx.mol_struct = self.ctx.gas_opt.outputs.output_structure
+        return engine.ExitCode(0)
+
+    def gw(self):
+        self.report("Submitting GW.")
+
+        builder = Cp2kMoleculeGwWorkChain.get_builder()
+        builder.code = self.inputs.code
+        builder.protocol = self.inputs.protocol
+        builder.structure = self.ctx.mol_struct
+        builder.magnetization_per_site = self.ctx.mol_mag_per_site
+        builder.multiplicity = self.inputs.multiplicity
+        builder.debug = self.inputs.debug
+        builder.options.scf = self.inputs.options.geo_opt
+        builder.options.gw = self.inputs.options.gw
+        builder.metadata.description = "gw"
         submitted_node = self.submit(builder)
-        return ToContext(opt=submitted_node)
+        return engine.ToContext(gw=submitted_node)
 
     def finalize(self):
         self.report("Finalizing...")
 
-        if not self.ctx.opt.is_finished_ok:
+        if not self.ctx.gw.is_finished_ok:
             return self.exit_codes.ERROR_TERMINATION
 
-        for out in self.ctx.opt.outputs:
-            self.out(out, self.ctx.opt.outputs[out])
+        gw_out_params = self.ctx.gw.outputs.gw_output_parameters
+        self.out("gw_output_parameters", gw_out_params)
 
-        # Add extras
-        struc = self.ctx.opt.outputs.output_structure
-        ase_geom = struc.get_ase()
-        self.node.base.extras.set(
-            "thumbnail", common_utils.thumbnail(ase_struc=ase_geom)
-        )
-        self.node.base.extras.set("formula", struc.get_formula())
+        self.out("output_structure", self.ctx.mol_struct)
+
+        # Add the workchain pk to the input/geo_opt structure extras.
+        struc_to_label = self.ctx.mol_struct
+        extras_label = "Cp2kMoleculeOptGwWorkChain_pks"
+        if extras_label not in struc_to_label.base.extras.all:
+            extras_list = []
+        else:
+            extras_list = struc_to_label.base.extras.all[extras_label]
+        extras_list.append(self.node.pk)
+        struc_to_label.base.extras.set(extras_label, extras_list)
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 import numpy as np
 import yaml
 from aiida import engine, orm, plugins
 
-from aiida_nanotech_empa.utils import analyze_structure
-from aiida_nanotech_empa.workflows.cp2k import cp2k_utils
+from ...utils import analyze_structure, common_utils
+from . import cp2k_utils
 
 StructureData = plugins.DataFactory("core.structure")
 Cp2kBaseWorkChain = plugins.WorkflowFactory("cp2k.base")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute() / "data"
 
 
@@ -83,64 +83,43 @@
         spec.input("code", valid_type=orm.Code)
 
         # Specify the input structure and its fragments.
         spec.input(
             "structure", valid_type=StructureData, help="A molecule on a substrate."
         )
 
-        spec.input(
-            "uks", valid_type=orm.Bool, required=False, default=lambda: orm.Bool(False)
-        )
-
         spec.input_namespace(
             "fragments",
             valid_type=orm.List,
             help="List of indices of atoms defining individual fragments.",
         )
 
-        # Charges of each fragment.
-        spec.input_namespace(
-            "charges",  # +1 means one electron removed
-            valid_type=orm.Int,
-            required=False,
-            help="Charges of each fragment. No need to specify the charge of the full system as it would be computed automatically.",
-        )
-
-        # Multiplicity of each fragment.
-        spec.input_namespace(
-            "multiplicities",
-            valid_type=orm.Int,
-            required=False,
-            help="Multiplicity of each fragment. Use 'all' to specify the multiplicity of the whole system.",
+        # dft parameters
+        spec.input(
+            "dft_params",
+            valid_type=orm.Dict,
+            help="""
+        multiplicities, dictionary: multiplicity of each fragment. Use 'all' to specify the multiplicity of the whole system.
+        magnetization_per_site: Magnetization per site of the whole system.
+            Magnetization per site of the fragments will be extracted automatically.
+        charges, dictionary: Charges of each fragment. No need to specify the charge of the full system
+            as it would be computed automatically.
+        protocol: Protocol to use for the calculation.
+        uks: Use unrestricted Kohn-Sham.
+        """,
         )
 
         # Fixed atoms and magnetization per site defined for the whole system. Information for the fragments will extracted automatically.
         spec.input(
             "fixed_atoms",
             valid_type=orm.List,
             required=False,
             help="Fixed atoms of the whole system. Fixed atoms of the fragments will be extracted automatically.",
         )
 
-        spec.input(
-            "magnetization_per_site",
-            valid_type=orm.List,
-            required=False,
-            help="Magnetization per site of the whole system. Magnetization per site of the fragments will be extracted automatically.",
-        )
-
-        # Protocol that defines the simulation settings.
-        spec.input(
-            "protocol",
-            valid_type=orm.Str,
-            default=lambda: orm.Str("standard"),
-            required=False,
-            help="Settings to run simulations with.",
-        )
-
         spec.input_namespace(
             "auxilary_dictionaries",
             valid_type=orm.Dict,
             help="Dictionaries to append to the CP2K input dictionary right before the job submission. "
             "It is useful to add constraints and collective variables to the input.",
         )
 
@@ -148,14 +127,17 @@
             "options",
             valid_type=int,
             non_db=True,
             required=False,
             help="Define options for the cacluations: walltime, memory, CPUs, etc.",
         )
 
+        # in case wfn for the whole system is available and matches uks/rks parameters
+        spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+
         # Outline.
         spec.outline(cls.setup, cls.run_scfs, cls.run_geo_opts, cls.finalize)
 
         # Dynamic outputs.
         spec.outputs.dynamic = True
 
         # Exit code.
@@ -167,16 +149,16 @@
 
     def setup(self):
         """Setup the work chain."""
 
         self.report("Inspecting input and setting things up.")
 
         n_atoms = len(self.inputs.structure.sites)
-        if "magnetization_per_site" in self.inputs:
-            n_mags = len(list(self.inputs.magnetization_per_site))
+        if "magnetization_per_site" in self.inputs.dft_params:
+            n_mags = len(list(self.inputs.dft_params["magnetization_per_site"]))
             if n_mags not in (0, n_atoms):
                 self.report(
                     "If set, magnetization_per_site needs a value for every atom."
                 )
                 return self.exit_codes.ERROR_TERMINATION
 
         self.ctx.cutoff = cp2k_utils.get_cutoff(structure=self.inputs.structure)
@@ -193,23 +175,23 @@
 
     def run_scfs(self):
         """Run SCF calculation for the whole system and for fragments."""
         # Firt run SCF for the whole system and its fragments.
         for inputs in split_structure(
             structure=self.inputs.structure,
             fixed_atoms=self.inputs.fixed_atoms,
-            magnetization_per_site=self.inputs.magnetization_per_site
-            if "magnetization_per_site" in self.inputs
+            magnetization_per_site=self.inputs.dft_params["magnetization_per_site"]
+            if "magnetization_per_site" in self.inputs.dft_params
             else None,
             fragments=self.inputs.fragments,
         ):
-
             # Re-loading the input dictionary for the given protocol.
             input_dict = load_protocol(
-                fname="slab_opt_protocol.yml", protocol=self.inputs.protocol.value
+                fname="geo_opt_protocol.yml",
+                protocol=self.inputs.dft_params["protocol"],
             )
 
             self.report(
                 f"""Running SCF for the fragment '{inputs['label']}' consisting of {len(inputs['structure'].sites)} atoms, """
                 f"""where {analyze_structure.list_to_string_range(inputs['fixed_atoms']) or 'None'} atoms are fixed."""
             )
 
@@ -217,44 +199,52 @@
             fragment = inputs["label"]
 
             # Generic inputs that are always the same.
             builder = Cp2kBaseWorkChain.get_builder()
             builder.cp2k.code = self.inputs.code
             builder.cp2k.metadata.options.parser_name = "cp2k_advanced_parser"
 
+            # restart wfn in case of fragment 'all'
+            if inputs["label"] == "all":
+                if "parent_calc_folder" in self.inputs:
+                    builder.cp2k.parent_calc_folder = self.inputs.parent_calc_folder
+
             # If options are defined for a specific fragment, use them.
             if "options" in self.inputs and fragment in self.inputs.options:
                 builder.cp2k.metadata.options = self.inputs.options[fragment]
 
             builder.cp2k.file = self.ctx.file
             input_dict["GLOBAL"]["RUN_TYPE"] = "ENERGY"
             input_dict["FORCE_EVAL"]["DFT"]["MGRID"]["CUTOFF"] = self.ctx.cutoff
 
             # Always compute charge density with STRIDE 2 2 2 for the SCF part of the work chain.
             input_dict["FORCE_EVAL"]["DFT"]["PRINT"]["E_DENSITY_CUBE"][
                 "STRIDE"
             ] = "2 2 2"
 
             # If charge is set, add it to the corresponding section of the input.
-            if "charges" in self.inputs and fragment in self.inputs.charges:
-                input_dict["FORCE_EVAL"]["DFT"]["CHARGE"] = self.inputs.charges[
-                    fragment
-                ].value
+            if (
+                "charges" in self.inputs.dft_params
+                and fragment in self.inputs.dft_params["charges"]
+            ):
+                input_dict["FORCE_EVAL"]["DFT"]["CHARGE"] = self.inputs.dft_params[
+                    "charges"
+                ][fragment]
 
-            if self.inputs.uks:
+            if "uks" in self.inputs.dft_params and self.inputs.dft_params["uks"]:
                 input_dict["FORCE_EVAL"]["DFT"]["UKS"] = ".TRUE."
 
                 # If the multiplicity is set, add it to the corresponding section of the input.
                 if (
-                    "multiplicities" in self.inputs
-                    and fragment in self.inputs.multiplicities
+                    "multiplicities" in self.inputs.dft_params
+                    and fragment in self.inputs.dft_params["multiplicities"]
                 ):
                     input_dict["FORCE_EVAL"]["DFT"][
                         "MULTIPLICITY"
-                    ] = self.inputs.multiplicities[fragment].value
+                    ] = self.inputs.dft_params["multiplicities"][fragment]
 
                 # Adding magnetisation tags to the structure and to the CP2K input dictionary.
                 structure, kinds_dict = cp2k_utils.determine_kinds(
                     inputs["structure"], inputs["magnetization_per_site"]
                 )
             else:
                 structure, kinds_dict = cp2k_utils.determine_kinds(inputs["structure"])
@@ -282,15 +272,14 @@
 
             builder.cp2k.parameters = orm.Dict(dict=input_dict)
 
             submitted_node = self.submit(builder)
             self.to_context(**{f"scf.{fragment}": submitted_node})
 
     def run_geo_opts(self):
-
         for fragment in self.inputs.fragments.keys():
             # We deliberately do not run optimisation for the full structure.
             if fragment == "all":
                 continue
 
             # Generic inputs that are always the same.
             builder = Cp2kBaseWorkChain.get_builder()
@@ -321,15 +310,14 @@
         self.report("Finalizing...")
         energies["all"] = self.ctx.scf["all"].outputs.output_parameters["energy"]
 
         separation_energy = energies["all"]
         unrelaxed_separation_energy = energies["all"]
 
         for fragment in list(self.inputs.fragments.keys()):
-
             # The geometry optimisation is not run for the full structure.
             if fragment == "all":
                 continue
 
             energies[fragment] = {
                 "unrelaxed": self.ctx.scf[fragment].outputs.output_parameters["energy"],
                 "relaxed": self.ctx.opt[fragment].outputs.output_parameters["energy"],
@@ -340,14 +328,8 @@
         energies["unrelaxed_separation_energy"] = unrelaxed_separation_energy
         energies["separation_energy"] = separation_energy
 
         energies = orm.Dict(dict=energies).store()
         self.out("energies", energies)
 
         # Add the workchain pk to the input structure extras
-        extras_label = "Cp2kAdsorptionEnergyWorkChain_pks"
-        if extras_label not in self.inputs.structure.base.extras.all:
-            extras_list = []
-        else:
-            extras_list = self.inputs.structure.base.extras.all[extras_label]
-        extras_list.append(self.node.pk)
-        self.inputs.structure.base.extras.set(extras_label, extras_list)
+        common_utils.add_extras(self.inputs.structure, "surfaces", self.node.uuid)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 import copy
-import os
 import pathlib
 
 import numpy as np
 import yaml
-from aiida.engine import ExitCode, ToContext, WorkChain, while_
-from aiida.orm import (
-    Bool,
-    Code,
-    Dict,
-    Float,
-    Int,
-    List,
-    SinglefileData,
-    Str,
-    StructureData,
-)
+from aiida import engine, orm
 from aiida_cp2k.calculations import Cp2kCalculation
 
-from aiida_nanotech_empa.workflows.cp2k.cp2k_utils import (
-    determine_kinds,
-    dict_merge,
-    get_cutoff,
-    get_kinds_section,
-)
+from . import cp2k_utils
 
 ALLOWED_PROTOCOLS = ["gapw_std", "gapw_hq", "gpw_std"]
 
 
-class Cp2kMoleculeGwWorkChain(WorkChain):
+class Cp2kMoleculeGwWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
-        spec.input("code", valid_type=Code)
-        spec.input("structure", valid_type=StructureData)
+        spec.input("code", valid_type=orm.Code)
+        spec.input("structure", valid_type=orm.StructureData)
 
         spec.input(
             "protocol",
-            valid_type=Str,
-            default=lambda: Str("gapw_std"),
+            valid_type=orm.Str,
+            default=lambda: orm.Str("gapw_std"),
             required=False,
             help="Either 'gapw_std', 'gapw_hq', 'gpw_std'",
         )
 
         spec.input(
             "run_image_charge",
-            valid_type=Bool,
-            default=lambda: Bool(False),
+            valid_type=orm.Bool,
+            default=lambda: orm.Bool(False),
             required=False,
             help="Run the image charge correction calculation.",
         )
         spec.input(
-            "z_ic_plane", valid_type=Float, default=lambda: Float(8.22), required=False
+            "z_ic_plane",
+            valid_type=orm.Float,
+            default=lambda: orm.Float(8.22),
+            required=False,
         )
 
         spec.input(
-            "multiplicity", valid_type=Int, default=lambda: Int(0), required=False
+            "multiplicity",
+            valid_type=orm.Int,
+            default=lambda: orm.Int(0),
+            required=False,
         )
         spec.input(
             "magnetization_per_site",
-            valid_type=List,
-            default=lambda: List(list=[]),
+            valid_type=orm.List,
+            default=lambda: orm.List(list=[]),
             required=False,
         )
         spec.input_namespace(
             "options",
             valid_type=dict,
             non_db=True,
             required=False,
@@ -85,23 +74,23 @@
             non_db=True,
             required=False,
             help="Define options for the GW cacluation: walltime, memory, CPUs, etc.",
         )
 
         spec.input(
             "debug",
-            valid_type=Bool,
-            default=lambda: Bool(False),
+            valid_type=orm.Bool,
+            default=lambda: orm.Bool(False),
             required=False,
             help="Run with fast parameters for debugging.",
         )
 
         spec.outline(
             cls.setup,
-            while_(cls.scf_is_not_done)(cls.submit_scf, cls.check_scf),
+            engine.while_(cls.scf_is_not_done)(cls.submit_scf, cls.check_scf),
             cls.submit_gw,
             cls.finalize,
         )
         spec.outputs.dynamic = True
 
         spec.exit_code(
             381,
@@ -121,92 +110,86 @@
         spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
     def setup(self):
-
         self.report("Inspecting input and setting up things")
 
         if self.inputs.protocol not in ALLOWED_PROTOCOLS:
             self.report("Error: protocol not supported.")
             return self.exit_codes.ERROR_TERMINATION
 
-        # Load protocol templates
+        # Load protocol templates.
         with open(
             pathlib.Path(__file__).parent.joinpath("./protocols/gw_protocols.yml"),
             encoding="utf-8",
         ) as handle:
             self.ctx.protocols = yaml.safe_load(handle)
 
         structure = self.inputs.structure
-        self.ctx.cutoff = get_cutoff(structure=structure)
+        self.ctx.cutoff = cp2k_utils.get_cutoff(structure=structure)
         magnetization_per_site = copy.deepcopy(self.inputs.magnetization_per_site)
         ghost_per_site = None
 
-        # Add ghost atoms in case of gw-ic
+        # Add ghost atoms in case of gw-ic.
         if self.inputs.run_image_charge:
             atoms = self.inputs.structure.get_ase()
             image = atoms.copy()
             image.positions[:, 2] = (
                 2 * self.inputs.z_ic_plane.value - atoms.positions[:, 2]
             )
             ghost_per_site = [0 for a in atoms] + [1 for a in image]
             if magnetization_per_site:
                 magnetization_per_site += [0 for i in range(len(image))]
-            structure = StructureData(ase=atoms + image)
+            structure = orm.StructureData(ase=atoms + image)
 
-        structure_with_tags, kinds_dict = determine_kinds(
+        structure_with_tags, kinds_dict = cp2k_utils.determine_kinds(
             structure, magnetization_per_site, ghost_per_site
         )
 
-        # KINDS section
-        self.ctx.kinds_section = get_kinds_section(
+        # KINDS section.
+        self.ctx.kinds_section = cp2k_utils.get_kinds_section(
             kinds_dict, protocol=self.inputs.protocol
         )
 
-        # make sure cell is big enough for MT poisson solver
+        # Make sure cell is big enough for MT poisson solver.
         if self.inputs.debug:
             extra_cell = 5.0
         else:
             extra_cell = 15.0
         atoms = structure_with_tags.get_ase()
         atoms.cell = 2 * (np.ptp(atoms.positions, axis=0)) + extra_cell
         atoms.center()
-        self.ctx.structure = StructureData(ase=atoms)
+        self.ctx.structure = orm.StructureData(ase=atoms)
 
         # Determine which basis and pseudo files to include
         if self.inputs.protocol in ["gapw_std", "gapw_hq"]:
             basis = "GW_BASIS_SET"
             potential = "ALL_POTENTIALS"
         elif self.inputs.protocol == "gpw_std":
             basis = "K_GW_BASIS"
             potential = "POTENTIAL"
 
         self.ctx.files = {
-            "basis": SinglefileData(
-                file=os.path.join(
-                    os.path.dirname(os.path.realpath(__file__)), ".", "data", basis
-                )
+            "basis": orm.SinglefileData(
+                file=pathlib.Path(__file__).parent / "data" / basis,
             ),
-            "pseudo": SinglefileData(
-                file=os.path.join(
-                    os.path.dirname(os.path.realpath(__file__)), ".", "data", potential
-                )
+            "pseudo": orm.SinglefileData(
+                file=pathlib.Path(__file__).parent / "data" / potential,
             ),
         }
 
         self.ctx.current_scf_protocol = None
         self.ctx.scf_restart_from_last = False
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
 
     def scf_is_not_done(self):
-
         if hasattr(self.ctx, "scf"):
             scf_out_params = self.ctx.scf.outputs.output_parameters
 
             scf_converged = scf_out_params["motion_step_info"]["scf_converged"][-1]
 
             if not scf_converged:
                 self.report("SCF did not converge, try the next protocol.")
@@ -219,37 +202,38 @@
                     scf_out_params["bandgap_spin2_au"],
                 )
                 >= 0.0
             )
 
             if not gap_positive:
                 self.report("Gap is negative, try the next protocol.")
-                # If the SCF converged but the gap was negative,
-                # restart in the next step
+                # If the SCF converged but the gap was negative, restart in the next step
                 self.ctx.scf_restart_from_last = True
                 return True
 
-            self.report("SCF finished well, continue to GW!")
+            self.report("SCF finished well, continue to GW.")
             return False
 
         return True
 
     def _check_and_set_uks(self, input_dict):
         if self.inputs.multiplicity.value > 0:
             input_dict["FORCE_EVAL"]["DFT"]["UKS"] = ".TRUE."
             input_dict["FORCE_EVAL"]["DFT"][
                 "MULTIPLICITY"
             ] = self.inputs.multiplicity.value
 
     def _set_debug(self, input_dict):
         input_dict["FORCE_EVAL"]["DFT"]["PRINT"]["MO_CUBES"]["STRIDE"] = "6 6 6"
         input_dict["FORCE_EVAL"]["DFT"]["PRINT"]["E_DENSITY_CUBE"]["STRIDE"] = "6 6 6"
+        input_dict["FORCE_EVAL"]["DFT"]["SCF"]["EPS_SCF"] = 0.2
+        input_dict["FORCE_EVAL"]["DFT"]["SCF"]["EPS_EIGVAL"] = 0.2
+        input_dict["FORCE_EVAL"]["DFT"]["SCF"]["OUTER_SCF"]["EPS_SCF"] = 0.2
 
     def submit_scf(self):
-
         # Try the next SCF section:
         if self.ctx.current_scf_protocol is None:
             # First try
             self.ctx.current_scf_protocol = "scf_ot_cg"
         elif self.ctx.current_scf_protocol == "scf_ot_cg":
             # Second try
             self.ctx.current_scf_protocol = "scf_ot_diis"
@@ -258,24 +242,24 @@
             self.ctx.current_scf_protocol = "scf_diag_smearing"
         else:
             # Failure
             return self.exit_codes.ERROR_CONVERGENCE1
 
         self.report(f"Submitting SCF (protocol {self.ctx.current_scf_protocol})")
 
-        # Build the input dictionary
+        # Build the input dictionary.
         step_protocol = self.inputs.protocol.value + "_scf_step"
         input_dict = copy.deepcopy(self.ctx.protocols[step_protocol])
 
         scf_section = copy.deepcopy(self.ctx.protocols[self.ctx.current_scf_protocol])
         input_dict["FORCE_EVAL"]["DFT"]["SCF"] = scf_section
 
         self._check_and_set_uks(input_dict)
 
-        dict_merge(input_dict, self.ctx.kinds_section)
+        cp2k_utils.dict_merge(input_dict, self.ctx.kinds_section)
 
         input_dict["FORCE_EVAL"]["DFT"]["MGRID"]["CUTOFF"] = self.ctx.cutoff
 
         if self.inputs.debug:
             self._set_debug(input_dict)
 
         # Prepare the builder.
@@ -294,46 +278,43 @@
         builder.metadata.options = self.inputs.options.scf
         if "max_wallclock_seconds" in self.inputs.options:
             input_dict["GLOBAL"]["WALLTIME"] = max(
                 self.inputs.options["max_wallclock_seconds"] - 600, 600
             )
         builder.metadata.options["parser_name"] = "cp2k_advanced_parser"
 
-        builder.parameters = Dict(input_dict)
+        builder.parameters = orm.Dict(input_dict)
 
-        submitted_node = self.submit(builder)
-        return ToContext(scf=submitted_node)
+        return engine.ToContext(scf=self.submit(builder))
 
     def check_scf(self):
         return (
-            ExitCode(0)
+            engine.ExitCode(0)
             if self.ctx.scf.is_finished_ok
             else self.exit_codes.ERROR_TERMINATION
         )
 
     def submit_gw(self):
-
         self.report("Submitting GW.")
 
-        # -------------------------------------------------------
         # Build the input dictionary
 
         if self.inputs.run_image_charge:
             step_protocol = self.inputs.protocol.value + "_ic_step"
         else:
             step_protocol = self.inputs.protocol.value + "_gw_step"
 
         input_dict = copy.deepcopy(self.ctx.protocols[step_protocol])
 
         scf_section = copy.deepcopy(self.ctx.protocols[self.ctx.current_scf_protocol])
         input_dict["FORCE_EVAL"]["DFT"]["SCF"] = scf_section
 
         self._check_and_set_uks(input_dict)
 
-        dict_merge(input_dict, self.ctx.kinds_section)
+        cp2k_utils.dict_merge(input_dict, self.ctx.kinds_section)
 
         input_dict["FORCE_EVAL"]["DFT"]["MGRID"]["CUTOFF"] = self.ctx.cutoff
 
         if self.inputs.debug:
             self._set_debug(input_dict)
 
         # Prepare the builder.
@@ -350,18 +331,17 @@
         if "max_wallclock_seconds" in self.inputs.options:
             input_dict["GLOBAL"]["WALLTIME"] = max(
                 self.inputs.options["max_wallclock_seconds"] - 600, 600
             )
 
         builder.metadata.options["parser_name"] = "nanotech_empa.cp2k_gw_parser"
 
-        builder.parameters = Dict(input_dict)
+        builder.parameters = orm.Dict(input_dict)
 
-        submitted_node = self.submit(builder)
-        return ToContext(second_step=submitted_node)
+        return engine.ToContext(second_step=self.submit(builder))
 
     def finalize(self):
         self.report("Finalizing...")
 
         if not self.ctx.second_step.is_finished_ok:
             return self.exit_codes.ERROR_TERMINATION
         if not self.ctx.second_step.outputs.std_output_parameters["motion_step_info"][
@@ -373,8 +353,8 @@
         self.out(
             "std_output_parameters", self.ctx.second_step.outputs.std_output_parameters
         )
         self.out(
             "gw_output_parameters", self.ctx.second_step.outputs.gw_output_parameters
         )
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,198 +1,176 @@
+import copy
+
 import numpy as np
-from aiida.engine import ExitCode, ToContext, WorkChain, calcfunction, if_
-from aiida.orm import Bool, Code, Int, List, Str, StructureData
+from aiida import engine, orm, plugins
 
-from .molecule_gw_workchain import Cp2kMoleculeGwWorkChain
-from .molecule_opt_workchain import Cp2kMoleculeOptWorkChain
+from ...utils import common_utils
+from . import cp2k_utils
 
+Cp2kDiagWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.diag")
+OverlapCalculation = plugins.CalculationFactory("nanotech_empa.overlap")
 
-@calcfunction
-def analyze_structure(structure, mag_per_site):
-
-    mol_atoms = structure.get_ase()
-
-    mps = []
-    if list(mag_per_site):
-        mol_at_tuples = [
-            (e, *np.round(p, 2))
-            for e, p in zip(mol_atoms.get_chemical_symbols(), mol_atoms.positions)
-        ]
-        mps = [
-            m
-            for at, m in zip(mol_atoms, list(mag_per_site))
-            if (at.symbol, *np.round(at.position, 2)) in mol_at_tuples
-        ]
-
-    return {
-        "mol_struct": StructureData(ase=mol_atoms),
-        "mol_mag_per_site": List(mps),
-    }
-
-
-class Cp2kMoleculeOptGwWorkChain(WorkChain):
-    """
-    WorkChain to  optimize molecule and run GW
-
-    Two different ways to run:
-    1) optimize geo and run gw
-    2) run gw
-    """
 
+class Cp2kPdosWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
-        spec.input("code", valid_type=Code)
 
-        spec.input("structure", valid_type=StructureData, help="An isolated molecule.")
-        spec.input(
-            "protocol",
-            valid_type=Str,
-            default=lambda: Str("gpw_std"),
-            required=False,
-            help="Protocol supported by the GW workchain.",
-        )
-        spec.input(
-            "multiplicity", valid_type=Int, default=lambda: Int(0), required=False
-        )
-        spec.input(
-            "magnetization_per_site",
-            valid_type=List,
-            default=lambda: List(list=[]),
-            required=False,
-        )
+        spec.input("cp2k_code", valid_type=orm.Code)
+        spec.input("slabsys_structure", valid_type=orm.StructureData)
+        spec.input("mol_structure", valid_type=orm.StructureData)
+        spec.input("pdos_lists", valid_type=orm.List)
+        spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input("dft_params", valid_type=orm.Dict)
+        spec.input("overlap_code", valid_type=orm.Code)
+        spec.input("overlap_params", valid_type=orm.Dict)
         spec.input_namespace(
             "options",
-            valid_type=dict,
+            valid_type=int,
             non_db=True,
-            required=False,
             help="Define options for the cacluations: walltime, memory, CPUs, etc.",
         )
 
-        spec.input(
-            "options.geo_opt",
-            valid_type=dict,
-            non_db=True,
-            required=False,
-            help="Define options for the GEO_OPT cacluation: walltime, memory, CPUs, etc.",
-        )
-
-        spec.input(
-            "options.gw",
-            valid_type=dict,
-            non_db=True,
-            required=False,
-            help="Define options for the GW cacluation: walltime, memory, CPUs, etc.",
-        )
-        spec.input(
-            "debug",
-            valid_type=Bool,
-            default=lambda: Bool(False),
-            required=False,
-            help="Run with fast parameters for debugging.",
-        )
-        spec.input(
-            "geo_opt",
-            valid_type=Bool,
-            default=lambda: Bool(True),
-            required=False,
-            help="Perform geo opt step.",
-        )
-
         spec.outline(
             cls.setup,
-            if_(cls.gas_opt_selected)(cls.gas_opt, cls.check_gas_opt),
-            cls.gw,
+            cls.run_diags,
+            cls.run_overlap,
             cls.finalize,
         )
+
         spec.outputs.dynamic = True
 
         spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
     def setup(self):
-        self.report("Inspecting input and setting up things.")
-
-        n_atoms = len(self.inputs.structure.get_ase())
-        n_mags = len(list(self.inputs.magnetization_per_site))
-        if n_mags not in (0, n_atoms):
-            self.report("If set, magnetization_per_site needs a value for every atom.")
-            return self.exit_codes.ERROR_TERMINATION
-
-        an_out = analyze_structure(
-            self.inputs.structure, self.inputs.magnetization_per_site
-        )
+        self.report("Setting up workchain")
 
-        self.ctx.mol_struct = an_out["mol_struct"]
-        self.ctx.mol_mag_per_site = an_out["mol_mag_per_site"]
-
-        return ExitCode(0)
-
-    def gas_opt_selected(self):
-        return self.inputs.geo_opt.value
-
-    def gas_opt(self):
-        builder = Cp2kMoleculeOptWorkChain.get_builder()
-        builder.code = self.inputs.code
-        builder.structure = self.ctx.mol_struct
-        builder.multiplicity = self.inputs.multiplicity
-        builder.magnetization_per_site = self.ctx.mol_mag_per_site
-        builder.vdw = Bool(True)
-        builder.protocol = Str("standard")
-        if self.inputs.debug.value:
-            builder.protocol = Str("debug")
-        builder.options = self.inputs.options.geo_opt
-        builder.metadata.description = "Submitted by Cp2kMoleculeOptGwWorkChain."
-        builder.metadata.label = "Cp2kMoleculeOptWorkChain"
-        submitted_node = self.submit(builder)
-        return ToContext(gas_opt=submitted_node)
-
-    def check_gas_opt(self):
-        if not self.ctx.gas_opt.is_finished_ok:
-            return self.exit_codes.ERROR_TERMINATION
-        # set the optimized geometry as ctx geometry
-
-        self.ctx.mol_struct = self.ctx.gas_opt.outputs.output_structure
-        return ExitCode(0)
-
-    def gw(self):
-
-        self.report("Submitting GW.")
-
-        builder = Cp2kMoleculeGwWorkChain.get_builder()
-        builder.code = self.inputs.code
-        builder.protocol = self.inputs.protocol
-        builder.structure = self.ctx.mol_struct
-        builder.magnetization_per_site = self.ctx.mol_mag_per_site
-        builder.multiplicity = self.inputs.multiplicity
-        builder.debug = self.inputs.debug
-        builder.options.scf = self.inputs.options.geo_opt
-        builder.options.gw = self.inputs.options.gw
-        builder.metadata.description = "gw"
-        submitted_node = self.submit(builder)
-        return ToContext(gw=submitted_node)
+        self.ctx.n_slab_atoms = len(self.inputs.slabsys_structure.sites)
+        self.ctx.slab_options = self.inputs.options["slab"]
+        self.ctx.mol_options = self.inputs.options["molecule"]
+        emax = float(self.inputs.overlap_params.get_dict()["--emax1"])
+        nlumo = int(self.inputs.overlap_params.get_dict()["--nlumo2"])
+
+        # Set up slab DFT parameters.
+        self.ctx.slab_dft_params = copy.deepcopy(self.inputs.dft_params.get_dict())
+        self.ctx.slab_dft_params["added_mos"] = np.max(
+            [100, int(1.2 * self.ctx.n_slab_atoms * emax / 5.0)]
+        )
+
+        # Set up mol DFT parameters.
+        self.ctx.mol_dft_params = copy.deepcopy(self.ctx.slab_dft_params)
+        self.ctx.mol_dft_params["added_mos"] = nlumo + 2
+
+        # Force same cutoff for molecule and slab.
+        self.ctx.mol_dft_params["cutoff"] = cp2k_utils.get_cutoff(
+            self.inputs.slabsys_structure
+        )
+        self.ctx.mol_dft_params[
+            "elpa_switch"
+        ] = False  # Elpa can cause problems with small systems
+
+        slab_atoms = self.inputs.slabsys_structure.get_ase()
+        mol_atoms = self.inputs.mol_structure.get_ase()
+
+        if self.ctx.mol_dft_params["uks"]:
+            mol_spin_up = []
+            mol_spin_dw = []
+            mol_at_tuples = [
+                (e, *np.round(p, 2))
+                for e, p in zip(mol_atoms.get_chemical_symbols(), mol_atoms.positions)
+            ]
+
+            for i_up in self.ctx.mol_dft_params["spin_up_guess"]:
+                at = slab_atoms[i_up]
+                at_tup = (at.symbol, *np.round(at.position, 2))
+                if at_tup in mol_at_tuples:
+                    mol_spin_up.append(mol_at_tuples.index(at_tup))
+
+            for i_dw in self.ctx.mol_dft_params["spin_dw_guess"]:
+                at = slab_atoms[i_dw]
+                at_tup = (at.symbol, *np.round(at.position, 2))
+                if at_tup in mol_at_tuples:
+                    mol_spin_dw.append(mol_at_tuples.index(at_tup))
+
+            self.ctx.mol_dft_params["spin_up_guess"] = mol_spin_up
+            self.ctx.mol_dft_params["spin_dw_guess"] = mol_spin_dw
+
+    def run_diags(self):
+        # Slab part.
+        self.report("Running Diag Workchain for slab")
+
+        builder = Cp2kDiagWorkChain.get_builder()
+        builder.cp2k_code = self.inputs.cp2k_code
+        builder.structure = self.inputs.slabsys_structure
+        builder.dft_params = orm.Dict(self.ctx.slab_dft_params)
+        builder.settings = orm.Dict({"additional_retrieve_list": ["*.pdos"]})
+        builder.options = orm.Dict(self.ctx.slab_options)
+
+        # Restart WFN.
+        if "parent_calc_folder" in self.inputs:
+            builder.parent_calc_folder = self.inputs.parent_calc_folder
+        # PDOS.
+        if self.inputs.pdos_lists is not None:
+            builder.pdos_lists = orm.List([pdos[0] for pdos in self.inputs.pdos_lists])
+
+        slab_future = self.submit(builder)
+        self.to_context(slab_diag_scf=slab_future)
+        # End slab part.
+
+        # Molecule part.
+        self.report("Running Diag Workchain for molecule")
+
+        builder = Cp2kDiagWorkChain.get_builder()
+        builder.cp2k_code = self.inputs.cp2k_code
+        builder.structure = self.inputs.mol_structure
+        builder.dft_params = orm.Dict(self.ctx.mol_dft_params)
+        builder.options = orm.Dict(self.ctx.mol_options)
+
+        mol_future = self.submit(builder)
+        self.to_context(mol_diag_scf=mol_future)
+        # End molecule part.
+
+    def run_overlap(self):
+        for calculation in [self.ctx.slab_diag_scf, self.ctx.mol_diag_scf]:
+            if not common_utils.check_if_calc_ok(self, calculation):
+                return self.exit_codes.ERROR_TERMINATION
+        self.report("Running overlap")
+
+        inputs = {}
+        inputs["metadata"] = {}
+        inputs["metadata"]["label"] = "overlap"
+        inputs["code"] = self.inputs.overlap_code
+        inputs["parameters"] = self.inputs.overlap_params
+        inputs["parent_slab_folder"] = self.ctx.slab_diag_scf.outputs.remote_folder
+        inputs["parent_mol_folder"] = self.ctx.mol_diag_scf.outputs.remote_folder
+
+        n_machines = 4 if self.ctx.n_slab_atoms < 2000 else 8
+
+        inputs["metadata"]["options"] = {
+            "resources": {"num_machines": n_machines},
+            "max_wallclock_seconds": 86400,
+        }
+
+        if self.inputs.dft_params["protocol"] == "debug":
+            inputs["metadata"]["options"]["max_wallclock_seconds"] = 600
+        settings = orm.Dict({"additional_retrieve_list": ["overlap.npz"]})
+        inputs["settings"] = settings
+        future = self.submit(OverlapCalculation, **inputs)
+        return engine.ToContext(overlap=future)
 
     def finalize(self):
-        self.report("Finalizing...")
-
-        if not self.ctx.gw.is_finished_ok:
+        if "overlap.npz" not in [
+            obj.name for obj in self.ctx.overlap.outputs.retrieved.list_objects()
+        ]:
+            self.report("Overlap calculation did not finish correctly")
             return self.exit_codes.ERROR_TERMINATION
+        self.out("slab_retrieved", self.ctx.slab_diag_scf.outputs.retrieved)
 
-        gw_out_params = self.ctx.gw.outputs.gw_output_parameters
-        self.out("gw_output_parameters", gw_out_params)
-
-        self.out("output_structure", self.ctx.mol_struct)
-        # Add the workchain pk to the input/geo_opt structure extras
-
-        struc_to_label = self.ctx.mol_struct
-        extras_label = "Cp2kMoleculeOptGwWorkChain_pks"
-        if extras_label not in struc_to_label.base.extras.all:
-            extras_list = []
-        else:
-            extras_list = struc_to_label.base.extras.all[extras_label]
-        extras_list.append(self.node.pk)
-        struc_to_label.base.extras.set(extras_label, extras_list)
-
-        return ExitCode(0)
+        # Add the workchain uuid to the input structure extras.
+        common_utils.add_extras(
+            self.inputs.slabsys_structure, "surfaces", self.node.uuid
+        )
+        self.report("Work chain is finished")
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/bulk_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 standard:
     GLOBAL:
-        EXTENDED_FFT_LENGTHS: ''
+        EXTENDED_FFT_LENGTHS: ""
         PRINT_LEVEL: MEDIUM
-        RUN_TYPE: GEO_OPT
+        RUN_TYPE: ENERGY
         WALLTIME: 600
-    MOTION:
-        CONSTRAINT:
-            FIXED_ATOMS:
-                LIST: ''
-        GEO_OPT:
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.0001
-            RMS_DR: 0.001
-            RMS_FORCE: 0.0001
-            MAX_DR: 0.003
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
-        PRINT:
-            RESTART_HISTORY:
-                _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
         SUBSYS:
             CELL:
                 PERIODIC: XYZ
         DFT:
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
             CHARGE: 0
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
             QS:
                 EPS_DEFAULT: 1.0E-14
                 EXTRAPOLATION: ASPC
                 EXTRAPOLATION_ORDER: 3
@@ -48,77 +35,71 @@
                 OUTER_SCF:
                     EPS_SCF: 1.0E-7
                     MAX_SCF: 50
                 PRINT:
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
-                            GEO_OPT: 1
+                            GEO_OPT: 0
                             QS_SCF: 0
                         FILENAME: RESTART
                     RESTART_HISTORY:
-                        _: 'OFF'
+                        _: "OFF"
             XC:
                 VDW_POTENTIAL:
                     DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
                     PAIR_POTENTIAL:
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
-                        _: PBE
+                    _: PBE
             PRINT:
                 MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                    NHOMO: "1"
+                    NLUMO: "1"
+                    STRIDE: "4 4 4"
+                    EACH:
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
                 E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
+                    STRIDE: "2 2 2"
                     EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
+                V_HARTREE_CUBE:
+                    STRIDE: "2 2 2"
+                    FILENAME: "HART"
+                    EACH:
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
 low_accuracy:
     GLOBAL:
-        EXTENDED_FFT_LENGTHS: ''
+        EXTENDED_FFT_LENGTHS: ""
         PRINT_LEVEL: MEDIUM
-        RUN_TYPE: GEO_OPT
+        RUN_TYPE: ENERGY
         WALLTIME: 600
-    MOTION:
-        CONSTRAINT:
-            FIXED_ATOMS:
-                LIST: ''
-        GEO_OPT:
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.00045
-            RMS_DR: 0.0015
-            RMS_FORCE: 0.0003
-            MAX_DR: 0.003
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
-        PRINT:
-            RESTART_HISTORY:
-                _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
         SUBSYS:
             CELL:
                 PERIODIC: XYZ
         DFT:
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
             CHARGE: 0
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
             QS:
                 EPS_DEFAULT: 1.0E-14
                 EXTRAPOLATION: ASPC
                 EXTRAPOLATION_ORDER: 3
@@ -137,119 +118,120 @@
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
                             GEO_OPT: 1
                             QS_SCF: 0
                         FILENAME: RESTART
                     RESTART_HISTORY:
-                        _: 'OFF'
+                        _: "OFF"
             XC:
                 VDW_POTENTIAL:
                     DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
                     PAIR_POTENTIAL:
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
-                        _: PBE
+                    _: PBE
             PRINT:
                 MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                    NHOMO: "1"
+                    NLUMO: "1"
+                    STRIDE: "4 4 4"
+                    EACH:
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
                 E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
+                    STRIDE: "2 2 2"
                     EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
+                V_HARTREE_CUBE:
+                    STRIDE: "2 2 2"
+                    FILENAME: "HART"
+                    EACH:
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
 debug:
     GLOBAL:
-        EXTENDED_FFT_LENGTHS: ''
+        EXTENDED_FFT_LENGTHS: ""
         PRINT_LEVEL: MEDIUM
-        RUN_TYPE: GEO_OPT
+        RUN_TYPE: ENERGY
         WALLTIME: 600
-    MOTION:
-        CONSTRAINT:
-            FIXED_ATOMS:
-                LIST: ''
-        GEO_OPT:
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.1
-            RMS_DR: 0.1
-            RMS_FORCE: 0.1
-            MAX_DR: 0.1
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
-        PRINT:
-            RESTART_HISTORY:
-                _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
         SUBSYS:
             CELL:
                 PERIODIC: XYZ
         DFT:
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
             CHARGE: 0
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
             QS:
                 EPS_DEFAULT: 1.0E-14
                 EXTRAPOLATION: ASPC
                 EXTRAPOLATION_ORDER: 3
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
-                EPS_SCF: 1.0E-2
+                EPS_SCF: 5.0E-2
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
                     PRECONDITIONER: FULL_SINGLE_INVERSE
                 OUTER_SCF:
-                    EPS_SCF: 1.0E-2
+                    EPS_SCF: 5.0E-2
                     MAX_SCF: 50
                 PRINT:
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
                             GEO_OPT: 1
                             QS_SCF: 0
                         FILENAME: RESTART
                     RESTART_HISTORY:
-                        _: 'OFF'
+                        _: "OFF"
             XC:
                 VDW_POTENTIAL:
                     DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
                     PAIR_POTENTIAL:
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
-                        _: PBE
+                    _: PBE
             PRINT:
                 MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                    NHOMO: "1"
+                    NLUMO: "1"
+                    STRIDE: "4 4 4"
+                    EACH:
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
                 E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
+                    STRIDE: "2 2 2"
                     EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
+                V_HARTREE_CUBE:
+                    STRIDE: "2 2 2"
+                    FILENAME: "HART"
+                    EACH:
+                        QS_SCF: "0"
+                        GEO_OPT: "0"
+                    ADD_LAST: "NUMERIC"
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,64 @@
 standard:
     GLOBAL:
         EXTENDED_FFT_LENGTHS: ''
         PRINT_LEVEL: MEDIUM
-        RUN_TYPE: CELL_OPT
+        RUN_TYPE: BAND
         WALLTIME: 600
     MOTION:
-        CELL_OPT:
-            EXTERNAL_PRESSURE: 0
-            PRESSURE_TOLERANCE: 100
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.0001
-            RMS_DR: 0.001
-            RMS_FORCE: 0.0001
-            MAX_DR: 0.003
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
-            TYPE: DIRECT_CELL_OPT
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
+        BAND:
+            ALIGN_FRAMES: .FALSE.
+            BAND_TYPE: CI-NEB
+            CI_NEB:
+                NSTEPS_IT: 5
+            CONVERGENCE_CONTROL:
+                MAX_DR: 0.002
+                MAX_FORCE: 0.0001
+                RMS_DR: 0.005
+                RMS_FORCE: 0.001
+            CONVERGENCE_INFO :
+                _: ''
+            K_SPRING: 0.05
+            NPROC_REP: 1
+            NUMBER_OF_REPLICA: 3
+            OPTIMIZE_BAND:
+                DIIS:
+                    MAX_STEPS: 1000
+                OPTIMIZE_END_POINTS: .FALSE.
+                OPT_TYPE: DIIS
+            PROGRAM_RUN_INFO:
+                INITIAL_CONFIGURATION_INFO: ''
         PRINT:
             RESTART_HISTORY:
                 _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
-        STRESS_TENSOR: ANALYTICAL
         SUBSYS:
             CELL:
                 PERIODIC: XYZ
                 SYMMETRY: ORTHORHOMBIC
         DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
+            CHARGE: 0
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
-            RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
-            CHARGE: 0
+            RESTART_FILE_NAME: RESTART
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             QS:
                 EPS_DEFAULT: 1.0E-14
-                EXTRAPOLATION: ASPC
-                EXTRAPOLATION_ORDER: 3
+                EXTRAPOLATION: USE_GUESS
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
                 EPS_SCF: 1.0E-7
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
@@ -66,70 +82,71 @@
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
                         _: PBE
-            PRINT:
-                MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        CELL_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
-                E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        CELL_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
 low_accuracy:
     GLOBAL:
         EXTENDED_FFT_LENGTHS: ''
         PRINT_LEVEL: MEDIUM
-        RUN_TYPE: CELL_OPT
+        RUN_TYPE: BAND
         WALLTIME: 600
     MOTION:
-        CELL_OPT:
-            EXTERNAL_PRESSURE: 0
-            PRESSURE_TOLERANCE: 100
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.00045
-            RMS_DR: 0.0015
-            RMS_FORCE: 0.0003
-            MAX_DR: 0.003
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
-            TYPE: DIRECT_CELL_OPT
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
+        BAND:
+            ALIGN_FRAMES: .FALSE.
+            BAND_TYPE: CI-NEB
+            CI_NEB:
+                NSTEPS_IT: 5
+            CONVERGENCE_CONTROL:
+                MAX_DR: 0.002
+                MAX_FORCE: 0.00045
+                RMS_DR: 0.005
+                RMS_FORCE: 0.003
+            CONVERGENCE_INFO :
+                _: ''
+            K_SPRING: 0.05
+            NPROC_REP: 1
+            NUMBER_OF_REPLICA: 3
+            OPTIMIZE_BAND:
+                DIIS:
+                    MAX_STEPS: 1000
+                OPTIMIZE_END_POINTS: .FALSE.
+                OPT_TYPE: DIIS
+            PROGRAM_RUN_INFO:
+                INITIAL_CONFIGURATION_INFO: ''
         PRINT:
             RESTART_HISTORY:
                 _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
-        STRESS_TENSOR: ANALYTICAL
         SUBSYS:
             CELL:
                 PERIODIC: XYZ
                 SYMMETRY: ORTHORHOMBIC
         DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
+            CHARGE: 0
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
-            CHARGE: 0
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             QS:
                 EPS_DEFAULT: 1.0E-14
-                EXTRAPOLATION: ASPC
-                EXTRAPOLATION_ORDER: 3
+                EXTRAPOLATION: USE_GUESS
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
                 EPS_SCF: 1.0E-6
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
@@ -153,80 +170,81 @@
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
                         _: PBE
-            PRINT:
-                MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        CELL_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
-                E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        CELL_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
 debug:
     GLOBAL:
         EXTENDED_FFT_LENGTHS: ''
         PRINT_LEVEL: MEDIUM
-        RUN_TYPE: CELL_OPT
+        RUN_TYPE: BAND
         WALLTIME: 600
     MOTION:
-        CELL_OPT:
-            EXTERNAL_PRESSURE: 90000
-            PRESSURE_TOLERANCE: 15000
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.1
-            RMS_DR: 0.1
-            RMS_FORCE: 0.1
-            MAX_DR: 0.1
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
-            TYPE: DIRECT_CELL_OPT
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
+        BAND:
+            ALIGN_FRAMES: .FALSE.
+            BAND_TYPE: CI-NEB
+            CI_NEB:
+                NSTEPS_IT: 1
+            CONVERGENCE_CONTROL:
+                MAX_DR: 5
+                MAX_FORCE: 5
+                RMS_DR: 5
+                RMS_FORCE: 5
+            CONVERGENCE_INFO :
+                _: ''
+            K_SPRING: 0.05
+            NPROC_REP: 1
+            NUMBER_OF_REPLICA: 3
+            OPTIMIZE_BAND:
+                DIIS:
+                    MAX_STEPS: 2
+                OPTIMIZE_END_POINTS: .FALSE.
+                OPT_TYPE: DIIS
+            PROGRAM_RUN_INFO:
+                INITIAL_CONFIGURATION_INFO: ''
         PRINT:
             RESTART_HISTORY:
                 _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
-        STRESS_TENSOR: ANALYTICAL
         SUBSYS:
             CELL:
                 PERIODIC: XYZ
                 SYMMETRY: ORTHORHOMBIC
         DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
+            CHARGE: 0
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
-            CHARGE: 0
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             QS:
                 EPS_DEFAULT: 1.0E-14
-                EXTRAPOLATION: ASPC
-                EXTRAPOLATION_ORDER: 3
+                EXTRAPOLATION: USE_GUESS
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
-                EPS_SCF: 1.0E-2
+                EPS_SCF: 1.0E-1
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
                     PRECONDITIONER: FULL_SINGLE_INVERSE
                 OUTER_SCF:
-                    EPS_SCF: 1.0E-2
+                    EPS_SCF: 1.0E-1
                     MAX_SCF: 50
                 PRINT:
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
                             GEO_OPT: 1
                             QS_SCF: 0
@@ -240,22 +258,7 @@
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
                         _: PBE
-            PRINT:
-                MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        CELL_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
-                E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        CELL_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/protocols/molecule_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,255 +1,332 @@
-standard:
+phonons:
     GLOBAL:
         EXTENDED_FFT_LENGTHS: ''
-        PRINT_LEVEL: MEDIUM
-        RUN_TYPE: GEO_OPT
+        PRINT_LEVEL: LOW
+        RUN_TYPE: NORMAL_MODES
         WALLTIME: 600
+        PREFERRED_DIAG_LIBRARY: ELPA
+        ELPA_KERNEL: AUTO
+        DBCSR:
+            USE_MPI_ALLOCATOR: .FALSE.
+    VIBRATIONAL_ANALYSIS:
+        FULLY_PERIODIC: .TRUE.
+        NPROC_REP: 228
+        DX: 0.002
+        INTENSITIES: ''
+        PRINT:
+            PROGRAM_RUN_INFO:
+                _: 'ON'
     MOTION:
-        GEO_OPT:
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.000100
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
         PRINT:
             RESTART_HISTORY:
                 _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
         SUBSYS:
             CELL:
-                PERIODIC: NONE
+                PERIODIC: XYZ
                 SYMMETRY: ORTHORHOMBIC
         DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
+            CHARGE: 0
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
+            MGRID:
+                CUTOFF: 600
+                NGRIDS: 5
+            POISSON:
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
+            QS:
+                EPS_DEFAULT: 1.0E-14
+                EXTRAPOLATION: ASPC
+                EXTRAPOLATION_ORDER: 3
+                METHOD: GPW
+            SCF:
+                SCF_GUESS: RESTART
+                EPS_SCF: 1.0E-9
+                MAX_SCF: 40
+                OT:
+                    MINIMIZER: CG
+                    PRECONDITIONER: FULL_SINGLE_INVERSE
+                OUTER_SCF:
+                    EPS_SCF: 1.0E-9
+                    MAX_SCF: 50
+                PRINT:
+                    RESTART:
+                        ADD_LAST: NUMERIC
+                        EACH:
+                            GEO_OPT: 1
+                            QS_SCF: 0
+                        FILENAME: RESTART
+                    RESTART_HISTORY:
+                        _: 'OFF'
+                        BACKUP_COPIES: 0
+            XC:
+                VDW_POTENTIAL:
+                    DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
+                    PAIR_POTENTIAL:
+                        CALCULATE_C9_TERM: .TRUE.
+                        PARAMETER_FILE_NAME: dftd3.dat
+                        REFERENCE_FUNCTIONAL: PBE
+                        R_CUTOFF: 15
+                        TYPE: DFTD3
+                XC_FUNCTIONAL:
+                        _: PBE
+            PRINT:
+                MOMENTS:
+                    PERIODIC: .TRUE.
+standard:
+    GLOBAL:
+        EXTENDED_FFT_LENGTHS: ''
+        PRINT_LEVEL: LOW
+        RUN_TYPE: NORMAL_MODES
+        WALLTIME: 600
+        PREFERRED_DIAG_LIBRARY: ELPA
+        ELPA_KERNEL: AUTO
+        DBCSR:
+            USE_MPI_ALLOCATOR: .FALSE.
+    VIBRATIONAL_ANALYSIS:
+        FULLY_PERIODIC: .TRUE.
+        NPROC_REP: 228
+        DX: 0.002
+        INTENSITIES: ''
+        PRINT:
+            PROGRAM_RUN_INFO:
+                _: 'ON'
+    MOTION:
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
+        PRINT:
+            RESTART_HISTORY:
+                _: 'OFF'
+    FORCE_EVAL:
+        METHOD: Quickstep
+        SUBSYS:
+            CELL:
+                PERIODIC: XYZ
+                SYMMETRY: ORTHORHOMBIC
+        DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
             CHARGE: 0
+            BASIS_SET_FILE_NAME: BASIS_MOLOPT
+            POTENTIAL_FILE_NAME: POTENTIAL
+            RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
             POISSON:
-                PERIODIC: NONE
-                PSOLVER: MT
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             QS:
                 EPS_DEFAULT: 1.0E-14
                 EXTRAPOLATION: ASPC
                 EXTRAPOLATION_ORDER: 3
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
-                EPS_SCF: 1.0E-7
+                EPS_SCF: 1.0E-9
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
                     PRECONDITIONER: FULL_SINGLE_INVERSE
                 OUTER_SCF:
-                    EPS_SCF: 1.0E-7
+                    EPS_SCF: 1.0E-9
                     MAX_SCF: 50
                 PRINT:
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
                             GEO_OPT: 1
                             QS_SCF: 0
                         FILENAME: RESTART
                     RESTART_HISTORY:
                         _: 'OFF'
+                        BACKUP_COPIES: 0
             XC:
                 VDW_POTENTIAL:
                     DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
                     PAIR_POTENTIAL:
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
                         _: PBE
             PRINT:
-                MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
-                E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                MOMENTS:
+                    PERIODIC: .TRUE.
 low_accuracy:
     GLOBAL:
         EXTENDED_FFT_LENGTHS: ''
-        PRINT_LEVEL: MEDIUM
-        RUN_TYPE: GEO_OPT
+        PRINT_LEVEL: LOW
+        RUN_TYPE: NORMAL_MODES
         WALLTIME: 600
+        PREFERRED_DIAG_LIBRARY: ELPA
+        ELPA_KERNEL: AUTO
+        DBCSR:
+            USE_MPI_ALLOCATOR: .FALSE.
+    VIBRATIONAL_ANALYSIS:
+        FULLY_PERIODIC: .TRUE.
+        NPROC_REP: 228
+        DX: 0.002
+        INTENSITIES: ''
+        PRINT:
+            PROGRAM_RUN_INFO:
+                _: 'ON'
     MOTION:
-        GEO_OPT:
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.00045
-            RMS_DR: 0.0015
-            RMS_FORCE: 0.0003
-            MAX_DR: 0.003
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
         PRINT:
             RESTART_HISTORY:
                 _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
         SUBSYS:
             CELL:
-                PERIODIC: NONE
+                PERIODIC: XYZ
                 SYMMETRY: ORTHORHOMBIC
         DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
+            CHARGE: 0
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
-            CHARGE: 0
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
             POISSON:
-                PERIODIC: NONE
-                PSOLVER: MT
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             QS:
                 EPS_DEFAULT: 1.0E-14
                 EXTRAPOLATION: ASPC
                 EXTRAPOLATION_ORDER: 3
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
-                EPS_SCF: 1.0E-6
+                EPS_SCF: 1.0E-9
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
                     PRECONDITIONER: FULL_SINGLE_INVERSE
                 OUTER_SCF:
-                    EPS_SCF: 1.0E-6
+                    EPS_SCF: 1.0E-9
                     MAX_SCF: 50
                 PRINT:
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
                             GEO_OPT: 1
                             QS_SCF: 0
                         FILENAME: RESTART
                     RESTART_HISTORY:
                         _: 'OFF'
+                        BACKUP_COPIES: 0
             XC:
                 VDW_POTENTIAL:
                     DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
                     PAIR_POTENTIAL:
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
                         _: PBE
             PRINT:
-                MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
-                E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                MOMENTS:
+                    PERIODIC: .TRUE.
 debug:
     GLOBAL:
         EXTENDED_FFT_LENGTHS: ''
-        PRINT_LEVEL: MEDIUM
-        RUN_TYPE: GEO_OPT
+        PRINT_LEVEL: LOW
+        RUN_TYPE: NORMAL_MODES
         WALLTIME: 600
+        PREFERRED_DIAG_LIBRARY: ELPA
+        ELPA_KERNEL: AUTO
+        DBCSR:
+            USE_MPI_ALLOCATOR: .FALSE.
+    VIBRATIONAL_ANALYSIS:
+        FULLY_PERIODIC: .TRUE.
+        NPROC_REP: 228
+        DX: 0.002
+        INTENSITIES: ''
+        PRINT:
+            PROGRAM_RUN_INFO:
+                _: 'ON'
     MOTION:
-        GEO_OPT:
-            BFGS:
-                TRUST_RADIUS: '[bohr] 0.1'
-            MAX_FORCE: 0.1
-            RMS_DR: 0.1
-            RMS_FORCE: 0.1
-            MAX_DR: 0.1
-            MAX_ITER: 1000
-            OPTIMIZER: BFGS
+        CONSTRAINT:
+            FIXED_ATOMS:
+                LIST: ''
         PRINT:
             RESTART_HISTORY:
                 _: 'OFF'
     FORCE_EVAL:
         METHOD: Quickstep
         SUBSYS:
             CELL:
-                PERIODIC: NONE
+                PERIODIC: XYZ
                 SYMMETRY: ORTHORHOMBIC
         DFT:
+            UKS: .FALSE.
+            MULTIPLICITY: 0
+            CHARGE: 0
             BASIS_SET_FILE_NAME: BASIS_MOLOPT
             POTENTIAL_FILE_NAME: POTENTIAL
             RESTART_FILE_NAME: ./parent_calc/aiida-RESTART.wfn
-            CHARGE: 0
             MGRID:
                 CUTOFF: 600
                 NGRIDS: 5
             POISSON:
-                PERIODIC: NONE
-                PSOLVER: MT
+                PERIODIC: XYZ
+                POISSON_SOLVER: PERIODIC
             QS:
                 EPS_DEFAULT: 1.0E-14
                 EXTRAPOLATION: ASPC
                 EXTRAPOLATION_ORDER: 3
                 METHOD: GPW
             SCF:
                 SCF_GUESS: RESTART
-                EPS_SCF: 1.0E-2
+                EPS_SCF: 1.0
                 MAX_SCF: 40
                 OT:
                     MINIMIZER: CG
                     PRECONDITIONER: FULL_SINGLE_INVERSE
                 OUTER_SCF:
-                    EPS_SCF: 1.0E-2
+                    EPS_SCF: 1.0
                     MAX_SCF: 50
                 PRINT:
                     RESTART:
                         ADD_LAST: NUMERIC
                         EACH:
                             GEO_OPT: 1
                             QS_SCF: 0
                         FILENAME: RESTART
                     RESTART_HISTORY:
                         _: 'OFF'
+                        BACKUP_COPIES: 0
             XC:
                 VDW_POTENTIAL:
                     DISPERSION_FUNCTIONAL: PAIR_POTENTIAL
                     PAIR_POTENTIAL:
                         CALCULATE_C9_TERM: .TRUE.
                         PARAMETER_FILE_NAME: dftd3.dat
                         REFERENCE_FUNCTIONAL: PBE
                         R_CUTOFF: 15
                         TYPE: DFTD3
                 XC_FUNCTIONAL:
                         _: PBE
             PRINT:
-                MO_CUBES:
-                    NHOMO: '1'
-                    NLUMO: '1'
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
-                E_DENSITY_CUBE:
-                    STRIDE: '4 4 4'
-                    EACH:
-                        QS_SCF: '0'
-                        GEO_OPT: '0'
-                    ADD_LAST: 'NUMERIC'
+                MOMENTS:
+                    PERIODIC: .TRUE.
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/cp2k/slab_opt_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,250 @@
-import copy
-import os
-import pathlib
-
-import yaml
-from aiida.engine import ExitCode, ToContext, WorkChain
-from aiida.orm import Bool, Code, Dict, Int, List, SinglefileData, Str, StructureData
-from aiida.plugins import WorkflowFactory
-
-from aiida_nanotech_empa.utils import analyze_structure, common_utils
-from aiida_nanotech_empa.workflows.cp2k.cp2k_utils import (
-    determine_kinds,
-    dict_merge,
-    get_cutoff,
-    get_kinds_section,
-)
+from aiida import engine, orm, plugins
 
-Cp2kBaseWorkChain = WorkflowFactory("cp2k.base")
+from ...utils import common_utils
+from . import common
 
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
 
-class Cp2kSlabOptWorkChain(WorkChain):
+
+@engine.calcfunction
+def subtract(a, b):
+    return a - b
+
+
+class GaussianDeltaScfWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
-        spec.input("code", valid_type=Code)
-        spec.input("structure", valid_type=StructureData)
+
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
-            "charge",  # +1 means one electron removed
-            valid_type=Int,
-            default=lambda: Int(0),
-            required=False,
-        )
-        spec.input(
-            "fixed_atoms", valid_type=Str, default=lambda: Str(""), required=False
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
         )
         spec.input(
-            "multiplicity", valid_type=Int, default=lambda: Int(0), required=False
+            "functional", valid_type=orm.Str, required=True, help="xc functional"
         )
+
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="basis_set")
+
         spec.input(
-            "magnetization_per_site",
-            valid_type=List,
-            default=lambda: List(list=[]),
+            "multiplicity",
+            valid_type=orm.Int,
             required=False,
+            default=lambda: orm.Int(1),
+            help="spin multiplicity; 0 means RKS",
         )
-        spec.input("vdw", valid_type=Bool, default=lambda: Bool(False), required=False)
+
         spec.input(
-            "protocol",
-            valid_type=Str,
-            default=lambda: Str("standard"),
+            "parent_calc_folder",
+            valid_type=orm.RemoteData,
             required=False,
-            help="Settings to run simulations with.",
+            help="the folder of a completed gaussian calculation",
         )
+
         spec.input(
             "options",
-            valid_type=dict,
-            non_db=True,
+            valid_type=orm.Dict,
             required=False,
-            help="Define options for the cacluations: walltime, memory, CPUs, etc.",
+            help="Use custom metadata.options instead of the automatic ones.",
         )
 
-        # workchain outline
-        spec.outline(cls.setup, cls.submit_calc, cls.finalize)
+        spec.outline(cls.setup, cls.submit_scfs, cls.finalize)
+
         spec.outputs.dynamic = True
 
         spec.exit_code(
+            301,
+            "ERROR_MULTIPLICITY",
+            message="Multiplicity and number of el. doesn't match.",
+        )
+        spec.exit_code(
+            302,
+            "ERROR_OPTIONS",
+            message="Input options are invalid.",
+        )
+        spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
+    def is_uks(self):
+        if self.inputs.multiplicity.value == 0:
+            return False
+        return True
+
     def setup(self):
-        self.report("Inspecting input and setting up things")
+        self.report("Inspecting input and setting up things.")
+
+        common.setup_context_variables(self)
 
-        # --------------------------------------------------
+        if self.ctx.mult % 2 == self.ctx.n_electrons % 2:
+            return self.exit_codes.ERROR_MULTIPLICITY
 
-    def submit_calc(self):
-        with open(
-            pathlib.Path(__file__).parent / "./protocols/slab_opt_protocol.yml",
-            encoding="utf-8",
-        ) as handle:
-            protocols = yaml.safe_load(handle)
-            input_dict = copy.deepcopy(protocols[self.inputs.protocol.value])
-
-        structure = self.inputs.structure
-        # cutoff
-        self.ctx.cutoff = get_cutoff(structure=structure)
-
-        # get initial magnetization
-        magnetization_per_site = copy.deepcopy(self.inputs.magnetization_per_site)
-        structure_with_tags, kinds_dict = determine_kinds(
-            structure, magnetization_per_site
-        )
-
-        ase_atoms = structure_with_tags.get_ase()
-
-        builder = Cp2kBaseWorkChain.get_builder()
-        builder.cp2k.code = self.inputs.code
-        builder.cp2k.structure = StructureData(ase=ase_atoms)
-        builder.cp2k.file = {
-            "basis": SinglefileData(
-                file=os.path.join(
-                    os.path.dirname(os.path.realpath(__file__)),
-                    ".",
-                    "data",
-                    "BASIS_MOLOPT",
-                )
-            ),
-            "pseudo": SinglefileData(
-                file=os.path.join(
-                    os.path.dirname(os.path.realpath(__file__)),
-                    ".",
-                    "data",
-                    "POTENTIAL",
-                )
-            ),
+        success = common.determine_metadata_options(self)
+        if not success:
+            return self.exit_codes.ERROR_OPTIONS
+
+        num_cores, memory_mb = common.get_gaussian_cores_and_memory(
+            self.ctx.metadata_options, self.ctx.comp
+        )
+
+        self.ctx.link0 = {
+            "%chk": "aiida.chk",
+            "%mem": "%dMB" % memory_mb,
+            "%nprocshared": str(num_cores),
         }
 
-        # charge
-        input_dict["FORCE_EVAL"]["DFT"]["CHARGE"] = self.inputs.charge.value
-        # vdw
-        if not self.inputs.vdw.value:
-            input_dict["FORCE_EVAL"]["DFT"]["XC"].pop("VDW_POTENTIAL")
-
-        # UKS
-        if self.inputs.multiplicity.value > 0:
-            input_dict["FORCE_EVAL"]["DFT"]["UKS"] = ".TRUE."
-            input_dict["FORCE_EVAL"]["DFT"][
-                "MULTIPLICITY"
-            ] = self.inputs.multiplicity.value
-
-        # fixed atoms
-        input_dict["MOTION"]["CONSTRAINT"]["FIXED_ATOMS"][
-            "LIST"
-        ] = self.inputs.fixed_atoms.value
-
-        # cutoff
-        input_dict["FORCE_EVAL"]["DFT"]["MGRID"]["CUTOFF"] = self.ctx.cutoff
-
-        # KINDS section
-        self.ctx.kinds_section = get_kinds_section(kinds_dict, protocol="gpw")
-        dict_merge(input_dict, self.ctx.kinds_section)
-
-        # Setup options.
-        if "options" in self.inputs:
-            builder.cp2k.metadata.options = self.inputs.options
-
-        # Setup walltime.
-        if "max_wallclock_seconds" in self.inputs.options:
-            input_dict["GLOBAL"]["WALLTIME"] = max(
-                self.inputs.options["max_wallclock_seconds"] - 600, 600
-            )
+        return engine.ExitCode(0)
 
-        # parser
-        builder.cp2k.metadata.options.parser_name = "cp2k_advanced_parser"
+    def setup_common_builder_params(self, builder):
+        builder.gaussian.structure = self.inputs.structure
+        builder.gaussian.code = self.inputs.gaussian_code
+        builder.gaussian.metadata.options = self.ctx.metadata_options
+
+    def submit_scfs(self):
+        self.report("Submitting NEUTRAL SCF.")
+
+        parameters = orm.Dict(
+            {
+                "link0_parameters": self.ctx.link0.copy(),
+                "functional": self.ctx.functional,
+                "basis_set": self.inputs.basis_set.value,
+                "charge": 0,
+                "multiplicity": self.ctx.mult,
+                "route_parameters": {
+                    "scf": {"conver": 7, "maxcycle": 140},
+                    "sp": None,
+                },
+            }
+        )
+
+        builder = GaussianBaseWorkChain.get_builder()
+
+        if "parent_calc_folder" in self.inputs:
+            # Read WFN from parent calc.
+            parameters["link0_parameters"]["%oldchk"] = "parent_calc/aiida.chk"
+            parameters["route_parameters"]["guess"] = "read"
+            builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
+        elif self.is_uks() and self.ctx.mult == 1:
+            # For open-shell singlet, mix homo & lumo.
+            parameters["route_parameters"]["guess"] = "mix"
 
-        # handlers
-        builder.handler_overrides = Dict(
-            {"restart_incomplete_calculation": {"enabled": True}}
-        )
+        builder.gaussian.parameters = parameters
+        self.setup_common_builder_params(builder)
+        submitted_node = self.submit(builder)
+        self.to_context(neutral=submitted_node)
+
+        self.report("Submitting CATION SCF")
 
-        # cp2k input dictionary
-        builder.cp2k.parameters = Dict(input_dict)
+        if self.ctx.mult == 1:
+            pos_mult = 2
+        else:
+            pos_mult = self.ctx.mult - 1
+
+        if self.is_uks():
+            functional = self.ctx.functional
+        else:
+            functional = "u" + self.ctx.functional
+
+        parameters = orm.Dict(
+            {
+                "link0_parameters": self.ctx.link0.copy(),
+                "functional": functional,
+                "basis_set": self.inputs.basis_set.value,
+                "charge": 1,
+                "multiplicity": pos_mult,
+                "route_parameters": {
+                    "scf": {"conver": 7, "maxcycle": 140},
+                    "sp": None,
+                },
+            }
+        )
+
+        builder = GaussianBaseWorkChain.get_builder()
+
+        if pos_mult == 1:
+            # For open-shell singlet, mix homo & lumo
+            parameters["route_parameters"]["guess"] = "mix"
 
+        builder.gaussian.parameters = parameters
+        self.setup_common_builder_params(builder)
         submitted_node = self.submit(builder)
-        return ToContext(opt=submitted_node)
+        self.to_context(pos=submitted_node)
 
-    def finalize(self):
-        self.report("Finalizing...")
+        self.report("Submitting ANION SCF")
+
+        # For the ANION, the added electron could go opposite or parallel
+        # if the system was already spin-polarized
+
+        if self.ctx.mult == 1:
+            self.ctx.neg_mults = [2]
+        else:
+            self.ctx.neg_mults = [self.ctx.mult - 1, self.ctx.mult + 1]
+
+        for neg_mult in self.ctx.neg_mults:
+            parameters = orm.Dict(
+                {
+                    "link0_parameters": self.ctx.link0.copy(),
+                    "functional": functional,
+                    "basis_set": self.inputs.basis_set.value,
+                    "charge": -1,
+                    "multiplicity": neg_mult,
+                    "route_parameters": {
+                        "scf": {"conver": 7, "maxcycle": 140},
+                        "sp": None,
+                    },
+                }
+            )
+
+            builder = GaussianBaseWorkChain.get_builder()
 
-        if not self.ctx.opt.is_finished_ok:
+            if neg_mult == 1:
+                # For open-shell singlet, mix homo & lumo.
+                parameters["route_parameters"]["guess"] = "mix"
+
+            builder.gaussian.parameters = parameters
+            self.setup_common_builder_params(builder)
+            submitted_node = self.submit(builder)
+            label = f"neg_m{neg_mult}"
+            self.to_context(**{label: submitted_node})
+
+    def finalize(self):
+        if not common_utils.check_if_calc_ok(
+            self, self.ctx.neutral
+        ) or not common_utils.check_if_calc_ok(self, self.ctx.pos):
             return self.exit_codes.ERROR_TERMINATION
 
-        for out in self.ctx.opt.outputs:
-            self.out(out, self.ctx.opt.outputs[out])
+        anion_energies = []
+
+        for neg_mult in self.ctx.neg_mults:
+            label = f"neg_m{neg_mult}"
+            if not common_utils.check_if_calc_ok(self, self.ctx[label]):
+                return self.exit_codes.ERROR_TERMINATION
+
+            anion_energies.append(self.ctx[label].outputs.energy_ev)
+
+            if len(self.ctx.neg_mults) > 1:
+                self.out(f"anion_energy_m{neg_mult}", self.ctx[label].outputs.energy_ev)
+
+        anion_energy = min(anion_energies)
+
+        self.out("neutral_energy", self.ctx.neutral.outputs.energy_ev)
+        self.out("cation_energy", self.ctx.pos.outputs.energy_ev)
+        self.out("anion_energy", anion_energy)
+
+        ip = subtract(
+            self.ctx.pos.outputs.energy_ev, self.ctx.neutral.outputs.energy_ev
+        )
+        ea = subtract(self.ctx.neutral.outputs.energy_ev, anion_energy)
 
-        # Add extras
-        struc = self.ctx.opt.outputs.output_structure
-        ase_geom = struc.get_ase()
-        self.node.base.extras.set(
-            "thumbnail", common_utils.thumbnail(ase_struc=ase_geom)
-        )
-
-        # add formula to extra as molecule@surface
-        try:  # mainly for debug cases where the analyzer could crash due to odd geometries
-            analyzer = analyze_structure.StructureAnalyzer()
-            analyzer.structure = ase_geom
-            res = analyzer.details
-
-            mol_formula = ""
-            for imol in res["all_molecules"]:
-                mol_formula += ase_geom[imol].get_chemical_formula() + " "
-            if len(res["slabatoms"]) > 0:
-                mol_formula += "at " + ase_geom[res["slabatoms"]].get_chemical_formula()
-                if len(res["bottom_H"]) > 0:
-                    mol_formula += (
-                        " saturated: "
-                        + ase_geom[res["bottom_H"]].get_chemical_formula()
-                    )
-                if len(res["adatoms"]) > 0:
-                    mol_formula += (
-                        " Adatoms: " + ase_geom[res["adatoms"]].get_chemical_formula()
-                    )
-        except ValueError:
-            mol_formula = struc.get_formula()
+        self.out("ionization_potential", ip)
+        self.out("electron_affinity", ea)
 
-        self.node.base.extras.set("formula", mol_formula)
+        self.out("fundamental_gap", subtract(ip, ea))
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/__init__.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from .delta_scf_workchain import GaussianDeltaScfWorkChain
 from .hf_mp2_workchain import GaussianHfMp2WorkChain
 from .natorb_workchain import GaussianNatOrbWorkChain
 from .relax_workchain import GaussianRelaxWorkChain
 from .scf_workchain import GaussianScfWorkChain
 from .spin_workchain import GaussianSpinWorkChain
 
-__all__ = [
+__all__ = (
     "GaussianScfWorkChain",
     "GaussianRelaxWorkChain",
     "GaussianDeltaScfWorkChain",
     "GaussianNatOrbWorkChain",
     "GaussianSpinWorkChain",
     "GaussianHfMp2WorkChain",
     "GaussianConstrOptChainWorkChain",
     "GaussianCasscfWorkChain",
     "GaussianCasscfSeriesWorkChain",
-]
+)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from aiida.engine import ExitCode, ToContext, WorkChain, if_, while_
-from aiida.orm import Bool, Code, Dict, Int, List, RemoteData, Str, StructureData
-from aiida.plugins import WorkflowFactory
-
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.gaussian import common
+from aiida import engine, orm, plugins
 
+from ...utils import common_utils
+from . import common
 from .casscf_workchain import GaussianCasscfWorkChain
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
-GaussianCubesWorkChain = WorkflowFactory("gaussian.cubes")
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
+GaussianCubesWorkChain = plugins.WorkflowFactory("gaussian.cubes")
 
 
-class GaussianCasscfSeriesWorkChain(WorkChain):
+class GaussianCasscfSeriesWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
             "nm_list",
-            valid_type=List,
+            valid_type=orm.List,
             required=True,
             help="Successive list of (n,m) tuples to run CAS(n,m).",
         )
 
         spec.input(
-            "structure", valid_type=StructureData, required=True, help="input geometry"
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
         )
 
         spec.input(
             "init_functional",
-            valid_type=Str,
+            valid_type=orm.Str,
             required=False,
-            default=lambda: Str("UHF"),
+            default=lambda: orm.Str("UHF"),
             help="Functional for the initial orbitals.",
         )
 
         spec.input(
             "start_calc_folder",
-            valid_type=RemoteData,
+            valid_type=orm.RemoteData,
             required=False,
             help="Read starting orbitals from here instead.",
         )
 
-        spec.input("basis_set", valid_type=Str, required=True, help="Basis set")
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="Basis set")
 
         spec.input(
             "multiplicity_list",
-            valid_type=List,
+            valid_type=orm.List,
             required=False,
-            default=lambda: List(list=[1, 3]),
+            default=lambda: orm.List(list=[1, 3]),
             help="spin multiplicity",
         )
 
         spec.input(
             "start_uno",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(True),
+            default=lambda: orm.Bool(True),
             help="Use natural orbitals of the start calculation.",
         )
 
         spec.input(
             "mp2",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="calculate the MP2 correction (CASMP2).",
         )
 
         spec.input(
             "num_orbital_cubes",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="Generate cubes for orbitals (n*occ and n*virt).",
         )
 
-        spec.input("formchk_code", valid_type=Code, required=False)
-        spec.input("cubegen_code", valid_type=Code, required=False)
+        spec.input("formchk_code", valid_type=orm.Code, required=False)
+        spec.input("cubegen_code", valid_type=orm.Code, required=False)
 
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
         spec.outline(
             cls.setup,
-            if_(cls.should_do_init)(cls.initial_scf),
-            while_(cls.any_multiplicity_left)(
-                while_(cls.any_casscf_nm_left)(cls.casscf)
+            engine.if_(cls.should_do_init)(cls.initial_scf),
+            engine.while_(cls.any_multiplicity_left)(
+                engine.while_(cls.any_casscf_nm_left)(cls.casscf)
             ),
             cls.finalize,
         )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
@@ -134,26 +134,25 @@
         }
 
         self.ctx.i_current_mult = 0
         self.ctx.i_current_nm = 0
 
         self.ctx.last_submitted_label = None
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
 
     def should_do_init(self):
         return "start_calc_folder" not in self.inputs
 
     def initial_scf(self):
-
         self.report("Submitting initial SCF")
 
         self.ctx.init_mult = list(self.inputs.multiplicity_list)[0]
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
                 "dieze_tag": "#P",
                 "functional": self.inputs.init_functional.value,
                 "basis_set": self.inputs.basis_set.value,
                 "charge": 0,
                 "multiplicity": self.ctx.init_mult,
@@ -174,15 +173,15 @@
         builder.gaussian.structure = self.inputs.structure
         builder.gaussian.code = self.inputs.gaussian_code
         builder.gaussian.metadata.options = self.ctx.metadata_options
 
         future = self.submit(builder)
 
         self.ctx.last_submitted_label = "init_scf"
-        return ToContext(init_scf=future)
+        return engine.ToContext(init_scf=future)
 
     def any_multiplicity_left(self):
         if self.ctx.i_current_mult == len(self.inputs.multiplicity_list):
             return False
         self.ctx.current_mult = list(self.inputs.multiplicity_list)[
             self.ctx.i_current_mult
         ]
@@ -194,90 +193,69 @@
         if self.ctx.i_current_nm == len(self.inputs.nm_list):
             return False
         self.ctx.current_nm = list(self.inputs.nm_list)[self.ctx.i_current_nm]
         self.ctx.i_current_nm += 1
         return True
 
     def casscf(self):
-
         if self.ctx.last_submitted_label is not None:
             if not common_utils.check_if_calc_ok(
                 self, self.ctx[self.ctx.last_submitted_label]
             ):
                 return self.exit_codes.ERROR_TERMINATION
 
-        # Set output already for the previous step
-        # lsc = self.ctx.last_submitted_label
-        # if lsc.startswith('cas'):
-        #    self.out(f"{lsc}_out_params",
-        #             self.ctx[lsc].outputs.output_parameters)
-        #    if 'cube_image_folder' in self.ctx[lsc].outputs:
-        #        self.out(f"{lsc}_cube_image_folder",
-        #                 self.ctx[lsc].outputs.cube_image_folder)
-
         uno = False
 
-        # determine previous node
+        # Determine previous node.
         if self.ctx.i_current_mult == 1 and self.ctx.i_current_nm == 1:
-            # first one uses the initial_scf or the specified calculation
+            # First one uses the initial_scf or the specified calculation.
             if "start_calc_folder" in self.inputs:
                 prev_calc_folder = self.inputs.start_calc_folder
             else:
                 prev_calc_folder = self.ctx.init_scf.outputs.remote_folder
             if self.inputs.start_uno:
                 uno = True
         elif self.ctx.i_current_mult == 1:
-            # for the "base" multiplicity, use the natural orbitals of the previous casscf
+            # For the "base" multiplicity, use the natural orbitals of the previous casscf.
             prev_nm = list(self.inputs.nm_list)[self.ctx.i_current_nm - 2]
             prev_label = f"cas_{prev_nm[0]}_{prev_nm[1]}_m{self.ctx.current_mult}"
             prev_calc_folder = self.ctx[prev_label].outputs.remote_folder
         else:
-            # for any other multiplicity, use the orbitals of the corresponding base casscf
+            # For any other multiplicity, use the orbitals of the corresponding base casscf.
             prev_label = "cas_{}_{}_m{}".format(
                 self.ctx.current_nm[0],
                 self.ctx.current_nm[1],
                 self.inputs.multiplicity_list[0],
             )
             prev_calc_folder = self.ctx[prev_label].outputs.remote_folder
 
         builder = GaussianCasscfWorkChain.get_builder()
-
         builder.parent_calc_folder = prev_calc_folder
-
         builder.gaussian_code = self.inputs.gaussian_code
-
-        builder.n = Int(self.ctx.current_nm[0])
-        builder.m = Int(self.ctx.current_nm[1])
-
+        builder.n = orm.Int(self.ctx.current_nm[0])
+        builder.m = orm.Int(self.ctx.current_nm[1])
         builder.basis_set = self.inputs.basis_set
-
-        builder.multiplicity = Int(self.ctx.current_mult)
-
-        builder.uno = Bool(uno)
+        builder.multiplicity = orm.Int(self.ctx.current_mult)
+        builder.uno = orm.Bool(uno)
         builder.mp2 = self.inputs.mp2
 
         codes_set = "formchk_code" in self.inputs and "cubegen_code" in self.inputs
         if self.inputs.num_orbital_cubes > 0 and codes_set:
             builder.num_orbital_cubes = self.inputs.num_orbital_cubes
             builder.formchk_code = self.inputs.formchk_code
             builder.cubegen_code = self.inputs.cubegen_code
 
         builder.options = self.inputs.options
 
-        label = "cas_{}_{}_m{}".format(
-            self.ctx.current_nm[0], self.ctx.current_nm[1], self.ctx.current_mult
-        )
-
+        label = f"cas_{self.ctx.current_nm[0]}_{self.ctx.current_nm[1]}_m{self.ctx.current_mult}"
         submitted_node = self.submit(builder)
-
         self.ctx.last_submitted_label = label
-        return ToContext(**{label: submitted_node})
+        return engine.ToContext(**{label: submitted_node})
 
     def finalize(self):
-
         self.report("Finalizing...")
 
         if not common_utils.check_if_calc_ok(
             self, self.ctx[self.ctx.last_submitted_label]
         ):
             return self.exit_codes.ERROR_TERMINATION
 
@@ -286,8 +264,8 @@
                 self.out(f"{var}_out_params", self.ctx[var].outputs.output_parameters)
                 if "cube_image_folder" in self.ctx[var].outputs:
                     self.out(
                         f"{var}_cube_image_folder",
                         self.ctx[var].outputs.cube_image_folder,
                     )
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,87 @@
-from aiida.engine import ExitCode, ToContext, WorkChain, if_
-from aiida.engine.processes.functions import calcfunction
-from aiida.orm import Bool, Code, Dict, Int, List, RemoteData, Str
-from aiida.plugins import WorkflowFactory
+from aiida import engine, orm, plugins
 
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.gaussian import common
+from ...utils import common_utils
+from . import common
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
-GaussianCubesWorkChain = WorkflowFactory("gaussian.cubes")
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
+GaussianCubesWorkChain = plugins.WorkflowFactory("gaussian.cubes")
 
 
-@calcfunction
+@engine.calcfunction
 def add_mp2_to_out_params(out_params, mp2_energy):
     new_params = dict(out_params)
     new_params["casmp2_energy_ev"] = mp2_energy.value
-    return Dict(new_params)
+    return orm.Dict(new_params)
 
 
-class GaussianCasscfWorkChain(WorkChain):
+class GaussianCasscfWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
             "parent_calc_folder",
-            valid_type=RemoteData,
+            valid_type=orm.RemoteData,
             required=True,
             help="parent Gaussian calculation directory",
         )
 
         spec.input(
-            "n", valid_type=Int, required=True, help="Number of electrons CAS(n,m)."
+            "n", valid_type=orm.Int, required=True, help="Number of electrons CAS(n,m)."
         )
-
         spec.input(
-            "m", valid_type=Int, required=True, help="Number of orbitals CAS(n,m)."
+            "m", valid_type=orm.Int, required=True, help="Number of orbitals CAS(n,m)."
         )
-
-        spec.input("basis_set", valid_type=Str, required=True, help="basis_set")
-
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="basis_set")
         spec.input(
             "multiplicity",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(1),
+            default=lambda: orm.Int(1),
             help="spin multiplicity",
         )
-
         spec.input(
             "uno",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="Use the natural orbitals from the previous calculation.",
         )
-
         spec.input(
             "mp2",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="calculate the MP2 correction (CASMP2).",
         )
-
         spec.input(
             "num_orbital_cubes",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="Generate cubes for orbitals (n*occ and n*virt).",
         )
-
-        spec.input("formchk_code", valid_type=Code, required=False)
-        spec.input("cubegen_code", valid_type=Code, required=False)
+        spec.input("formchk_code", valid_type=orm.Code, required=False)
+        spec.input("cubegen_code", valid_type=orm.Code, required=False)
 
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
         spec.outline(
             cls.setup,
             cls.casscf,
-            if_(cls.should_do_mp2)(cls.casmp2),
-            if_(cls.should_do_cubes)(cls.cubes),
+            engine.if_(cls.should_do_mp2)(cls.casmp2),
+            engine.if_(cls.should_do_cubes)(cls.cubes),
             cls.finalize,
         )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
             302,
@@ -137,25 +127,24 @@
         self.ctx.link0 = {
             "%chk": "aiida.chk",
             "%mem": "%dMB" % memory_mb,
             "%nprocshared": str(num_cores),
             "%oldchk": "parent_calc/aiida.chk",
         }
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
 
     def casscf(self):
-
         self.report("Submitting CASSCF")
 
         func_str = "CASSCF({},{}{})".format(
             self.inputs.n.value, self.inputs.m.value, ",UNO" if self.inputs.uno else ""
         )
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
                 "dieze_tag": "#P",
                 "functional": func_str,
                 "basis_set": self.inputs.basis_set.value,
                 "charge": 0,
                 "multiplicity": self.inputs.multiplicity.value,
@@ -177,26 +166,25 @@
         builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
         builder.gaussian.metadata.options = self.ctx.metadata_options
         builder.gaussian.metadata.options[
             "parser_name"
         ] = "nanotech_empa.gaussian.casscf"
 
         future = self.submit(builder)
-        return ToContext(casscf=future)
+        return engine.ToContext(casscf=future)
 
     def casmp2(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.casscf):
             return self.exit_codes.ERROR_TERMINATION
 
         self.report("Submitting CASMP2")
 
         func_str = f"CASSCF({self.inputs.n.value},{self.inputs.m.value})"
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
                 "dieze_tag": "#P",
                 "functional": func_str,
                 "basis_set": self.inputs.basis_set.value,
                 "charge": 0,
                 "multiplicity": self.inputs.multiplicity.value,
@@ -218,38 +206,35 @@
         builder.gaussian.parent_calc_folder = self.ctx.casscf.outputs.remote_folder
         builder.gaussian.metadata.options = self.ctx.metadata_options
         builder.gaussian.metadata.options[
             "parser_name"
         ] = "nanotech_empa.gaussian.casscf"
 
         future = self.submit(builder)
-        return ToContext(casmp2=future)
+        return engine.ToContext(casmp2=future)
 
     def cubes(self):
-
         n_d = self.inputs.num_orbital_cubes.value
         n_u = self.inputs.num_orbital_cubes.value
 
         builder = GaussianCubesWorkChain.get_builder()
         builder.formchk_code = self.inputs.formchk_code
         builder.cubegen_code = self.inputs.cubegen_code
         builder.gaussian_calc_folder = self.ctx.casscf.outputs.remote_folder
         builder.gaussian_output_params = self.ctx.casscf.outputs.output_parameters
-        builder.orbital_indexes = List(list(range(-n_d + 1, n_u + 1)))
-        builder.natural_orbitals = Bool(True)
-
+        builder.orbital_indexes = orm.List(list(range(-n_d + 1, n_u + 1)))
+        builder.natural_orbitals = orm.Bool(True)
         builder.cubegen_parser_name = "nanotech_empa.gaussian.cubegen_pymol"
-        builder.cubegen_parser_params = Dict(
+        builder.cubegen_parser_params = orm.Dict(
             {"isovalues": [0.050], "orient_cube": True}
         )
         future = self.submit(builder)
-        return ToContext(cubes=future)
+        return engine.ToContext(cubes=future)
 
     def finalize(self):
-
         self.report("Finalizing...")
 
         if not common_utils.check_if_calc_ok(self, self.ctx.casscf):
             return self.exit_codes.ERROR_TERMINATION
 
         out_params = self.ctx.casscf.outputs.output_parameters
 
@@ -264,11 +249,10 @@
         if self.should_do_cubes():
             if not common_utils.check_if_calc_ok(self, self.ctx.cubes):
                 return self.exit_codes.ERROR_TERMINATION
             self.out("cube_image_folder", self.ctx.cubes.outputs.cube_image_folder)
 
         self.out("output_parameters", out_params)
         self.out("casscf_energy_ev", self.ctx.casscf.outputs.casscf_energy_ev)
-
         self.out("remote_folder", self.ctx.casscf.outputs.remote_folder)
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/common.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,15 @@
 
 def _get_gaussian_mem_mb(total_mem_kb, computer):
     if computer.scheduler_type == "direct":
         return total_mem_kb // 1024 - 1536
     return (total_mem_kb // 1024 - 100) // 1.25
 
 
-# -------------------------------------------------------------------------------------
-
-
 def setup_context_variables(self_):
-
     pymatgen_structure = self_.inputs.structure.get_pymatgen_molecule()
     self_.ctx.n_atoms = pymatgen_structure.num_sites
     self_.ctx.n_electrons = pymatgen_structure.nelectrons
 
     if self_.inputs.multiplicity.value == 0:
         # RKS calculation
         self_.ctx.functional = self_.inputs.functional.value
@@ -43,45 +39,44 @@
         self_.ctx.functional = "u" + self_.inputs.functional.value
         self_.ctx.mult = self_.inputs.multiplicity.value
 
     self_.ctx.comp = self_.inputs.gaussian_code.computer
 
 
 def determine_comp_resources(num_atoms, basis_set=""):
-
-    # Very small basis sets:
+    # Very small basis sets.
     if basis_set.lower() in ("sto-3g", "sv", "svp", "def2sv", "def2svp"):
         num_cores = int(np.round(num_atoms / 20))
         mem_per_core = 512
-    # Large basis sets:
+
+    # Large basis sets.
     elif basis_set.lower() in ("6-311g*", "6-311g**", "6-311+g*", "6-311+g**"):
         num_cores = int(np.round(num_atoms / 16))
         mem_per_core = 4096
-    # Default:
+
+    # Default.
     else:
         num_cores = int(np.round(num_atoms / 18))
         mem_per_core = 2048
 
     num_cores = max(1, num_cores)
     num_cores = min(24, num_cores)
 
     memory_mb = num_cores * mem_per_core
 
     return num_cores, memory_mb
 
 
 def get_default_metadata_options(num_atoms, computer, basis_set):
-
     num_cores, memory_mb = determine_comp_resources(num_atoms, basis_set)
 
-    options = {}
-
-    options["max_memory_kb"] = _get_total_mem_kb(memory_mb, computer)
-
-    options["max_wallclock_seconds"] = 24 * 60 * 60
+    options = {
+        "max_memory_kb": _get_total_mem_kb(memory_mb, computer),
+        "max_wallclock_seconds": 24 * 60 * 60,
+    }
 
     if "lsf" in computer.scheduler_type:
         # LSF scheduler has some peculiarities:
         # 'num_machines' can not be set
         # tot_num_mpiprocs determines the number of cores
         options["resources"] = {
             "tot_num_mpiprocs": num_cores,
@@ -93,15 +88,14 @@
             "num_cores_per_machine": num_cores,
         }
 
     return options
 
 
 def validate_metadata_options(options, computer):
-
     if "resources" not in options:
         return "'resources' needs to be set"
 
     res = options["resources"]
 
     if get_total_number_of_cores(res, computer) is None:
         return "num_cores can not be determined from the inputted resources"
@@ -137,22 +131,21 @@
         elif "basis_set" in self_.inputs:
             bset = self_.inputs.basis_set.value
 
         self_.ctx.metadata_options = get_default_metadata_options(
             self_.ctx.n_atoms, self_.ctx.comp, bset
         )
 
-    # Always use the gaussian_advanced_parser
+    # Always use the gaussian_advanced_parser.
     self_.ctx.metadata_options["parser_name"] = "gaussian.advanced"
 
     return True
 
 
 def get_total_number_of_cores(resources, computer):
-
     num_machines = 1
     if "num_machines" in resources:
         num_machines = resources["num_machines"]
 
     if "num_cores_per_machine" in resources:
         return num_machines * resources["num_cores_per_machine"]
 
@@ -169,17 +162,14 @@
     if "num_cores_per_mpiproc" in resources:
         return tot_num_mpiprocs * resources["num_cores_per_mpiproc"]
 
     return tot_num_mpiprocs
 
 
 def get_gaussian_cores_and_memory(options, computer):
-
     num_cores = get_total_number_of_cores(options["resources"], computer)
-
     if "max_memory_kb" not in options:
         # If no memory is specified for the scheduler, set 2GB memory to Gaussian
         memory_mb = 2048
     else:
         memory_mb = _get_gaussian_mem_mb(options["max_memory_kb"], computer)
-
     return num_cores, memory_mb
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,93 @@
-from aiida.engine import ExitCode, ToContext, WorkChain, while_
-from aiida.orm import Bool, Code, Dict, Int, List, Str, StructureData
-
-from aiida_nanotech_empa.utils import common_utils
+from aiida import engine, orm
 
+from ...utils import common_utils
 from .relax_workchain import GaussianRelaxWorkChain
 from .scf_workchain import GaussianScfWorkChain
 
 
-class GaussianConstrOptChainWorkChain(WorkChain):
+class GaussianConstrOptChainWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
-            "structure", valid_type=StructureData, required=True, help="input geometry"
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
         )
 
-        spec.input("functional", valid_type=Str, required=True, help="xc functional")
+        spec.input(
+            "functional", valid_type=orm.Str, required=True, help="xc functional"
+        )
 
-        spec.input("basis_set", valid_type=Str, required=True, help="basis_set")
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="basis_set")
 
         spec.input(
-            "basis_set_scf", valid_type=Str, required=False, help="basis_set for SCF"
+            "basis_set_scf",
+            valid_type=orm.Str,
+            required=False,
+            help="basis_set for SCF",
         )
 
         spec.input(
             "multiplicity",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="spin multiplicity; 0 means RKS",
         )
 
         spec.input(
             "extra_scf_mults",
-            valid_type=List,
+            valid_type=orm.List,
             required=False,
-            default=lambda: List(list=[]),
+            default=lambda: orm.List(list=[]),
             help="Extra multiplicites for the SCF",
         )
 
         spec.input(
             "tight",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="Use tight optimization criteria.",
         )
 
         spec.input(
             "empirical_dispersion",
-            valid_type=Str,
+            valid_type=orm.Str,
             required=False,
-            default=lambda: Str(""),
+            default=lambda: orm.Str(""),
             help=("Include empirical dispersion corrections" '(e.g. "GD3", "GD3BJ")'),
         )
 
         spec.input(
             "list_of_constraints",
-            valid_type=List,
+            valid_type=orm.List,
             required=False,
-            default=lambda: List(list=[]),
+            default=lambda: orm.List(list=[]),
             help='Supported constraints: ("distance", n1, n2, d)',
         )
 
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
         spec.outline(
             cls.setup,
-            while_(cls.any_constraint_left)(cls.submit_opt, cls.submit_extra_mults),
+            engine.while_(cls.any_constraint_left)(
+                cls.submit_opt, cls.submit_extra_mults
+            ),
             cls.finalize,
         )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
             390,
@@ -95,15 +103,14 @@
     def setup(self):
         self.ctx.i_constr = 0
 
     def any_constraint_left(self):
         return len(self.inputs.list_of_constraints) > self.ctx.i_constr
 
     def submit_opt(self):
-
         label = f"opt_{self.ctx.i_constr}"
         if self.ctx.i_constr == 0:
             structure = self.inputs.structure
         else:
             prev_label = f"opt_{self.ctx.i_constr-1}"
 
             for extra_mult in self.inputs.extra_scf_mults:
@@ -125,65 +132,61 @@
         builder.functional = self.inputs.functional
         builder.basis_set = self.inputs.basis_set
 
         if "basis_set_scf" in self.inputs:
             builder.basis_set_scf = self.inputs.basis_set_scf
 
         builder.multiplicity = self.inputs.multiplicity
-        builder.wfn_stable_opt = Bool(self.is_uks())
+        builder.wfn_stable_opt = orm.Bool(self.is_uks())
 
         builder.empirical_dispersion = self.inputs.empirical_dispersion
 
         builder.tight = self.inputs.tight
 
-        builder.constraints = List(cur_constr)
+        builder.constraints = orm.List(cur_constr)
 
         if "options" in self.inputs:
             builder.options = self.inputs.options
 
         submitted_node = self.submit(builder)
         submitted_node.description = label
-        return ToContext(**{label: submitted_node})
+        return engine.ToContext(**{label: submitted_node})
 
     def submit_extra_mults(self):
-
         opt_label = f"opt_{self.ctx.i_constr-1}"
 
         if not common_utils.check_if_calc_ok(self, self.ctx[opt_label]):
             return self.exit_codes.ERROR_TERMINATION
 
         for extra_mult in self.inputs.extra_scf_mults:
-
             label = opt_label + f"_m{extra_mult}"
             self.report(f"Submitting scf {label}")
 
             builder = GaussianScfWorkChain.get_builder()
             builder.gaussian_code = self.inputs.gaussian_code
             builder.structure = self.ctx[opt_label].outputs.output_structure
             builder.functional = self.inputs.functional
             builder.empirical_dispersion = self.inputs.empirical_dispersion
             builder.basis_set = self.inputs.basis_set_scf
-            builder.multiplicity = Int(extra_mult)
-            builder.wfn_stable_opt = Bool(True)
+            builder.multiplicity = orm.Int(extra_mult)
+            builder.wfn_stable_opt = orm.Bool(True)
 
             if "options" in self.inputs:
                 builder.options = self.inputs.options
 
             submitted_node = self.submit(builder)
             submitted_node.description = label
             self.to_context(**{label: submitted_node})
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
 
     def finalize(self):
-
         self.report("Finalizing...")
 
         for i_constr in range(len(self.inputs.list_of_constraints)):
-
             label = f"opt_{i_constr}"
             if not common_utils.check_if_calc_ok(self, self.ctx[label]):
                 return self.exit_codes.ERROR_TERMINATION
 
             self.out(
                 f"opt_{i_constr}_structure", self.ctx[label].outputs.output_structure
             )
@@ -199,8 +202,8 @@
             for extra_mult in self.inputs.extra_scf_mults:
                 extra_label = label + f"_m{extra_mult}"
                 self.out(
                     f"{extra_label}_scf_out_params",
                     self.ctx[extra_label].outputs.output_parameters,
                 )
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,128 @@
-from aiida.engine import ExitCode, WorkChain, calcfunction
-from aiida.orm import Code, Dict, Int, RemoteData, Str, StructureData
-from aiida.plugins import WorkflowFactory
+from aiida import engine, orm, plugins
 
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.gaussian import common
+from ...utils import common_utils
+from . import common
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
+GaussianCubesWorkChain = plugins.WorkflowFactory("gaussian.cubes")
 
 
-@calcfunction
-def subtract(a, b):
-    return a - b
-
-
-class GaussianDeltaScfWorkChain(WorkChain):
+class GaussianScfWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
-
+        spec.input("gaussian_code", valid_type=orm.Code)
+        spec.input(
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
+        )
+        spec.input(
+            "functional", valid_type=orm.Str, required=True, help="xc functional"
+        )
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="basis_set")
+        spec.input(
+            "multiplicity",
+            valid_type=orm.Int,
+            required=False,
+            default=lambda: orm.Int(1),
+            help="Spin multiplicity; 0 means RKS",
+        )
         spec.input(
-            "structure", valid_type=StructureData, required=True, help="input geometry"
+            "wfn_stable_opt",
+            valid_type=orm.Bool,
+            required=False,
+            default=lambda: orm.Bool(False),
+            help="If true, perform wfn stability optimization.",
         )
-        spec.input("functional", valid_type=Str, required=True, help="xc functional")
 
-        spec.input("basis_set", valid_type=Str, required=True, help="basis_set")
+        spec.input(
+            "wfn_stable_opt_min_basis",
+            valid_type=orm.Bool,
+            required=False,
+            default=lambda: orm.Bool(False),
+            help="If true, perform first a minimal basis stability opt.",
+        )
 
         spec.input(
-            "multiplicity",
-            valid_type=Int,
+            "empirical_dispersion",
+            valid_type=orm.Str,
             required=False,
-            default=lambda: Int(1),
-            help="spin multiplicity; 0 means RKS",
+            default=lambda: orm.Str(""),
+            help=("Include empirical dispersion corrections" '(e.g. "GD3", "GD3BJ")'),
         )
 
         spec.input(
             "parent_calc_folder",
-            valid_type=RemoteData,
+            valid_type=orm.RemoteData,
             required=False,
             help="the folder of a completed gaussian calculation",
         )
 
+        # Inputs for cubes generation.
+        spec.input("formchk_code", valid_type=orm.Code, required=False)
+        spec.input("cubegen_code", valid_type=orm.Code, required=False)
+
+        spec.input(
+            "cubes_n_occ",
+            valid_type=orm.Int,
+            required=False,
+            default=lambda: orm.Int(0),
+            help="Number of occupied orbital cubes to generate",
+        )
+
+        spec.input(
+            "cubes_n_virt",
+            valid_type=orm.Int,
+            required=False,
+            default=lambda: orm.Int(0),
+            help="Number of virtual orbital cubes to generate",
+        )
+
+        spec.input(
+            "cubes_edge_space",
+            valid_type=orm.Float,
+            required=False,
+            default=lambda: orm.Float(3.0),
+            help="Extra cube space in addition to bounding box [ang].",
+        )
+
+        spec.input(
+            "cubegen_parser_name",
+            valid_type=str,
+            default="nanotech_empa.gaussian.cubegen_pymol",
+            non_db=True,
+        )
+
+        spec.input(
+            "cubegen_parser_params",
+            valid_type=orm.Dict,
+            required=False,
+            default=lambda: orm.Dict(dict={}),
+            help="Additional parameters to cubegen parser.",
+        )
+
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
-        spec.outline(cls.setup, cls.submit_scfs, cls.finalize)
+        spec.outline(
+            cls.setup,
+            engine.if_(cls.should_do_min_basis_stable_opt)(cls.min_basis_stable_opt),
+            cls.scf,
+            engine.if_(cls.did_scf_fail)(cls.scf),
+            engine.if_(cls.should_do_cubes)(cls.cubes),
+            cls.finalize,
+        )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
             301,
             "ERROR_MULTIPLICITY",
             message="Multiplicity and number of el. doesn't match.",
@@ -71,15 +140,15 @@
 
     def is_uks(self):
         if self.inputs.multiplicity.value == 0:
             return False
         return True
 
     def setup(self):
-        self.report("Inspecting input and setting up things.")
+        self.report("Inspecting input and setting up things")
 
         common.setup_context_variables(self)
 
         if self.ctx.mult % 2 == self.ctx.n_electrons % 2:
             return self.exit_codes.ERROR_MULTIPLICITY
 
         success = common.determine_metadata_options(self)
@@ -92,36 +161,38 @@
 
         self.ctx.link0 = {
             "%chk": "aiida.chk",
             "%mem": "%dMB" % memory_mb,
             "%nprocshared": str(num_cores),
         }
 
-        return ExitCode(0)
+        # Use default convergence criterion at the start
+        # but switch to conver=7 in case of failure.
+        self.ctx.conver = None
+        self.ctx.scf_label = "scf"
 
-    def setup_common_builder_params(self, builder):
-        builder.gaussian.structure = self.inputs.structure
-        builder.gaussian.code = self.inputs.gaussian_code
-        builder.gaussian.metadata.options = self.ctx.metadata_options
+        return engine.ExitCode(0)
+
+    def should_do_min_basis_stable_opt(self):
+        return self.inputs.wfn_stable_opt_min_basis
 
-    def submit_scfs(self):
-        # --------------------------------------------------
-        self.report("Submitting NEUTRAL SCF")
-        # --------------------------------------------------
+    def min_basis_stable_opt(self):
+        self.report("Submitting minimal basis stable opt")
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
+                "dieze_tag": "#P",
                 "functional": self.ctx.functional,
-                "basis_set": self.inputs.basis_set.value,
+                "basis_set": "STO-3G",
                 "charge": 0,
                 "multiplicity": self.ctx.mult,
                 "route_parameters": {
-                    "scf": {"conver": 7, "maxcycle": 140},
-                    "sp": None,
+                    "scf": {"maxcycle": 140},
+                    "stable": "opt",
                 },
             }
         )
 
         builder = GaussianBaseWorkChain.get_builder()
 
         if "parent_calc_folder" in self.inputs:
@@ -130,124 +201,141 @@
             parameters["route_parameters"]["guess"] = "read"
             builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
         elif self.is_uks() and self.ctx.mult == 1:
             # For open-shell singlet, mix homo & lumo
             parameters["route_parameters"]["guess"] = "mix"
 
         builder.gaussian.parameters = parameters
-        self.setup_common_builder_params(builder)
-        submitted_node = self.submit(builder)
-        self.to_context(neutral=submitted_node)
-
-        # --------------------------------------------------
-        self.report("Submitting CATION SCF")
-        # --------------------------------------------------
+        builder.gaussian.structure = self.inputs.structure
+        builder.gaussian.code = self.inputs.gaussian_code
+        builder.gaussian.metadata.options = self.ctx.metadata_options
 
-        if self.ctx.mult == 1:
-            pos_mult = 2
-        else:
-            pos_mult = self.ctx.mult - 1
+        future = self.submit(builder)
+        return engine.ToContext(min_stable=future)
 
-        if self.is_uks():
-            functional = self.ctx.functional
-        else:
-            functional = "u" + self.ctx.functional
+    def scf(self):
+        self.report("Submitting SCF")
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
-                "functional": functional,
+                "dieze_tag": "#P",
+                "functional": self.ctx.functional,
                 "basis_set": self.inputs.basis_set.value,
-                "charge": 1,
-                "multiplicity": pos_mult,
+                "charge": 0,
+                "multiplicity": self.ctx.mult,
                 "route_parameters": {
-                    "scf": {"conver": 7, "maxcycle": 140},
-                    "sp": None,
+                    "scf": {"maxcycle": 140},
                 },
             }
         )
+        if self.inputs.wfn_stable_opt:
+            parameters["route_parameters"]["stable"] = "opt"
+        else:
+            parameters["route_parameters"]["sp"] = None
 
         builder = GaussianBaseWorkChain.get_builder()
 
-        if pos_mult == 1:
+        if self.should_do_min_basis_stable_opt():
+            # Read WFN from min basis stable opt
+            parameters["link0_parameters"]["%oldchk"] = "parent_calc/aiida.chk"
+            parameters["route_parameters"]["guess"] = "read"
+            builder.gaussian.parent_calc_folder = (
+                self.ctx.min_stable.outputs.remote_folder
+            )
+        elif "parent_calc_folder" in self.inputs:
+            # Read WFN from parent calc
+            parameters["link0_parameters"]["%oldchk"] = "parent_calc/aiida.chk"
+            parameters["route_parameters"]["guess"] = "read"
+            builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
+        elif self.is_uks() and self.ctx.mult == 1:
             # For open-shell singlet, mix homo & lumo
             parameters["route_parameters"]["guess"] = "mix"
 
-        builder.gaussian.parameters = parameters
-        self.setup_common_builder_params(builder)
-        submitted_node = self.submit(builder)
-        self.to_context(pos=submitted_node)
-
-        # --------------------------------------------------
-        self.report("Submitting ANION SCF")
-        # --------------------------------------------------
-        # For the ANION, the added electron could go opposite or parallel
-        # if the system was already spin-polarized
+        if self.inputs.empirical_dispersion.value != "":
+            parameters["route_parameters"][
+                "empiricaldispersion"
+            ] = self.inputs.empirical_dispersion.value
 
-        if self.ctx.mult == 1:
-            self.ctx.neg_mults = [2]
-        else:
-            self.ctx.neg_mults = [self.ctx.mult - 1, self.ctx.mult + 1]
+        if self.ctx.conver is not None:
+            parameters["route_parameters"]["scf"]["conver"] = self.ctx.conver
 
-        for neg_mult in self.ctx.neg_mults:
-            parameters = Dict(
-                {
-                    "link0_parameters": self.ctx.link0.copy(),
-                    "functional": functional,
-                    "basis_set": self.inputs.basis_set.value,
-                    "charge": -1,
-                    "multiplicity": neg_mult,
-                    "route_parameters": {
-                        "scf": {"conver": 7, "maxcycle": 140},
-                        "sp": None,
-                    },
-                }
-            )
+        builder.gaussian.parameters = parameters
+        builder.gaussian.structure = self.inputs.structure
+        builder.gaussian.code = self.inputs.gaussian_code
+        builder.gaussian.metadata.options = self.ctx.metadata_options
 
-            builder = GaussianBaseWorkChain.get_builder()
+        future = self.submit(builder)
+        future.description = self.ctx.scf_label
+        return engine.ToContext(**{self.ctx.scf_label: future})
+
+    def did_scf_fail(self):
+        scf_node = self.ctx[self.ctx.scf_label]
+        if not common_utils.check_if_calc_ok(self, scf_node):
+            # Set up for conver=7 calculation.
+            self.report("SCF failed with default convergence criterion!")
+            self.report("Switching to a looser threshold.")
+            self.ctx.conver = 7
+            self.ctx.scf_label = f"scf_c{self.ctx.conver}"
+            return True
+        return False
+
+    def should_do_cubes(self):
+        codes_set = "formchk_code" in self.inputs and "cubegen_code" in self.inputs
+        non_zero_num = (
+            self.inputs.cubes_n_occ.value > 0 and self.inputs.cubes_n_virt.value > 0
+        )
+        return codes_set and non_zero_num
 
-            if neg_mult == 1:
-                # For open-shell singlet, mix homo & lumo
-                parameters["route_parameters"]["guess"] = "mix"
-
-            builder.gaussian.parameters = parameters
-            self.setup_common_builder_params(builder)
-            submitted_node = self.submit(builder)
-            label = f"neg_m{neg_mult}"
-            self.to_context(**{label: submitted_node})
+    def cubes(self):
+        scf_node = self.ctx[self.ctx.scf_label]
 
-    def finalize(self):
-
-        if not common_utils.check_if_calc_ok(
-            self, self.ctx.neutral
-        ) or not common_utils.check_if_calc_ok(self, self.ctx.pos):
+        if not common_utils.check_if_calc_ok(self, scf_node):
             return self.exit_codes.ERROR_TERMINATION
 
-        anion_energies = []
+        self.report("Generating cubes")
 
-        for neg_mult in self.ctx.neg_mults:
-            label = f"neg_m{neg_mult}"
-            if not common_utils.check_if_calc_ok(self, self.ctx[label]):
-                return self.exit_codes.ERROR_TERMINATION
+        orb_index_list = list(
+            range(
+                -self.inputs.cubes_n_occ.value + 1, self.inputs.cubes_n_virt.value + 1
+            )
+        )
 
-            anion_energies.append(self.ctx[label].outputs.energy_ev)
+        future = self.submit(
+            GaussianCubesWorkChain,
+            formchk_code=self.inputs.formchk_code,
+            cubegen_code=self.inputs.cubegen_code,
+            gaussian_calc_folder=scf_node.outputs.remote_folder,
+            gaussian_output_params=scf_node.outputs["output_parameters"],
+            orbital_indexes=orm.List(list=orb_index_list),
+            orbital_index_ref=orm.Str("half_num_el"),
+            edge_space=self.inputs.cubes_edge_space,
+            dx=orm.Float(0.15),
+            retrieve_cubes=orm.Bool(False),
+            cubegen_parser_name=self.inputs.cubegen_parser_name,
+            cubegen_parser_params=self.inputs.cubegen_parser_params,
+        )
+        return engine.ToContext(cubes=future)
 
-            if len(self.ctx.neg_mults) > 1:
-                self.out(f"anion_energy_m{neg_mult}", self.ctx[label].outputs.energy_ev)
+    def finalize(self):
+        scf_node = self.ctx[self.ctx.scf_label]
 
-        anion_energy = min(anion_energies)
+        if not common_utils.check_if_calc_ok(self, scf_node):
+            return self.exit_codes.ERROR_TERMINATION
 
-        self.out("neutral_energy", self.ctx.neutral.outputs.energy_ev)
-        self.out("cation_energy", self.ctx.pos.outputs.energy_ev)
-        self.out("anion_energy", anion_energy)
+        self.report("Finalizing...")
 
-        ip = subtract(
-            self.ctx.pos.outputs.energy_ev, self.ctx.neutral.outputs.energy_ev
-        )
-        ea = subtract(self.ctx.neutral.outputs.energy_ev, anion_energy)
+        if self.should_do_cubes():
+            if not common_utils.check_if_calc_ok(self, self.ctx.cubes):
+                return self.exit_codes.ERROR_TERMINATION
+            for cubes_out in list(self.ctx.cubes.outputs):
+                if cubes_out.startswith("cube"):
+                    self.out(cubes_out, self.ctx.cubes.outputs[cubes_out])
+                elif cubes_out == "retrieved":
+                    self.out("cubes_retrieved", self.ctx.cubes.outputs[cubes_out])
 
-        self.out("ionization_potential", ip)
-        self.out("electron_affinity", ea)
+        self.out("energy_ev", scf_node.outputs.energy_ev)
+        self.out("output_parameters", scf_node.outputs["output_parameters"])
 
-        self.out("fundamental_gap", subtract(ip, ea))
+        self.out("remote_folder", scf_node.outputs["remote_folder"])
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,77 @@
-from aiida.engine import ExitCode, ToContext, WorkChain
-from aiida.orm import Bool, Code, Dict, Float, Int, RemoteData, Str, StructureData
-from aiida.plugins import WorkflowFactory
-
-from aiida_nanotech_empa.utils import common_utils
+from aiida import engine, orm, plugins
 
+from ...utils import common_utils
 from .scf_workchain import GaussianScfWorkChain
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
-GaussianCubesWorkChain = WorkflowFactory("gaussian.cubes")
-
-# -------------------------------------------------------------
-# Work Chain to run HF and MP2
-# -------------------------------------------------------------
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
+GaussianCubesWorkChain = plugins.WorkflowFactory("gaussian.cubes")
 
 
-class GaussianHfMp2WorkChain(WorkChain):
+class GaussianHfMp2WorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
-            "structure", valid_type=StructureData, required=True, help="input geometry"
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
         )
 
-        spec.input("basis_set", valid_type=Str, required=True, help="basis_set")
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="basis_set")
 
         spec.input(
             "multiplicity",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(1),
+            default=lambda: orm.Int(1),
             help="spin multiplicity; 0 means RKS",
         )
 
         spec.input(
             "parent_calc_folder",
-            valid_type=RemoteData,
+            valid_type=orm.RemoteData,
             required=False,
             help="the folder of a completed gaussian calculation",
         )
 
-        # -------------------------------------------------------------------
         # CUBE GENERATION INPUTS
         spec.input(
             "num_orbital_cubes",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="Generate cubes for the mp2 orbitals (n*occ and n*virt).",
         )
 
-        spec.input("formchk_code", valid_type=Code, required=False)
-        spec.input("cubegen_code", valid_type=Code, required=False)
+        spec.input("formchk_code", valid_type=orm.Code, required=False)
+        spec.input("cubegen_code", valid_type=orm.Code, required=False)
 
         spec.input(
             "edge_space",
-            valid_type=Float,
+            valid_type=orm.Float,
             required=False,
-            default=lambda: Float(3.0),
+            default=lambda: orm.Float(3.0),
             help="Extra cube space in addition to molecule bounding box [ang].",
         )
         spec.input(
             "cubegen_parser_params",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
-            default=lambda: Dict(dict={}),
+            default=lambda: orm.Dict(dict={}),
             help="Additional parameters to cubegen parser.",
         )
-        # -------------------------------------------------------------------
 
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
         spec.outline(cls.hf, cls.mp2, cls.finalize)
 
         spec.outputs.dynamic = True
@@ -95,50 +89,48 @@
         spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
     def hf(self):
-
         self.report("Submitting HF")
 
         builder = GaussianScfWorkChain.get_builder()
         builder.gaussian_code = self.inputs.gaussian_code
 
         builder.structure = self.inputs.structure
-        builder.functional = Str("hf")
+        builder.functional = orm.Str("hf")
         builder.basis_set = self.inputs.basis_set
         builder.multiplicity = self.inputs.multiplicity
 
-        builder.wfn_stable_opt_min_basis = Bool(True)
+        builder.wfn_stable_opt_min_basis = orm.Bool(True)
 
         if "options" in self.inputs:
             builder.options = self.inputs.options
 
         future = self.submit(builder)
-        return ToContext(hf=future)
+        return engine.ToContext(hf=future)
 
     def should_do_cubes(self):
         codes_set = "formchk_code" in self.inputs and "cubegen_code" in self.inputs
         non_zero_num = self.inputs.num_orbital_cubes.value > 0
         return codes_set and non_zero_num
 
     def mp2(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.hf):
             return self.exit_codes.ERROR_TERMINATION
 
         self.report("Submitting MP2")
 
         builder = GaussianScfWorkChain.get_builder()
         builder.gaussian_code = self.inputs.gaussian_code
 
         builder.structure = self.inputs.structure
-        builder.functional = Str("mp2")
+        builder.functional = orm.Str("mp2")
         builder.basis_set = self.inputs.basis_set
         builder.multiplicity = self.inputs.multiplicity
 
         builder.parent_calc_folder = self.ctx.hf.outputs.remote_folder
 
         if self.should_do_cubes():
             builder.n_occ = self.inputs.num_orbital_cubes
@@ -148,25 +140,24 @@
             builder.edge_space = self.inputs.edge_space
             builder.cubegen_parser_params = self.inputs.cubegen_parser_params
 
         if "options" in self.inputs:
             builder.options = self.inputs.options
 
         future = self.submit(builder)
-        return ToContext(mp2=future)
+        return engine.ToContext(mp2=future)
 
     def finalize(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.mp2):
             return self.exit_codes.ERROR_TERMINATION
 
         self.report("Finalizing...")
 
         self.out("hf_output_parameters", self.ctx.hf.outputs.output_parameters)
         self.out("mp2_output_parameters", self.ctx.mp2.outputs.output_parameters)
 
         if self.should_do_cubes():
             self.out("mp2_cube_images", self.ctx.mp2.outputs.cube_image_folder)
 
         self.out("remote_folder", self.ctx.mp2.outputs.remote_folder)
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import numpy as np
-from aiida.engine import ExitCode, ToContext, WorkChain, calcfunction, if_
-from aiida.orm import Bool, Code, Dict, Float, Int, List, RemoteData
-from aiida.plugins import WorkflowFactory
+from aiida import engine, orm, plugins
 
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.gaussian import common
+from ...utils import common_utils
+from . import common
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
-GaussianCubesWorkChain = WorkflowFactory("gaussian.cubes")
-
-# Natural orbital processing:
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
+GaussianCubesWorkChain = plugins.WorkflowFactory("gaussian.cubes")
 
 
+# Natural orbital processing.
 def standard_num_odd(no_occs):
     n_odd = 0.0
     for n in no_occs:
         n_odd += 2 * n - n**2
     return n_odd
 
 
@@ -30,46 +27,48 @@
     n_odd = 0.0
     for n in no_occs:
         n_odd += n**2 * (2 - n) ** 2
     return n_odd
 
 
 def spin_proj_nakano(no_occs, i_hono=None):
-    # "perfect-pairing spin projection scheme"
-    #     Nakano 2011: (Hyper)polarizability density analysis...
-    # More recent citation, also reveals the connection to Yamaguchi's scheme:
-    #     Nakano 2015: Approximate spin projected spin-unrestricted...
-
-    # Equivalent to "Yamaguchi's scheme"
-    # Original citation:
-    #    Yamaguchi 1988: A spin correction procedure...
-    #    (No radical character BUT singlet-triplet energy gap correction)
-    # Recent citation:
-    #    Minami, Nakano 2012: Diradical Character View of Singlet Fission
-    #    (Radical and multiradical characters)
-    # An application paper:
-    #    Lu 2016: Stable 3,6-Linked Fluorenyl Radical Oligomers with...
-
+    """
+    "perfect-pairing spin projection scheme"
+        Nakano 2011: (Hyper)polarizability density analysis...
+    More recent citation, also reveals the connection to Yamaguchi's scheme:
+        Nakano 2015: Approximate spin projected spin-unrestricted...
+
+    Equivalent to "Yamaguchi's scheme"
+    Original citation:
+       Yamaguchi 1988: A spin correction procedure...
+       (No radical character BUT singlet-triplet energy gap correction)
+    Recent citation:
+       Minami, Nakano 2012: Diradical Character View of Singlet Fission
+       (Radical and multiradical characters)
+    An application paper:
+       Lu 2016: Stable 3,6-Linked Fluorenyl Radical Oligomers with...
+    """
     if i_hono is None:
         no_hono = no_occs[no_occs > 1.0]
         no_luno = no_occs[no_occs <= 1.0]
     else:
         no_hono = no_occs[: i_hono + 1]
         no_luno = no_occs[i_hono + 1 :]
 
     c = np.min([len(no_hono), len(no_luno)])
 
     no_hono = no_hono[::-1]
-    # overlap between pairs
+
+    # Overlap between pairs.
     s = (no_hono[:c] - no_luno[:c]) / 2
 
     no_hono_sp = no_hono[:c] ** 2 / (1 + s**2)
     no_luno_sp = no_luno[:c] ** 2 / (1 + s**2)
 
-    # pad the spin proj array to initial array shape
+    # Pad the spin proj array to initial array shape.
     no_hono_sp = np.pad(
         no_hono_sp,
         (0, len(no_hono) - len(no_hono_sp)),
         mode="constant",
         constant_values=2.0,
     )
     no_luno_sp = np.pad(
@@ -78,104 +77,102 @@
         mode="constant",
         constant_values=0.0,
     )
 
     return np.concatenate([no_hono_sp[::-1], no_luno_sp])
 
 
-@calcfunction
+@engine.calcfunction
 def process_natural_orb_occupations(natorb_parameters):
-
     no_occs = natorb_parameters["nooccnos"]
     i_homo = natorb_parameters["homos"][0]
     no_occs_sp = list(spin_proj_nakano(np.array(no_occs), i_hono=i_homo))
 
-    return Dict(
+    return orm.Dict(
         {
             "no_occs": no_occs,
             "no_occs_sp": no_occs_sp,
             "std_num_odd": standard_num_odd(no_occs),
             "std_num_odd_sp": standard_num_odd(no_occs_sp),
             "hg_num_odd": head_gordon_num_odd(no_occs),
             "hg_num_odd_sp": head_gordon_num_odd(no_occs_sp),
         }
     )
 
 
-class GaussianNatOrbWorkChain(WorkChain):
+class GaussianNatOrbWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
             "parent_calc_folder",
-            valid_type=RemoteData,
+            valid_type=orm.RemoteData,
             required=True,
             help="parent Gaussian calculation directory",
         )
 
         spec.input(
             "parent_calc_params",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=True,
             help="parent Gaussian calculation output parameters",
         )
 
         spec.input(
             "save_natorb_chk",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help=(
                 "Save natural orbitals in the chk file."
                 + "Can introduce errors for larger systems"
             ),
         )
 
-        # -------------------------------------------------------------------
-        # CUBE GENERATION INPUTS
+        # Cube inputs generation.
         spec.input(
             "num_natural_orbital_cubes",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="Generate cubes for SAVED natural orbitals (n*occ and n*virt).",
         )
-        spec.input("formchk_code", valid_type=Code, required=False)
-        spec.input("cubegen_code", valid_type=Code, required=False)
+        spec.input("formchk_code", valid_type=orm.Code, required=False)
+        spec.input("cubegen_code", valid_type=orm.Code, required=False)
 
         spec.input(
             "edge_space",
-            valid_type=Float,
+            valid_type=orm.Float,
             required=False,
-            default=lambda: Float(3.0),
+            default=lambda: orm.Float(3.0),
             help="Extra cube space in addition to molecule bounding box [ang].",
         )
         spec.input(
             "cubegen_parser_params",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
-            default=lambda: Dict(dict={}),
+            default=lambda: orm.Dict(dict={}),
             help="Additional parameters to cubegen parser.",
         )
         # -------------------------------------------------------------------
 
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
         spec.outline(
             cls.submit_calc,
-            if_(cls.save_natorb_chk)(
-                cls.submit_save, if_(cls.should_do_cubes)(cls.cubes)
+            engine.if_(cls.save_natorb_chk)(
+                cls.submit_save, engine.if_(cls.should_do_cubes)(cls.cubes)
             ),
             cls.finalize,
         )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
@@ -186,15 +183,14 @@
         spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
     def submit_calc(self):
-
         self.ctx.n_atoms = self.inputs.parent_calc_params["natom"]
         self.ctx.basis_set = self.inputs.parent_calc_params["metadata"]["basis_set"]
         self.ctx.comp = self.inputs.gaussian_code.computer
 
         success = common.determine_metadata_options(self)
         if not success:
             return self.exit_codes.ERROR_OPTIONS
@@ -228,33 +224,31 @@
             },
             "functional": "",  # ignored
             "basis_set": "",  # ignored
             "charge": -1,  # ignored
             "multiplicity": -1,  # ignored
         }
 
-        builder.gaussian.parameters = Dict(parameters)
+        builder.gaussian.parameters = orm.Dict(parameters)
 
         builder.gaussian.metadata.options = self.ctx.metadata_options
 
         submitted_node = self.submit(builder)
         submitted_node.description = "naturalorbitals population"
-        return ToContext(natorb=submitted_node)
+        return engine.ToContext(natorb=submitted_node)
 
     def save_natorb_chk(self):
         return self.inputs.save_natorb_chk
 
     def submit_save(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.natorb):
             return self.exit_codes.ERROR_TERMINATION
 
         builder = GaussianBaseWorkChain.get_builder()
         builder.gaussian.code = self.inputs.gaussian_code
-        # builder.gaussian.parent_calc_folder = self.ctx.natorb.outputs.remote_folder
         builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
 
         parameters = {
             "link0_parameters": {
                 "%chk": "aiida.chk",
                 "%oldchk": "parent_calc/aiida.chk",
                 "%mem": "%dMB" % self.ctx.memory_mb,
@@ -271,52 +265,49 @@
             },
             "functional": "",  # ignored
             "basis_set": "",  # ignored
             "charge": -1,  # ignored
             "multiplicity": -1,  # ignored
         }
 
-        builder.gaussian.parameters = Dict(parameters)
-
+        builder.gaussian.parameters = orm.Dict(parameters)
         builder.gaussian.metadata.options = self.ctx.metadata_options
 
         submitted_node = self.submit(builder)
         submitted_node.description = "naturalorbitals save"
-        return ToContext(natorb_save=submitted_node)
+        return engine.ToContext(natorb_save=submitted_node)
 
     def should_do_cubes(self):
         codes_set = "formchk_code" in self.inputs and "cubegen_code" in self.inputs
         pos_num_specified = self.inputs.num_natural_orbital_cubes.value > 0
         return self.save_natorb_chk() and codes_set and pos_num_specified
 
     def cubes(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.natorb_save):
             return self.exit_codes.ERROR_TERMINATION
 
         n_d = self.inputs.num_natural_orbital_cubes.value
         n_u = self.inputs.num_natural_orbital_cubes.value
 
         builder = GaussianCubesWorkChain.get_builder()
         builder.formchk_code = self.inputs.formchk_code
         builder.cubegen_code = self.inputs.cubegen_code
         builder.gaussian_calc_folder = self.ctx.natorb_save.outputs.remote_folder
         builder.gaussian_output_params = self.ctx.natorb.outputs.output_parameters
-        builder.orbital_indexes = List(list(range(-n_d + 1, n_u + 1)))
-        builder.natural_orbitals = Bool(True)
+        builder.orbital_indexes = orm.List(list(range(-n_d + 1, n_u + 1)))
+        builder.natural_orbitals = orm.Bool(True)
         builder.edge_space = self.inputs.edge_space
-        builder.dx = Float(0.15)
+        builder.dx = orm.Float(0.15)
         builder.cubegen_parser_name = "nanotech_empa.gaussian.cubegen_pymol"
         builder.cubegen_parser_params = self.inputs.cubegen_parser_params
 
         future = self.submit(builder)
-        return ToContext(cubes=future)
+        return engine.ToContext(cubes=future)
 
     def finalize(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.natorb):
             return self.exit_codes.ERROR_TERMINATION
 
         if self.save_natorb_chk():
             if not common_utils.check_if_calc_ok(self, self.ctx.natorb_save):
                 return self.exit_codes.ERROR_TERMINATION
             self.out("remote_folder", self.ctx.natorb_save.outputs.remote_folder)
@@ -332,8 +323,8 @@
 
         self.out("natorb_raw_parameters", self.ctx.natorb.outputs.output_parameters)
         self.out(
             "natorb_proc_parameters",
             process_natural_orb_occupations(self.ctx.natorb.outputs.output_parameters),
         )
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,143 +1,145 @@
-from aiida.engine import ExitCode, ToContext, WorkChain, if_
-from aiida.orm import Bool, Code, Dict, Float, Int, List, Str, StructureData
-from aiida.plugins import WorkflowFactory
-
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.gaussian import common
+from aiida import engine, orm, plugins
 
+from ...utils import common_utils
+from . import common
 from .scf_workchain import GaussianScfWorkChain
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
 
 
-class GaussianRelaxWorkChain(WorkChain):
+class GaussianRelaxWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
 
         spec.input(
-            "structure", valid_type=StructureData, required=True, help="input geometry"
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
+        )
+        spec.input(
+            "functional", valid_type=orm.Str, required=True, help="xc functional"
         )
-        spec.input("functional", valid_type=Str, required=True, help="xc functional")
 
-        spec.input("basis_set", valid_type=Str, required=True, help="basis_set")
+        spec.input("basis_set", valid_type=orm.Str, required=True, help="basis_set")
 
         spec.input(
             "multiplicity",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="spin multiplicity; 0 means RKS",
         )
 
         spec.input(
             "wfn_stable_opt",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="if true, perform wfn stability optimization",
         )
 
         spec.input(
             "tight",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="Use tight optimization criteria.",
         )
 
         spec.input(
             "freq",
-            valid_type=Bool,
+            valid_type=orm.Bool,
             required=False,
-            default=lambda: Bool(False),
+            default=lambda: orm.Bool(False),
             help="Also run vibrational analysis.",
         )
 
         spec.input(
             "empirical_dispersion",
-            valid_type=Str,
+            valid_type=orm.Str,
             required=False,
-            default=lambda: Str(""),
+            default=lambda: orm.Str(""),
             help=("Include empirical dispersion corrections" '(e.g. "GD3", "GD3BJ")'),
         )
 
         spec.input(
             "constraints",
-            valid_type=List,
+            valid_type=orm.List,
             required=False,
-            default=lambda: List(list=[]),
+            default=lambda: orm.List(list=[]),
             help='Supported constraints: ("distance", n1, n2, d)',
         )
 
         # Do an extra SCF step at the end and potentially create cubes.
         spec.input(
             "basis_set_scf",
-            valid_type=Str,
+            valid_type=orm.Str,
             required=False,
             help="Basis set for SCF. If not present, SCF is skipped.",
         )
 
-        spec.input("formchk_code", valid_type=Code, required=False)
-        spec.input("cubegen_code", valid_type=Code, required=False)
+        spec.input("formchk_code", valid_type=orm.Code, required=False)
+        spec.input("cubegen_code", valid_type=orm.Code, required=False)
 
         spec.input(
             "cubes_n_occ",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="Number of occupied orbital cubes to generate",
         )
 
         spec.input(
             "cubes_n_virt",
-            valid_type=Int,
+            valid_type=orm.Int,
             required=False,
-            default=lambda: Int(0),
+            default=lambda: orm.Int(0),
             help="Number of virtual orbital cubes to generate",
         )
 
         spec.input(
             "cubes_edge_space",
-            valid_type=Float,
+            valid_type=orm.Float,
             required=False,
-            default=lambda: Float(3.0),
+            default=lambda: orm.Float(3.0),
             help="Extra cube space in addition to bounding box [ang].",
         )
 
         spec.input(
             "cubegen_parser_name",
             valid_type=str,
             default="nanotech_empa.gaussian.cubegen_pymol",
             non_db=True,
         )
 
         spec.input(
             "cubegen_parser_params",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
-            default=lambda: Dict(dict={}),
+            default=lambda: orm.Dict(dict={}),
             help="Additional parameters to cubegen parser.",
         )
 
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of automatic.",
         )
 
         spec.outline(
             cls.setup,
-            if_(cls.should_do_wfn_stability)(cls.uks_wfn_stability),
+            engine.if_(cls.should_do_wfn_stability)(cls.uks_wfn_stability),
             cls.optimization,
-            if_(cls.should_do_scf)(cls.scf),
+            engine.if_(cls.should_do_scf)(cls.scf),
             cls.finalize,
         )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
             301,
@@ -188,21 +190,20 @@
 
         self.ctx.link0 = {
             "%chk": "aiida.chk",
             "%mem": "%dMB" % memory_mb,
             "%nprocshared": str(num_cores),
         }
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
 
     def uks_wfn_stability(self):
-
         self.report("Running UKS WFN Stability")
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
                 "dieze_tag": "#P",
                 "functional": self.ctx.functional,
                 "basis_set": self.inputs.basis_set.value,
                 "charge": 0,
                 "multiplicity": self.ctx.mult,
@@ -222,21 +223,20 @@
 
         builder.gaussian.parameters = parameters
         builder.gaussian.structure = self.inputs.structure
         builder.gaussian.code = self.inputs.gaussian_code
         builder.gaussian.metadata.options = self.ctx.metadata_options
 
         future = self.submit(builder)
-        return ToContext(uks_stab=future)
+        return engine.ToContext(uks_stab=future)
 
     def optimization(self):
-
         self.report("Submitting optimization")
 
-        parameters = Dict(
+        parameters = orm.Dict(
             {
                 "link0_parameters": self.ctx.link0.copy(),
                 "dieze_tag": "#P",
                 "functional": self.ctx.functional,
                 "basis_set": self.inputs.basis_set.value,
                 "charge": 0,
                 "multiplicity": self.ctx.mult,
@@ -255,15 +255,15 @@
             builder.gaussian.parent_calc_folder = (
                 self.ctx.uks_stab.outputs.remote_folder
             )
         elif self.inputs.multiplicity == 1:
             parameters["route_parameters"]["guess"] = "mix"
 
         # In case of the open-shell singlet, take smaller steps to prevent
-        # losing the spin solution
+        # losing the spin solution.
         if self.inputs.multiplicity == 1:
             parameters["route_parameters"]["opt"] = {"maxstep": 10}
 
         if self.inputs.freq:
             parameters["route_parameters"]["freq"] = None
 
         if self.inputs.empirical_dispersion.value != "":
@@ -293,21 +293,20 @@
 
         builder.gaussian.parameters = parameters
         builder.gaussian.structure = self.inputs.structure
         builder.gaussian.code = self.inputs.gaussian_code
         builder.gaussian.metadata.options = self.ctx.metadata_options
 
         submitted_node = self.submit(builder)
-        return ToContext(opt=submitted_node)
+        return engine.ToContext(opt=submitted_node)
 
     def should_do_scf(self):
         return "basis_set_scf" in self.inputs
 
     def scf(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.opt):
             return self.exit_codes.ERROR_TERMINATION
 
         self.report("Submitting SCF")
 
         builder = GaussianScfWorkChain.get_builder()
         builder.gaussian_code = self.inputs.gaussian_code
@@ -327,18 +326,17 @@
             builder.cubegen_parser_name = self.inputs.cubegen_parser_name
             builder.cubegen_parser_params = self.inputs.cubegen_parser_params
 
         if "options" in self.inputs:
             builder.options = self.inputs.options
 
         submitted_node = self.submit(builder)
-        return ToContext(scf=submitted_node)
+        return engine.ToContext(scf=submitted_node)
 
     def finalize(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.opt):
             return self.exit_codes.ERROR_TERMINATION
 
         if self.inputs.freq:
             if "vibfreqs" not in dict(self.ctx.opt.outputs.output_parameters):
                 return self.exit_codes.ERROR_NO_VIBR_ANALYSIS
 
@@ -357,8 +355,8 @@
             self.out("scf_remote_folder", self.ctx.scf.outputs.remote_folder)
             for cubes_out in list(self.ctx.scf.outputs):
                 if cubes_out.startswith("cube"):
                     self.out(cubes_out, self.ctx.scf.outputs[cubes_out])
                 elif cubes_out == "retrieved":
                     self.out("cubes_retrieved", self.ctx.scf.outputs[cubes_out])
 
-        return ExitCode(0)
+        return engine.ExitCode(0)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,353 +1,305 @@
-from aiida.engine import ExitCode, ToContext, WorkChain, if_
-from aiida.orm import Bool, Code, Dict, Float, Int, List, RemoteData, Str, StructureData
-from aiida.plugins import WorkflowFactory
+import numpy as np
+from aiida import engine, orm, plugins
 
-from aiida_nanotech_empa.utils import common_utils
-from aiida_nanotech_empa.workflows.gaussian import common
+from ...utils import common_utils
+from .delta_scf_workchain import GaussianDeltaScfWorkChain
+from .natorb_workchain import GaussianNatOrbWorkChain
+from .relax_workchain import GaussianRelaxWorkChain
+from .scf_workchain import GaussianScfWorkChain
 
-GaussianBaseWorkChain = WorkflowFactory("gaussian.base")
-GaussianCubesWorkChain = WorkflowFactory("gaussian.cubes")
+GaussianBaseWorkChain = plugins.WorkflowFactory("gaussian.base")
+GaussianCubesWorkChain = plugins.WorkflowFactory("gaussian.cubes")
 
-# -------------------------------------------------------------
-# Work Chain to run SCF and possibly CUBES
-# -------------------------------------------------------------
 
-
-class GaussianScfWorkChain(WorkChain):
+class GaussianSpinWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        spec.input("gaussian_code", valid_type=Code)
+        spec.input("gaussian_code", valid_type=orm.Code)
+        spec.input("formchk_code", valid_type=orm.Code)
+        spec.input("cubegen_code", valid_type=orm.Code)
 
         spec.input(
-            "structure", valid_type=StructureData, required=True, help="input geometry"
+            "structure",
+            valid_type=orm.StructureData,
+            required=True,
+            help="input geometry",
         )
-
-        spec.input("functional", valid_type=Str, required=True, help="xc functional")
-
-        spec.input("basis_set", valid_type=Str, required=True, help="basis_set")
-
         spec.input(
-            "multiplicity",
-            valid_type=Int,
-            required=False,
-            default=lambda: Int(1),
-            help="spin multiplicity; 0 means RKS",
+            "functional", valid_type=orm.Str, required=True, help="xc functional"
         )
-
-        spec.input(
-            "wfn_stable_opt",
-            valid_type=Bool,
-            required=False,
-            default=lambda: Bool(False),
-            help="if true, perform wfn stability optimization",
-        )
-
-        spec.input(
-            "wfn_stable_opt_min_basis",
-            valid_type=Bool,
-            required=False,
-            default=lambda: Bool(False),
-            help="if true, perform first a minimal basis stability opt",
-        )
-
         spec.input(
             "empirical_dispersion",
-            valid_type=Str,
+            valid_type=orm.Str,
             required=False,
-            default=lambda: Str(""),
+            default=lambda: orm.Str(""),
             help=("Include empirical dispersion corrections" '(e.g. "GD3", "GD3BJ")'),
         )
-
-        spec.input(
-            "parent_calc_folder",
-            valid_type=RemoteData,
-            required=False,
-            help="the folder of a completed gaussian calculation",
-        )
-
-        # -------------------------------------------------------------------
-        # CUBE GENERATION INPUTS
-
-        spec.input("formchk_code", valid_type=Code, required=False)
-        spec.input("cubegen_code", valid_type=Code, required=False)
-
         spec.input(
-            "cubes_n_occ",
-            valid_type=Int,
-            required=False,
-            default=lambda: Int(0),
-            help="Number of occupied orbital cubes to generate",
+            "basis_set_opt", valid_type=orm.Str, required=True, help="basis_set for opt"
         )
-
         spec.input(
-            "cubes_n_virt",
-            valid_type=Int,
-            required=False,
-            default=lambda: Int(0),
-            help="Number of virtual orbital cubes to generate",
+            "basis_set_scf", valid_type=orm.Str, required=True, help="basis_set for scf"
         )
-
         spec.input(
-            "cubes_edge_space",
-            valid_type=Float,
-            required=False,
-            default=lambda: Float(3.0),
-            help="Extra cube space in addition to bounding box [ang].",
+            "multiplicity_list",
+            valid_type=orm.List,
+            required=True,
+            help="spin multiplicities",
         )
-
-        spec.input(
-            "cubegen_parser_name",
-            valid_type=str,
-            default="nanotech_empa.gaussian.cubegen_pymol",
-            non_db=True,
-        )
-
-        spec.input(
-            "cubegen_parser_params",
-            valid_type=Dict,
-            required=False,
-            default=lambda: Dict(dict={}),
-            help="Additional parameters to cubegen parser.",
-        )
-        # -------------------------------------------------------------------
-
         spec.input(
             "options",
-            valid_type=Dict,
+            valid_type=orm.Dict,
             required=False,
             help="Use custom metadata.options instead of the automatic ones.",
         )
 
         spec.outline(
-            cls.setup,
-            if_(cls.should_do_min_basis_stable_opt)(cls.min_basis_stable_opt),
-            cls.scf,
-            if_(cls.did_scf_fail)(cls.scf),
-            if_(cls.should_do_cubes)(cls.cubes),
+            cls.submit_opts,
+            cls.inspect_opts,
+            cls.submit_next_steps,
+            cls.inspect_next_steps,
+            engine.if_(cls.is_gs_oss)(cls.submit_nat_orb, cls.inspect_nat_orb),
             cls.finalize,
         )
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
-            301,
-            "ERROR_MULTIPLICITY",
-            message="Multiplicity and number of el. doesn't match.",
-        )
-        spec.exit_code(
-            302,
-            "ERROR_OPTIONS",
-            message="Input options are invalid.",
-        )
-        spec.exit_code(
             390,
             "ERROR_TERMINATION",
             message="One or more steps of the work chain failed.",
         )
 
-    def is_uks(self):
-        if self.inputs.multiplicity.value == 0:
-            return False
-        return True
-
-    def setup(self):
-        self.report("Inspecting input and setting up things")
+    def submit_opts(self):
+        # Multiplicity 0 means RKS calculation.
+        for mult in self.inputs.multiplicity_list:
+            label = f"m{mult}_opt"
+
+            builder = GaussianRelaxWorkChain.get_builder()
+            builder.gaussian_code = self.inputs.gaussian_code
+            builder.structure = self.inputs.structure
+            builder.functional = self.inputs.functional
+            builder.empirical_dispersion = self.inputs.empirical_dispersion
+            builder.basis_set = self.inputs.basis_set_opt
+            builder.multiplicity = orm.Int(mult)
+
+            builder.basis_set_scf = self.inputs.basis_set_scf
+            builder.formchk_code = self.inputs.formchk_code
+            builder.cubegen_code = self.inputs.cubegen_code
+
+            builder.cubes_n_occ = orm.Int(2)
+            builder.cubes_n_virt = orm.Int(2)
+            builder.cubes_edge_space = orm.Float(4.0)
+            builder.cubegen_parser_params = orm.Dict(
+                {
+                    "heights": [4.0],
+                    "orient_cube": True,
+                    "isovalues": [0.01],
+                }
+            )
 
-        common.setup_context_variables(self)
+            if "options" in self.inputs:
+                builder.options = self.inputs.options
 
-        if self.ctx.mult % 2 == self.ctx.n_electrons % 2:
-            return self.exit_codes.ERROR_MULTIPLICITY
+            submitted_node = self.submit(builder)
+            submitted_node.description = label
+            self.to_context(**{label: submitted_node})
 
-        success = common.determine_metadata_options(self)
-        if not success:
-            return self.exit_codes.ERROR_OPTIONS
+    def inspect_opts(self):
+        opt_energies = []
 
-        num_cores, memory_mb = common.get_gaussian_cores_and_memory(
-            self.ctx.metadata_options, self.ctx.comp
-        )
+        for mult in self.inputs.multiplicity_list:
+            label = f"m{mult}_opt"
 
-        self.ctx.link0 = {
-            "%chk": "aiida.chk",
-            "%mem": "%dMB" % memory_mb,
-            "%nprocshared": str(num_cores),
-        }
-
-        # Use default convergence criterion at the start
-        # but switch to conver=7 in case of failure
-        self.ctx.conver = None
-        self.ctx.scf_label = "scf"
-
-        return ExitCode(0)
+            # check if everything finished nicely
+            if not common_utils.check_if_calc_ok(self, self.ctx[label]):
+                return self.exit_codes.ERROR_TERMINATION
 
-    def should_do_min_basis_stable_opt(self):
-        return self.inputs.wfn_stable_opt_min_basis
+            opt_energy = self.ctx[label].outputs.scf_energy_ev
+            opt_energies.append(opt_energy)
+            self.out(f"m{mult}_opt_energy", opt_energy)
+            self.out(f"m{mult}_opt_structure", self.ctx[label].outputs.output_structure)
+            self.out(
+                f"m{mult}_opt_out_params", self.ctx[label].outputs.scf_output_parameters
+            )
+            self.out(
+                f"m{mult}_opt_cube_images", self.ctx[label].outputs.cube_image_folder
+            )
+            self.out(
+                f"m{mult}_opt_cube_planes", self.ctx[label].outputs.cube_planes_array
+            )
 
-    def min_basis_stable_opt(self):
-        self.report("Submitting minimal basis stable opt")
+        gs_i = np.argmin(opt_energies)
 
-        parameters = Dict(
+        # If open-shell singlet is degenerate with closed-shell solution, prefer closed-shell.
+        if (
+            self.inputs.multiplicity_list[gs_i] == 1
+            and 0 in self.inputs.multiplicity_list
+        ):
+            cs_i = self.inputs.multiplicity_list.index(0)
+            if np.abs(opt_energies[cs_i].value - opt_energies[gs_i].value) < 1e-6:
+                gs_i = cs_i
+
+        self.ctx.gs_mult = orm.Int(self.inputs.multiplicity_list[gs_i]).store()
+        self.ctx.gs_energy = opt_energies[gs_i]
+        gs_opt_label = f"m{self.ctx.gs_mult.value}_opt"
+        self.ctx.gs_structure = self.ctx[gs_opt_label].outputs.output_structure
+
+        self.ctx.gs_out_params = self.ctx[gs_opt_label].outputs.scf_output_parameters
+        self.ctx.gs_scf_remote_folder = self.ctx[gs_opt_label].outputs.scf_remote_folder
+
+        self.out("gs_multiplicity", self.ctx.gs_mult)
+        self.out("gs_energy", self.ctx.gs_energy)
+        self.out("gs_structure", self.ctx.gs_structure)
+        self.out("gs_out_params", self.ctx.gs_out_params)
+
+        return engine.ExitCode(0)
+
+    def submit_next_steps(self):
+        cubes_n_occ = 5
+        cubes_n_virt = 5
+        cubes_orb_indexes = list(range(-cubes_n_occ + 1, cubes_n_virt + 1))
+        cubes_isovalues = [0.010, 0.001]
+        cubes_heights = [3.0, 4.0]
+
+        self.report("Submitting GS cubes")
+
+        builder = GaussianCubesWorkChain.get_builder()
+        builder.formchk_code = self.inputs.formchk_code
+        builder.cubegen_code = self.inputs.cubegen_code
+        builder.gaussian_calc_folder = self.ctx.gs_scf_remote_folder
+        builder.gaussian_output_params = self.ctx.gs_out_params
+        builder.orbital_indexes = orm.List(cubes_orb_indexes)
+        builder.edge_space = orm.Float(max(cubes_heights))
+        builder.cubegen_parser_name = "nanotech_empa.gaussian.cubegen_pymol"
+        builder.cubegen_parser_params = orm.Dict(
             {
-                "link0_parameters": self.ctx.link0.copy(),
-                "dieze_tag": "#P",
-                "functional": self.ctx.functional,
-                "basis_set": "STO-3G",
-                "charge": 0,
-                "multiplicity": self.ctx.mult,
-                "route_parameters": {
-                    "scf": {"maxcycle": 140},
-                    "stable": "opt",
-                },
+                "isovalues": cubes_isovalues,
+                "heights": cubes_heights,
+                "orient_cube": True,
             }
         )
 
-        builder = GaussianBaseWorkChain.get_builder()
-
-        if "parent_calc_folder" in self.inputs:
-            # Read WFN from parent calc
-            parameters["link0_parameters"]["%oldchk"] = "parent_calc/aiida.chk"
-            parameters["route_parameters"]["guess"] = "read"
-            builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
-        elif self.is_uks() and self.ctx.mult == 1:
-            # For open-shell singlet, mix homo & lumo
-            parameters["route_parameters"]["guess"] = "mix"
-
-        builder.gaussian.parameters = parameters
-        builder.gaussian.structure = self.inputs.structure
-        builder.gaussian.code = self.inputs.gaussian_code
-        builder.gaussian.metadata.options = self.ctx.metadata_options
-
-        future = self.submit(builder)
-        return ToContext(min_stable=future)
+        submitted_node = self.submit(builder)
+        submitted_node.description = "gs cubes"
+        self.to_context(gs_cubes=submitted_node)
+
+        self.report("Submitting Delta SCF")
+
+        builder = GaussianDeltaScfWorkChain.get_builder()
+        builder.gaussian_code = self.inputs.gaussian_code
+        builder.structure = self.ctx.gs_structure
+        builder.functional = self.inputs.functional
+        builder.basis_set = self.inputs.basis_set_scf
+        builder.multiplicity = self.ctx.gs_mult
+        builder.parent_calc_folder = self.ctx.gs_scf_remote_folder
+        if "options" in self.inputs:
+            builder.options = self.inputs.options
+
+        submitted_node = self.submit(builder)
+        submitted_node.description = "delta scf"
+        self.to_context(dscf=submitted_node)
+
+        self.report("Submitting vertical calculations")
+
+        for mult in self.inputs.multiplicity_list:
+            label = f"m{mult}_vert"
+            opt_label = f"m{mult}_opt"
+
+            if mult == self.ctx.gs_mult:
+                continue
+
+            builder = GaussianScfWorkChain.get_builder()
+            builder.gaussian_code = self.inputs.gaussian_code
+            builder.formchk_code = self.inputs.formchk_code
+            builder.cubegen_code = self.inputs.cubegen_code
+            builder.structure = self.ctx.gs_structure
+            builder.functional = self.inputs.functional
+            builder.empirical_dispersion = self.inputs.empirical_dispersion
+            builder.basis_set = self.inputs.basis_set_scf
+            builder.multiplicity = orm.Int(mult)
+            builder.parent_calc_folder = self.ctx[opt_label].outputs.remote_folder
+            builder.cubes_n_occ = orm.Int(cubes_n_occ)
+            builder.cubes_n_virt = orm.Int(cubes_n_virt)
+            builder.cubegen_parser_params = orm.Dict(
+                {
+                    "isovalues": cubes_isovalues,
+                    "heights": cubes_heights,
+                    "orient_cube": True,
+                }
+            )
 
-    def scf(self):
-        self.report("Submitting SCF")
+            if "options" in self.inputs:
+                builder.options = self.inputs.options
 
-        parameters = Dict(
-            {
-                "link0_parameters": self.ctx.link0.copy(),
-                "dieze_tag": "#P",
-                "functional": self.ctx.functional,
-                "basis_set": self.inputs.basis_set.value,
-                "charge": 0,
-                "multiplicity": self.ctx.mult,
-                "route_parameters": {
-                    "scf": {"maxcycle": 140},
-                },
-            }
-        )
-        if self.inputs.wfn_stable_opt:
-            parameters["route_parameters"]["stable"] = "opt"
-        else:
-            parameters["route_parameters"]["sp"] = None
-
-        builder = GaussianBaseWorkChain.get_builder()
-
-        if self.should_do_min_basis_stable_opt():
-            # Read WFN from min basis stable opt
-            parameters["link0_parameters"]["%oldchk"] = "parent_calc/aiida.chk"
-            parameters["route_parameters"]["guess"] = "read"
-            builder.gaussian.parent_calc_folder = (
-                self.ctx.min_stable.outputs.remote_folder
-            )
-        elif "parent_calc_folder" in self.inputs:
-            # Read WFN from parent calc
-            parameters["link0_parameters"]["%oldchk"] = "parent_calc/aiida.chk"
-            parameters["route_parameters"]["guess"] = "read"
-            builder.gaussian.parent_calc_folder = self.inputs.parent_calc_folder
-        elif self.is_uks() and self.ctx.mult == 1:
-            # For open-shell singlet, mix homo & lumo
-            parameters["route_parameters"]["guess"] = "mix"
-
-        if self.inputs.empirical_dispersion.value != "":
-            parameters["route_parameters"][
-                "empiricaldispersion"
-            ] = self.inputs.empirical_dispersion.value
-
-        if self.ctx.conver is not None:
-            parameters["route_parameters"]["scf"]["conver"] = self.ctx.conver
-
-        builder.gaussian.parameters = parameters
-        builder.gaussian.structure = self.inputs.structure
-        builder.gaussian.code = self.inputs.gaussian_code
-        builder.gaussian.metadata.options = self.ctx.metadata_options
-
-        future = self.submit(builder)
-        future.description = self.ctx.scf_label
-        return ToContext(**{self.ctx.scf_label: future})
-
-    def did_scf_fail(self):
-
-        scf_node = self.ctx[self.ctx.scf_label]
-        if not common_utils.check_if_calc_ok(self, scf_node):
-            # set up for conver=7 calculation
-            self.report("SCF failed with default convergence criterion!")
-            self.report("Switching to a looser threshold.")
-            self.ctx.conver = 7
-            self.ctx.scf_label = f"scf_c{self.ctx.conver}"
-            return True
-        return False
-
-    def should_do_cubes(self):
-        codes_set = "formchk_code" in self.inputs and "cubegen_code" in self.inputs
-        non_zero_num = (
-            self.inputs.cubes_n_occ.value > 0 and self.inputs.cubes_n_virt.value > 0
-        )
-        return codes_set and non_zero_num
+            submitted_node = self.submit(builder)
+            submitted_node.description = label
+            self.to_context(**{label: submitted_node})
 
-    def cubes(self):
+    def inspect_next_steps(self):
+        if not common_utils.check_if_calc_ok(self, self.ctx.gs_cubes):
+            return self.exit_codes.ERROR_TERMINATION
 
-        scf_node = self.ctx[self.ctx.scf_label]
+        self.out("gs_cube_images", self.ctx.gs_cubes.outputs.cube_image_folder)
+        self.out("gs_cube_planes", self.ctx.gs_cubes.outputs.cube_planes_array)
 
-        if not common_utils.check_if_calc_ok(self, scf_node):
+        if not common_utils.check_if_calc_ok(self, self.ctx.dscf):
             return self.exit_codes.ERROR_TERMINATION
 
-        self.report("Generating cubes")
+        self.out("gs_ionization_potential", self.ctx.dscf.outputs.ionization_potential)
+        self.out("gs_electron_affinity", self.ctx.dscf.outputs.electron_affinity)
 
-        orb_index_list = list(
-            range(
-                -self.inputs.cubes_n_occ.value + 1, self.inputs.cubes_n_virt.value + 1
-            )
-        )
+        for mult in self.inputs.multiplicity_list:
+            label = f"m{mult}_vert"
 
-        future = self.submit(
-            GaussianCubesWorkChain,
-            formchk_code=self.inputs.formchk_code,
-            cubegen_code=self.inputs.cubegen_code,
-            gaussian_calc_folder=scf_node.outputs.remote_folder,
-            gaussian_output_params=scf_node.outputs["output_parameters"],
-            orbital_indexes=List(list=orb_index_list),
-            orbital_index_ref=Str("half_num_el"),
-            edge_space=self.inputs.cubes_edge_space,
-            dx=Float(0.15),
-            retrieve_cubes=Bool(False),
-            cubegen_parser_name=self.inputs.cubegen_parser_name,
-            cubegen_parser_params=self.inputs.cubegen_parser_params,
-        )
-        return ToContext(cubes=future)
+            if mult == self.ctx.gs_mult:
+                continue
 
-    def finalize(self):
+            # Check if everything finished nicely.
+            if not common_utils.check_if_calc_ok(self, self.ctx[label]):
+                return self.exit_codes.ERROR_TERMINATION
 
-        scf_node = self.ctx[self.ctx.scf_label]
+            vert_energy = self.ctx[label].outputs.energy_ev
+            self.out(f"m{mult}_vert_energy", vert_energy)
+            self.out(
+                f"m{mult}_vert_out_params", self.ctx[label].outputs.output_parameters
+            )
+            self.out(
+                f"m{mult}_vert_cube_images", self.ctx[label].outputs.cube_image_folder
+            )
+            self.out(
+                f"m{mult}_vert_cube_planes", self.ctx[label].outputs.cube_planes_array
+            )
 
-        if not common_utils.check_if_calc_ok(self, scf_node):
-            return self.exit_codes.ERROR_TERMINATION
+        return engine.ExitCode(0)
 
-        self.report("Finalizing...")
+    def is_gs_oss(self):
+        """Is ground state an open-shell singlet?"""
+        return self.ctx.gs_mult == 1
+
+    def submit_nat_orb(self):
+        self.report("Submitting natural pop analysis")
+
+        builder = GaussianNatOrbWorkChain.get_builder()
+        builder.gaussian_code = self.inputs.gaussian_code
+        builder.parent_calc_folder = self.ctx.gs_scf_remote_folder
+        builder.parent_calc_params = self.ctx.gs_out_params
+        if "options" in self.inputs:
+            builder.options = self.inputs.options
+
+        submitted_node = self.submit(builder)
+        submitted_node.description = "natural orbitals pop"
+        self.to_context(natorb=submitted_node)
 
-        if self.should_do_cubes():
-            if not common_utils.check_if_calc_ok(self, self.ctx.cubes):
-                return self.exit_codes.ERROR_TERMINATION
-            for cubes_out in list(self.ctx.cubes.outputs):
-                if cubes_out.startswith("cube"):
-                    self.out(cubes_out, self.ctx.cubes.outputs[cubes_out])
-                elif cubes_out == "retrieved":
-                    self.out("cubes_retrieved", self.ctx.cubes.outputs[cubes_out])
+    def inspect_nat_orb(self):
+        if not common_utils.check_if_calc_ok(self, self.ctx.natorb):
+            return self.exit_codes.ERROR_TERMINATION
 
-        self.out("energy_ev", scf_node.outputs.energy_ev)
-        self.out("output_parameters", scf_node.outputs["output_parameters"])
+        self.out("gs_natorb_params", self.ctx.natorb.outputs.natorb_proc_parameters)
 
-        self.out("remote_folder", scf_node.outputs["remote_folder"])
+        return engine.ExitCode(0)
 
-        return ExitCode(0)
+    def finalize(self):
+        self.report("Finalizing...")
```

### Comparing `aiida-nanotech-empa-1.0.0a0/aiida_nanotech_empa/workflows/qe/nanoribbon.py` & `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/qe/nanoribbon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import numpy as np
-from aiida.engine import ToContext, WorkChain, while_
+from aiida import engine, orm, plugins
 
-# AiiDA imports
-from aiida.orm import (
-    Bool,
-    Code,
-    Dict,
-    Float,
-    Int,
-    KpointsData,
-    Str,
-    StructureData,
-    load_group,
-)
-from aiida_quantumespresso.calculations.pp import PpCalculation
-from aiida_quantumespresso.calculations.projwfc import ProjwfcCalculation
-
-# aiida_quantumespresso imports
-from aiida_quantumespresso.calculations.pw import PwCalculation
+from ...utils import common_utils
 
-from aiida_nanotech_empa.utils import common_utils
+PwCalculation = plugins.CalculationFactory("quantumespresso.pw")
+PpCalculation = plugins.CalculationFactory("quantumespresso.pp")
+ProjwfcCalculation = plugins.CalculationFactory("quantumespresso.projwfc")
 
-# from aiida.orm.nodes.data.upf import get_pseudos_dict, get_pseudos_from_structure
 
-
-class NanoribbonWorkChain(WorkChain):
+class NanoribbonWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
         spec.input(
-            "optimize_cell", valid_type=Bool, default=lambda: Bool(True), required=False
+            "optimize_cell",
+            valid_type=orm.Bool,
+            default=lambda: orm.Bool(True),
+            required=False,
+        )
+        spec.input(
+            "max_kpoints",
+            valid_type=orm.Int,
+            default=lambda: orm.Int(120),
+            required=False,
+        )
+        spec.input(
+            "max_nodes", valid_type=orm.Int, default=lambda: orm.Int(24), required=False
         )
         spec.input(
-            "max_kpoints", valid_type=Int, default=lambda: Int(120), required=False
+            "mem_node", valid_type=orm.Int, default=lambda: orm.Int(64), required=False
         )
-        spec.input("max_nodes", valid_type=Int, default=lambda: Int(24), required=False)
-        spec.input("mem_node", valid_type=Int, default=lambda: Int(64), required=False)
-        spec.input("pw_code", valid_type=Code)
-        spec.input("pp_code", valid_type=Code)
-        spec.input("projwfc_code", valid_type=Code)
-        spec.input("structure", valid_type=StructureData)
+        spec.input("pw_code", valid_type=orm.Code)
+        spec.input("pp_code", valid_type=orm.Code)
+        spec.input("projwfc_code", valid_type=orm.Code)
+        spec.input("structure", valid_type=orm.StructureData)
         spec.input(
-            "tot_charge", valid_type=Float, default=lambda: Float(0.0), required=False
+            "tot_charge",
+            valid_type=orm.Float,
+            default=lambda: orm.Float(0.0),
+            required=False,
         )
         spec.input(
-            "precision", valid_type=Float, default=lambda: Float(1.0), required=False
+            "precision",
+            valid_type=orm.Float,
+            default=lambda: orm.Float(1.0),
+            required=False,
         )
         spec.input(
-            "num_export_bands", valid_type=Int, default=lambda: Int(8), required=False
+            "num_export_bands",
+            valid_type=orm.Int,
+            default=lambda: orm.Int(8),
+            required=False,
         )
         spec.input(
             "pseudo_family",
-            valid_type=Str,
+            valid_type=orm.Str,
             required=True,
             help="An alternative to specifying the pseudo potentials manually in `pseudos`: one can specify the name "
             "of an existing pseudo potential family and the work chain will generate the pseudos automatically "
             "based on the input structure.",
         )
         # TODO: check why it does not work
         # spec.inputs("metadata.label", valid_type=six.string_types,
@@ -65,25 +68,24 @@
             cls.run_cell_opt2,
             cls.run_scf,
             cls.run_export_hartree,
             cls.run_bands,
             cls.run_export_pdos,
             cls.run_bands_lowres,
             cls.prepare_export_orbitals,
-            while_(cls.should_run_export_orbitals)(
+            engine.while_(cls.should_run_export_orbitals)(
                 cls.run_export_orbitals,
             ),
             cls.run_export_spinden,
             cls.run_closing,
         )
         spec.outputs.dynamic = True
 
         spec.exit_code(300, "CALC_FAILED", message="The calculation failed.")
 
-    # =========================================================================
     def run_cell_opt1(self):
         if self.inputs.optimize_cell.value:
             structure = self.inputs.structure
             return self._submit_pw_calc(
                 structure,
                 tot_charge=self.inputs.tot_charge.value,
                 label="cell_opt1",
@@ -92,15 +94,14 @@
                 min_kpoints=int(1),
                 max_nodes=self.inputs.max_nodes.value,
                 mem_node=self.inputs.mem_node.value,
             )
         self.report("Skipping: cell_opt = False")
         return
 
-    # =========================================================================
     def run_cell_opt2(self):
         if self.inputs.optimize_cell.value:
             prev_calc = self.ctx.cell_opt1
 
             if not common_utils.check_if_calc_ok(self, prev_calc):
                 return self.exit_codes.CALC_FAILED
 
@@ -114,15 +115,14 @@
                 min_kpoints=int(1),
                 max_nodes=self.inputs.max_nodes.value,
                 mem_node=self.inputs.mem_node.value,
             )
         self.report("Skipping: cell_opt = False")
         return
 
-    # =========================================================================
     def run_scf(self):
         if self.inputs.optimize_cell.value:
             prev_calc = self.ctx.cell_opt2
 
             if not common_utils.check_if_calc_ok(self, prev_calc):
                 return self.exit_codes.CALC_FAILED
 
@@ -138,15 +138,14 @@
             precision=3.0,
             min_kpoints=min_kpoints,
             max_nodes=self.inputs.max_nodes.value,
             mem_node=self.inputs.mem_node.value,
             wallhours=4,
         )
 
-    # =========================================================================
     def run_export_hartree(self):
         self.report("Running pp.x to export hartree potential")
         label = "export_hartree"
 
         builder = PpCalculation.get_builder()
         builder.code = self.inputs.pp_code
 
@@ -158,15 +157,15 @@
         builder.parent_folder = prev_calc.outputs.remote_folder
 
         structure = prev_calc.inputs.structure
         cell_a = structure.cell[0][0]
         cell_b = structure.cell[1][1]
         cell_c = structure.cell[2][2]
 
-        builder.parameters = Dict(
+        builder.parameters = orm.Dict(
             {
                 "INPUTPP": {
                     "plot_num": 11,  # the V_bare + V_H potential
                 },
                 "PLOT": {
                     "iflag": 2,
                     "x0(1)": 0.0,
@@ -202,30 +201,18 @@
             "resources": {
                 "num_machines": int(nnodes),
                 "num_mpiprocs_per_machine": nproc_mach,
             },
             "max_wallclock_seconds": 1200,  # 30 minutes
             "withmpi": True,
         }
-        builder.settings = Dict({"cmdline": ["-npools", str(npools)]})
+        builder.settings = orm.Dict({"cmdline": ["-npools", str(npools)]})
+        return engine.ToContext(**{label: self.submit(builder)})
 
-        #        builder.metadata.options = {
-        #            "resources": {
-        #                "num_machines": int(1),
-        #            },
-        #            "max_wallclock_seconds": 1200,
-        #            "withmpi": True,
-        #        }
-
-        running = self.submit(builder)
-        return ToContext(**{label: running})
-
-    # =========================================================================
     def run_bands(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.export_hartree):
             return self.exit_codes.CALC_FAILED
 
         prev_calc = self.ctx.scf
         structure = prev_calc.inputs.structure
         parent_folder = prev_calc.outputs.remote_folder
         min_kpoints = min(int(20), self.inputs.max_kpoints.value)
@@ -238,17 +225,15 @@
             precision=4.0,
             min_kpoints=min_kpoints,
             max_nodes=self.inputs.max_nodes.value,
             mem_node=self.inputs.mem_node.value,
             wallhours=6,
         )
 
-    # =========================================================================
     def run_export_pdos(self):
-
         prev_calc = self.ctx.bands
         if not common_utils.check_if_calc_ok(self, prev_calc):
             return self.exit_codes.CALC_FAILED
 
         self.report("Running projwfc.x to export PDOS")
         label = "export_pdos"
 
@@ -271,15 +256,15 @@
             npools = previous_pools
             nproc_mach = builder.code.computer.get_default_mpiprocs_per_machine()
 
         nhours = 24
         builder.parent_folder = prev_calc.outputs.remote_folder
 
         # use the same number of pools as in bands calculation
-        builder.parameters = Dict(
+        builder.parameters = orm.Dict(
             {
                 "projwfc": {
                     "ngauss": 1,
                     "degauss": 0.007,
                     "DeltaE": 0.01,
                     "filproj": "projection.out",
                 },
@@ -292,32 +277,30 @@
                 "num_machines": int(nnodes),
                 "num_mpiprocs_per_machine": nproc_mach,
             },
             "max_wallclock_seconds": nhours * 60 * 60,  # hours
             "withmpi": True,
         }
 
-        builder.settings = Dict(
+        builder.settings = orm.Dict(
             {
                 "additional_retrieve_list": [
                     "./out/aiida.save/*.xml",
                     "*_up",
                     "*_down",
                     "*_tot",
                 ],
                 "cmdline": ["-npools", str(npools)],
             }
         )
 
         future = self.submit(builder)
-        return ToContext(**{label: future})
+        return engine.ToContext(**{label: future})
 
-    # =========================================================================
     def run_bands_lowres(self):
-
         if not common_utils.check_if_calc_ok(self, self.ctx.export_pdos):
             return self.exit_codes.CALC_FAILED
 
         self.report("Running bands with fewer kpt to export KS")
 
         prev_calc = self.ctx.scf
         structure = prev_calc.inputs.structure
@@ -332,17 +315,15 @@
             precision=0.0,
             min_kpoints=min_kpoints,
             max_nodes=self.inputs.max_nodes.value,
             mem_node=self.inputs.mem_node.value,
             wallhours=2,
         )
 
-    # =========================================================================
     def prepare_export_orbitals(self):
-
         prev_calc = self.ctx.bands_lowres
         if not common_utils.check_if_calc_ok(self, prev_calc):
             return self.exit_codes.CALC_FAILED
 
         self.report("Getting ready to export KS orbitals.")
 
         self.ctx.export_orbitals_parameters = {
@@ -369,24 +350,24 @@
         nnodes = min(
             self.inputs.max_nodes.value, (1 + int(natoms / self.inputs.mem_node.value))
         )
         npools = 1
         self.ctx.export_orbitals_options = {
             "resources": {
                 "num_machines": int(nnodes),
-                # int(prev_calc.attributes['resources']['num_machines']),
                 "num_mpiprocs_per_machine": self.inputs.pp_code.computer.get_default_mpiprocs_per_machine(),
             },
-            "max_wallclock_seconds": nhours * 60 * 60,  # 6 hours
-            # Add the post-processing python scripts
+            "max_wallclock_seconds": nhours * 60 * 60,
+            # Add the post-processing python scripts.
             "withmpi": True,
             "parser_name": "nanotech_empa.pp",
         }
-        # npools = int(prev_calc.inputs.settings['cmdline'][1])
-        self.ctx.export_orbitals_settings = Dict({"cmdline": ["-npools", str(npools)]})
+        self.ctx.export_orbitals_settings = orm.Dict(
+            {"cmdline": ["-npools", str(npools)]}
+        )
 
         kband1 = max(
             int(prev_calc.res.number_of_electrons / 2)
             - int(self.inputs.num_export_bands.value / 2)
             + 1,
             1,
         )
@@ -399,21 +380,19 @@
             int(prev_calc.res.number_of_electrons / 2)
             + int(self.inputs.num_export_bands.value / 2),
             int(prev_calc.res.number_of_bands),
         )
         return self.ctx.export_orbitals_band_number <= kband2
 
     def run_export_orbitals(self):
-        # check if previous calc was okay
+        # Check if the previous calculation has finished successfully.
         if self.ctx.export_orbitals_band_number == self.ctx.first_band:
             to_check = "bands_lowres"
         else:
-            to_check = "export_orbitals_{}".format(
-                self.ctx.export_orbitals_band_number - 1
-            )
+            to_check = f"export_orbitals_{self.ctx.export_orbitals_band_number-1}"
         if not common_utils.check_if_calc_ok(self, getattr(self.ctx, to_check)):
             return self.exit_codes.CALC_FAILED
 
         self.report("Running pp.x to export KS orbitals")
 
         builder = PpCalculation.get_builder()
         builder.code = self.inputs.pp_code
@@ -426,23 +405,22 @@
         # Modifying the band number.
         self.ctx.export_orbitals_parameters["INPUTPP"][
             "kband(1)"
         ] = self.ctx.export_orbitals_band_number
         self.ctx.export_orbitals_parameters["INPUTPP"][
             "kband(2)"
         ] = self.ctx.export_orbitals_band_number
-        builder.parameters = Dict(self.ctx.export_orbitals_parameters)
+        builder.parameters = orm.Dict(self.ctx.export_orbitals_parameters)
 
         # Running the calculation.
         running = self.submit(builder)
         label = f"export_orbitals_{self.ctx.export_orbitals_band_number}"
         self.ctx.export_orbitals_band_number += 1
-        return ToContext(**{label: running})
+        return engine.ToContext(**{label: running})
 
-    # =========================================================================
     def run_export_spinden(self):
         self.report("Running pp.x to compute spinden")
         label = "export_spinden"
         last_ks = f"export_orbitals_{self.ctx.export_orbitals_band_number - 1}"
 
         if not common_utils.check_if_calc_ok(self, getattr(self.ctx, last_ks)):
             return self.exit_codes.CALC_FAILED
@@ -456,21 +434,19 @@
         nspin = prev_calc.res.number_of_spin_components
         natoms = len(prev_calc.inputs.structure.base.attributes.all["sites"])
         nnodes = min(
             self.inputs.max_nodes.value, (1 + int(natoms / self.inputs.mem_node.value))
         )
         # Reconsider the following lines, when https://gitlab.com/QEF/q-e/-/issues/221 is fixed.
         npools = 1
-        # nnodes = int(prev_calc.attributes['resources']['num_machines'])
-        # npools = int(prev_calc.inputs.settings.get_dict()['cmdline'][1])
         if nspin == 1:
             self.report("Skipping, got only one spin channel")
             return
 
-        builder.parameters = Dict(
+        builder.parameters = orm.Dict(
             {
                 "INPUTPP": {
                     "plot_num": 6,  # spin polarization (rho(up)-rho(down))
                 },
                 "PLOT": {
                     "iflag": 3,  # 3D plot
                 },
@@ -484,41 +460,37 @@
                 "num_mpiprocs_per_machine": nproc_mach,
             },
             "max_wallclock_seconds": 30 * 60,  # 30 minutes
             "withmpi": True,
             "parser_name": "nanotech_empa.pp",
         }
 
-        builder.settings = Dict({"cmdline": ["-npools", str(npools)]})
+        builder.settings = orm.Dict({"cmdline": ["-npools", str(npools)]})
 
         future = self.submit(builder)
-        return ToContext(**{label: future})
-
-    # =========================================================================
+        return engine.ToContext(**{label: future})
 
     def run_closing(self):
         self.report("Running final check")
         # Getting and checking the previous calculation.
         nspin = self.ctx.scf.res.number_of_spin_components
 
-        # ---
-        # check if previous calc was okay
+        # Check if previous calc was okay.
         if nspin > 1:
             prev_calc = self.ctx.export_spinden
             if not common_utils.check_if_calc_ok(self, prev_calc):
                 return self.exit_codes.CALC_FAILED
 
             self.out(
                 "spin_density_arraydata", self.ctx.export_spinden.outputs.output_data
             )
 
         self.report("END of workchain")
         return
 
-    # =========================================================================
     def _submit_pw_calc(
         self,
         structure,
         tot_charge,
         label,
         runtype,
         precision,
@@ -530,18 +502,17 @@
     ):
         self.report("Running pw.x for " + label)
         builder = PwCalculation.get_builder()
 
         builder.code = self.inputs.pw_code
         builder.structure = structure
         builder.parameters = self._get_parameters(structure, tot_charge, runtype, label)
-        # builder.pseudos = validate_and_prepare_pseudos_inputs(
-        #    structure, None, self.inputs.pseudo_family)
-        # loading family from input
-        family_pseudo = load_group(self.inputs.pseudo_family.value)
+
+        # Loading family from input.
+        family_pseudo = orm.load_group(self.inputs.pseudo_family.value)
         builder.pseudos = family_pseudo.get_pseudos(structure=structure)
 
         if parent_folder:
             builder.parent_folder = parent_folder
 
         # kpoints
         cell_a = builder.structure.cell[0][0]
@@ -592,20 +563,19 @@
         # nnodes.store
         builder.metadata.options = {
             "resources": {"num_machines": int(nnodes)},
             "withmpi": True,
             "max_wallclock_seconds": wallhours * 60 * 60,
         }
 
-        builder.parallelization = Dict({"npool": int(npools)})
+        builder.parallelization = orm.Dict({"npool": int(npools)})
 
         future = self.submit(builder)
-        return ToContext(**{label: future})
+        return engine.ToContext(**{label: future})
 
-    # =========================================================================
     def _get_parameters(self, structure, tot_charge, runtype, label):
         params = {
             "CONTROL": {
                 "calculation": runtype,
                 "wf_collect": True,
                 "forc_conv_thr": 0.0001,
                 "nstep": 500,
@@ -624,41 +594,36 @@
                 "scf_must_converge": False,
             },
         }
 
         if label == "cell_opt1":
             params["CONTROL"]["forc_conv_thr"] = 0.0005
         if runtype == "vc-relax":
-            # in y and z direction there is only vacuum
+            # In y and z direction there is only vacuum.
             params["CELL"] = {"cell_dofree": "x"}
 
-        # if runtype == "bands":
-        #     params['CONTROL']['restart_mode'] = 'restart'
-
         start_mag = self._get_magnetization(structure)
         if any(m != 0 for m in start_mag.values()):
             params["SYSTEM"]["nspin"] = 2
             params["SYSTEM"]["starting_magnetization"] = start_mag
 
-        return Dict(params)
+        return orm.Dict(params)
 
-    # =========================================================================
     def _get_kpoints(self, nx, use_symmetry=True):
         nx = max(1, nx)
 
-        kpoints = KpointsData()
+        kpoints = orm.KpointsData()
         if use_symmetry:
             kpoints.set_kpoints_mesh([nx, 1, 1], offset=[0.0, 0.0, 0.0])
         else:
             # List kpoints explicitly.
             points = [[r, 0.0, 0.0] for r in np.linspace(0, 0.5, nx)]
             kpoints.set_kpoints(points)
         return kpoints
 
-    # =========================================================================
     def _get_magnetization(self, structure):
         start_mag = {}
         for i in structure.kinds:
             if i.name.endswith("1"):
                 start_mag[i.name] = 1.0
             elif i.name.endswith("2"):
                 start_mag[i.name] = -1.0
```

### Comparing `aiida-nanotech-empa-1.0.0a0/conftest.py` & `aiida_nanotech_empa-1.0.0b0/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 @pytest.fixture(scope="function")
 def local_code_factory(fixture_localhost):
     """Modified version of aiida_local_code_factory, that uses fixture_localhost"""
 
     def get_code(
         entry_point, executable, label=None, prepend_text=None, append_text=None
     ):
-
         if label is None:
             label = executable
 
         computer = fixture_localhost
 
         builder = QueryBuilder().append(
             Computer, filters={"uuid": computer.uuid}, tag="computer"
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/data/sssp_minimal/C.upf` & `aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/C.upf`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/data/sssp_minimal/H.upf` & `aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/H.upf`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/benzene-diradical.xyz` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/benzene-diradical.xyz`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_ads_gw_ic.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_ads_gw_ic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import os
 
-import ase.io
-from aiida.engine import run_get_node
-from aiida.orm import Bool, Float, Int, List, Str, StructureData, load_code
-from aiida.plugins import WorkflowFactory
-from ase import Atoms
+import ase
+from aiida import engine, orm, plugins
 
-Cp2kAdsorbedGwIcWorkChain = WorkflowFactory("nanotech_empa.cp2k.ads_gw_ic")
+Cp2kAdsorbedGwIcWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.ads_gw_ic")
 
 DATA_DIR = os.path.dirname(os.path.abspath(__file__))
 GEO_FILE = "h2_on_au111.xyz"
 
 
 def _example_cp2k_ads_gw_ic(cp2k_code, slab_included):
-
     builder = Cp2kAdsorbedGwIcWorkChain.get_builder()
 
     builder.metadata.description = os.path.splitext(GEO_FILE)[0]
     builder.code = cp2k_code
 
     if slab_included:
         ase_geom = ase.io.read(os.path.join(DATA_DIR, GEO_FILE))
         # Convert ase tags to magnetization list
         mag_list = [-1 if t == 1 else 1 if t == 2 else 0 for t in ase_geom.get_tags()]
     else:
-        ase_geom = Atoms(
+        ase_geom = ase.Atoms(
             "HH", positions=[[0, 0, 0], [0.75, 0, 0]], cell=[4.0, 4.0, 4.0]
         )
         mag_list = [-1, 1]
-        builder.ads_height = Float(3.0)
+        builder.ads_height = orm.Float(3.0)
 
-    builder.structure = StructureData(ase=ase_geom)
-    builder.magnetization_per_site = List(mag_list)
+    builder.structure = orm.StructureData(ase=ase_geom)
+    builder.magnetization_per_site = orm.List(mag_list)
 
-    builder.protocol = Str("gpw_std")
-    builder.multiplicity = Int(1)
+    builder.protocol = orm.Str("gpw_std")
+    builder.multiplicity = orm.Int(1)
 
-    builder.geometry_mode = Str("ads_geo")
+    builder.geometry_mode = orm.Str("ads_geo")
 
-    builder.debug = Bool(True)
+    builder.debug = orm.Bool(True)
     builder.options.scf = {
         "max_wallclock_seconds": 600,
         "resources": {
             "num_machines": 1,
             "num_mpiprocs_per_machine": 1,
             "num_cores_per_mpiproc": 1,
         },
@@ -59,15 +55,15 @@
         "max_wallclock_seconds": 600,
         "resources": {
             "num_machines": 1,
             "num_mpiprocs_per_machine": 1,
             "num_cores_per_mpiproc": 1,
         },
     }
-    _, calc_node = run_get_node(builder)
+    _, calc_node = engine.run_get_node(builder)
 
     assert calc_node.is_finished_ok
 
     gw_ic_res = dict(calc_node.outputs.gw_ic_parameters)
     print()
     for k in gw_ic_res:
         print(f"  {k}: {gw_ic_res[k]}")
@@ -80,10 +76,10 @@
 
 def example_cp2k_ads_gw_ic_implicit_slab(cp2k_code):
     _example_cp2k_ads_gw_ic(cp2k_code, slab_included=False)
 
 
 if __name__ == "__main__":
     print("# Slab in geometry explicitly #")
-    _example_cp2k_ads_gw_ic(load_code("cp2k@localhost"), slab_included=True)
+    _example_cp2k_ads_gw_ic(orm.load_code("cp2k@localhost"), slab_included=True)
     print("# Slab specified implicitly #")
-    _example_cp2k_ads_gw_ic(load_code("cp2k@localhost"), slab_included=False)
+    _example_cp2k_ads_gw_ic(orm.load_code("cp2k@localhost"), slab_included=False)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_bulkopt.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_phonons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,95 @@
-import os
+import pathlib
 
 import ase.io
-from aiida.engine import run_get_node
-from aiida.orm import Bool, Int, List, Str, StructureData, load_code
-from aiida.plugins import WorkflowFactory
+from aiida import engine, orm, plugins
 
-Cp2kBulkOptWorkChain = WorkflowFactory("nanotech_empa.cp2k.bulk_opt")
+Cp2kPhononsWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.phonons")
+DATA_DIR = pathlib.Path(__file__).parent.absolute()
+GEO_FILE = "c2h2.xyz"
+
+
+def _example_cp2k_phonons(cp2k_code, uks):
+    # check test geometry is already in database
+    qb = orm.QueryBuilder()
+    qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
+    structure = None
+    for node_tuple in qb.iterall():
+        node = node_tuple[0]
+        structure = node
+    if structure is not None:
+        print(f"Found existing structure: {structure.pk}")
+    else:
+        structure = orm.StructureData(ase=ase.io.read(DATA_DIR / GEO_FILE))
+        structure.label = GEO_FILE
+        structure.store()
+        print(f"Created new structure: {structure.pk}")
 
-DATA_DIR = os.path.dirname(os.path.abspath(__file__))
-GEO_FILE = "si_bulk.xyz"
+    builder = Cp2kPhononsWorkChain.get_builder()
 
-
-def _example_cp2k_bulkopt(cp2k_code, cell_opt, mult):
-
-    builder = Cp2kBulkOptWorkChain.get_builder()
-
-    builder.metadata.label = "Cp2kBulkOptWorkChain"
-    builder.metadata.description = "test description"
+    builder.metadata.label = "CP2K_Phonons"
+    builder.metadata.description = "test phonons c2h2"
     builder.code = cp2k_code
-    ase_geom = ase.io.read(os.path.join(DATA_DIR, GEO_FILE))
-    builder.structure = StructureData(ase=ase_geom)
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 1,
+            "num_machines": 3,
             "num_mpiprocs_per_machine": 1,
             "num_cores_per_mpiproc": 1,
         },
     }
-    builder.protocol = Str("debug")
-    if cell_opt:
-        builder.cell_opt = Bool(True)
-        builder.symmetry = Str("ORTHORHOMBIC")
-        builder.cell_freedom = Str("KEEP_SYMMETRY")
-    builder.multiplicity = Int(mult)
-    mag = [0 for i in ase_geom]
-    if mult == 1:
-        mag[0] = 1
-        mag[1] = -1
-        builder.magnetization_per_site = List(mag)
 
-    _, calc_node = run_get_node(builder)
+    dft_params = {
+        "protocol": "debug",
+        "cutoff": 300,
+    }
 
-    assert calc_node.is_finished_ok
+    if uks:
+        magnetization_per_site = [0 for i in range(len(structure.sites))]
+        magnetization_per_site[1] = 1
+        magnetization_per_site[2] = -1
+        dft_params = {
+            "protocol": "debug",
+            "uks": uks,
+            "magnetization_per_site": magnetization_per_site,
+            "charge": 0,
+            "periodic": "XYZ",
+            "vdw": False,
+            "multiplicity": 1,
+            "cutoff": 300,
+        }
+
+    sys_params = {}
+
+    dft_params["periodic"] = "NONE"
+    phonons_params = {"nproc_rep": 1}
+    sys_params["colvars"] = "distance atoms 2 3 , distance atoms 1 2"
+
+    builder.structure = structure
+    builder.dft_params = orm.Dict(dft_params)
+    builder.sys_params = orm.Dict(sys_params)
+    builder.phonons_params = orm.Dict(phonons_params)
 
-    bulkopt_out_dict = dict(calc_node.outputs.output_parameters)
-    print()
-    for k in bulkopt_out_dict:
-        print(f"  {k}: {bulkopt_out_dict[k]}")
+    _, calc_node = engine.run_get_node(builder)
 
+    assert calc_node.is_finished_ok
 
-def example_cp2k_bulkopt_rks(cp2k_code):
-    _example_cp2k_bulkopt(cp2k_code, False, 0)
+    # phonons_out_dict = dict(calc_node.outputs.output_parameters)
+    # print()
+    # for k in phonons_out_dict:
+    #    print(f"  {k}: {phonons_out_dict[k]}")
 
 
-def example_cp2k_cellkopt_rks(cp2k_code):
-    _example_cp2k_bulkopt(cp2k_code, True, 0)
+def example_cp2k_phonons_rks(cp2k_code):
+    _example_cp2k_phonons(cp2k_code, "SlabXY", False)
 
 
-def example_cp2k_cellopt_uks(cp2k_code):
-    _example_cp2k_bulkopt(cp2k_code, True, 1)
+def example_cp2k_phonons_uks(cp2k_code):
+    _example_cp2k_phonons(cp2k_code, "SlabXY", True)
 
 
 if __name__ == "__main__":
-    print("#### Bulk opt  RKS")
-    _example_cp2k_bulkopt(load_code("cp2k@localhost"), False, 0)
-
-    print("#### Cell opt RKS")
-    _example_cp2k_bulkopt(load_code("cp2k@localhost"), True, 0)
+    print("#### ", " RKS")
+    _example_cp2k_phonons(orm.load_code("cp2k@localhost"), False)
 
-    print("#### Cell opt UKS")
-    _example_cp2k_bulkopt(load_code("cp2k@localhost"), True, 1)
+    print("#### ", " UKS")
+    _example_cp2k_phonons(orm.load_code("cp2k@localhost"), True)
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_gw.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_gw.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from aiida.plugins import WorkflowFactory
 from ase import Atoms
 
 Cp2kMoleculeGwWorkChain = WorkflowFactory("nanotech_empa.cp2k.molecule_gw")
 
 
 def _example_cp2k_gw(cp2k_code, ic, protocol, mult):
-
     builder = Cp2kMoleculeGwWorkChain.get_builder()
 
     builder.metadata.label = "Cp2kMoleculeGwWorkChain"
     builder.metadata.description = "test description"
     builder.code = cp2k_code
 
     ase_geom = Atoms("HH", positions=[[0, 0, 0], [0.75, 0, 0]], cell=[4.0, 4.0, 4.0])
@@ -100,15 +99,14 @@
 
 
 def example_cp2k_ic_gapw_hq_uks(cp2k_code):
     _example_cp2k_gw(cp2k_code, True, "gapw_hq", 1)
 
 
 if __name__ == "__main__":
-
     for ic in [False, True]:
         for pc in ["gpw_std", "gapw_std", "gapw_hq"]:
             for mult in [0, 1]:
                 print()
                 print("####################################")
                 print(f"#### ic={ic}; {pc}; mult={mult}")
                 print("####################################")
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_cp2k_mol_opt_gw.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_mol_opt_gw.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from aiida.plugins import WorkflowFactory
 from ase import Atoms
 
 Cp2kMoleculeOptGwWorkChain = WorkflowFactory("nanotech_empa.cp2k.mol_opt_gw")
 
 
 def _example_cp2k_mol_opt_gw(cp2k_code, geo_opt):
-
     builder = Cp2kMoleculeOptGwWorkChain.get_builder()
 
     builder.metadata.description = "H2 gas"
     builder.code = cp2k_code
 
     ase_geom = Atoms("HH", positions=[[0, 0, 0], [0.75, 0, 0]], cell=[4.0, 4.0, 4.0])
     mag_list = [-1, 1]
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_gaussian_casscf.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_casscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 GaussianCasscfSeriesWorkChain = WorkflowFactory("nanotech_empa.gaussian.casscf_series")
 
 DATA_DIR = os.path.dirname(os.path.abspath(__file__))
 OUTPUT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 def _example_gaussian_casscf(gaussian_code, formchk_code, cubegen_code):
-
     ase_geom = ase.io.read(os.path.join(DATA_DIR, "benzene-diradical.xyz"))
     ase_geom.cell = np.diag([10.0, 10.0, 10.0])
 
     builder = GaussianCasscfSeriesWorkChain.get_builder()
     builder.gaussian_code = gaussian_code
     builder.formchk_code = formchk_code
     builder.cubegen_code = cubegen_code
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_gaussian_spin.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_spin.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 GaussianSpinWorkChain = WorkflowFactory("nanotech_empa.gaussian.spin")
 
 DATA_DIR = os.path.dirname(os.path.abspath(__file__))
 OUTPUT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 def _example_gaussian_spin(gaussian_code, formchk_code, cubegen_code):
-
     ase_geom = ase.io.read(os.path.join(DATA_DIR, "benzene-diradical.xyz"))
     ase_geom.cell = np.diag([10.0, 10.0, 10.0])
 
     builder = GaussianSpinWorkChain.get_builder()
     builder.gaussian_code = gaussian_code
     builder.formchk_code = formchk_code
     builder.cubegen_code = cubegen_code
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/example_nanoribbon.py` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_nanoribbon.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     if "spin_density_arraydata" in node.outputs:
         cube = cube_from_qe_pp_arraydata(node.outputs.spin_density_arraydata)
         cube.write_cube_file(os.path.join(OUTPUT_DIR, "spin.cube"))
         print("Wrote spin.cube!")
 
 
 def example_nanoribbon_no_spin(qe_pw_code, qe_pp_code, qe_projwfc_code):
-
     _example_nanoribbon(
         True,
         qe_pw_code,
         qe_pp_code,
         qe_projwfc_code,
         os.path.join(DATA_DIR, "c2h2_no_spin.xyz"),
         "Test calculation no spin",
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_on_au111.xyz`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-38
-Lattice="8.84399664 0.0 0.0 0.0 10.21216768 0.0 0.0 0.0 43.31675909" Properties=species:S:1:pos:R:3:tags:I:1 uhf-sto3g=T pbc="T T T"
-H        4.04838778       5.20767820      16.51675909        1
-H        3.42838778       4.08448949      16.51675909        2
-Au       0.00000000       3.40405590      13.31675909        0
-Au       1.47399944       0.85101397      13.31675909        0
-Au       0.00000000       8.51013974      13.31675909        0
-Au       1.47399944       5.95709781      13.31675909        0
-Au       2.94799888       3.40405590      13.31675909        0
-Au       4.42199832       0.85101397      13.31675909        0
-Au       2.94799888       8.51013974      13.31675909        0
-Au       4.42199832       5.95709781      13.31675909        0
-Au       5.89599776       3.40405590      13.31675909        0
-Au       7.36999720       0.85101397      13.31675909        0
-Au       5.89599776       8.51013974      13.31675909        0
-Au       7.36999720       5.95709781      13.31675909        0
-Au       0.00000000       0.00000000      10.86519004        0
-Au       1.47399944       2.55304192      10.86519004        0
-Au       0.00000000       5.10608384      10.86519004        0
-Au       1.47399944       7.65912576      10.86519004        0
-Au       2.94799888       0.00000000      10.86519004        0
-Au       4.42199832       2.55304192      10.86519004        0
-Au       2.94799888       5.10608384      10.86519004        0
-Au       4.42199832       7.65912576      10.86519004        0
-Au       5.89599776       0.00000000      10.86519004        0
-Au       7.36999720       2.55304192      10.86519004        0
-Au       5.89599776       5.10608384      10.86519004        0
-Au       7.36999720       7.65912576      10.86519004        0
-H        0.00000000       1.70202795      10.00000000        0
-H        1.47399944       4.25506987      10.00000000        0
-H        0.00000000       6.80811179      10.00000000        0
-H        1.47399944       9.36115371      10.00000000        0
-H        2.94799888       1.70202795      10.00000000        0
-H        4.42199832       4.25506987      10.00000000        0
-H        2.94799888       6.80811179      10.00000000        0
-H        4.42199832       9.36115371      10.00000000        0
-H        5.89599776       1.70202795      10.00000000        0
-H        7.36999720       4.25506987      10.00000000        0
-H        5.89599776       6.80811179      10.00000000        0
-H        7.36999720       9.36115371      10.00000000        0
+40
+Lattice="8.84399664 0.0 0.0 0.0 10.21216768 0.0 0.0 0.0 20.0" Properties=species:S:1:pos:R:3:masses:R:1 pbc="T T T"
+H        2.89445002       3.11134486       9.51675909       1.00800000
+C        3.40914678       4.04942122       9.51675909      12.01100000
+C        4.06762878       5.24274647       9.51675909      12.01100000
+H        4.58232554       6.18082283       9.51675909       1.00800000
+Au       0.00000000       3.40405590       6.31675909     196.96656900
+Au       1.47399944       0.85101397       6.31675909     196.96656900
+Au       0.00000000       8.51013974       6.31675909     196.96656900
+Au       1.47399944       5.95709781       6.31675909     196.96656900
+Au       2.94799888       3.40405590       6.31675909     196.96656900
+Au       4.42199832       0.85101397       6.31675909     196.96656900
+Au       2.94799888       8.51013974       6.31675909     196.96656900
+Au       4.42199832       5.95709781       6.31675909     196.96656900
+Au       5.89599776       3.40405590       6.31675909     196.96656900
+Au       7.36999720       0.85101397       6.31675909     196.96656900
+Au       5.89599776       8.51013974       6.31675909     196.96656900
+Au       7.36999720       5.95709781       6.31675909     196.96656900
+Au       0.00000000       0.00000000       3.86519004     196.96656900
+Au       1.47399944       2.55304192       3.86519004     196.96656900
+Au       0.00000000       5.10608384       3.86519004     196.96656900
+Au       1.47399944       7.65912576       3.86519004     196.96656900
+Au       2.94799888       0.00000000       3.86519004     196.96656900
+Au       4.42199832       2.55304192       3.86519004     196.96656900
+Au       2.94799888       5.10608384       3.86519004     196.96656900
+Au       4.42199832       7.65912576       3.86519004     196.96656900
+Au       5.89599776       0.00000000       3.86519004     196.96656900
+Au       7.36999720       2.55304192       3.86519004     196.96656900
+Au       5.89599776       5.10608384       3.86519004     196.96656900
+Au       7.36999720       7.65912576       3.86519004     196.96656900
+H        0.00000000       1.70202795       3.00000000       1.00800000
+H        1.47399944       4.25506987       3.00000000       1.00800000
+H        0.00000000       6.80811179       3.00000000       1.00800000
+H        1.47399944       9.36115371       3.00000000       1.00800000
+H        2.94799888       1.70202795       3.00000000       1.00800000
+H        4.42199832       4.25506987       3.00000000       1.00800000
+H        2.94799888       6.80811179       3.00000000       1.00800000
+H        4.42199832       9.36115371       3.00000000       1.00800000
+H        5.89599776       1.70202795       3.00000000       1.00800000
+H        7.36999720       4.25506987       3.00000000       1.00800000
+H        5.89599776       6.80811179       3.00000000       1.00800000
+H        7.36999720       9.36115371       3.00000000       1.00800000
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/h2_on_hbn.xyz` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_hbn.xyz`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 18
 Lattice="5.021998126 0.0 0.0 0.0 4.34917796 0.0 0.0 0.0 12.0" Properties=species:S:1:pos:R:3:tags:I:1:masses:R:1 pbc="T T T"
-H        2.52851027       3.96611323       6.60565171        0       1.00800000
-H        2.51592826       4.76539961       6.57251428        0       1.00800000
-N        0.00000000       2.89945197       3.42144871        0      14.00700000
-B        1.25549953       3.62431496       3.42144871        0      10.81000000
-N        1.25549953       5.07404095       3.42144871        0      14.00700000
-B        0.00000000       5.79890394       3.42144871        0      10.81000000
-N        2.51099906       2.89945197       3.42144871        0      14.00700000
-B        3.76649859       3.62431496       3.42144871        0      10.81000000
-N        3.76649859       5.07404095       3.42144871        0      14.00700000
-B        2.51099906       5.79890394       3.42144871        0      10.81000000
-B        0.00000000       2.89945197       0.00000000        0      10.81000000
-N        1.25549953       3.62431496       0.00000000        0      14.00700000
-B        1.25549953       5.07404095       0.00000000        0      10.81000000
-N        0.00000000       5.79890394       0.00000000        0      14.00700000
-B        2.51099906       2.89945197       0.00000000        0      10.81000000
-N        3.76649859       3.62431496       0.00000000        0      14.00700000
-B        3.76649859       5.07404095       0.00000000        0      10.81000000
-N        2.51099906       5.79890394       0.00000000        0      14.00700000
+H        2.52851027       1.96611323       6.60565171        0       1.00800000
+H        2.51592826       2.76539961       6.57251428        0       1.00800000
+N        0.00000000       0.89945197       3.42144871        0      14.00700000
+B        1.25549953       1.62431496       3.42144871        0      10.81000000
+N        1.25549953       3.07404095       3.42144871        0      14.00700000
+B        0.00000000       3.79890394       3.42144871        0      10.81000000
+N        2.51099906       0.89945197       3.42144871        0      14.00700000
+B        3.76649859       1.62431496       3.42144871        0      10.81000000
+N        3.76649859       3.07404095       3.42144871        0      14.00700000
+B        2.51099906       3.79890394       3.42144871        0      10.81000000
+B        0.00000000       0.89945197       0.00000000        0      10.81000000
+N        1.25549953       1.62431496       0.00000000        0      14.00700000
+B        1.25549953       2.07404095       0.00000000        0      10.81000000
+N        0.00000000       2.79890394       0.00000000        0      14.00700000
+B        2.51099906       0.89945197       0.00000000        0      10.81000000
+N        3.76649859       1.62431496       0.00000000        0      14.00700000
+B        3.76649859       3.07404095       0.00000000        0      10.81000000
+N        2.51099906       3.79890394       0.00000000        0      14.00700000
```

### Comparing `aiida-nanotech-empa-1.0.0a0/examples/workflows/si_bulk.xyz` & `aiida_nanotech_empa-1.0.0b0/examples/workflows/si_bulk.xyz`

 * *Files identical despite different names*

### Comparing `aiida-nanotech-empa-1.0.0a0/pyproject.toml` & `aiida_nanotech_empa-1.0.0b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "aiida-core>=2.0.0,<3.0.0",
-    "aiida-quantumespresso>=4.1.0",
-    "aiida-pseudo>=0.8.0",
-    "aiida-cp2k>=2.0.0b0",
-    "ase",
-    "aiida-gaussian>=2.0.0",
+    "aiida-core~=2.2",
+    "aiida-quantumespresso~=4.1",
+    "aiida-pseudo~=1.0",
+    "aiida-cp2k~=2.0",
+    "ase~=3.21",
+    "aiida-gaussian~=2.0",
     "pillow>=8.0.0",
     "more-itertools",
 ]
 
 [project.urls]
 Homepage = "https://github.com/nanotech-empa/aiida-nanotech-empa"
 
@@ -43,43 +43,58 @@
     "pytest-cov",
     "pre-commit>=2.19",
     "bumpver==2022.1119",
     "coverage",
 ]
 
 [project.entry-points."aiida.parsers"]
-"nanotech_empa.pp" = "aiida_nanotech_empa.parsers.pp_parser:PpParser"
-"nanotech_empa.cp2k_gw_parser" = "aiida_nanotech_empa.parsers.cp2k_gw_parser:Cp2kGWParser"
+"nanotech_empa.pp" = "aiida_nanotech_empa.parsers:PpParser"
+"nanotech_empa.cp2k_gw_parser" = "aiida_nanotech_empa.parsers:Cp2kGwParser"
+"nanotech_empa.cp2k_neb_parser" = "aiida_nanotech_empa.parsers:Cp2kNebParser"
 "nanotech_empa.gaussian.cubegen_pymol" = "aiida_nanotech_empa.parsers.cubegen_pymol_parser:CubegenPymolParser"
-"nanotech_empa.gaussian.casscf" = "aiida_nanotech_empa.parsers.gaussian_casscf_parser:GaussianCasscfParser"
+"nanotech_empa.gaussian.casscf" = "aiida_nanotech_empa.parsers:GaussianCasscfParser"
+
+[project.entry-points."aiida.calculations"]
+"nanotech_empa.stm" = "aiida_nanotech_empa.plugins:StmCalculation"
+"nanotech_empa.overlap" = "aiida_nanotech_empa.plugins:OverlapCalculation"
+"nanotech_empa.afm" = "aiida_nanotech_empa.plugins:AfmCalculation"
+"nanotech_empa.hrstm" = "aiida_nanotech_empa.plugins:HrstmCalculation"
 
 [project.entry-points."aiida.workflows"]
-"nanotech_empa.nanoribbon" = "aiida_nanotech_empa.workflows.qe.nanoribbon:NanoribbonWorkChain"
+"nanotech_empa.nanoribbon" = "aiida_nanotech_empa.workflows.qe:NanoribbonWorkChain"
 "nanotech_empa.gaussian.scf" = "aiida_nanotech_empa.workflows.gaussian:GaussianScfWorkChain"
 "nanotech_empa.gaussian.relax" = "aiida_nanotech_empa.workflows.gaussian:GaussianRelaxWorkChain"
 "nanotech_empa.gaussian.delta_scf" = "aiida_nanotech_empa.workflows.gaussian:GaussianDeltaScfWorkChain"
 "nanotech_empa.gaussian.natorb" = "aiida_nanotech_empa.workflows.gaussian:GaussianNatOrbWorkChain"
 "nanotech_empa.gaussian.spin" = "aiida_nanotech_empa.workflows.gaussian:GaussianSpinWorkChain"
 "nanotech_empa.gaussian.hf_mp2" = "aiida_nanotech_empa.workflows.gaussian:GaussianHfMp2WorkChain"
 "nanotech_empa.gaussian.constr_opt_chain" = "aiida_nanotech_empa.workflows.gaussian:GaussianConstrOptChainWorkChain"
 "nanotech_empa.gaussian.casscf" = "aiida_nanotech_empa.workflows.gaussian:GaussianCasscfWorkChain"
 "nanotech_empa.gaussian.casscf_series" = "aiida_nanotech_empa.workflows.gaussian:GaussianCasscfSeriesWorkChain"
-"nanotech_empa.cp2k.molecule_opt" = "aiida_nanotech_empa.workflows.cp2k.molecule_opt_workchain:Cp2kMoleculeOptWorkChain"
-"nanotech_empa.cp2k.slab_opt" = "aiida_nanotech_empa.workflows.cp2k.slab_opt_workchain:Cp2kSlabOptWorkChain"
-"nanotech_empa.cp2k.bulk_opt" = "aiida_nanotech_empa.workflows.cp2k.bulk_opt_workchain:Cp2kBulkOptWorkChain"
-"nanotech_empa.cp2k.molecule_gw" = "aiida_nanotech_empa.workflows.cp2k.molecule_gw_workchain:Cp2kMoleculeGwWorkChain"
-"nanotech_empa.cp2k.fragment_separation" = "aiida_nanotech_empa.workflows.cp2k.fragment_separation:Cp2kFragmentSeparationWorkChain"
-"nanotech_empa.cp2k.ads_gw_ic" = "aiida_nanotech_empa.workflows.cp2k.adsorbed_gw_ic_workchain:Cp2kAdsorbedGwIcWorkChain"
-"nanotech_empa.cp2k.mol_opt_gw" = "aiida_nanotech_empa.workflows.cp2k.molecule_opt_gw_workchain:Cp2kMoleculeOptGwWorkChain"
+"nanotech_empa.cp2k.geo_opt" = "aiida_nanotech_empa.workflows.cp2k:Cp2kGeoOptWorkChain"
+"nanotech_empa.cp2k.fragment_separation" = "aiida_nanotech_empa.workflows.cp2k:Cp2kFragmentSeparationWorkChain"
+"nanotech_empa.cp2k.ads_gw_ic" = "aiida_nanotech_empa.workflows.cp2k:Cp2kAdsorbedGwIcWorkChain"
+"nanotech_empa.cp2k.molecule_gw" = "aiida_nanotech_empa.workflows.cp2k:Cp2kMoleculeGwWorkChain"
+"nanotech_empa.cp2k.mol_opt_gw" = "aiida_nanotech_empa.workflows.cp2k:Cp2kMoleculeOptGwWorkChain"
+"nanotech_empa.cp2k.pdos" = "aiida_nanotech_empa.workflows.cp2k:Cp2kPdosWorkChain"
+"nanotech_empa.cp2k.orbitals" = "aiida_nanotech_empa.workflows.cp2k:Cp2kOrbitalsWorkChain"
+"nanotech_empa.cp2k.stm" = "aiida_nanotech_empa.workflows.cp2k:Cp2kStmWorkChain"
+"nanotech_empa.cp2k.afm" = "aiida_nanotech_empa.workflows.cp2k:Cp2kAfmWorkChain"
+"nanotech_empa.cp2k.hrstm" = "aiida_nanotech_empa.workflows.cp2k:Cp2kHrstmWorkChain"
+"nanotech_empa.cp2k.diag" = "aiida_nanotech_empa.workflows.cp2k:Cp2kDiagWorkChain"
+"nanotech_empa.cp2k.replica" = "aiida_nanotech_empa.workflows.cp2k:Cp2kReplicaWorkChain"
+"nanotech_empa.cp2k.neb" = "aiida_nanotech_empa.workflows.cp2k:Cp2kNebWorkChain"
+"nanotech_empa.cp2k.phonons" = "aiida_nanotech_empa.workflows.cp2k:Cp2kPhononsWorkChain"
+
 
 [project.entry-points."aiida.schedulers"]
-lsf_ethz_euler = "aiida_nanotech_empa.schedulers.lsf_ethz_euler:ETHZEulerLsfScheduler"
+slurm_ethz_euler = "aiida_nanotech_empa.schedulers:ETHZEulerSlurmScheduler"
 
 [tool.bumpver]
-current_version = "v1.0.0a0"
+current_version = "v1.0.0b0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}."
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `aiida-nanotech-empa-1.0.0a0/PKG-INFO` & `aiida_nanotech_empa-1.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aiida-nanotech-empa
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: AiiDA plugins and workflows developed at nanotech@surfaces group from Empa.
 Author: nanotech@surfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: aiida-core>=2.0.0,<3.0.0
-Requires-Dist: aiida-quantumespresso>=4.1.0
-Requires-Dist: aiida-pseudo>=0.8.0
-Requires-Dist: aiida-cp2k>=2.0.0b0
-Requires-Dist: ase
-Requires-Dist: aiida-gaussian>=2.0.0
+Requires-Dist: aiida-core~=2.2
+Requires-Dist: aiida-quantumespresso~=4.1
+Requires-Dist: aiida-pseudo~=1.0
+Requires-Dist: aiida-cp2k~=2.0
+Requires-Dist: ase~=3.21
+Requires-Dist: aiida-gaussian~=2.0
 Requires-Dist: pillow>=8.0.0
 Requires-Dist: more-itertools
 Requires-Dist: pgtest~=1.3.1 ; extra == "dev"
 Requires-Dist: pytest~=6.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit>=2.19 ; extra == "dev"
 Requires-Dist: bumpver==2022.1119 ; extra == "dev"
```

