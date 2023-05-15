# Comparing `tmp/hurdat2parser-2.2.tar.gz` & `tmp/hurdat2parser-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurdat2parser-2.2.tar", last modified: Sun Apr  9 01:27:04 2023, max compression
+gzip compressed data, was "hurdat2parser-2.2.2.tar", last modified: Mon Apr 24 15:16:58 2023, max compression
```

## Comparing `hurdat2parser-2.2.tar` & `hurdat2parser-2.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 01:27:04.086099 hurdat2parser-2.2/
--rw-rw-rw-   0        0        0     1115 2023-04-09 01:19:53.000000 hurdat2parser-2.2/LICENSE.txt
--rw-rw-rw-   0        0        0    33455 2023-04-09 01:27:04.086099 hurdat2parser-2.2/PKG-INFO
--rw-rw-rw-   0        0        0    32862 2023-04-09 01:14:18.000000 hurdat2parser-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 01:27:04.014084 hurdat2parser-2.2/hurdat2parser/
--rw-rw-rw-   0        0        0    57354 2023-04-07 05:04:47.000000 hurdat2parser-2.2/hurdat2parser/__init__.py
--rw-rw-rw-   0        0        0     7088 2023-02-28 07:16:47.000000 hurdat2parser-2.2/hurdat2parser/_aliases.py
--rw-rw-rw-   0        0        0    80092 2023-02-26 03:51:21.000000 hurdat2parser-2.2/hurdat2parser/_calculations.py
--rw-rw-rw-   0        0        0    14830 2023-02-24 08:17:51.000000 hurdat2parser-2.2/hurdat2parser/_future.py
--rw-rw-rw-   0        0        0   163453 2022-07-18 22:48:06.000000 hurdat2parser-2.2/hurdat2parser/_maps.py
--rw-rw-rw-   0        0        0    37465 2023-03-02 07:25:50.000000 hurdat2parser-2.2/hurdat2parser/_reports.py
-drwxrwxrwx   0        0        0        0 2023-04-09 01:27:04.086099 hurdat2parser-2.2/hurdat2parser.egg-info/
--rw-rw-rw-   0        0        0    33455 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 01:27:02.000000 hurdat2parser-2.2/hurdat2parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-22 04:30:18.000000 hurdat2parser-2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 01:27:04.086099 hurdat2parser-2.2/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-04-09 01:21:06.000000 hurdat2parser-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:16:58.370981 hurdat2parser-2.2.2/
+-rw-rw-rw-   0        0        0     1117 2023-04-24 15:12:41.000000 hurdat2parser-2.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    27935 2023-04-24 15:16:58.368980 hurdat2parser-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27340 2023-04-24 15:14:27.000000 hurdat2parser-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:16:58.327093 hurdat2parser-2.2.2/hurdat2parser/
+-rw-rw-rw-   0        0        0    57368 2023-04-24 15:14:52.000000 hurdat2parser-2.2.2/hurdat2parser/__init__.py
+-rw-rw-rw-   0        0        0     7088 2023-02-28 07:16:47.000000 hurdat2parser-2.2.2/hurdat2parser/_aliases.py
+-rw-rw-rw-   0        0        0    79986 2023-04-24 14:42:33.000000 hurdat2parser-2.2.2/hurdat2parser/_calculations.py
+-rw-rw-rw-   0        0        0    14830 2023-02-24 08:17:51.000000 hurdat2parser-2.2.2/hurdat2parser/_future.py
+-rw-rw-rw-   0        0        0   163453 2022-07-18 22:48:06.000000 hurdat2parser-2.2.2/hurdat2parser/_maps.py
+-rw-rw-rw-   0        0        0    37465 2023-03-02 07:25:50.000000 hurdat2parser-2.2.2/hurdat2parser/_reports.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:16:58.365090 hurdat2parser-2.2.2/hurdat2parser.egg-info/
+-rw-rw-rw-   0        0        0    27935 2023-04-24 15:16:58.000000 hurdat2parser-2.2.2/hurdat2parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-04-24 15:16:58.000000 hurdat2parser-2.2.2/hurdat2parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:16:58.000000 hurdat2parser-2.2.2/hurdat2parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 15:16:57.000000 hurdat2parser-2.2.2/hurdat2parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-04-24 15:16:58.000000 hurdat2parser-2.2.2/hurdat2parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 15:16:58.000000 hurdat2parser-2.2.2/hurdat2parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-22 04:30:18.000000 hurdat2parser-2.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:16:58.371982 hurdat2parser-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      900 2023-04-24 15:15:51.000000 hurdat2parser-2.2.2/setup.py
```

### Comparing `hurdat2parser-2.2/LICENSE.txt` & `hurdat2parser-2.2.2/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-hurdat2parser 2.2, Copyright (c) 2019-2023, Kyle S. Gentry
+hurdat2parser 2.2.2, Copyright (c) 2019-2023, Kyle S. Gentry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hurdat2parser-2.2/PKG-INFO` & `hurdat2parser-2.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hurdat2parser
-Version: 2.2
+Version: 2.2.2
 Summary: Interpret Hurricane Data contained in HURDAT2
 Home-page: http://github.com/ksgwxfan/hurdat2parser
 Author: Kyle S. Gentry
 Author-email: KyleSGentry@outlook.com
 License: MIT
 Keywords: hurricane hurdat2 meteorology weather
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# hurdat2parser -- v2.2
+# hurdat2parser -- v2.2.2
 ---
 ### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
