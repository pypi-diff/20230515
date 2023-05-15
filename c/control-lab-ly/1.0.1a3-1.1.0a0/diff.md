# Comparing `tmp/control-lab-ly-1.0.1a3.tar.gz` & `tmp/control-lab-ly-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.0.1a3.tar", last modified: Tue May  2 09:32:31 2023, max compression
+gzip compressed data, was "control-lab-ly-1.1.0a0.tar", last modified: Mon May 15 14:04:14 2023, max compression
```

## Comparing `control-lab-ly-1.0.1a3.tar` & `control-lab-ly-1.1.0a0.tar`

### file list

```diff
@@ -1,218 +1,228 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.522635 control-lab-ly-1.0.1a3/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a3/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/MANIFEST.in
--rw-rw-rw-   0        0        0    17492 2023-05-02 09:32:31.530653 control-lab-ly-1.0.1a3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.006379 control-lab-ly-1.0.1a3/docs/
--rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.1a3/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a3/docs/LICENSE.md
--rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.0.1a3/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/pyproject.toml
--rw-rw-rw-   0        0        0     1560 2023-05-02 09:32:31.530653 control-lab-ly-1.0.1a3/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.1a3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:29.635697 control-lab-ly-1.0.1a3/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.040899 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    17492 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7306 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.050378 control-lab-ly-1.0.1a3/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.050874 control-lab-ly-1.0.1a3/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.061383 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.079349 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.114659 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.131858 control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.142625 control-lab-ly-1.0.1a3/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.150637 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.174831 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    17622 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.174831 control-lab-ly-1.0.1a3/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.248341 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15405 2023-04-27 03:04:50.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3767 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.264326 control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.288326 control-lab-ly-1.0.1a3/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.304818 control-lab-ly-1.0.1a3/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10533 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.327661 control-lab-ly-1.0.1a3/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9118 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.347192 control-lab-ly-1.0.1a3/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.363650 control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9684 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.403965 control-lab-ly-1.0.1a3/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.435867 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.471799 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.516873 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.534963 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.570797 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10345 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.597459 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.650685 control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8427 2023-04-27 03:04:50.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.662413 control-lab-ly-1.0.1a3/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.700109 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.716482 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.747133 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.769957 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15883 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.779587 control-lab-ly-1.0.1a3/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.850288 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.909703 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.942686 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29855 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.969417 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    31524 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13186 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.979991 control-lab-ly-1.0.1a3/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.995994 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.017387 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.033391 control-lab-ly-1.0.1a3/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.049382 control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.080412 control-lab-ly-1.0.1a3/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.096990 control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.113028 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.122188 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.168105 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.184151 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      310 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15591 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    15865 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.232436 control-lab-ly-1.0.1a3/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6559 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a3/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.240816 control-lab-ly-1.0.1a3/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.257346 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.285558 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.337557 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.522635 control-lab-ly-1.0.1a3/tests/
--rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      629 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.1a3/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      390 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.378557 control-lab-ly-1.1.0a0/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0a0/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18871 2023-05-15 14:04:14.380947 control-lab-ly-1.1.0a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.151796 control-lab-ly-1.1.0a0/docs/
+-rw-rw-rw-   0        0        0     5644 2023-05-15 13:59:45.000000 control-lab-ly-1.1.0a0/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.0a0/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0a0/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.1.0a0/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1559 2023-05-15 14:04:14.401059 control-lab-ly-1.1.0a0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.0a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:11.791488 control-lab-ly-1.1.0a0/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.205931 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    18871 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7781 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.221443 control-lab-ly-1.1.0a0/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.225133 control-lab-ly-1.1.0a0/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.233432 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.260868 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.297495 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.319968 control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.366749 control-lab-ly-1.1.0a0/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.389946 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.409910 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17622 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.419711 control-lab-ly-1.1.0a0/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.511823 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      658 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0     5544 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    17966 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0     8757 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/liquid_panel.py
+-rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     7373 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15419 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3775 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.527946 control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.583054 control-lab-ly-1.1.0a0/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.590031 control-lab-ly-1.1.0a0/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10712 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.602987 control-lab-ly-1.1.0a0/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9118 2023-05-12 05:43:18.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.612265 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.641242 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    23118 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.730314 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37208 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.767908 control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9684 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3989 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.902347 control-lab-ly-1.1.0a0/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.924529 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.976210 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18014 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.005819 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.023228 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.059844 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10345 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-05-12 05:43:18.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.071087 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.084284 control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8427 2023-05-05 09:28:56.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.118283 control-lab-ly-1.1.0a0/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.167233 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3450 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.187296 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.234375 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.262286 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24280 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15883 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.317381 control-lab-ly-1.1.0a0/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.357489 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.385737 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.425074 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29862 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.467891 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    31585 2023-05-15 13:59:45.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13191 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.485042 control-lab-ly-1.1.0a0/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.509326 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.562012 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     9316 2023-05-15 13:59:45.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.635650 control-lab-ly-1.1.0a0/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.691292 control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.707631 control-lab-ly-1.1.0a0/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.749564 control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.814548 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.825322 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.890281 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.915566 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      310 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15591 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    15865 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.000324 control-lab-ly-1.1.0a0/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6559 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.1.0a0/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.017274 control-lab-ly-1.1.0a0/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.034992 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.063944 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.094843 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.372578 control-lab-ly-1.1.0a0/tests/
+-rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      629 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      586 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      390 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-05-04 09:11:29.000000 control-lab-ly-1.1.0a0/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0     1011 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/tests/test_mixture_shaker.py
+-rw-rw-rw-   0        0        0     1020 2023-05-09 08:54:35.000000 control-lab-ly-1.1.0a0/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.1a3/LICENSE.md` & `control-lab-ly-1.1.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/PKG-INFO` & `control-lab-ly-1.1.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.1a3
+Version: 1.1.0a0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -340,89 +340,89 @@
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
 ## Unreleased
 *Items under development*
+### 1.1.0
+- Integration for orbital shaker \[QInstruments\]
+- Integration for pH meter probe \[Sentron\]
+- Integration for force sensor
 
