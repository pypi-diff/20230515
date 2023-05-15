# Comparing `tmp/FAST-OAD-CS25-0.2.0.tar.gz` & `tmp/fast_oad_cs25-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAST-OAD-CS25-0.2.0.tar", max compression
+gzip compressed data, was "fast_oad_cs25-0.3.0.tar", max compression
```

## Comparing `FAST-OAD-CS25-0.2.0.tar` & `fast_oad_cs25-0.3.0.tar`

### file list

```diff
@@ -1,213 +1,216 @@
--rw-r--r--   0        0        0    35149 2023-02-08 16:03:07.826153 FAST-OAD-CS25-0.2.0/LICENSE
--rw-r--r--   0        0        0     2292 2023-02-08 16:03:07.826153 FAST-OAD-CS25-0.2.0/README.md
--rw-r--r--   0        0        0     3112 2023-02-08 16:03:15.594129 FAST-OAD-CS25-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/__init__.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/configurations/__init__.py
--rw-r--r--   0        0        0     2460 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/configurations/cs25_base.yaml
--rw-r--r--   0        0        0      906 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/__init__.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/__init__.py
--rw-r--r--   0        0        0     2984 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_high_speed.py
--rw-r--r--   0        0        0     7117 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_landing.py
--rw-r--r--   0        0        0     3286 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_low_speed.py
--rw-r--r--   0        0        0     1758 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_takeoff.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/__init__.py
--rw-r--r--   0        0        0     2636 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0.py
--rw-r--r--   0        0        0     4299 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_fuselage.py
--rw-r--r--   0        0        0     3824 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_ht.py
--rw-r--r--   0        0        0     4936 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_nacelles_pylons.py
--rw-r--r--   0        0        0     5654 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_total.py
--rw-r--r--   0        0        0     3702 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_vt.py
--rw-r--r--   0        0        0     4097 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_wing.py
--rw-r--r--   0        0        0     3737 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd_compressibility.py
--rw-r--r--   0        0        0     2495 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd_trim.py
--rw-r--r--   0        0        0     2775 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_alpha.py
--rw-r--r--   0        0        0     4340 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_cl_alpha.py
--rw-r--r--   0        0        0     2091 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_max_cl_landing.py
--rw-r--r--   0        0        0     8702 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_polar.py
--rw-r--r--   0        0        0     2524 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_reynolds.py
--rw-r--r--   0        0        0    11130 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/high_lift_aero.py
--rw-r--r--   0        0        0     2728 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/initialize_cl.py
--rw-r--r--   0        0        0     5792 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/oswald.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/resources/__init__.py
--rw-r--r--   0        0        0     2590 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/resources/interpolation of lift effectiveness.txt
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/utils/__init__.py
--rw-r--r--   0        0        0     3153 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/utils/cd0_lifting_surface.py
--rw-r--r--   0        0        0     1146 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/utils/friction_drag.py
--rw-r--r--   0        0        0     2265 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/constants.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/__init__.py
--rw-r--r--   0        0        0      757 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/__init__.py
--rw-r--r--   0        0        0     2222 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/BACJ.txt
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.830153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/__init__.py
--rw-r--r--   0        0        0      124 2023-02-08 16:03:07.834153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/polar_session.txt
--rw-r--r--   0        0        0        0 2023-02-08 16:03:07.834153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/Xfoil699src.zip
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.834153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/__init__.py
--rw-r--r--   0        0        0   480337 2023-02-08 16:03:07.838153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pplot.exe
--rw-r--r--   0        0        0   450687 2023-02-08 16:03:07.838153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pxplot.exe
--rw-r--r--   0        0        0  1002125 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/xfoil.exe
--rw-r--r--   0        0        0    10688 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil_polar.py
--rw-r--r--   0        0        0      867 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/constants.py
--rw-r--r--   0        0        0      763 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/__init__.py
--rw-r--r--   0        0        0     3984 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/compute_aero_center.py
--rw-r--r--   0        0        0     1386 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/constants.py
--rw-r--r--   0        0        0      756 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/__init__.py
--rw-r--r--   0        0        0     2801 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/compute_wetted_area.py
--rw-r--r--   0        0        0      754 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/__init__.py
--rw-r--r--   0        0        0     2858 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_cnbeta_fuselage.py
--rw-r--r--   0        0        0    12898 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_fuselage.py
--rw-r--r--   0        0        0      770 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/__init__.py
--rw-r--r--   0        0        0      973 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/__init__.py
--rw-r--r--   0        0        0     2557 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_chords.py
--rw-r--r--   0        0        0     2276 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_cl_alpha.py
--rw-r--r--   0        0        0     3654 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_mac.py
--rw-r--r--   0        0        0     3090 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_sweep.py
--rw-r--r--   0        0        0     1491 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/compute_horizontal_tail.py
--rw-r--r--   0        0        0      755 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/__init__.py
--rw-r--r--   0        0        0    10014 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/compute_nacelle_pylons.py
--rw-r--r--   0        0        0      768 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/__init__.py
--rw-r--r--   0        0        0     1022 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/__init__.py
--rw-r--r--   0        0        0     2448 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_chords.py
--rw-r--r--   0        0        0     2507 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_clalpha.py
--rw-r--r--   0        0        0     2183 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_distance.py
--rw-r--r--   0        0        0     3318 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_mac.py
--rw-r--r--   0        0        0     2996 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_sweep.py
--rw-r--r--   0        0        0     1871 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/compute_vertical_tail.py
--rw-r--r--   0        0        0      750 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/__init__.py
--rw-r--r--   0        0        0      763 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/__init__.py
--rw-r--r--   0        0        0     2175 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_b_50.py
--rw-r--r--   0        0        0     2888 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l1_l4.py
--rw-r--r--   0        0        0     3946 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l2_l3.py
--rw-r--r--   0        0        0     5186 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mac_wing.py
--rw-r--r--   0        0        0     1986 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mfw.py
--rw-r--r--   0        0        0     4200 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_sweep_wing.py
--rw-r--r--   0        0        0     2707 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_toc_wing.py
--rw-r--r--   0        0        0     2518 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_wet_area_wing.py
--rw-r--r--   0        0        0     3411 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_x_wing.py
--rw-r--r--   0        0        0     3085 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_y_wing.py
--rw-r--r--   0        0        0     2363 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/compute_wing.py
--rw-r--r--   0        0        0     3509 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geometry.py
--rw-r--r--   0        0        0      750 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/__init__.py
--rw-r--r--   0        0        0     8348 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/profile.py
--rw-r--r--   0        0        0     1713 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/profile_getter.py
--rw-r--r--   0        0        0     2222 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/BACJ.txt
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/__init__.py
--rw-r--r--   0        0        0     2790 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_11.txt
--rw-r--r--   0        0        0     2789 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_12.txt
--rw-r--r--   0        0        0     2789 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_15.txt
--rw-r--r--   0        0        0     1017 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/naca23012.txt
--rw-r--r--   0        0        0     2995 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/wing_global_positions.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.846153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/__init__.py
--rw-r--r--   0        0        0     1950 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/compute_static_margin.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/__init__.py
--rw-r--r--   0        0        0     5858 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_ht_area.py
--rw-r--r--   0        0        0     1619 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_tail_areas.py
--rw-r--r--   0        0        0     3676 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_vt_area.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/loops/__init__.py
--rw-r--r--   0        0        0     5303 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/loops/compute_wing_area.py
--rw-r--r--   0        0        0     2413 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/loops/compute_wing_position.py
--rw-r--r--   0        0        0      753 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/__init__.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/__init__.py
--rw-r--r--   0        0        0      933 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/__init__.py
--rw-r--r--   0        0        0     2178 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/constants.py
--rw-r--r--   0        0        0      906 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/exceptions.py
--rw-r--r--   0        0        0     6949 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/openmdao.py
--rw-r--r--   0        0        0    22127 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/rubber_engine.py
--rw-r--r--   0        0        0    39322 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/variable_descriptions.txt
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/__init__.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/__init__.py
--rw-r--r--   0        0        0     3863 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg.py
--rw-r--r--   0        0        0      755 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/__init__.py
--rw-r--r--   0        0        0     3958 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_control_surfaces.py
--rw-r--r--   0        0        0    13057 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_others.py
--rw-r--r--   0        0        0     7279 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_ratio_aft.py
--rw-r--r--   0        0        0    10938 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_tanks.py
--rw-r--r--   0        0        0     5735 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_wing.py
--rw-r--r--   0        0        0     1651 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_global_cg.py
--rw-r--r--   0        0        0     3224 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_ht_cg.py
--rw-r--r--   0        0        0     1946 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_max_cg_ratio.py
--rw-r--r--   0        0        0     3141 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_vt_cg.py
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/__init__.py
--rw-r--r--   0        0        0     1478 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase1.py
--rw-r--r--   0        0        0     1552 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase2.py
--rw-r--r--   0        0        0     1480 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase3.py
--rw-r--r--   0        0        0     1478 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase4.py
--rw-r--r--   0        0        0     4513 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase_base.py
--rw-r--r--   0        0        0     3280 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcases.py
--rw-r--r--   0        0        0     2442 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/update_mlg.py
--rw-r--r--   0        0        0     1261 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/constants.py
--rw-r--r--   0        0        0      860 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/constants.py
--rw-r--r--   0        0        0      811 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/__init__.py
--rw-r--r--   0        0        0     1143 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/__init__.py
--rw-r--r--   0        0        0     7147 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a1_wing_weight.py
--rw-r--r--   0        0        0     2961 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a2_fuselage_weight.py
--rw-r--r--   0        0        0     3329 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a3_empennage_weight.py
--rw-r--r--   0        0        0     2850 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a4_flight_control_weight.py
--rw-r--r--   0        0        0     2393 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a5_landing_gear_weight.py
--rw-r--r--   0        0        0     2713 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a6_pylons_weight.py
--rw-r--r--   0        0        0     2001 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a7_paint_weight.py
--rw-r--r--   0        0        0     1166 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/constants.py
--rw-r--r--   0        0        0     3330 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/sum.py
--rw-r--r--   0        0        0      921 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/__init__.py
--rw-r--r--   0        0        0     2333 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b1_engine_weight.py
--rw-r--r--   0        0        0     2349 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b2_fuel_lines_weight.py
--rw-r--r--   0        0        0     2234 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b3_unconsumables_weight.py
--rw-r--r--   0        0        0      949 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/constants.py
--rw-r--r--   0        0        0     2213 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/sum.py
--rw-r--r--   0        0        0     1175 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/__init__.py
--rw-r--r--   0        0        0     4224 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c1_power_systems_weight.py
--rw-r--r--   0        0        0     9037 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c2_life_support_systems_weight.py
--rw-r--r--   0        0        0     2675 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c3_navigation_systems_weight.py
--rw-r--r--   0        0        0     2354 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c4_transmissions_systems_weight.py
--rw-r--r--   0        0        0     3577 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c5_fixed_operational_systems_weight.py
--rw-r--r--   0        0        0     2160 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c6_flight_kit_weight.py
--rw-r--r--   0        0        0     1172 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/constants.py
--rw-r--r--   0        0        0     3735 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/sum.py
--rw-r--r--   0        0        0     1109 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/constants.py
--rw-r--r--   0        0        0     4971 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/cs25.py
--rw-r--r--   0        0        0     1047 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/__init__.py
--rw-r--r--   0        0        0     1095 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/constants.py
--rw-r--r--   0        0        0     2772 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d1_cargo_configuration_weight.py
--rw-r--r--   0        0        0     2399 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d2_passenger_seats_weight.py
--rw-r--r--   0        0        0     2005 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d3_food_water_weight.py
--rw-r--r--   0        0        0     2041 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d4_security_kit_weight.py
--rw-r--r--   0        0        0     2358 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d5_toilets_weight.py
--rw-r--r--   0        0        0     2467 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/sum.py
--rw-r--r--   0        0        0      801 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/__init__.py
--rw-r--r--   0        0        0     1784 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/crew_weight.py
--rw-r--r--   0        0        0     4207 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/mass_breakdown.py
--rw-r--r--   0        0        0     2264 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/payload.py
--rw-r--r--   0        0        0     1767 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/update_mlw_and_mzfw.py
--rw-r--r--   0        0        0     2393 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/weight.py
--rw-r--r--   0        0        0       35 2023-02-08 16:03:07.850153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/.gitignore
--rw-r--r--   0        0        0    16246 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/01_tutorial.ipynb
--rw-r--r--   0        0        0     8609 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/02_postprocessing.ipynb
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/__init__.py
--rw-r--r--   0        0        0   129349 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/data/CeRAS01_baseline.xml
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/data/__init__.py
--rw-r--r--   0        0        0     2457 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/data/oad_process_timestep_mission.yml
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/__init__.py
--rw-r--r--   0        0        0    18684 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0    23022 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-onera.png
--rw-r--r--   0        0        0    19493 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/user_files_arch.svg
--rw-r--r--   0        0        0   266366 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/variable_viewer_change_range.gif
--rw-r--r--   0        0        0    20214 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/CeRAS_case_study.ipynb
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/__init__.py
--rw-r--r--   0        0        0     4251 2023-02-08 16:03:07.854153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/ceras_utils.py
--rw-r--r--   0        0        0  2020992 2023-02-08 16:03:07.866153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionDesign_R4630_PL17000_out.csv
--rw-r--r--   0        0        0  2147719 2023-02-08 16:03:07.878153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R5093_PL13608_out.csv
--rw-r--r--   0        0        0  1285241 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R926_PL13608_out.csv
--rw-r--r--   0        0        0     8645 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_data_for_plots.xml
--rw-r--r--   0        0        0     4185 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_missions.yml
--rw-r--r--   0        0        0   137335 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_reference_data.xml
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/__init__.py
--rw-r--r--   0        0        0     1446 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing.yml
--rw-r--r--   0        0        0   107154 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing_out.xml
--rw-r--r--   0        0        0     1152 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/operational_missions.yml
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/__init__.py
--rw-r--r--   0        0        0    18684 2023-02-08 16:03:07.886153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0    23022 2023-02-08 16:03:07.890153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-onera.png
--rw-r--r--   0        0        0   124900 2023-02-08 16:03:07.890153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_1.png
--rw-r--r--   0        0        0   147435 2023-02-08 16:03:07.890153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_2.png
--rw-r--r--   0        0        0    83712 2023-02-08 16:03:07.890153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/wing_parameters.png
--rw-r--r--   0        0        0      714 2023-02-08 16:03:07.890153 FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/__init__.py
--rw-r--r--   0        0        0     5531 2023-02-08 16:03:18.004992 FAST-OAD-CS25-0.2.0/setup.py
--rw-r--r--   0        0        0     3646 2023-02-08 16:03:18.005371 FAST-OAD-CS25-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2292 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/README.md
+-rw-r--r--   0        0        0     3343 2023-05-15 10:25:34.405137 fast_oad_cs25-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/configurations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/configurations/cs25_base.yaml
+-rw-r--r--   0        0        0      906 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/__init__.py
+-rw-r--r--   0        0        0     2984 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_high_speed.py
+-rw-r--r--   0        0        0     7117 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_landing.py
+-rw-r--r--   0        0        0     3286 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_low_speed.py
+-rw-r--r--   0        0        0     1758 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_takeoff.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/__init__.py
+-rw-r--r--   0        0        0     2636 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0.py
+-rw-r--r--   0        0        0     4299 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_fuselage.py
+-rw-r--r--   0        0        0     3824 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_ht.py
+-rw-r--r--   0        0        0     4936 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_nacelles_pylons.py
+-rw-r--r--   0        0        0     5654 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_total.py
+-rw-r--r--   0        0        0     3702 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_vt.py
+-rw-r--r--   0        0        0     4097 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_wing.py
+-rw-r--r--   0        0        0     3737 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd_compressibility.py
+-rw-r--r--   0        0        0     2495 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd_trim.py
+-rw-r--r--   0        0        0     2775 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_alpha.py
+-rw-r--r--   0        0        0     4370 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_cl_alpha.py
+-rw-r--r--   0        0        0     2091 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_max_cl_landing.py
+-rw-r--r--   0        0        0     8702 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_polar.py
+-rw-r--r--   0        0        0     2524 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_reynolds.py
+-rw-r--r--   0        0        0    11130 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/high_lift_aero.py
+-rw-r--r--   0        0        0     2728 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/initialize_cl.py
+-rw-r--r--   0        0        0     5792 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/oswald.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/resources/__init__.py
+-rw-r--r--   0        0        0     2590 2023-05-15 10:25:19.781349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/resources/interpolation of lift effectiveness.txt
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/utils/__init__.py
+-rw-r--r--   0        0        0     3153 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/utils/cd0_lifting_surface.py
+-rw-r--r--   0        0        0     1146 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/utils/friction_drag.py
+-rw-r--r--   0        0        0     2265 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/constants.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/__init__.py
+-rw-r--r--   0        0        0      757 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/__init__.py
+-rw-r--r--   0        0        0     2222 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/BACJ.txt
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/polar_session.txt
+-rw-r--r--   0        0        0        0 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/Xfoil699src.zip
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.785349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/__init__.py
+-rw-r--r--   0        0        0   480337 2023-05-15 10:25:19.789349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pplot.exe
+-rw-r--r--   0        0        0   450687 2023-05-15 10:25:19.789349 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pxplot.exe
+-rw-r--r--   0        0        0  1002125 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/xfoil.exe
+-rw-r--r--   0        0        0    10688 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil_polar.py
+-rw-r--r--   0        0        0      867 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/constants.py
+-rw-r--r--   0        0        0      763 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/__init__.py
+-rw-r--r--   0        0        0     4036 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/compute_aero_center.py
+-rw-r--r--   0        0        0     1386 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/constants.py
+-rw-r--r--   0        0        0      756 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/__init__.py
+-rw-r--r--   0        0        0     2801 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/compute_wetted_area.py
+-rw-r--r--   0        0        0      754 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/__init__.py
+-rw-r--r--   0        0        0     2858 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_cnbeta_fuselage.py
+-rw-r--r--   0        0        0    12898 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_fuselage.py
+-rw-r--r--   0        0        0      770 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/__init__.py
+-rw-r--r--   0        0        0      973 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/__init__.py
+-rw-r--r--   0        0        0     2557 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_chords.py
+-rw-r--r--   0        0        0     2291 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_cl_alpha.py
+-rw-r--r--   0        0        0     3654 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_mac.py
+-rw-r--r--   0        0        0     3090 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_sweep.py
+-rw-r--r--   0        0        0     1491 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/compute_horizontal_tail.py
+-rw-r--r--   0        0        0      755 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/__init__.py
+-rw-r--r--   0        0        0    10014 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/compute_nacelle_pylons.py
+-rw-r--r--   0        0        0      768 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_chords.py
+-rw-r--r--   0        0        0     2522 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_clalpha.py
+-rw-r--r--   0        0        0     2183 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_distance.py
+-rw-r--r--   0        0        0     3318 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_mac.py
+-rw-r--r--   0        0        0     2996 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_sweep.py
+-rw-r--r--   0        0        0     1871 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/compute_vertical_tail.py
+-rw-r--r--   0        0        0      750 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/__init__.py
+-rw-r--r--   0        0        0     2175 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_b_50.py
+-rw-r--r--   0        0        0     2888 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l1_l4.py
+-rw-r--r--   0        0        0     3946 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l2_l3.py
+-rw-r--r--   0        0        0     5186 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mac_wing.py
+-rw-r--r--   0        0        0     1986 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mfw.py
+-rw-r--r--   0        0        0     4200 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_sweep_wing.py
+-rw-r--r--   0        0        0     2707 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_toc_wing.py
+-rw-r--r--   0        0        0     2518 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_wet_area_wing.py
+-rw-r--r--   0        0        0     3411 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_x_wing.py
+-rw-r--r--   0        0        0     3085 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_y_wing.py
+-rw-r--r--   0        0        0     2363 2023-05-15 10:25:19.797350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/compute_wing.py
+-rw-r--r--   0        0        0     3509 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geometry.py
+-rw-r--r--   0        0        0      750 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/__init__.py
+-rw-r--r--   0        0        0     8348 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/profile.py
+-rw-r--r--   0        0        0     1713 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/profile_getter.py
+-rw-r--r--   0        0        0     2222 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/BACJ.txt
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/__init__.py
+-rw-r--r--   0        0        0     2790 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_11.txt
+-rw-r--r--   0        0        0     2789 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_12.txt
+-rw-r--r--   0        0        0     2789 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_15.txt
+-rw-r--r--   0        0        0     1017 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/naca23012.txt
+-rw-r--r--   0        0        0     2995 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/wing_global_positions.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/__init__.py
+-rw-r--r--   0        0        0     1950 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/compute_static_margin.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/__init__.py
+-rw-r--r--   0        0        0     5858 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_ht_area.py
+-rw-r--r--   0        0        0     1619 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_tail_areas.py
+-rw-r--r--   0        0        0     3691 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_vt_area.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/__init__.py
+-rw-r--r--   0        0        0     3715 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/compute_wing_area.py
+-rw-r--r--   0        0        0     2413 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/compute_wing_position.py
+-rw-r--r--   0        0        0     1045 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/constants.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/wing_area_component/__init__.py
+-rw-r--r--   0        0        0     5539 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/wing_area_component/update_wing_area_aero.py
+-rw-r--r--   0        0        0     5404 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/wing_area_component/update_wing_area_geom.py
+-rw-r--r--   0        0        0      753 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/__init__.py
+-rw-r--r--   0        0        0      933 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/__init__.py
+-rw-r--r--   0        0        0     2178 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/constants.py
+-rw-r--r--   0        0        0      906 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/exceptions.py
+-rw-r--r--   0        0        0     6949 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/openmdao.py
+-rw-r--r--   0        0        0    22127 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/rubber_engine.py
+-rw-r--r--   0        0        0    39322 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/variable_descriptions.txt
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/__init__.py
+-rw-r--r--   0        0        0     3863 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg.py
+-rw-r--r--   0        0        0      755 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/__init__.py
+-rw-r--r--   0        0        0     3958 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_control_surfaces.py
+-rw-r--r--   0        0        0    13057 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_others.py
+-rw-r--r--   0        0        0     7279 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_ratio_aft.py
+-rw-r--r--   0        0        0    10938 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_tanks.py
+-rw-r--r--   0        0        0     5735 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_wing.py
+-rw-r--r--   0        0        0     1651 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_global_cg.py
+-rw-r--r--   0        0        0     3224 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_ht_cg.py
+-rw-r--r--   0        0        0     1946 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_max_cg_ratio.py
+-rw-r--r--   0        0        0     3141 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_vt_cg.py
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/__init__.py
+-rw-r--r--   0        0        0     1478 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase1.py
+-rw-r--r--   0        0        0     1552 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase2.py
+-rw-r--r--   0        0        0     1480 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase3.py
+-rw-r--r--   0        0        0     1478 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase4.py
+-rw-r--r--   0        0        0     4513 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase_base.py
+-rw-r--r--   0        0        0     3280 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcases.py
+-rw-r--r--   0        0        0     2442 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/update_mlg.py
+-rw-r--r--   0        0        0     1261 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/constants.py
+-rw-r--r--   0        0        0      860 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/constants.py
+-rw-r--r--   0        0        0      811 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/__init__.py
+-rw-r--r--   0        0        0     1143 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/__init__.py
+-rw-r--r--   0        0        0     7147 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a1_wing_weight.py
+-rw-r--r--   0        0        0     2961 2023-05-15 10:25:19.801350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a2_fuselage_weight.py
+-rw-r--r--   0        0        0     3329 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a3_empennage_weight.py
+-rw-r--r--   0        0        0     2850 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a4_flight_control_weight.py
+-rw-r--r--   0        0        0     2393 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a5_landing_gear_weight.py
+-rw-r--r--   0        0        0     2713 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a6_pylons_weight.py
+-rw-r--r--   0        0        0     2001 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a7_paint_weight.py
+-rw-r--r--   0        0        0     1166 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/constants.py
+-rw-r--r--   0        0        0     3330 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/sum.py
+-rw-r--r--   0        0        0      921 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/__init__.py
+-rw-r--r--   0        0        0     2333 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b1_engine_weight.py
+-rw-r--r--   0        0        0     2349 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b2_fuel_lines_weight.py
+-rw-r--r--   0        0        0     2234 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b3_unconsumables_weight.py
+-rw-r--r--   0        0        0      949 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/constants.py
+-rw-r--r--   0        0        0     2213 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/sum.py
+-rw-r--r--   0        0        0     1175 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/__init__.py
+-rw-r--r--   0        0        0     4224 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c1_power_systems_weight.py
+-rw-r--r--   0        0        0     9037 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c2_life_support_systems_weight.py
+-rw-r--r--   0        0        0     2675 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c3_navigation_systems_weight.py
+-rw-r--r--   0        0        0     2354 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c4_transmissions_systems_weight.py
+-rw-r--r--   0        0        0     3577 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c5_fixed_operational_systems_weight.py
+-rw-r--r--   0        0        0     2160 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c6_flight_kit_weight.py
+-rw-r--r--   0        0        0     1172 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/constants.py
+-rw-r--r--   0        0        0     3735 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/sum.py
+-rw-r--r--   0        0        0     1109 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/constants.py
+-rw-r--r--   0        0        0     5245 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/cs25.py
+-rw-r--r--   0        0        0     1047 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/constants.py
+-rw-r--r--   0        0        0     2772 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d1_cargo_configuration_weight.py
+-rw-r--r--   0        0        0     2399 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d2_passenger_seats_weight.py
+-rw-r--r--   0        0        0     2005 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d3_food_water_weight.py
+-rw-r--r--   0        0        0     2041 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d4_security_kit_weight.py
+-rw-r--r--   0        0        0     2358 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d5_toilets_weight.py
+-rw-r--r--   0        0        0     2467 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/sum.py
+-rw-r--r--   0        0        0      801 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/crew_weight.py
+-rw-r--r--   0        0        0     4207 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/mass_breakdown.py
+-rw-r--r--   0        0        0     2264 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/payload.py
+-rw-r--r--   0        0        0     1767 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/update_mlw_and_mzfw.py
+-rw-r--r--   0        0        0     2393 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/weight.py
+-rw-r--r--   0        0        0       35 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/.gitignore
+-rw-r--r--   0        0        0    16246 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/01_tutorial.ipynb
+-rw-r--r--   0        0        0     8609 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/02_postprocessing.ipynb
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/__init__.py
+-rw-r--r--   0        0        0   129349 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/data/CeRAS01_baseline.xml
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/data/__init__.py
+-rw-r--r--   0        0        0     2457 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/data/oad_process_timestep_mission.yml
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/__init__.py
+-rw-r--r--   0        0        0    18684 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0    23022 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-onera.png
+-rw-r--r--   0        0        0    19493 2023-05-15 10:25:19.805350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/user_files_arch.svg
+-rw-r--r--   0        0        0   266366 2023-05-15 10:25:19.809350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/variable_viewer_change_range.gif
+-rw-r--r--   0        0        0    20214 2023-05-15 10:25:19.809350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/CeRAS_case_study.ipynb
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.809350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/__init__.py
+-rw-r--r--   0        0        0     4251 2023-05-15 10:25:19.809350 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/ceras_utils.py
+-rw-r--r--   0        0        0  2020992 2023-05-15 10:25:19.821351 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionDesign_R4630_PL17000_out.csv
+-rw-r--r--   0        0        0  2147719 2023-05-15 10:25:19.833352 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R5093_PL13608_out.csv
+-rw-r--r--   0        0        0  1285241 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R926_PL13608_out.csv
+-rw-r--r--   0        0        0     8645 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_data_for_plots.xml
+-rw-r--r--   0        0        0     4185 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_missions.yml
+-rw-r--r--   0        0        0   137335 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_reference_data.xml
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/__init__.py
+-rw-r--r--   0        0        0     1446 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing.yml
+-rw-r--r--   0        0        0   107154 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing_out.xml
+-rw-r--r--   0        0        0     1152 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/operational_missions.yml
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/__init__.py
+-rw-r--r--   0        0        0    18684 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0    23022 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-onera.png
+-rw-r--r--   0        0        0   124900 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_1.png
+-rw-r--r--   0        0        0   147435 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_2.png
+-rw-r--r--   0        0        0    83712 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/wing_parameters.png
+-rw-r--r--   0        0        0      714 2023-05-15 10:25:19.841353 fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/__init__.py
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 fast_oad_cs25-0.3.0/PKG-INFO
```

### Comparing `FAST-OAD-CS25-0.2.0/LICENSE` & `fast_oad_cs25-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/README.md` & `fast_oad_cs25-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/pyproject.toml` & `fast_oad_cs25-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FAST-OAD-CS25"
-version = "v0.2.0"
+version = "0.3.0"
 description = "FAST-OAD_CS25 is a FAST-OAD plugin with CS25/FAR25-related models."
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
     "Scott DELBECQ <Scott.DELBECQ@isae-supaero.fr>"
 ]
 packages = [
@@ -39,41 +39,52 @@
 # IMPORTANT: when modifying this list, docs/requirements.txt must be updated for
 # ReadTheDocs to be able to compile the documentation.
 # A pre-commit hook has been added to do this task. As a result, any modification
 # of poetry.lock file will modify docs/requirements.txt and make
 # the commit fail because "files were modified by this hook". In that case,
 # doing again the commit including changes in docs/requirements.txt will succeed.
 python = "^3.7"
-fast-oad-core = ">=1.4.2, <2.0"
-openmdao = "^3.10"
+fast-oad-core = "^1.4.2"
+openmdao = "^3.18"
 numpy = "^1.21.0"
 scipy = "^1.4.1"
 pandas = "^1.1.0"
 stdatm = "0.*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+
+[tool.poetry.group.test.dependencies]
 pytest = "^6.2"
 pytest-cov = "^3.0"
 coverage = { extras = ["toml"], version = "^5.5" }
-pre-commit = "^2.14.1"
-black = { version = "22.1", extras = ["jupyter"] }
-pylint = "^2.10.2"
 nbval = "^0.9.6"
+
+[tool.poetry.group.doc.dependencies]
 sphinx = "^4.1.2"
 sphinx-rtd-theme = "^1.0"
 sphinxcontrib-bibtex = "^2.3.0"
+
+[tool.poetry.group.lint.dependencies]
+pre-commit = "^2.14.1"
+black = { version = "22.1", extras = ["jupyter"] }
+pylint = "^2.10.2"
 flake8 = "^4.0.1"
 nbstripout = "^0.5.0"
 
 [tool.poetry.plugins."fastoad.plugins"]
 "cs25" = "fastoad_cs25"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov fastoad_cs25 --cov-report term-missing --cov-report html --verbose"
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/configurations/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/configurations/cs25_base.yaml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/configurations/cs25_base.yaml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_high_speed.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_high_speed.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_landing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_landing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_low_speed.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_low_speed.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_takeoff.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/aerodynamics_takeoff.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_fuselage.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_fuselage.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_ht.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_ht.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_nacelles_pylons.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_nacelles_pylons.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_total.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_total.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_vt.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_vt.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd0_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd0_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd_compressibility.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd_compressibility.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/cd_trim.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/cd_trim.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_alpha.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_alpha.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_cl_alpha.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_cl_alpha.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         self.add_input("data:geometry:wing:tip:chord", val=np.nan, units="m")
         self.add_input("data:geometry:wing:sweep_25", val=np.nan, units="rad")
         self.add_input("data:geometry:wing:root:chord", val=np.nan, units="m")
         self.add_input("data:geometry:wing:area", val=np.nan, units="m**2")
         self.add_input("data:geometry:wing:tip:thickness_ratio", val=np.nan)
 
         if self.options["low_speed_aero"]:
-            self.add_output("data:aerodynamics:aircraft:low_speed:CL_alpha")
+            self.add_output("data:aerodynamics:aircraft:low_speed:CL_alpha", units="1/rad")
         else:
-            self.add_output("data:aerodynamics:aircraft:cruise:CL_alpha")
+            self.add_output("data:aerodynamics:aircraft:cruise:CL_alpha", units="1/rad")
 
     def setup_partials(self):
         if self.options["low_speed_aero"]:
             self.declare_partials("data:aerodynamics:aircraft:low_speed:CL_alpha", "*", method="fd")
         else:
             self.declare_partials("data:aerodynamics:aircraft:cruise:CL_alpha", "*", method="fd")
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_max_cl_landing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_max_cl_landing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_polar.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_polar.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/compute_reynolds.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/compute_reynolds.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/high_lift_aero.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/high_lift_aero.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/initialize_cl.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/initialize_cl.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/oswald.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/oswald.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/resources/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/resources/interpolation of lift effectiveness.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/resources/interpolation of lift effectiveness.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/utils/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/utils/cd0_lifting_surface.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/utils/cd0_lifting_surface.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/components/utils/friction_drag.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/components/utils/friction_drag.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/BACJ.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/BACJ.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pplot.exe` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pplot.exe`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pxplot.exe` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/pxplot.exe`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/xfoil.exe` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil699/xfoil.exe`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil_polar.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/aerodynamics/external/xfoil/xfoil_polar.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/compute_aero_center.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/compute_aero_center.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     Estimation of aerodynamic center
 """
 #  This file is part of FAST-OAD_CS25
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -37,16 +37,18 @@
         self.add_input("data:geometry:fuselage:length", val=np.nan, units="m")
         self.add_input("data:geometry:wing:MAC:at25percent:x", val=np.nan, units="m")
         self.add_input("data:geometry:wing:area", val=np.nan, units="m**2")
         self.add_input("data:geometry:horizontal_tail:area", val=np.nan, units="m**2")
         self.add_input(
             "data:geometry:horizontal_tail:MAC:at25percent:x:from_wingMAC25", val=np.nan, units="m"
         )
-        self.add_input("data:aerodynamics:aircraft:cruise:CL_alpha", val=np.nan)
-        self.add_input("data:aerodynamics:horizontal_tail:cruise:CL_alpha", val=np.nan)
+        self.add_input("data:aerodynamics:aircraft:cruise:CL_alpha", val=np.nan, units="1/rad")
+        self.add_input(
+            "data:aerodynamics:horizontal_tail:cruise:CL_alpha", val=np.nan, units="1/rad"
+        )
 
         self.add_output("data:aerodynamics:cruise:neutral_point:x")
 
     def setup_partials(self):
         self.declare_partials("*", "*", method="fd")
 
     def compute(self, inputs, outputs):
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/compute_wetted_area.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/compute_wetted_area.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_cnbeta_fuselage.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_cnbeta_fuselage.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_fuselage.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/fuselage/compute_fuselage.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_chords.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_chords.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_cl_alpha.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_cl_alpha.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Estimation of horizontal tail lift coefficient
 """
 
 #  This file is part of FAST-OAD_CS25
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -26,15 +26,15 @@
     """Horizontal tail lift coefficient estimation"""
 
     def setup(self):
         self.add_input("data:geometry:horizontal_tail:aspect_ratio", val=np.nan)
         self.add_input("data:TLAR:cruise_mach", val=np.nan)
         self.add_input("data:geometry:horizontal_tail:sweep_25", val=np.nan, units="deg")
 
-        self.add_output("data:aerodynamics:horizontal_tail:cruise:CL_alpha")
+        self.add_output("data:aerodynamics:horizontal_tail:cruise:CL_alpha", units="1/rad")
 
     def setup_partials(self):
         self.declare_partials("data:aerodynamics:horizontal_tail:cruise:CL_alpha", "*", method="fd")
 
     def compute(self, inputs, outputs):
         cruise_mach = inputs["data:TLAR:cruise_mach"]
         lambda_ht = inputs["data:geometry:horizontal_tail:aspect_ratio"]
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_mac.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_mac.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_sweep.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/components/compute_ht_sweep.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/ht/compute_horizontal_tail.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/ht/compute_horizontal_tail.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/compute_nacelle_pylons.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/nacelle_pylons/compute_nacelle_pylons.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_chords.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_chords.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_clalpha.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_clalpha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     Estimation of vertical tail lift coefficient
 """
 #  This file is part of FAST-OAD_CS25
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -29,15 +29,15 @@
 
     def setup(self):
         self.add_input("data:TLAR:cruise_mach", val=np.nan)
         self.add_input("data:geometry:has_T_tail", val=np.nan)
         self.add_input("data:geometry:vertical_tail:aspect_ratio", val=np.nan)
         self.add_input("data:geometry:vertical_tail:sweep_25", val=np.nan, units="deg")
 
-        self.add_output("data:aerodynamics:vertical_tail:cruise:CL_alpha")
+        self.add_output("data:aerodynamics:vertical_tail:cruise:CL_alpha", units="1/rad")
 
     def setup_partials(self):
         self.declare_partials("data:aerodynamics:vertical_tail:cruise:CL_alpha", "*", method="fd")
 
     def compute(self, inputs, outputs, discrete_inputs=None, discrete_outputs=None):
         tail_type = np.round(inputs["data:geometry:has_T_tail"])
         cruise_mach = inputs["data:TLAR:cruise_mach"]
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_distance.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_distance.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_mac.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_mac.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_sweep.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/components/compute_vt_sweep.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/vt/compute_vertical_tail.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/vt/compute_vertical_tail.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_b_50.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_b_50.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l1_l4.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l1_l4.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l2_l3.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_l2_l3.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mac_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mac_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mfw.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_mfw.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_sweep_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_sweep_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_toc_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_toc_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_wet_area_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_wet_area_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_x_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_x_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_y_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/components/compute_y_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geom_components/wing/compute_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geom_components/wing/compute_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/geometry.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/profile.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/profile_getter.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/profile_getter.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/BACJ.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/BACJ.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_11.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_11.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_12.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_12.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_15.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/airfoil_f_15_15.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/profiles/resources/naca23012.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/profiles/resources/naca23012.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/geometry/wing_global_positions.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/geometry/wing_global_positions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/compute_static_margin.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/compute_static_margin.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_ht_area.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_ht_area.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_tail_areas.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_tail_areas.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_vt_area.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/handling_qualities/tail_sizing/compute_vt_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Estimation of vertical tail area
 """
 #  This file is part of FAST-OAD_CS25
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -26,15 +26,15 @@
     as stated in :cite:raymer:1992.
     """
 
     def setup(self):
         self.add_input("data:TLAR:cruise_mach", val=np.nan)
         self.add_input("data:weight:aircraft:CG:aft:MAC_position", val=np.nan)
         self.add_input("data:aerodynamics:fuselage:cruise:CnBeta", val=np.nan)
-        self.add_input("data:aerodynamics:vertical_tail:cruise:CL_alpha", val=np.nan)
+        self.add_input("data:aerodynamics:vertical_tail:cruise:CL_alpha", val=np.nan, units="1/rad")
         self.add_input("data:geometry:wing:MAC:length", val=np.nan, units="m")
         self.add_input("data:geometry:wing:area", val=np.nan, units="m**2")
         self.add_input("data:geometry:wing:span", val=np.nan, units="m")
         self.add_input(
             "data:geometry:vertical_tail:MAC:at25percent:x:from_wingMAC25", val=np.nan, units="m"
         )
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/loops/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/loops/compute_wing_area.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/cs25.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,135 @@
 """
-Computation of wing area
+Computation of load cases
 """
 #  This file is part of FAST-OAD_CS25
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import numpy as np
-import openmdao.api as om
-from fastoad.module_management.constants import ModelDomain
-from fastoad.module_management.service_registry import RegisterOpenMDAOSystem
-from scipy.constants import g
+from fastoad.module_management.service_registry import RegisterSubmodel
+from openmdao.core.explicitcomponent import ExplicitComponent
+from stdatm import Atmosphere
 
+from .constants import SERVICE_GUST_LOADS
 
-@RegisterOpenMDAOSystem("fastoad.loop.wing_area", domain=ModelDomain.OTHER)
-class ComputeWingArea(om.Group):
-    """
-    Computes needed wing area for:
-      - having enough lift at required approach speed
-      - being able to load enough fuel to achieve the sizing mission
-    """
-
-    def setup(self):
-        self.add_subsystem("wing_area", _ComputeWingArea(), promotes=["*"])
-        self.add_subsystem("constraints", _ComputeWingAreaConstraints(), promotes=["*"])
 
+@RegisterSubmodel(SERVICE_GUST_LOADS, "fastoad.submodel.gust_loads")
+class Loads(ExplicitComponent):
+    """
+    Computes gust load cases
 
-class _ComputeWingArea(om.ExplicitComponent):
-    """Computation of wing area from needed approach speed and mission fuel"""
-
-    def setup(self):
-        self.add_input("data:geometry:wing:aspect_ratio", val=np.nan)
-        self.add_input("data:geometry:wing:root:thickness_ratio", val=np.nan)
-        self.add_input("data:geometry:wing:tip:thickness_ratio", val=np.nan)
-        self.add_input("data:weight:aircraft:sizing_block_fuel", val=np.nan, units="kg")
-        self.add_input("data:TLAR:approach_speed", val=np.nan, units="m/s")
-
-        self.add_input("data:weight:aircraft:MLW", val=np.nan, units="kg")
-        self.add_input("data:aerodynamics:aircraft:landing:CL_max", val=np.nan)
-
-        self.add_output("data:geometry:wing:area", val=100.0, units="m**2")
-
-    def setup_partials(self):
-        self.declare_partials("data:geometry:wing:area", "*", method="fd")
-
-    def compute(self, inputs, outputs, discrete_inputs=None, discrete_outputs=None):
-        lambda_wing = inputs["data:geometry:wing:aspect_ratio"]
-        root_thickness_ratio = inputs["data:geometry:wing:root:thickness_ratio"]
-        tip_thickness_ratio = inputs["data:geometry:wing:tip:thickness_ratio"]
-        mfw_mission = inputs["data:weight:aircraft:sizing_block_fuel"]
-        wing_area_mission = (
-            max(1000.0, mfw_mission - 1570.0)
-            / 224
-            / lambda_wing**-0.4
-            / (0.6 * root_thickness_ratio + 0.4 * tip_thickness_ratio)
-        ) ** (1.0 / 1.5)
-
-        approach_speed = inputs["data:TLAR:approach_speed"]
-        mlw = inputs["data:weight:aircraft:MLW"]
-        max_CL = inputs["data:aerodynamics:aircraft:landing:CL_max"]
-        wing_area_approach = 2 * mlw * g / ((approach_speed / 1.23) ** 2) / (1.225 * max_CL)
+    Load case 1: with wings with almost no fuel
+    Load case 2: at maximum take-off weight
 
-        outputs["data:geometry:wing:area"] = np.nanmax([wing_area_mission, wing_area_approach])
+    Based on formulas in :cite:`supaero:2014`, §6.3
 
+    """
 
-class _ComputeWingAreaConstraints(om.ExplicitComponent):
     def setup(self):
-        self.add_input("data:weight:aircraft:sizing_block_fuel", val=np.nan, units="kg")
-        self.add_input("data:weight:aircraft:MFW", val=np.nan, units="kg")
-
-        self.add_input("data:TLAR:approach_speed", val=np.nan, units="m/s")
-        self.add_input("data:weight:aircraft:MLW", val=np.nan, units="kg")
-        self.add_input("data:aerodynamics:aircraft:landing:CL_max", val=np.nan)
         self.add_input("data:geometry:wing:area", val=np.nan, units="m**2")
-
-        self.add_output("data:weight:aircraft:additional_fuel_capacity", units="kg")
-        self.add_output("data:aerodynamics:aircraft:landing:additional_CL_capacity")
+        self.add_input("data:geometry:wing:span", val=np.nan, units="m")
+        self.add_input("data:weight:aircraft:MZFW", val=np.nan, units="kg")
+        self.add_input("data:weight:aircraft:MFW", val=np.nan, units="kg")
+        self.add_input("data:weight:aircraft:MTOW", val=np.nan, units="kg")
+        self.add_input("data:aerodynamics:aircraft:cruise:CL_alpha", val=np.nan, units="1/rad")
+        self.add_input("data:load_case:lc1:U_gust", val=np.nan, units="m/s")
+        self.add_input("data:load_case:lc1:altitude", val=np.nan, units="ft")
+        self.add_input("data:load_case:lc1:Vc_EAS", val=np.nan, units="m/s")
+        self.add_input("data:load_case:lc2:U_gust", val=np.nan, units="m/s")
+        self.add_input("data:load_case:lc2:altitude", val=np.nan, units="ft")
+        self.add_input("data:load_case:lc2:Vc_EAS", val=np.nan, units="m/s")
+
+        self.add_output("data:mission:sizing:cs25:load_factor_1")
+        self.add_output("data:mission:sizing:cs25:load_factor_2")
+        self.add_output("data:mission:sizing:cs25:sizing_load_1", units="kg")
+        self.add_output("data:mission:sizing:cs25:sizing_load_2", units="kg")
 
     def setup_partials(self):
-        self.declare_partials(
-            "data:weight:aircraft:additional_fuel_capacity",
-            ["data:weight:aircraft:MFW", "data:weight:aircraft:sizing_block_fuel"],
-            method="fd",
-        )
-        self.declare_partials(
-            "data:aerodynamics:aircraft:landing:additional_CL_capacity",
-            [
-                "data:TLAR:approach_speed",
-                "data:weight:aircraft:MLW",
-                "data:aerodynamics:aircraft:landing:CL_max",
-                "data:geometry:wing:area",
-            ],
-            method="fd",
-        )
+        self.declare_partials("*", "*", method="fd")
 
+    # pylint: disable=too-many-locals
+    # pylint: disable=invalid-name
     def compute(self, inputs, outputs, discrete_inputs=None, discrete_outputs=None):
-        mfw = inputs["data:weight:aircraft:MFW"]
-        mission_fuel = inputs["data:weight:aircraft:sizing_block_fuel"]
-        v_approach = inputs["data:TLAR:approach_speed"]
-        cl_max = inputs["data:aerodynamics:aircraft:landing:CL_max"]
-        mlw = inputs["data:weight:aircraft:MLW"]
+        sea_level_density = Atmosphere(0).density
         wing_area = inputs["data:geometry:wing:area"]
+        span = inputs["data:geometry:wing:span"]
+        mzfw = inputs["data:weight:aircraft:MZFW"]
+        mfw = inputs["data:weight:aircraft:MFW"]
+        mtow = inputs["data:weight:aircraft:MTOW"]
+        cl_alpha = inputs["data:aerodynamics:aircraft:cruise:CL_alpha"]
+        u_gust1 = inputs["data:load_case:lc1:U_gust"]
+        alt_1 = inputs["data:load_case:lc1:altitude"]
+        vc_eas1 = inputs["data:load_case:lc1:Vc_EAS"]
+        u_gust2 = inputs["data:load_case:lc2:U_gust"]
+        alt_2 = inputs["data:load_case:lc2:altitude"]
+        vc_eas2 = inputs["data:load_case:lc2:Vc_EAS"]
+
+        # calculation of mean geometric chord
+        chord_geom = wing_area / span
+
+        # load case #1
+        m1 = 1.05 * mzfw
+        n_gust_1 = self.__n_gust(
+            m1,
+            wing_area,
+            Atmosphere(alt_1).density,
+            sea_level_density,
+            chord_geom,
+            vc_eas1,
+            cl_alpha,
+            u_gust1,
+        )
+        n1 = 1.5 * max(2.5, n_gust_1)
+        n1m1 = n1 * m1
 
-        outputs["data:weight:aircraft:additional_fuel_capacity"] = mfw - mission_fuel
-        outputs["data:aerodynamics:aircraft:landing:additional_CL_capacity"] = cl_max - mlw * g / (
-            0.5 * 1.225 * (v_approach / 1.23) ** 2 * wing_area
+        # load case #2
+        n_gust_2 = self.__n_gust(
+            mtow,
+            wing_area,
+            Atmosphere(alt_2).density,
+            sea_level_density,
+            chord_geom,
+            vc_eas2,
+            cl_alpha,
+            u_gust2,
+        )
+        n2 = 1.5 * max(2.5, n_gust_2)
+        mcv = min(0.8 * mfw, mtow - mzfw)
+        n2m2 = n2 * (mtow - 0.55 * mcv)
+
+        outputs["data:mission:sizing:cs25:load_factor_1"] = n1
+        outputs["data:mission:sizing:cs25:load_factor_2"] = n2
+        outputs["data:mission:sizing:cs25:sizing_load_1"] = n1m1
+        outputs["data:mission:sizing:cs25:sizing_load_2"] = n2m2
+
+    @staticmethod
+    def __n_gust(mass, wing_area, rho, sea_level_density, chord_geom, vc_eas, cl_alpha, u_gust):
+        """
+        Computes a reference gust load.
+
+        :param mass:
+        :param wing_area:
+        :param rho:
+        :param sea_level_density:
+        :param chord_geom:
+        :param vc_eas: Vc (Equivalent AirSpeed)
+        :param cl_alpha:
+        :param u_gust:
+        :return:
+        """
+        mu_g = 2 * mass / rho / wing_area / chord_geom / cl_alpha
+        k_g = 0.88 * mu_g / (5.3 + mu_g)  # attenuation factor
+        n_gust = 1 + (sea_level_density / 2 / 9.81) * k_g * u_gust * (
+            vc_eas * cl_alpha / mass / wing_area
         )
+
+        return n_gust
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/loops/compute_wing_position.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/loops/compute_wing_position.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/exceptions.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/openmdao.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/openmdao.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/rubber_engine.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/propulsion/fuel_propulsion/rubber_engine/rubber_engine.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/variable_descriptions.txt` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/variable_descriptions.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_control_surfaces.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_control_surfaces.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_others.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_others.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_ratio_aft.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_ratio_aft.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_tanks.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_tanks.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_wing.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_cg_wing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_global_cg.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_global_cg.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_ht_cg.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_ht_cg.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_max_cg_ratio.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_max_cg_ratio.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_vt_cg.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/compute_vt_cg.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase1.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase1.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase2.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase2.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase3.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase3.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase4.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase4.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase_base.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcase_base.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcases.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/load_cases/compute_cg_loadcases.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/cg_components/update_mlg.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/cg_components/update_mlg.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/cg/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/cg/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a1_wing_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a1_wing_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a2_fuselage_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a2_fuselage_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a3_empennage_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a3_empennage_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a4_flight_control_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a4_flight_control_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a5_landing_gear_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a5_landing_gear_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a6_pylons_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a6_pylons_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a7_paint_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/a7_paint_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/sum.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/a_airframe/sum.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b1_engine_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b1_engine_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b2_fuel_lines_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b2_fuel_lines_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b3_unconsumables_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/b3_unconsumables_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/sum.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/b_propulsion/sum.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c1_power_systems_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c1_power_systems_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c2_life_support_systems_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c2_life_support_systems_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c3_navigation_systems_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c3_navigation_systems_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c4_transmissions_systems_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c4_transmissions_systems_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c5_fixed_operational_systems_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c5_fixed_operational_systems_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c6_flight_kit_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/c6_flight_kit_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/sum.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/c_systems/sum.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/constants.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d1_cargo_configuration_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d1_cargo_configuration_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d2_passenger_seats_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d2_passenger_seats_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d3_food_water_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d3_food_water_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d4_security_kit_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d4_security_kit_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d5_toilets_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/d5_toilets_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/sum.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/d_furniture/sum.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/crew_weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/e_crew/crew_weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/mass_breakdown.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/mass_breakdown.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/payload.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/payload.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/mass_breakdown/update_mlw_and_mzfw.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/mass_breakdown/update_mlw_and_mzfw.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/models/weight/weight.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/models/weight/weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/01_tutorial.ipynb` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/01_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/02_postprocessing.ipynb` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/02_postprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/data/CeRAS01_baseline.xml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/data/CeRAS01_baseline.xml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/data/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/data/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/data/oad_process_timestep_mission.yml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/data/oad_process_timestep_mission.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-ISAE_SUPAERO.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-onera.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/logo-onera.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/user_files_arch.svg` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/user_files_arch.svg`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/01_tutorial/img/variable_viewer_change_range.gif` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/01_tutorial/img/variable_viewer_change_range.gif`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/CeRAS_case_study.ipynb` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/CeRAS_case_study.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/ceras_utils.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/ceras_utils.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionDesign_R4630_PL17000_out.csv` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionDesign_R4630_PL17000_out.csv`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R5093_PL13608_out.csv` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R5093_PL13608_out.csv`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R926_PL13608_out.csv` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CSR-01_missionStudy_R926_PL13608_out.csv`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_data_for_plots.xml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_data_for_plots.xml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_missions.yml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_missions.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_reference_data.xml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/CeRAS_reference_data.xml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing.yml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing_out.xml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/oad_sizing_out.xml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/operational_missions.yml` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/data/operational_missions.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-ISAE_SUPAERO.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-onera.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/logo-onera.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_1.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_1.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_2.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/mass_breakdown_2.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/wing_parameters.png` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/02_CeRAS_case_study/img/wing_parameters.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/src/fastoad_cs25/notebooks/__init__.py` & `fast_oad_cs25-0.3.0/src/fastoad_cs25/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-CS25-0.2.0/PKG-INFO` & `fast_oad_cs25-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-oad-cs25
-Version: 0.2.0
+Version: 0.3.0
 Summary: FAST-OAD_CS25 is a FAST-OAD plugin with CS25/FAR25-related models.
 Home-page: https://github.com/fast-aircraft-design/FAST-OAD
 License: GPL-3.0-only
 Keywords: aircraft,design,multi-disciplinary
 Author: Christophe DAVID
 Author-email: christophe.david@onera.fr
 Requires-Python: >=3.7,<4.0
@@ -14,22 +14,26 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: fast-oad-core (>=1.4.2,<2.0)
+Requires-Dist: fast-oad-core (>=1.4.2,<2.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: openmdao (>=3.10,<4.0)
+Requires-Dist: openmdao (>=3.18,<4.0)
 Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
 Requires-Dist: stdatm (<1.0.0)
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/fast-aircraft-design/FAST-OAD_CS25/workflows/Tests/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/06d1fb8ee5c3429cb3cbb165413187bc)](https://www.codacy.com/gh/fast-aircraft-design/FAST-OAD_CS25/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fast-aircraft-design/FAST-OAD_CS25&amp;utm_campaign=Badge_Grade)
```