@@ -34,65 +34,18 @@
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
 * [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.2)
+## Changes in this Version (2.2.2)
 
-- Docstring'd `TCRecordEntry` properties
-- Changes to the `<Hurdat2>` object:
-  - when reading-in files on `__init__`, multiple local files are now supported.
-  - enabled download of the most-recent hurdat2 dataset through the `basin` kwarg.
-  - added a `urlcheck` kwarg. If `True`, the "file-path"s listed will be treated like URLs and a download attempt will be made.
-  - removed the `_filesappended` attribute
-  - Searching for notoriously-named storms can be done by a dash (`"-"`) prefix to the search string in addition to an underscore (see [Example Calls](#example-calls) section)
-  - Revamped `output_climo_csv`, `output_season_csv`, and `output_storms_csv` methods
-    - simplified code; updated and unified attributes used in the reports and made it significantly easier for future maintenance.
-  - moved `multi_season_info` method to `_reports`
-- New properties for both `Season` and `TropicalCyclone`:
-  - `duration`
-    - `Season` version reports time between the first and last day of the season (see further in the document for explanation)
-	- `TropicalCyclone` version just reports the track-life in days, regardless of status. More useful status-based duration properties were created too. Keep reading (a few lines down).
-  - `tc_entries` returns a list of `TCRecordEntry`s where a storm was a designated tropical cyclone.
-  - `start_date`, `start_ordinal`, and `end_date`, `end_ordinal` report the starting/ending dates and/or days of the year
-- New `TropicalCyclone` variables:
-  - `ACE_no_landfall`
-  - `duration_<TC, TS, HU, MHU>` - These properties report the aggregate time in days that a tropical cyclone was designated that status or stronger, accounting for fluxuations in storm statuses and strengths.
-  - removed `coord_list` method. It was redundant as it was like a shortened combination of the `summary` method.
-- New `TCRecordEntry` variables:
-  - tweaked how location variables are defined. `location` and `location_reversed` are now properties that depend on the express definition of the variables `lat` and `lon` rather than the other way around.
-  - tweak of not-available wind-extent data. As of the moment typing this, wind-extent data is only provided for storms since 2004. All previous wind-extent data is `-999`, meaning its unavailable. But if a storm has max winds of `<` 64, its Hurricane wind extent has to be 0. So when ingesting the data, this determination is made.
-  - tweaked ingest of data to prevent errors due to possible new Hurdat2 categories introduced in future versions. This was the problem with `v2.1` that was responsible for the need for a `v2.11` release. This particular version wouldn't be able to read-in the new variables in such a situation, but it would still be functional with the newer database (unless order of variables are switched around).
-  - the formerly-called variable `wind_radii` from `v2.11` is now called `maxwind_radius`. I don't know why I called it `radii`, as in plural of radius. I guess it sounded science-y or smart. haha. But the change is also more readable.
-  - Surface Area (coverage)-based variables `areal_extent_TS`, `areal_extent_TS50`, and `areal_extent_HU`.
-    - These are calculated from reported wind-extents in the database.
-  - `track_distance`: the track distance of the cyclone up to the point of the respective entry; this does not account for storm status
-  - `previous_entries` and `next_entries`: lists of the previous and next recorded entries, respectively, in the `TropicalCyclone`'s record
-  - `previous_entry` and `next_entry`: the previous and next recorded entry, respectively, in the `TropicalCyclone`'s record
-  - `direction()`: the `TropicalCyclone`'s heading in degrees (or cardinal, if desired...see docstring)
-  - `speed`: the `TropicalCyclone`'s forward speed in knots.
-  - Properties to simplify coding and reduce probability of coding errors.
-    - `is_TC`: `bool` indicating whether or not a storm was designated as a tropical cyclone at the `<TCRecordEntry>.entrytime`.
-    - `is_synoptic`: `bool` indicating whether or not an entry occurred at a synoptic time (0Z, 6Z, 12Z, 18Z).
-- Added `report_type` default keyword argument to the `<Season>.stats` method. User can dictate if report prints to the console or gets back a string version of the report.
-- Fixed an exclusion of `maxwind_radius` (formerly called `wind_radii`) from `<TCRecordEntry>.hurdat2()` calls. (which was only introduced in the previous version).
-- Tweaked landfall-disclaimer in `<Season>.stats()` output to reflect the April 2022 release of the Hurdat2 database.
-- Changed `<Season>.__getitem__` method to account for the possibility of merged basin databases, giving the user a choice between mulitple storms that occurred in the same year, but in different geographical basins with shared cyclone numbers. The East Pacific Hurdat2 is an example, natively including storms from the East and Central Pacific Basins.
-- `<TropicalCyclone>.track_map()` tweaks:
-  - focuses on the part of the track where the storm was designated a tropical cyclone.
-  - now fills more of the screen, offering a better user experience, and lessens the likelihood of the user feeling compelled to resize the initial window.
-  - added legend. By default, it will display. But if you'd rather it not display, there is a keyword to turn it off
-  - I believe it may be slightly faster now, thanks to performance tips in matplotlib docs.
-  - map coordinate lists used now significantly smaller.
-- tweaked a very minor syntax quirk. Somewhere in the code I had used `is not` instead of the more-proper `!=`.
-- `basin` tweaks
-  - introduced a new method `<Hurdat2>.basin_abbr()` which returns a list of basin abbreviations used; will be used in report outputs.
-- Fixed memory-location identification in `__repr__` methods
+- Hotfix for `<TCRecordEntry>` vars `previous_entries` and `next_entries`. These vars were introduced in `v2.2`. I thought I had confirmed that they worked, but I was getting issues with trying to call. Fixed now though.
+- small formatting tweak (wasn't throwing errors) of a (mostly) internal method `_season_stats_str`.
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
   - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
```

### Comparing `hurdat2parser-2.2/README.md` & `hurdat2parser-2.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# hurdat2parser -- v2.2
+# hurdat2parser -- v2.2.2
 ---
 ### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
@@ -17,65 +17,18 @@
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
 * [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.2)
+## Changes in this Version (2.2.2)
 
-- Docstring'd `TCRecordEntry` properties
-- Changes to the `<Hurdat2>` object:
-  - when reading-in files on `__init__`, multiple local files are now supported.
-  - enabled download of the most-recent hurdat2 dataset through the `basin` kwarg.
-  - added a `urlcheck` kwarg. If `True`, the "file-path"s listed will be treated like URLs and a download attempt will be made.
-  - removed the `_filesappended` attribute
-  - Searching for notoriously-named storms can be done by a dash (`"-"`) prefix to the search string in addition to an underscore (see [Example Calls](#example-calls) section)
-  - Revamped `output_climo_csv`, `output_season_csv`, and `output_storms_csv` methods
-    - simplified code; updated and unified attributes used in the reports and made it significantly easier for future maintenance.
-  - moved `multi_season_info` method to `_reports`
-- New properties for both `Season` and `TropicalCyclone`:
-  - `duration`
-    - `Season` version reports time between the first and last day of the season (see further in the document for explanation)
-	- `TropicalCyclone` version just reports the track-life in days, regardless of status. More useful status-based duration properties were created too. Keep reading (a few lines down).
-  - `tc_entries` returns a list of `TCRecordEntry`s where a storm was a designated tropical cyclone.
-  - `start_date`, `start_ordinal`, and `end_date`, `end_ordinal` report the starting/ending dates and/or days of the year
-- New `TropicalCyclone` variables:
-  - `ACE_no_landfall`
-  - `duration_<TC, TS, HU, MHU>` - These properties report the aggregate time in days that a tropical cyclone was designated that status or stronger, accounting for fluxuations in storm statuses and strengths.
-  - removed `coord_list` method. It was redundant as it was like a shortened combination of the `summary` method.
-- New `TCRecordEntry` variables:
-  - tweaked how location variables are defined. `location` and `location_reversed` are now properties that depend on the express definition of the variables `lat` and `lon` rather than the other way around.
-  - tweak of not-available wind-extent data. As of the moment typing this, wind-extent data is only provided for storms since 2004. All previous wind-extent data is `-999`, meaning its unavailable. But if a storm has max winds of `<` 64, its Hurricane wind extent has to be 0. So when ingesting the data, this determination is made.
-  - tweaked ingest of data to prevent errors due to possible new Hurdat2 categories introduced in future versions. This was the problem with `v2.1` that was responsible for the need for a `v2.11` release. This particular version wouldn't be able to read-in the new variables in such a situation, but it would still be functional with the newer database (unless order of variables are switched around).
-  - the formerly-called variable `wind_radii` from `v2.11` is now called `maxwind_radius`. I don't know why I called it `radii`, as in plural of radius. I guess it sounded science-y or smart. haha. But the change is also more readable.
-  - Surface Area (coverage)-based variables `areal_extent_TS`, `areal_extent_TS50`, and `areal_extent_HU`.
-    - These are calculated from reported wind-extents in the database.
-  - `track_distance`: the track distance of the cyclone up to the point of the respective entry; this does not account for storm status
-  - `previous_entries` and `next_entries`: lists of the previous and next recorded entries, respectively, in the `TropicalCyclone`'s record
-  - `previous_entry` and `next_entry`: the previous and next recorded entry, respectively, in the `TropicalCyclone`'s record
-  - `direction()`: the `TropicalCyclone`'s heading in degrees (or cardinal, if desired...see docstring)
-  - `speed`: the `TropicalCyclone`'s forward speed in knots.
-  - Properties to simplify coding and reduce probability of coding errors.
-    - `is_TC`: `bool` indicating whether or not a storm was designated as a tropical cyclone at the `<TCRecordEntry>.entrytime`.
-    - `is_synoptic`: `bool` indicating whether or not an entry occurred at a synoptic time (0Z, 6Z, 12Z, 18Z).
-- Added `report_type` default keyword argument to the `<Season>.stats` method. User can dictate if report prints to the console or gets back a string version of the report.
-- Fixed an exclusion of `maxwind_radius` (formerly called `wind_radii`) from `<TCRecordEntry>.hurdat2()` calls. (which was only introduced in the previous version).
-- Tweaked landfall-disclaimer in `<Season>.stats()` output to reflect the April 2022 release of the Hurdat2 database.
-- Changed `<Season>.__getitem__` method to account for the possibility of merged basin databases, giving the user a choice between mulitple storms that occurred in the same year, but in different geographical basins with shared cyclone numbers. The East Pacific Hurdat2 is an example, natively including storms from the East and Central Pacific Basins.
-- `<TropicalCyclone>.track_map()` tweaks:
-  - focuses on the part of the track where the storm was designated a tropical cyclone.
-  - now fills more of the screen, offering a better user experience, and lessens the likelihood of the user feeling compelled to resize the initial window.
-  - added legend. By default, it will display. But if you'd rather it not display, there is a keyword to turn it off
-  - I believe it may be slightly faster now, thanks to performance tips in matplotlib docs.
-  - map coordinate lists used now significantly smaller.
-- tweaked a very minor syntax quirk. Somewhere in the code I had used `is not` instead of the more-proper `!=`.
-- `basin` tweaks
-  - introduced a new method `<Hurdat2>.basin_abbr()` which returns a list of basin abbreviations used; will be used in report outputs.
-- Fixed memory-location identification in `__repr__` methods
+- Hotfix for `<TCRecordEntry>` vars `previous_entries` and `next_entries`. These vars were introduced in `v2.2`. I thought I had confirmed that they worked, but I was getting issues with trying to call. Fixed now though.
+- small formatting tweak (wasn't throwing errors) of a (mostly) internal method `_season_stats_str`.
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
   - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
```

### Comparing `hurdat2parser-2.2/hurdat2parser/__init__.py` & `hurdat2parser-2.2.2/hurdat2parser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""hurdat2parser v2.2
+"""hurdat2parser v2.2.2
 
 https://github.com/ksgwxfan/hurdat2parser
 
 hurdat2parser v2.x is provides a convenient access to interpret and work with
 tropical cyclone data that is contained in a widely-used and updated dataset,
 HURDAT2 (https://www.nhc.noaa.gov/data/#hurdat). The purpose of this module is to
 provide a quick way to investigate HURDAT2 data. It includes methods for
@@ -1327,15 +1327,15 @@
 
     @property
     def previous_entries(self):
         """
         Returns a list of preceding <TCRecordEntry>s in the parent
         <TropicalCyclone>.entry list.
         """
-        return self._tc[0:self._tc.entry.index(self)]
+        return self._tc.entry[0:self._tc.entry.index(self)]
 
     @property
     def previous_entry(self):
         """
         Returns the <TCRecordEntry> that occurred PREVIOUS (preceding this
         entry) in the parent <TropicalCyclone>.entry list. Returns None if it
         is the first index (index 0).
@@ -1347,15 +1347,15 @@
 
     @property
     def next_entries(self):
         """
         Returns a list of succeeding <TCRecordEntry>s in the parent
         <TropicalCyclone>.entry list.
         """
-        return self._tc[self._tc.entry.index(self)+1:]
+        return self._tc.entry[self._tc.entry.index(self)+1:]
 
     @property
     def next_entry(self):
         """
         Returns the <TCRecordEntry> that occurs NEXT (following this entry) in
         the parent <TropicalCyclone>.entry list. Returns None if it is the last
         entry.
```

### Comparing `hurdat2parser-2.2/hurdat2parser/_aliases.py` & `hurdat2parser-2.2.2/hurdat2parser/_aliases.py`

 * *Files identical despite different names*

### Comparing `hurdat2parser-2.2/hurdat2parser/_calculations.py` & `hurdat2parser-2.2.2/hurdat2parser/_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,38 +813,36 @@
             if current_rank is not None and current_rank not in printedqty:
                 printedqty.append(current_rank)
         print("")
 
     def _season_stats_str(self, seasonreq, year1, year2, rstart, rthru, width, **kw):
         strlist = []
         yr = seasonreq
-        strlist.append("\n")
         strlist.append("-" * width)
         strlist.append("Tropical Cyclone Stats for {}".format(yr).center(width))
         strlist.append(
             "{}{}".format(
                 self.basin(),
                 ""
             ).center(width)
         )
         strlist[-1] += "\n"
-        for line in textwrap.wrap(
-            "Stats calculated for Seasons {}".format(
-                "{}-{}".format(
-                    year1,
-                    year2
-                ) if year2 != self.record_range[1] \
-                else "since {} ({} total seasons)".format(
-                    year1,
-                    self.record_range[1] - year1 + 1
-                )
-            ),
-            width,
-        ):
-            strlist.append(line)
+
+        statyrline = "Stats calculated for Seasons {}".format(
+            "{}-{}".format(
+                year1,
+                year2
+            ) if year2 != self.record_range[1] \
+            else "since {} ({} total seasons)".format(
+                year1,
+                self.record_range[1] - year1 + 1
+            )
+        ).center(width)
+        strlist.append(statyrline)
+
         if rstart != (1,1) or rthru != (12,31):
             strlist.append(
                 "from {} thru {}".format(
                     "{} {}".format(
                         calendar.month_name[rstart[0]],
                         rstart[1],
                     ),
```

### Comparing `hurdat2parser-2.2/hurdat2parser/_future.py` & `hurdat2parser-2.2.2/hurdat2parser/_future.py`

 * *Files identical despite different names*

### Comparing `hurdat2parser-2.2/hurdat2parser/_maps.py` & `hurdat2parser-2.2.2/hurdat2parser/_maps.py`

 * *Files identical despite different names*

### Comparing `hurdat2parser-2.2/hurdat2parser/_reports.py` & `hurdat2parser-2.2.2/hurdat2parser/_reports.py`

 * *Files identical despite different names*

### Comparing `hurdat2parser-2.2/hurdat2parser.egg-info/PKG-INFO` & `hurdat2parser-2.2.2/hurdat2parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hurdat2parser
-Version: 2.2
+Version: 2.2.2
 Summary: Interpret Hurricane Data contained in HURDAT2
 Home-page: http://github.com/ksgwxfan/hurdat2parser
 Author: Kyle S. Gentry
 Author-email: KyleSGentry@outlook.com
 License: MIT
 Keywords: hurricane hurdat2 meteorology weather
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# hurdat2parser -- v2.2
+# hurdat2parser -- v2.2.2
 ---
 ### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
@@ -34,65 +34,18 @@
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
 * [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.2)
+## Changes in this Version (2.2.2)
 
-- Docstring'd `TCRecordEntry` properties
-- Changes to the `<Hurdat2>` object:
-  - when reading-in files on `__init__`, multiple local files are now supported.
-  - enabled download of the most-recent hurdat2 dataset through the `basin` kwarg.
-  - added a `urlcheck` kwarg. If `True`, the "file-path"s listed will be treated like URLs and a download attempt will be made.
-  - removed the `_filesappended` attribute
-  - Searching for notoriously-named storms can be done by a dash (`"-"`) prefix to the search string in addition to an underscore (see [Example Calls](#example-calls) section)
-  - Revamped `output_climo_csv`, `output_season_csv`, and `output_storms_csv` methods
-    - simplified code; updated and unified attributes used in the reports and made it significantly easier for future maintenance.
-  - moved `multi_season_info` method to `_reports`
-- New properties for both `Season` and `TropicalCyclone`:
-  - `duration`
-    - `Season` version reports time between the first and last day of the season (see further in the document for explanation)
-	- `TropicalCyclone` version just reports the track-life in days, regardless of status. More useful status-based duration properties were created too. Keep reading (a few lines down).
-  - `tc_entries` returns a list of `TCRecordEntry`s where a storm was a designated tropical cyclone.
-  - `start_date`, `start_ordinal`, and `end_date`, `end_ordinal` report the starting/ending dates and/or days of the year
-- New `TropicalCyclone` variables:
-  - `ACE_no_landfall`
-  - `duration_<TC, TS, HU, MHU>` - These properties report the aggregate time in days that a tropical cyclone was designated that status or stronger, accounting for fluxuations in storm statuses and strengths.
-  - removed `coord_list` method. It was redundant as it was like a shortened combination of the `summary` method.
-- New `TCRecordEntry` variables:
-  - tweaked how location variables are defined. `location` and `location_reversed` are now properties that depend on the express definition of the variables `lat` and `lon` rather than the other way around.
-  - tweak of not-available wind-extent data. As of the moment typing this, wind-extent data is only provided for storms since 2004. All previous wind-extent data is `-999`, meaning its unavailable. But if a storm has max winds of `<` 64, its Hurricane wind extent has to be 0. So when ingesting the data, this determination is made.
-  - tweaked ingest of data to prevent errors due to possible new Hurdat2 categories introduced in future versions. This was the problem with `v2.1` that was responsible for the need for a `v2.11` release. This particular version wouldn't be able to read-in the new variables in such a situation, but it would still be functional with the newer database (unless order of variables are switched around).
-  - the formerly-called variable `wind_radii` from `v2.11` is now called `maxwind_radius`. I don't know why I called it `radii`, as in plural of radius. I guess it sounded science-y or smart. haha. But the change is also more readable.
-  - Surface Area (coverage)-based variables `areal_extent_TS`, `areal_extent_TS50`, and `areal_extent_HU`.
-    - These are calculated from reported wind-extents in the database.
-  - `track_distance`: the track distance of the cyclone up to the point of the respective entry; this does not account for storm status
-  - `previous_entries` and `next_entries`: lists of the previous and next recorded entries, respectively, in the `TropicalCyclone`'s record
-  - `previous_entry` and `next_entry`: the previous and next recorded entry, respectively, in the `TropicalCyclone`'s record
-  - `direction()`: the `TropicalCyclone`'s heading in degrees (or cardinal, if desired...see docstring)
-  - `speed`: the `TropicalCyclone`'s forward speed in knots.
-  - Properties to simplify coding and reduce probability of coding errors.
-    - `is_TC`: `bool` indicating whether or not a storm was designated as a tropical cyclone at the `<TCRecordEntry>.entrytime`.
-    - `is_synoptic`: `bool` indicating whether or not an entry occurred at a synoptic time (0Z, 6Z, 12Z, 18Z).
-- Added `report_type` default keyword argument to the `<Season>.stats` method. User can dictate if report prints to the console or gets back a string version of the report.
-- Fixed an exclusion of `maxwind_radius` (formerly called `wind_radii`) from `<TCRecordEntry>.hurdat2()` calls. (which was only introduced in the previous version).
-- Tweaked landfall-disclaimer in `<Season>.stats()` output to reflect the April 2022 release of the Hurdat2 database.
-- Changed `<Season>.__getitem__` method to account for the possibility of merged basin databases, giving the user a choice between mulitple storms that occurred in the same year, but in different geographical basins with shared cyclone numbers. The East Pacific Hurdat2 is an example, natively including storms from the East and Central Pacific Basins.
-- `<TropicalCyclone>.track_map()` tweaks:
-  - focuses on the part of the track where the storm was designated a tropical cyclone.
-  - now fills more of the screen, offering a better user experience, and lessens the likelihood of the user feeling compelled to resize the initial window.
-  - added legend. By default, it will display. But if you'd rather it not display, there is a keyword to turn it off
-  - I believe it may be slightly faster now, thanks to performance tips in matplotlib docs.
-  - map coordinate lists used now significantly smaller.
-- tweaked a very minor syntax quirk. Somewhere in the code I had used `is not` instead of the more-proper `!=`.
-- `basin` tweaks
-  - introduced a new method `<Hurdat2>.basin_abbr()` which returns a list of basin abbreviations used; will be used in report outputs.
-- Fixed memory-location identification in `__repr__` methods
+- Hotfix for `<TCRecordEntry>` vars `previous_entries` and `next_entries`. These vars were introduced in `v2.2`. I thought I had confirmed that they worked, but I was getting issues with trying to call. Fixed now though.
+- small formatting tweak (wasn't throwing errors) of a (mostly) internal method `_season_stats_str`.
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
   - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
```

### Comparing `hurdat2parser-2.2/setup.py` & `hurdat2parser-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
  
 with open("README.md", "r") as fh: 
     readme = fh.read() 
 
 setup(
     name = 'hurdat2parser',
-    version = '2.2',
+    version = '2.2.2',
     author = 'Kyle S. Gentry',
     author_email = 'KyleSGentry@outlook.com',
     url = 'http://github.com/ksgwxfan/hurdat2parser',
     description = 'Interpret Hurricane Data contained in HURDAT2',
     long_description = readme,
     long_description_content_type = "text/markdown",
     license = 'MIT',
```

