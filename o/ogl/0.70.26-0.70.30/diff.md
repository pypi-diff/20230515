# Comparing `tmp/ogl-0.70.26.tar.gz` & `tmp/ogl-0.70.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogl-0.70.26.tar", last modified: Thu Apr 13 20:22:30 2023, max compression
+gzip compressed data, was "ogl-0.70.30.tar", last modified: Mon May 15 00:20:45 2023, max compression
```

## Comparing `ogl-0.70.26.tar` & `ogl-0.70.30.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.170659 ogl-0.70.26/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.26/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-04-13 20:22:30.170521 ogl-0.70.26/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.26/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.162524 ogl-0.70.26/miniogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/AnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.26/miniogl/AttachmentSide.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2916 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/Constants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/ControlPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-02-11 18:19:50.000000 ogl-0.70.26/miniogl/Diagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-03-25 20:34:07.000000 ogl-0.70.26/miniogl/DiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/DlgDebugDiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/LinePoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/LineShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.26/miniogl/LollipopLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.26/miniogl/MiniOglColorEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/MiniOglPenStyle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/MiniOglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/PointShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10735 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/RectangleShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/RectangleShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.26/miniogl/RotatableShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/SelectAnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/Shape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2322 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/ShapeEventHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.26/miniogl/ShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/SizerShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.26/miniogl/TextShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/TextShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.26/miniogl/VShapes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/miniogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/miniogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.165331 ogl-0.70.26/ogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/IllegalOperationException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3747 2022-06-08 19:34:57.000000 ogl-0.70.26/ogl/OglActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.26/ogl/OglAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.26/ogl/OglAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      204 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/OglAssociationLabel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-03-25 20:34:07.000000 ogl-0.70.26/ogl/OglClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.26/ogl/OglComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/OglConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/OglDimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.26/ogl/OglInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.26/ogl/OglInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.26/ogl/OglInterface2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.26/ogl/OglLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.26/ogl/OglLinkFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.26/ogl/OglNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.26/ogl/OglNoteLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5511 2023-02-11 18:20:44.000000 ogl-0.70.26/ogl/OglObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      473 2022-07-18 19:30:46.000000 ogl-0.70.26/ogl/OglPosition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8713 2023-03-22 20:23:56.000000 ogl-0.70.26/ogl/OglText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/OglTextFontFamily.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.26/ogl/OglUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/OglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.166747 ogl-0.70.26/ogl/events/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.26/ogl/events/IOglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/events/InvalidKeywordException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.26/ogl/events/OglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.26/ogl/events/OglEvents.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/events/ShapeSelectedEventData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/events/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/events/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.167048 ogl-0.70.26/ogl/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21283 2023-03-26 21:40:46.000000 ogl-0.70.26/ogl/preferences/OglPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.167136 ogl-0.70.26/ogl/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.167693 ogl-0.70.26/ogl/resources/img/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/Display.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/DoNotDisplay.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/UnSpecified.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/resources/img/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.168154 ogl-0.70.26/ogl/resources/img/textdetails/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/textdetails/DecreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/textdetails/IncreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/resources/img/textdetails/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/resources/img/textdetails/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.168718 ogl-0.70.26/ogl/sd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1212 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/sd/OglInstanceName.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-03-26 01:49:15.000000 ogl-0.70.26/ogl/sd/OglSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7333 2023-03-26 01:50:44.000000 ogl-0.70.26/ogl/sd/OglSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.26/ogl/sd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/sd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.169506 ogl-0.70.26/ogl/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-02-08 20:22:10.000000 ogl-0.70.26/ogl/ui/BaseOglPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.26/ogl/ui/DefaultValuesPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.26/ogl/ui/DiagramPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.26/ogl/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.26/ogl/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.170380 ogl-0.70.26/ogl/ui/valuecontrols/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.26/ogl/ui/valuecontrols/AssociationAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.26/ogl/ui/valuecontrols/ClassAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.26/ogl/ui/valuecontrols/DefaultNamesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.26/ogl/ui/valuecontrols/NoteAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.26/ogl/ui/valuecontrols/SDAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4427 2023-02-09 23:51:26.000000 ogl-0.70.26/ogl/ui/valuecontrols/TextAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.26/ogl/ui/valuecontrols/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 20:22:30.165917 ogl-0.70.26/ogl.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-04-13 20:22:30.000000 ogl-0.70.26/ogl.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2500 2023-04-13 20:22:30.000000 ogl-0.70.26/ogl.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 20:22:30.000000 ogl-0.70.26/ogl.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-04-13 20:22:30.000000 ogl-0.70.26/ogl.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-13 20:22:30.000000 ogl-0.70.26/ogl.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 20:22:30.170697 ogl-0.70.26/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-04-13 20:20:53.000000 ogl-0.70.26/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.213016 ogl-0.70.30/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.30/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-05-15 00:20:45.212892 ogl-0.70.30/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.30/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.205310 ogl-0.70.30/miniogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/AnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.30/miniogl/AttachmentSide.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2916 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/Constants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/ControlPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-02-11 18:19:50.000000 ogl-0.70.30/miniogl/Diagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-03-25 20:34:07.000000 ogl-0.70.30/miniogl/DiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/DlgDebugDiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/LinePoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/LineShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.30/miniogl/LollipopLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.30/miniogl/MiniOglColorEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/MiniOglPenStyle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/MiniOglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/PointShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-03 16:34:04.000000 ogl-0.70.30/miniogl/RectangleShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/RectangleShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.30/miniogl/RotatableShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/SelectAnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/Shape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2322 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/ShapeEventHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/ShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/SizerShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.30/miniogl/TextShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/TextShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.30/miniogl/VShapes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/miniogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.208340 ogl-0.70.30/ogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/IllegalOperationException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3747 2022-06-08 19:34:57.000000 ogl-0.70.30/ogl/OglActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.30/ogl/OglAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.30/ogl/OglAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      204 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglAssociationLabel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-03-25 20:34:07.000000 ogl-0.70.30/ogl/OglClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.30/ogl/OglComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglDimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.30/ogl/OglInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.30/ogl/OglInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.30/ogl/OglInterface2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.30/ogl/OglLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.30/ogl/OglLinkFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.30/ogl/OglNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.30/ogl/OglNoteLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5544 2023-05-03 16:33:14.000000 ogl-0.70.30/ogl/OglObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      473 2022-07-18 19:30:46.000000 ogl-0.70.30/ogl/OglPosition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8713 2023-03-22 20:23:56.000000 ogl-0.70.30/ogl/OglText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglTextFontFamily.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.30/ogl/OglUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.70.30/ogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       24 2023-05-15 00:08:21.000000 ogl-0.70.30/ogl/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.209696 ogl-0.70.30/ogl/events/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.30/ogl/events/IOglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/events/InvalidKeywordException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.30/ogl/events/OglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.30/ogl/events/OglEvents.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/events/ShapeSelectedEventData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/events/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/events/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210009 ogl-0.70.30/ogl/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.70.30/ogl/preferences/OglPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210097 ogl-0.70.30/ogl/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210587 ogl-0.70.30/ogl/resources/img/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/Display.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/DoNotDisplay.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/UnSpecified.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/resources/img/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210988 ogl-0.70.30/ogl/resources/img/textdetails/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/textdetails/DecreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/textdetails/IncreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/textdetails/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/resources/img/textdetails/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.211480 ogl-0.70.30/ogl/sd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.70.30/ogl/sd/OglInstanceName.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-03-26 01:49:15.000000 ogl-0.70.30/ogl/sd/OglSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.70.30/ogl/sd/OglSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/sd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/sd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.211986 ogl-0.70.30/ogl/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-02-08 20:22:10.000000 ogl-0.70.30/ogl/ui/BaseOglPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.30/ogl/ui/DefaultValuesPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.30/ogl/ui/DiagramPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.30/ogl/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.212730 ogl-0.70.30/ogl/ui/valuecontrols/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.30/ogl/ui/valuecontrols/AssociationAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.30/ogl/ui/valuecontrols/ClassAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.30/ogl/ui/valuecontrols/DefaultNamesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.30/ogl/ui/valuecontrols/NoteAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.30/ogl/ui/valuecontrols/SDAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.70.30/ogl/ui/valuecontrols/TextAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.30/ogl/ui/valuecontrols/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.208952 ogl-0.70.30/ogl.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 00:20:45.213049 ogl-0.70.30/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1565 2023-05-14 21:30:41.000000 ogl-0.70.30/setup.py
```

### Comparing `ogl-0.70.26/LICENSE` & `ogl-0.70.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/PKG-INFO` & `ogl-0.70.30/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 0.70.26
+Version: 0.70.30
 Summary: External Pyut Graphical Shapes
 Home-page: https://github.com/hasii2011/ogl
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.26 Summary: External Pyut
+Metadata-Version: 2.1 Name: ogl Version: 0.70.30 Summary: External Pyut
 Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
 A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
 Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE [./developer/
 agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
```

### Comparing `ogl-0.70.26/README.md` & `ogl-0.70.30/README.md`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/AnchorPoint.py` & `ogl-0.70.30/miniogl/AnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/AttachmentSide.py` & `ogl-0.70.30/miniogl/AttachmentSide.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/Common.py` & `ogl-0.70.30/miniogl/Common.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/ControlPoint.py` & `ogl-0.70.30/miniogl/ControlPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/Diagram.py` & `ogl-0.70.30/miniogl/Diagram.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/DiagramFrame.py` & `ogl-0.70.30/miniogl/DiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/DlgDebugDiagramFrame.py` & `ogl-0.70.30/miniogl/DlgDebugDiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/LinePoint.py` & `ogl-0.70.30/miniogl/LinePoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/LineShape.py` & `ogl-0.70.30/miniogl/LineShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/LollipopLine.py` & `ogl-0.70.30/miniogl/LollipopLine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/MiniOglColorEnum.py` & `ogl-0.70.30/miniogl/MiniOglColorEnum.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/MiniOglPenStyle.py` & `ogl-0.70.30/miniogl/MiniOglPenStyle.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/PointShape.py` & `ogl-0.70.30/miniogl/PointShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/RectangleShape.py` & `ogl-0.70.30/miniogl/RectangleShape.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,16 @@
     @deprecated(reason='Use the .selected property')
     def SetSelected(self, state: bool = True):
         """
         Select the shape.
 
         @param state
         """
-        Shape.SetSelected(self, state)
+        # Shape.SetSelected(self, state)
+        self.selected = state
         if self._resizable:
             self.ShowSizers(state)
 
     def Detach(self):
         """
         Detach the shape from its diagram.
         This is the way to delete a shape. All anchor points are also
```

### Comparing `ogl-0.70.26/miniogl/RectangleShapeModel.py` & `ogl-0.70.30/miniogl/RectangleShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/RotatableShape.py` & `ogl-0.70.30/miniogl/RotatableShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/SelectAnchorPoint.py` & `ogl-0.70.30/miniogl/SelectAnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/Shape.py` & `ogl-0.70.30/miniogl/Shape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/ShapeEventHandler.py` & `ogl-0.70.30/miniogl/ShapeEventHandler.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/ShapeModel.py` & `ogl-0.70.30/miniogl/ShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/SizerShape.py` & `ogl-0.70.30/miniogl/SizerShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/TextShape.py` & `ogl-0.70.30/miniogl/TextShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/TextShapeModel.py` & `ogl-0.70.30/miniogl/TextShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/miniogl/VShapes.py` & `ogl-0.70.30/miniogl/VShapes.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglActor.py` & `ogl-0.70.30/ogl/OglActor.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglAggregation.py` & `ogl-0.70.30/ogl/OglAggregation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglAssociation.py` & `ogl-0.70.30/ogl/OglAssociation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglClass.py` & `ogl-0.70.30/ogl/OglClass.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglComposition.py` & `ogl-0.70.30/ogl/OglComposition.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglConstants.py` & `ogl-0.70.30/ogl/OglConstants.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglDimensions.py` & `ogl-0.70.30/ogl/OglDimensions.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglInheritance.py` & `ogl-0.70.30/ogl/OglInheritance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglInterface.py` & `ogl-0.70.30/ogl/OglInterface.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglInterface2.py` & `ogl-0.70.30/ogl/OglInterface2.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglLink.py` & `ogl-0.70.30/ogl/OglLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglLinkFactory.py` & `ogl-0.70.30/ogl/OglLinkFactory.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglNote.py` & `ogl-0.70.30/ogl/OglNote.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglNoteLink.py` & `ogl-0.70.30/ogl/OglNoteLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglObject.py` & `ogl-0.70.30/ogl/OglObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,8 +175,10 @@
 
         # from org.pyut.ui.Mediator import Mediator          # avoid circular import
         # from org.pyut.ui.Mediator import ACTION_ZOOM_OUT   # avoid circular import
 
         # mediator: Mediator = Mediator()
         # if mediator.getCurrentAction() != ACTION_ZOOM_OUT:
         # TODO:  I took this out because could never cause this to happen;  Conveniently, this removes all mediator calls
-        RectangleShape.SetSelected(self, state)
+        # RectangleShape.SetSelected(self, state)
+        self.selected = state
+
```

### Comparing `ogl-0.70.26/ogl/OglText.py` & `ogl-0.70.30/ogl/OglText.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglUseCase.py` & `ogl-0.70.30/ogl/OglUseCase.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/OglUtils.py` & `ogl-0.70.30/ogl/OglUtils.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/events/IOglEventEngine.py` & `ogl-0.70.30/ogl/events/IOglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/events/OglEventEngine.py` & `ogl-0.70.30/ogl/events/OglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/events/OglEvents.py` & `ogl-0.70.30/ogl/events/OglEvents.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/preferences/OglPreferences.py` & `ogl-0.70.30/ogl/preferences/OglPreferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         NOTE_DIMENSIONS:        OglDimensions(100, 50).__str__(),
         TEXT_DIMENSIONS:        OglDimensions(125, 50).__str__(),
         TEXT_BOLD:              'False',
         TEXT_ITALICIZE:         'False',
         TEXT_FONT_FAMILY:       'Swiss',
         TEXT_FONT_SIZE:         '14',
         TEXT_VALUE:             'Donec eleifend luctus enim vel mollis',
-        CLASS_DIMENSIONS:        OglDimensions(100, 100).__str__(),
+        CLASS_DIMENSIONS:        OglDimensions(150, 75).__str__(),
         CLASS_BACKGROUND_COLOR:  DEFAULT_CLASS_BACKGROUND_COLOR,
         CLASS_TEXT_COLOR:        DEFAULT_CLASS_TEXT_COLOR,
     }
 
     DEFAULT_GRID_LINE_COLOR: str = MiniOglColorEnum.LIGHT_GREY.value
     DEFAULT_GRID_LINE_STYLE: str = MiniOglPenStyle.DOT.value