-## 1.0.0.x
+
+## Version 1.0.1
+Bug fixes and minor feature enhancements. First released 08 May 2023.
+### Added
+- `LiquidMover`
+  - Added `LiquidMover.touchTip()` method to touch the pipette tip against the walls of the vessel to remove excess liquid on the outside of the tip (#62)
+  - Added option to indicate the position of the first available pipette tip in `LiquidMover` (#61)
+- Added adaptive GUI controls for `Liquid` objects (#70)
+- Added option to indicate which digital IO channel to use with Dobot attachments (#53)
+### Changed
+- `MassBalance`
+  - Updated to the use `pd.concat()` instead of `pd.DataFrame.append()`, which is going ot be deprecated (#63)
+  - Fixed endless loop for when `MassBalance` tries to `zero()` while recording data (#60)
+- Changed the `Image` class and methods into functions within a module (#54)
+- Fixed the tool offset of pipette when pipette tip is attached, and accounts for the length of pipette that enters the pipette tip (#64)
+- Changed to using more precise time interval measurements by moving from `time.time()` to `time.perf_counter()` (#68)
+- Fixed discrepancy in aspirate and dispense speed for `Sartorius` (#73) and let speed return to a global default value (#72)
+- Updated documentation
+
+
+## Version 1.0.0
 Major overhaul in package structure. Standardisation of methods and consolidation of common methods. First released 12 Apr 2023.
 ### Added
-#### 1.0.0
-- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing
-- Usage of Protocols to provide an interface between different classes of objects
+- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing (#31)
+- Usage of Protocols to provide an interface between different classes of objects (#30)
 - Usage of Dataclasses to store complex data 
 - Usage of decorators to modify methods
 - Introduced different functions to parse the program docstring and find program parameters
 ### Changed
-#### 1.0.0
 - Standardised methods and consolidated common methods
-- Added type hints
+- Added type hints (#28)
 - Moved Dobot attachments from Mover to Transfer.Substrate
 - Split GUI Panels into individual files
 - Split Dobot arms into individual files
 - Split functions/methods in `misc.py` into individual files.
 - Changed `_flags` to a public attribute `flags`
-- Update documentation
+- Update documentation (#27, #28, #29)
 ### Removed
-#### 1.0.0
 - Unnecessary commented-out blocks of code
 
-## 0.0.4.x
-Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.
+
+## Version 0.0.x
+(0.0.4.x) Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.\
+(0.0.3.x) Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.\
+(0.0.2.x) Updates in setting up configuration files. First released 24 Feb 2023.\
+(0.0.1.x) First release of [Control.lab.ly](https://pypi.org/project/control-lab-ly/) distributed on 23 Feb 2023.\
+(0.0.0.x) Pre-release packaging checks
 ### Added
 #### 0.0.4
-- Added control for `Peltier`
+- Added control for `Peltier` (#23)
   - set and get temperatures
   - hold temperatures for desired duration
   - checks if target temperature has been reached by checking power level lower than a threshold or time passed over a predefined duration, once the temperature is within tolerance
   - ability to record temperatures and timestamps 
-- Added control for `TriContinent` and `TriContinentEnsemble`
+- Added control for `TriContinent` and `TriContinentEnsemble` (#25)
   - single actions such as `empty`, `fill`, `initialise`, move actions, set speeds and valves, and wait
   - compound actions such as `aspirate`, `dispense`, and `prime`
-### Changed
-#### 0.0.4
-- Update documentation
-
-## 0.0.3.x
-Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.
-### Added
 #### 0.0.3
-- Added safety measures for movement actions
+- Added safety measures for movement actions (#24)
   - In `Deck`, added exclusion zones when reading the `layout.json` file and new method `is_excluded()` to check if target coordinate is within the exclusion zone
   - In `Mover`, update `isFeasible()` method to check if target coordinates violates the deck's exclusion zone
   - New function `set_safety()` defines safety modes when starting a new session to pause for input (in "high" safety setting) and to wait for safety countdown (in "low" safety setting)
-- `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations
-### Changed
-#### 0.0.3.1
-- Update documentation
-#### 0.0.3
-- `Sartorius`
-  - made the blowout/home optional for the dispense method upon emptying the pipette
-- Update documentation
-
-## 0.0.2.x
-Updates in setting up configuration files. First released 24 Feb 2023.
-### Added
+- `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations (#35)
 #### 0.0.2.2
 - Added import of `CompoundSetup` class
 #### 0.0.2
 - `Deck.at()` method for directly referencing slots using either index numbers or names
 - New `CompoundSetup` class for common methods of `Compound` devices
 - New `load_deck()` function to load `Deck` after initialisation
-### Changed
-#### 0.0.2.1
-- Changed template files for `lab.create_setup()`
-#### 0.0.2
-- Update documentation
-
-## 0.0.1.x
-First release of [Control.lab.ly](https://pypi.org/project/control-lab-ly/) distributed on 23 Feb 2023.
-### Added
+#### 0.0.1
 - Make
   - Multi-channel spin-coater \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - Precision mass balance \[Arduino\]
 - Move
@@ -438,9 +438,20 @@
   - Web cameras \[General\] 
 - misc
   - Helper class for most common actions
   - create_configs: make new directory for configuration files
   - create_setup: make new directory for specific setup-related files
   - load_setup: initialise setup on import during runtime
 
-## 0.0.0.x
-Pre-release packaging checks
+### Changed
+#### 0.0.4
+- Update documentation
+#### 0.0.3.1
+- Update documentation
+#### 0.0.3
+- `Sartorius`
+  - made the blowout/home optional for the dispense method upon emptying the pipette
+- Update documentation
+#### 0.0.2.1
+- Changed template files for `lab.create_setup()`
+#### 0.0.2
+- Update documentation
```

### Comparing `control-lab-ly-1.0.1a3/docs/CHANGELOG.md` & `control-lab-ly-1.1.0a0/docs/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 # Change Log
 
 ## Unreleased
 *Items under development*
+### 1.1.0
+- Integration for orbital shaker \[QInstruments\]
+- Integration for pH meter probe \[Sentron\]
+- Integration for force sensor
 
-## 1.0.0.x
+
+## Version 1.0.1
+Bug fixes and minor feature enhancements. First released 08 May 2023.
+### Added
+- `LiquidMover`
+  - Added `LiquidMover.touchTip()` method to touch the pipette tip against the walls of the vessel to remove excess liquid on the outside of the tip (#62)
+  - Added option to indicate the position of the first available pipette tip in `LiquidMover` (#61)
+- Added adaptive GUI controls for `Liquid` objects (#70)
+- Added option to indicate which digital IO channel to use with Dobot attachments (#53)
+### Changed
+- `MassBalance`
+  - Updated to the use `pd.concat()` instead of `pd.DataFrame.append()`, which is going ot be deprecated (#63)
+  - Fixed endless loop for when `MassBalance` tries to `zero()` while recording data (#60)
+- Changed the `Image` class and methods into functions within a module (#54)
+- Fixed the tool offset of pipette when pipette tip is attached, and accounts for the length of pipette that enters the pipette tip (#64)
+- Changed to using more precise time interval measurements by moving from `time.time()` to `time.perf_counter()` (#68)
+- Fixed discrepancy in aspirate and dispense speed for `Sartorius` (#73) and let speed return to a global default value (#72)
+- Updated documentation
+
+
+## Version 1.0.0
 Major overhaul in package structure. Standardisation of methods and consolidation of common methods. First released 12 Apr 2023.
 ### Added
-#### 1.0.0
-- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing
-- Usage of Protocols to provide an interface between different classes of objects
+- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing (#31)
+- Usage of Protocols to provide an interface between different classes of objects (#30)
 - Usage of Dataclasses to store complex data 
 - Usage of decorators to modify methods
 - Introduced different functions to parse the program docstring and find program parameters
 ### Changed
-#### 1.0.0
 - Standardised methods and consolidated common methods
-- Added type hints
+- Added type hints (#28)
 - Moved Dobot attachments from Mover to Transfer.Substrate
 - Split GUI Panels into individual files
 - Split Dobot arms into individual files
 - Split functions/methods in `misc.py` into individual files.
 - Changed `_flags` to a public attribute `flags`
-- Update documentation
+- Update documentation (#27, #28, #29)
 ### Removed
-#### 1.0.0
 - Unnecessary commented-out blocks of code
 
-## 0.0.4.x
-Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.
+
+## Version 0.0.x
+(0.0.4.x) Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.\
+(0.0.3.x) Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.\
+(0.0.2.x) Updates in setting up configuration files. First released 24 Feb 2023.\
+(0.0.1.x) First release of [Control.lab.ly](https://pypi.org/project/control-lab-ly/) distributed on 23 Feb 2023.\
+(0.0.0.x) Pre-release packaging checks
 ### Added
 #### 0.0.4
-- Added control for `Peltier`
+- Added control for `Peltier` (#23)
   - set and get temperatures
   - hold temperatures for desired duration
   - checks if target temperature has been reached by checking power level lower than a threshold or time passed over a predefined duration, once the temperature is within tolerance
   - ability to record temperatures and timestamps 
-- Added control for `TriContinent` and `TriContinentEnsemble`
+- Added control for `TriContinent` and `TriContinentEnsemble` (#25)
   - single actions such as `empty`, `fill`, `initialise`, move actions, set speeds and valves, and wait
   - compound actions such as `aspirate`, `dispense`, and `prime`
-### Changed
-#### 0.0.4
-- Update documentation
-
-## 0.0.3.x
-Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.
-### Added
 #### 0.0.3
-- Added safety measures for movement actions
+- Added safety measures for movement actions (#24)
   - In `Deck`, added exclusion zones when reading the `layout.json` file and new method `is_excluded()` to check if target coordinate is within the exclusion zone
   - In `Mover`, update `isFeasible()` method to check if target coordinates violates the deck's exclusion zone
   - New function `set_safety()` defines safety modes when starting a new session to pause for input (in "high" safety setting) and to wait for safety countdown (in "low" safety setting)
-- `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations
-### Changed
-#### 0.0.3.1
-- Update documentation
-#### 0.0.3
-- `Sartorius`
-  - made the blowout/home optional for the dispense method upon emptying the pipette
-- Update documentation
-
-## 0.0.2.x
-Updates in setting up configuration files. First released 24 Feb 2023.
-### Added
+- `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations (#35)
 #### 0.0.2.2
 - Added import of `CompoundSetup` class
 #### 0.0.2
 - `Deck.at()` method for directly referencing slots using either index numbers or names
 - New `CompoundSetup` class for common methods of `Compound` devices
 - New `load_deck()` function to load `Deck` after initialisation
-### Changed
-#### 0.0.2.1
-- Changed template files for `lab.create_setup()`
-#### 0.0.2
-- Update documentation
-
-## 0.0.1.x
-First release of [Control.lab.ly](https://pypi.org/project/control-lab-ly/) distributed on 23 Feb 2023.
-### Added
+#### 0.0.1
 - Make
   - Multi-channel spin-coater \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - Precision mass balance \[Arduino\]
 - Move
@@ -96,9 +96,20 @@
   - Web cameras \[General\] 
 - misc
   - Helper class for most common actions
   - create_configs: make new directory for configuration files
   - create_setup: make new directory for specific setup-related files
   - load_setup: initialise setup on import during runtime
 
-## 0.0.0.x
-Pre-release packaging checks
+### Changed
+#### 0.0.4
+- Update documentation
+#### 0.0.3.1
+- Update documentation
+#### 0.0.3
+- `Sartorius`
+  - made the blowout/home optional for the dispense method upon emptying the pipette
+- Update documentation
+#### 0.0.2.1
+- Changed template files for `lab.create_setup()`
+#### 0.0.2
+- Update documentation
```

### Comparing `control-lab-ly-1.0.1a3/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.1.0a0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/docs/LICENSE.md` & `control-lab-ly-1.1.0a0/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/docs/README.md` & `control-lab-ly-1.1.0a0/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/setup.cfg` & `control-lab-ly-1.1.0a0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
-00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e31 2d61 330d 0a64 6573 6372 6970 7469  .1-a3..descripti
-00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
-00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
-00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
-00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
-00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
-000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000b0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000c0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000d0: 0d0a 6175 7468 6f72 203d 2043 6861 6e67  ..author = Chang
-000000e0: 204a 6965 204c 656f 6e67 0d0a 6175 7468   Jie Leong..auth
-000000f0: 6f72 5f65 6d61 696c 203d 2063 6861 6e67  or_email = chang
-00000100: 6a69 652e 6c65 6f6e 6740 6f75 746c 6f6f  jie.leong@outloo
-00000110: 6b2e 636f 6d0d 0a75 726c 203d 2068 7474  k.com..url = htt
-00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000130: 6b79 6c65 6a65 616e 6c65 7769 732f 636f  kylejeanlewis/co
-00000140: 6e74 726f 6c2d 6c61 622d 6c65 0d0a 7072  ntrol-lab-le..pr
-00000150: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000160: 4769 7448 7562 203d 2068 7474 7073 3a2f  GitHub = https:/
-00000170: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
-00000180: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
-00000190: 6c2d 6c61 622d 6c65 0d0a 0944 6f63 756d  l-lab-le...Docum
-000001a0: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
-000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
-000001c0: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
-000001d0: 726f 6c2d 6c61 622d 6c65 2f62 6c6f 622f  rol-lab-le/blob/
-000001e0: 6d61 696e 2f64 6f63 732f 5245 4144 4d45  main/docs/README
-000001f0: 2e6d 640d 0a09 4368 616e 6765 6c6f 6720  .md...Changelog 
-00000200: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000210: 2e63 6f6d 2f6b 796c 656a 6561 6e6c 6577  .com/kylejeanlew
-00000220: 6973 2f63 6f6e 7472 6f6c 2d6c 6162 2d6c  is/control-lab-l
-00000230: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
-00000240: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a09  /CHANGELOG.md...
-00000250: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
-00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
-00000270: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
-00000280: 6f6c 2d6c 6162 2d6c 652f 6973 7375 6573  ol-lab-le/issues
-00000290: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
-000002a0: 0a6b 6579 776f 7264 7320 3d20 0d0a 0970  .keywords = ...p
-000002b0: 7974 686f 6e0d 0a09 6c61 6220 6175 746f  ython...lab auto
-000002c0: 6d61 7469 6f6e 0d0a 636c 6173 7369 6669  mation..classifi
-000002d0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000002e0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000002f0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-00000300: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000310: 4465 7665 6c6f 7065 7273 0d0a 0949 6e74  Developers...Int
-00000320: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000330: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000340: 6368 0d0a 094c 6963 656e 7365 203a 3a20  ch...License :: 
-00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000360: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-00000370: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000380: 3a20 4d69 6372 6f73 6f66 7420 3a3a 2057  : Microsoft :: W
-00000390: 696e 646f 7773 0d0a 0950 726f 6772 616d  indows...Program
-000003a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000003c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003e0: 2033 2e38 0d0a 0954 6f70 6963 203a 3a20   3.8...Topic :: 
-000003f0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
-00000400: 6565 7269 6e67 0d0a 0d0a 5b6f 7074 696f  eering....[optio
-00000410: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-00000420: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-00000430: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
-00000440: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000450: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
-00000460: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000470: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
-00000480: 7569 7265 7320 3d20 0d0a 0964 6173 683e  uires = ...dash>
-00000490: 3d32 2e37 0d0a 0969 6d70 6564 616e 6365  =2.7...impedance
-000004a0: 3e3d 312e 340d 0a09 696d 7574 696c 733e  >=1.4...imutils>
-000004b0: 3d30 2e35 0d0a 096d 6174 706c 6f74 6c69  =0.5...matplotli
-000004c0: 623e 3d33 2e33 0d0a 096e 6573 745f 6173  b>=3.3...nest_as
-000004d0: 796e 6369 6f3e 3d31 2e35 0d0a 096e 756d  yncio>=1.5...num
-000004e0: 7079 3e3d 312e 3139 0d0a 096f 7065 6e63  py>=1.19...openc
-000004f0: 765f 7079 7468 6f6e 3e3d 342e 352e 300d  v_python>=4.5.0.
-00000500: 0a09 7061 6e64 6173 3e3d 312e 320d 0a09  ..pandas>=1.2...
-00000510: 706c 6f74 6c79 3e3d 352e 330d 0a09 7079  plotly>=5.3...py
-00000520: 4d6f 6462 7573 5443 503e 3d30 2e32 0d0a  ModbusTCP>=0.2..
-00000530: 0970 7973 6572 6961 6c3e 3d33 2e35 0d0a  .pyserial>=3.5..
-00000540: 0950 7953 696d 706c 6547 5549 3e3d 342e  .PySimpleGUI>=4.
-00000550: 3630 0d0a 0950 7956 4953 413e 3d31 2e31  60...PyVISA>=1.1
-00000560: 320d 0a09 5079 5941 4d4c 3e3d 362e 300d  2...PyYAML>=6.0.
-00000570: 0a09 7363 6970 793e 3d31 2e36 0d0a 0d0a  ..scipy>=1.6....
-00000580: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000590: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000005a0: 2073 7263 0d0a 6578 636c 7564 6520 3d20   src..exclude = 
-000005b0: 7465 7374 730d 0a0d 0a5b 6f70 7469 6f6e  tests....[option
-000005c0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-000005d0: 0a2a 203d 202a 2e6a 736f 6e2c 202a 2e79  .* = *.json, *.y
-000005e0: 616d 6c2c 202a 2e70 6e67 0d0a 0d0a 5b65  aml, *.png....[e
-000005f0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000600: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000610: 203d 2030 0d0a 0d0a                       = 0....
+00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e31  y..version = 1.1
+00000030: 2e30 2d61 0d0a 6465 7363 7269 7074 696f  .0-a..descriptio
+00000040: 6e20 3d20 4c61 6220 4571 7569 706d 656e  n = Lab Equipmen
+00000050: 7420 4175 746f 6d61 7469 6f6e 2050 6163  t Automation Pac
+00000060: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
+00000070: 6970 7469 6f6e 203d 2066 696c 653a 2064  iption = file: d
+00000080: 6f63 732f 5245 4144 4d45 2e6d 642c 2064  ocs/README.md, d
+00000090: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
+000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000b0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000c0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000d0: 0a61 7574 686f 7220 3d20 4368 616e 6720  .author = Chang 
+000000e0: 4a69 6520 4c65 6f6e 670d 0a61 7574 686f  Jie Leong..autho
+000000f0: 725f 656d 6169 6c20 3d20 6368 616e 676a  r_email = changj
+00000100: 6965 2e6c 656f 6e67 406f 7574 6c6f 6f6b  ie.leong@outlook
+00000110: 2e63 6f6d 0d0a 7572 6c20 3d20 6874 7470  .com..url = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+00000130: 796c 656a 6561 6e6c 6577 6973 2f63 6f6e  ylejeanlewis/con
+00000140: 7472 6f6c 2d6c 6162 2d6c 650d 0a70 726f  trol-lab-le..pro
+00000150: 6a65 6374 5f75 726c 7320 3d20 0d0a 0947  ject_urls = ...G
+00000160: 6974 4875 6220 3d20 6874 7470 733a 2f2f  itHub = https://
+00000170: 6769 7468 7562 2e63 6f6d 2f6b 796c 656a  github.com/kylej
+00000180: 6561 6e6c 6577 6973 2f63 6f6e 7472 6f6c  eanlewis/control
+00000190: 2d6c 6162 2d6c 650d 0a09 446f 6375 6d65  -lab-le...Docume
+000001a0: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
+000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+000001c0: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+000001d0: 6f6c 2d6c 6162 2d6c 652f 626c 6f62 2f6d  ol-lab-le/blob/m
+000001e0: 6169 6e2f 646f 6373 2f52 4541 444d 452e  ain/docs/README.
+000001f0: 6d64 0d0a 0943 6861 6e67 656c 6f67 203d  md...Changelog =
+00000200: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000210: 636f 6d2f 6b79 6c65 6a65 616e 6c65 7769  com/kylejeanlewi
+00000220: 732f 636f 6e74 726f 6c2d 6c61 622d 6c65  s/control-lab-le
+00000230: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+00000240: 4348 414e 4745 4c4f 472e 6d64 0d0a 0954  CHANGELOG.md...T
+00000250: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+00000260: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
+00000270: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
+00000280: 6c2d 6c61 622d 6c65 2f69 7373 7565 730d  l-lab-le/issues.
+00000290: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
+000002a0: 6b65 7977 6f72 6473 203d 200d 0a09 7079  keywords = ...py
+000002b0: 7468 6f6e 0d0a 096c 6162 2061 7574 6f6d  thon...lab autom
+000002c0: 6174 696f 6e0d 0a63 6c61 7373 6966 6965  ation..classifie
+000002d0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
+000002e0: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
+000002f0: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
+00000300: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+00000310: 6576 656c 6f70 6572 730d 0a09 496e 7465  evelopers...Inte
+00000320: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000330: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+00000340: 680d 0a09 4c69 6365 6e73 6520 3a3a 204f  h...License :: O
+00000350: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000360: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000370: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000380: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
+00000390: 6e64 6f77 730d 0a09 5072 6f67 7261 6d6d  ndows...Programm
+000003a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003b0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
+000003c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000003d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003e0: 332e 380d 0a09 546f 7069 6320 3a3a 2053  3.8...Topic :: S
+000003f0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000400: 6572 696e 670d 0a0d 0a5b 6f70 7469 6f6e  ering....[option
+00000410: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000420: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000430: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+00000440: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000450: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
+00000460: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000470: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
+00000480: 6972 6573 203d 200d 0a09 6461 7368 3e3d  ires = ...dash>=
+00000490: 322e 370d 0a09 696d 7065 6461 6e63 653e  2.7...impedance>
+000004a0: 3d31 2e34 0d0a 0969 6d75 7469 6c73 3e3d  =1.4...imutils>=
+000004b0: 302e 350d 0a09 6d61 7470 6c6f 746c 6962  0.5...matplotlib
+000004c0: 3e3d 332e 330d 0a09 6e65 7374 5f61 7379  >=3.3...nest_asy
+000004d0: 6e63 696f 3e3d 312e 350d 0a09 6e75 6d70  ncio>=1.5...nump
+000004e0: 793e 3d31 2e31 390d 0a09 6f70 656e 6376  y>=1.19...opencv
+000004f0: 5f70 7974 686f 6e3e 3d34 2e35 2e30 0d0a  _python>=4.5.0..
+00000500: 0970 616e 6461 733e 3d31 2e32 0d0a 0970  .pandas>=1.2...p
+00000510: 6c6f 746c 793e 3d35 2e33 0d0a 0970 794d  lotly>=5.3...pyM
+00000520: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
+00000530: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
+00000540: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
+00000550: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
+00000560: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
+00000570: 0973 6369 7079 3e3d 312e 360d 0a0d 0a5b  .scipy>=1.6....[
+00000580: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000590: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+000005a0: 7372 630d 0a65 7863 6c75 6465 203d 2074  src..exclude = t
+000005b0: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
+000005c0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+000005d0: 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e 7961  * = *.json, *.ya
+000005e0: 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b 6567  ml, *.png....[eg
+000005f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000600: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000610: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.1a3
+Version: 1.1.0a0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -340,89 +340,89 @@
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
 ## Unreleased
 *Items under development*
+### 1.1.0
+- Integration for orbital shaker \[QInstruments\]
+- Integration for pH meter probe \[Sentron\]
+- Integration for force sensor
 
-## 1.0.0.x
+
+## Version 1.0.1
+Bug fixes and minor feature enhancements. First released 08 May 2023.
+### Added
+- `LiquidMover`
+  - Added `LiquidMover.touchTip()` method to touch the pipette tip against the walls of the vessel to remove excess liquid on the outside of the tip (#62)
+  - Added option to indicate the position of the first available pipette tip in `LiquidMover` (#61)
+- Added adaptive GUI controls for `Liquid` objects (#70)
+- Added option to indicate which digital IO channel to use with Dobot attachments (#53)
+### Changed
+- `MassBalance`
+  - Updated to the use `pd.concat()` instead of `pd.DataFrame.append()`, which is going ot be deprecated (#63)
+  - Fixed endless loop for when `MassBalance` tries to `zero()` while recording data (#60)
+- Changed the `Image` class and methods into functions within a module (#54)
+- Fixed the tool offset of pipette when pipette tip is attached, and accounts for the length of pipette that enters the pipette tip (#64)
+- Changed to using more precise time interval measurements by moving from `time.time()` to `time.perf_counter()` (#68)
+- Fixed discrepancy in aspirate and dispense speed for `Sartorius` (#73) and let speed return to a global default value (#72)
+- Updated documentation
+
+
+## Version 1.0.0
 Major overhaul in package structure. Standardisation of methods and consolidation of common methods. First released 12 Apr 2023.
 ### Added
-#### 1.0.0
-- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing
-- Usage of Protocols to provide an interface between different classes of objects
+- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing (#31)
+- Usage of Protocols to provide an interface between different classes of objects (#30)
 - Usage of Dataclasses to store complex data 
 - Usage of decorators to modify methods
 - Introduced different functions to parse the program docstring and find program parameters
 ### Changed
-#### 1.0.0
 - Standardised methods and consolidated common methods
-- Added type hints
+- Added type hints (#28)
 - Moved Dobot attachments from Mover to Transfer.Substrate
 - Split GUI Panels into individual files
 - Split Dobot arms into individual files
 - Split functions/methods in `misc.py` into individual files.
 - Changed `_flags` to a public attribute `flags`
-- Update documentation
+- Update documentation (#27, #28, #29)
 ### Removed
-#### 1.0.0
 - Unnecessary commented-out blocks of code
 
-## 0.0.4.x
-Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.
+
+## Version 0.0.x
+(0.0.4.x) Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.\
+(0.0.3.x) Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.\
+(0.0.2.x) Updates in setting up configuration files. First released 24 Feb 2023.\
+(0.0.1.x) First release of [Control.lab.ly](https://pypi.org/project/control-lab-ly/) distributed on 23 Feb 2023.\
+(0.0.0.x) Pre-release packaging checks
 ### Added
 #### 0.0.4
-- Added control for `Peltier`
+- Added control for `Peltier` (#23)
   - set and get temperatures
   - hold temperatures for desired duration
   - checks if target temperature has been reached by checking power level lower than a threshold or time passed over a predefined duration, once the temperature is within tolerance
   - ability to record temperatures and timestamps 
-- Added control for `TriContinent` and `TriContinentEnsemble`
+- Added control for `TriContinent` and `TriContinentEnsemble` (#25)
   - single actions such as `empty`, `fill`, `initialise`, move actions, set speeds and valves, and wait
   - compound actions such as `aspirate`, `dispense`, and `prime`
-### Changed
-#### 0.0.4
-- Update documentation
-
-## 0.0.3.x
-Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.
-### Added
 #### 0.0.3
-- Added safety measures for movement actions
+- Added safety measures for movement actions (#24)
   - In `Deck`, added exclusion zones when reading the `layout.json` file and new method `is_excluded()` to check if target coordinate is within the exclusion zone
   - In `Mover`, update `isFeasible()` method to check if target coordinates violates the deck's exclusion zone
   - New function `set_safety()` defines safety modes when starting a new session to pause for input (in "high" safety setting) and to wait for safety countdown (in "low" safety setting)
-- `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations
-### Changed
-#### 0.0.3.1
-- Update documentation
-#### 0.0.3
-- `Sartorius`
-  - made the blowout/home optional for the dispense method upon emptying the pipette
-- Update documentation
-
-## 0.0.2.x
-Updates in setting up configuration files. First released 24 Feb 2023.
-### Added
+- `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations (#35)
 #### 0.0.2.2
 - Added import of `CompoundSetup` class
 #### 0.0.2
 - `Deck.at()` method for directly referencing slots using either index numbers or names
 - New `CompoundSetup` class for common methods of `Compound` devices
 - New `load_deck()` function to load `Deck` after initialisation
-### Changed
-#### 0.0.2.1
-- Changed template files for `lab.create_setup()`
-#### 0.0.2
-- Update documentation
-
-## 0.0.1.x
-First release of [Control.lab.ly](https://pypi.org/project/control-lab-ly/) distributed on 23 Feb 2023.
-### Added
+#### 0.0.1
 - Make
   - Multi-channel spin-coater \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - Precision mass balance \[Arduino\]
 - Move
@@ -438,9 +438,20 @@
   - Web cameras \[General\] 
 - misc
   - Helper class for most common actions
   - create_configs: make new directory for configuration files
   - create_setup: make new directory for specific setup-related files
   - load_setup: initialise setup on import during runtime
 
-## 0.0.0.x
-Pre-release packaging checks
+### Changed
+#### 0.0.4
+- Update documentation
+#### 0.0.3.1
+- Update documentation
+#### 0.0.3
+- `Sartorius`
+  - made the blowout/home optional for the dispense method upon emptying the pipette
+- Update documentation
+#### 0.0.2.1
+- Changed template files for `lab.create_setup()`
+#### 0.0.2
+- Update documentation
```

### Comparing `control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,35 @@
 src/controllably/Compound/LiquidMover/__init__.py
 src/controllably/Compound/LiquidMover/liquidmover_utils.py
 src/controllably/Compound/LiquidMover/Opentrons/__init__.py
 src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
 src/controllably/Control/__init__.py
 src/controllably/Control/GUI/__init__.py
 src/controllably/Control/GUI/_guibuilder.py
+src/controllably/Control/GUI/compound_panel.py
 src/controllably/Control/GUI/gui_utils.py
+src/controllably/Control/GUI/liquid_panel.py
 src/controllably/Control/GUI/loader_panel.py
 src/controllably/Control/GUI/measurer_panel.py
 src/controllably/Control/GUI/mover_panel.py
 src/controllably/Control/GUI/viewer_panel.py
 src/controllably/Control/Schedule/__init__.py
 src/controllably/Control/Schedule/schedule_utils.py
 src/controllably/Make/__init__.py
 src/controllably/Make/make_utils.py
 src/controllably/Make/Heat/__init__.py
 src/controllably/Make/Heat/peltier_utils.py
 src/controllably/Make/Light/__init__.py
 src/controllably/Make/Light/led_utils.py
 src/controllably/Make/Mixture/__init__.py
+src/controllably/Make/Mixture/QInstruments/__init__.py
+src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
 src/controllably/Make/ThinFilm/__init__.py
 src/controllably/Make/ThinFilm/spinner_utils.py
 src/controllably/Measure/__init__.py
 src/controllably/Measure/instrument_utils.py
 src/controllably/Measure/measure_utils.py
 src/controllably/Measure/program_utils.py
 src/controllably/Measure/Electrical/__init__.py
@@ -152,10 +159,11 @@
 tests/test_film_spin.py
 tests/test_heat_peltier.py
 tests/test_light_led_array.py
 tests/test_liquid_sartorius.py
 tests/test_liquid_syringe_assembly.py
 tests/test_liquid_tricontinent.py
 tests/test_mechanical_piezorobotics.py
+tests/test_mixture_shaker.py
 tests/test_panels.py
 tests/test_physical_balance.py
 tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 This sub-package imports the base class for control panels as well as basic panels
 for measurers, movers, and viewers.
 
 Classes:
     Panel (ABC)
     CompoundPanel (Panel)
+    LiquidPanel (Panel)
     MeasurerPanel (Panel)
     MoverPanel (Panel)
+    MultiChannelPanel (Panel)
     ViewerPanel (Panel)
 """
-from .gui_utils import Panel, CompoundPanel
+from .gui_utils import Panel, MultiChannelPanel
+from .compound_panel import CompoundPanel
+from .liquid_panel import LiquidPanel
 from .measurer_panel import MeasurerPanel
 from .mover_panel import MoverPanel
 from .viewer_panel import ViewerPanel
 
 from controllably import include_this_module
 include_this_module(get_local_only=False)
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/gui_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the base class for control panels as well as compound panels.
+This module holds the base class for control panels as well as multichannel panels.
 
 Classes:
     Panel (ABC)
-    CompoundPanel (Panel)
+    MultiChannelPanel (Panel)
     
 Other constants and variables:
     HEIGHT (int): height of screen size in number of pixels
     WIDTH (int): width of screen size in number of pixels
 """
 # Standard library imports
 from __future__ import annotations
@@ -55,14 +55,15 @@
     - `getLayout`: build `sg.Column` object
     - `listenEvents`: listen to events and act on values
     #### Public
     - `arrangeElements`: arrange elements in a horizontal, vertical, or cross-shape pattern
     - `close`: exit the application
     - `configure`: configure GUI defaults
     - `getButtons`: get a list of panel buttons
+    - `getInputs`: get the layout for the input section
     - `getWindow`: build `sg.Window` object
     - `pad`: add spacer in GUI
     - `parseInput`: parse inputs from GUI
     - `runGUI`: run the GUI loop
     - `setFlag`: set flags by using keyword arguments
     """
     
@@ -226,46 +227,83 @@
     @staticmethod
     def getButtons(
         labels: list[str], 
         size: Union[int, tuple], 
         key_prefix: str, 
         font: tuple[str, int], 
         texts: Optional[list[str]] = None, 
+        tooltips: Optional[list[str]] = None, 
         **kwargs
     ) -> list[sg.Button]:
         """
         Get list of panel buttons
 
         Args:
             labels (list[str]): list of button labels
             size (Union[int, tuple]): button width (,height)
             key_prefix (str): prefix of button key
             font (tuple[str, int]): (typeface, font size)
             texts (Optional[list[str]], optional): alternative text labels for buttons. Defaults to None.
-
+            tooltips (Optional[list[str]], optional): tooltip labels for buttons. Defaults to None.
+            
         Returns:
-            list: list of PySimpleGUI.Button objects
+            list[sg.Button]: list of buttons
         """
         texts = [] if texts is None else texts
+        tooltips = [] if tooltips is None else tooltips
         buttons = []
         specials = kwargs.pop('specials', {})
         for i,label in enumerate(labels):
             key_string = label.replace('\n','')
             key = f"-{key_prefix}-{key_string}-" if key_prefix else f"-{key_string}-"
             kw = kwargs.copy()
             if label in specials.keys():
                 for k,v in specials[label].items():
                     kw[k] = v
-            if len(texts):
-                try:
-                    label = texts[i]
-                except IndexError:
-                    pass
-            buttons.append(sg.Button(label, size=size, key=key, font=font, **kw))
+            label = texts[i] if i<len(texts) else label
+            tooltip = tooltips[i] if i<len(tooltips) else None
+            buttons.append(sg.Button(label, size=size, key=key, font=font, tooltip=tooltip, **kw))
         return buttons
+    
+    @staticmethod
+    def getInputs(fields:list[str], key_prefix: str) -> list[sg.Column]:
+        """
+        Get the layout for the input section
+        
+        Args:
+            fields (list[str]): list of field names
+            key_prefix (str): prefix of button key
+
+        Returns:
+            list[sg.Column]: list of columns
+        """
+        # template for procedurally adding input fields
+        labels = []
+        inputs = []
+        for input_field in fields:
+            key_label = f'-{key_prefix}-{input_field.upper()}-LABEL-'
+            key_input = f'-{key_prefix}-{input_field.upper()}-VALUE-'
+            _label = sg.pin(
+                sg.Column(
+                    [[sg.Text(input_field.title(), key=key_label, visible=True)]],
+                    key=f'{key_label}BOX-', visible=True
+                )
+            )
+            _input = sg.pin(
+                sg.Column(
+                    [[sg.Input(size=(5,2), key=key_input, visible=True, tooltip='')]],
+                    key=f'{key_input}BOX-', visible=True
+                )
+            )
+            labels.append([_label])
+            inputs.append([_input])
+        labels_column = sg.Column(labels, justification='right', pad=10, visible=True)
+        inputs_column = sg.Column(inputs, justification='left', pad=10, visible=True)
+        labels_inputs = [labels_column, inputs_column]
+        return labels_inputs
 
     def getWindow(self, title:str = 'Application', **kwargs) -> sg.Window:
         """
         Build `sg.Window` object
 
         Args:
             title (str, optional): title of window. Defaults to 'Application'.
@@ -384,125 +422,91 @@
 
         Returns:
             str: mangled text
         """
         return f'-{self.name}{text}'
     
 
-class CompoundPanel(Panel):
+class MultiChannelPanel(Panel):
     """
-    CompoundPanel provides methods to form a multi-tool control panel
+    Abstract Base Class (ABC) for Multi-Channel Panel objects (i.e. GUI panels for tools with multiple channels).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
 
     ### Constructor
     Args:
-        `ensemble` (dict[str, Panel]): dictionary of individual sub-panels
+        `name` (str, optional): name of panel. Defaults to ''.
         `group` (Optional[str], optional): name of group. Defaults to None.
-        
-    ### Attributes
-    - `panels` (dict[str, Panel]): dictionary of individual sub-panels
     
     ### Methods
-    - `close`: exit the application
-    - `getLayout`: build `sg.Column` object
+    #### Abstract
+    - `getChannelPanel`: get the panel layout for a single channel
     - `listenEvents`: listen to events and act on values
+    #### Public
+    - `getLayout`: build `sg.Column` object
     """
     
-    def __init__(self, 
-        ensemble: dict[str, Panel],
-        group: Optional[str] = None,
-        **kwargs
-    ):
+    def __init__(self, name:str = '', group:Optional[str] = None):
         """
         Instantiate the class
 
         Args:
-            ensemble (dict[str, Panel]): dictionary of individual sub-panels
+            name (str, optional): name of panel. Defaults to ''.
             group (Optional[str], optional): name of group. Defaults to None.
         """
-        super().__init__(group=group, **kwargs)
-        self.panels = {key: value for key,value in ensemble.items()}
+        super().__init__(name=name, group=group)
         return
     
-    def close(self):
-        """Exit the application"""
-        for panel in self.panels.values():
-            panel.close()
-        return super().close()
-    
-    def getLayout(self, title:str = 'Control Panel', title_font_level:int = 0, **kwargs) -> sg.Column:
+    @abstractmethod
+    def getChannelPanel(self, channel_id:int, tool:object, **kwargs) -> sg.Column:
+        """
+        Get the panel layout for a single channel
+
+        Args:
+            channel_id (int): channel index
+            tool (object): tool object
+
+        Returns:
+            sg.Column: Column object
+        """
+        
+    def getLayout(self, title:str = 'Tool Control', title_font_level:int = 1, **kwargs) -> sg.Column:
         """
         Build `sg.Column` object
 
         Args:
-            title (str, optional): title of layout. Defaults to 'Control Panel'.
-            title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 0.
+            title (str, optional): title of layout. Defaults to 'Tool Control'.
+            title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 1.
 
         Returns:
             sg.Column: Column object
         """
-        font = (self.typeface, self.font_sizes[title_font_level], 'bold')
+        font = (self.typeface, self.font_sizes[title_font_level])
         layout = super().getLayout(title, justification='center', font=font)
+        channels = {}
+        if 'channels' in dir(self.tool):
+            channels = self.tool.channels
+        else:
+            channels = {self.tool.channel: self.tool}
+        if len(channels) == 0:
+            return layout
         
-        tab_groups = {'main': []}
-        for key, panel in self.panels.items():
-            group = panel.group
-            _layout = panel.getLayout(title_font_level=title_font_level+1)
-            if not group:
-                group = 'main'
-            if group not in tab_groups.keys():
-                tab_groups[group] = []
-            tab_groups[group].append((key, _layout))
-            
-        tab_group_order = ['main', 'viewer', 'mover', 'measurer'] 
-        tab_group_order = tab_group_order + [grp for grp in list(tab_groups.keys()) if grp not in tab_group_order]
-        ordered_tab_groups = OrderedDict()
-        for key in tab_group_order:
-            if key not in tab_groups:
-                continue
-            ordered_tab_groups[key] = tab_groups.get(key)
-        tab_groups = ordered_tab_groups
-        
-        panels = []
-        excluded = ['main']
-        for group, _layouts in tab_groups.items():
-            if group == 'main':
-                panels = panels + [_layout for _,_layout in _layouts]
-                continue
-            if len(_layouts) == 1:
-                panels.append(_layouts[0][1])
-                excluded.append(group)
-            else:
-                tabs = [sg.Tab(key, [[_layout]], expand_x=True) for key,_layout in tab_groups[group]]
-                tab_group = sg.TabGroup([tabs], tab_location='bottomright', key=f'-{group}-TABS-', 
-                                        expand_x=True, expand_y=True)
-                tab_groups[group] = tab_group
-                panels.append(tab_group)
-        # panels = panels + [element for group,element in tab_groups.items() if group not in excluded]
-        panel_list = [panels[0]]
-        for p in range(1, len(panels)):
-            panel_list.append(sg.VerticalSeparator(color="#ffffff", pad=5))
-            panel_list.append(panels[p])
+        channel_panels = []
+        for channel_id, tool in channels.items():
+            _layout = self.getChannelPanel(channel_id, tool)
+            channel_panels.append((channel_id, _layout))
+        if len(channel_panels) == 1:
+            panel = channel_panels[0][1]
+        else:
+            tabs = [sg.Tab(key, [[_layout]], expand_x=True) for key,_layout in channel_panels]
+            panel = sg.TabGroup(
+                [tabs], tab_location='topleft', key=f'-{self.name}-TABS-', 
+                expand_x=True, expand_y=True
+            )
         
-        suite = sg.Column([panel_list], vertical_alignment='top')
+        suite = sg.Column([[panel]], vertical_alignment='top')
         layout = [
             [layout],
+            [sg.Push()],
             [suite]
         ]
         layout = sg.Column(layout, vertical_alignment='top')
         return layout
-    
-    def listenEvents(self, event:str, values:dict[str, str]) -> dict[str, dict]:
-        """
-        Listen to events and act on values
-
-        Args:
-            event (str): event triggered
-            values (dict[str, str]): dictionary of values from window
-
-        Returns:
-            dict: dictionary of updates
-        """
-        updates = {}
-        for panel in self.panels.values():
-            update = panel.listenEvents(event, values)
-            updates.update(update)
-        return updates
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/measurer_panel.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,25 +102,25 @@
             title (str, optional): title of layout. Defaults to 'Panel'.
             title_font_level (int, optional): index of font size from levels in font_sizes. Defaults to 0.
 
         Returns:
             sg.Column: Column object
         """
         font = (self.typeface, self.font_sizes[title_font_level])
-        layout = super().getLayout(f'{self.name} Control', justification='center', font=font)
+        layout = super().getLayout(f'{self.name.title()} Control', justification='center', font=font)
         
         font = (self.typeface, self.font_sizes[title_font_level+1])
         # add dropdown for program list
         dropdown = sg.Combo(
             values=self.measurer.available_programs, size=(20, 1), 
             key=self._mangle('-PROGRAMS-'), enable_events=True, readonly=True
         )
         
         # add template for procedurally adding input fields
-        labels_inputs = self._get_input_section()
+        labels_inputs = self.getInputs(fields=self.measurer.possible_inputs, key_prefix=self.name)
         
         # add run, clear, reset buttons
         layout = [
             [layout],
             [self.pad()],
             [sg.Column([[dropdown]], justification='center')],
             [self.pad()],
@@ -175,47 +175,15 @@
         
         # 4. Clear input fields
         if event == self._mangle('-Clear-'):
             update_part = self._show_inputs(self.measurer.program_details)
             updates.update(update_part)
         return updates
     
-    # Protected method(s)
-    def _get_input_section(self) -> list[sg.Column]:
-        """
-        Get the layout for the input section
-
-        Returns:
-            list[sg.Column]: list of columns
-        """
-        # template for procedurally adding input fields
-        labels = []
-        inputs = []
-        for input_field in self.measurer.possible_inputs:
-            key_label = self._mangle(f'-{input_field}-LABEL-')
-            key_input = self._mangle(f'-{input_field}-VALUE-')
-            _label = sg.pin(
-                sg.Column(
-                    [[sg.Text(input_field.title(), key=key_label, visible=True)]],
-                    key=f'{key_label}BOX-', visible=False
-                )
-            )
-            _input = sg.pin(
-                sg.Column(
-                    [[sg.Input(0, size=(5,2), key=key_input, visible=True, tooltip='')]],
-                    key=f'{key_input}BOX-', visible=False
-                )
-            )
-            labels.append([_label])
-            inputs.append([_input])
-        labels_column = sg.Column(labels, justification='right', pad=10, visible=True)
-        inputs_column = sg.Column(inputs, justification='left', pad=10, visible=True)
-        labels_inputs = [labels_column, inputs_column]
-        return labels_inputs
-    
+    # Protected method(s)    
     def _show_inputs(self, program_details: ProgramDetails) -> dict[str, dict]:
         """
         Show the relevant input fields
 
         Args:
             program_details (ProgramDetails): details of loaded program
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/mover_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,17 +106,17 @@
         Args:
             title_font_level (int, optional): index of font size from levels in font_sizes. Defaults to 1.
 
         Returns:
             sg.Column: Column object
         """
         font = (self.typeface, self.font_sizes[title_font_level])
-        layout = super().getLayout(f'{self.name} Control', justification='center', font=font)
+        layout = super().getLayout(f'{self.name.title()} Control', justification='center', font=font)
         
-        # yaw (alpha, about z-axis), pitch (beta, about x-axis), roll (gamma, about y-axis)
+        # yaw (alpha/a, about z-axis), pitch (beta/b, about x-axis), roll (gamma/c, about y-axis)
         axes = ['X','Y','Z','a','b','c']
         increments = ['-10','-1','-0.1',0,'+0.1','+1','+10']
         center_buttons = ['home']*2 + ['safe'] + ['zero']*3
         font = (self.typeface, self.font_sizes[title_font_level+1])
         color_codes = {
             'X':None, 'Y':None, 'Z':None,
             'a':'#ffffbb', 'b':'#ffbbff', 'c':'#bbffff'
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/viewer_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         Args:
             title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 1.
 
         Returns:
             sg.Column: Column object
         """
         font = (self.typeface, self.font_sizes[title_font_level])
-        layout = super().getLayout(f'{self.name} Control', justification='center', font=font)
+        layout = super().getLayout(f'{self.name.title()} Control', justification='center', font=font)
         layout = [
             [layout],
             [sg.Image(filename='', key=self.display_box, enable_events=True)]
         ]
         layout = sg.Column(layout, vertical_alignment='top')
         return layout
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     COLUMNS (tuple)
 """
 # Standard library imports
 from datetime import datetime
 import pandas as pd
 from threading import Thread
 import time
+from typing import Union
 
 # Third party imports
 import serial   # pip install pyserial
 
 # Local application imports
 from ..make_utils import Maker
 print(f"Import: OK <{__name__}>")
@@ -33,27 +34,27 @@
         `port` (str): COM port of device
         `power_threshold` (float, optional): minimum threshold under which temperature can be considered stable. Defaults to 20.
         `stabilize_buffer_time` (float, optional): buffer time over which temperature can be considered stable. Defaults to 10.
         `tolerance` (float, optional): tolerance above and below target temperature. Defaults to 1.5.
             
     ### Attributes
     - `power_threshold` (float): minimum threshold under which temperature can be considered stable
-    - `set_point` (float): temperature set point
+    - `set_temperature` (float): temperature set point
     - `stabilize_buffer_time` (float): buffer time over which temperature can be considered stable
     - `temperature` (float): temperature at sample site
     - `tolerance` (float): tolerance above and below target temperature
     
     ### Properties
     - `port`: COM port of device
     
     ### Methods
     - `clearCache`: clears and remove data in buffer
-    - `getTemperatures`: retrieve temperatures from device
+    - `getTemperature`: retrieve temperatures from device
     - `holdTemperature`: hold target temperature for desired duration
-    - `isReady`: checks and returns whether target temperature has been reached
+    - `isAtTemperature`: checks and returns whether target temperature has been reached
     - `reset`: reset the device
     - `setTemperature`: set a target temperature
     - `shutdown`: shutdown procedure for tool
     - `toggleFeedbackLoop`: start or stop feedback loop
     - `toggleRecord`: start or stop data recording
     """
     
@@ -89,15 +90,15 @@
         self.tolerance = tolerance
         
         self._columns = list(COLUMNS)
         self._stabilize_time = None
         self._threads = {}
         
         # Device read-outs
-        self.set_point = None
+        self.set_temperature = None
         self.temperature = None
         self._cold_point = None
         self._power = None
         self._connect(port)
         return
     
     # Properties
@@ -109,42 +110,43 @@
         """Clears and remove data in buffer"""
         self.setFlag(pause_feedback=True)
         time.sleep(0.1)
         self.buffer_df = pd.DataFrame(columns=self._columns)
         self.setFlag(pause_feedback=False)
         return
     
-    def getTemperatures(self) -> str:
+    def getTemperature(self) -> Union[tuple, str]:
         """
         Retrieve temperatures from device 
         Including the set temperature, hot temperature, cold temperature, and the power level
         
         Returns:
-            str: response from device
+            Union[tuple, str]: response from device
         """
         response = self._read()
         now = datetime.now()
         try:
             values = [float(v) for v in response.split(';')]
-            self.set_point, self.temperature, self._cold_point, self._power = values
+            self.set_temperature, self.temperature, self._cold_point, self._power = values
         except ValueError:
             pass
         else:
-            ready = (abs(self.set_point - self.temperature)<=self.tolerance)
+            response = tuple(values)
+            ready = (abs(self.set_temperature - self.temperature)<=self.tolerance)
             if not ready:
                 pass
             elif not self._stabilize_time:
                 self._stabilize_time = time.perf_counter()
                 print(response)
             elif self.flags['temperature_reached']:
                 pass
             elif (self._power <= self.power_threshold) or (time.perf_counter()-self._stabilize_time >= self.stabilize_buffer_time):
                 print(response)
                 self.setFlag(temperature_reached=True)
-                print(f"Temperature of {self.set_point}°C reached!")
+                print(f"Temperature of {self.set_temperature}°C reached!")
             if self.flags['record']:
                 values = [now] + values
                 row = {k:v for k,v in zip(self._columns, values)}
                 # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
                 new_row_df = pd.DataFrame(row)
                 self.buffer_df = pd.concat([self.buffer_df, new_row_df])
         return response
@@ -154,61 +156,61 @@
         Hold target temperature for desired duration
 
         Args:
             temperature (float): temperature in degree Celsius
             time_s (float): duration in seconds
         """
         self.setTemperature(temperature)
-        print(f"Holding at {self.set_point}°C for {time_s} seconds")
+        print(f"Holding at {self.set_temperature}°C for {time_s} seconds")
         time.sleep(time_s)
         print(f"End of temperature hold")
         return
     
-    def isReady(self) -> bool:
+    def isAtTemperature(self) -> bool:
         """
         Checks and returns whether target temperature has been reached
 
         Returns:
             bool: whether target temperature has been reached
         """
         return self.flags['temperature_reached']
     
     def reset(self):
         """Reset the device"""
         self.toggleRecord(False)
         self.clearCache()
-        self.setTemperature(set_point=25, blocking=False)
+        self.setTemperature(temperature=25, blocking=False)
         return
     
-    def setTemperature(self, set_point:int, blocking:bool = True):
+    def setTemperature(self, temperature:int, blocking:bool = True):
         """
         Set a temperature
 
         Args:
-            set_point (int): target temperature in degree Celsius
+            temperature (int): target temperature in degree Celsius
             blocking (bool, optional): whether to wait for temperature to reach set point. Defaults to True.
         """
         self.setFlag(pause_feedback=True)
         time.sleep(0.5)
         try:
-            self.device.write(bytes(f"{set_point}\n", 'utf-8'))
+            self.device.write(bytes(f"{temperature}\n", 'utf-8'))
         except AttributeError:
             pass
         else:
-            while self.set_point != float(set_point):
-                self.getTemperatures()
-        print(f"New set temperature at {set_point}°C")
+            while self.set_temperature != float(temperature):
+                self.getTemperature()
+        print(f"New set temperature at {self.set_temperature}°C")
         
         self._stabilize_time = None
         self.setFlag(temperature_reached=False, pause_feedback=False)
         if blocking:
-            print(f"Waiting for temperature to reach {self.set_point}°C")
-        while not self.isReady():
+            print(f"Waiting for temperature to reach {self.set_temperature}°C")
+        while not self.isAtTemperature():
             if not self.flags['get_feedback']:
-                self.getTemperatures()
+                self.getTemperature()
             time.sleep(0.1)
             if not blocking:
                 break
         return
     
     def shutdown(self):
         """Shutdown procedure for tool"""
@@ -267,25 +269,25 @@
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
             time.sleep(1)
-            print(self.getTemperatures())
+            print(self.getTemperature())
         self.device = device
         return
     
     def _loop_feedback(self):
         """Loop to constantly read from device"""
         print('Listening...')
         while self.flags['get_feedback']:
             if self.flags['pause_feedback']:
                 continue
-            self.getTemperatures()
+            self.getTemperature()
             time.sleep(0.1)
         print('Stop listening...')
         return
 
     def _read(self) -> str:
         """
         Read response from device
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Make/make_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Make/make_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     - `disconnect`: disconnect from device
     - `isBusy`: checks and returns whether the device is busy
     - `isConnected`: checks and returns whether the device is connected
     - `resetFlags`: reset all flags to class attribute `_default_flags`
     - `setFlag`: set flags by using keyword arguments
     """
     
-    _default_flags: dict[str, bool] = {}
+    _default_flags: dict[str, bool] = {'busy': False, 'connected': False}
     def __init__(self, verbose:bool = False, **kwargs):
         """
         Instantiate the class
 
         Args:
             verbose (bool, optional): verbosity of class. Defaults to False.
         """
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             return 0,0
         start = max(1, start)
         end = max(start, end)
         return start,end
     
     def getErrors(self) -> list[str]:
         """
-        Gget error messages from device
+        Get error messages from device
         
         Returns:
             list[str]: list of error messages from device
         """
         errors = []
         reply = ''
         while not reply.isnumeric():
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/__init__.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,30 +66,30 @@
         self._query("G90\n")
         self._query("G1 F10800\n")
         
         self.coordinates = self.home_coordinates
         print("Homed")
         return True
 
-    def setTemperature(self, set_point: float) -> bool:
+    def setTemperature(self, set_temperature: float) -> bool:
         """
         Set the temperature of the 3-D printer platform bed
 
         Args:
-            set_point (float): set point for platform temperature
+            set_temperature (float): set point for platform temperature
 
         Returns:
             bool: whether setting bed temperature was successful
         """
-        if set_point < self.temperature_range[0] or set_point > self.temperature_range[1]:
+        if set_temperature < self.temperature_range[0] or set_temperature > self.temperature_range[1]:
             print(f'Please select a temperature between {self.temperature_range[0]} and {self.temperature_range[1]}°C.')
             return False
-        set_point = round( min(max(set_point,0), 110) )
+        set_temperature = round( min(max(set_temperature,0), 110) )
         try:
-            print(f"New set temperature at {set_point}°C")
-            self.device.write(bytes(f'M140 S{set_point}\n', 'utf-8'))
+            print(f"New set temperature at {set_temperature}°C")
+            self.device.write(bytes(f'M140 S{set_temperature}\n', 'utf-8'))
         except Exception as e:
             print('Unable to heat stage!')
             if self.verbose:
                 print(e)
             return False
         return True
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Created on Wed Apr  6 12:51:41 2022
-
-@author: jjcheng3
+API from Dobot: [source](https://github.com/Dobot-Arm/TCP-IP-4Axis-Python)
 """
 
 import socket
 from threading import Timer
 import numpy as np
 
 # Port Feedback
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Move/move_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,46 +47,46 @@
     
     ### Attributes
     - `busy` (bool): whether the pump is busy
     - `capacity` (int): syringe capacity
     - `channel` (int): channel id
     - `command` (str): command string
     - `init_status` (bool): whether the pump has been initialised
+    - `limits` (int): maximum allowable position
     - `model` (str): TriContinent pump model name
     - `name` (str): name of the pump
     - `output_right` (bool): whether liquid is pumped out to the right
     - `position` (int): position of plunger
     - `reagent` (str): name of reagent in pump
     - `resolution` (float): volume resolution of pump (i.e. uL per step)
-    - `step_limit` (int): maximum allowable position
     
     ### Properties
     - `status` (str): pump device status
     - `volume` (float): volume of reagent in pump
     """
     
     channel: int
     model: str
     capacity: int
     output_right: bool
     name: str = ''
     reagent: str = ''
+    limits: int = field(init=False)
     resolution: float = field(init=False)
-    step_limit: int = field(init=False)
     
     busy: bool = field(default=False, init=False)
     init_status: bool = field(default=False, init=False)
     
     command: str = field(default='', init=False)
     position: int = field(default=0, init=False)
     _status_code: str = field(default='', init=False)
     
     def __post_init__(self):
-        self.step_limit = int(''.join(filter(str.isdigit, self.model)))
-        self.resolution = self.capacity / self.step_limit
+        self.limits = int(''.join(filter(str.isdigit, self.model)))
+        self.resolution = self.capacity / self.limits
         if len(self.name) == 0:
             self.name = f"Pump {self.channel}"
         return
     
     # Properties
     @property
     def status(self) -> str:
@@ -96,8 +96,8 @@
         if value not in ErrorCode._member_names_:
             raise ValueError("Please provide a valid error code.")
         self._status_code = value
         return
     
     @property
     def volume(self) -> float:
-        return self.position/self.step_limit * self.capacity
+        return self.position/self.limits * self.capacity
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         
     ### Attributes
     - `channels` (dict[int, TriContinentPump]): dictionary of {channel id, TriContinentPump object}
     - `current_channel` (TriContinentPump): currently active pump
     - `name` (str): name of current pump
     - `capacity` (int): syringe capacity of current pump
     - `resolution` (float): volume resolution of current pump (i.e. uL per step)
-    - `step_limit` (int): maximum allowable position of current pump
+    - `limits` (int): maximum allowable position of current pump
     - `position` (int): position of plunger for current pump
     
     ### Properties
     - `current_pump` (TriContinentPump): alias for `current_channel`
     - `pumps` (dict[int, TriContinentPump]): alias for `channels`
     - `status` (str): current status of active pump
     - `volume` (float): volume of current pump
@@ -113,15 +113,15 @@
         )
         self.current_channel = None
         
         self.channel = list(self.channels)[0]
         self.name = ''
         self.capacity = 0
         self.resolution = 1
-        self.step_limit = 1
+        self.limits = 1
         
         self.position = 0
         for channel in self.channels:
             self.setCurrentChannel(channel=channel)
             self.initialise()
         self.resetChannel()
         return
@@ -137,15 +137,15 @@
     
     @property
     def status(self) -> str:
         return self.getStatus()
     
     @property
     def volume(self) -> float:
-        return self.position/self.step_limit * self.capacity
+        return self.position/self.limits * self.capacity
     
     # Decorators
     def _single_action(func: Callable) -> Callable:
         """
         Turns a method into a single action that runs only if it is not contained in a compound action
 
         Args:
@@ -207,15 +207,15 @@
             start_speed (int, optional): starting speed of plunger. Defaults to 50.
             reagent (Optional[str], optional): name of reagent. Defaults to None.
             channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
 
         Returns:
             str: command string
         """
-        steps = min(int(volume/self.resolution), self.step_limit-self.position)
+        steps = min(int(volume/self.resolution), self.limits-self.position)
         volume = steps * self.resolution
         self.queue([
             self.setStartSpeed(start_speed),
             self.setTopSpeed(speed),
             self.setSpeedRamp(1),
             self.setValve('I'),
             self.moveBy(steps),
@@ -296,15 +296,15 @@
             pause (bool, optional): whether to pause for user intervention. Defaults to False.
             start_speed (int, optional): starting speed of plunger. Defaults to 50.
             channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
 
         Returns:
             str: command string
         """
-        steps = min(int(volume/self.resolution), self.step_limit)
+        steps = min(int(volume/self.resolution), self.limits)
         volume = steps * self.resolution
         self.queue([
             self.setStartSpeed(start_speed),
             self.setTopSpeed(speed),
             self.setSpeedRamp(1)
         ], channel=channel)
         if self.position <= steps:
@@ -345,17 +345,17 @@
 
         Args:
             channel (Optional[int], optional): channel id(s). Defaults to None.
 
         Returns:
             str: command string
         """
-        self.position = self.step_limit
+        self.position = self.limits
         self.current_pump.position = self.position
-        return f"IA{self.step_limit}"
+        return f"IA{self.limits}"
 
     def getPosition(self, channel:Optional[int] = None) -> int:
         """
         Get the position of the pump plunger from the device
 
         Args:
             channel (Optional[int], optional): channel id(s). Defaults to None.
@@ -384,14 +384,15 @@
             str: status message
         """
         self.setCurrentChannel(channel=channel)
         response = self._query('Q')
         _status_code = response[2] if len(response) else ''
         if self.device is not None:
             if _status_code not in StatusCode.Busy.value and _status_code not in StatusCode.Idle.value:
+                print(repr(_status_code))
                 raise RuntimeError(f"Unable to get status from Pump: {self.name}")
     
         if _status_code in StatusCode.Busy.value:
             self.setFlag(busy=True)
             self.current_pump.busy = True
         elif _status_code in StatusCode.Idle.value:
             self.setFlag(busy=False)
@@ -634,15 +635,15 @@
         self.current_channel = self.channels[channel]
         pump = self.current_pump
         
         self.channel = pump.channel
         self.name = pump.name
         self.capacity = pump.capacity
         self.resolution = pump.resolution
-        self.step_limit = pump.step_limit
+        self.limits = pump.limits
         self.position = pump.position
         return
  
     @_single_action
     def setSpeedRamp(self, ramp:int, channel:Optional[int] = None) -> str:
         """
         Set the acceleration from start speed to top speed
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,1372 +600,1376 @@
 00002570: 2020 2020 2070 7269 6e74 2873 7065 6564       print(speed
 00002580: 5f70 6172 616d 6574 6572 7329 0d0a 2020  _parameters)..  
 00002590: 2020 2020 2020 2020 2020 7072 6573 6574            preset
 000025a0: 203d 2073 7065 6564 5f70 6172 616d 6574   = speed_paramet
 000025b0: 6572 732e 7072 6573 6574 0d0a 2020 2020  ers.preset..    
 000025c0: 2020 2020 2020 2020 6966 2070 7265 7365          if prese
 000025d0: 7420 6973 204e 6f6e 653a 0d0a 2020 2020  t is None:..    
-000025e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000025f0: 6520 5275 6e74 696d 6545 7272 6f72 2827  e RuntimeError('
-00002600: 5461 7267 6574 2073 7065 6564 206e 6f74  Target speed not
-00002610: 2070 6f73 7369 626c 652e 2729 0d0a 2020   possible.')..  
-00002620: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00002630: 6574 5370 6565 6428 7370 6565 643d 7072  etSpeed(speed=pr
-00002640: 6573 6574 2c20 7570 3d54 7275 652c 2064  eset, up=True, d
-00002650: 6566 6175 6c74 3d46 616c 7365 290d 0a20  efault=False).. 
-00002660: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002670: 2020 2020 2020 2020 2073 7465 7073 5f6c           steps_l
-00002680: 6566 7420 3d20 7374 6570 730d 0a20 2020  eft = steps..   
-00002690: 2020 2020 2020 2020 2064 656c 6179 203d           delay =
-000026a0: 2073 7065 6564 5f70 6172 616d 6574 6572   speed_parameter
-000026b0: 732e 6465 6c61 790d 0a20 2020 2020 2020  s.delay..       
-000026c0: 2020 2020 2073 7465 705f 7369 7a65 203d       step_size =
-000026d0: 2073 7065 6564 5f70 6172 616d 6574 6572   speed_parameter
-000026e0: 732e 7374 6570 5f73 697a 650d 0a20 2020  s.step_size..   
-000026f0: 2020 2020 2020 2020 2069 6e74 6572 7661           interva
-00002700: 6c73 203d 2073 7065 6564 5f70 6172 616d  ls = speed_param
-00002710: 6574 6572 732e 696e 7465 7276 616c 730d  eters.intervals.
-00002720: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-00002730: 7274 5f61 7370 6972 6174 6520 3d20 7469  rt_aspirate = ti
-00002740: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
-00002750: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00002760: 6f72 2069 2069 6e20 7261 6e67 6528 696e  or i in range(in
-00002770: 7465 7276 616c 7329 3a0d 0a20 2020 2020  tervals):..     
-00002780: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00002790: 5f74 696d 6520 3d20 7469 6d65 2e70 6572  _time = time.per
-000027a0: 665f 636f 756e 7465 7228 290d 0a20 2020  f_counter()..   
-000027b0: 2020 2020 2020 2020 2020 2020 2073 7465               ste
-000027c0: 7020 3d20 7374 6570 5f73 697a 6520 6966  p = step_size if
-000027d0: 2028 692b 3120 213d 2069 6e74 6572 7661   (i+1 != interva
-000027e0: 6c73 2920 656c 7365 2073 7465 7073 5f6c  ls) else steps_l
-000027f0: 6566 740d 0a20 2020 2020 2020 2020 2020  eft..           
-00002800: 2020 2020 206d 6f76 655f 7469 6d65 203d       move_time =
-00002810: 2073 7465 702a 7365 6c66 2e72 6573 6f6c   step*self.resol
-00002820: 7574 696f 6e20 2f20 7072 6573 6574 0d0a  ution / preset..
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00002850: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
-00002860: 7d27 2c20 7265 7375 6d65 5f66 6565 6462  }', resume_feedb
-00002870: 6163 6b3d 4661 6c73 652c 2067 6574 5f70  ack=False, get_p
-00002880: 6f73 6974 696f 6e3d 4661 6c73 6529 0d0a  osition=False)..
-00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028a0: 2320 6966 2072 6573 706f 6e73 6520 213d  # if response !=
-000028b0: 2027 6f6b 273a 0d0a 2020 2020 2020 2020   'ok':..        
-000028c0: 2020 2020 2020 2020 2320 2020 2020 7072          #     pr
-000028d0: 696e 7428 2241 7370 6972 6174 696f 6e20  int("Aspiration 
-000028e0: 6661 696c 6564 2229 0d0a 2020 2020 2020  failed")..      
-000028f0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00002900: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
-00002910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002920: 2073 7465 7073 5f6c 6566 7420 2d3d 2073   steps_left -= s
-00002930: 7465 700d 0a20 2020 2020 2020 2020 2020  tep..           
-00002940: 2020 2020 2064 7572 6174 696f 6e20 3d20       duration = 
-00002950: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
-00002960: 7228 2920 2d20 7374 6172 745f 7469 6d65  r() - start_time
-00002970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002980: 2020 6966 2064 7572 6174 696f 6e20 3c20    if duration < 
-00002990: 2864 656c 6179 2b6d 6f76 655f 7469 6d65  (delay+move_time
-000029a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000029b0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-000029c0: 6570 2864 656c 6179 2b6d 6f76 655f 7469  ep(delay+move_ti
-000029d0: 6d65 2d64 7572 6174 696f 6e29 0d0a 2020  me-duration)..  
-000029e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000029f0: 2320 5570 6461 7465 2076 616c 7565 730d  # Update values.
-00002a00: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00002a10: 2741 7370 6972 6174 696f 6e20 7469 6d65  'Aspiration time
-00002a20: 3a20 7b74 696d 652e 7065 7266 5f63 6f75  : {time.perf_cou
-00002a30: 6e74 6572 2829 2d73 7461 7274 5f61 7370  nter()-start_asp
-00002a40: 6972 6174 657d 7327 290d 0a20 2020 2020  irate}s')..     
-00002a50: 2020 2074 696d 652e 736c 6565 7028 7761     time.sleep(wa
-00002a60: 6974 290d 0a20 2020 2020 2020 2073 656c  it)..        sel
-00002a70: 662e 7365 7446 6c61 6728 6f63 6375 7069  f.setFlag(occupi
-00002a80: 6564 3d46 616c 7365 2c20 7061 7573 655f  ed=False, pause_
-00002a90: 6665 6564 6261 636b 3d46 616c 7365 290d  feedback=False).
-00002aa0: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
-00002ab0: 7450 6f73 6974 696f 6e28 290d 0a20 2020  tPosition()..   
-00002ac0: 2020 2020 2073 656c 662e 766f 6c75 6d65       self.volume
-00002ad0: 202b 3d20 766f 6c75 6d65 0d0a 2020 2020   += volume..    
-00002ae0: 2020 2020 7365 6c66 2e70 6f73 6974 696f      self.positio
-00002af0: 6e20 2b3d 2073 7465 7073 0d0a 2020 2020  n += steps..    
-00002b00: 2020 2020 6966 2072 6561 6765 6e74 2069      if reagent i
-00002b10: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00002b20: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00002b30: 6167 656e 7420 3d20 7265 6167 656e 740d  agent = reagent.
-00002b40: 0a20 2020 2020 2020 2069 6620 7061 7573  .        if paus
-00002b50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002b60: 696e 7075 7428 2250 7265 7373 2027 456e  input("Press 'En
-00002b70: 7465 7227 2074 6f20 7072 6f63 6565 642e  ter' to proceed.
-00002b80: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00002b90: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-00002ba0: 200d 0a20 2020 2064 6566 2062 6c6f 776f   ..    def blowo
-00002bb0: 7574 2873 656c 662c 2068 6f6d 653a 626f  ut(self, home:bo
-00002bc0: 6f6c 203d 2054 7275 652c 202a 2a6b 7761  ol = True, **kwa
-00002bd0: 7267 7329 202d 3e20 7374 723a 0d0a 2020  rgs) -> str:..  
-00002be0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00002bf0: 2020 2042 6c6f 776f 7574 206c 6971 7569     Blowout liqui
-00002c00: 6420 6672 6f6d 2074 6970 0d0a 0d0a 2020  d from tip....  
-00002c10: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00002c20: 2020 2020 2020 2020 2068 6f6d 6520 2862           home (b
-00002c30: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-00002c40: 7768 6574 6865 7220 746f 2072 6574 7572  whether to retur
-00002c50: 6e20 706c 756e 6765 7220 746f 2068 6f6d  n plunger to hom
-00002c60: 6520 706f 7369 7469 6f6e 2e20 4465 6661  e position. Defa
-00002c70: 756c 7473 2074 6f20 5472 7565 2e0d 0a0d  ults to True....
-00002c80: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00002c90: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00002ca0: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
-00002cb0: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
-00002cc0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-00002cd0: 6420 3d20 6627 5242 7b73 656c 662e 686f  d = f'RB{self.ho
-00002ce0: 6d65 5f70 6f73 6974 696f 6e7d 2720 6966  me_position}' if
-00002cf0: 2068 6f6d 6520 656c 7365 2027 5242 270d   home else 'RB'.
-00002d00: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00002d10: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
-00002d20: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
-00002d30: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00002d40: 3d20 7365 6c66 2e68 6f6d 655f 706f 7369  = self.home_posi
-00002d50: 7469 6f6e 0d0a 2020 2020 2020 2020 7469  tion..        ti
-00002d60: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
-00002d70: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00002d80: 6f6e 7365 0d0a 2020 2020 0d0a 2020 2020  onse..    ..    
-00002d90: 6465 6620 6469 7370 656e 7365 2873 656c  def dispense(sel
-00002da0: 662c 200d 0a20 2020 2020 2020 2076 6f6c  f, ..        vol
-00002db0: 756d 653a 2066 6c6f 6174 2c20 0d0a 2020  ume: float, ..  
-00002dc0: 2020 2020 2020 7370 6565 643a 204f 7074        speed: Opt
-00002dd0: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
-00002de0: 6f6e 652c 200d 0a20 2020 2020 2020 2077  one, ..        w
-00002df0: 6169 743a 2069 6e74 203d 2030 2c20 0d0a  ait: int = 0, ..
-00002e00: 2020 2020 2020 2020 7061 7573 653a 2062          pause: b
-00002e10: 6f6f 6c20 3d20 4661 6c73 652c 200d 0a20  ool = False, .. 
-00002e20: 2020 2020 2020 2062 6c6f 776f 7574 3a20         blowout: 
-00002e30: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
-00002e40: 2020 2020 2020 2062 6c6f 776f 7574 5f68         blowout_h
-00002e50: 6f6d 653a 2062 6f6f 6c20 3d20 5472 7565  ome: bool = True
-00002e60: 2c0d 0a20 2020 2020 2020 2066 6f72 6365  ,..        force
-00002e70: 5f64 6973 7065 6e73 653a 2062 6f6f 6c20  _dispense: bool 
-00002e80: 3d20 4661 6c73 652c 200d 0a20 2020 2020  = False, ..     
-00002e90: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
-00002ea0: 2029 202d 3e20 7374 723a 0d0a 2020 2020   ) -> str:..    
-00002eb0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00002ec0: 2044 6973 7065 6e73 6520 6465 7369 7265   Dispense desire
-00002ed0: 6420 766f 6c75 6d65 206f 6620 7265 6167  d volume of reag
-00002ee0: 656e 740d 0a0d 0a20 2020 2020 2020 2041  ent....        A
-00002ef0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00002f00: 2020 766f 6c75 6d65 2028 666c 6f61 7429    volume (float)
-00002f10: 3a20 7461 7267 6574 2076 6f6c 756d 650d  : target volume.
-00002f20: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00002f30: 6564 2028 4f70 7469 6f6e 616c 5b66 6c6f  ed (Optional[flo
-00002f40: 6174 5d2c 206f 7074 696f 6e61 6c29 3a20  at], optional): 
-00002f50: 7370 6565 6420 746f 2064 6973 7065 6e73  speed to dispens
-00002f60: 6520 6174 2e20 4465 6661 756c 7473 2074  e at. Defaults t
-00002f70: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
-00002f80: 2020 2020 2077 6169 7420 2869 6e74 2c20       wait (int, 
-00002f90: 6f70 7469 6f6e 616c 293a 2074 696d 6520  optional): time 
-00002fa0: 6465 6c61 7920 6166 7465 7220 6469 7370  delay after disp
-00002fb0: 656e 7365 2e20 4465 6661 756c 7473 2074  ense. Defaults t
-00002fc0: 6f20 302e 0d0a 2020 2020 2020 2020 2020  o 0...          
-00002fd0: 2020 7061 7573 6520 2862 6f6f 6c2c 206f    pause (bool, o
-00002fe0: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
-00002ff0: 7220 746f 2070 6175 7365 2066 6f72 2075  r to pause for u
-00003000: 7365 7220 696e 7465 7276 656e 7469 6f6e  ser intervention
-00003010: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-00003020: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-00003030: 2020 626c 6f77 6f75 7420 2862 6f6f 6c2c    blowout (bool,
-00003040: 206f 7074 696f 6e61 6c29 3a20 7768 6574   optional): whet
-00003050: 6865 7220 7065 7266 6f72 6d20 626c 6f77  her perform blow
-00003060: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
-00003070: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
-00003080: 2020 2020 2062 6c6f 776f 7574 5f68 6f6d       blowout_hom
-00003090: 6520 2862 6f6f 6c2c 206f 7074 696f 6e61  e (bool, optiona
-000030a0: 6c29 3a20 7768 6574 6865 7220 746f 2072  l): whether to r
-000030b0: 6574 7572 6e20 7468 6520 706c 756e 6765  eturn the plunge
-000030c0: 7220 686f 6d65 2061 6674 6572 2062 6c6f  r home after blo
-000030d0: 776f 7574 2e20 4465 6661 756c 7473 2074  wout. Defaults t
-000030e0: 6f20 5472 7565 2e0d 0a20 2020 2020 2020  o True...       
-000030f0: 2020 2020 2066 6f72 6365 5f64 6973 7065       force_dispe
-00003100: 6e73 6520 2862 6f6f 6c2c 206f 7074 696f  nse (bool, optio
-00003110: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
-00003120: 2064 6973 7065 6e73 6520 7265 6167 656e   dispense reagen
-00003130: 7420 7265 6761 7264 6c65 7373 2e20 4465  t regardless. De
-00003140: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
-00003150: 0d0a 0d0a 2020 2020 2020 2020 5261 6973  ....        Rais
-00003160: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00003170: 2056 616c 7565 4572 726f 723a 2052 6571   ValueError: Req
-00003180: 7569 7265 6420 6469 7370 656e 7365 2076  uired dispense v
-00003190: 6f6c 756d 6520 6973 2067 7265 6174 6572  olume is greater
-000031a0: 2074 6861 6e20 766f 6c75 6d65 2069 6e20   than volume in 
-000031b0: 7469 700d 0a0d 0a20 2020 2020 2020 2052  tip....        R
-000031c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000031d0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-000031e0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000031f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00003200: 7365 6c66 2e73 6574 466c 6167 2870 6175  self.setFlag(pau
-00003210: 7365 5f66 6565 6462 6163 6b3d 5472 7565  se_feedback=True
-00003220: 2c20 6f63 6375 7069 6564 3d54 7275 6529  , occupied=True)
-00003230: 0d0a 2020 2020 2020 2020 6966 2066 6f72  ..        if for
-00003240: 6365 5f64 6973 7065 6e73 653a 0d0a 2020  ce_dispense:..  
-00003250: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
-00003260: 203d 206d 696e 2876 6f6c 756d 652c 2073   = min(volume, s
-00003270: 656c 662e 766f 6c75 6d65 290d 0a20 2020  elf.volume)..   
-00003280: 2020 2020 2065 6c69 6620 766f 6c75 6d65       elif volume
-00003290: 203e 2073 656c 662e 766f 6c75 6d65 3a0d   > self.volume:.
-000032a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000032b0: 7365 2056 616c 7565 4572 726f 7228 2752  se ValueError('R
-000032c0: 6571 7569 7265 6420 6469 7370 656e 7365  equired dispense
-000032d0: 2076 6f6c 756d 6520 6973 2067 7265 6174   volume is great
-000032e0: 6572 2074 6861 6e20 766f 6c75 6d65 2069  er than volume i
-000032f0: 6e20 7469 702e 2729 0d0a 2020 2020 2020  n tip.')..      
-00003300: 2020 7374 6570 7320 3d20 696e 7428 766f    steps = int(vo
-00003310: 6c75 6d65 202f 2073 656c 662e 7265 736f  lume / self.reso
-00003320: 6c75 7469 6f6e 290d 0a20 2020 2020 2020  lution)..       
-00003330: 2076 6f6c 756d 6520 3d20 7374 6570 7320   volume = steps 
-00003340: 2a20 7365 6c66 2e72 6573 6f6c 7574 696f  * self.resolutio
-00003350: 6e0d 0a20 2020 2020 2020 2069 6620 766f  n..        if vo
-00003360: 6c75 6d65 203d 3d20 303a 0d0a 2020 2020  lume == 0:..    
-00003370: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-00003380: 270d 0a20 2020 2020 2020 2070 7269 6e74  '..        print
-00003390: 2866 2744 6973 7065 6e73 696e 6720 7b76  (f'Dispensing {v
-000033a0: 6f6c 756d 657d 2075 4c2e 2e2e 2729 0d0a  olume} uL...')..
-000033b0: 2020 2020 2020 2020 7374 6172 745f 6469          start_di
-000033c0: 7370 656e 7365 203d 2074 696d 652e 7065  spense = time.pe
-000033d0: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
-000033e0: 2020 2020 2020 7370 6565 6420 3d20 7365        speed = se
-000033f0: 6c66 2e73 7065 6564 2e64 6f77 6e20 6966  lf.speed.down if
-00003400: 2073 7065 6564 2069 7320 4e6f 6e65 2065   speed is None e
-00003410: 6c73 6520 7370 6565 640d 0a0d 0a20 2020  lse speed....   
-00003420: 2020 2020 2069 6620 7370 6565 6420 696e       if speed in
-00003430: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
-00003440: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
-00003450: 2020 6966 2073 7065 6564 2021 3d20 7365    if speed != se
-00003460: 6c66 2e73 7065 6564 2e64 6f77 6e3a 0d0a  lf.speed.down:..
-00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 7365 6c66 2e73 6574 5370 6565 6428 7370  self.setSpeed(sp
-00003490: 6565 643d 7370 6565 642c 2075 703d 4661  eed=speed, up=Fa
-000034a0: 6c73 652c 2064 6566 6175 6c74 3d46 616c  lse, default=Fal
-000034b0: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
-000034c0: 2073 7461 7274 5f64 6973 7065 6e73 6520   start_dispense 
-000034d0: 3d20 7469 6d65 2e70 6572 665f 636f 756e  = time.perf_coun
-000034e0: 7465 7228 290d 0a20 2020 2020 2020 2020  ter()..         
-000034f0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00003500: 6c66 2e5f 7175 6572 7928 6627 524f 7b73  lf._query(f'RO{s
-00003510: 7465 7073 7d27 290d 0a20 2020 2020 2020  teps}')..       
-00003520: 2020 2020 206d 6f76 655f 7469 6d65 203d       move_time =
-00003530: 2073 7465 7073 2a73 656c 662e 7265 736f   steps*self.reso
-00003540: 6c75 7469 6f6e 202f 2073 7065 6564 0d0a  lution / speed..
-00003550: 2020 2020 2020 2020 2020 2020 6475 7261              dura
-00003560: 7469 6f6e 203d 2074 696d 652e 7065 7266  tion = time.perf
-00003570: 5f63 6f75 6e74 6572 2829 202d 2073 7461  _counter() - sta
-00003580: 7274 5f64 6973 7065 6e73 650d 0a20 2020  rt_dispense..   
-00003590: 2020 2020 2020 2020 2069 6620 6475 7261           if dura
-000035a0: 7469 6f6e 203c 2028 6d6f 7665 5f74 696d  tion < (move_tim
-000035b0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-000035c0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-000035d0: 6d6f 7665 5f74 696d 652d 6475 7261 7469  move_time-durati
-000035e0: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
-000035f0: 2023 2069 6620 7265 7370 6f6e 7365 2021   # if response !
-00003600: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
-00003610: 2020 2020 2023 2020 2020 2072 6574 7572       #     retur
-00003620: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
-00003630: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00003640: 2020 656c 6966 2073 7065 6564 206e 6f74    elif speed not
-00003650: 2069 6e20 7365 6c66 2e73 7065 6564 5f70   in self.speed_p
-00003660: 7265 7365 7473 3a0d 0a20 2020 2020 2020  resets:..       
-00003670: 2020 2020 2070 7269 6e74 2866 2254 6172       print(f"Tar
-00003680: 6765 743a 207b 766f 6c75 6d65 7d20 754c  get: {volume} uL
-00003690: 2061 7420 7b73 7065 6564 7d20 754c 2f73   at {speed} uL/s
-000036a0: 2e2e 2e22 290d 0a20 2020 2020 2020 2020  ...")..         
-000036b0: 2020 2073 7065 6564 5f70 6172 616d 6574     speed_paramet
-000036c0: 6572 7320 3d20 7365 6c66 2e5f 6361 6c63  ers = self._calc
-000036d0: 756c 6174 655f 7370 6565 645f 7061 7261  ulate_speed_para
-000036e0: 6d65 7465 7273 2876 6f6c 756d 653d 766f  meters(volume=vo
-000036f0: 6c75 6d65 2c20 7370 6565 643d 7370 6565  lume, speed=spee
-00003700: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00003710: 7072 696e 7428 7370 6565 645f 7061 7261  print(speed_para
-00003720: 6d65 7465 7273 290d 0a20 2020 2020 2020  meters)..       
-00003730: 2020 2020 2070 7265 7365 7420 3d20 7370       preset = sp
-00003740: 6565 645f 7061 7261 6d65 7465 7273 2e70  eed_parameters.p
-00003750: 7265 7365 740d 0a20 2020 2020 2020 2020  reset..         
-00003760: 2020 2069 6620 7072 6573 6574 2069 7320     if preset is 
-00003770: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00003780: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00003790: 7469 6d65 4572 726f 7228 2754 6172 6765  timeError('Targe
-000037a0: 7420 7370 6565 6420 6e6f 7420 706f 7373  t speed not poss
-000037b0: 6962 6c65 2e27 290d 0a20 2020 2020 2020  ible.')..       
-000037c0: 2020 2020 2073 656c 662e 7365 7453 7065       self.setSpe
-000037d0: 6564 2873 7065 6564 3d70 7265 7365 742c  ed(speed=preset,
-000037e0: 2075 703d 4661 6c73 652c 2064 6566 6175   up=False, defau
-000037f0: 6c74 3d46 616c 7365 290d 0a20 2020 2020  lt=False)..     
-00003800: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00003810: 2073 7465 7073 5f6c 6566 7420 3d20 7374   steps_left = st
-00003820: 6570 730d 0a20 2020 2020 2020 2020 2020  eps..           
-00003830: 2064 656c 6179 203d 2073 7065 6564 5f70   delay = speed_p
-00003840: 6172 616d 6574 6572 732e 6465 6c61 790d  arameters.delay.
-00003850: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
-00003860: 705f 7369 7a65 203d 2073 7065 6564 5f70  p_size = speed_p
-00003870: 6172 616d 6574 6572 732e 7374 6570 5f73  arameters.step_s
-00003880: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
-00003890: 2069 6e74 6572 7661 6c73 203d 2073 7065   intervals = spe
-000038a0: 6564 5f70 6172 616d 6574 6572 732e 696e  ed_parameters.in
-000038b0: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
-000038c0: 2020 2020 2073 7461 7274 5f64 6973 7065       start_dispe
-000038d0: 6e73 6520 3d20 7469 6d65 2e70 6572 665f  nse = time.perf_
-000038e0: 636f 756e 7465 7228 290d 0a20 2020 2020  counter()..     
-000038f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00003900: 7261 6e67 6528 696e 7465 7276 616c 7329  range(intervals)
-00003910: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003920: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
-00003930: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
-00003940: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
-00003950: 2020 2020 2073 7465 7020 3d20 7374 6570       step = step
-00003960: 5f73 697a 6520 6966 2028 692b 3120 213d  _size if (i+1 !=
-00003970: 2069 6e74 6572 7661 6c73 2920 656c 7365   intervals) else
-00003980: 2073 7465 7073 5f6c 6566 740d 0a20 2020   steps_left..   
-00003990: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
-000039a0: 655f 7469 6d65 203d 2073 7465 702a 7365  e_time = step*se
-000039b0: 6c66 2e72 6573 6f6c 7574 696f 6e20 2f20  lf.resolution / 
-000039c0: 7072 6573 6574 0d0a 2020 2020 2020 2020  preset..        
-000039d0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000039e0: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
-000039f0: 2752 4f7b 7374 6570 7d27 2c20 7265 7375  'RO{step}', resu
-00003a00: 6d65 5f66 6565 6462 6163 6b3d 4661 6c73  me_feedback=Fals
-00003a10: 652c 2067 6574 5f70 6f73 6974 696f 6e3d  e, get_position=
-00003a20: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-00003a30: 2020 2020 2020 2020 2320 6966 2072 6573          # if res
-00003a40: 706f 6e73 6520 213d 2027 6f6b 273a 0d0a  ponse != 'ok':..
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2320 2020 2020 7072 696e 7428 2244 6973  #     print("Dis
-00003a70: 7065 6e73 6520 6661 696c 6564 2229 0d0a  pense failed")..
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
-00003aa0: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
-00003ab0: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
-00003ac0: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
-00003ad0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-00003ae0: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
-00003af0: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
-00003b00: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
-00003b10: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
-00003b20: 696f 6e20 3c20 2864 656c 6179 2b6d 6f76  ion < (delay+mov
-00003b30: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
-00003b40: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00003b50: 6d65 2e73 6c65 6570 2864 656c 6179 2b6d  me.sleep(delay+m
-00003b60: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
-00003b70: 6e29 0d0a 0d0a 2020 2020 2020 2020 2320  n)....        # 
-00003b80: 5570 6461 7465 2076 616c 7565 730d 0a20  Update values.. 
-00003b90: 2020 2020 2020 2070 7269 6e74 2866 2744         print(f'D
-00003ba0: 6973 7065 6e73 6520 7469 6d65 3a20 7b74  ispense time: {t
-00003bb0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
-00003bc0: 2829 2d73 7461 7274 5f64 6973 7065 6e73  ()-start_dispens
-00003bd0: 657d 7327 290d 0a20 2020 2020 2020 2074  e}s')..        t
-00003be0: 696d 652e 736c 6565 7028 7761 6974 290d  ime.sleep(wait).
-00003bf0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00003c00: 7446 6c61 6728 6f63 6375 7069 6564 3d46  tFlag(occupied=F
-00003c10: 616c 7365 2c20 7061 7573 655f 6665 6564  alse, pause_feed
-00003c20: 6261 636b 3d46 616c 7365 290d 0a20 2020  back=False)..   
-00003c30: 2020 2020 2073 656c 662e 6765 7450 6f73       self.getPos
-00003c40: 6974 696f 6e28 290d 0a20 2020 2020 2020  ition()..       
-00003c50: 2073 656c 662e 766f 6c75 6d65 203d 206d   self.volume = m
-00003c60: 6178 2873 656c 662e 766f 6c75 6d65 202d  ax(self.volume -
-00003c70: 2076 6f6c 756d 652c 2030 290d 0a20 2020   volume, 0)..   
-00003c80: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-00003c90: 6f6e 202d 3d20 7374 6570 730d 0a20 2020  on -= steps..   
-00003ca0: 2020 2020 2069 6620 7365 6c66 2e76 6f6c       if self.vol
-00003cb0: 756d 6520 3d3d 2030 2061 6e64 2062 6c6f  ume == 0 and blo
-00003cc0: 776f 7574 3a0d 0a20 2020 2020 2020 2020  wout:..         
-00003cd0: 2020 2073 656c 662e 626c 6f77 6f75 7428     self.blowout(
-00003ce0: 686f 6d65 3d62 6c6f 776f 7574 5f68 6f6d  home=blowout_hom
-00003cf0: 6529 0d0a 2020 2020 2020 2020 6966 2070  e)..        if p
-00003d00: 6175 7365 3a0d 0a20 2020 2020 2020 2020  ause:..         
-00003d10: 2020 2069 6e70 7574 2822 5072 6573 7320     input("Press 
-00003d20: 2745 6e74 6572 2720 746f 2070 726f 6365  'Enter' to proce
-00003d30: 6564 2e22 290d 0a20 2020 2020 2020 2072  ed.")..        r
-00003d40: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00003d50: 2020 2020 0d0a 2020 2020 6465 6620 656a      ..    def ej
-00003d60: 6563 7428 7365 6c66 2c20 686f 6d65 3a62  ect(self, home:b
-00003d70: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2073  ool = True) -> s
-00003d80: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-00003d90: 0d0a 2020 2020 2020 2020 456a 6563 7420  ..        Eject 
-00003da0: 7468 6520 7069 7065 7474 6520 7469 700d  the pipette tip.
-00003db0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00003dc0: 0d0a 2020 2020 2020 2020 2020 2020 686f  ..            ho
-00003dd0: 6d65 2028 626f 6f6c 2c20 6f70 7469 6f6e  me (bool, option
-00003de0: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
-00003df0: 7265 7475 726e 2070 6c75 6e67 6572 2074  return plunger t
-00003e00: 6f20 686f 6d65 2070 6f73 6974 696f 6e2e  o home position.
-00003e10: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-00003e20: 652e 0d0a 0d0a 2020 2020 2020 2020 5265  e.....        Re
-00003e30: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00003e40: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
-00003e50: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00003e60: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-00003e70: 656c 662e 7265 6167 656e 7420 3d20 2727  elf.reagent = ''
-00003e80: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-00003e90: 6420 3d20 6627 5245 7b73 656c 662e 686f  d = f'RE{self.ho
-00003ea0: 6d65 5f70 6f73 6974 696f 6e7d 2720 6966  me_position}' if
-00003eb0: 2068 6f6d 6520 656c 7365 2027 5245 270d   home else 'RE'.
-00003ec0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00003ed0: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
-00003ee0: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
-00003ef0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00003f00: 3d20 7365 6c66 2e68 6f6d 655f 706f 7369  = self.home_posi
-00003f10: 7469 6f6e 2069 6620 686f 6d65 2065 6c73  tion if home els
-00003f20: 6520 300d 0a20 2020 2020 2020 2074 696d  e 0..        tim
-00003f30: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
-00003f40: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00003f50: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
-00003f60: 6566 2065 6d70 7479 2873 656c 662c 202a  ef empty(self, *
-00003f70: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-00003f80: 2020 2022 2222 456d 7074 7920 7468 6520     """Empty the 
-00003f90: 7069 7065 7474 6522 2222 0d0a 2020 2020  pipette"""..    
-00003fa0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00003fb0: 686f 6d65 2829 0d0a 2020 2020 0d0a 2020  home()..    ..  
-00003fc0: 2020 6465 6620 6765 7443 6170 6163 6974    def getCapacit
-00003fd0: 616e 6365 2873 656c 6629 202d 3e20 556e  ance(self) -> Un
-00003fe0: 696f 6e5b 696e 742c 2073 7472 5d3a 0d0a  ion[int, str]:..
-00003ff0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004000: 2020 2020 2047 6574 2074 6865 2063 6170       Get the cap
-00004010: 6163 6974 616e 6365 2061 7320 6d65 6173  acitance as meas
-00004020: 7572 6564 2061 7420 7468 6520 656e 6420  ured at the end 
-00004030: 6f66 2074 6865 2070 6970 6574 7465 0d0a  of the pipette..
-00004040: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004050: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00004060: 2020 2020 2020 2020 556e 696f 6e5b 696e          Union[in
-00004070: 742c 2073 7472 5d3a 2063 6170 6163 6974  t, str]: capacit
-00004080: 616e 6365 2076 616c 7565 2c20 6f72 2064  ance value, or d
-00004090: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
-000040a0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000040b0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-000040c0: 7365 6c66 2e5f 7175 6572 7928 2744 4e27  self._query('DN'
-000040d0: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
-000040e0: 0a20 2020 2020 2020 2020 2020 2063 6170  .            cap
-000040f0: 6163 6974 616e 6365 203d 2069 6e74 2872  acitance = int(r
-00004100: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
-00004110: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-00004120: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-00004130: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00004140: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00004150: 5f63 6170 6163 6974 616e 6365 203d 2063  _capacitance = c
-00004160: 6170 6163 6974 616e 6365 0d0a 2020 2020  apacitance..    
-00004170: 2020 2020 7265 7475 726e 2063 6170 6163      return capac
-00004180: 6974 616e 6365 0d0a 200d 0a20 2020 2064  itance.. ..    d
-00004190: 6566 2067 6574 4572 726f 7273 2873 656c  ef getErrors(sel
-000041a0: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
-000041b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000041c0: 2047 6574 2065 7272 6f72 7320 6672 6f6d   Get errors from
-000041d0: 2074 6865 2064 6576 6963 650d 0a0d 0a20   the device.... 
-000041e0: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-000041f0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00004200: 3a20 6465 7669 6365 2072 6573 706f 6e73  : device respons
-00004210: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
-00004220: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00004230: 656c 662e 5f71 7565 7279 2827 4445 2729  elf._query('DE')
-00004240: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00004250: 6765 7449 6e66 6f28 7365 6c66 2c20 6d6f  getInfo(self, mo
-00004260: 6465 6c3a 204f 7074 696f 6e61 6c5b 7374  del: Optional[st
-00004270: 725d 203d 204e 6f6e 6529 3a0d 0a20 2020  r] = None):..   
-00004280: 2020 2020 2022 2222 4765 7420 6465 7461       """Get deta
-00004290: 696c 7320 6f66 2074 6865 2053 6172 746f  ils of the Sarto
-000042a0: 7269 7573 2070 6970 6574 7465 206d 6f64  rius pipette mod
-000042b0: 656c 2222 220d 0a20 2020 2020 2020 206d  el"""..        m
-000042c0: 6f64 656c 203d 2073 656c 662e 5f5f 6d6f  odel = self.__mo
-000042d0: 6465 6c5f 5f28 292e 7370 6c69 7428 272d  del__().split('-
-000042e0: 2729 5b30 5d20 6966 206d 6f64 656c 2069  ')[0] if model i
-000042f0: 7320 4e6f 6e65 2065 6c73 6520 6d6f 6465  s None else mode
-00004300: 6c0d 0a20 2020 2020 2020 2069 6620 6d6f  l..        if mo
-00004310: 6465 6c20 6e6f 7420 696e 204d 6f64 656c  del not in Model
-00004320: 496e 666f 2e5f 6d65 6d62 6572 5f6e 616d  Info._member_nam
-00004330: 6573 5f3a 0d0a 2020 2020 2020 2020 2020  es_:..          
-00004340: 2020 7072 696e 7428 6627 5265 6365 6976    print(f'Receiv
-00004350: 6564 3a20 7b6d 6f64 656c 7d27 290d 0a20  ed: {model}').. 
-00004360: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00004370: 203d 2027 4252 4c30 270d 0a20 2020 2020   = 'BRL0'..     
-00004380: 2020 2020 2020 2070 7269 6e74 2866 2244         print(f"D
-00004390: 6566 6175 6c74 696e 6720 746f 3a20 7b27  efaulting to: {'
-000043a0: 4252 4c30 277d 2229 0d0a 2020 2020 2020  BRL0'}")..      
-000043b0: 2020 2020 2020 7072 696e 7428 6622 5661        print(f"Va
-000043c0: 6c69 6420 6d6f 6465 6c73 2061 7265 3a20  lid models are: 
-000043d0: 7b27 2c20 272e 6a6f 696e 284d 6f64 656c  {', '.join(Model
-000043e0: 496e 666f 2e5f 6d65 6d62 6572 5f6e 616d  Info._member_nam
-000043f0: 6573 5f29 7d22 290d 0a20 2020 2020 2020  es_)}")..       
-00004400: 2069 6e66 6f3a 204d 6f64 656c 203d 204d   info: Model = M
-00004410: 6f64 656c 496e 666f 5b6d 6f64 656c 5d2e  odelInfo[model].
-00004420: 7661 6c75 650d 0a20 2020 2020 2020 2070  value..        p
-00004430: 7269 6e74 2869 6e66 6f29 0d0a 2020 2020  rint(info)..    
-00004440: 2020 2020 7365 6c66 2e6d 6f64 656c 5f69      self.model_i
-00004450: 6e66 6f20 3d20 696e 666f 0d0a 2020 2020  nfo = info..    
-00004460: 2020 2020 7365 6c66 2e63 6170 6163 6974      self.capacit
-00004470: 7920 3d20 696e 666f 2e63 6170 6163 6974  y = info.capacit
-00004480: 790d 0a20 2020 2020 2020 2073 656c 662e  y..        self.
-00004490: 6c69 6d69 7473 203d 2028 696e 666f 2e74  limits = (info.t
-000044a0: 6970 5f65 6a65 6374 5f70 6f73 6974 696f  ip_eject_positio
-000044b0: 6e2c 2069 6e66 6f2e 6d61 785f 706f 7369  n, info.max_posi
-000044c0: 7469 6f6e 290d 0a20 2020 2020 2020 2073  tion)..        s
-000044d0: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
-000044e0: 7320 3d20 696e 666f 2e70 7265 7365 745f  s = info.preset_
-000044f0: 7370 6565 6473 0d0a 2020 2020 2020 2020  speeds..        
-00004500: 7365 6c66 2e73 7065 6564 2e75 7020 3d20  self.speed.up = 
-00004510: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
-00004520: 7473 5b73 656c 662e 7370 6565 645f 636f  ts[self.speed_co
-00004530: 6465 2e75 702d 315d 0d0a 2020 2020 2020  de.up-1]..      
-00004540: 2020 7365 6c66 2e73 7065 6564 2e64 6f77    self.speed.dow
-00004550: 6e20 3d20 7365 6c66 2e73 7065 6564 5f70  n = self.speed_p
-00004560: 7265 7365 7473 5b73 656c 662e 7370 6565  resets[self.spee
-00004570: 645f 636f 6465 2e64 6f77 6e2d 315d 0d0a  d_code.down-1]..
-00004580: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-00004590: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
-000045a0: 7450 6f73 6974 696f 6e28 7365 6c66 2c20  tPosition(self, 
-000045b0: 2a2a 6b77 6172 6773 2920 2d3e 2069 6e74  **kwargs) -> int
-000045c0: 3a0d 0a20 2020 2020 2020 2022 2222 4765  :..        """Ge
-000045d0: 7420 7468 6520 6375 7272 656e 7420 706f  t the current po
-000045e0: 7369 7469 6f6e 206f 6620 7468 6520 7069  sition of the pi
-000045f0: 7065 7474 6522 2222 0d0a 2020 2020 2020  pette"""..      
-00004600: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00004610: 662e 5f71 7565 7279 2827 4450 2729 0d0a  f._query('DP')..
-00004620: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00004630: 2020 2020 2020 2020 2020 706f 7369 7469            positi
-00004640: 6f6e 203d 2069 6e74 2872 6573 706f 6e73  on = int(respons
-00004650: 6529 0d0a 2020 2020 2020 2020 6578 6365  e)..        exce
-00004660: 7074 2056 616c 7565 4572 726f 723a 0d0a  pt ValueError:..
-00004670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004680: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-00004690: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-000046a0: 6f6e 203d 2070 6f73 6974 696f 6e0d 0a20  on = position.. 
-000046b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000046c0: 6c66 2e70 6f73 6974 696f 6e0d 0a20 2020  lf.position..   
-000046d0: 2020 200d 0a20 2020 2064 6566 2067 6574     ..    def get
-000046e0: 5374 6174 7573 2873 656c 662c 202a 2a6b  Status(self, **k
-000046f0: 7761 7267 7329 202d 3e20 7374 723a 0d0a  wargs) -> str:..
-00004700: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004710: 2020 2020 2047 6574 2074 6865 2073 7461       Get the sta
-00004720: 7475 7320 6f66 2074 6865 2070 6970 6574  tus of the pipet
-00004730: 7465 0d0a 0d0a 2020 2020 2020 2020 5265  te....        Re
-00004740: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00004750: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
-00004760: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00004770: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00004780: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00004790: 7175 6572 7928 2744 5327 290d 0a20 2020  query('DS')..   
-000047a0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000047b0: 2020 2020 2020 2073 7461 7475 7320 3d20         status = 
-000047c0: 696e 7428 7265 7370 6f6e 7365 290d 0a20  int(response).. 
-000047d0: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-000047e0: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
-000047f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00004800: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00004810: 6966 2072 6573 706f 6e73 6520 6e6f 7420  if response not 
-00004820: 696e 205b 5f73 7461 7475 732e 7661 6c75  in [_status.valu
-00004830: 6520 666f 7220 5f73 7461 7475 7320 696e  e for _status in
-00004840: 2053 7461 7475 7343 6f64 655d 3a0d 0a20   StatusCode]:.. 
-00004850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004860: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
-00004870: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
-00004880: 6c66 2e5f 7374 6174 7573 5f63 6f64 6520  lf._status_code 
-00004890: 3d20 7374 6174 7573 0d0a 2020 2020 2020  = status..      
-000048a0: 2020 6966 2073 7461 7475 7320 696e 205b    if status in [
-000048b0: 342c 362c 385d 3a0d 0a20 2020 2020 2020  4,6,8]:..       
-000048c0: 2020 2020 2073 656c 662e 7365 7446 6c61       self.setFla
-000048d0: 6728 6275 7379 3d54 7275 6529 0d0a 2020  g(busy=True)..  
-000048e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000048f0: 662e 7665 7262 6f73 653a 0d0a 2020 2020  f.verbose:..    
-00004900: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00004910: 7428 5374 6174 7573 436f 6465 2873 7461  t(StatusCode(sta
-00004920: 7475 7329 2e6e 616d 6529 0d0a 2020 2020  tus).name)..    
-00004930: 2020 2020 656c 6966 2073 7461 7475 7320      elif status 
-00004940: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-00004950: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
-00004960: 6275 7379 3d46 616c 7365 290d 0a20 2020  busy=False)..   
-00004970: 2020 2020 2072 6574 7572 6e20 5374 6174       return Stat
-00004980: 7573 436f 6465 2873 656c 662e 5f73 7461  usCode(self._sta
-00004990: 7475 735f 636f 6465 292e 6e61 6d65 0d0a  tus_code).name..
-000049a0: 2020 2020 0d0a 2020 2020 6465 6620 686f      ..    def ho
-000049b0: 6d65 2873 656c 6629 202d 3e20 7374 723a  me(self) -> str:
-000049c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000049d0: 2020 2020 2020 2052 6574 7572 6e20 706c         Return pl
-000049e0: 756e 6765 7220 746f 2068 6f6d 6520 706f  unger to home po
-000049f0: 7369 7469 6f6e 0d0a 2020 2020 2020 2020  sition..        
-00004a00: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00004a10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004a20: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
-00004a30: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
-00004a40: 220d 0a20 2020 2020 2020 2072 6573 706f  "..        respo
-00004a50: 6e73 6520 3d20 7365 6c66 2e5f 7175 6572  nse = self._quer
-00004a60: 7928 6627 5250 7b73 656c 662e 686f 6d65  y(f'RP{self.home
-00004a70: 5f70 6f73 6974 696f 6e7d 2729 0d0a 2020  _position}')..  
-00004a80: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-00004a90: 6520 3d20 300d 0a20 2020 2020 2020 2073  e = 0..        s
-00004aa0: 656c 662e 706f 7369 7469 6f6e 203d 2073  elf.position = s
-00004ab0: 656c 662e 686f 6d65 5f70 6f73 6974 696f  elf.home_positio
-00004ac0: 6e0d 0a20 2020 2020 2020 2074 696d 652e  n..        time.
-00004ad0: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
-00004ae0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00004af0: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
-00004b00: 2069 7346 6561 7369 626c 6528 7365 6c66   isFeasible(self
-00004b10: 2c20 706f 7369 7469 6f6e 3a69 6e74 2920  , position:int) 
-00004b20: 2d3e 2062 6f6f 6c3a 0d0a 2020 2020 2020  -> bool:..      
-00004b30: 2020 2222 220d 0a20 2020 2020 2020 2043    """..        C
-00004b40: 6865 636b 7320 616e 6420 7265 7475 726e  hecks and return
-00004b50: 7320 7768 6574 6865 7220 7468 6520 706c  s whether the pl
-00004b60: 756e 6765 7220 706f 7369 7469 6f6e 2069  unger position i
-00004b70: 7320 6665 6173 6962 6c65 0d0a 0d0a 2020  s feasible....  
-00004b80: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00004b90: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-00004ba0: 6e20 2869 6e74 293a 2070 6c75 6e67 6572  n (int): plunger
-00004bb0: 2070 6f73 6974 696f 6e0d 0a0d 0a20 2020   position....   
-00004bc0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00004bd0: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
-00004be0: 2077 6865 7468 6572 2070 6c75 6e67 6572   whether plunger
-00004bf0: 2070 6f73 6974 696f 6e20 6973 2066 6561   position is fea
-00004c00: 7369 626c 650d 0a20 2020 2020 2020 2022  sible..        "
-00004c10: 2222 0d0a 2020 2020 2020 2020 6966 2028  ""..        if (
-00004c20: 7365 6c66 2e6c 696d 6974 735b 305d 203c  self.limits[0] <
-00004c30: 3d20 706f 7369 7469 6f6e 203c 3d20 7365  = position <= se
-00004c40: 6c66 2e6c 696d 6974 735b 315d 293a 0d0a  lf.limits[1]):..
-00004c50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004c60: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
-00004c70: 2070 7269 6e74 2866 2252 616e 6765 206c   print(f"Range l
-00004c80: 696d 6974 7320 7265 6163 6865 6421 207b  imits reached! {
-00004c90: 7365 6c66 2e6c 696d 6974 737d 2229 0d0a  self.limits}")..
-00004ca0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00004cb0: 616c 7365 0d0a 2020 2020 0d0a 2020 2020  alse..    ..    
-00004cc0: 6465 6620 6973 5469 704f 6e28 7365 6c66  def isTipOn(self
-00004cd0: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
-00004ce0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00004cf0: 2043 6865 636b 7320 616e 6420 7265 7475   Checks and retu
-00004d00: 726e 7320 7768 6574 6865 7220 6120 7069  rns whether a pi
-00004d10: 7065 7474 6520 7469 7020 6973 2061 7474  pette tip is att
-00004d20: 6163 6865 640d 0a20 2020 2020 2020 200d  ached..        .
-00004d30: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004d40: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
-00004d50: 6f6f 6c3a 2077 6865 7468 6572 2061 2070  ool: whether a p
-00004d60: 6970 6574 7465 2074 6970 2069 6e20 6174  ipette tip in at
-00004d70: 7461 6368 6564 0d0a 2020 2020 2020 2020  tached..        
-00004d80: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00004d90: 662e 6765 7443 6170 6163 6974 616e 6365  f.getCapacitance
-00004da0: 2829 0d0a 2020 2020 2020 2020 7072 696e  ()..        prin
-00004db0: 7428 6627 5469 7020 6361 7061 6369 7461  t(f'Tip capacita
-00004dc0: 6e63 653a 207b 7365 6c66 2e63 6170 6163  nce: {self.capac
-00004dd0: 6974 616e 6365 7d27 290d 0a20 2020 2020  itance}')..     
-00004de0: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
-00004df0: 5b27 636f 6e64 7563 7469 7665 5f74 6970  ['conductive_tip
-00004e00: 7327 5d3a 0d0a 2020 2020 2020 2020 2020  s']:..          
-00004e10: 2020 7469 705f 6f6e 203d 2028 7365 6c66    tip_on = (self
-00004e20: 2e63 6170 6163 6974 616e 6365 203e 2073  .capacitance > s
-00004e30: 656c 662e 7469 705f 7468 7265 7368 6f6c  elf.tip_threshol
-00004e40: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00004e50: 7365 6c66 2e73 6574 466c 6167 2874 6970  self.setFlag(tip
-00004e60: 5f6f 6e3d 7469 705f 6f6e 290d 0a20 2020  _on=tip_on)..   
-00004e70: 2020 2020 2074 6970 5f6f 6e20 3d20 7365       tip_on = se
-00004e80: 6c66 2e66 6c61 6773 5b27 7469 705f 6f6e  lf.flags['tip_on
-00004e90: 275d 0d0a 2020 2020 2020 2020 7265 7475  ']..        retu
-00004ea0: 726e 2074 6970 5f6f 6e0d 0a20 2020 200d  rn tip_on..    .
-00004eb0: 0a20 2020 2064 6566 206d 6f76 6528 7365  .    def move(se
-00004ec0: 6c66 2c20 7374 6570 733a 696e 742c 2075  lf, steps:int, u
-00004ed0: 703a 626f 6f6c 2c20 2a2a 6b77 6172 6773  p:bool, **kwargs
-00004ee0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00004ef0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004f00: 4d6f 7665 2074 6865 2070 6c75 6e67 6572  Move the plunger
-00004f10: 2065 6974 6865 7220 7570 206f 7220 646f   either up or do
-00004f20: 776e 2062 7920 6120 7370 6563 6966 6965  wn by a specifie
-00004f30: 6420 6e75 6d62 6572 206f 6620 7374 6570  d number of step
-00004f40: 730d 0a0d 0a20 2020 2020 2020 2041 7267  s....        Arg
-00004f50: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004f60: 7374 6570 7320 2869 6e74 293a 206e 756d  steps (int): num
-00004f70: 6265 7220 6f66 2073 7465 7073 2074 6f20  ber of steps to 
-00004f80: 6d6f 7665 2070 6c75 6e67 6572 2062 790d  move plunger by.
-00004f90: 0a20 2020 2020 2020 2020 2020 2075 7020  .            up 
-00004fa0: 2862 6f6f 6c29 3a20 7768 6574 6865 7220  (bool): whether 
-00004fb0: 746f 206d 6f76 6520 7468 6520 706c 756e  to move the plun
-00004fc0: 6765 7220 7570 0d0a 0d0a 2020 2020 2020  ger up....      
-00004fd0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00004fe0: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
-00004ff0: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
-00005000: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005010: 2020 2073 7465 7073 203d 2061 6273 2873     steps = abs(s
-00005020: 7465 7073 2920 6966 2075 7020 656c 7365  teps) if up else
-00005030: 202d 6162 7328 7374 6570 7329 0d0a 2020   -abs(steps)..  
-00005040: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005050: 662e 6d6f 7665 4279 2873 7465 7073 290d  f.moveBy(steps).
-00005060: 0a20 2020 200d 0a20 2020 2064 6566 206d  .    ..    def m
-00005070: 6f76 6542 7928 7365 6c66 2c20 7374 6570  oveBy(self, step
-00005080: 733a 696e 742c 202a 2a6b 7761 7267 7329  s:int, **kwargs)
-00005090: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-000050a0: 2020 2222 220d 0a20 2020 2020 2020 204d    """..        M
-000050b0: 6f76 6520 7468 6520 706c 756e 6765 7220  ove the plunger 
-000050c0: 6279 2073 7065 6369 6669 6564 206e 756d  by specified num
-000050d0: 6265 7220 6f66 2073 7465 7073 0d0a 0d0a  ber of steps....
-000050e0: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
-000050f0: 2020 2020 2020 2020 2020 2073 7465 7073             steps
-00005100: 2028 696e 7429 3a20 6e75 6d62 6572 206f   (int): number o
-00005110: 6620 7374 6570 7320 746f 206d 6f76 6520  f steps to move 
-00005120: 706c 756e 6765 7220 6279 2028 3c30 3a20  plunger by (<0: 
-00005130: 6d6f 7665 2064 6f77 6e2f 6469 7370 656e  move down/dispen
-00005140: 7365 3b20 3e30 206d 6f76 6520 7570 2f61  se; >0 move up/a
-00005150: 7370 6972 6174 6529 0d0a 0d0a 2020 2020  spirate)....    
-00005160: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-00005170: 2020 2020 2020 2020 2020 7374 723a 2064            str: d
-00005180: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
-00005190: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000051a0: 2020 2020 2063 6f6d 6d61 6e64 203d 2066       command = f
-000051b0: 2752 497b 7374 6570 737d 2720 6966 2073  'RI{steps}' if s
-000051c0: 7465 7073 203e 2030 2065 6c73 6520 6627  teps > 0 else f'
-000051d0: 524f 7b2d 7374 6570 737d 270d 0a20 2020  RO{-steps}'..   
-000051e0: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-000051f0: 6f6e 202b 3d20 7374 6570 730d 0a20 2020  on += steps..   
-00005200: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00005210: 2e5f 7175 6572 7928 636f 6d6d 616e 6429  ._query(command)
-00005220: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00005230: 6d6f 7665 546f 2873 656c 662c 2070 6f73  moveTo(self, pos
-00005240: 6974 696f 6e3a 696e 742c 202a 2a6b 7761  ition:int, **kwa
-00005250: 7267 7329 202d 3e20 7374 723a 0d0a 2020  rgs) -> str:..  
-00005260: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005270: 2020 204d 6f76 6520 7468 6520 706c 756e     Move the plun
-00005280: 6765 7220 746f 2061 2073 7065 6369 6669  ger to a specifi
-00005290: 6564 2070 6f73 6974 696f 6e0d 0a0d 0a20  ed position.... 
-000052a0: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
-000052b0: 2020 2020 2020 2020 2020 706f 7369 7469            positi
-000052c0: 6f6e 2028 696e 7429 3a20 7461 7267 6574  on (int): target
-000052d0: 2070 6c75 6e67 6572 2070 6f73 6974 696f   plunger positio
-000052e0: 6e0d 0a0d 0a20 2020 2020 2020 2052 6574  n....        Ret
-000052f0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00005300: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
-00005310: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00005320: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-00005330: 6c66 2e70 6f73 6974 696f 6e20 3d20 706f  lf.position = po
-00005340: 7369 7469 6f6e 0d0a 2020 2020 2020 2020  sition..        
-00005350: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
-00005360: 7279 2866 2752 507b 706f 7369 7469 6f6e  ry(f'RP{position
-00005370: 7d27 290d 0a20 2020 200d 0a20 2020 2064  }')..    ..    d
-00005380: 6566 2070 756c 6c62 6163 6b28 7365 6c66  ef pullback(self
-00005390: 2c20 7374 6570 733a 696e 7420 3d20 352c  , steps:int = 5,
-000053a0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
-000053b0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-000053c0: 0a20 2020 2020 2020 2050 756c 6c62 6163  .        Pullbac
-000053d0: 6b20 6c69 7175 6964 2066 726f 6d20 7469  k liquid from ti
-000053e0: 700d 0a20 2020 2020 2020 200d 0a20 2020  p..        ..   
-000053f0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
-00005400: 2020 2020 2020 2020 7374 6570 7320 2869          steps (i
-00005410: 6e74 2c20 6f70 7469 6f6e 616c 293a 206e  nt, optional): n
-00005420: 756d 6265 7220 6f66 2073 7465 7073 2074  umber of steps t
-00005430: 6f20 7075 6c6c 6261 636b 2e20 4465 6661  o pullback. Defa
-00005440: 756c 7473 2074 6f20 352e 0d0a 0d0a 2020  ults to 5.....  
-00005450: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005460: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00005470: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00005480: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005490: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-000054a0: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
-000054b0: 5249 7b73 7465 7073 7d27 290d 0a20 2020  RI{steps}')..   
-000054c0: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-000054d0: 6f6e 202b 3d20 7374 6570 730d 0a20 2020  on += steps..   
-000054e0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-000054f0: 3129 0d0a 2020 2020 2020 2020 7265 7475  1)..        retu
-00005500: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-00005510: 200d 0a20 2020 2064 6566 2072 6573 6574   ..    def reset
-00005520: 2873 656c 6629 202d 3e20 7374 723a 0d0a  (self) -> str:..
-00005530: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00005540: 2020 2020 2052 6573 6574 2074 6865 2070       Reset the p
-00005550: 6970 6574 7465 0d0a 0d0a 2020 2020 2020  ipette....      
-00005560: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00005570: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
-00005580: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
-00005590: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000055a0: 2020 2073 656c 662e 7a65 726f 2829 0d0a     self.zero()..
-000055b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000055c0: 656c 662e 686f 6d65 2829 0d0a 2020 2020  elf.home()..    
-000055d0: 0d0a 2020 2020 6465 6620 7365 7453 7065  ..    def setSpe
-000055e0: 6564 2873 656c 662c 2073 7065 6564 3a69  ed(self, speed:i
-000055f0: 6e74 2c20 7570 3a62 6f6f 6c2c 2064 6566  nt, up:bool, def
-00005600: 6175 6c74 3a62 6f6f 6c20 3d20 5472 7565  ault:bool = True
-00005610: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2073  , **kwargs) -> s
-00005620: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-00005630: 0d0a 2020 2020 2020 2020 5365 7420 7468  ..        Set th
-00005640: 6520 7370 6565 6420 6f66 2074 6865 2070  e speed of the p
-00005650: 6c75 6e67 6572 0d0a 0d0a 2020 2020 2020  lunger....      
-00005660: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00005670: 2020 2020 2073 7065 6564 2028 696e 7429       speed (int)
-00005680: 3a20 7370 6565 6420 6f66 2070 6c75 6e67  : speed of plung
-00005690: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-000056a0: 7570 2028 626f 6f6c 293a 2064 6972 6563  up (bool): direc
-000056b0: 7469 6f6e 206f 6620 7472 6176 656c 0d0a  tion of travel..
-000056c0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-000056d0: 756c 7420 2862 6f6f 6c2c 206f 7074 696f  ult (bool, optio
-000056e0: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
-000056f0: 2073 6574 2073 7065 6564 2061 7320 6120   set speed as a 
-00005700: 6465 6661 756c 742e 2044 6566 6175 6c74  default. Default
-00005710: 7320 746f 2054 7275 652e 0d0a 0d0a 2020  s to True.....  
-00005720: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005730: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00005740: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00005750: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005760: 2020 2020 2020 2073 7065 6564 5f63 6f64         speed_cod
-00005770: 6520 3d20 3120 2b20 5b78 2066 6f72 2078  e = 1 + [x for x
-00005780: 2c76 616c 2069 6e20 656e 756d 6572 6174  ,val in enumerat
-00005790: 6528 6e70 2e61 7272 6179 2873 656c 662e  e(np.array(self.
-000057a0: 7370 6565 645f 7072 6573 6574 7329 2d73  speed_presets)-s
-000057b0: 7065 6564 2920 6966 2076 616c 203e 3d20  peed) if val >= 
-000057c0: 305d 5b30 5d0d 0a20 2020 2020 2020 2070  0][0]..        p
-000057d0: 7269 6e74 2866 2753 7065 6564 207b 7370  rint(f'Speed {sp
-000057e0: 6565 645f 636f 6465 7d3a 207b 7365 6c66  eed_code}: {self
-000057f0: 2e73 7065 6564 5f70 7265 7365 7473 5b73  .speed_presets[s
-00005800: 7065 6564 5f63 6f64 652d 315d 7d20 754c  peed_code-1]} uL
-00005810: 2f73 2729 0d0a 2020 2020 2020 2020 6469  /s')..        di
-00005820: 7265 6374 696f 6e20 3d20 2749 2720 6966  rection = 'I' if
-00005830: 2075 7020 656c 7365 2027 4f27 0d0a 2020   up else 'O'..  
-00005840: 2020 2020 2020 7365 6c66 2e5f 7175 6572        self._quer
-00005850: 7928 6627 537b 6469 7265 6374 696f 6e7d  y(f'S{direction}
-00005860: 7b73 7065 6564 5f63 6f64 657d 2729 0d0a  {speed_code}')..
-00005870: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-00005880: 6566 6175 6c74 3a0d 0a20 2020 2020 2020  efault:..       
-00005890: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000058a0: 2e5f 7175 6572 7928 6627 447b 6469 7265  ._query(f'D{dire
-000058b0: 6374 696f 6e7d 2729 0d0a 2020 2020 2020  ction}')..      
-000058c0: 2020 6966 2075 703a 0d0a 2020 2020 2020    if up:..      
-000058d0: 2020 2020 2020 7365 6c66 2e73 7065 6564        self.speed
-000058e0: 5f63 6f64 652e 7570 203d 2073 7065 6564  _code.up = speed
-000058f0: 5f63 6f64 650d 0a20 2020 2020 2020 2020  _code..         
-00005900: 2020 2073 656c 662e 7370 6565 642e 7570     self.speed.up
-00005910: 203d 2073 656c 662e 7370 6565 645f 7072   = self.speed_pr
-00005920: 6573 6574 735b 7370 6565 645f 636f 6465  esets[speed_code
-00005930: 2d31 5d0d 0a20 2020 2020 2020 2065 6c73  -1]..        els
-00005940: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00005950: 7365 6c66 2e73 7065 6564 5f63 6f64 652e  self.speed_code.
-00005960: 646f 776e 203d 2073 7065 6564 5f63 6f64  down = speed_cod
-00005970: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
-00005980: 656c 662e 7370 6565 642e 646f 776e 203d  elf.speed.down =
-00005990: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
-000059a0: 6574 735b 7370 6565 645f 636f 6465 2d31  ets[speed_code-1
-000059b0: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-000059c0: 6e20 7365 6c66 2e5f 7175 6572 7928 6627  n self._query(f'
-000059d0: 447b 6469 7265 6374 696f 6e7d 2729 0d0a  D{direction}')..
-000059e0: 2020 2020 0d0a 2020 2020 6465 6620 7368      ..    def sh
-000059f0: 7574 646f 776e 2873 656c 6629 3a0d 0a20  utdown(self):.. 
-00005a00: 2020 2020 2020 2022 2222 5368 7574 646f         """Shutdo
-00005a10: 776e 2070 726f 6365 6475 7265 2066 6f72  wn procedure for
-00005a20: 2074 6f6f 6c22 2222 0d0a 2020 2020 2020   tool"""..      
-00005a30: 2020 7365 6c66 2e74 6f67 676c 6546 6565    self.toggleFee
-00005a40: 6462 6163 6b4c 6f6f 7028 6f6e 3d46 616c  dbackLoop(on=Fal
-00005a50: 7365 290d 0a20 2020 2020 2020 2072 6574  se)..        ret
-00005a60: 7572 6e20 7375 7065 7228 292e 7368 7574  urn super().shut
-00005a70: 646f 776e 2829 0d0a 2020 2020 0d0a 2020  down()..    ..  
-00005a80: 2020 6465 6620 746f 6767 6c65 4665 6564    def toggleFeed
-00005a90: 6261 636b 4c6f 6f70 2873 656c 662c 206f  backLoop(self, o
-00005aa0: 6e3a 626f 6f6c 293a 0d0a 2020 2020 2020  n:bool):..      
-00005ab0: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
-00005ac0: 7461 7274 206f 7220 7374 6f70 2066 6565  tart or stop fee
-00005ad0: 6462 6163 6b20 6c6f 6f70 0d0a 2020 2020  dback loop..    
-00005ae0: 2020 2020 0d0a 2020 2020 2020 2020 4172      ..        Ar
-00005af0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-00005b00: 206f 6e20 2862 6f6f 6c29 3a20 7768 6574   on (bool): whet
-00005b10: 6865 7220 746f 2073 7461 7274 2066 6565  her to start fee
-00005b20: 6462 6163 6b20 6c6f 6f70 0d0a 2020 2020  dback loop..    
-00005b30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00005b40: 2073 656c 662e 7365 7446 6c61 6728 6765   self.setFlag(ge
-00005b50: 745f 6665 6564 6261 636b 3d6f 6e29 0d0a  t_feedback=on)..
-00005b60: 2020 2020 2020 2020 6966 206f 6e3a 0d0a          if on:..
-00005b70: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-00005b80: 6665 6564 6261 636b 5f6c 6f6f 7027 2069  feedback_loop' i
-00005b90: 6e20 7365 6c66 2e5f 7468 7265 6164 733a  n self._threads:
-00005ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005bb0: 2020 7365 6c66 2e5f 7468 7265 6164 735b    self._threads[
-00005bc0: 2766 6565 6462 6163 6b5f 6c6f 6f70 275d  'feedback_loop']
-00005bd0: 2e6a 6f69 6e28 290d 0a20 2020 2020 2020  .join()..       
-00005be0: 2020 2020 2074 6872 6561 6420 3d20 5468       thread = Th
-00005bf0: 7265 6164 2874 6172 6765 743d 7365 6c66  read(target=self
-00005c00: 2e5f 6c6f 6f70 5f66 6565 6462 6163 6b29  ._loop_feedback)
-00005c10: 0d0a 2020 2020 2020 2020 2020 2020 7468  ..            th
-00005c20: 7265 6164 2e73 7461 7274 2829 0d0a 2020  read.start()..  
-00005c30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00005c40: 7468 7265 6164 735b 2766 6565 6462 6163  threads['feedbac
-00005c50: 6b5f 6c6f 6f70 275d 203d 2074 6872 6561  k_loop'] = threa
-00005c60: 640d 0a20 2020 2020 2020 2065 6c73 653a  d..        else:
-00005c70: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00005c80: 2027 6665 6564 6261 636b 5f6c 6f6f 7027   'feedback_loop'
-00005c90: 2069 6e20 7365 6c66 2e5f 7468 7265 6164   in self._thread
-00005ca0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005cb0: 2020 2020 7365 6c66 2e5f 7468 7265 6164      self._thread
-00005cc0: 735b 2766 6565 6462 6163 6b5f 6c6f 6f70  s['feedback_loop
-00005cd0: 275d 2e6a 6f69 6e28 290d 0a20 2020 2020  '].join()..     
-00005ce0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-00005cf0: 2064 6566 207a 6572 6f28 7365 6c66 2920   def zero(self) 
-00005d00: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
-00005d10: 2022 2222 0d0a 2020 2020 2020 2020 5a65   """..        Ze
-00005d20: 726f 2074 6865 2070 6c75 6e67 6572 2070  ro the plunger p
-00005d30: 6f73 6974 696f 6e0d 0a20 2020 2020 2020  osition..       
-00005d40: 200d 0a20 2020 2020 2020 2052 6574 7572   ..        Retur
-00005d50: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00005d60: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
-00005d70: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
-00005d80: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00005d90: 2e65 6a65 6374 2829 0d0a 2020 2020 2020  .eject()..      
-00005da0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00005db0: 662e 5f71 7565 7279 2827 525a 2729 0d0a  f._query('RZ')..
-00005dc0: 2020 2020 2020 2020 7365 6c66 2e70 6f73          self.pos
-00005dd0: 6974 696f 6e20 3d20 300d 0a20 2020 2020  ition = 0..     
-00005de0: 2020 2074 696d 652e 736c 6565 7028 3229     time.sleep(2)
-00005df0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00005e00: 2072 6573 706f 6e73 650d 0a0d 0a20 2020   response....   
-00005e10: 2023 2050 726f 7465 6374 6564 206d 6574   # Protected met
-00005e20: 686f 6428 7329 0d0a 2020 2020 6465 6620  hod(s)..    def 
-00005e30: 5f63 616c 6375 6c61 7465 5f73 7065 6564  _calculate_speed
-00005e40: 5f70 6172 616d 6574 6572 7328 7365 6c66  _parameters(self
-00005e50: 2c20 766f 6c75 6d65 3a69 6e74 2c20 7370  , volume:int, sp
-00005e60: 6565 643a 696e 7429 202d 3e20 5370 6565  eed:int) -> Spee
-00005e70: 6450 6172 616d 6574 6572 733a 0d0a 2020  dParameters:..  
-00005e80: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005e90: 2020 2043 616c 6375 6c61 7465 7320 7468     Calculates th
-00005ea0: 6520 6265 7374 2070 6172 616d 6574 6572  e best parameter
-00005eb0: 7320 666f 7220 766f 6c75 6d65 2061 6e64  s for volume and
-00005ec0: 2073 7065 6564 0d0a 0d0a 2020 2020 2020   speed....      
-00005ed0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00005ee0: 2020 2020 2076 6f6c 756d 6520 2869 6e74       volume (int
-00005ef0: 293a 2076 6f6c 756d 6520 746f 2062 6520  ): volume to be 
-00005f00: 7472 616e 7366 6572 7265 640d 0a20 2020  transferred..   
-00005f10: 2020 2020 2020 2020 2073 7065 6564 2028           speed (
-00005f20: 696e 7429 3a20 7370 6565 6420 6174 2077  int): speed at w
-00005f30: 6869 6368 206c 6971 7569 6420 6973 2074  hich liquid is t
-00005f40: 7261 6e73 6665 7272 6564 0d0a 0d0a 2020  ransferred....  
-00005f50: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005f60: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-00005f70: 3a20 6469 6374 696f 6e61 7279 206f 6620  : dictionary of 
-00005f80: 6265 7374 2070 6172 616d 6574 6572 730d  best parameters.
-00005f90: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005fa0: 2020 2020 2020 6f75 7463 6f6d 6573 203d        outcomes =
-00005fb0: 207b 7d0d 0a20 2020 2020 2020 2073 7465   {}..        ste
-00005fc0: 705f 696e 7465 7276 616c 5f6c 696d 6974  p_interval_limit
-00005fd0: 203d 2069 6e74 2876 6f6c 756d 652f 7365   = int(volume/se
-00005fe0: 6c66 2e72 6573 6f6c 7574 696f 6e2f 5354  lf.resolution/ST
-00005ff0: 4550 5f52 4553 4f4c 5554 494f 4e29 0d0a  EP_RESOLUTION)..
-00006000: 2020 2020 2020 2020 666f 7220 7072 6573          for pres
-00006010: 6574 2069 6e20 7365 6c66 2e73 7065 6564  et in self.speed
-00006020: 5f70 7265 7365 7473 3a0d 0a20 2020 2020  _presets:..     
-00006030: 2020 2020 2020 2069 6620 7072 6573 6574         if preset
-00006040: 203c 2073 7065 6564 3a0d 0a20 2020 2020   < speed:..     
-00006050: 2020 2020 2020 2020 2020 2023 2070 7265             # pre
-00006060: 7365 7420 6973 2073 6c6f 7765 7220 7468  set is slower th
-00006070: 616e 2074 6172 6765 7420 7370 6565 642c  an target speed,
-00006080: 2069 7420 7769 6c6c 206e 6576 6572 2068   it will never h
-00006090: 6974 2074 6172 6765 7420 7370 6565 640d  it target speed.
-000060a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000060b0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-000060c0: 2020 2020 2020 2074 696d 655f 696e 7465         time_inte
-000060d0: 7276 616c 5f6c 696d 6974 203d 2069 6e74  rval_limit = int
-000060e0: 2876 6f6c 756d 652a 2831 2f73 7065 6564  (volume*(1/speed
-000060f0: 202d 2031 2f70 7265 7365 7429 2f73 656c   - 1/preset)/sel
-00006100: 662e 7265 7370 6f6e 7365 5f74 696d 6529  f.response_time)
-00006110: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00006120: 206e 6f74 2073 7465 705f 696e 7465 7276   not step_interv
-00006130: 616c 5f6c 696d 6974 206f 7220 6e6f 7420  al_limit or not 
-00006140: 7469 6d65 5f69 6e74 6572 7661 6c5f 6c69  time_interval_li
-00006150: 6d69 743a 0d0a 2020 2020 2020 2020 2020  mit:..          
-00006160: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00006170: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-00006180: 7276 616c 7320 3d20 6d61 7828 6d69 6e28  rvals = max(min(
-00006190: 7374 6570 5f69 6e74 6572 7661 6c5f 6c69  step_interval_li
-000061a0: 6d69 742c 2074 696d 655f 696e 7465 7276  mit, time_interv
-000061b0: 616c 5f6c 696d 6974 292c 2031 290d 0a20  al_limit), 1).. 
-000061c0: 2020 2020 2020 2020 2020 2065 6163 685f             each_
-000061d0: 7374 6570 7320 3d20 766f 6c75 6d65 2f73  steps = volume/s
-000061e0: 656c 662e 7265 736f 6c75 7469 6f6e 2f69  elf.resolution/i
-000061f0: 6e74 6572 7661 6c73 0d0a 2020 2020 2020  ntervals..      
-00006200: 2020 2020 2020 6561 6368 5f64 656c 6179        each_delay
-00006210: 203d 2076 6f6c 756d 652a 2831 2f73 7065   = volume*(1/spe
-00006220: 6564 202d 2031 2f70 7265 7365 7429 2f69  ed - 1/preset)/i
-00006230: 6e74 6572 7661 6c73 0d0a 2020 2020 2020  ntervals..      
-00006240: 2020 2020 2020 6172 6561 203d 2030 2e35        area = 0.5
-00006250: 202a 2028 766f 6c75 6d65 2a2a 3229 202a   * (volume**2) *
-00006260: 2028 312f 7365 6c66 2e72 6573 6f6c 7574   (1/self.resolut
-00006270: 696f 6e29 202a 2028 312f 696e 7465 7276  ion) * (1/interv
-00006280: 616c 7329 202a 2028 312f 7370 6565 6420  als) * (1/speed 
-00006290: 2d20 312f 7072 6573 6574 290d 0a20 2020  - 1/preset)..   
-000062a0: 2020 2020 2020 2020 206f 7574 636f 6d65           outcome
-000062b0: 735b 6172 6561 5d20 3d20 5370 6565 6450  s[area] = SpeedP
-000062c0: 6172 616d 6574 6572 7328 7072 6573 6574  arameters(preset
-000062d0: 2c20 696e 7465 7276 616c 732c 2069 6e74  , intervals, int
-000062e0: 2865 6163 685f 7374 6570 7329 2c20 6561  (each_steps), ea
-000062f0: 6368 5f64 656c 6179 290d 0a20 2020 2020  ch_delay)..     
-00006300: 2020 2069 6620 6c65 6e28 6f75 7463 6f6d     if len(outcom
-00006310: 6573 2920 3d3d 2030 3a0d 0a20 2020 2020  es) == 0:..     
-00006320: 2020 2020 2020 2070 7269 6e74 2822 4e6f         print("No
-00006330: 2066 6561 7369 626c 6520 7370 6565 6420   feasible speed 
-00006340: 7061 7261 6d65 7465 7273 2e22 290d 0a20  parameters.").. 
-00006350: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006360: 6e20 5370 6565 6450 6172 616d 6574 6572  n SpeedParameter
-00006370: 7328 4e6f 6e65 2c20 5354 4550 5f52 4553  s(None, STEP_RES
-00006380: 4f4c 5554 494f 4e2c 2053 5445 505f 5245  OLUTION, STEP_RE
-00006390: 534f 4c55 5449 4f4e 2c20 7365 6c66 2e72  SOLUTION, self.r
-000063a0: 6573 706f 6e73 655f 7469 6d65 290d 0a20  esponse_time).. 
-000063b0: 2020 2020 2020 2070 7269 6e74 2866 2742         print(f'B
-000063c0: 6573 7420 7061 7261 6d65 7465 7273 3a20  est parameters: 
-000063d0: 7b6f 7574 636f 6d65 735b 6d69 6e28 6f75  {outcomes[min(ou
-000063e0: 7463 6f6d 6573 295d 7d27 290d 0a20 2020  tcomes)]}')..   
-000063f0: 2020 2020 2072 6574 7572 6e20 6f75 7463       return outc
-00006400: 6f6d 6573 5b6d 696e 286f 7574 636f 6d65  omes[min(outcome
-00006410: 7329 5d0d 0a20 2020 200d 0a20 2020 2064  s)]..    ..    d
-00006420: 6566 205f 636f 6e6e 6563 7428 7365 6c66  ef _connect(self
-00006430: 2c20 706f 7274 3a73 7472 2c20 6261 7564  , port:str, baud
-00006440: 7261 7465 3a69 6e74 203d 2039 3630 302c  rate:int = 9600,
-00006450: 2074 696d 656f 7574 3a69 6e74 203d 2031   timeout:int = 1
-00006460: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00006470: 0a20 2020 2020 2020 2043 6f6e 6e65 6374  .        Connect
-00006480: 696f 6e20 7072 6f63 6564 7572 6520 666f  ion procedure fo
-00006490: 7220 746f 6f6c 0d0a 0d0a 2020 2020 2020  r tool....      
-000064a0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-000064b0: 2020 2020 2070 6f72 7420 2873 7472 293a       port (str):
-000064c0: 2043 4f4d 2070 6f72 7420 6164 6472 6573   COM port addres
-000064d0: 730d 0a20 2020 2020 2020 2020 2020 2062  s..            b
-000064e0: 6175 6472 6174 6520 2869 6e74 2c20 6f70  audrate (int, op
-000064f0: 7469 6f6e 616c 293a 2062 6175 6472 6174  tional): baudrat
-00006500: 652e 2044 6566 6175 6c74 7320 746f 2039  e. Defaults to 9
-00006510: 3630 302e 0d0a 2020 2020 2020 2020 2020  600...          
-00006520: 2020 7469 6d65 6f75 7420 2869 6e74 2c20    timeout (int, 
-00006530: 6f70 7469 6f6e 616c 293a 2074 696d 656f  optional): timeo
-00006540: 7574 2069 6e20 7365 636f 6e64 732e 2044  ut in seconds. D
-00006550: 6566 6175 6c74 7320 746f 2031 2e0d 0a20  efaults to 1... 
-00006560: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00006570: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
-00006580: 696f 6e5f 6465 7461 696c 7320 3d20 7b0d  ion_details = {.
-00006590: 0a20 2020 2020 2020 2020 2020 2027 706f  .            'po
-000065a0: 7274 273a 2070 6f72 742c 0d0a 2020 2020  rt': port,..    
-000065b0: 2020 2020 2020 2020 2762 6175 6472 6174          'baudrat
-000065c0: 6527 3a20 6261 7564 7261 7465 2c0d 0a20  e': baudrate,.. 
-000065d0: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
-000065e0: 6f75 7427 3a20 7469 6d65 6f75 740d 0a20  out': timeout.. 
-000065f0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00006600: 2020 6465 7669 6365 203d 204e 6f6e 650d    device = None.
-00006610: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00006620: 2020 2020 2020 2020 2020 2064 6576 6963             devic
-00006630: 6520 3d20 7365 7269 616c 2e53 6572 6961  e = serial.Seria
-00006640: 6c28 706f 7274 2c20 6261 7564 7261 7465  l(port, baudrate
-00006650: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
-00006660: 7429 0d0a 2020 2020 2020 2020 6578 6365  t)..        exce
-00006670: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00006680: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00006690: 7072 696e 7428 6622 436f 756c 6420 6e6f  print(f"Could no
-000066a0: 7420 636f 6e6e 6563 7420 746f 207b 706f  t connect to {po
-000066b0: 7274 7d22 290d 0a20 2020 2020 2020 2020  rt}")..         
-000066c0: 2020 2069 6620 7365 6c66 2e76 6572 626f     if self.verbo
-000066d0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000066e0: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-000066f0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00006700: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00006710: 6c65 6570 2832 2920 2020 2320 5761 6974  leep(2)   # Wait
-00006720: 2066 6f72 2067 7262 6c20 746f 2069 6e69   for grbl to ini
-00006730: 7469 616c 697a 650d 0a20 2020 2020 2020  tialize..       
-00006740: 2020 2020 2064 6576 6963 652e 666c 7573       device.flus
-00006750: 6849 6e70 7574 2829 0d0a 2020 2020 2020  hInput()..      
-00006760: 2020 2020 2020 7072 696e 7428 6622 436f        print(f"Co
-00006770: 6e6e 6563 7469 6f6e 206f 7065 6e65 6420  nnection opened 
-00006780: 746f 207b 706f 7274 7d22 290d 0a20 2020  to {port}")..   
-00006790: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000067a0: 7446 6c61 6728 636f 6e6e 6563 7465 643d  tFlag(connected=
-000067b0: 5472 7565 290d 0a20 2020 2020 2020 2073  True)..        s
-000067c0: 656c 662e 6465 7669 6365 203d 2064 6576  elf.device = dev
-000067d0: 6963 650d 0a20 2020 2020 2020 2073 656c  ice..        sel
-000067e0: 662e 6765 7449 6e66 6f28 290d 0a20 2020  f.getInfo()..   
-000067f0: 2020 2020 2073 656c 662e 7265 7365 7428       self.reset(
-00006800: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00006810: 6e0d 0a20 2020 200d 0a20 2020 2064 6566  n..    ..    def
-00006820: 205f 6973 5f65 7870 6563 7465 645f 7265   _is_expected_re
-00006830: 706c 7928 7365 6c66 2c20 7265 7370 6f6e  ply(self, respon
-00006840: 7365 3a73 7472 2c20 636f 6d6d 616e 645f  se:str, command_
-00006850: 636f 6465 3a73 7472 2c20 2a2a 6b77 6172  code:str, **kwar
-00006860: 6773 2920 2d3e 2062 6f6f 6c3a 0d0a 2020  gs) -> bool:..  
-00006870: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00006880: 2020 2043 6865 636b 7320 616e 6420 7265     Checks and re
-00006890: 7475 726e 7320 7768 6574 6865 7220 7468  turns whether th
-000068a0: 6520 7265 7370 6f6e 7365 2069 7320 616e  e response is an
-000068b0: 2065 7870 6563 7465 6420 7265 706c 790d   expected reply.
-000068c0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-000068d0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000068e0: 7370 6f6e 7365 2028 7374 7229 3a20 7265  sponse (str): re
-000068f0: 7370 6f6e 7365 2073 7472 696e 6720 6672  sponse string fr
-00006900: 6f6d 2064 6576 6963 650d 0a20 2020 2020  om device..     
-00006910: 2020 2020 2020 2063 6f6d 6d61 6e64 5f63         command_c
-00006920: 6f64 6520 2873 7472 293a 2074 776f 2d63  ode (str): two-c
-00006930: 6861 7261 6374 6572 2063 6f6d 6d61 6e64  haracter command
-00006940: 2063 6f64 650d 0a0d 0a20 2020 2020 2020   code....       
-00006950: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00006960: 2020 2020 2020 2062 6f6f 6c3a 2077 6865         bool: whe
-00006970: 7468 6572 2074 6865 2072 6573 706f 6e73  ther the respons
-00006980: 6520 6973 2061 6e20 6578 7065 6374 6564  e is an expected
-00006990: 2072 6570 6c79 0d0a 2020 2020 2020 2020   reply..        
-000069a0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-000069b0: 7265 7370 6f6e 7365 2069 6e20 4572 726f  response in Erro
-000069c0: 7243 6f64 652e 5f6d 656d 6265 725f 6e61  rCode._member_na
-000069d0: 6d65 735f 3a0d 0a20 2020 2020 2020 2020  mes_:..         
-000069e0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-000069f0: 2020 2020 2020 2020 6966 2063 6f6d 6d61          if comma
-00006a00: 6e64 5f63 6f64 6520 6e6f 7420 696e 2051  nd_code not in Q
-00006a10: 5545 5249 4553 2061 6e64 2072 6573 706f  UERIES and respo
-00006a20: 6e73 6520 3d3d 2027 6f6b 273a 0d0a 2020  nse == 'ok':..  
-00006a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006a40: 2054 7275 650d 0a20 2020 2020 2020 2069   True..        i
-00006a50: 6620 636f 6d6d 616e 645f 636f 6465 2069  f command_code i
-00006a60: 6e20 5155 4552 4945 5320 616e 6420 7265  n QUERIES and re
-00006a70: 7370 6f6e 7365 5b3a 325d 203d 3d20 636f  sponse[:2] == co
-00006a80: 6d6d 616e 645f 636f 6465 2e6c 6f77 6572  mmand_code.lower
-00006a90: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00006aa0: 2072 6570 6c79 5f63 6f64 652c 2064 6174   reply_code, dat
-00006ab0: 6120 3d20 7265 7370 6f6e 7365 5b3a 325d  a = response[:2]
-00006ac0: 2c20 7265 7370 6f6e 7365 5b32 3a5d 0d0a  , response[2:]..
-00006ad0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00006ae0: 656c 662e 7665 7262 6f73 653a 0d0a 2020  elf.verbose:..  
-00006af0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00006b00: 696e 7428 6627 5b7b 7265 706c 795f 636f  int(f'[{reply_co
-00006b10: 6465 7d5d 207b 6461 7461 7d27 290d 0a20  de}] {data}').. 
-00006b20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006b30: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
-00006b40: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-00006b50: 2020 2020 6465 6620 5f6c 6f6f 705f 6665      def _loop_fe
-00006b60: 6564 6261 636b 2873 656c 6629 3a0d 0a20  edback(self):.. 
-00006b70: 2020 2020 2020 2022 2222 4c6f 6f70 2074         """Loop t
-00006b80: 6f20 636f 6e73 7461 6e74 6c79 2072 6561  o constantly rea
-00006b90: 6420 6672 6f6d 2064 6576 6963 6522 2222  d from device"""
-00006ba0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00006bb0: 274c 6973 7465 6e69 6e67 2e2e 2e27 290d  'Listening...').
-00006bc0: 0a20 2020 2020 2020 2077 6869 6c65 2073  .        while s
-00006bd0: 656c 662e 666c 6167 735b 2767 6574 5f66  elf.flags['get_f
-00006be0: 6565 6462 6163 6b27 5d3a 0d0a 2020 2020  eedback']:..    
-00006bf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006c00: 666c 6167 735b 2770 6175 7365 5f66 6565  flags['pause_fee
-00006c10: 6462 6163 6b27 5d3a 0d0a 2020 2020 2020  dback']:..      
-00006c20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00006c30: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00006c40: 7365 6c66 2e67 6574 5374 6174 7573 2829  self.getStatus()
-00006c50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00006c60: 6c66 2e67 6574 4361 7061 6369 7461 6e63  lf.getCapacitanc
-00006c70: 6528 290d 0a20 2020 2020 2020 2070 7269  e()..        pri
-00006c80: 6e74 2827 5374 6f70 206c 6973 7465 6e69  nt('Stop listeni
-00006c90: 6e67 2e2e 2e27 290d 0a20 2020 2020 2020  ng...')..       
-00006ca0: 2072 6574 7572 6e0d 0a20 2020 200d 0a20   return..    .. 
-00006cb0: 2020 2064 6566 205f 7175 6572 7928 7365     def _query(se
-00006cc0: 6c66 2c20 0d0a 2020 2020 2020 2020 636f  lf, ..        co
-00006cd0: 6d6d 616e 643a 2073 7472 2c20 0d0a 2020  mmand: str, ..  
-00006ce0: 2020 2020 2020 7469 6d65 6f75 745f 733a        timeout_s:
-00006cf0: 2066 6c6f 6174 203d 2030 2e33 2c20 0d0a   float = 0.3, ..
-00006d00: 2020 2020 2020 2020 7265 7375 6d65 5f66          resume_f
-00006d10: 6565 6462 6163 6b3a 2062 6f6f 6c20 3d20  eedback: bool = 
-00006d20: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00006d30: 6765 745f 706f 7369 7469 6f6e 3a20 626f  get_position: bo
-00006d40: 6f6c 203d 2054 7275 650d 0a20 2020 2029  ol = True..    )
-00006d50: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-00006d60: 2020 2222 220d 0a20 2020 2020 2020 2057    """..        W
-00006d70: 7269 7465 2063 6f6d 6d61 6e64 2074 6f20  rite command to 
-00006d80: 616e 6420 7265 6164 2072 6573 706f 6e73  and read respons
-00006d90: 6520 6672 6f6d 2064 6576 6963 650d 0a0d  e from device...
-00006da0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00006db0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-00006dc0: 616e 6420 2873 7472 293a 2063 6f6d 6d61  and (str): comma
-00006dd0: 6e64 2073 7472 696e 670d 0a20 2020 2020  nd string..     
-00006de0: 2020 2020 2020 2074 696d 656f 7574 5f73         timeout_s
-00006df0: 2028 666c 6f61 742c 206f 7074 696f 6e61   (float, optiona
-00006e00: 6c29 3a20 6475 7261 7469 6f6e 2074 6f20  l): duration to 
-00006e10: 7761 6974 2062 6566 6f72 6520 7469 6d65  wait before time
-00006e20: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
-00006e30: 2030 2e33 2e0d 0a20 2020 2020 2020 2020   0.3...         
-00006e40: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
-00006e50: 636b 2028 626f 6f6c 2c20 6f70 7469 6f6e  ck (bool, option
-00006e60: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
-00006e70: 7265 7375 6d65 2072 6561 6469 6e67 2066  resume reading f
-00006e80: 726f 6d20 6465 7669 6365 2e20 4465 6661  rom device. Defa
-00006e90: 756c 7473 2074 6f20 4661 6c73 652e 0d0a  ults to False...
-00006ea0: 2020 2020 2020 2020 2020 2020 6765 745f              get_
-00006eb0: 706f 7369 7469 6f6e 2028 626f 6f6c 2c20  position (bool, 
-00006ec0: 6f70 7469 6f6e 616c 293a 2077 6865 7468  optional): wheth
-00006ed0: 6572 2074 6f20 6765 7420 7468 6520 706f  er to get the po
-00006ee0: 7369 7469 6f6e 206f 6620 7468 6520 706c  sition of the pl
-00006ef0: 756e 6765 722e 2044 6566 6175 6c74 7320  unger. Defaults 
-00006f00: 746f 2054 7275 652e 0d0a 2020 2020 2020  to True...      
-00006f10: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00006f20: 2020 2020 2020 2020 7374 723a 2072 6573          str: res
-00006f30: 706f 6e73 6520 7374 7269 6e67 0d0a 2020  ponse string..  
-00006f40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00006f50: 2020 2063 6f6d 6d61 6e64 5f63 6f64 6520     command_code 
-00006f60: 3d20 636f 6d6d 616e 645b 3a32 5d0d 0a20  = command[:2].. 
-00006f70: 2020 2020 2020 2069 6620 636f 6d6d 616e         if comman
-00006f80: 645f 636f 6465 206e 6f74 2069 6e20 5354  d_code not in ST
-00006f90: 4154 5553 5f51 5545 5249 4553 3a0d 0a20  ATUS_QUERIES:.. 
-00006fa0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00006fb0: 6c66 2e66 6c61 6773 5b27 6765 745f 6665  lf.flags['get_fe
-00006fc0: 6564 6261 636b 275d 2061 6e64 206e 6f74  edback'] and not
-00006fd0: 2073 656c 662e 666c 6167 735b 2770 6175   self.flags['pau
-00006fe0: 7365 5f66 6565 6462 6163 6b27 5d3a 0d0a  se_feedback']:..
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 7365 6c66 2e73 6574 466c 6167 2870 6175  self.setFlag(pau
-00007010: 7365 5f66 6565 6462 6163 6b3d 5472 7565  se_feedback=True
-00007020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007030: 2020 2074 696d 652e 736c 6565 7028 7469     time.sleep(ti
-00007040: 6d65 6f75 745f 7329 0d0a 2020 2020 2020  meout_s)..      
-00007050: 2020 2020 2020 2320 7365 6c66 2e67 6574        # self.get
-00007060: 5374 6174 7573 2829 0d0a 2020 2020 2020  Status()..      
-00007070: 2020 2020 2020 2320 7768 696c 6520 7365        # while se
-00007080: 6c66 2e69 7342 7573 7928 293a 0d0a 2020  lf.isBusy():..  
-00007090: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-000070a0: 7365 6c66 2e67 6574 5374 6174 7573 2829  self.getStatus()
-000070b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000070c0: 2073 656c 662e 6973 4275 7379 2829 3a0d   self.isBusy():.
-000070d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000070e0: 2074 696d 652e 736c 6565 7028 7469 6d65   time.sleep(time
-000070f0: 6f75 745f 7329 0d0a 2020 2020 2020 2020  out_s)..        
-00007100: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
-00007110: 7469 6d65 203d 2074 696d 652e 7065 7266  time = time.perf
-00007120: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
-00007130: 2020 2020 7365 6c66 2e5f 7772 6974 6528      self._write(
-00007140: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
-00007150: 2020 7265 7370 6f6e 7365 203d 2027 270d    response = ''.
-00007160: 0a20 2020 2020 2020 2077 6869 6c65 206e  .        while n
-00007170: 6f74 2073 656c 662e 5f69 735f 6578 7065  ot self._is_expe
-00007180: 6374 6564 5f72 6570 6c79 2872 6573 706f  cted_reply(respo
-00007190: 6e73 652c 2063 6f6d 6d61 6e64 5f63 6f64  nse, command_cod
-000071a0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-000071b0: 2069 6620 7469 6d65 2e70 6572 665f 636f   if time.perf_co
-000071c0: 756e 7465 7228 2920 2d20 7374 6172 745f  unter() - start_
-000071d0: 7469 6d65 203e 2074 696d 656f 7574 5f73  time > timeout_s
-000071e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000071f0: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
-00007200: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00007210: 2073 656c 662e 5f72 6561 6428 290d 0a20   self._read().. 
-00007220: 2020 2020 2020 2023 2070 7269 6e74 2874         # print(t
-00007230: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
-00007240: 2829 202d 2073 7461 7274 5f74 696d 6529  () - start_time)
-00007250: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
-00007260: 6d61 6e64 5f63 6f64 6520 696e 2051 5545  mand_code in QUE
-00007270: 5249 4553 3a0d 0a20 2020 2020 2020 2020  RIES:..         
-00007280: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
-00007290: 7370 6f6e 7365 5b32 3a5d 0d0a 2020 2020  sponse[2:]..    
-000072a0: 2020 2020 6966 2063 6f6d 6d61 6e64 5f63      if command_c
-000072b0: 6f64 6520 6e6f 7420 696e 2053 5441 5455  ode not in STATU
-000072c0: 535f 5155 4552 4945 533a 0d0a 2020 2020  S_QUERIES:..    
-000072d0: 2020 2020 2020 2020 6966 2067 6574 5f70          if get_p
-000072e0: 6f73 6974 696f 6e3a 0d0a 2020 2020 2020  osition:..      
-000072f0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00007300: 6574 506f 7369 7469 6f6e 2829 0d0a 2020  etPosition()..  
-00007310: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-00007320: 756d 655f 6665 6564 6261 636b 3a0d 0a20  ume_feedback:.. 
-00007330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007340: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
-00007350: 655f 6665 6564 6261 636b 3d46 616c 7365  e_feedback=False
-00007360: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00007370: 6e20 7265 7370 6f6e 7365 0d0a 0d0a 2020  n response....  
-00007380: 2020 6465 6620 5f72 6561 6428 7365 6c66    def _read(self
-00007390: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-000073a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000073b0: 5265 6164 2072 6573 706f 6e73 6520 6672  Read response fr
-000073c0: 6f6d 2064 6576 6963 650d 0a0d 0a20 2020  om device....   
-000073d0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-000073e0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
-000073f0: 7265 7370 6f6e 7365 2073 7472 696e 670d  response string.
-00007400: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00007410: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00007420: 2027 270d 0a20 2020 2020 2020 2074 7279   ''..        try
-00007430: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00007440: 6573 706f 6e73 6520 3d20 7365 6c66 2e64  esponse = self.d
-00007450: 6576 6963 652e 7265 6164 6c69 6e65 2829  evice.readline()
-00007460: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00007470: 206c 656e 2872 6573 706f 6e73 6529 203d   len(response) =
-00007480: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-00007490: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-000074a0: 2073 656c 662e 6465 7669 6365 2e72 6561   self.device.rea
-000074b0: 646c 696e 6528 290d 0a20 2020 2020 2020  dline()..       
-000074c0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-000074d0: 7265 7370 6f6e 7365 5b32 3a2d 325d 2e64  response[2:-2].d
-000074e0: 6563 6f64 6528 2775 7466 2d38 2729 0d0a  ecode('utf-8')..
-000074f0: 2020 2020 2020 2020 6578 6365 7074 2041          except A
-00007500: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
-00007510: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00007520: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00007530: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00007540: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00007550: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
-00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
-00007580: 2020 6966 2072 6573 706f 6e73 6520 696e    if response in
-00007590: 2045 7272 6f72 436f 6465 2e5f 6d65 6d62   ErrorCode._memb
-000075a0: 6572 5f6e 616d 6573 5f3a 0d0a 2020 2020  er_names_:..    
-000075b0: 2020 2020 2020 2020 7072 696e 7428 4572          print(Er
-000075c0: 726f 7243 6f64 655b 7265 7370 6f6e 7365  rorCode[response
-000075d0: 5d2e 7661 6c75 6529 0d0a 2020 2020 2020  ].value)..      
-000075e0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-000075f0: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
-00007600: 205f 7365 745f 6368 616e 6e65 6c5f 6964   _set_channel_id
-00007610: 2873 656c 662c 206e 6577 5f63 6861 6e6e  (self, new_chann
-00007620: 656c 5f69 643a 696e 7429 3a0d 0a20 2020  el_id:int):..   
-00007630: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00007640: 2020 5365 7420 6368 616e 6e65 6c20 6964    Set channel id
-00007650: 206f 6620 6465 7669 6365 0d0a 0d0a 2020   of device....  
-00007660: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00007670: 2020 2020 2020 2020 206e 6577 5f63 6861           new_cha
-00007680: 6e6e 656c 2028 696e 7429 3a20 6e65 7720  nnel (int): new 
-00007690: 6368 616e 6e65 6c20 6964 0d0a 0d0a 2020  channel id....  
-000076a0: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
-000076b0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-000076c0: 4572 726f 723a 2050 6c65 6173 6520 7365  Error: Please se
-000076d0: 6c65 6374 2061 2076 616c 6964 2072 4c69  lect a valid rLi
-000076e0: 6e65 2061 6464 7265 7373 2066 726f 6d20  ne address from 
-000076f0: 3120 746f 2039 0d0a 2020 2020 2020 2020  1 to 9..        
-00007700: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00007710: 6e6f 7420 2830 203c 206e 6577 5f63 6861  not (0 < new_cha
-00007720: 6e6e 656c 5f69 6420 3c20 3130 293a 0d0a  nnel_id < 10):..
-00007730: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00007740: 6520 5661 6c75 6545 7272 6f72 2827 506c  e ValueError('Pl
-00007750: 6561 7365 2073 656c 6563 7420 6120 7661  ease select a va
-00007760: 6c69 6420 724c 696e 6520 6164 6472 6573  lid rLine addres
-00007770: 7320 6672 6f6d 2031 2074 6f20 392e 2729  s from 1 to 9.')
-00007780: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00007790: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-000077a0: 2866 272a 417b 6e65 775f 6368 616e 6e65  (f'*A{new_channe
-000077b0: 6c5f 6964 7d27 290d 0a20 2020 2020 2020  l_id}')..       
-000077c0: 2069 6620 7265 7370 6f6e 7365 203d 3d20   if response == 
-000077d0: 276f 6b27 3a0d 0a20 2020 2020 2020 2020  'ok':..         
-000077e0: 2020 2073 656c 662e 6368 616e 6e65 6c20     self.channel 
-000077f0: 3d20 6e65 775f 6368 616e 6e65 6c5f 6964  = new_channel_id
-00007800: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00007810: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00007820: 5f77 7269 7465 2873 656c 662c 2063 6f6d  _write(self, com
-00007830: 6d61 6e64 3a73 7472 2920 2d3e 2062 6f6f  mand:str) -> boo
-00007840: 6c3a 0d0a 2020 2020 2020 2020 2222 220d  l:..        """.
-00007850: 0a20 2020 2020 2020 2057 7269 7465 2063  .        Write c
-00007860: 6f6d 6d61 6e64 2074 6f20 6465 7669 6365  ommand to device
-00007870: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
-00007880: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
-00007890: 6f6d 6d61 6e64 2028 7374 7229 3a20 3c63  ommand (str): <c
-000078a0: 6f6d 6d61 6e64 2063 6f64 653e 3c76 616c  ommand code><val
-000078b0: 7565 3e0d 0a0d 0a20 2020 2020 2020 2052  ue>....        R
-000078c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000078d0: 2020 2020 2062 6f6f 6c3a 2077 6865 7468       bool: wheth
-000078e0: 6572 2063 6f6d 6d61 6e64 2077 6173 2073  er command was s
-000078f0: 656e 7420 7375 6363 6573 7366 756c 6c79  ent successfully
-00007900: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00007910: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-00007920: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00007930: 2020 2020 2070 7269 6e74 2863 6f6d 6d61       print(comma
-00007940: 6e64 290d 0a20 2020 2020 2020 2066 7374  nd)..        fst
-00007950: 7269 6e67 203d 2066 2701 7b73 656c 662e  ring = f'.{self.
-00007960: 6368 616e 6e65 6c7d 7b63 6f6d 6d61 6e64  channel}{command
-00007970: 7dc2 ba5c 7227 2023 2063 6f6d 6d61 6e64  }..\r' # command
-00007980: 2074 656d 706c 6174 653a 203c 5052 453e   template: <PRE>
-00007990: 3c41 4452 3e3c 434f 4445 3e3c 4441 5441  <ADR><CODE><DATA
-000079a0: 3e3c 4c52 433e 3c50 4f53 543e 0d0a 2020  ><LRC><POST>..  
-000079b0: 2020 2020 2020 2320 6273 7472 696e 6720        # bstring 
-000079c0: 3d20 6279 7465 6172 7261 792e 6672 6f6d  = bytearray.from
-000079d0: 6865 7828 6673 7472 696e 672e 656e 636f  hex(fstring.enco
-000079e0: 6465 2827 7574 662d 3827 292e 6865 7828  de('utf-8').hex(
-000079f0: 2929 0d0a 2020 2020 2020 2020 7472 793a  ))..        try:
-00007a00: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00007a10: 5479 7069 6361 6c20 7469 6d65 6f75 7420  Typical timeout 
-00007a20: 7761 6974 2069 7320 3430 306d 730d 0a20  wait is 400ms.. 
-00007a30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007a40: 6465 7669 6365 2e77 7269 7465 2866 7374  device.write(fst
-00007a50: 7269 6e67 2e65 6e63 6f64 6528 2775 7466  ring.encode('utf
-00007a60: 2d38 2729 290d 0a20 2020 2020 2020 2065  -8'))..        e
-00007a70: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
-00007a80: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00007a90: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-00007aa0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00007ab0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-00007ac0: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
-00007ad0: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
-00007ae0: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
-00007af0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007b00: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-00007b10: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00007b20: 2020 2020                                    
+000025e0: 2020 2020 2020 2020 2020 2020 2320 7261              # ra
+000025f0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00002600: 2827 5461 7267 6574 2073 7065 6564 206e  ('Target speed n
+00002610: 6f74 2070 6f73 7369 626c 652e 2729 0d0a  ot possible.')..
+00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 7072 696e 7428 2754 6172 6765 7420 7370  print('Target sp
+00002640: 6565 6420 6e6f 7420 706f 7373 6962 6c65  eed not possible
+00002650: 2e27 290d 0a20 2020 2020 2020 2020 2020  .')..           
+00002660: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00002670: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00002680: 7453 7065 6564 2873 7065 6564 3d70 7265  tSpeed(speed=pre
+00002690: 7365 742c 2075 703d 5472 7565 2c20 6465  set, up=True, de
+000026a0: 6661 756c 743d 4661 6c73 6529 0d0a 2020  fault=False)..  
+000026b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000026c0: 2020 2020 2020 2020 7374 6570 735f 6c65          steps_le
+000026d0: 6674 203d 2073 7465 7073 0d0a 2020 2020  ft = steps..    
+000026e0: 2020 2020 2020 2020 6465 6c61 7920 3d20          delay = 
+000026f0: 7370 6565 645f 7061 7261 6d65 7465 7273  speed_parameters
+00002700: 2e64 656c 6179 0d0a 2020 2020 2020 2020  .delay..        
+00002710: 2020 2020 7374 6570 5f73 697a 6520 3d20      step_size = 
+00002720: 7370 6565 645f 7061 7261 6d65 7465 7273  speed_parameters
+00002730: 2e73 7465 705f 7369 7a65 0d0a 2020 2020  .step_size..    
+00002740: 2020 2020 2020 2020 696e 7465 7276 616c          interval
+00002750: 7320 3d20 7370 6565 645f 7061 7261 6d65  s = speed_parame
+00002760: 7465 7273 2e69 6e74 6572 7661 6c73 0d0a  ters.intervals..
+00002770: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00002780: 745f 6173 7069 7261 7465 203d 2074 696d  t_aspirate = tim
+00002790: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
+000027a0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+000027b0: 7220 6920 696e 2072 616e 6765 2869 6e74  r i in range(int
+000027c0: 6572 7661 6c73 293a 0d0a 2020 2020 2020  ervals):..      
+000027d0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+000027e0: 7469 6d65 203d 2074 696d 652e 7065 7266  time = time.perf
+000027f0: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
+00002800: 2020 2020 2020 2020 2020 2020 7374 6570              step
+00002810: 203d 2073 7465 705f 7369 7a65 2069 6620   = step_size if 
+00002820: 2869 2b31 2021 3d20 696e 7465 7276 616c  (i+1 != interval
+00002830: 7329 2065 6c73 6520 7374 6570 735f 6c65  s) else steps_le
+00002840: 6674 0d0a 2020 2020 2020 2020 2020 2020  ft..            
+00002850: 2020 2020 6d6f 7665 5f74 696d 6520 3d20      move_time = 
+00002860: 7374 6570 2a73 656c 662e 7265 736f 6c75  step*self.resolu
+00002870: 7469 6f6e 202f 2070 7265 7365 740d 0a20  tion / preset.. 
+00002880: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002890: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+000028a0: 7175 6572 7928 6627 5249 7b73 7465 707d  query(f'RI{step}
+000028b0: 272c 2072 6573 756d 655f 6665 6564 6261  ', resume_feedba
+000028c0: 636b 3d46 616c 7365 2c20 6765 745f 706f  ck=False, get_po
+000028d0: 7369 7469 6f6e 3d46 616c 7365 290d 0a20  sition=False).. 
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000028f0: 2069 6620 7265 7370 6f6e 7365 2021 3d20   if response != 
+00002900: 276f 6b27 3a0d 0a20 2020 2020 2020 2020  'ok':..         
+00002910: 2020 2020 2020 2023 2020 2020 2070 7269         #     pri
+00002920: 6e74 2822 4173 7069 7261 7469 6f6e 2066  nt("Aspiration f
+00002930: 6169 6c65 6422 290d 0a20 2020 2020 2020  ailed")..       
+00002940: 2020 2020 2020 2020 2023 2020 2020 2072           #     r
+00002950: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 7374 6570 735f 6c65 6674 202d 3d20 7374  steps_left -= st
+00002980: 6570 0d0a 2020 2020 2020 2020 2020 2020  ep..            
+00002990: 2020 2020 6475 7261 7469 6f6e 203d 2074      duration = t
+000029a0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+000029b0: 2829 202d 2073 7461 7274 5f74 696d 650d  () - start_time.
+000029c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029d0: 2069 6620 6475 7261 7469 6f6e 203c 2028   if duration < (
+000029e0: 6465 6c61 792b 6d6f 7665 5f74 696d 6529  delay+move_time)
+000029f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002a00: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00002a10: 7028 6465 6c61 792b 6d6f 7665 5f74 696d  p(delay+move_tim
+00002a20: 652d 6475 7261 7469 6f6e 290d 0a20 2020  e-duration)..   
+00002a30: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+00002a40: 2055 7064 6174 6520 7661 6c75 6573 0d0a   Update values..
+00002a50: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00002a60: 4173 7069 7261 7469 6f6e 2074 696d 653a  Aspiration time:
+00002a70: 207b 7469 6d65 2e70 6572 665f 636f 756e   {time.perf_coun
+00002a80: 7465 7228 292d 7374 6172 745f 6173 7069  ter()-start_aspi
+00002a90: 7261 7465 7d73 2729 0d0a 2020 2020 2020  rate}s')..      
+00002aa0: 2020 7469 6d65 2e73 6c65 6570 2877 6169    time.sleep(wai
+00002ab0: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
+00002ac0: 2e73 6574 466c 6167 286f 6363 7570 6965  .setFlag(occupie
+00002ad0: 643d 4661 6c73 652c 2070 6175 7365 5f66  d=False, pause_f
+00002ae0: 6565 6462 6163 6b3d 4661 6c73 6529 0d0a  eedback=False)..
+00002af0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+00002b00: 506f 7369 7469 6f6e 2829 0d0a 2020 2020  Position()..    
+00002b10: 2020 2020 7365 6c66 2e76 6f6c 756d 6520      self.volume 
+00002b20: 2b3d 2076 6f6c 756d 650d 0a20 2020 2020  += volume..     
+00002b30: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00002b40: 202b 3d20 7374 6570 730d 0a20 2020 2020   += steps..     
+00002b50: 2020 2069 6620 7265 6167 656e 7420 6973     if reagent is
+00002b60: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00002b70: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+00002b80: 6765 6e74 203d 2072 6561 6765 6e74 0d0a  gent = reagent..
+00002b90: 2020 2020 2020 2020 6966 2070 6175 7365          if pause
+00002ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00002bb0: 6e70 7574 2822 5072 6573 7320 2745 6e74  nput("Press 'Ent
+00002bc0: 6572 2720 746f 2070 726f 6365 6564 2e22  er' to proceed."
+00002bd0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00002be0: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00002bf0: 0d0a 2020 2020 6465 6620 626c 6f77 6f75  ..    def blowou
+00002c00: 7428 7365 6c66 2c20 686f 6d65 3a62 6f6f  t(self, home:boo
+00002c10: 6c20 3d20 5472 7565 2c20 2a2a 6b77 6172  l = True, **kwar
+00002c20: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
+00002c30: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002c40: 2020 426c 6f77 6f75 7420 6c69 7175 6964    Blowout liquid
+00002c50: 2066 726f 6d20 7469 700d 0a0d 0a20 2020   from tip....   
+00002c60: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+00002c70: 2020 2020 2020 2020 686f 6d65 2028 626f          home (bo
+00002c80: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2077  ol, optional): w
+00002c90: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
+00002ca0: 2070 6c75 6e67 6572 2074 6f20 686f 6d65   plunger to home
+00002cb0: 2070 6f73 6974 696f 6e2e 2044 6566 6175   position. Defau
+00002cc0: 6c74 7320 746f 2054 7275 652e 0d0a 0d0a  lts to True.....
+00002cd0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00002ce0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00002cf0: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
+00002d00: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
+00002d10: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+00002d20: 203d 2066 2752 427b 7365 6c66 2e68 6f6d   = f'RB{self.hom
+00002d30: 655f 706f 7369 7469 6f6e 7d27 2069 6620  e_position}' if 
+00002d40: 686f 6d65 2065 6c73 6520 2752 4227 0d0a  home else 'RB'..
+00002d50: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00002d60: 203d 2073 656c 662e 5f71 7565 7279 2863   = self._query(c
+00002d70: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
+00002d80: 2073 656c 662e 706f 7369 7469 6f6e 203d   self.position =
+00002d90: 2073 656c 662e 686f 6d65 5f70 6f73 6974   self.home_posit
+00002da0: 696f 6e0d 0a20 2020 2020 2020 2074 696d  ion..        tim
+00002db0: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
+00002dc0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00002dd0: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
+00002de0: 6566 2064 6973 7065 6e73 6528 7365 6c66  ef dispense(self
+00002df0: 2c20 0d0a 2020 2020 2020 2020 766f 6c75  , ..        volu
+00002e00: 6d65 3a20 666c 6f61 742c 200d 0a20 2020  me: float, ..   
+00002e10: 2020 2020 2073 7065 6564 3a20 4f70 7469       speed: Opti
+00002e20: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
+00002e30: 6e65 2c20 0d0a 2020 2020 2020 2020 7761  ne, ..        wa
+00002e40: 6974 3a20 696e 7420 3d20 302c 200d 0a20  it: int = 0, .. 
+00002e50: 2020 2020 2020 2070 6175 7365 3a20 626f         pause: bo
+00002e60: 6f6c 203d 2046 616c 7365 2c20 0d0a 2020  ol = False, ..  
+00002e70: 2020 2020 2020 626c 6f77 6f75 743a 2062        blowout: b
+00002e80: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+00002e90: 2020 2020 2020 626c 6f77 6f75 745f 686f        blowout_ho
+00002ea0: 6d65 3a20 626f 6f6c 203d 2054 7275 652c  me: bool = True,
+00002eb0: 0d0a 2020 2020 2020 2020 666f 7263 655f  ..        force_
+00002ec0: 6469 7370 656e 7365 3a20 626f 6f6c 203d  dispense: bool =
+00002ed0: 2046 616c 7365 2c20 0d0a 2020 2020 2020   False, ..      
+00002ee0: 2020 2a2a 6b77 6172 6773 0d0a 2020 2020    **kwargs..    
+00002ef0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00002f00: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002f10: 4469 7370 656e 7365 2064 6573 6972 6564  Dispense desired
+00002f20: 2076 6f6c 756d 6520 6f66 2072 6561 6765   volume of reage
+00002f30: 6e74 0d0a 0d0a 2020 2020 2020 2020 4172  nt....        Ar
+00002f40: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+00002f50: 2076 6f6c 756d 6520 2866 6c6f 6174 293a   volume (float):
+00002f60: 2074 6172 6765 7420 766f 6c75 6d65 0d0a   target volume..
+00002f70: 2020 2020 2020 2020 2020 2020 7370 6565              spee
+00002f80: 6420 284f 7074 696f 6e61 6c5b 666c 6f61  d (Optional[floa
+00002f90: 745d 2c20 6f70 7469 6f6e 616c 293a 2073  t], optional): s
+00002fa0: 7065 6564 2074 6f20 6469 7370 656e 7365  peed to dispense
+00002fb0: 2061 742e 2044 6566 6175 6c74 7320 746f   at. Defaults to
+00002fc0: 204e 6f6e 652e 0d0a 2020 2020 2020 2020   None...        
+00002fd0: 2020 2020 7761 6974 2028 696e 742c 206f      wait (int, o
+00002fe0: 7074 696f 6e61 6c29 3a20 7469 6d65 2064  ptional): time d
+00002ff0: 656c 6179 2061 6674 6572 2064 6973 7065  elay after dispe
+00003000: 6e73 652e 2044 6566 6175 6c74 7320 746f  nse. Defaults to
+00003010: 2030 2e0d 0a20 2020 2020 2020 2020 2020   0...           
+00003020: 2070 6175 7365 2028 626f 6f6c 2c20 6f70   pause (bool, op
+00003030: 7469 6f6e 616c 293a 2077 6865 7468 6572  tional): whether
+00003040: 2074 6f20 7061 7573 6520 666f 7220 7573   to pause for us
+00003050: 6572 2069 6e74 6572 7665 6e74 696f 6e2e  er intervention.
+00003060: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
+00003070: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
+00003080: 2062 6c6f 776f 7574 2028 626f 6f6c 2c20   blowout (bool, 
+00003090: 6f70 7469 6f6e 616c 293a 2077 6865 7468  optional): wheth
+000030a0: 6572 2070 6572 666f 726d 2062 6c6f 776f  er perform blowo
+000030b0: 7574 2e20 4465 6661 756c 7473 2074 6f20  ut. Defaults to 
+000030c0: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
+000030d0: 2020 2020 626c 6f77 6f75 745f 686f 6d65      blowout_home
+000030e0: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
+000030f0: 293a 2077 6865 7468 6572 2074 6f20 7265  ): whether to re
+00003100: 7475 726e 2074 6865 2070 6c75 6e67 6572  turn the plunger
+00003110: 2068 6f6d 6520 6166 7465 7220 626c 6f77   home after blow
+00003120: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
+00003130: 2054 7275 652e 0d0a 2020 2020 2020 2020   True...        
+00003140: 2020 2020 666f 7263 655f 6469 7370 656e      force_dispen
+00003150: 7365 2028 626f 6f6c 2c20 6f70 7469 6f6e  se (bool, option
+00003160: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
+00003170: 6469 7370 656e 7365 2072 6561 6765 6e74  dispense reagent
+00003180: 2072 6567 6172 646c 6573 732e 2044 6566   regardless. Def
+00003190: 6175 6c74 7320 746f 2046 616c 7365 2e0d  aults to False..
+000031a0: 0a0d 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+000031b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000031c0: 5661 6c75 6545 7272 6f72 3a20 5265 7175  ValueError: Requ
+000031d0: 6972 6564 2064 6973 7065 6e73 6520 766f  ired dispense vo
+000031e0: 6c75 6d65 2069 7320 6772 6561 7465 7220  lume is greater 
+000031f0: 7468 616e 2076 6f6c 756d 6520 696e 2074  than volume in t
+00003200: 6970 0d0a 0d0a 2020 2020 2020 2020 5265  ip....        Re
+00003210: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00003220: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
+00003230: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00003240: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
+00003250: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
+00003260: 655f 6665 6564 6261 636b 3d54 7275 652c  e_feedback=True,
+00003270: 206f 6363 7570 6965 643d 5472 7565 290d   occupied=True).
+00003280: 0a20 2020 2020 2020 2069 6620 666f 7263  .        if forc
+00003290: 655f 6469 7370 656e 7365 3a0d 0a20 2020  e_dispense:..   
+000032a0: 2020 2020 2020 2020 2076 6f6c 756d 6520           volume 
+000032b0: 3d20 6d69 6e28 766f 6c75 6d65 2c20 7365  = min(volume, se
+000032c0: 6c66 2e76 6f6c 756d 6529 0d0a 2020 2020  lf.volume)..    
+000032d0: 2020 2020 656c 6966 2076 6f6c 756d 6520      elif volume 
+000032e0: 3e20 7365 6c66 2e76 6f6c 756d 653a 0d0a  > self.volume:..
+000032f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00003300: 6520 5661 6c75 6545 7272 6f72 2827 5265  e ValueError('Re
+00003310: 7175 6972 6564 2064 6973 7065 6e73 6520  quired dispense 
+00003320: 766f 6c75 6d65 2069 7320 6772 6561 7465  volume is greate
+00003330: 7220 7468 616e 2076 6f6c 756d 6520 696e  r than volume in
+00003340: 2074 6970 2e27 290d 0a20 2020 2020 2020   tip.')..       
+00003350: 2073 7465 7073 203d 2069 6e74 2876 6f6c   steps = int(vol
+00003360: 756d 6520 2f20 7365 6c66 2e72 6573 6f6c  ume / self.resol
+00003370: 7574 696f 6e29 0d0a 2020 2020 2020 2020  ution)..        
+00003380: 766f 6c75 6d65 203d 2073 7465 7073 202a  volume = steps *
+00003390: 2073 656c 662e 7265 736f 6c75 7469 6f6e   self.resolution
+000033a0: 0d0a 2020 2020 2020 2020 6966 2076 6f6c  ..        if vol
+000033b0: 756d 6520 3d3d 2030 3a0d 0a20 2020 2020  ume == 0:..     
+000033c0: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
+000033d0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+000033e0: 6627 4469 7370 656e 7369 6e67 207b 766f  f'Dispensing {vo
+000033f0: 6c75 6d65 7d20 754c 2e2e 2e27 290d 0a20  lume} uL...').. 
+00003400: 2020 2020 2020 2073 7461 7274 5f64 6973         start_dis
+00003410: 7065 6e73 6520 3d20 7469 6d65 2e70 6572  pense = time.per
+00003420: 665f 636f 756e 7465 7228 290d 0a20 2020  f_counter()..   
+00003430: 2020 2020 2073 7065 6564 203d 2073 656c       speed = sel
+00003440: 662e 7370 6565 642e 646f 776e 2069 6620  f.speed.down if 
+00003450: 7370 6565 6420 6973 204e 6f6e 6520 656c  speed is None el
+00003460: 7365 2073 7065 6564 0d0a 0d0a 2020 2020  se speed....    
+00003470: 2020 2020 6966 2073 7065 6564 2069 6e20      if speed in 
+00003480: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
+00003490: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+000034a0: 2069 6620 7370 6565 6420 213d 2073 656c   if speed != sel
+000034b0: 662e 7370 6565 642e 646f 776e 3a0d 0a20  f.speed.down:.. 
+000034c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000034d0: 656c 662e 7365 7453 7065 6564 2873 7065  elf.setSpeed(spe
+000034e0: 6564 3d73 7065 6564 2c20 7570 3d46 616c  ed=speed, up=Fal
+000034f0: 7365 2c20 6465 6661 756c 743d 4661 6c73  se, default=Fals
+00003500: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00003510: 7374 6172 745f 6469 7370 656e 7365 203d  start_dispense =
+00003520: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
+00003530: 6572 2829 0d0a 2020 2020 2020 2020 2020  er()..          
+00003540: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00003550: 662e 5f71 7565 7279 2866 2752 4f7b 7374  f._query(f'RO{st
+00003560: 6570 737d 2729 0d0a 2020 2020 2020 2020  eps}')..        
+00003570: 2020 2020 6d6f 7665 5f74 696d 6520 3d20      move_time = 
+00003580: 7374 6570 732a 7365 6c66 2e72 6573 6f6c  steps*self.resol
+00003590: 7574 696f 6e20 2f20 7370 6565 640d 0a20  ution / speed.. 
+000035a0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+000035b0: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
+000035c0: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
+000035d0: 745f 6469 7370 656e 7365 0d0a 2020 2020  t_dispense..    
+000035e0: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
+000035f0: 696f 6e20 3c20 286d 6f76 655f 7469 6d65  ion < (move_time
+00003600: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00003610: 2020 2020 7469 6d65 2e73 6c65 6570 286d      time.sleep(m
+00003620: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
+00003630: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00003640: 2320 6966 2072 6573 706f 6e73 6520 213d  # if response !=
+00003650: 2027 6f6b 273a 0d0a 2020 2020 2020 2020   'ok':..        
+00003660: 2020 2020 2320 2020 2020 7265 7475 726e      #     return
+00003670: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00003680: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003690: 2065 6c69 6620 7370 6565 6420 6e6f 7420   elif speed not 
+000036a0: 696e 2073 656c 662e 7370 6565 645f 7072  in self.speed_pr
+000036b0: 6573 6574 733a 0d0a 2020 2020 2020 2020  esets:..        
+000036c0: 2020 2020 7072 696e 7428 6622 5461 7267      print(f"Targ
+000036d0: 6574 3a20 7b76 6f6c 756d 657d 2075 4c20  et: {volume} uL 
+000036e0: 6174 207b 7370 6565 647d 2075 4c2f 732e  at {speed} uL/s.
+000036f0: 2e2e 2229 0d0a 2020 2020 2020 2020 2020  ..")..          
+00003700: 2020 7370 6565 645f 7061 7261 6d65 7465    speed_paramete
+00003710: 7273 203d 2073 656c 662e 5f63 616c 6375  rs = self._calcu
+00003720: 6c61 7465 5f73 7065 6564 5f70 6172 616d  late_speed_param
+00003730: 6574 6572 7328 766f 6c75 6d65 3d76 6f6c  eters(volume=vol
+00003740: 756d 652c 2073 7065 6564 3d73 7065 6564  ume, speed=speed
+00003750: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00003760: 7269 6e74 2873 7065 6564 5f70 6172 616d  rint(speed_param
+00003770: 6574 6572 7329 0d0a 2020 2020 2020 2020  eters)..        
+00003780: 2020 2020 7072 6573 6574 203d 2073 7065      preset = spe
+00003790: 6564 5f70 6172 616d 6574 6572 732e 7072  ed_parameters.pr
+000037a0: 6573 6574 0d0a 2020 2020 2020 2020 2020  eset..          
+000037b0: 2020 6966 2070 7265 7365 7420 6973 204e    if preset is N
+000037c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000037d0: 2020 2020 2020 2320 7261 6973 6520 5275        # raise Ru
+000037e0: 6e74 696d 6545 7272 6f72 2827 5461 7267  ntimeError('Targ
+000037f0: 6574 2073 7065 6564 206e 6f74 2070 6f73  et speed not pos
+00003800: 7369 626c 652e 2729 0d0a 2020 2020 2020  sible.')..      
+00003810: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00003820: 2754 6172 6765 7420 7370 6565 6420 6e6f  'Target speed no
+00003830: 7420 706f 7373 6962 6c65 2e27 290d 0a20  t possible.').. 
+00003840: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003850: 6574 7572 6e0d 0a20 2020 2020 2020 2020  eturn..         
+00003860: 2020 2073 656c 662e 7365 7453 7065 6564     self.setSpeed
+00003870: 2873 7065 6564 3d70 7265 7365 742c 2075  (speed=preset, u
+00003880: 703d 4661 6c73 652c 2064 6566 6175 6c74  p=False, default
+00003890: 3d46 616c 7365 290d 0a20 2020 2020 2020  =False)..       
+000038a0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+000038b0: 7465 7073 5f6c 6566 7420 3d20 7374 6570  teps_left = step
+000038c0: 730d 0a20 2020 2020 2020 2020 2020 2064  s..            d
+000038d0: 656c 6179 203d 2073 7065 6564 5f70 6172  elay = speed_par
+000038e0: 616d 6574 6572 732e 6465 6c61 790d 0a20  ameters.delay.. 
+000038f0: 2020 2020 2020 2020 2020 2073 7465 705f             step_
+00003900: 7369 7a65 203d 2073 7065 6564 5f70 6172  size = speed_par
+00003910: 616d 6574 6572 732e 7374 6570 5f73 697a  ameters.step_siz
+00003920: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00003930: 6e74 6572 7661 6c73 203d 2073 7065 6564  ntervals = speed
+00003940: 5f70 6172 616d 6574 6572 732e 696e 7465  _parameters.inte
+00003950: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
+00003960: 2020 2073 7461 7274 5f64 6973 7065 6e73     start_dispens
+00003970: 6520 3d20 7469 6d65 2e70 6572 665f 636f  e = time.perf_co
+00003980: 756e 7465 7228 290d 0a20 2020 2020 2020  unter()..       
+00003990: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+000039a0: 6e67 6528 696e 7465 7276 616c 7329 3a0d  nge(intervals):.
+000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000039c0: 2073 7461 7274 5f74 696d 6520 3d20 7469   start_time = ti
+000039d0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+000039e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000039f0: 2020 2073 7465 7020 3d20 7374 6570 5f73     step = step_s
+00003a00: 697a 6520 6966 2028 692b 3120 213d 2069  ize if (i+1 != i
+00003a10: 6e74 6572 7661 6c73 2920 656c 7365 2073  ntervals) else s
+00003a20: 7465 7073 5f6c 6566 740d 0a20 2020 2020  teps_left..     
+00003a30: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
+00003a40: 7469 6d65 203d 2073 7465 702a 7365 6c66  time = step*self
+00003a50: 2e72 6573 6f6c 7574 696f 6e20 2f20 7072  .resolution / pr
+00003a60: 6573 6574 0d0a 2020 2020 2020 2020 2020  eset..          
+00003a70: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00003a80: 2073 656c 662e 5f71 7565 7279 2866 2752   self._query(f'R
+00003a90: 4f7b 7374 6570 7d27 2c20 7265 7375 6d65  O{step}', resume
+00003aa0: 5f66 6565 6462 6163 6b3d 4661 6c73 652c  _feedback=False,
+00003ab0: 2067 6574 5f70 6f73 6974 696f 6e3d 4661   get_position=Fa
+00003ac0: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+00003ad0: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
+00003ae0: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
+00003af0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003b00: 2020 2020 7072 696e 7428 2244 6973 7065      print("Dispe
+00003b10: 6e73 6520 6661 696c 6564 2229 0d0a 2020  nse failed")..  
+00003b20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003b30: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00003b40: 6e73 650d 0a20 2020 2020 2020 2020 2020  nse..           
+00003b50: 2020 2020 2073 7465 7073 5f6c 6566 7420       steps_left 
+00003b60: 2d3d 2073 7465 700d 0a20 2020 2020 2020  -= step..       
+00003b70: 2020 2020 2020 2020 2064 7572 6174 696f           duratio
+00003b80: 6e20 3d20 7469 6d65 2e70 6572 665f 636f  n = time.perf_co
+00003b90: 756e 7465 7228 2920 2d20 7374 6172 745f  unter() - start_
+00003ba0: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
+00003bb0: 2020 2020 2020 6966 2064 7572 6174 696f        if duratio
+00003bc0: 6e20 3c20 2864 656c 6179 2b6d 6f76 655f  n < (delay+move_
+00003bd0: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
+00003be0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00003bf0: 2e73 6c65 6570 2864 656c 6179 2b6d 6f76  .sleep(delay+mov
+00003c00: 655f 7469 6d65 2d64 7572 6174 696f 6e29  e_time-duration)
+00003c10: 0d0a 0d0a 2020 2020 2020 2020 2320 5570  ....        # Up
+00003c20: 6461 7465 2076 616c 7565 730d 0a20 2020  date values..   
+00003c30: 2020 2020 2070 7269 6e74 2866 2744 6973       print(f'Dis
+00003c40: 7065 6e73 6520 7469 6d65 3a20 7b74 696d  pense time: {tim
+00003c50: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
+00003c60: 2d73 7461 7274 5f64 6973 7065 6e73 657d  -start_dispense}
+00003c70: 7327 290d 0a20 2020 2020 2020 2074 696d  s')..        tim
+00003c80: 652e 736c 6565 7028 7761 6974 290d 0a20  e.sleep(wait).. 
+00003c90: 2020 2020 2020 2073 656c 662e 7365 7446         self.setF
+00003ca0: 6c61 6728 6f63 6375 7069 6564 3d46 616c  lag(occupied=Fal
+00003cb0: 7365 2c20 7061 7573 655f 6665 6564 6261  se, pause_feedba
+00003cc0: 636b 3d46 616c 7365 290d 0a20 2020 2020  ck=False)..     
+00003cd0: 2020 2073 656c 662e 6765 7450 6f73 6974     self.getPosit
+00003ce0: 696f 6e28 290d 0a20 2020 2020 2020 2073  ion()..        s
+00003cf0: 656c 662e 766f 6c75 6d65 203d 206d 6178  elf.volume = max
+00003d00: 2873 656c 662e 766f 6c75 6d65 202d 2076  (self.volume - v
+00003d10: 6f6c 756d 652c 2030 290d 0a20 2020 2020  olume, 0)..     
+00003d20: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00003d30: 202d 3d20 7374 6570 730d 0a20 2020 2020   -= steps..     
+00003d40: 2020 2069 6620 7365 6c66 2e76 6f6c 756d     if self.volum
+00003d50: 6520 3d3d 2030 2061 6e64 2062 6c6f 776f  e == 0 and blowo
+00003d60: 7574 3a0d 0a20 2020 2020 2020 2020 2020  ut:..           
+00003d70: 2073 656c 662e 626c 6f77 6f75 7428 686f   self.blowout(ho
+00003d80: 6d65 3d62 6c6f 776f 7574 5f68 6f6d 6529  me=blowout_home)
+00003d90: 0d0a 2020 2020 2020 2020 6966 2070 6175  ..        if pau
+00003da0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00003db0: 2069 6e70 7574 2822 5072 6573 7320 2745   input("Press 'E
+00003dc0: 6e74 6572 2720 746f 2070 726f 6365 6564  nter' to proceed
+00003dd0: 2e22 290d 0a20 2020 2020 2020 2072 6574  .")..        ret
+00003de0: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
+00003df0: 2020 0d0a 2020 2020 6465 6620 656a 6563    ..    def ejec
+00003e00: 7428 7365 6c66 2c20 686f 6d65 3a62 6f6f  t(self, home:boo
+00003e10: 6c20 3d20 5472 7565 2920 2d3e 2073 7472  l = True) -> str
+00003e20: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00003e30: 2020 2020 2020 2020 456a 6563 7420 7468          Eject th
+00003e40: 6520 7069 7065 7474 6520 7469 700d 0a0d  e pipette tip...
+00003e50: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00003e60: 2020 2020 2020 2020 2020 2020 686f 6d65              home
+00003e70: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
+00003e80: 293a 2077 6865 7468 6572 2074 6f20 7265  ): whether to re
+00003e90: 7475 726e 2070 6c75 6e67 6572 2074 6f20  turn plunger to 
+00003ea0: 686f 6d65 2070 6f73 6974 696f 6e2e 2044  home position. D
+00003eb0: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
+00003ec0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00003ed0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+00003ee0: 2020 7374 723a 2064 6576 6963 6520 7265    str: device re
+00003ef0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+00003f00: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00003f10: 662e 7265 6167 656e 7420 3d20 2727 0d0a  f.reagent = ''..
+00003f20: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00003f30: 3d20 6627 5245 7b73 656c 662e 686f 6d65  = f'RE{self.home
+00003f40: 5f70 6f73 6974 696f 6e7d 2720 6966 2068  _position}' if h
+00003f50: 6f6d 6520 656c 7365 2027 5245 270d 0a20  ome else 'RE'.. 
+00003f60: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00003f70: 3d20 7365 6c66 2e5f 7175 6572 7928 636f  = self._query(co
+00003f80: 6d6d 616e 6429 0d0a 2020 2020 2020 2020  mmand)..        
+00003f90: 7365 6c66 2e70 6f73 6974 696f 6e20 3d20  self.position = 
+00003fa0: 7365 6c66 2e68 6f6d 655f 706f 7369 7469  self.home_positi
+00003fb0: 6f6e 2069 6620 686f 6d65 2065 6c73 6520  on if home else 
+00003fc0: 300d 0a20 2020 2020 2020 2074 696d 652e  0..        time.
+00003fd0: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
+00003fe0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00003ff0: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
+00004000: 2067 6574 4361 7061 6369 7461 6e63 6528   getCapacitance(
+00004010: 7365 6c66 2920 2d3e 2055 6e69 6f6e 5b69  self) -> Union[i
+00004020: 6e74 2c20 7374 725d 3a0d 0a20 2020 2020  nt, str]:..     
+00004030: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004040: 4765 7420 7468 6520 6361 7061 6369 7461  Get the capacita
+00004050: 6e63 6520 6173 206d 6561 7375 7265 6420  nce as measured 
+00004060: 6174 2074 6865 2065 6e64 206f 6620 7468  at the end of th
+00004070: 6520 7069 7065 7474 650d 0a20 2020 2020  e pipette..     
+00004080: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
+00004090: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000040a0: 2020 2055 6e69 6f6e 5b69 6e74 2c20 7374     Union[int, st
+000040b0: 725d 3a20 6361 7061 6369 7461 6e63 6520  r]: capacitance 
+000040c0: 7661 6c75 652c 206f 7220 6465 7669 6365  value, or device
+000040d0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+000040e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000040f0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00004100: 5f71 7565 7279 2827 444e 2729 0d0a 2020  _query('DN')..  
+00004110: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00004120: 2020 2020 2020 2020 6361 7061 6369 7461          capacita
+00004130: 6e63 6520 3d20 696e 7428 7265 7370 6f6e  nce = int(respon
+00004140: 7365 290d 0a20 2020 2020 2020 2065 7863  se)..        exc
+00004150: 6570 7420 5661 6c75 6545 7272 6f72 3a0d  ept ValueError:.
+00004160: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004170: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
+00004180: 2020 2020 2020 7365 6c66 2e5f 6361 7061        self._capa
+00004190: 6369 7461 6e63 6520 3d20 6361 7061 6369  citance = capaci
+000041a0: 7461 6e63 650d 0a20 2020 2020 2020 2072  tance..        r
+000041b0: 6574 7572 6e20 6361 7061 6369 7461 6e63  eturn capacitanc
+000041c0: 650d 0a20 0d0a 2020 2020 6465 6620 6765  e.. ..    def ge
+000041d0: 7445 7272 6f72 7328 7365 6c66 2920 2d3e  tErrors(self) ->
+000041e0: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
+000041f0: 2222 0d0a 2020 2020 2020 2020 4765 7420  ""..        Get 
+00004200: 6572 726f 7273 2066 726f 6d20 7468 6520  errors from the 
+00004210: 6465 7669 6365 0d0a 0d0a 2020 2020 2020  device....      
+00004220: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00004230: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
+00004240: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
+00004250: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004260: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00004270: 7175 6572 7928 2744 4527 290d 0a20 2020  query('DE')..   
+00004280: 200d 0a20 2020 2064 6566 2067 6574 496e   ..    def getIn
+00004290: 666f 2873 656c 662c 206d 6f64 656c 3a20  fo(self, model: 
+000042a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000042b0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+000042c0: 2222 2247 6574 2064 6574 6169 6c73 206f  """Get details o
+000042d0: 6620 7468 6520 5361 7274 6f72 6975 7320  f the Sartorius 
+000042e0: 7069 7065 7474 6520 6d6f 6465 6c22 2222  pipette model"""
+000042f0: 0d0a 2020 2020 2020 2020 6d6f 6465 6c20  ..        model 
+00004300: 3d20 7365 6c66 2e5f 5f6d 6f64 656c 5f5f  = self.__model__
+00004310: 2829 2e73 706c 6974 2827 2d27 295b 305d  ().split('-')[0]
+00004320: 2069 6620 6d6f 6465 6c20 6973 204e 6f6e   if model is Non
+00004330: 6520 656c 7365 206d 6f64 656c 0d0a 2020  e else model..  
+00004340: 2020 2020 2020 6966 206d 6f64 656c 206e        if model n
+00004350: 6f74 2069 6e20 4d6f 6465 6c49 6e66 6f2e  ot in ModelInfo.
+00004360: 5f6d 656d 6265 725f 6e61 6d65 735f 3a0d  _member_names_:.
+00004370: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004380: 6e74 2866 2752 6563 6569 7665 643a 207b  nt(f'Received: {
+00004390: 6d6f 6465 6c7d 2729 0d0a 2020 2020 2020  model}')..      
+000043a0: 2020 2020 2020 6d6f 6465 6c20 3d20 2742        model = 'B
+000043b0: 524c 3027 0d0a 2020 2020 2020 2020 2020  RL0'..          
+000043c0: 2020 7072 696e 7428 6622 4465 6661 756c    print(f"Defaul
+000043d0: 7469 6e67 2074 6f3a 207b 2742 524c 3027  ting to: {'BRL0'
+000043e0: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
+000043f0: 2070 7269 6e74 2866 2256 616c 6964 206d   print(f"Valid m
+00004400: 6f64 656c 7320 6172 653a 207b 272c 2027  odels are: {', '
+00004410: 2e6a 6f69 6e28 4d6f 6465 6c49 6e66 6f2e  .join(ModelInfo.
+00004420: 5f6d 656d 6265 725f 6e61 6d65 735f 297d  _member_names_)}
+00004430: 2229 0d0a 2020 2020 2020 2020 696e 666f  ")..        info
+00004440: 3a20 4d6f 6465 6c20 3d20 4d6f 6465 6c49  : Model = ModelI
+00004450: 6e66 6f5b 6d6f 6465 6c5d 2e76 616c 7565  nfo[model].value
+00004460: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00004470: 696e 666f 290d 0a20 2020 2020 2020 2073  info)..        s
+00004480: 656c 662e 6d6f 6465 6c5f 696e 666f 203d  elf.model_info =
+00004490: 2069 6e66 6f0d 0a20 2020 2020 2020 2073   info..        s
+000044a0: 656c 662e 6361 7061 6369 7479 203d 2069  elf.capacity = i
+000044b0: 6e66 6f2e 6361 7061 6369 7479 0d0a 2020  nfo.capacity..  
+000044c0: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
+000044d0: 7320 3d20 2869 6e66 6f2e 7469 705f 656a  s = (info.tip_ej
+000044e0: 6563 745f 706f 7369 7469 6f6e 2c20 696e  ect_position, in
+000044f0: 666f 2e6d 6178 5f70 6f73 6974 696f 6e29  fo.max_position)
+00004500: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00004510: 7065 6564 5f70 7265 7365 7473 203d 2069  peed_presets = i
+00004520: 6e66 6f2e 7072 6573 6574 5f73 7065 6564  nfo.preset_speed
+00004530: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+00004540: 7370 6565 642e 7570 203d 2073 656c 662e  speed.up = self.
+00004550: 7370 6565 645f 7072 6573 6574 735b 7365  speed_presets[se
+00004560: 6c66 2e73 7065 6564 5f63 6f64 652e 7570  lf.speed_code.up
+00004570: 2d31 5d0d 0a20 2020 2020 2020 2073 656c  -1]..        sel
+00004580: 662e 7370 6565 642e 646f 776e 203d 2073  f.speed.down = s
+00004590: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
+000045a0: 735b 7365 6c66 2e73 7065 6564 5f63 6f64  s[self.speed_cod
+000045b0: 652e 646f 776e 2d31 5d0d 0a20 2020 2020  e.down-1]..     
+000045c0: 2020 2072 6574 7572 6e0d 0a20 2020 200d     return..    .
+000045d0: 0a20 2020 2064 6566 2067 6574 506f 7369  .    def getPosi
+000045e0: 7469 6f6e 2873 656c 662c 202a 2a6b 7761  tion(self, **kwa
+000045f0: 7267 7329 202d 3e20 696e 743a 0d0a 2020  rgs) -> int:..  
+00004600: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
+00004610: 2063 7572 7265 6e74 2070 6f73 6974 696f   current positio
+00004620: 6e20 6f66 2074 6865 2070 6970 6574 7465  n of the pipette
+00004630: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
+00004640: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
+00004650: 6572 7928 2744 5027 290d 0a20 2020 2020  ery('DP')..     
+00004660: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00004670: 2020 2020 2070 6f73 6974 696f 6e20 3d20       position = 
+00004680: 696e 7428 7265 7370 6f6e 7365 290d 0a20  int(response).. 
+00004690: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+000046a0: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
+000046b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000046c0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+000046d0: 7365 6c66 2e70 6f73 6974 696f 6e20 3d20  self.position = 
+000046e0: 706f 7369 7469 6f6e 0d0a 2020 2020 2020  position..      
+000046f0: 2020 7265 7475 726e 2073 656c 662e 706f    return self.po
+00004700: 7369 7469 6f6e 0d0a 2020 2020 2020 0d0a  sition..      ..
+00004710: 2020 2020 6465 6620 6765 7453 7461 7475      def getStatu
+00004720: 7328 7365 6c66 2c20 2a2a 6b77 6172 6773  s(self, **kwargs
+00004730: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00004740: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004750: 4765 7420 7468 6520 7374 6174 7573 206f  Get the status o
+00004760: 6620 7468 6520 7069 7065 7474 650d 0a0d  f the pipette...
+00004770: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00004780: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00004790: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
+000047a0: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
+000047b0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+000047c0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+000047d0: 2827 4453 2729 0d0a 2020 2020 2020 2020  ('DS')..        
+000047e0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000047f0: 2020 7374 6174 7573 203d 2069 6e74 2872    status = int(r
+00004800: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
+00004810: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00004820: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00004830: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00004840: 650d 0a20 2020 2020 2020 2069 6620 7265  e..        if re
+00004850: 7370 6f6e 7365 206e 6f74 2069 6e20 5b5f  sponse not in [_
+00004860: 7374 6174 7573 2e76 616c 7565 2066 6f72  status.value for
+00004870: 205f 7374 6174 7573 2069 6e20 5374 6174   _status in Stat
+00004880: 7573 436f 6465 5d3a 0d0a 2020 2020 2020  usCode]:..      
+00004890: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000048a0: 706f 6e73 650d 0a20 2020 2020 2020 200d  ponse..        .
+000048b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+000048c0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000048d0: 7475 730d 0a20 2020 2020 2020 2069 6620  tus..        if 
+000048e0: 7374 6174 7573 2069 6e20 5b34 2c36 2c38  status in [4,6,8
+000048f0: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00004900: 7365 6c66 2e73 6574 466c 6167 2862 7573  self.setFlag(bus
+00004910: 793d 5472 7565 290d 0a20 2020 2020 2020  y=True)..       
+00004920: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
+00004930: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+00004940: 2020 2020 2020 2070 7269 6e74 2853 7461         print(Sta
+00004950: 7475 7343 6f64 6528 7374 6174 7573 292e  tusCode(status).
+00004960: 6e61 6d65 290d 0a20 2020 2020 2020 2065  name)..        e
+00004970: 6c69 6620 7374 6174 7573 203d 3d20 303a  lif status == 0:
+00004980: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00004990: 6c66 2e73 6574 466c 6167 2862 7573 793d  lf.setFlag(busy=
+000049a0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+000049b0: 7265 7475 726e 2053 7461 7475 7343 6f64  return StatusCod
+000049c0: 6528 7365 6c66 2e5f 7374 6174 7573 5f63  e(self._status_c
+000049d0: 6f64 6529 2e6e 616d 650d 0a20 2020 200d  ode).name..    .
+000049e0: 0a20 2020 2064 6566 2068 6f6d 6528 7365  .    def home(se
+000049f0: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
+00004a00: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004a10: 2020 5265 7475 726e 2070 6c75 6e67 6572    Return plunger
+00004a20: 2074 6f20 686f 6d65 2070 6f73 6974 696f   to home positio
+00004a30: 6e0d 0a20 2020 2020 2020 200d 0a20 2020  n..        ..   
+00004a40: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+00004a50: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
+00004a60: 6465 7669 6365 2072 6573 706f 6e73 650d  device response.
+00004a70: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00004a80: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00004a90: 2073 656c 662e 5f71 7565 7279 2866 2752   self._query(f'R
+00004aa0: 507b 7365 6c66 2e68 6f6d 655f 706f 7369  P{self.home_posi
+00004ab0: 7469 6f6e 7d27 290d 0a20 2020 2020 2020  tion}')..       
+00004ac0: 2073 656c 662e 766f 6c75 6d65 203d 2030   self.volume = 0
+00004ad0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00004ae0: 6f73 6974 696f 6e20 3d20 7365 6c66 2e68  osition = self.h
+00004af0: 6f6d 655f 706f 7369 7469 6f6e 0d0a 2020  ome_position..  
+00004b00: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00004b10: 2831 290d 0a20 2020 2020 2020 2072 6574  (1)..        ret
+00004b20: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
+00004b30: 2020 0d0a 2020 2020 6465 6620 6973 4665    ..    def isFe
+00004b40: 6173 6962 6c65 2873 656c 662c 2070 6f73  asible(self, pos
+00004b50: 6974 696f 6e3a 696e 7429 202d 3e20 626f  ition:int) -> bo
+00004b60: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
+00004b70: 0d0a 2020 2020 2020 2020 4368 6563 6b73  ..        Checks
+00004b80: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
+00004b90: 7468 6572 2074 6865 2070 6c75 6e67 6572  ther the plunger
+00004ba0: 2070 6f73 6974 696f 6e20 6973 2066 6561   position is fea
+00004bb0: 7369 626c 650d 0a0d 0a20 2020 2020 2020  sible....       
+00004bc0: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00004bd0: 2020 2020 706f 7369 7469 6f6e 2028 696e      position (in
+00004be0: 7429 3a20 706c 756e 6765 7220 706f 7369  t): plunger posi
+00004bf0: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00004c00: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+00004c10: 2020 2020 2020 626f 6f6c 3a20 7768 6574        bool: whet
+00004c20: 6865 7220 706c 756e 6765 7220 706f 7369  her plunger posi
+00004c30: 7469 6f6e 2069 7320 6665 6173 6962 6c65  tion is feasible
+00004c40: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00004c50: 2020 2020 2020 2069 6620 2873 656c 662e         if (self.
+00004c60: 6c69 6d69 7473 5b30 5d20 3c3d 2070 6f73  limits[0] <= pos
+00004c70: 6974 696f 6e20 3c3d 2073 656c 662e 6c69  ition <= self.li
+00004c80: 6d69 7473 5b31 5d29 3a0d 0a20 2020 2020  mits[1]):..     
+00004c90: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00004ca0: 7565 0d0a 2020 2020 2020 2020 7072 696e  ue..        prin
+00004cb0: 7428 6622 5261 6e67 6520 6c69 6d69 7473  t(f"Range limits
+00004cc0: 2072 6561 6368 6564 2120 7b73 656c 662e   reached! {self.
+00004cd0: 6c69 6d69 7473 7d22 290d 0a20 2020 2020  limits}")..     
+00004ce0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00004cf0: 0a20 2020 200d 0a20 2020 2064 6566 2069  .    ..    def i
+00004d00: 7354 6970 4f6e 2873 656c 6629 202d 3e20  sTipOn(self) -> 
+00004d10: 626f 6f6c 3a0d 0a20 2020 2020 2020 2022  bool:..        "
+00004d20: 2222 0d0a 2020 2020 2020 2020 4368 6563  ""..        Chec
+00004d30: 6b73 2061 6e64 2072 6574 7572 6e73 2077  ks and returns w
+00004d40: 6865 7468 6572 2061 2070 6970 6574 7465  hether a pipette
+00004d50: 2074 6970 2069 7320 6174 7461 6368 6564   tip is attached
+00004d60: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00004d70: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00004d80: 2020 2020 2020 2020 2020 626f 6f6c 3a20            bool: 
+00004d90: 7768 6574 6865 7220 6120 7069 7065 7474  whether a pipett
+00004da0: 6520 7469 7020 696e 2061 7474 6163 6865  e tip in attache
+00004db0: 640d 0a20 2020 2020 2020 2022 2222 0d0a  d..        """..
+00004dc0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+00004dd0: 4361 7061 6369 7461 6e63 6528 290d 0a20  Capacitance().. 
+00004de0: 2020 2020 2020 2070 7269 6e74 2866 2754         print(f'T
+00004df0: 6970 2063 6170 6163 6974 616e 6365 3a20  ip capacitance: 
+00004e00: 7b73 656c 662e 6361 7061 6369 7461 6e63  {self.capacitanc
+00004e10: 657d 2729 0d0a 2020 2020 2020 2020 6966  e}')..        if
+00004e20: 2073 656c 662e 666c 6167 735b 2763 6f6e   self.flags['con
+00004e30: 6475 6374 6976 655f 7469 7073 275d 3a0d  ductive_tips']:.
+00004e40: 0a20 2020 2020 2020 2020 2020 2074 6970  .            tip
+00004e50: 5f6f 6e20 3d20 2873 656c 662e 6361 7061  _on = (self.capa
+00004e60: 6369 7461 6e63 6520 3e20 7365 6c66 2e74  citance > self.t
+00004e70: 6970 5f74 6872 6573 686f 6c64 290d 0a20  ip_threshold).. 
+00004e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004e90: 7365 7446 6c61 6728 7469 705f 6f6e 3d74  setFlag(tip_on=t
+00004ea0: 6970 5f6f 6e29 0d0a 2020 2020 2020 2020  ip_on)..        
+00004eb0: 7469 705f 6f6e 203d 2073 656c 662e 666c  tip_on = self.fl
+00004ec0: 6167 735b 2774 6970 5f6f 6e27 5d0d 0a20  ags['tip_on'].. 
+00004ed0: 2020 2020 2020 2072 6574 7572 6e20 7469         return ti
+00004ee0: 705f 6f6e 0d0a 2020 2020 0d0a 2020 2020  p_on..    ..    
+00004ef0: 6465 6620 6d6f 7665 2873 656c 662c 2073  def move(self, s
+00004f00: 7465 7073 3a69 6e74 2c20 7570 3a62 6f6f  teps:int, up:boo
+00004f10: 6c2c 202a 2a6b 7761 7267 7329 202d 3e20  l, **kwargs) -> 
+00004f20: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
+00004f30: 220d 0a20 2020 2020 2020 204d 6f76 6520  "..        Move 
+00004f40: 7468 6520 706c 756e 6765 7220 6569 7468  the plunger eith
+00004f50: 6572 2075 7020 6f72 2064 6f77 6e20 6279  er up or down by
+00004f60: 2061 2073 7065 6369 6669 6564 206e 756d   a specified num
+00004f70: 6265 7220 6f66 2073 7465 7073 0d0a 0d0a  ber of steps....
+00004f80: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+00004f90: 2020 2020 2020 2020 2020 2073 7465 7073             steps
+00004fa0: 2028 696e 7429 3a20 6e75 6d62 6572 206f   (int): number o
+00004fb0: 6620 7374 6570 7320 746f 206d 6f76 6520  f steps to move 
+00004fc0: 706c 756e 6765 7220 6279 0d0a 2020 2020  plunger by..    
+00004fd0: 2020 2020 2020 2020 7570 2028 626f 6f6c          up (bool
+00004fe0: 293a 2077 6865 7468 6572 2074 6f20 6d6f  ): whether to mo
+00004ff0: 7665 2074 6865 2070 6c75 6e67 6572 2075  ve the plunger u
+00005000: 700d 0a0d 0a20 2020 2020 2020 2052 6574  p....        Ret
+00005010: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00005020: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+00005030: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00005040: 2022 2222 0d0a 2020 2020 2020 2020 7374   """..        st
+00005050: 6570 7320 3d20 6162 7328 7374 6570 7329  eps = abs(steps)
+00005060: 2069 6620 7570 2065 6c73 6520 2d61 6273   if up else -abs
+00005070: 2873 7465 7073 290d 0a20 2020 2020 2020  (steps)..       
+00005080: 2072 6574 7572 6e20 7365 6c66 2e6d 6f76   return self.mov
+00005090: 6542 7928 7374 6570 7329 0d0a 2020 2020  eBy(steps)..    
+000050a0: 0d0a 2020 2020 6465 6620 6d6f 7665 4279  ..    def moveBy
+000050b0: 2873 656c 662c 2073 7465 7073 3a69 6e74  (self, steps:int
+000050c0: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2073  , **kwargs) -> s
+000050d0: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+000050e0: 0d0a 2020 2020 2020 2020 4d6f 7665 2074  ..        Move t
+000050f0: 6865 2070 6c75 6e67 6572 2062 7920 7370  he plunger by sp
+00005100: 6563 6966 6965 6420 6e75 6d62 6572 206f  ecified number o
+00005110: 6620 7374 6570 730d 0a0d 0a20 2020 2020  f steps....     
+00005120: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
+00005130: 2020 2020 2020 7374 6570 7320 2869 6e74        steps (int
+00005140: 293a 206e 756d 6265 7220 6f66 2073 7465  ): number of ste
+00005150: 7073 2074 6f20 6d6f 7665 2070 6c75 6e67  ps to move plung
+00005160: 6572 2062 7920 283c 303a 206d 6f76 6520  er by (<0: move 
+00005170: 646f 776e 2f64 6973 7065 6e73 653b 203e  down/dispense; >
+00005180: 3020 6d6f 7665 2075 702f 6173 7069 7261  0 move up/aspira
+00005190: 7465 290d 0a0d 0a20 2020 2020 2020 2052  te)....        R
+000051a0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000051b0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+000051c0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+000051d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000051e0: 636f 6d6d 616e 6420 3d20 6627 5249 7b73  command = f'RI{s
+000051f0: 7465 7073 7d27 2069 6620 7374 6570 7320  teps}' if steps 
+00005200: 3e20 3020 656c 7365 2066 2752 4f7b 2d73  > 0 else f'RO{-s
+00005210: 7465 7073 7d27 0d0a 2020 2020 2020 2020  teps}'..        
+00005220: 7365 6c66 2e70 6f73 6974 696f 6e20 2b3d  self.position +=
+00005230: 2073 7465 7073 0d0a 2020 2020 2020 2020   steps..        
+00005240: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
+00005250: 7279 2863 6f6d 6d61 6e64 290d 0a20 2020  ry(command)..   
+00005260: 200d 0a20 2020 2064 6566 206d 6f76 6554   ..    def moveT
+00005270: 6f28 7365 6c66 2c20 706f 7369 7469 6f6e  o(self, position
+00005280: 3a69 6e74 2c20 2a2a 6b77 6172 6773 2920  :int, **kwargs) 
+00005290: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+000052a0: 2022 2222 0d0a 2020 2020 2020 2020 4d6f   """..        Mo
+000052b0: 7665 2074 6865 2070 6c75 6e67 6572 2074  ve the plunger t
+000052c0: 6f20 6120 7370 6563 6966 6965 6420 706f  o a specified po
+000052d0: 7369 7469 6f6e 0d0a 0d0a 2020 2020 2020  sition....      
+000052e0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+000052f0: 2020 2020 2070 6f73 6974 696f 6e20 2869       position (i
+00005300: 6e74 293a 2074 6172 6765 7420 706c 756e  nt): target plun
+00005310: 6765 7220 706f 7369 7469 6f6e 0d0a 0d0a  ger position....
+00005320: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00005330: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00005340: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
+00005350: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
+00005360: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
+00005370: 7369 7469 6f6e 203d 2070 6f73 6974 696f  sition = positio
+00005380: 6e0d 0a20 2020 2020 2020 2072 6574 7572  n..        retur
+00005390: 6e20 7365 6c66 2e5f 7175 6572 7928 6627  n self._query(f'
+000053a0: 5250 7b70 6f73 6974 696f 6e7d 2729 0d0a  RP{position}')..
+000053b0: 2020 2020 0d0a 2020 2020 6465 6620 7075      ..    def pu
+000053c0: 6c6c 6261 636b 2873 656c 662c 2073 7465  llback(self, ste
+000053d0: 7073 3a69 6e74 203d 2035 2c20 2a2a 6b77  ps:int = 5, **kw
+000053e0: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
+000053f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00005400: 2020 2020 5075 6c6c 6261 636b 206c 6971      Pullback liq
+00005410: 7569 6420 6672 6f6d 2074 6970 0d0a 2020  uid from tip..  
+00005420: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005430: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00005440: 2020 2073 7465 7073 2028 696e 742c 206f     steps (int, o
+00005450: 7074 696f 6e61 6c29 3a20 6e75 6d62 6572  ptional): number
+00005460: 206f 6620 7374 6570 7320 746f 2070 756c   of steps to pul
+00005470: 6c62 6163 6b2e 2044 6566 6175 6c74 7320  lback. Defaults 
+00005480: 746f 2035 2e0d 0a0d 0a20 2020 2020 2020  to 5.....       
+00005490: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+000054a0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
+000054b0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
+000054c0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000054d0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+000054e0: 662e 5f71 7565 7279 2866 2752 497b 7374  f._query(f'RI{st
+000054f0: 6570 737d 2729 0d0a 2020 2020 2020 2020  eps}')..        
+00005500: 7365 6c66 2e70 6f73 6974 696f 6e20 2b3d  self.position +=
+00005510: 2073 7465 7073 0d0a 2020 2020 2020 2020   steps..        
+00005520: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
+00005530: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00005540: 7370 6f6e 7365 0d0a 2020 2020 0d0a 2020  sponse..    ..  
+00005550: 2020 6465 6620 7265 7365 7428 7365 6c66    def reset(self
+00005560: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00005570: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00005580: 5265 7365 7420 7468 6520 7069 7065 7474  Reset the pipett
+00005590: 650d 0a0d 0a20 2020 2020 2020 2052 6574  e....        Ret
+000055a0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000055b0: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+000055c0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+000055d0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+000055e0: 6c66 2e7a 6572 6f28 290d 0a20 2020 2020  lf.zero()..     
+000055f0: 2020 2072 6574 7572 6e20 7365 6c66 2e68     return self.h
+00005600: 6f6d 6528 290d 0a20 2020 200d 0a20 2020  ome()..    ..   
+00005610: 2064 6566 2073 6574 5370 6565 6428 7365   def setSpeed(se
+00005620: 6c66 2c20 7370 6565 643a 696e 742c 2075  lf, speed:int, u
+00005630: 703a 626f 6f6c 2c20 6465 6661 756c 743a  p:bool, default:
+00005640: 626f 6f6c 203d 2046 616c 7365 2c20 2a2a  bool = False, **
+00005650: 6b77 6172 6773 2920 2d3e 2073 7472 3a0d  kwargs) -> str:.
+00005660: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00005670: 2020 2020 2020 5365 7420 7468 6520 7370        Set the sp
+00005680: 6565 6420 6f66 2074 6865 2070 6c75 6e67  eed of the plung
+00005690: 6572 0d0a 0d0a 2020 2020 2020 2020 4172  er....        Ar
+000056a0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+000056b0: 2073 7065 6564 2028 696e 7429 3a20 7370   speed (int): sp
+000056c0: 6565 6420 6f66 2070 6c75 6e67 6572 0d0a  eed of plunger..
+000056d0: 2020 2020 2020 2020 2020 2020 7570 2028              up (
+000056e0: 626f 6f6c 293a 2064 6972 6563 7469 6f6e  bool): direction
+000056f0: 206f 6620 7472 6176 656c 0d0a 2020 2020   of travel..    
+00005700: 2020 2020 2020 2020 6465 6661 756c 7420          default 
+00005710: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
+00005720: 3a20 7768 6574 6865 7220 746f 2073 6574  : whether to set
+00005730: 2073 7065 6564 2061 7320 6120 6465 6661   speed as a defa
+00005740: 756c 742e 2044 6566 6175 6c74 7320 746f  ult. Defaults to
+00005750: 2046 616c 7365 2e0d 0a0d 0a20 2020 2020   False.....     
+00005760: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00005770: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
+00005780: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
+00005790: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000057a0: 2020 2020 7370 6565 645f 636f 6465 203d      speed_code =
+000057b0: 2031 202b 205b 7820 666f 7220 782c 7661   1 + [x for x,va
+000057c0: 6c20 696e 2065 6e75 6d65 7261 7465 286e  l in enumerate(n
+000057d0: 702e 6172 7261 7928 7365 6c66 2e73 7065  p.array(self.spe
+000057e0: 6564 5f70 7265 7365 7473 292d 7370 6565  ed_presets)-spee
+000057f0: 6429 2069 6620 7661 6c20 3e3d 2030 5d5b  d) if val >= 0][
+00005800: 305d 0d0a 2020 2020 2020 2020 7072 696e  0]..        prin
+00005810: 7428 6627 5370 6565 6420 7b73 7065 6564  t(f'Speed {speed
+00005820: 5f63 6f64 657d 3a20 7b73 656c 662e 7370  _code}: {self.sp
+00005830: 6565 645f 7072 6573 6574 735b 7370 6565  eed_presets[spee
+00005840: 645f 636f 6465 2d31 5d7d 2075 4c2f 7327  d_code-1]} uL/s'
+00005850: 290d 0a20 2020 2020 2020 2064 6972 6563  )..        direc
+00005860: 7469 6f6e 203d 2027 4927 2069 6620 7570  tion = 'I' if up
+00005870: 2065 6c73 6520 274f 270d 0a20 2020 2020   else 'O'..     
+00005880: 2020 2073 656c 662e 5f71 7565 7279 2866     self._query(f
+00005890: 2753 7b64 6972 6563 7469 6f6e 7d7b 7370  'S{direction}{sp
+000058a0: 6565 645f 636f 6465 7d27 290d 0a20 2020  eed_code}')..   
+000058b0: 2020 2020 2069 6620 6e6f 7420 6465 6661       if not defa
+000058c0: 756c 743a 0d0a 2020 2020 2020 2020 2020  ult:..          
+000058d0: 2020 7265 7475 726e 2073 656c 662e 5f71    return self._q
+000058e0: 7565 7279 2866 2744 7b64 6972 6563 7469  uery(f'D{directi
+000058f0: 6f6e 7d27 290d 0a20 2020 2020 2020 2069  on}')..        i
+00005900: 6620 7570 3a0d 0a20 2020 2020 2020 2020  f up:..         
+00005910: 2020 2073 656c 662e 7370 6565 645f 636f     self.speed_co
+00005920: 6465 2e75 7020 3d20 7370 6565 645f 636f  de.up = speed_co
+00005930: 6465 0d0a 2020 2020 2020 2020 2020 2020  de..            
+00005940: 7365 6c66 2e73 7065 6564 2e75 7020 3d20  self.speed.up = 
+00005950: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
+00005960: 7473 5b73 7065 6564 5f63 6f64 652d 315d  ts[speed_code-1]
+00005970: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00005980: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005990: 662e 7370 6565 645f 636f 6465 2e64 6f77  f.speed_code.dow
+000059a0: 6e20 3d20 7370 6565 645f 636f 6465 0d0a  n = speed_code..
+000059b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000059c0: 2e73 7065 6564 2e64 6f77 6e20 3d20 7365  .speed.down = se
+000059d0: 6c66 2e73 7065 6564 5f70 7265 7365 7473  lf.speed_presets
+000059e0: 5b73 7065 6564 5f63 6f64 652d 315d 0d0a  [speed_code-1]..
+000059f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005a00: 656c 662e 5f71 7565 7279 2866 2744 7b64  elf._query(f'D{d
+00005a10: 6972 6563 7469 6f6e 7d27 290d 0a20 2020  irection}')..   
+00005a20: 200d 0a20 2020 2064 6566 2073 6875 7464   ..    def shutd
+00005a30: 6f77 6e28 7365 6c66 293a 0d0a 2020 2020  own(self):..    
+00005a40: 2020 2020 2222 2253 6875 7464 6f77 6e20      """Shutdown 
+00005a50: 7072 6f63 6564 7572 6520 666f 7220 746f  procedure for to
+00005a60: 6f6c 2222 220d 0a20 2020 2020 2020 2073  ol"""..        s
+00005a70: 656c 662e 746f 6767 6c65 4665 6564 6261  elf.toggleFeedba
+00005a80: 636b 4c6f 6f70 286f 6e3d 4661 6c73 6529  ckLoop(on=False)
+00005a90: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005aa0: 2073 7570 6572 2829 2e73 6875 7464 6f77   super().shutdow
+00005ab0: 6e28 290d 0a20 2020 200d 0a20 2020 2064  n()..    ..    d
+00005ac0: 6566 2074 6f67 676c 6546 6565 6462 6163  ef toggleFeedbac
+00005ad0: 6b4c 6f6f 7028 7365 6c66 2c20 6f6e 3a62  kLoop(self, on:b
+00005ae0: 6f6f 6c29 3a0d 0a20 2020 2020 2020 2022  ool):..        "
+00005af0: 2222 0d0a 2020 2020 2020 2020 5374 6172  ""..        Star
+00005b00: 7420 6f72 2073 746f 7020 6665 6564 6261  t or stop feedba
+00005b10: 636b 206c 6f6f 700d 0a20 2020 2020 2020  ck loop..       
+00005b20: 200d 0a20 2020 2020 2020 2041 7267 733a   ..        Args:
+00005b30: 0d0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
+00005b40: 2028 626f 6f6c 293a 2077 6865 7468 6572   (bool): whether
+00005b50: 2074 6f20 7374 6172 7420 6665 6564 6261   to start feedba
+00005b60: 636b 206c 6f6f 700d 0a20 2020 2020 2020  ck loop..       
+00005b70: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+00005b80: 6c66 2e73 6574 466c 6167 2867 6574 5f66  lf.setFlag(get_f
+00005b90: 6565 6462 6163 6b3d 6f6e 290d 0a20 2020  eedback=on)..   
+00005ba0: 2020 2020 2069 6620 6f6e 3a0d 0a20 2020       if on:..   
+00005bb0: 2020 2020 2020 2020 2069 6620 2766 6565           if 'fee
+00005bc0: 6462 6163 6b5f 6c6f 6f70 2720 696e 2073  dback_loop' in s
+00005bd0: 656c 662e 5f74 6872 6561 6473 3a0d 0a20  elf._threads:.. 
+00005be0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005bf0: 656c 662e 5f74 6872 6561 6473 5b27 6665  elf._threads['fe
+00005c00: 6564 6261 636b 5f6c 6f6f 7027 5d2e 6a6f  edback_loop'].jo
+00005c10: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
+00005c20: 2020 7468 7265 6164 203d 2054 6872 6561    thread = Threa
+00005c30: 6428 7461 7267 6574 3d73 656c 662e 5f6c  d(target=self._l
+00005c40: 6f6f 705f 6665 6564 6261 636b 290d 0a20  oop_feedback).. 
+00005c50: 2020 2020 2020 2020 2020 2074 6872 6561             threa
+00005c60: 642e 7374 6172 7428 290d 0a20 2020 2020  d.start()..     
+00005c70: 2020 2020 2020 2073 656c 662e 5f74 6872         self._thr
+00005c80: 6561 6473 5b27 6665 6564 6261 636b 5f6c  eads['feedback_l
+00005c90: 6f6f 7027 5d20 3d20 7468 7265 6164 0d0a  oop'] = thread..
+00005ca0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00005cb0: 2020 2020 2020 2020 2020 2069 6620 2766             if 'f
+00005cc0: 6565 6462 6163 6b5f 6c6f 6f70 2720 696e  eedback_loop' in
+00005cd0: 2073 656c 662e 5f74 6872 6561 6473 3a0d   self._threads:.
+00005ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005cf0: 2073 656c 662e 5f74 6872 6561 6473 5b27   self._threads['
+00005d00: 6665 6564 6261 636b 5f6c 6f6f 7027 5d2e  feedback_loop'].
+00005d10: 6a6f 696e 2829 0d0a 2020 2020 2020 2020  join()..        
+00005d20: 7265 7475 726e 0d0a 0d0a 2020 2020 6465  return....    de
+00005d30: 6620 7a65 726f 2873 656c 6629 202d 3e20  f zero(self) -> 
+00005d40: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
+00005d50: 220d 0a20 2020 2020 2020 205a 6572 6f20  "..        Zero 
+00005d60: 7468 6520 706c 756e 6765 7220 706f 7369  the plunger posi
+00005d70: 7469 6f6e 0d0a 2020 2020 2020 2020 0d0a  tion..        ..
+00005d80: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00005d90: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00005da0: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
+00005db0: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
+00005dc0: 0a20 2020 2020 2020 2073 656c 662e 656a  .        self.ej
+00005dd0: 6563 7428 290d 0a20 2020 2020 2020 2072  ect()..        r
+00005de0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00005df0: 7175 6572 7928 2752 5a27 290d 0a20 2020  query('RZ')..   
+00005e00: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+00005e10: 6f6e 203d 2030 0d0a 2020 2020 2020 2020  on = 0..        
+00005e20: 7469 6d65 2e73 6c65 6570 2832 290d 0a20  time.sleep(2).. 
+00005e30: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00005e40: 7370 6f6e 7365 0d0a 0d0a 2020 2020 2320  sponse....    # 
+00005e50: 5072 6f74 6563 7465 6420 6d65 7468 6f64  Protected method
+00005e60: 2873 290d 0a20 2020 2064 6566 205f 6361  (s)..    def _ca
+00005e70: 6c63 756c 6174 655f 7370 6565 645f 7061  lculate_speed_pa
+00005e80: 7261 6d65 7465 7273 2873 656c 662c 2076  rameters(self, v
+00005e90: 6f6c 756d 653a 696e 742c 2073 7065 6564  olume:int, speed
+00005ea0: 3a69 6e74 2920 2d3e 2053 7065 6564 5061  :int) -> SpeedPa
+00005eb0: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
+00005ec0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00005ed0: 4361 6c63 756c 6174 6573 2074 6865 2062  Calculates the b
+00005ee0: 6573 7420 7061 7261 6d65 7465 7273 2066  est parameters f
+00005ef0: 6f72 2076 6f6c 756d 6520 616e 6420 7370  or volume and sp
+00005f00: 6565 640d 0a0d 0a20 2020 2020 2020 2041  eed....        A
+00005f10: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00005f20: 2020 766f 6c75 6d65 2028 696e 7429 3a20    volume (int): 
+00005f30: 766f 6c75 6d65 2074 6f20 6265 2074 7261  volume to be tra
+00005f40: 6e73 6665 7272 6564 0d0a 2020 2020 2020  nsferred..      
+00005f50: 2020 2020 2020 7370 6565 6420 2869 6e74        speed (int
+00005f60: 293a 2073 7065 6564 2061 7420 7768 6963  ): speed at whic
+00005f70: 6820 6c69 7175 6964 2069 7320 7472 616e  h liquid is tran
+00005f80: 7366 6572 7265 640d 0a0d 0a20 2020 2020  sferred....     
+00005f90: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00005fa0: 2020 2020 2020 2020 2064 6963 743a 2064           dict: d
+00005fb0: 6963 7469 6f6e 6172 7920 6f66 2062 6573  ictionary of bes
+00005fc0: 7420 7061 7261 6d65 7465 7273 0d0a 2020  t parameters..  
+00005fd0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00005fe0: 2020 206f 7574 636f 6d65 7320 3d20 7b7d     outcomes = {}
+00005ff0: 0d0a 2020 2020 2020 2020 7374 6570 5f69  ..        step_i
+00006000: 6e74 6572 7661 6c5f 6c69 6d69 7420 3d20  nterval_limit = 
+00006010: 696e 7428 766f 6c75 6d65 2f73 656c 662e  int(volume/self.
+00006020: 7265 736f 6c75 7469 6f6e 2f53 5445 505f  resolution/STEP_
+00006030: 5245 534f 4c55 5449 4f4e 290d 0a20 2020  RESOLUTION)..   
+00006040: 2020 2020 2066 6f72 2070 7265 7365 7420       for preset 
+00006050: 696e 2073 656c 662e 7370 6565 645f 7072  in self.speed_pr
+00006060: 6573 6574 733a 0d0a 2020 2020 2020 2020  esets:..        
+00006070: 2020 2020 6966 2070 7265 7365 7420 3c20      if preset < 
+00006080: 7370 6565 643a 0d0a 2020 2020 2020 2020  speed:..        
+00006090: 2020 2020 2020 2020 2320 7072 6573 6574          # preset
+000060a0: 2069 7320 736c 6f77 6572 2074 6861 6e20   is slower than 
+000060b0: 7461 7267 6574 2073 7065 6564 2c20 6974  target speed, it
+000060c0: 2077 696c 6c20 6e65 7665 7220 6869 7420   will never hit 
+000060d0: 7461 7267 6574 2073 7065 6564 0d0a 2020  target speed..  
+000060e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000060f0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+00006100: 2020 2020 7469 6d65 5f69 6e74 6572 7661      time_interva
+00006110: 6c5f 6c69 6d69 7420 3d20 696e 7428 766f  l_limit = int(vo
+00006120: 6c75 6d65 2a28 312f 7370 6565 6420 2d20  lume*(1/speed - 
+00006130: 312f 7072 6573 6574 292f 7365 6c66 2e72  1/preset)/self.r
+00006140: 6573 706f 6e73 655f 7469 6d65 290d 0a20  esponse_time).. 
+00006150: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00006160: 7420 7374 6570 5f69 6e74 6572 7661 6c5f  t step_interval_
+00006170: 6c69 6d69 7420 6f72 206e 6f74 2074 696d  limit or not tim
+00006180: 655f 696e 7465 7276 616c 5f6c 696d 6974  e_interval_limit
+00006190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000061a0: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
+000061b0: 2020 2020 2020 2020 2069 6e74 6572 7661           interva
+000061c0: 6c73 203d 206d 6178 286d 696e 2873 7465  ls = max(min(ste
+000061d0: 705f 696e 7465 7276 616c 5f6c 696d 6974  p_interval_limit
+000061e0: 2c20 7469 6d65 5f69 6e74 6572 7661 6c5f  , time_interval_
+000061f0: 6c69 6d69 7429 2c20 3129 0d0a 2020 2020  limit), 1)..    
+00006200: 2020 2020 2020 2020 6561 6368 5f73 7465          each_ste
+00006210: 7073 203d 2076 6f6c 756d 652f 7365 6c66  ps = volume/self
+00006220: 2e72 6573 6f6c 7574 696f 6e2f 696e 7465  .resolution/inte
+00006230: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
+00006240: 2020 2065 6163 685f 6465 6c61 7920 3d20     each_delay = 
+00006250: 766f 6c75 6d65 2a28 312f 7370 6565 6420  volume*(1/speed 
+00006260: 2d20 312f 7072 6573 6574 292f 696e 7465  - 1/preset)/inte
+00006270: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
+00006280: 2020 2061 7265 6120 3d20 302e 3520 2a20     area = 0.5 * 
+00006290: 2876 6f6c 756d 652a 2a32 2920 2a20 2831  (volume**2) * (1
+000062a0: 2f73 656c 662e 7265 736f 6c75 7469 6f6e  /self.resolution
+000062b0: 2920 2a20 2831 2f69 6e74 6572 7661 6c73  ) * (1/intervals
+000062c0: 2920 2a20 2831 2f73 7065 6564 202d 2031  ) * (1/speed - 1
+000062d0: 2f70 7265 7365 7429 0d0a 2020 2020 2020  /preset)..      
+000062e0: 2020 2020 2020 6f75 7463 6f6d 6573 5b61        outcomes[a
+000062f0: 7265 615d 203d 2053 7065 6564 5061 7261  rea] = SpeedPara
+00006300: 6d65 7465 7273 2870 7265 7365 742c 2069  meters(preset, i
+00006310: 6e74 6572 7661 6c73 2c20 696e 7428 6561  ntervals, int(ea
+00006320: 6368 5f73 7465 7073 292c 2065 6163 685f  ch_steps), each_
+00006330: 6465 6c61 7929 0d0a 2020 2020 2020 2020  delay)..        
+00006340: 6966 206c 656e 286f 7574 636f 6d65 7329  if len(outcomes)
+00006350: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00006360: 2020 2020 7072 696e 7428 224e 6f20 6665      print("No fe
+00006370: 6173 6962 6c65 2073 7065 6564 2070 6172  asible speed par
+00006380: 616d 6574 6572 732e 2229 0d0a 2020 2020  ameters.")..    
+00006390: 2020 2020 2020 2020 7265 7475 726e 2053          return S
+000063a0: 7065 6564 5061 7261 6d65 7465 7273 284e  peedParameters(N
+000063b0: 6f6e 652c 2053 5445 505f 5245 534f 4c55  one, STEP_RESOLU
+000063c0: 5449 4f4e 2c20 5354 4550 5f52 4553 4f4c  TION, STEP_RESOL
+000063d0: 5554 494f 4e2c 2073 656c 662e 7265 7370  UTION, self.resp
+000063e0: 6f6e 7365 5f74 696d 6529 0d0a 2020 2020  onse_time)..    
+000063f0: 2020 2020 7072 696e 7428 6627 4265 7374      print(f'Best
+00006400: 2070 6172 616d 6574 6572 733a 207b 6f75   parameters: {ou
+00006410: 7463 6f6d 6573 5b6d 696e 286f 7574 636f  tcomes[min(outco
+00006420: 6d65 7329 5d7d 2729 0d0a 2020 2020 2020  mes)]}')..      
+00006430: 2020 7265 7475 726e 206f 7574 636f 6d65    return outcome
+00006440: 735b 6d69 6e28 6f75 7463 6f6d 6573 295d  s[min(outcomes)]
+00006450: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00006460: 5f63 6f6e 6e65 6374 2873 656c 662c 2070  _connect(self, p
+00006470: 6f72 743a 7374 722c 2062 6175 6472 6174  ort:str, baudrat
+00006480: 653a 696e 7420 3d20 3936 3030 2c20 7469  e:int = 9600, ti
+00006490: 6d65 6f75 743a 696e 7420 3d20 3129 3a0d  meout:int = 1):.
+000064a0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000064b0: 2020 2020 2020 436f 6e6e 6563 7469 6f6e        Connection
+000064c0: 2070 726f 6365 6475 7265 2066 6f72 2074   procedure for t
+000064d0: 6f6f 6c0d 0a0d 0a20 2020 2020 2020 2041  ool....        A
+000064e0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+000064f0: 2020 706f 7274 2028 7374 7229 3a20 434f    port (str): CO
+00006500: 4d20 706f 7274 2061 6464 7265 7373 0d0a  M port address..
+00006510: 2020 2020 2020 2020 2020 2020 6261 7564              baud
+00006520: 7261 7465 2028 696e 742c 206f 7074 696f  rate (int, optio
+00006530: 6e61 6c29 3a20 6261 7564 7261 7465 2e20  nal): baudrate. 
+00006540: 4465 6661 756c 7473 2074 6f20 3936 3030  Defaults to 9600
+00006550: 2e0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+00006560: 696d 656f 7574 2028 696e 742c 206f 7074  imeout (int, opt
+00006570: 696f 6e61 6c29 3a20 7469 6d65 6f75 7420  ional): timeout 
+00006580: 696e 2073 6563 6f6e 6473 2e20 4465 6661  in seconds. Defa
+00006590: 756c 7473 2074 6f20 312e 0d0a 2020 2020  ults to 1...    
+000065a0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000065b0: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
+000065c0: 5f64 6574 6169 6c73 203d 207b 0d0a 2020  _details = {..  
+000065d0: 2020 2020 2020 2020 2020 2770 6f72 7427            'port'
+000065e0: 3a20 706f 7274 2c0d 0a20 2020 2020 2020  : port,..       
+000065f0: 2020 2020 2027 6261 7564 7261 7465 273a       'baudrate':
+00006600: 2062 6175 6472 6174 652c 0d0a 2020 2020   baudrate,..    
+00006610: 2020 2020 2020 2020 2774 696d 656f 7574          'timeout
+00006620: 273a 2074 696d 656f 7574 0d0a 2020 2020  ': timeout..    
+00006630: 2020 2020 7d0d 0a20 2020 2020 2020 2064      }..        d
+00006640: 6576 6963 6520 3d20 4e6f 6e65 0d0a 2020  evice = None..  
+00006650: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00006660: 2020 2020 2020 2020 6465 7669 6365 203d          device =
+00006670: 2073 6572 6961 6c2e 5365 7269 616c 2870   serial.Serial(p
+00006680: 6f72 742c 2062 6175 6472 6174 652c 2074  ort, baudrate, t
+00006690: 696d 656f 7574 3d74 696d 656f 7574 290d  imeout=timeout).
+000066a0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000066b0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+000066c0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000066d0: 6e74 2866 2243 6f75 6c64 206e 6f74 2063  nt(f"Could not c
+000066e0: 6f6e 6e65 6374 2074 6f20 7b70 6f72 747d  onnect to {port}
+000066f0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00006700: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
+00006710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006720: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
+00006730: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00006740: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00006750: 7028 3229 2020 2023 2057 6169 7420 666f  p(2)   # Wait fo
+00006760: 7220 6772 626c 2074 6f20 696e 6974 6961  r grbl to initia
+00006770: 6c69 7a65 0d0a 2020 2020 2020 2020 2020  lize..          
+00006780: 2020 6465 7669 6365 2e66 6c75 7368 496e    device.flushIn
+00006790: 7075 7428 290d 0a20 2020 2020 2020 2020  put()..         
+000067a0: 2020 2070 7269 6e74 2866 2243 6f6e 6e65     print(f"Conne
+000067b0: 6374 696f 6e20 6f70 656e 6564 2074 6f20  ction opened to 
+000067c0: 7b70 6f72 747d 2229 0d0a 2020 2020 2020  {port}")..      
+000067d0: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
+000067e0: 6167 2863 6f6e 6e65 6374 6564 3d54 7275  ag(connected=Tru
+000067f0: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00006800: 2e64 6576 6963 6520 3d20 6465 7669 6365  .device = device
+00006810: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00006820: 6574 496e 666f 2829 0d0a 2020 2020 2020  etInfo()..      
+00006830: 2020 7365 6c66 2e72 6573 6574 2829 0d0a    self.reset()..
+00006840: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00006850: 2020 2020 0d0a 2020 2020 6465 6620 5f69      ..    def _i
+00006860: 735f 6578 7065 6374 6564 5f72 6570 6c79  s_expected_reply
+00006870: 2873 656c 662c 2072 6573 706f 6e73 653a  (self, response:
+00006880: 7374 722c 2063 6f6d 6d61 6e64 5f63 6f64  str, command_cod
+00006890: 653a 7374 722c 202a 2a6b 7761 7267 7329  e:str, **kwargs)
+000068a0: 202d 3e20 626f 6f6c 3a0d 0a20 2020 2020   -> bool:..     
+000068b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000068c0: 4368 6563 6b73 2061 6e64 2072 6574 7572  Checks and retur
+000068d0: 6e73 2077 6865 7468 6572 2074 6865 2072  ns whether the r
+000068e0: 6573 706f 6e73 6520 6973 2061 6e20 6578  esponse is an ex
+000068f0: 7065 6374 6564 2072 6570 6c79 0d0a 0d0a  pected reply....
+00006900: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+00006910: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+00006920: 6e73 6520 2873 7472 293a 2072 6573 706f  nse (str): respo
+00006930: 6e73 6520 7374 7269 6e67 2066 726f 6d20  nse string from 
+00006940: 6465 7669 6365 0d0a 2020 2020 2020 2020  device..        
+00006950: 2020 2020 636f 6d6d 616e 645f 636f 6465      command_code
+00006960: 2028 7374 7229 3a20 7477 6f2d 6368 6172   (str): two-char
+00006970: 6163 7465 7220 636f 6d6d 616e 6420 636f  acter command co
+00006980: 6465 0d0a 0d0a 2020 2020 2020 2020 5265  de....        Re
+00006990: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+000069a0: 2020 2020 626f 6f6c 3a20 7768 6574 6865      bool: whethe
+000069b0: 7220 7468 6520 7265 7370 6f6e 7365 2069  r the response i
+000069c0: 7320 616e 2065 7870 6563 7465 6420 7265  s an expected re
+000069d0: 706c 790d 0a20 2020 2020 2020 2022 2222  ply..        """
+000069e0: 0d0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
+000069f0: 706f 6e73 6520 696e 2045 7272 6f72 436f  ponse in ErrorCo
+00006a00: 6465 2e5f 6d65 6d62 6572 5f6e 616d 6573  de._member_names
+00006a10: 5f3a 0d0a 2020 2020 2020 2020 2020 2020  _:..            
+00006a20: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00006a30: 2020 2020 2069 6620 636f 6d6d 616e 645f       if command_
+00006a40: 636f 6465 206e 6f74 2069 6e20 5155 4552  code not in QUER
+00006a50: 4945 5320 616e 6420 7265 7370 6f6e 7365  IES and response
+00006a60: 203d 3d20 276f 6b27 3a0d 0a20 2020 2020   == 'ok':..     
+00006a70: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00006a80: 7565 0d0a 2020 2020 2020 2020 6966 2063  ue..        if c
+00006a90: 6f6d 6d61 6e64 5f63 6f64 6520 696e 2051  ommand_code in Q
+00006aa0: 5545 5249 4553 2061 6e64 2072 6573 706f  UERIES and respo
+00006ab0: 6e73 655b 3a32 5d20 3d3d 2063 6f6d 6d61  nse[:2] == comma
+00006ac0: 6e64 5f63 6f64 652e 6c6f 7765 7228 293a  nd_code.lower():
+00006ad0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006ae0: 706c 795f 636f 6465 2c20 6461 7461 203d  ply_code, data =
+00006af0: 2072 6573 706f 6e73 655b 3a32 5d2c 2072   response[:2], r
+00006b00: 6573 706f 6e73 655b 323a 5d0d 0a20 2020  esponse[2:]..   
+00006b10: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00006b20: 2e76 6572 626f 7365 3a0d 0a20 2020 2020  .verbose:..     
+00006b30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00006b40: 2866 275b 7b72 6570 6c79 5f63 6f64 657d  (f'[{reply_code}
+00006b50: 5d20 7b64 6174 617d 2729 0d0a 2020 2020  ] {data}')..    
+00006b60: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00006b70: 7275 650d 0a20 2020 2020 2020 2072 6574  rue..        ret
+00006b80: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
+00006b90: 2064 6566 205f 6c6f 6f70 5f66 6565 6462   def _loop_feedb
+00006ba0: 6163 6b28 7365 6c66 293a 0d0a 2020 2020  ack(self):..    
+00006bb0: 2020 2020 2222 224c 6f6f 7020 746f 2063      """Loop to c
+00006bc0: 6f6e 7374 616e 746c 7920 7265 6164 2066  onstantly read f
+00006bd0: 726f 6d20 6465 7669 6365 2222 220d 0a20  rom device""".. 
+00006be0: 2020 2020 2020 2070 7269 6e74 2827 4c69         print('Li
+00006bf0: 7374 656e 696e 672e 2e2e 2729 0d0a 2020  stening...')..  
+00006c00: 2020 2020 2020 7768 696c 6520 7365 6c66        while self
+00006c10: 2e66 6c61 6773 5b27 6765 745f 6665 6564  .flags['get_feed
+00006c20: 6261 636b 275d 3a0d 0a20 2020 2020 2020  back']:..       
+00006c30: 2020 2020 2069 6620 7365 6c66 2e66 6c61       if self.fla
+00006c40: 6773 5b27 7061 7573 655f 6665 6564 6261  gs['pause_feedba
+00006c50: 636b 275d 3a0d 0a20 2020 2020 2020 2020  ck']:..         
+00006c60: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00006c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006c80: 662e 6765 7453 7461 7475 7328 290d 0a20  f.getStatus().. 
+00006c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006ca0: 6765 7443 6170 6163 6974 616e 6365 2829  getCapacitance()
+00006cb0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00006cc0: 2753 746f 7020 6c69 7374 656e 696e 672e  'Stop listening.
+00006cd0: 2e2e 2729 0d0a 2020 2020 2020 2020 7265  ..')..        re
+00006ce0: 7475 726e 0d0a 2020 2020 0d0a 2020 2020  turn..    ..    
+00006cf0: 6465 6620 5f71 7565 7279 2873 656c 662c  def _query(self,
+00006d00: 200d 0a20 2020 2020 2020 2063 6f6d 6d61   ..        comma
+00006d10: 6e64 3a20 7374 722c 200d 0a20 2020 2020  nd: str, ..     
+00006d20: 2020 2074 696d 656f 7574 5f73 3a20 666c     timeout_s: fl
+00006d30: 6f61 7420 3d20 302e 332c 200d 0a20 2020  oat = 0.3, ..   
+00006d40: 2020 2020 2072 6573 756d 655f 6665 6564       resume_feed
+00006d50: 6261 636b 3a20 626f 6f6c 203d 2046 616c  back: bool = Fal
+00006d60: 7365 2c0d 0a20 2020 2020 2020 2067 6574  se,..        get
+00006d70: 5f70 6f73 6974 696f 6e3a 2062 6f6f 6c20  _position: bool 
+00006d80: 3d20 5472 7565 0d0a 2020 2020 2920 2d3e  = True..    ) ->
+00006d90: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
+00006da0: 2222 0d0a 2020 2020 2020 2020 5772 6974  ""..        Writ
+00006db0: 6520 636f 6d6d 616e 6420 746f 2061 6e64  e command to and
+00006dc0: 2072 6561 6420 7265 7370 6f6e 7365 2066   read response f
+00006dd0: 726f 6d20 6465 7669 6365 0d0a 0d0a 2020  rom device....  
+00006de0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00006df0: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
+00006e00: 2028 7374 7229 3a20 636f 6d6d 616e 6420   (str): command 
+00006e10: 7374 7269 6e67 0d0a 2020 2020 2020 2020  string..        
+00006e20: 2020 2020 7469 6d65 6f75 745f 7320 2866      timeout_s (f
+00006e30: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
+00006e40: 2064 7572 6174 696f 6e20 746f 2077 6169   duration to wai
+00006e50: 7420 6265 666f 7265 2074 696d 656f 7574  t before timeout
+00006e60: 2e20 4465 6661 756c 7473 2074 6f20 302e  . Defaults to 0.
+00006e70: 332e 0d0a 2020 2020 2020 2020 2020 2020  3...            
+00006e80: 7265 7375 6d65 5f66 6565 6462 6163 6b20  resume_feedback 
+00006e90: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
+00006ea0: 3a20 7768 6574 6865 7220 746f 2072 6573  : whether to res
+00006eb0: 756d 6520 7265 6164 696e 6720 6672 6f6d  ume reading from
+00006ec0: 2064 6576 6963 652e 2044 6566 6175 6c74   device. Default
+00006ed0: 7320 746f 2046 616c 7365 2e0d 0a20 2020  s to False...   
+00006ee0: 2020 2020 2020 2020 2067 6574 5f70 6f73           get_pos
+00006ef0: 6974 696f 6e20 2862 6f6f 6c2c 206f 7074  ition (bool, opt
+00006f00: 696f 6e61 6c29 3a20 7768 6574 6865 7220  ional): whether 
+00006f10: 746f 2067 6574 2074 6865 2070 6f73 6974  to get the posit
+00006f20: 696f 6e20 6f66 2074 6865 2070 6c75 6e67  ion of the plung
+00006f30: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
+00006f40: 5472 7565 2e0d 0a20 2020 2020 2020 2052  True...        R
+00006f50: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00006f60: 2020 2020 2073 7472 3a20 7265 7370 6f6e       str: respon
+00006f70: 7365 2073 7472 696e 670d 0a20 2020 2020  se string..     
+00006f80: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00006f90: 636f 6d6d 616e 645f 636f 6465 203d 2063  command_code = c
+00006fa0: 6f6d 6d61 6e64 5b3a 325d 0d0a 2020 2020  ommand[:2]..    
+00006fb0: 2020 2020 6966 2063 6f6d 6d61 6e64 5f63      if command_c
+00006fc0: 6f64 6520 6e6f 7420 696e 2053 5441 5455  ode not in STATU
+00006fd0: 535f 5155 4552 4945 533a 0d0a 2020 2020  S_QUERIES:..    
+00006fe0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006ff0: 666c 6167 735b 2767 6574 5f66 6565 6462  flags['get_feedb
+00007000: 6163 6b27 5d20 616e 6420 6e6f 7420 7365  ack'] and not se
+00007010: 6c66 2e66 6c61 6773 5b27 7061 7573 655f  lf.flags['pause_
+00007020: 6665 6564 6261 636b 275d 3a0d 0a20 2020  feedback']:..   
+00007030: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007040: 662e 7365 7446 6c61 6728 7061 7573 655f  f.setFlag(pause_
+00007050: 6665 6564 6261 636b 3d54 7275 6529 0d0a  feedback=True)..
+00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007070: 7469 6d65 2e73 6c65 6570 2874 696d 656f  time.sleep(timeo
+00007080: 7574 5f73 290d 0a20 2020 2020 2020 2020  ut_s)..         
+00007090: 2020 2023 2073 656c 662e 6765 7453 7461     # self.getSta
+000070a0: 7475 7328 290d 0a20 2020 2020 2020 2020  tus()..         
+000070b0: 2020 2023 2077 6869 6c65 2073 656c 662e     # while self.
+000070c0: 6973 4275 7379 2829 3a0d 0a20 2020 2020  isBusy():..     
+000070d0: 2020 2020 2020 2023 2020 2020 2073 656c         #     sel
+000070e0: 662e 6765 7453 7461 7475 7328 290d 0a20  f.getStatus().. 
+000070f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00007100: 6c66 2e69 7342 7573 7928 293a 0d0a 2020  lf.isBusy():..  
+00007110: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00007120: 6d65 2e73 6c65 6570 2874 696d 656f 7574  me.sleep(timeout
+00007130: 5f73 290d 0a20 2020 2020 2020 200d 0a20  _s)..        .. 
+00007140: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
+00007150: 6520 3d20 7469 6d65 2e70 6572 665f 636f  e = time.perf_co
+00007160: 756e 7465 7228 290d 0a20 2020 2020 2020  unter()..       
+00007170: 2073 656c 662e 5f77 7269 7465 2863 6f6d   self._write(com
+00007180: 6d61 6e64 290d 0a20 2020 2020 2020 2072  mand)..        r
+00007190: 6573 706f 6e73 6520 3d20 2727 0d0a 2020  esponse = ''..  
+000071a0: 2020 2020 2020 7768 696c 6520 6e6f 7420        while not 
+000071b0: 7365 6c66 2e5f 6973 5f65 7870 6563 7465  self._is_expecte
+000071c0: 645f 7265 706c 7928 7265 7370 6f6e 7365  d_reply(response
+000071d0: 2c20 636f 6d6d 616e 645f 636f 6465 293a  , command_code):
+000071e0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000071f0: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
+00007200: 6572 2829 202d 2073 7461 7274 5f74 696d  er() - start_tim
+00007210: 6520 3e20 7469 6d65 6f75 745f 733a 0d0a  e > timeout_s:..
+00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007230: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00007240: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00007250: 6c66 2e5f 7265 6164 2829 0d0a 2020 2020  lf._read()..    
+00007260: 2020 2020 2320 7072 696e 7428 7469 6d65      # print(time
+00007270: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
+00007280: 2d20 7374 6172 745f 7469 6d65 290d 0a20  - start_time).. 
+00007290: 2020 2020 2020 2069 6620 636f 6d6d 616e         if comman
+000072a0: 645f 636f 6465 2069 6e20 5155 4552 4945  d_code in QUERIE
+000072b0: 533a 0d0a 2020 2020 2020 2020 2020 2020  S:..            
+000072c0: 7265 7370 6f6e 7365 203d 2072 6573 706f  response = respo
+000072d0: 6e73 655b 323a 5d0d 0a20 2020 2020 2020  nse[2:]..       
+000072e0: 2069 6620 636f 6d6d 616e 645f 636f 6465   if command_code
+000072f0: 206e 6f74 2069 6e20 5354 4154 5553 5f51   not in STATUS_Q
+00007300: 5545 5249 4553 3a0d 0a20 2020 2020 2020  UERIES:..       
+00007310: 2020 2020 2069 6620 6765 745f 706f 7369       if get_posi
+00007320: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
+00007330: 2020 2020 2020 2073 656c 662e 6765 7450         self.getP
+00007340: 6f73 6974 696f 6e28 290d 0a20 2020 2020  osition()..     
+00007350: 2020 2020 2020 2069 6620 7265 7375 6d65         if resume
+00007360: 5f66 6565 6462 6163 6b3a 0d0a 2020 2020  _feedback:..    
+00007370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007380: 2e73 6574 466c 6167 2870 6175 7365 5f66  .setFlag(pause_f
+00007390: 6565 6462 6163 6b3d 4661 6c73 6529 0d0a  eedback=False)..
+000073a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000073b0: 6573 706f 6e73 650d 0a0d 0a20 2020 2064  esponse....    d
+000073c0: 6566 205f 7265 6164 2873 656c 6629 202d  ef _read(self) -
+000073d0: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
+000073e0: 2222 220d 0a20 2020 2020 2020 2052 6561  """..        Rea
+000073f0: 6420 7265 7370 6f6e 7365 2066 726f 6d20  d response from 
+00007400: 6465 7669 6365 0d0a 0d0a 2020 2020 2020  device....      
+00007410: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00007420: 2020 2020 2020 2020 7374 723a 2072 6573          str: res
+00007430: 706f 6e73 6520 7374 7269 6e67 0d0a 2020  ponse string..  
+00007440: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00007450: 2020 2072 6573 706f 6e73 6520 3d20 2727     response = ''
+00007460: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00007470: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00007480: 6f6e 7365 203d 2073 656c 662e 6465 7669  onse = self.devi
+00007490: 6365 2e72 6561 646c 696e 6528 290d 0a20  ce.readline().. 
+000074a0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+000074b0: 6e28 7265 7370 6f6e 7365 2920 3d3d 2030  n(response) == 0
+000074c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000074d0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+000074e0: 6c66 2e64 6576 6963 652e 7265 6164 6c69  lf.device.readli
+000074f0: 6e65 2829 0d0a 2020 2020 2020 2020 2020  ne()..          
+00007500: 2020 7265 7370 6f6e 7365 203d 2072 6573    response = res
+00007510: 706f 6e73 655b 323a 2d32 5d2e 6465 636f  ponse[2:-2].deco
+00007520: 6465 2827 7574 662d 3827 290d 0a20 2020  de('utf-8')..   
+00007530: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
+00007540: 6962 7574 6545 7272 6f72 3a0d 0a20 2020  ibuteError:..   
+00007550: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+00007560: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00007570: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00007580: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00007590: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
+000075a0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000075b0: 6e74 2865 290d 0a20 2020 2020 2020 2069  nt(e)..        i
+000075c0: 6620 7265 7370 6f6e 7365 2069 6e20 4572  f response in Er
+000075d0: 726f 7243 6f64 652e 5f6d 656d 6265 725f  rorCode._member_
+000075e0: 6e61 6d65 735f 3a0d 0a20 2020 2020 2020  names_:..       
+000075f0: 2020 2020 2070 7269 6e74 2845 7272 6f72       print(Error
+00007600: 436f 6465 5b72 6573 706f 6e73 655d 2e76  Code[response].v
+00007610: 616c 7565 290d 0a20 2020 2020 2020 2072  alue)..        r
+00007620: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00007630: 2020 2020 0d0a 2020 2020 6465 6620 5f73      ..    def _s
+00007640: 6574 5f63 6861 6e6e 656c 5f69 6428 7365  et_channel_id(se
+00007650: 6c66 2c20 6e65 775f 6368 616e 6e65 6c5f  lf, new_channel_
+00007660: 6964 3a69 6e74 293a 0d0a 2020 2020 2020  id:int):..      
+00007670: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
+00007680: 6574 2063 6861 6e6e 656c 2069 6420 6f66  et channel id of
+00007690: 2064 6576 6963 650d 0a0d 0a20 2020 2020   device....     
+000076a0: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
+000076b0: 2020 2020 2020 6e65 775f 6368 616e 6e65        new_channe
+000076c0: 6c20 2869 6e74 293a 206e 6577 2063 6861  l (int): new cha
+000076d0: 6e6e 656c 2069 640d 0a0d 0a20 2020 2020  nnel id....     
+000076e0: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
+000076f0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+00007700: 6f72 3a20 506c 6561 7365 2073 656c 6563  or: Please selec
+00007710: 7420 6120 7661 6c69 6420 724c 696e 6520  t a valid rLine 
+00007720: 6164 6472 6573 7320 6672 6f6d 2031 2074  address from 1 t
+00007730: 6f20 390d 0a20 2020 2020 2020 2022 2222  o 9..        """
+00007740: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00007750: 2028 3020 3c20 6e65 775f 6368 616e 6e65   (0 < new_channe
+00007760: 6c5f 6964 203c 2031 3029 3a0d 0a20 2020  l_id < 10):..   
+00007770: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00007780: 616c 7565 4572 726f 7228 2750 6c65 6173  alueError('Pleas
+00007790: 6520 7365 6c65 6374 2061 2076 616c 6964  e select a valid
+000077a0: 2072 4c69 6e65 2061 6464 7265 7373 2066   rLine address f
+000077b0: 726f 6d20 3120 746f 2039 2e27 290d 0a20  rom 1 to 9.').. 
+000077c0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000077d0: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
+000077e0: 2a41 7b6e 6577 5f63 6861 6e6e 656c 5f69  *A{new_channel_i
+000077f0: 647d 2729 0d0a 2020 2020 2020 2020 6966  d}')..        if
+00007800: 2072 6573 706f 6e73 6520 3d3d 2027 6f6b   response == 'ok
+00007810: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+00007820: 7365 6c66 2e63 6861 6e6e 656c 203d 206e  self.channel = n
+00007830: 6577 5f63 6861 6e6e 656c 5f69 640d 0a20  ew_channel_id.. 
+00007840: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
+00007850: 2020 200d 0a20 2020 2064 6566 205f 7772     ..    def _wr
+00007860: 6974 6528 7365 6c66 2c20 636f 6d6d 616e  ite(self, comman
+00007870: 643a 7374 7229 202d 3e20 626f 6f6c 3a0d  d:str) -> bool:.
+00007880: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00007890: 2020 2020 2020 5772 6974 6520 636f 6d6d        Write comm
+000078a0: 616e 6420 746f 2064 6576 6963 650d 0a0d  and to device...
+000078b0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+000078c0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+000078d0: 616e 6420 2873 7472 293a 203c 636f 6d6d  and (str): <comm
+000078e0: 616e 6420 636f 6465 3e3c 7661 6c75 653e  and code><value>
+000078f0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00007900: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+00007910: 2020 626f 6f6c 3a20 7768 6574 6865 7220    bool: whether 
+00007920: 636f 6d6d 616e 6420 7761 7320 7365 6e74  command was sent
+00007930: 2073 7563 6365 7373 6675 6c6c 790d 0a20   successfully.. 
+00007940: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00007950: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
+00007960: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
+00007970: 2020 7072 696e 7428 636f 6d6d 616e 6429    print(command)
+00007980: 0d0a 2020 2020 2020 2020 6673 7472 696e  ..        fstrin
+00007990: 6720 3d20 6627 017b 7365 6c66 2e63 6861  g = f'.{self.cha
+000079a0: 6e6e 656c 7d7b 636f 6d6d 616e 647d c2ba  nnel}{command}..
+000079b0: 5c72 2720 2320 636f 6d6d 616e 6420 7465  \r' # command te
+000079c0: 6d70 6c61 7465 3a20 3c50 5245 3e3c 4144  mplate: <PRE><AD
+000079d0: 523e 3c43 4f44 453e 3c44 4154 413e 3c4c  R><CODE><DATA><L
+000079e0: 5243 3e3c 504f 5354 3e0d 0a20 2020 2020  RC><POST>..     
+000079f0: 2020 2023 2062 7374 7269 6e67 203d 2062     # bstring = b
+00007a00: 7974 6561 7272 6179 2e66 726f 6d68 6578  ytearray.fromhex
+00007a10: 2866 7374 7269 6e67 2e65 6e63 6f64 6528  (fstring.encode(
+00007a20: 2775 7466 2d38 2729 2e68 6578 2829 290d  'utf-8').hex()).
+00007a30: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00007a40: 2020 2020 2020 2020 2020 2023 2054 7970             # Typ
+00007a50: 6963 616c 2074 696d 656f 7574 2077 6169  ical timeout wai
+00007a60: 7420 6973 2034 3030 6d73 0d0a 2020 2020  t is 400ms..    
+00007a70: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
+00007a80: 6963 652e 7772 6974 6528 6673 7472 696e  ice.write(fstrin
+00007a90: 672e 656e 636f 6465 2827 7574 662d 3827  g.encode('utf-8'
+00007aa0: 2929 0d0a 2020 2020 2020 2020 6578 6365  ))..        exce
+00007ab0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
+00007ac0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00007ad0: 7061 7373 0d0a 2020 2020 2020 2020 6578  pass..        ex
+00007ae0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+00007af0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
+00007b00: 2020 6966 2073 656c 662e 7665 7262 6f73    if self.verbos
+00007b10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00007b20: 2020 2020 7072 696e 7428 6529 0d0a 2020      print(e)..  
+00007b30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007b40: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00007b50: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00007b60: 20
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             reagent (Optional[str], optional): name of reagent. Defaults to None.
             channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
 
         Returns:
             bool: whether the action is successful
         """
         success = []
-        for _ in range(cycles):
+        for _ in range(int(cycles)):
             ret1 = self.aspirate(volume=volume, speed=speed, wait=wait, pause=False, reagent=reagent, channel=channel)
             ret2 = self.dispense(volume=volume, speed=speed, wait=wait, pause=False, force_dispense=True, channel=channel)
             success.extend([ret1,ret2])
         return all(success)
     
     def disconnect(self):
         """Disconnect from device"""
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,153 +26,165 @@
     """
     Abstract Base Class (ABC) for Dobot Gripper objects.
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
 
     ### Constructor
     Args:
         `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-        `channel` (int, optional): digital I/O channel. Defaults to 1.
+        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
     
     ### Attributes
     - `dashboard` (Callable): connection to status and signal control
     
+    ### Properties
+    - `channel_map` (dict): mapping of digital I/O channel(s)
+    - `implement_offset` (np.ndarray): offset from attachment site to tooltip
+    
     ### Methods
     #### Abstract
     - `drop`: releases an object
     - `grab`: picks up an object
     #### Public
     - `setDashboard`: set the dashboard object
     """
     
     _implement_offset: tuple[float] = (0,0,0)
-    def __init__(self, dashboard:Optional[Callable] = None, channel:int = 1):
+    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
         """
         Instantiate the class
 
         Args:
             dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-            channel (int, optional): digital I/O channel. Defaults to 1.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         """
         self.dashboard = None
-        self._channel = 0
-        self.setDashboard(dashboard=dashboard, channel=channel)
+        self._channel_map = {}
+        self.setDashboard(dashboard=dashboard, channel_map=channel_map)
         return
     
     # Properties
     @property
-    def channel(self) -> int:
-        return self._channel
-    @channel.setter
-    def channel(self, value:int):
-        if 1<= value <= 24:
-            self._channel = value
+    def channel_map(self) -> dict:
+        return self._channel_map
+    @channel_map.setter
+    def channel_map(self, value:dict):
+        if value is None:
+            self._channel_map = {}
+            return
+        if all([(1<= v <=24) for v in value.values()]):
+            self._channel_map = value
         else:
-            raise ValueError("Please provide a valid channel id from 1 to 24.")
+            raise ValueError("Please provide valid channel ids from 1 to 24.")
         return
+    
     @property
     def implement_offset(self) -> np.ndarray:
         return np.array(self._implement_offset)
     
-    def setDashboard(self, dashboard:Callable, channel:int = 1):
+    def setDashboard(self, dashboard:Callable, channel_map:Optional[dict] = None):
         """
         Set the dashboard object
 
         Args:
             dashboard (Callable): connection to status and signal control
-            channel (int, optional): digital I/O channel. Defaults to 1.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         """
         self.dashboard = dashboard
-        self.channel= channel
+        self.channel_map = channel_map
         return
     
     
 class TwoJawGrip(DobotGripper):
     """
-    TwoJawGrip provides methods to operate the Dobot jaw gripper
+    TwoJawGrip provides methods to operate the Dobot jaw gripper.
+    Channel map labels: `grab`
     
     ### Constructor
     Args:
         `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-        `channel` (int, optional): digital I/O channel. Defaults to 1.
+        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         
     ### Methods
     - `drop`: releases an object by opening the gripper
     - `grab`: picks up an object by closing the gripper
     """
     
     _implement_offset = (0,0,-95)
-    def __init__(self, dashboard:Optional[Callable] = None, channel:int = 1):
+    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
         """
         Instantiate the class
 
         Args:
             dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-            channel (int, optional): digital I/O channel. Defaults to 1.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         """
-        super().__init__(dashboard=dashboard, channel=channel)
+        super().__init__(dashboard=dashboard, channel_map=channel_map)
         return
 
     def drop(self) -> bool:
         """
         Releases an object by opening the gripper
         
         Returns:
             bool: whether action is successful
         """
+        channel = self.channel_map.get("grab", 1)
         try:
-            self.dashboard.DOExecute(1,1)
+            self.dashboard.DOExecute(channel, 1)
         except (AttributeError, OSError):
             print('Tried to drop...')
             print("Not connected to arm.")
             return False
         return True
     
     def grab(self) -> bool:
         """
         Picks up an object by closing the gripper
         
         Returns:
             bool: whether action is successful
         """
+        channel = self.channel_map.get("grab", 1)
         try:
-            self.dashboard.DOExecute(1,0)
+            self.dashboard.DOExecute(channel, 0)
         except (AttributeError, OSError):
             print('Tried to grab...')
             print("Not connected to arm.")
             return False
         return True
 
 
 class VacuumGrip(DobotGripper):
     """
-    VacuumGrip provides methods to operate the Dobot vacuum grip
+    VacuumGrip provides methods to operate the Dobot vacuum grip.
+    Channel map labels: `pull`, `push`
     
     ### Constructor
     Args:
         `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-        `channel` (int, optional): digital I/O channel. Defaults to 1.
+        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         
     ### Methods
     - `drop`: releases an object by pushing out air
     - `grab`: picks up an object by pulling in air
     - `pull`: activate pump to suck in air
     - `push`: activate pump to blow out air
     - `stop`: stop airflow
     """
     
     _implement_offset = (0,0,-60)
-    def __init__(self, dashboard:Optional[Callable] = None, channel:int = 1):
+    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
         """
         Instantiate the class
 
         Args:
             dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-            channel (int, optional): digital I/O channel. Defaults to 1.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         """
-        super().__init__(dashboard=dashboard, channel=channel)
+        super().__init__(dashboard=dashboard, channel_map=channel_map)
         return
 
     def drop(self) -> bool:
         """
         Releases an object by pushing out air
         
         Returns:
@@ -197,60 +209,63 @@
         
         Args:
             duration (Optional[int], optional): number of seconds to pull air. Defaults to None.
         
         Returns:
             bool: whether action is successful
         """
+        channel = self.channel_map.get("pull", 1)
         try:
-            self.dashboard.DOExecute(1,1)
+            self.dashboard.DOExecute(channel, 1)
         except (AttributeError, OSError):
             print('Tried to pull...')
             print("Not connected to arm.")
             return False
         else:
             if duration is not None:
                 time.sleep(duration)
-                self.dashboard.DOExecute(1,0)
+                self.dashboard.DOExecute(channel, 0)
                 time.sleep(1)
         return True
     
     def push(self, duration:Optional[int] = None) -> bool:
         """
         Activate pump to blow out air
         
         Args:
             duration (Optional[int], optional): number of seconds to push air. Defaults to None.
             
         Returns:
             bool: whether action is successful
         """
+        channel = self.channel_map.get("push", 2)
         try:
-            self.dashboard.DOExecute(2,1)
+            self.dashboard.DOExecute(channel, 1)
         except (AttributeError, OSError):
             print('Tried to push...')
             print("Not connected to arm.")
             return False
         else:
             if duration is not None:
                 time.sleep(duration)
-                self.dashboard.DOExecute(2,0)
+                self.dashboard.DOExecute(channel, 0)
                 time.sleep(1)
         return True
     
     def stop(self) -> bool:
         """
         Stop airflow
         
         Returns:
             bool: whether action is successful
         """
+        channels = [v for v in self.channel_map.values()] if len(self.channel_map) else [1,2]
         try:
-            self.dashboard.DOExecute(2,0)
-            self.dashboard.DOExecute(1,0)
+            for channel in channels:
+                self.dashboard.DOExecute(channel, 0)
             time.sleep(1)
         except (AttributeError, OSError):
             print('Tried to stop...')
             print("Not connected to arm.")
             return False
         return True
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     Abstract Base Class (ABC) for Gripper objects (i.e. tools that picks up and places objects).
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
 
     ### Methods
     #### Abstract
     - `drop`: releases an object
     - `grab`: picks up an object
+    #### Public
+    - `toggleGrip`: grip or release the object
     """
     
     def __init__(self):
         """Instantiate the class"""
         ...
     
     @abstractmethod
@@ -37,7 +39,20 @@
     def grab(self) -> bool:
         """
         Picks up an object
         
         Returns:
             bool: whether action is successful
         """
+    
+    def toggleGrip(self, on:bool):
+        """
+        Grip or release the object
+
+        Args:
+            on (bool): whether to grip the object
+        """
+        if on:
+            self.grab()
+        else:
+            self.drop()
+        return
```

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/image_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/View/image_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/View/view_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/__init__.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/decorators.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/factory.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/helper.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/layout.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/logger.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/tests/test_compound_liquidmover.py` & `control-lab-ly-1.1.0a0/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/tests/test_compound_spin_printer.py` & `control-lab-ly-1.1.0a0/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/tests/test_dobot_m1pro.py` & `control-lab-ly-1.1.0a0/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/tests/test_dobot_mg400.py` & `control-lab-ly-1.1.0a0/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a3/tests/test_heat_peltier.py` & `control-lab-ly-1.1.0a0/tests/test_heat_peltier.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # %%
 me.holdTemperature(30, 90)
 # %%
 me.setTemperature(35, blocking=False)
 # %%
 me.toggleRecord(False)
 # %%
-me.getTemperatures()
+me.getTemperature()
 # %%
 me.setTemperature(25, blocking=False)
 # %%
 import plotly.express as px
 me.clearCache()
 me.toggleRecord(True)
 for temperature in [25,30,35,40,45,50]:
```

### Comparing `control-lab-ly-1.0.1a3/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.1.0a0/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

