# Comparing `tmp/PyFlyt-0.7.0.tar.gz` & `tmp/PyFlyt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.7.0.tar", last modified: Fri May 12 22:23:11 2023, max compression
+gzip compressed data, was "PyFlyt-0.7.1.tar", last modified: Mon May 15 15:53:26 2023, max compression
```

## Comparing `PyFlyt-0.7.0.tar` & `PyFlyt-0.7.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.7.0/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.7.0/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.7.0/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2799 2023-05-12 21:50:26.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4454 2023-05-12 22:13:35.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15316 2023-05-12 22:13:14.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.7.0/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    17975 2023-05-12 22:20:50.000000 PyFlyt-0.7.0/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.7.0/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.7.0/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18407 2023-05-12 22:08:36.000000 PyFlyt-0.7.0/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-12 21:46:35.000000 PyFlyt-0.7.0/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.7.0/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.7.0/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.7.0/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.7.0/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.7.0/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.7.0/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.7.0/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.310949 PyFlyt-0.7.0/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 22:23:11.000000 PyFlyt-0.7.0/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-05-12 22:23:11.000000 PyFlyt-0.7.0/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-12 22:23:11.000000 PyFlyt-0.7.0/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-05-12 22:23:11.000000 PyFlyt-0.7.0/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-12 22:23:11.000000 PyFlyt-0.7.0/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-05-12 22:23:04.000000 PyFlyt-0.7.0/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.7.0/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.7.0/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 22:23:11.314949 PyFlyt-0.7.0/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8567 2023-05-12 21:34:19.000000 PyFlyt-0.7.0/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.7.0/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-06-30 13:35:00.000000 PyFlyt-0.7.1/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.556448 PyFlyt-0.7.1/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.560449 PyFlyt-0.7.1/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-07 16:22:47.000000 PyFlyt-0.7.1/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.564448 PyFlyt-0.7.1/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4454 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15316 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    17975 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.568448 PyFlyt-0.7.1/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-11 16:33:17.000000 PyFlyt-0.7.1/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18407 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.568448 PyFlyt-0.7.1/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.568448 PyFlyt-0.7.1/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.572449 PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.572449 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-21 13:48:00.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.572449 PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-11 16:33:17.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.576449 PyFlyt-0.7.1/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-28 12:51:18.000000 PyFlyt-0.7.1/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-06-30 13:35:00.000000 PyFlyt-0.7.1/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-28 12:51:18.000000 PyFlyt-0.7.1/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.556448 PyFlyt-0.7.1/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.576449 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-22 14:06:54.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-21 13:48:00.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-07 01:25:05.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-07 01:25:05.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.560449 PyFlyt-0.7.1/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       49 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1171 2023-05-15 15:52:13.000000 PyFlyt-0.7.1/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 15:14:17.000000 PyFlyt-0.7.1/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-03-21 13:48:00.000000 PyFlyt-0.7.1/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.7.0/LICENSE.txt` & `PyFlyt-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PKG-INFO` & `PyFlyt-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.0
+Version: 0.7.1
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Defines a basic wind field class to inherit from when implementing custom wind field models."""
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 
 import numpy as np
 
 
 class WindFieldClass(ABC):
     """Basic WindField class to implement custom wind field models.
 
     Example Usage:
         >>> from PyFlyt.core import Aviary
-        >>> from PyFlyt.abstractions import WindFieldClass
+        >>> from PyFlyt.core.abstractions import WindFieldClass
         >>>
         >>> # define the wind field
         >>> class MyWindField(WindFieldClass):
         >>>     def __init__(self, my_parameter=1.0, np_random: None | np.random.RandomState = None):
         >>>         super().__init__(np_random)
         >>>         self.strength = my_parameter
         >>>
```

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.7.1/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/aviary.py` & `PyFlyt-0.7.1/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.7.1/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.7.1/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.7.1/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/core/load_objs.py` & `PyFlyt-0.7.1/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.7.1/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.7.1/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.7.1/PyFlyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.0
+Version: 0.7.1
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.7.0/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.7.1/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/pyproject.toml` & `PyFlyt-0.7.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["matplotlib", "gymnasium", "numpy", "pybullet", "pyyaml"]
+dependencies = ["wheel", "matplotlib", "gymnasium", "numpy", "pybullet", "pyyaml"]
 keywords = ["Reinforcement Learning", "UAVs", "drones", "Quadcopter", "AI", "RL", "Gymnasium"]
 license = { file="./LICENSE.txt" }
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
```

### Comparing `PyFlyt-0.7.0/readme.md` & `PyFlyt-0.7.1/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.0/tests/test_core.py` & `PyFlyt-0.7.1/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Tests the the core API functionality."""
+from __future__ import annotations
+
 import numpy as np
 import pytest
 from custom_uavs.rocket_brick import RocketBrick
 
 from PyFlyt.core import Aviary
 from PyFlyt.core.abstractions import ControlClass, WindFieldClass
```

### Comparing `PyFlyt-0.7.0/tests/test_gym_envs.py` & `PyFlyt-0.7.1/tests/test_gym_envs.py`

 * *Files identical despite different names*