```

### Comparing `ogl-0.70.26/ogl/resources/img/Display.py` & `ogl-0.70.30/ogl/resources/img/Display.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/resources/img/DoNotDisplay.py` & `ogl-0.70.30/ogl/resources/img/DoNotDisplay.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/resources/img/UnSpecified.py` & `ogl-0.70.30/ogl/resources/img/UnSpecified.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/resources/img/textdetails/DecreaseTextSize.py` & `ogl-0.70.30/ogl/resources/img/textdetails/DecreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/resources/img/textdetails/IncreaseTextSize.py` & `ogl-0.70.30/ogl/resources/img/textdetails/IncreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/sd/OglSDInstance.py` & `ogl-0.70.30/ogl/sd/OglSDInstance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/sd/OglSDMessage.py` & `ogl-0.70.30/ogl/sd/OglSDMessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,19 @@
+
 from typing import List
 from typing import Tuple
 
 from logging import Logger
 from logging import getLogger
 
 from deprecated import deprecated
 
 from wx import BLACK_PEN
-
-from wx import CANCEL
-from wx import CENTRE
 from wx import DC
-from wx import ID_OK
-from wx import OK
 from wx import RED_PEN
-from wx import TextEntryDialog
 
 from pyutmodel.PyutSDMessage import PyutSDMessage
 
 from miniogl.LineShape import LineShape
 from miniogl.AnchorPoint import AnchorPoint
 from miniogl.TextShape import TextShape
 
@@ -175,24 +170,14 @@
 
         links: List[OglSDMessage] = src.links
         links.remove(self)
 
         links = dst.links
         links.remove(self)
 
-    def OnLeftDClick(self, event):
-        """
-        Callback for left double clicks.
-
-        """
-        dlg = TextEntryDialog(None, "Message", "Enter message name", self._pyutSDMessage.getMessage(), OK | CANCEL | CENTRE)
-        if dlg.ShowModal() == ID_OK:
-            self._pyutSDMessage.setMessage(dlg.GetValue())
-        dlg.Destroy()
-
     def _createAnchorPoints(self, srcShape: OglSDInstance, dstShape: OglSDInstance,
                             pyutSDMessage: PyutSDMessage) -> Tuple[AnchorPoint, AnchorPoint]:
         """
         Royal ready to heat rice
 
         Args:
             dstShape:
```

### Comparing `ogl-0.70.26/ogl/ui/BaseOglPreferencesPage.py` & `ogl-0.70.30/ogl/ui/BaseOglPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/DefaultValuesPreferencesPage.py` & `ogl-0.70.30/ogl/ui/DefaultValuesPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/DiagramPreferencesPage.py` & `ogl-0.70.30/ogl/ui/DiagramPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/valuecontrols/AssociationAttributesControl.py` & `ogl-0.70.30/ogl/ui/valuecontrols/AssociationAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/valuecontrols/ClassAttributesControl.py` & `ogl-0.70.30/ogl/ui/valuecontrols/ClassAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/valuecontrols/DefaultNamesControl.py` & `ogl-0.70.30/ogl/ui/valuecontrols/DefaultNamesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/valuecontrols/NoteAttributesControl.py` & `ogl-0.70.30/ogl/ui/valuecontrols/NoteAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/valuecontrols/SDAttributesControl.py` & `ogl-0.70.30/ogl/ui/valuecontrols/SDAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.26/ogl/ui/valuecontrols/TextAttributesControl.py` & `ogl-0.70.30/ogl/ui/valuecontrols/TextAttributesControl.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from wx import CB_READONLY
 from wx import EVT_CHECKBOX
 from wx import EVT_COMBOBOX
 
 from wx import CheckBox
 from wx import ComboBox
 from wx import CommandEvent
+from wx import EVT_TEXT
+from wx import TextCtrl
 from wx import Window
 
 from wx.lib.sized_controls import SizedPanel
 from wx.lib.sized_controls import SizedStaticBox
 
 from hasiicommon.ui.widgets.DimensionsControl import DimensionsControl
 
@@ -29,14 +31,18 @@
 
     def __init__(self, parent: Window):
 
         self.logger:       Logger         = getLogger(__name__)
         self._preferences: OglPreferences = OglPreferences()
         super().__init__(parent)
 
+        self.SetSizerType('vertical')
+
+        self._textDefaultText: TextCtrl = self._createDefaultTextPanel(self)
+
         self._textDimensions: DimensionsControl = DimensionsControl(sizedPanel=self,
                                                                     displayText='Text Width/Height',
                                                                     valueChangedCallback=self._onTextDimensionsChanged,
                                                                     setControlsSize=False
                                                                     )
         self._boldText:         CheckBox = cast(CheckBox, None)
         self._italicizeText:    CheckBox = cast(CheckBox, None)
@@ -46,27 +52,40 @@
         self._createTextStylePanel(self)
         self._createFontAttributesPanel(self)
         self._setControlValues()
         self._bindControls()
 
     def _setControlValues(self):
 
+        self._textDefaultText.SetValue(self._preferences.textValue)
         self._textDimensions.dimensions = self._preferences.textDimensions
         self._boldText.SetValue(self._preferences.textBold)
         self._italicizeText.SetValue(self._preferences.textItalicize)
         self._fontSizeSelector.SetValue(str(self._preferences.textFontSize))
 
     def _bindControls(self):
 
+        self.Bind(EVT_TEXT,     self._onDefaultTextValueChanged,   self._textDefaultText)
         self.Bind(EVT_CHECKBOX, self._onTextBoldValueChanged,      self._boldText)
         self.Bind(EVT_CHECKBOX, self._onTextItalicizeValueChanged, self._italicizeText)
 
         self.Bind(EVT_COMBOBOX, self._onFontSelectionChanged,     self._fontSelector)
         self.Bind(EVT_COMBOBOX, self._onFontSizeSelectionChanged, self._fontSizeSelector)
 
+    def _createDefaultTextPanel(self, parent: SizedPanel):
+        directoryPanel: SizedStaticBox = SizedStaticBox(parent, label='Default Text')
+
+        directoryPanel.SetSizerType('horizontal')
+        directoryPanel.SetSizerProps(expand=True, proportion=1)
+
+        textCtrl: TextCtrl = TextCtrl(directoryPanel)
+        textCtrl.SetSizerProps(expand=True, proportion=5)
+
+        return textCtrl
+
     def _createTextStylePanel(self, parent: SizedPanel):
 
         stylePanel: SizedPanel = SizedPanel(parent)
         stylePanel.SetSizerType('horizontal')
         stylePanel.SetSizerProps(expand=True, proportion=1)
 
         self._boldText      = CheckBox(parent=stylePanel, label='Bold Text')
@@ -85,14 +104,17 @@
         self._fontSelector = ComboBox(fontPanel, choices=fontChoices, style=CB_READONLY)
         self._fontSelector.SetSizerProps(expand=True, proportion=1)
 
         fontSizes: List[str] = ['8', '9', '10', '11', '12', '13', '14', '15', '16', '17', '18', '19', '20']
         self._fontSizeSelector = ComboBox(fontPanel, choices=fontSizes, style=CB_READONLY)
         self._fontSizeSelector.SetSizerProps(expand=True, proportion=1)
 
+    def _onDefaultTextValueChanged(self, event: CommandEvent):
+        self._preferences.textValue = self._textDefaultText.GetValue()
+
     def _onTextDimensionsChanged(self, newValue: OglDimensions):
         self._preferences.textDimensions = newValue
 
     def _onTextBoldValueChanged(self, event: CommandEvent):
 
         val: bool = event.IsChecked()
```

### Comparing `ogl-0.70.26/ogl.egg-info/PKG-INFO` & `ogl-0.70.30/ogl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 0.70.26
+Version: 0.70.30
 Summary: External Pyut Graphical Shapes
 Home-page: https://github.com/hasii2011/ogl
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.26 Summary: External Pyut
+Metadata-Version: 2.1 Name: ogl Version: 0.70.30 Summary: External Pyut
 Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
 A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
 Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE [./developer/
 agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
```

### Comparing `ogl-0.70.26/ogl.egg-info/SOURCES.txt` & `ogl-0.70.30/ogl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 ogl/OglObject.py
 ogl/OglPosition.py
 ogl/OglText.py
 ogl/OglTextFontFamily.py
 ogl/OglUseCase.py
 ogl/OglUtils.py
 ogl/__init__.py
+ogl/_version.py
 ogl/py.typed
 ogl.egg-info/PKG-INFO
 ogl.egg-info/SOURCES.txt
 ogl.egg-info/dependency_links.txt
 ogl.egg-info/requires.txt
 ogl.egg-info/top_level.txt
 ogl/events/IOglEventEngine.py
```

### Comparing `ogl-0.70.26/setup.py` & `ogl-0.70.30/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+
 import pathlib
+
 from setuptools import setup
+from ogl import __version__ as oglVersion
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
+
 setup(
     name="ogl",
-    version="0.70.26",
+    version=oglVersion,
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Graphical Shapes',
     long_description=README,
     long_description_content_type="text/markdown",
```

