# Comparing `tmp/leeger-2.3.0.tar.gz` & `tmp/leeger-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leeger-2.3.0.tar", last modified: Mon May  1 04:01:37 2023, max compression
+gzip compressed data, was "leeger-2.4.0.tar", last modified: Mon May 15 00:40:21 2023, max compression
```

## Comparing `leeger-2.3.0.tar` & `leeger-2.4.0.tar`

### file list

```diff
@@ -1,207 +1,209 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.957072 leeger-2.3.0/
--rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.3.0/LICENSE
--rw-rw-rw-   0        0        0       24 2022-10-18 21:57:01.000000 leeger-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9659 2023-05-01 04:01:37.956072 leeger-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9248 2023-04-20 22:48:13.000000 leeger-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.580071 leeger-2.3.0/leeger/
--rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.3.0/leeger/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-01 04:00:10.000000 leeger-2.3.0/leeger/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.620071 leeger-2.3.0/leeger/calculator/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.3.0/leeger/calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.648074 leeger-2.3.0/leeger/calculator/all_time_calculator/
--rw-rw-rw-   0        0        0     5029 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9107 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1318 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0     4490 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9364 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9000 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0     2644 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0     3351 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0     8906 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1519 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
--rw-rw-rw-   0        0        0      712 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/all_time_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.659073 leeger-2.3.0/leeger/calculator/parent/
--rw-rw-rw-   0        0        0    15345 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/parent/AllTimeCalculator.py
--rw-rw-rw-   0        0        0     1671 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/parent/YearCalculator.py
--rw-rw-rw-   0        0        0       94 2022-08-13 05:45:45.000000 leeger-2.3.0/leeger/calculator/parent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.706074 leeger-2.3.0/leeger/calculator/year_calculator/
--rw-rw-rw-   0        0        0     9896 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/AWALYearCalculator.py
--rw-rw-rw-   0        0        0    18719 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     2018 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0     5843 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0     6208 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/SSLYearCalculator.py
--rw-rw-rw-   0        0        0     8945 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0     2396 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0     2973 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0     8392 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0     1699 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
--rw-rw-rw-   0        0        0      652 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/calculator/year_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.712072 leeger-2.3.0/leeger/decorator/
--rw-rw-rw-   0        0        0       85 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/decorator/__init__.py
--rw-rw-rw-   0        0        0     4853 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/decorator/validators.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.738072 leeger-2.3.0/leeger/enum/
--rw-rw-rw-   0        0        0      784 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/enum/MatchupType.py
--rw-rw-rw-   0        0        0       38 2022-09-29 19:44:58.000000 leeger-2.3.0/leeger/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.874073 leeger-2.3.0/leeger/exception/
--rw-rw-rw-   0        0        0      157 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/DoesNotExistException.py
--rw-rw-rw-   0        0        0      117 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidFilterException.py
--rw-rw-rw-   0        0        0      138 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidLeagueFormatException.py
--rw-rw-rw-   0        0        0      140 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidMatchupFormatException.py
--rw-rw-rw-   0        0        0      137 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidOwnerFormatException.py
--rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidTeamFormatException.py
--rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidWeekFormatException.py
--rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/exception/InvalidYearFormatException.py
--rw-rw-rw-   0        0        0      150 2022-10-16 01:33:13.000000 leeger-2.3.0/leeger/exception/InvalidYearSettingsFormatException.py
--rw-rw-rw-   0        0        0      126 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/exception/LeagueLoaderException.py
--rw-rw-rw-   0        0        0      136 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/exception/UnsupportedLeegerFeatureException.py
--rw-rw-rw-   0        0        0      762 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.897071 leeger-2.3.0/leeger/league_loader/
--rw-rw-rw-   0        0        0     8804 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/league_loader/ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0     7720 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/league_loader/FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0     2606 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/league_loader/LeagueLoader.py
--rw-rw-rw-   0        0        0    13103 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0    16345 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/league_loader/SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0    11236 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/league_loader/YahooLeagueLoader.py
--rw-rw-rw-   0        0        0      222 2022-08-08 20:13:25.000000 leeger-2.3.0/leeger/league_loader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.900070 leeger-2.3.0/leeger/model/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.3.0/leeger/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.912078 leeger-2.3.0/leeger/model/abstract/
--rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.3.0/leeger/model/abstract/UniqueId.py
--rw-rw-rw-   0        0        0       32 2022-08-13 05:49:03.000000 leeger-2.3.0/leeger/model/abstract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.921073 leeger-2.3.0/leeger/model/filter/
--rw-rw-rw-   0        0        0     5463 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/model/filter/AllTimeFilters.py
--rw-rw-rw-   0        0        0      321 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/model/filter/WeekFilters.py
--rw-rw-rw-   0        0        0     5200 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/model/filter/YearFilters.py
--rw-rw-rw-   0        0        0      120 2022-09-17 18:26:39.000000 leeger-2.3.0/leeger/model/filter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.982075 leeger-2.3.0/leeger/model/league/
--rw-rw-rw-   0        0        0     5605 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/model/league/League.py
--rw-rw-rw-   0        0        0     4753 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/model/league/Matchup.py
--rw-rw-rw-   0        0        0      843 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/model/league/Owner.py
--rw-rw-rw-   0        0        0     1348 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/model/league/Team.py
--rw-rw-rw-   0        0        0     2811 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/model/league/Week.py
--rw-rw-rw-   0        0        0     2857 2023-05-01 03:59:36.000000 leeger-2.3.0/leeger/model/league/Year.py
--rw-rw-rw-   0        0        0      975 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/model/league/YearSettings.py
--rw-rw-rw-   0        0        0      196 2022-10-16 01:33:13.000000 leeger-2.3.0/leeger/model/league/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.995072 leeger-2.3.0/leeger/model/league_helper/
--rw-rw-rw-   0        0        0     3711 2023-04-30 18:12:34.000000 leeger-2.3.0/leeger/model/league_helper/Performance.py
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.3.0/leeger/model/league_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.002071 leeger-2.3.0/leeger/model/stat/
--rw-rw-rw-   0        0        0     3880 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/model/stat/AllTimeStatSheet.py
--rw-rw-rw-   0        0        0     4126 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/model/stat/YearStatSheet.py
--rw-rw-rw-   0        0        0       90 2022-08-13 05:49:50.000000 leeger-2.3.0/leeger/model/stat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.109071 leeger-2.3.0/leeger/util/
--rw-rw-rw-   0        0        0     1114 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/util/CustomFormatter.py
--rw-rw-rw-   0        0        0      889 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/util/CustomLogger.py
--rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.3.0/leeger/util/Deci.py
--rw-rw-rw-   0        0        0     1426 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/util/GeneralUtil.py
--rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.3.0/leeger/util/IdGenerator.py
--rw-rw-rw-   0        0        0      310 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/util/JSONDeserializable.py
--rw-rw-rw-   0        0        0      276 2023-04-29 23:36:04.000000 leeger-2.3.0/leeger/util/JSONSerializable.py
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.3.0/leeger/util/__init__.py
--rw-rw-rw-   0        0        0    14428 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/util/excel.py
--rw-rw-rw-   0        0        0     9027 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/util/excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.162071 leeger-2.3.0/leeger/util/navigator/
--rw-rw-rw-   0        0        0     5682 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/util/navigator/LeagueNavigator.py
--rw-rw-rw-   0        0        0     2071 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/util/navigator/MatchupNavigator.py
--rw-rw-rw-   0        0        0     2207 2023-04-29 23:41:27.000000 leeger-2.3.0/leeger/util/navigator/WeekNavigator.py
--rw-rw-rw-   0        0        0     6659 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/util/navigator/YearNavigator.py
--rw-rw-rw-   0        0        0      178 2022-12-31 03:44:14.000000 leeger-2.3.0/leeger/util/navigator/__init__.py
--rw-rw-rw-   0        0        0    11436 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/util/stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.231070 leeger-2.3.0/leeger/validate/
--rw-rw-rw-   0        0        0      258 2022-08-13 06:01:19.000000 leeger-2.3.0/leeger/validate/__init__.py
--rw-rw-rw-   0        0        0     4326 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/validate/leagueValidation.py
--rw-rw-rw-   0        0        0     2481 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/validate/matchupValidation.py
--rw-rw-rw-   0        0        0      493 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/validate/ownerValidation.py
--rw-rw-rw-   0        0        0      598 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/validate/teamValidation.py
--rw-rw-rw-   0        0        0     4686 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/validate/weekValidation.py
--rw-rw-rw-   0        0        0      231 2023-02-17 19:20:27.000000 leeger-2.3.0/leeger/validate/yearSettingsValidation.py
--rw-rw-rw-   0        0        0    13564 2023-04-29 23:41:28.000000 leeger-2.3.0/leeger/validate/yearValidation.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.618070 leeger-2.3.0/leeger.egg-info/
--rw-rw-rw-   0        0        0     9659 2023-05-01 04:01:36.000000 leeger-2.3.0/leeger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7779 2023-05-01 04:01:36.000000 leeger-2.3.0/leeger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 04:01:36.000000 leeger-2.3.0/leeger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-05-01 04:01:36.000000 leeger-2.3.0/leeger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 04:01:36.000000 leeger-2.3.0/leeger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-13 04:26:54.000000 leeger-2.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 04:01:37.958076 leeger-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-04-29 23:41:28.000000 leeger-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:36.557070 leeger-2.3.0/test/
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.234074 leeger-2.3.0/test/test_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.3.0/test/test_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.371071 leeger-2.3.0/test/test_calculator/test_all_time_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/__init__.py
--rw-rw-rw-   0        0        0    86146 2023-04-29 23:41:33.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0   220423 2023-04-29 23:41:38.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0    24301 2023-04-29 23:41:29.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0    96680 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0    42298 2023-04-29 23:41:30.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0   107979 2023-04-29 23:41:35.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0    27851 2023-04-29 23:41:29.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0    47446 2023-04-29 23:41:31.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0   103504 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0    54546 2023-04-29 23:41:32.000000 leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.516069 leeger-2.3.0/test/test_calculator/test_year_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/__init__.py
--rw-rw-rw-   0        0        0   104455 2023-04-29 23:41:35.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
--rw-rw-rw-   0        0        0    84963 2023-04-29 23:41:33.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     9711 2023-04-29 23:41:30.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0    39044 2023-04-29 23:41:31.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0    29836 2023-04-29 23:41:33.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
--rw-rw-rw-   0        0        0    44383 2023-04-29 23:41:32.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0    12194 2023-04-29 23:41:31.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0    35141 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0    82020 2023-04-29 23:41:36.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0    21748 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.531072 leeger-2.3.0/test/test_decorator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.3.0/test/test_decorator/__init__.py
--rw-rw-rw-   0        0        0     4803 2023-04-29 23:41:33.000000 leeger-2.3.0/test/test_decorator/test_validators.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.583075 leeger-2.3.0/test/test_league_loader/
--rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.3.0/test/test_league_loader/__init__.py
--rw-rw-rw-   0        0        0    18765 2023-05-01 03:59:36.000000 leeger-2.3.0/test/test_league_loader/test_ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0      443 2023-04-30 18:26:27.000000 leeger-2.3.0/test/test_league_loader/test_FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0      949 2023-04-30 18:25:27.000000 leeger-2.3.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0      732 2023-04-30 18:25:36.000000 leeger-2.3.0/test/test_league_loader/test_SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0     1528 2023-04-30 18:25:44.000000 leeger-2.3.0/test/test_league_loader/test_YahooLeagueLoader.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.586071 leeger-2.3.0/test/test_model/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.3.0/test/test_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.602072 leeger-2.3.0/test/test_model/test_abstract/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.3.0/test/test_model/test_abstract/__init__.py
--rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.3.0/test/test_model/test_abstract/test_UniqueId.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.619073 leeger-2.3.0/test/test_model/test_filter/
--rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.3.0/test/test_model/test_filter/__init__.py
--rw-rw-rw-   0        0        0     2098 2023-04-29 23:41:33.000000 leeger-2.3.0/test/test_model/test_filter/test_AllTimeFilters.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.721084 leeger-2.3.0/test/test_model/test_league/
--rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.3.0/test/test_model/test_league/__init__.py
--rw-rw-rw-   0        0        0    22224 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_model/test_league/test_League.py
--rw-rw-rw-   0        0        0     8360 2023-04-29 23:41:33.000000 leeger-2.3.0/test/test_model/test_league/test_Matchup.py
--rw-rw-rw-   0        0        0     1136 2023-02-17 19:28:57.000000 leeger-2.3.0/test/test_model/test_league/test_Owner.py
--rw-rw-rw-   0        0        0     1219 2023-02-17 19:29:31.000000 leeger-2.3.0/test/test_model/test_league/test_Team.py
--rw-rw-rw-   0        0        0     9659 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_model/test_league/test_Week.py
--rw-rw-rw-   0        0        0     8823 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_model/test_league/test_Year.py
--rw-rw-rw-   0        0        0     1487 2023-02-17 19:34:39.000000 leeger-2.3.0/test/test_model/test_league/test_YearSettings.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.737073 leeger-2.3.0/test/test_model/test_league_helper/
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.3.0/test/test_model/test_league_helper/__init__.py
--rw-rw-rw-   0        0        0     6294 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_model/test_league_helper/test_Performance.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.806069 leeger-2.3.0/test/test_util/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.3.0/test/test_util/__init__.py
--rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.3.0/test/test_util/test_Deci.py
--rw-rw-rw-   0        0        0     1375 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_util/test_GeneralUtil.py
--rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.3.0/test/test_util/test_IdGenerator.py
--rw-rw-rw-   0        0        0    64759 2023-04-29 23:41:36.000000 leeger-2.3.0/test/test_util/test_excel.py
--rw-rw-rw-   0        0        0     7246 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_util/test_excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.859073 leeger-2.3.0/test/test_util/test_navigator/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.3.0/test/test_util/test_navigator/__init__.py
--rw-rw-rw-   0        0        0    52517 2023-04-29 23:41:36.000000 leeger-2.3.0/test/test_util/test_navigator/test_LeagueNavigator.py
--rw-rw-rw-   0        0        0     3970 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_util/test_navigator/test_MatchupNavigator.py
--rw-rw-rw-   0        0        0     6154 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_util/test_navigator/test_WeekNavigator.py
--rw-rw-rw-   0        0        0    27730 2023-04-29 23:41:35.000000 leeger-2.3.0/test/test_util/test_navigator/test_YearNavigator.py
--rw-rw-rw-   0        0        0    10570 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_util/test_stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:01:37.951077 leeger-2.3.0/test/test_validate/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.3.0/test/test_validate/__init__.py
--rw-rw-rw-   0        0        0     8903 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_validate/test_leagueValidation.py
--rw-rw-rw-   0        0        0     4772 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_validate/test_matchupValidation.py
--rw-rw-rw-   0        0        0      530 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_validate/test_ownerValidation.py
--rw-rw-rw-   0        0        0      838 2023-04-29 23:41:34.000000 leeger-2.3.0/test/test_validate/test_teamValidation.py
--rw-rw-rw-   0        0        0     6094 2023-04-29 23:41:35.000000 leeger-2.3.0/test/test_validate/test_weekValidation.py
--rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.3.0/test/test_validate/test_yearSettingsValidation.py
--rw-rw-rw-   0        0        0    25513 2023-04-29 23:41:35.000000 leeger-2.3.0/test/test_validate/test_yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.787891 leeger-2.4.0/
+-rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-10-18 21:57:01.000000 leeger-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9943 2023-05-15 00:40:21.784891 leeger-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9532 2023-05-15 00:38:33.000000 leeger-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.902387 leeger-2.4.0/leeger/
+-rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.4.0/leeger/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-15 00:39:59.000000 leeger-2.4.0/leeger/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.956388 leeger-2.4.0/leeger/calculator/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.4.0/leeger/calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.990387 leeger-2.4.0/leeger/calculator/all_time_calculator/
+-rw-rw-rw-   0        0        0     5029 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9107 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1318 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     4490 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9320 2023-05-11 04:31:22.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8996 2023-05-11 04:31:22.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     2644 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     3351 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8906 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1519 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
+-rw-rw-rw-   0        0        0      712 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.998386 leeger-2.4.0/leeger/calculator/parent/
+-rw-rw-rw-   0        0        0    15345 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/parent/AllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1671 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/parent/YearCalculator.py
+-rw-rw-rw-   0        0        0       94 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/calculator/parent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.044388 leeger-2.4.0/leeger/calculator/year_calculator/
+-rw-rw-rw-   0        0        0     9896 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/year_calculator/AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    18719 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     2018 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0     5843 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0     6208 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/year_calculator/SSLYearCalculator.py
+-rw-rw-rw-   0        0        0     8945 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0     2973 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0     8392 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0     1699 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
+-rw-rw-rw-   0        0        0      652 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/calculator/year_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.050393 leeger-2.4.0/leeger/decorator/
+-rw-rw-rw-   0        0        0       85 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/decorator/__init__.py
+-rw-rw-rw-   0        0        0     4853 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/decorator/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.055391 leeger-2.4.0/leeger/enum/
+-rw-rw-rw-   0        0        0      784 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/enum/MatchupType.py
+-rw-rw-rw-   0        0        0       38 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.125389 leeger-2.4.0/leeger/exception/
+-rw-rw-rw-   0        0        0      145 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/DoesNotExistException.py
+-rw-rw-rw-   0        0        0      105 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidFilterException.py
+-rw-rw-rw-   0        0        0      126 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidLeagueFormatException.py
+-rw-rw-rw-   0        0        0      128 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidMatchupFormatException.py
+-rw-rw-rw-   0        0        0      125 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidOwnerFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidTeamFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidWeekFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidYearFormatException.py
+-rw-rw-rw-   0        0        0      138 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidYearSettingsFormatException.py
+-rw-rw-rw-   0        0        0      126 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/exception/LeagueLoaderException.py
+-rw-rw-rw-   0        0        0      136 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/exception/UnsupportedLeegerFeatureException.py
+-rw-rw-rw-   0        0        0      762 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.221579 leeger-2.4.0/leeger/league_loader/
+-rw-rw-rw-   0        0        0     9195 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0     8032 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     4632 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/LeagueLoader.py
+-rw-rw-rw-   0        0        0    11954 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0    19866 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    11528 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/YahooLeagueLoader.py
+-rw-rw-rw-   0        0        0      222 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/league_loader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.226579 leeger-2.4.0/leeger/model/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.4.0/leeger/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.232577 leeger-2.4.0/leeger/model/abstract/
+-rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.4.0/leeger/model/abstract/UniqueId.py
+-rw-rw-rw-   0        0        0       32 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/abstract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.346576 leeger-2.4.0/leeger/model/filter/
+-rw-rw-rw-   0        0        0     5463 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/model/filter/AllTimeFilters.py
+-rw-rw-rw-   0        0        0      321 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/model/filter/WeekFilters.py
+-rw-rw-rw-   0        0        0     5200 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/model/filter/YearFilters.py
+-rw-rw-rw-   0        0        0      120 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/filter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.472580 leeger-2.4.0/leeger/model/league/
+-rw-rw-rw-   0        0        0     6088 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/League.py
+-rw-rw-rw-   0        0        0     5276 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Matchup.py
+-rw-rw-rw-   0        0        0     1347 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Owner.py
+-rw-rw-rw-   0        0        0     1689 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Team.py
+-rw-rw-rw-   0        0        0     3290 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Week.py
+-rw-rw-rw-   0        0        0     3336 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Year.py
+-rw-rw-rw-   0        0        0     1493 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/YearSettings.py
+-rw-rw-rw-   0        0        0      196 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/league/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.527578 leeger-2.4.0/leeger/model/league_helper/
+-rw-rw-rw-   0        0        0     3711 2023-04-30 18:12:34.000000 leeger-2.4.0/leeger/model/league_helper/Performance.py
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.4.0/leeger/model/league_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.690577 leeger-2.4.0/leeger/model/stat/
+-rw-rw-rw-   0        0        0     3880 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/model/stat/AllTimeStatSheet.py
+-rw-rw-rw-   0        0        0     4126 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/model/stat/YearStatSheet.py
+-rw-rw-rw-   0        0        0       90 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/stat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.844576 leeger-2.4.0/leeger/util/
+-rw-rw-rw-   0        0        0     1114 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/util/CustomFormatter.py
+-rw-rw-rw-   0        0        0      889 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/util/CustomLogger.py
+-rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.4.0/leeger/util/Deci.py
+-rw-rw-rw-   0        0        0     4056 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/util/GeneralUtil.py
+-rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.4.0/leeger/util/IdGenerator.py
+-rw-rw-rw-   0        0        0      296 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/util/JSONDeserializable.py
+-rw-rw-rw-   0        0        0      262 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/util/JSONSerializable.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.4.0/leeger/util/__init__.py
+-rw-rw-rw-   0        0        0    14428 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/util/excel.py
+-rw-rw-rw-   0        0        0     9027 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.117581 leeger-2.4.0/leeger/util/navigator/
+-rw-rw-rw-   0        0        0     5682 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/util/navigator/LeagueNavigator.py
+-rw-rw-rw-   0        0        0     2071 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/navigator/MatchupNavigator.py
+-rw-rw-rw-   0        0        0     2207 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/util/navigator/WeekNavigator.py
+-rw-rw-rw-   0        0        0     6659 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/navigator/YearNavigator.py
+-rw-rw-rw-   0        0        0      178 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/util/navigator/__init__.py
+-rw-rw-rw-   0        0        0    11436 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.147579 leeger-2.4.0/leeger/validate/
+-rw-rw-rw-   0        0        0      258 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/validate/__init__.py
+-rw-rw-rw-   0        0        0     4326 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/leagueValidation.py
+-rw-rw-rw-   0        0        0     2481 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/matchupValidation.py
+-rw-rw-rw-   0        0        0      493 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/ownerValidation.py
+-rw-rw-rw-   0        0        0      598 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/teamValidation.py
+-rw-rw-rw-   0        0        0     4686 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/weekValidation.py
+-rw-rw-rw-   0        0        0      221 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/validate/yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    13562 2023-05-11 04:31:22.000000 leeger-2.4.0/leeger/validate/yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.951388 leeger-2.4.0/leeger.egg-info/
+-rw-rw-rw-   0        0        0     9943 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7839 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      203 2023-05-15 00:38:33.000000 leeger-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      147 2023-04-13 04:26:54.000000 leeger-2.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 00:40:21.787891 leeger-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-04-29 23:41:28.000000 leeger-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.618668 leeger-2.4.0/test/
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.157575 leeger-2.4.0/test/test_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.763893 leeger-2.4.0/test/test_calculator/test_all_time_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/__init__.py
+-rw-rw-rw-   0        0        0    86146 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   220423 2023-04-29 23:41:38.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    24301 2023-04-29 23:41:29.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    96680 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    42298 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   107979 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    27851 2023-04-29 23:41:29.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    47446 2023-04-29 23:41:31.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   103504 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    54546 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.885892 leeger-2.4.0/test/test_calculator/test_year_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/__init__.py
+-rw-rw-rw-   0        0        0   104455 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    84963 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     9711 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0    39044 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0    29836 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
+-rw-rw-rw-   0        0        0    44383 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0    12194 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0    35141 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0    82020 2023-04-29 23:41:36.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0    21748 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.891891 leeger-2.4.0/test/test_decorator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_decorator/__init__.py
+-rw-rw-rw-   0        0        0     4803 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_decorator/test_validators.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.346892 leeger-2.4.0/test/test_league_loader/
+-rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.4.0/test/test_league_loader/__init__.py
+-rw-rw-rw-   0        0        0    36769 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0    38840 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     6530 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_LeagueLoader.py
+-rw-rw-rw-   0        0        0    69702 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0   112178 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    49966 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_YahooLeagueLoader.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.349891 leeger-2.4.0/test/test_model/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.353891 leeger-2.4.0/test/test_model/test_abstract/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_model/test_abstract/__init__.py
+-rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.4.0/test/test_model/test_abstract/test_UniqueId.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.361893 leeger-2.4.0/test/test_model/test_filter/
+-rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.4.0/test/test_model/test_filter/__init__.py
+-rw-rw-rw-   0        0        0     2098 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_model/test_filter/test_AllTimeFilters.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.391894 leeger-2.4.0/test/test_model/test_league/
+-rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.4.0/test/test_model/test_league/__init__.py
+-rw-rw-rw-   0        0        0    22224 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_model/test_league/test_League.py
+-rw-rw-rw-   0        0        0     8360 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_model/test_league/test_Matchup.py
+-rw-rw-rw-   0        0        0     1136 2023-02-17 19:28:57.000000 leeger-2.4.0/test/test_model/test_league/test_Owner.py
+-rw-rw-rw-   0        0        0     1219 2023-02-17 19:29:31.000000 leeger-2.4.0/test/test_model/test_league/test_Team.py
+-rw-rw-rw-   0        0        0     9659 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_model/test_league/test_Week.py
+-rw-rw-rw-   0        0        0     8823 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_model/test_league/test_Year.py
+-rw-rw-rw-   0        0        0     1487 2023-02-17 19:34:39.000000 leeger-2.4.0/test/test_model/test_league/test_YearSettings.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.397895 leeger-2.4.0/test/test_model/test_league_helper/
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.4.0/test/test_model/test_league_helper/__init__.py
+-rw-rw-rw-   0        0        0     6294 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_model/test_league_helper/test_Performance.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.420895 leeger-2.4.0/test/test_util/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_util/__init__.py
+-rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.4.0/test/test_util/test_Deci.py
+-rw-rw-rw-   0        0        0     8493 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_util/test_GeneralUtil.py
+-rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.4.0/test/test_util/test_IdGenerator.py
+-rw-rw-rw-   0        0        0    64757 2023-05-11 04:31:22.000000 leeger-2.4.0/test/test_util/test_excel.py
+-rw-rw-rw-   0        0        0     7246 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.610893 leeger-2.4.0/test/test_util/test_navigator/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.4.0/test/test_util/test_navigator/__init__.py
+-rw-rw-rw-   0        0        0    52517 2023-04-29 23:41:36.000000 leeger-2.4.0/test/test_util/test_navigator/test_LeagueNavigator.py
+-rw-rw-rw-   0        0        0     3970 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_navigator/test_MatchupNavigator.py
+-rw-rw-rw-   0        0        0     6154 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_navigator/test_WeekNavigator.py
+-rw-rw-rw-   0        0        0    27730 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_util/test_navigator/test_YearNavigator.py
+-rw-rw-rw-   0        0        0    10570 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.737893 leeger-2.4.0/test/test_validate/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.4.0/test/test_validate/__init__.py
+-rw-rw-rw-   0        0        0     8903 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_validate/test_leagueValidation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_validate/test_matchupValidation.py
+-rw-rw-rw-   0        0        0      530 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_validate/test_ownerValidation.py
+-rw-rw-rw-   0        0        0      838 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_validate/test_teamValidation.py
+-rw-rw-rw-   0        0        0     6094 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_validate/test_weekValidation.py
+-rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.4.0/test/test_validate/test_yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    25513 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_validate/test_yearValidation.py
```

### Comparing `leeger-2.3.0/LICENSE` & `leeger-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/PKG-INFO` & `leeger-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: leeger
-Version: 2.3.0
-Summary: Instant stats for your fantasy football league.
-Home-page: https://github.com/joeyagreco/leeger
-Author: Joey Greco
-Author-email: joeyagreco@gmail.com
-License: MIT
-Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
     <img src="https://raw.githubusercontent.com/joeyagreco/leeger/main/img/leeger-logo-cropped.png" alt="leeger logo" width="300"/>
 
 Instant stats for any fantasy football league.
 
 <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.10-teal.svg"></a>
 ![Main Build](https://github.com/joeyagreco/leeger/actions/workflows/main-build.yml/badge.svg)
@@ -154,15 +141,15 @@
 found [here](https://github.com/joeyagreco/leeger/blob/main/example/league/combiningLeagues.py).
 ___
 **Q:**
 Can I disable validation on my League object?
 
 **A:**
 Yes. While it is not recommended that you disable this, as validation ensures the stats are calculated properly,
-disabling validation can be done by passing `validate=False` into any method that takes a League object.
+disabling validation can be done by passing `validate=False` into any method that takes a League object OR any `loadLeague()` method from a League Loader.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install.
 
 ```bash
 pip install leeger
@@ -203,19 +190,27 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Development
+
+### Formatting
+
+_Run these commands from the root folder (leeger) before committing._\
+**General Format:** `black --config=pyproject.toml . `\
+**Import/Variable Format:** `autoflake --config=pyproject.toml .`
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Credit
 
 - [ESPN API](https://github.com/cwendt94/espn-api)
 - [ESPN Private Leagues](https://cran.r-project.org/web/packages/ffscrapr/vignettes/espn_authentication.html)
 - [fleaflicker](https://github.com/joeyagreco/fleaflicker)
 - [pymfl](https://github.com/joeyagreco/pymfl)
 - [sleeper](https://github.com/joeyagreco/sleeper)
-- [YahooFantasy](https://github.com/mattdodge/yahoofantasy)
+- [YahooFantasy](https://github.com/mattdodge/yahoofantasy)
```

### Comparing `leeger-2.3.0/README.md` & `leeger-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: leeger
+Version: 2.4.0
+Summary: Instant stats for your fantasy football league.
+Home-page: https://github.com/joeyagreco/leeger
+Author: Joey Greco
+Author-email: joeyagreco@gmail.com
+License: MIT
+Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <img src="https://raw.githubusercontent.com/joeyagreco/leeger/main/img/leeger-logo-cropped.png" alt="leeger logo" width="300"/>
 
 Instant stats for any fantasy football league.
 
 <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.10-teal.svg"></a>
 ![Main Build](https://github.com/joeyagreco/leeger/actions/workflows/main-build.yml/badge.svg)
@@ -141,15 +154,15 @@
 found [here](https://github.com/joeyagreco/leeger/blob/main/example/league/combiningLeagues.py).
 ___
 **Q:**
 Can I disable validation on my League object?
 
 **A:**
 Yes. While it is not recommended that you disable this, as validation ensures the stats are calculated properly,
-disabling validation can be done by passing `validate=False` into any method that takes a League object.
+disabling validation can be done by passing `validate=False` into any method that takes a League object OR any `loadLeague()` method from a League Loader.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install.
 
 ```bash
 pip install leeger
@@ -190,19 +203,27 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Development
+
+### Formatting
+
+_Run these commands from the root folder (leeger) before committing._\
+**General Format:** `black --config=pyproject.toml . `\
+**Import/Variable Format:** `autoflake --config=pyproject.toml .`
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Credit
 
 - [ESPN API](https://github.com/cwendt94/espn-api)
 - [ESPN Private Leagues](https://cran.r-project.org/web/packages/ffscrapr/vignettes/espn_authentication.html)
 - [fleaflicker](https://github.com/joeyagreco/fleaflicker)
 - [pymfl](https://github.com/joeyagreco/pymfl)
 - [sleeper](https://github.com/joeyagreco/sleeper)
-- [YahooFantasy](https://github.com/mattdodge/yahoofantasy)
+- [YahooFantasy](https://github.com/mattdodge/yahoofantasy)
```

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,33 +56,30 @@
             year = LeagueNavigator.getYearByYearNumber(league, int(yearNumber))
             gamesPlayedByYear[yearNumber] = TeamSummaryYearCalculator.getGamesPlayed(
                 year, **yearFiltersByYear[str(yearNumber)].asKwargs()
             )
 
         ownerIdToTeamScoreAndGamesPlayedListMap: dict[str, list[tuple[Deci, int]]] = dict()
         # {"someOwnerId": [(Deci("101.5"), 4), (Deci("109.4), 5)]}
-        for (yearNumber, teamScoreResultDict) in teamScoreResultsOrderedByYear.items():
+        for yearNumber, teamScoreResultDict in teamScoreResultsOrderedByYear.items():
             for teamId, teamScore in teamScoreResultDict.items():
                 team = LeagueNavigator.getTeamById(league, teamId)
                 gamesPlayed = gamesPlayedByYear[yearNumber][teamId]
                 if team.ownerId in ownerIdToTeamScoreAndGamesPlayedListMap:
                     ownerIdToTeamScoreAndGamesPlayedListMap[team.ownerId].append(
                         (teamScore, gamesPlayed)
                     )
                 else:
                     ownerIdToTeamScoreAndGamesPlayedListMap[team.ownerId] = [
                         (teamScore, gamesPlayed)
                     ]
 
         # adjust team scores by games played
         ownerIdAndAdjustedTeamScore: dict[str, Optional[Deci]] = dict()
-        for (
-            ownerId,
-            teamScoreAndGamesPlayedList,
-        ) in ownerIdToTeamScoreAndGamesPlayedListMap.items():
+        for ownerId, teamScoreAndGamesPlayedList in ownerIdToTeamScoreAndGamesPlayedListMap.items():
             totalGamesPlayed = sum([tsagp[1] for tsagp in teamScoreAndGamesPlayedList])
             if totalGamesPlayed > 0:
                 for teamScore, gamesPlayed in teamScoreAndGamesPlayedList:
                     if teamScore is not None:
                         percentageOfGamesPlayed = Deci(gamesPlayed / totalGamesPlayed)
                         adjustedTeamScore = Deci(teamScore * percentageOfGamesPlayed)
                         if ownerId in ownerIdAndAdjustedTeamScore:
@@ -126,15 +123,15 @@
             year = LeagueNavigator.getYearByYearNumber(league, int(yearNumber))
             gamesPlayedByYear[yearNumber] = TeamSummaryYearCalculator.getGamesPlayed(
                 year, **yearFiltersByYear[str(yearNumber)].asKwargs()
             )
 
         ownerIdToTeamSuccessAndGamesPlayedListMap: dict[str, list[tuple[Deci, int]]] = dict()
         # {"someOwnerId": [(Deci("101.5"), 4), (Deci("109.4), 5)]}
-        for (yearNumber, teamSuccessResultDict) in teamSuccessResultsOrderedByYear.items():
+        for yearNumber, teamSuccessResultDict in teamSuccessResultsOrderedByYear.items():
             for teamId, teamSuccess in teamSuccessResultDict.items():
                 team = LeagueNavigator.getTeamById(league, teamId)
                 gamesPlayed = gamesPlayedByYear[yearNumber][teamId]
                 if team.ownerId in ownerIdToTeamSuccessAndGamesPlayedListMap:
                     ownerIdToTeamSuccessAndGamesPlayedListMap[team.ownerId].append(
                         (teamSuccess, gamesPlayed)
                     )
```

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             ownerIdAndMaxScoringShare[ownerId] = None
 
         maxScoringSharesByYearTeamIds = cls._getAllResultDictsByYear(
             league, ScoringShareYearCalculator.getMaxScoringShare, **kwargs
         )
         # swap out team IDs for owner IDs
         maxScoringSharesByYear = dict()
-        for (yearNumber, maxScoringSharesByTeamId) in maxScoringSharesByYearTeamIds.items():
+        for yearNumber, maxScoringSharesByTeamId in maxScoringSharesByYearTeamIds.items():
             maxScoringSharesByYear[yearNumber] = dict()
             for teamId, maxScoringShare in maxScoringSharesByTeamId.items():
                 ownerId = LeagueNavigator.getTeamById(league, teamId).ownerId
                 maxScoringSharesByYear[yearNumber][ownerId] = maxScoringShare
 
         ownerIdAndMaxScoringShares: dict[str, list] = dict()
         for yearNumber in maxScoringSharesByYear.keys():
@@ -179,15 +179,15 @@
             ownerIdAndMinScoringShare[ownerId] = None
 
         minScoringSharesByYearTeamIds = cls._getAllResultDictsByYear(
             league, ScoringShareYearCalculator.getMinScoringShare, **kwargs
         )
         # swap out team IDs for owner IDs
         minScoringSharesByYear = dict()
-        for (yearNumber, minScoringSharesByTeamId) in minScoringSharesByYearTeamIds.items():
+        for yearNumber, minScoringSharesByTeamId in minScoringSharesByYearTeamIds.items():
             minScoringSharesByYear[yearNumber] = dict()
             for teamId, maxScoringShare in minScoringSharesByTeamId.items():
                 ownerId = LeagueNavigator.getTeamById(league, teamId).ownerId
                 minScoringSharesByYear[yearNumber][ownerId] = maxScoringShare
 
         ownerIdAndMinScoringShares: dict[str, list] = dict()
         for yearNumber in minScoringSharesByYear.keys():
```

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/all_time_calculator/__init__.py` & `leeger-2.4.0/leeger/calculator/all_time_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/parent/AllTimeCalculator.py` & `leeger-2.4.0/leeger/calculator/parent/AllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/parent/YearCalculator.py` & `leeger-2.4.0/leeger/calculator/parent/YearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/AWALYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/SSLYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py` & `leeger-2.4.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/calculator/year_calculator/__init__.py` & `leeger-2.4.0/leeger/calculator/year_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/decorator/validators.py` & `leeger-2.4.0/leeger/decorator/validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/enum/MatchupType.py` & `leeger-2.4.0/leeger/enum/MatchupType.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/exception/__init__.py` & `leeger-2.4.0/leeger/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/league_loader/ESPNLeagueLoader.py` & `leeger-2.4.0/leeger/league_loader/ESPNLeagueLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 import espn_api.football as espn
 from espn_api.football import League as ESPNLeague
 from espn_api.football import Team as ESPNTeam
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.league_loader.LeagueLoader import LeagueLoader
 from leeger.model.league.League import League
@@ -28,22 +29,28 @@
         4: 2,
         6: 3,
         7: 3,
         8: 3,
     }
 
     def __init__(
-        self, leagueId: str, years: list[int], espnS2: str = None, swid: str = None, **kwargs
+        self,
+        leagueId: str,
+        years: list[int],
+        *,
+        espnS2: str = None,
+        swid: str = None,
+        ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
     ):
         # validation
         try:
             int(leagueId)
         except ValueError:
             raise ValueError(f"League ID '{leagueId}' could not be turned into an int.")
-        super().__init__(leagueId, years, **kwargs)
+        super().__init__(leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
 
         self.__espnS2 = espnS2
         self.__swid = swid
         self.__espnTeamIdToTeamMap: dict[str, Team] = dict()
 
     def __getAllLeagues(self) -> list[ESPNLeague]:
         espnLeagueYears = list()
@@ -52,14 +59,15 @@
                 espn.League(
                     league_id=int(self._leagueId),
                     year=year,
                     espn_s2=self.__espnS2,
                     swid=self.__swid,
                 )
             )
+        self._validateRetrievedLeagues(espnLeagueYears)
         return espnLeagueYears
 
     def getOwnerNames(self) -> dict[int, list[str]]:
         yearToOwnerNamesMap: dict[int, list[str]] = dict()
         espnLeagueYears = self.__getAllLeagues()
         for espnLeagueYear in espnLeagueYears:
             yearToOwnerNamesMap[espnLeagueYear.year] = list()
@@ -74,18 +82,22 @@
             # validate new league
             leagueValidation.runAllChecks(league)
         return league
 
     def __buildLeague(self, espnLeagues: list[ESPNLeague]) -> League:
         years = list()
         for espnLeague in espnLeagues:
+            # save league name for each year
+            self._leagueNameByYear[espnLeague.year] = espnLeague.settings.name
             self.__loadOwners(espnLeague.teams)
             years.append(self.__buildYear(espnLeague))
         # use the league name from the most recent year
-        return League(name=espnLeagues[-1].settings.name, owners=self._owners, years=years)
+        return League(
+            name=self._getLeagueName(), owners=self._owners, years=self._getValidYears(years)
+        )
 
     def __loadOwners(self, espnTeams: list[ESPNTeam]) -> None:
         if self._owners is None:
             owners = list()
             for espnTeam in espnTeams:
                 # get general owner name if there is one
                 generalOwnerName = self._getGeneralOwnerNameFromGivenOwnerName(espnTeam.owner)
```

### Comparing `leeger-2.3.0/leeger/league_loader/FleaflickerLeagueLoader.py` & `leeger-2.4.0/leeger/league_loader/FleaflickerLeagueLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from fleaflicker.api.LeagueInfoAPIClient import LeagueInfoAPIClient
 from fleaflicker.api.ScoringAPIClient import ScoringAPIClient
 from fleaflicker.enum.Sport import Sport
 from sleeper.enum import Sport
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.league_loader.LeagueLoader import LeagueLoader
@@ -16,34 +17,41 @@
 
 class FleaflickerLeagueLoader(LeagueLoader):
     """
     Responsible for loading a League from Fleaflicker.
     https://www.fleaflicker.com/
     """
 
-    def __init__(self, leagueId: str, years: list[int], **kwargs):
+    def __init__(
+        self,
+        leagueId: str,
+        years: list[int],
+        *,
+        ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+    ):
         # validation
         try:
             int(leagueId)
         except ValueError:
             raise ValueError(f"League ID '{leagueId}' could not be turned into an int.")
-        super().__init__(leagueId, years, **kwargs)
+        super().__init__(leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
 
         self.__fleaflickerTeamIdToOwnerMap: dict[int, Owner] = dict()
         self.__fleaflickerTeamIdToTeamMap: dict[int, Team] = dict()
 
     def __getAllLeagues(self) -> list[dict]:
         # return a list of all leagues
         fleaflickerLeagues = list()
         for year in self._years:
             fleaflickerLeagues.append(
                 LeagueInfoAPIClient.get_league_standings(
                     sport=Sport.NFL, league_id=int(self._leagueId), season=year
                 )
             )
+        self._validateRetrievedLeagues(fleaflickerLeagues)
         return fleaflickerLeagues
 
     def getOwnerNames(self) -> dict[int, list[str]]:
         yearToOwnerNamesMap: dict[int, list[str]] = dict()
         fleaflickerLeagues = self.__getAllLeagues()
         for fleaflickerLeague in fleaflickerLeagues:
             yearToOwnerNamesMap[int(fleaflickerLeague["season"])] = list()
@@ -59,27 +67,23 @@
         if validate:
             # validate new league
             leagueValidation.runAllChecks(league)
         return league
 
     def __buildLeague(self, fleaflickerLeagues: list[dict]) -> League:
         years = list()
-        leagueName = None
         self.__loadOwners(fleaflickerLeagues)
         owners = list(self.__fleaflickerTeamIdToOwnerMap.values())
         for fleaflickerLeague in fleaflickerLeagues:
-            leagueName = fleaflickerLeague["league"]["name"] if leagueName is None else leagueName
-            year = self.__buildYear(fleaflickerLeague)
-            if len(year.weeks) > 0:
-                years.append(year)
-            else:
-                self._LOGGER.warning(
-                    f"Year '{year.yearNumber}' discarded for not having any weeks."
-                )
-        return League(name=leagueName, owners=owners, years=years)
+            # save league name for each year
+            self._leagueNameByYear[fleaflickerLeague["season"]] = fleaflickerLeague["league"][
+                "name"
+            ]
+            years.append(self.__buildYear(fleaflickerLeague))
+        return League(name=self._getLeagueName(), owners=owners, years=self._getValidYears(years))
 
     def __buildYear(self, fleaflickerLeague: dict) -> Year:
         teams = self.__buildTeams(fleaflickerLeague)
         weeks = self.__buildWeeks(fleaflickerLeague)
         return Year(yearNumber=int(fleaflickerLeague["season"]), teams=teams, weeks=weeks)
 
     def __buildWeeks(self, fleaflickerLeague: dict) -> list[Week]:
@@ -161,12 +165,16 @@
                 self.__fleaflickerTeamIdToTeamMap[teamId] = team
         return teams
 
     def __loadOwners(self, fleaflickerLeagues: list[dict]) -> None:
         for fleaflickerLeague in fleaflickerLeagues:
             for division in fleaflickerLeague["divisions"]:
                 for team in division["teams"]:
-                    ownerName = team["owners"][0]["displayName"]
+                    if "owners" not in team:
+                        # some teams don't have owners listed in them, use the team name instead
+                        ownerName = team["name"]
+                    else:
+                        ownerName = team["owners"][0]["displayName"]
                     # get general owner name if there is one
                     generalOwnerName = self._getGeneralOwnerNameFromGivenOwnerName(ownerName)
                     ownerName = generalOwnerName if generalOwnerName is not None else ownerName
                     self.__fleaflickerTeamIdToOwnerMap[team["id"]] = Owner(name=ownerName)
```

### Comparing `leeger-2.3.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py` & `leeger-2.4.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from typing import Optional
 from pymfl.api import CommonLeagueInfoAPIClient
 from pymfl.api.config import APIConfig
-from sleeper.model import Matchup as SleeperMatchup
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.league_loader.LeagueLoader import LeagueLoader
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
@@ -23,17 +23,17 @@
         self,
         leagueId: str,
         years: list[int],
         *,
         mflUsername: str,
         mflPassword: str,
         mflUserAgentName: str,
-        **kwargs,
+        ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
     ):
-        super().__init__(leagueId, years, **kwargs)
+        super().__init__(leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
 
         self.__mflUsername = mflUsername
         self.__mflPassword = mflPassword
         self.__mflUserAgentName = mflUserAgentName
 
         self.__mflLeagueIdToYearMap: dict[str, int] = dict()
         self.__mflFranchiseIdToOwnerMap: dict[str, Owner] = dict()
@@ -52,14 +52,15 @@
             )
 
             mflLeague = CommonLeagueInfoAPIClient.get_league(year=year, league_id=self._leagueId)[
                 "league"
             ]
             self.__mflLeagueIdToYearMap[mflLeague["id"]] = year
             mflLeagues.append(mflLeague)
+        self._validateRetrievedLeagues(mflLeagues)
         return mflLeagues
 
     def getOwnerNames(self) -> dict[int, list[str]]:
         yearToOwnerNamesMap: dict[int, list[str]] = dict()
         mflLeagues = self.__getAllLeagues()
         for mflLeague in mflLeagues:
             yearNumber = self.__mflLeagueIdToYearMap[mflLeague["id"]]
@@ -75,44 +76,35 @@
         if validate:
             # validate new league
             leagueValidation.runAllChecks(league)
         return league
 
     def __buildLeague(self, mflLeagues: list[dict]) -> League:
         years = list()
-        leagueName = None
         self.__loadOwners(mflLeagues)
         owners = list(self.__mflFranchiseIdToOwnerMap.values())
         for mflLeague in mflLeagues:
-            leagueName = mflLeague["name"] if leagueName is None else leagueName
-            year = self.__buildYear(mflLeague)
-            if len(year.weeks) > 0:
-                years.append(year)
-            else:
-                self._LOGGER.warning(
-                    f"Year '{year.yearNumber}' discarded for not having any weeks."
-                )
-        return League(name=leagueName, owners=owners, years=years)
+            # save league name for each year
+            self._leagueNameByYear[self.__mflLeagueIdToYearMap[mflLeague["id"]]] = mflLeague["name"]
+            years.append(self.__buildYear(mflLeague))
+        return League(name=self._getLeagueName(), owners=owners, years=self._getValidYears(years))
 
     def __buildYear(self, mflLeague: dict) -> Year:
         yearNumber = self.__mflLeagueIdToYearMap[mflLeague["id"]]
         teams = self.__buildTeams(mflLeague)
         weeks = self.__buildWeeks(mflLeague)
         return Year(yearNumber=yearNumber, teams=teams, weeks=weeks)
 
     def __buildWeeks(self, mflLeague: dict) -> list[Week]:
         yearNumber = self.__mflLeagueIdToYearMap[mflLeague["id"]]
         weeks = list()
         schedule: dict = CommonLeagueInfoAPIClient.get_schedule(
             year=yearNumber, league_id=mflLeague["id"]
         )["schedule"]
         # get playoff brackets
-        # playoffBrackets: dict = \
-        #     CommonLeagueInfoAPIClient.get_playoff_brackets(year=yearNumber, league_id=mflLeague["id"])[
-        #         "playoffBrackets"]
         playoffBracket: dict = CommonLeagueInfoAPIClient.get_playoff_bracket(
             year=yearNumber, league_id=mflLeague["id"], bracket_id="1"
         )["playoffBracket"]
 
         # we will assume that the "true" playoff bracket (i.e. the bracket where the winner of it is the league champion)
         # will always be the playoff bracket with id "1".
         # if this changes or is not the case, this will need to be refactored to reflect that.
@@ -122,14 +114,15 @@
         if isinstance(playoffBracket["playoffRound"], dict):
             # only 1 playoff round
             playoffWeeks.append(playoffBracket["playoffRound"])
         else:
             # multiple playoff rounds
             for playoffBracketInfo in playoffBracket["playoffRound"]:
                 playoffWeeks.append(playoffBracketInfo)
+
         playoffWeekNumbers = [int(playoffWeek["week"]) for playoffWeek in playoffWeeks]
 
         playoffsStarted = False
         for week in schedule["weeklySchedule"]:
             weekNumber = int(week["week"])
             if weekNumber > int(mflLeague["lastRegularSeasonWeek"]):
                 playoffsStarted = True
@@ -142,86 +135,35 @@
                 teamAHasTiebreaker = matchup["franchise"][0]["result"] == "W"
 
                 teamBMFLFranchiseId = matchup["franchise"][1]["id"]
                 teamBId = self.__mflFranchiseIdToTeamMap[teamBMFLFranchiseId].id
                 teamBScore = float(matchup["franchise"][1]["score"])
                 teamBHasTiebreaker = matchup["franchise"][1]["result"] == "W"
 
+                validPlayoffMatchup = False
+                validChampionshipMatchup = False
+
                 matchupType = MatchupType.REGULAR_SEASON
                 if playoffsStarted:
                     # this is a playoff matchup or a championship matchup
-                    validPlayoffMatchup = False
-                    validChampionshipMatchup = False
-
                     for playoffWeek in playoffWeeks:
-                        if weekNumber == max(playoffWeekNumbers):
-                            # this is the last week in the bracket, the championship week
-                            # if there is only 1 object in the playoffGame field, it is a dict, otherwise it is a list
-                            if isinstance(playoffWeek["playoffGame"], dict):
-                                # only 1 game
-                                if (
-                                    teamAMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["away"]["franchise_id"]
-                                    or teamBMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["away"]["franchise_id"]
-                                ) and (
-                                    teamAMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["home"]["franchise_id"]
-                                    or teamBMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["home"]["franchise_id"]
-                                ):
-                                    # this matchup is the championship game
-                                    validChampionshipMatchup = True
-                            else:
-                                # multiple games
-                                for playoffGame in playoffWeek["playoffGame"]:
-                                    if (
-                                        teamAMFLFranchiseId == playoffGame["away"]["franchise_id"]
-                                        or teamBMFLFranchiseId
-                                        == playoffGame["away"]["franchise_id"]
-                                    ) and (
-                                        teamAMFLFranchiseId == playoffGame["home"]["franchise_id"]
-                                        or teamBMFLFranchiseId
-                                        == playoffGame["home"]["franchise_id"]
-                                    ):
-                                        # this matchup is the championship game
-                                        validChampionshipMatchup = True
-                        else:
-                            # playoff week, but not the championship week
-                            # if there is only 1 object in the playoffGame field, it is a dict, otherwise it is a list
-                            if isinstance(playoffWeek["playoffGame"], dict):
-                                # only 1 game
-                                if (
-                                    teamAMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["away"]["franchise_id"]
-                                    or teamBMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["away"]["franchise_id"]
-                                ) and (
-                                    teamAMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["home"]["franchise_id"]
-                                    or teamBMFLFranchiseId
-                                    == playoffWeek["playoffGame"]["home"]["franchise_id"]
-                                ):
-                                    # this matchup is a valid playoff matchup
-                                    validPlayoffMatchup = True
-                            else:
-                                # multiple games
-                                for playoffGame in playoffWeek["playoffGame"]:
-                                    if (
-                                        teamAMFLFranchiseId == playoffGame["away"]["franchise_id"]
-                                        or teamBMFLFranchiseId
-                                        == playoffGame["away"]["franchise_id"]
-                                    ) and (
-                                        teamAMFLFranchiseId == playoffGame["home"]["franchise_id"]
-                                        or teamBMFLFranchiseId
-                                        == playoffGame["home"]["franchise_id"]
-                                    ):
-                                        # this matchup is a valid playoff matchup
-                                        validPlayoffMatchup = True
-
+                        (
+                            currentValidPlayoffMatchup,
+                            currentValidChampionshipMatchup,
+                        ) = self.__getPlayoffMatchupBooleansForPlayoffWeek(
+                            playoffWeek=playoffWeek,
+                            playoffWeekNumbers=playoffWeekNumbers,
+                            weekNumber=weekNumber,
+                            teamAMFLFranchiseId=teamAMFLFranchiseId,
+                            teamBMFLFranchiseId=teamBMFLFranchiseId,
+                        )
+                        validPlayoffMatchup = validPlayoffMatchup or currentValidPlayoffMatchup
+                        validChampionshipMatchup = (
+                            validChampionshipMatchup or currentValidChampionshipMatchup
+                        )
                     matchupType = MatchupType.IGNORE
                     if validPlayoffMatchup:
                         matchupType = MatchupType.PLAYOFF
                     if validChampionshipMatchup:
                         matchupType = MatchupType.CHAMPIONSHIP
 
                 matchups.append(
@@ -237,17 +179,74 @@
                 )
             if len(matchups) > 0:
                 weeks.append(Week(weekNumber=weekNumber, matchups=matchups))
 
         return weeks
 
     @staticmethod
-    def __isCompletedWeek(sleeperMatchups: list[SleeperMatchup]) -> bool:
-        # there might be a better way of determining this
-        return sum([sleeperMatchup.points for sleeperMatchup in sleeperMatchups]) != 0
+    def __getPlayoffMatchupBooleansForPlayoffWeek(
+        *,
+        playoffWeek: dict,
+        playoffWeekNumbers: list[int],
+        weekNumber: int,
+        teamAMFLFranchiseId: int,
+        teamBMFLFranchiseId: int,
+    ) -> tuple[bool, bool]:
+        """
+        Will return 2 booleans.
+        validPlayoffMatchup, validChampionshipMatchup
+        """
+
+        # helper method
+        def isValid(*, pGame: dict, aId: int, bId: int) -> bool:
+            return (
+                aId == pGame["away"]["franchise_id"] or bId == pGame["away"]["franchise_id"]
+            ) and (aId == pGame["home"]["franchise_id"] or bId == pGame["home"]["franchise_id"])
+
+        # this is a playoff matchup or a championship matchup
+        validPlayoffMatchup = False
+        validChampionshipMatchup = False
+
+        if weekNumber == max(playoffWeekNumbers):
+            # this is the last week in the bracket, the championship week
+            # if there is only 1 object in the playoffGame field, it is a dict, otherwise it is a list
+            if isinstance(playoffWeek["playoffGame"], dict):
+                # only 1 game
+                # check if this matchup is the championship game
+                validChampionshipMatchup = isValid(
+                    pGame=playoffWeek["playoffGame"],
+                    aId=teamAMFLFranchiseId,
+                    bId=teamBMFLFranchiseId,
+                )
+            else:
+                # multiple games
+                # check if this matchup is the championship game
+                for playoffGame in playoffWeek["playoffGame"]:
+                    validChampionshipMatchup = validChampionshipMatchup or isValid(
+                        pGame=playoffGame, aId=teamAMFLFranchiseId, bId=teamBMFLFranchiseId
+                    )
+        else:
+            # playoff week, but not the championship week
+            # if there is only 1 object in the playoffGame field, it is a dict, otherwise it is a list
+            if isinstance(playoffWeek["playoffGame"], dict):
+                # only 1 game
+                # check if this matchup is a valid playoff matchup
+                validPlayoffMatchup = isValid(
+                    pGame=playoffWeek["playoffGame"],
+                    aId=teamAMFLFranchiseId,
+                    bId=teamBMFLFranchiseId,
+                )
+            else:
+                # multiple games
+                for playoffGame in playoffWeek["playoffGame"]:
+                    # check if this matchup is a valid playoff matchup
+                    validPlayoffMatchup = validPlayoffMatchup or isValid(
+                        pGame=playoffGame, aId=teamAMFLFranchiseId, bId=teamBMFLFranchiseId
+                    )
+        return validPlayoffMatchup, validChampionshipMatchup
 
     def __buildTeams(self, mflLeague: dict) -> list[Team]:
         teams = list()
         for franchise in mflLeague["franchises"]["franchise"]:
             owner = self.__mflFranchiseIdToOwnerMap[franchise["id"]]
             team = Team(name=franchise["name"], ownerId=owner.id)
             self.__mflFranchiseIdToTeamMap[franchise["id"]] = team
```

### Comparing `leeger-2.3.0/leeger/league_loader/SleeperLeagueLoader.py` & `leeger-2.4.0/leeger/league_loader/SleeperLeagueLoader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,133 @@
 import itertools
+from typing import Optional
 
 from sleeper.api import LeagueAPIClient
-from sleeper.enum import Sport, SeasonStatus
-from sleeper.enum.PlayoffRoundType import PlayoffRoundType
+from sleeper.enum import Sport as SleeperSport
+from sleeper.enum import SeasonStatus as SleeperSeasonStatus
+from sleeper.enum import PlayoffRoundType as SleeperPlayoffRoundType
 from sleeper.model import League as SleeperLeague
 from sleeper.model import Matchup as SleeperMatchup
 from sleeper.model import PlayoffMatchup as SleeperPlayoffMatchup
+from sleeper.model import User as SleeperUser
+from sleeper.model import SportState as SleeperSportState
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception.DoesNotExistException import DoesNotExistException
 from leeger.league_loader.LeagueLoader import LeagueLoader
 from leeger.model.league import YearSettings
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.validate import leagueValidation
+from leeger.exception.LeagueLoaderException import LeagueLoaderException
 
 
 class SleeperLeagueLoader(LeagueLoader):
     """
     Responsible for loading a League from Sleeper Fantasy Football.
     https://sleeper.com/
     """
 
     __INVALID_SLEEPER_LEAGUE_IDS = [None, "0"]
 
-    def __init__(self, mostRecentLeagueId: str, years: list[int], **kwargs):
-        super().__init__(mostRecentLeagueId, years, **kwargs)
+    def __init__(
+        self,
+        mostRecentLeagueId: str,
+        years: list[int],
+        *,
+        ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+    ):
+        super().__init__(mostRecentLeagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
 
         self.__sleeperUserIdToOwnerMap: dict[str, Owner] = dict()
         self.__sleeperRosterIdToTeamMap: dict[int, Team] = dict()
+        self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE = dict()  # functions as a cache for Sleeper Users
+        self.__SLEEPER_SPORT_STATE_CACHE: SleeperSportState = (
+            None  # functions as a cache for Sleeper SportState
+        )
+
+    def __resetCaches(self) -> None:
+        self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE = dict()
+        self.__SLEEPER_SPORT_STATE_CACHE = None
+
+    def __getSleeperUsers(self, leagueId: str) -> list[SleeperUser]:
+        if leagueId not in self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE:
+            # don't have these users loaded yet
+            sleeperUsers = LeagueAPIClient.get_users_in_league(league_id=leagueId)
+            self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE[leagueId] = sleeperUsers
+            return sleeperUsers
+        # do have these users loaded
+        return self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE[leagueId]
+
+    def __getSleeperSportState(self):
+        if self.__SLEEPER_SPORT_STATE_CACHE is None:
+            self.__SLEEPER_SPORT_STATE_CACHE = LeagueAPIClient.get_sport_state(
+                sport=SleeperSport.NFL
+            )
+        return self.__SLEEPER_SPORT_STATE_CACHE
 
     def __getAllLeagues(self) -> list[SleeperLeague]:
         sleeperLeagues = list()
         years = self._years.copy()
         currentLeagueId = self._leagueId
         while len(years) > 0 and currentLeagueId not in self.__INVALID_SLEEPER_LEAGUE_IDS:
             currentLeague: SleeperLeague = LeagueAPIClient.get_league(league_id=currentLeagueId)
             if int(currentLeague.season) in years:
+                # we only want to add valid seasons
+                # NOTE: Not sure if we want to include SleeperSeasonStatus.POSTPONED here or not
+                if currentLeague.status not in (
+                    SleeperSeasonStatus.COMPLETE,
+                    SleeperSeasonStatus.IN_SEASON,
+                    SleeperSeasonStatus.POST_SEASON,
+                ):
+                    raise LeagueLoaderException(
+                        f"Year {currentLeague.season} has a status that is not supported: '{currentLeague.status}'"
+                    )
                 sleeperLeagues.append(currentLeague)
                 years.remove(int(currentLeague.season))
             currentLeagueId = currentLeague.previous_league_id
 
-        if len(years) > 0:
-            raise ValueError(f"Could not find years '{years}' for league.")
-
         # reverse list so most recent is last in list
         sleeperLeagues = sleeperLeagues[::-1]
+        self._validateRetrievedLeagues(sleeperLeagues)
         return sleeperLeagues
 
     def getOwnerNames(self) -> dict[int, list[str]]:
         yearToOwnerNamesMap: dict[int, list[str]] = dict()
         sleeperLeagues = self.__getAllLeagues()
         for sleeperLeague in sleeperLeagues:
             yearToOwnerNamesMap[int(sleeperLeague.season)] = list()
-            sleeperUsers = LeagueAPIClient.get_users_in_league(league_id=sleeperLeague.league_id)
+            sleeperUsers = self.__getSleeperUsers(sleeperLeague.league_id)
             for sleeperUser in sleeperUsers:
                 ownerName = sleeperUser.display_name
                 yearToOwnerNamesMap[int(sleeperLeague.season)].append(ownerName)
         return yearToOwnerNamesMap
 
     def loadLeague(self, validate: bool = True) -> League:
         sleeperLeagues = self.__getAllLeagues()
         league = self.__buildLeague(sleeperLeagues)
         if validate:
             # validate new league
             leagueValidation.runAllChecks(league)
+        self.__resetCaches()
         return league
 
     def __buildLeague(self, sleeperLeagues: list[SleeperLeague]) -> League:
         years = list()
-        leagueName = None
         self.__loadOwners(sleeperLeagues)
         owners = list(self.__sleeperUserIdToOwnerMap.values())
         for sleeperLeague in sleeperLeagues:
-            leagueName = sleeperLeague.name if leagueName is None else leagueName
-            year = self.__buildYear(sleeperLeague)
-            if len(year.weeks) > 0:
-                years.append(year)
-            else:
-                self._LOGGER.warning(
-                    f"Year '{year.yearNumber}' discarded for not having any weeks."
-                )
-        return League(name=leagueName, owners=owners, years=years)
+            # save league name for each year
+            self._leagueNameByYear[int(sleeperLeague.season)] = sleeperLeague.name
+            years.append(self.__buildYear(sleeperLeague))
+        return League(name=self._getLeagueName(), owners=owners, years=self._getValidYears(years))
 
     def __buildYear(self, sleeperLeague: SleeperLeague) -> Year:
         teams = self.__buildTeams(sleeperLeague)
         weeks = self.__buildWeeks(sleeperLeague)
         # add YearSettings
         yearSettings = YearSettings()
         if sleeperLeague.settings.league_average_match == 1:
@@ -100,23 +138,25 @@
             weeks=weeks,
             yearSettings=yearSettings,
         )
 
     def __buildWeeks(self, sleeperLeague: SleeperLeague) -> list[Week]:
         weeks = list()
         # get regular season weeks
+        # once we have found an incomplete week, all weeks after will also be incomplete
+        foundIncompleteWeek = False
         for i in range(sleeperLeague.settings.playoff_week_start - 1):
-            # get each teams matchup for that week
-            matchups = list()
-            sleeperMatchups = LeagueAPIClient.get_matchups_for_week(
-                league_id=sleeperLeague.league_id, week=i + 1
-            )
-            if self.__isCompletedWeek(i + 1, sleeperLeague):
+            if not foundIncompleteWeek and self.__isCompletedWeek(i + 1, sleeperLeague):
+                # get each teams matchup for that week
+                matchups = list()
+                sleeperMatchupsForThisWeek = LeagueAPIClient.get_matchups_for_week(
+                    league_id=sleeperLeague.league_id, week=i + 1
+                )
                 sleeperMatchupIdToSleeperMatchupMap: dict[int, list[SleeperMatchup]] = dict()
-                for sleeperMatchup in sleeperMatchups:
+                for sleeperMatchup in sleeperMatchupsForThisWeek:
                     if sleeperMatchup.matchup_id in sleeperMatchupIdToSleeperMatchupMap.keys():
                         sleeperMatchupIdToSleeperMatchupMap[sleeperMatchup.matchup_id].append(
                             sleeperMatchup
                         )
                     else:
                         sleeperMatchupIdToSleeperMatchupMap[sleeperMatchup.matchup_id] = [
                             sleeperMatchup
@@ -141,117 +181,125 @@
                             teamBScore=teamBSleeperMatchup.points,
                             teamAHasTiebreaker=False,
                             teamBHasTiebreaker=False,
                             matchupType=MatchupType.REGULAR_SEASON,
                         )
                     )
                 weeks.append(Week(weekNumber=i + 1, matchups=matchups))
+            else:
+                foundIncompleteWeek = True
         # get playoff weeks
-        sleeperPlayoffMatchups = LeagueAPIClient.get_winners_bracket(
+        # NOTE: bye weeks will not be returned here. That's ok because we don't want those anyways
+        allSleeperPlayoffMatchups = LeagueAPIClient.get_winners_bracket(
             league_id=sleeperLeague.league_id
         )
-        # sort sleeperPlayoffMatchups by round into a dict
-        playoffRoundAndSleeperPlayoffMatchups: dict[int, list[SleeperPlayoffMatchup]] = dict()
-        for sleeperPlayoffMatchup in sleeperPlayoffMatchups:
-            if sleeperPlayoffMatchup.round in playoffRoundAndSleeperPlayoffMatchups.keys():
-                playoffRoundAndSleeperPlayoffMatchups[sleeperPlayoffMatchup.round].append(
-                    sleeperPlayoffMatchup
+        if len(allSleeperPlayoffMatchups) > 0:
+            # sort sleeperPlayoffMatchups by round into a dict
+            playoffRoundAndSleeperPlayoffMatchups: dict[int, list[SleeperPlayoffMatchup]] = dict()
+            for sleeperPlayoffMatchup in allSleeperPlayoffMatchups:
+                if sleeperPlayoffMatchup.round in playoffRoundAndSleeperPlayoffMatchups.keys():
+                    playoffRoundAndSleeperPlayoffMatchups[sleeperPlayoffMatchup.round].append(
+                        sleeperPlayoffMatchup
+                    )
+                else:
+                    playoffRoundAndSleeperPlayoffMatchups[sleeperPlayoffMatchup.round] = [
+                        sleeperPlayoffMatchup
+                    ]
+            numberOfPlayoffRounds = max(
+                [playoffMatchup.round for playoffMatchup in allSleeperPlayoffMatchups]
+            )  # don't know a better way to determine this
+            numberOfPlayoffWeeks = self.__calculate_number_of_playoff_weeks(
+                sleeperLeague, allSleeperPlayoffMatchups
+            )
+            playoffWeeks = list(
+                range(
+                    sleeperLeague.settings.playoff_week_start,
+                    sleeperLeague.settings.playoff_week_start + numberOfPlayoffWeeks,
                 )
-            else:
-                playoffRoundAndSleeperPlayoffMatchups[sleeperPlayoffMatchup.round] = [
-                    sleeperPlayoffMatchup
-                ]
-        numberOfPlayoffRounds = max(
-            [playoffMatchup.round for playoffMatchup in sleeperPlayoffMatchups]
-        )  # don't know a better way to determine this
-        numberOfPlayoffWeeks = self.__calculate_number_of_playoff_weeks(
-            sleeperLeague, sleeperPlayoffMatchups
-        )
-        playoffWeeks = list(
-            range(
-                sleeperLeague.settings.playoff_week_start,
-                sleeperLeague.settings.playoff_week_start + numberOfPlayoffWeeks,
             )
-        )
-        playoffWeekRoundList = self.__create_playoff_week_round_list(
-            sleeperLeague, playoffWeeks, numberOfPlayoffRounds
-        )
-        for weekNumber, roundNumber in playoffWeekRoundList:
-            # get each teams matchup for that week
-            matchups = list()
-            sleeperMatchups = LeagueAPIClient.get_matchups_for_week(
-                league_id=sleeperLeague.league_id, week=weekNumber
+            playoffWeekRoundList = self.__create_playoff_week_round_list(
+                sleeperLeague, playoffWeeks, numberOfPlayoffRounds
             )
-            if self.__isCompletedWeek(weekNumber, sleeperLeague):
-                # sort matchups by roster IDs
-                rosterIdToSleeperMatchupMap: dict[int, SleeperMatchup] = dict()
-                for sleeperMatchup in sleeperMatchups:
-                    rosterIdToSleeperMatchupMap[sleeperMatchup.roster_id] = sleeperMatchup
-                for sleeperPlayoffMatchup in playoffRoundAndSleeperPlayoffMatchups[roundNumber]:
-                    # team A
-                    teamARosterId = sleeperPlayoffMatchup.team_1_roster_id
-                    teamA = self.__sleeperRosterIdToTeamMap[teamARosterId]
-                    teamAPoints = rosterIdToSleeperMatchupMap[teamARosterId].points
-                    teamAHasTiebreaker = (
-                        sleeperPlayoffMatchup.winning_roster_id
-                        == sleeperPlayoffMatchup.team_1_roster_id
-                    )
-                    # team B
-                    teamBRosterId = sleeperPlayoffMatchup.team_2_roster_id
-                    teamB = self.__sleeperRosterIdToTeamMap[teamBRosterId]
-                    teamBPoints = rosterIdToSleeperMatchupMap[teamBRosterId].points
-                    teamBHasTiebreaker = (
-                        sleeperPlayoffMatchup.winning_roster_id
-                        == sleeperPlayoffMatchup.team_2_roster_id
-                    )
-
-                    multiWeekMatchupId = None
-                    # determine if this is a championship matchup or not
-                    matchupType = MatchupType.PLAYOFF
-                    if sleeperPlayoffMatchup.p == 1:
-                        matchupType = MatchupType.CHAMPIONSHIP
-                        if (
-                            sleeperLeague.settings.playoff_round_type_enum
-                            == PlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND
-                        ):
-                            multiWeekMatchupId = f"{teamA.id}{teamB.id}"
-                    if (
-                        sleeperLeague.settings.playoff_round_type_enum
-                        == PlayoffRoundType.TWO_WEEKS_PER_ROUND
-                    ):
-                        multiWeekMatchupId = f"{teamA.id}{teamB.id}"
-                    matchups.append(
-                        Matchup(
-                            teamAId=teamA.id,
-                            teamBId=teamB.id,
-                            teamAScore=teamAPoints,
-                            teamBScore=teamBPoints,
-                            teamAHasTiebreaker=teamAHasTiebreaker,
-                            teamBHasTiebreaker=teamBHasTiebreaker,
-                            matchupType=matchupType,
-                            multiWeekMatchupId=multiWeekMatchupId,
-                        )
-                    )
-                weeks.append(Week(weekNumber=weekNumber, matchups=matchups))
-
+            for weekNumber, roundNumber in playoffWeekRoundList:
+                # get each teams matchup for that week
+                matchups = list()
+                sleeperMatchupsForThisWeek = LeagueAPIClient.get_matchups_for_week(
+                    league_id=sleeperLeague.league_id, week=weekNumber
+                )
+                # used to check if a Sleeper playoff matchup is in this week's matchups
+                sleeperMatchupIdsForThisWeek = [
+                    sleeperMatchup.matchup_id for sleeperMatchup in sleeperMatchupsForThisWeek
+                ]
+                if self.__isCompletedWeek(weekNumber, sleeperLeague):
+                    # sort matchups by roster IDs
+                    rosterIdToSleeperMatchupMap: dict[int, SleeperMatchup] = dict()
+                    for sleeperMatchup in sleeperMatchupsForThisWeek:
+                        rosterIdToSleeperMatchupMap[sleeperMatchup.roster_id] = sleeperMatchup
+                    for sleeperPlayoffMatchup in playoffRoundAndSleeperPlayoffMatchups[roundNumber]:
+                        # check if this matchup is in this week (needed for leagues with multiple weeks in a single round)
+                        if sleeperPlayoffMatchup.matchup_id in sleeperMatchupIdsForThisWeek:
+                            # team A
+                            teamARosterId = sleeperPlayoffMatchup.team_1_roster_id
+                            teamA = self.__sleeperRosterIdToTeamMap[teamARosterId]
+                            teamAPoints = rosterIdToSleeperMatchupMap[teamARosterId].points
+                            teamAHasTiebreaker = (
+                                sleeperPlayoffMatchup.winning_roster_id
+                                == sleeperPlayoffMatchup.team_1_roster_id
+                            )
+                            # team B
+                            teamBRosterId = sleeperPlayoffMatchup.team_2_roster_id
+                            teamB = self.__sleeperRosterIdToTeamMap[teamBRosterId]
+                            teamBPoints = rosterIdToSleeperMatchupMap[teamBRosterId].points
+                            teamBHasTiebreaker = (
+                                sleeperPlayoffMatchup.winning_roster_id
+                                == sleeperPlayoffMatchup.team_2_roster_id
+                            )
+
+                            multiWeekMatchupId = None
+                            # determine if this is a championship matchup or not
+                            matchupType = MatchupType.PLAYOFF
+                            if sleeperPlayoffMatchup.p == 1:
+                                matchupType = MatchupType.CHAMPIONSHIP
+                                if (
+                                    sleeperLeague.settings.playoff_round_type_enum
+                                    == SleeperPlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND
+                                ):
+                                    multiWeekMatchupId = f"{teamA.id}{teamB.id}"
+                            if (
+                                sleeperLeague.settings.playoff_round_type_enum
+                                == SleeperPlayoffRoundType.TWO_WEEKS_PER_ROUND
+                            ):
+                                multiWeekMatchupId = f"{teamA.id}{teamB.id}"
+                            matchups.append(
+                                Matchup(
+                                    teamAId=teamA.id,
+                                    teamBId=teamB.id,
+                                    teamAScore=teamAPoints,
+                                    teamBScore=teamBPoints,
+                                    teamAHasTiebreaker=teamAHasTiebreaker,
+                                    teamBHasTiebreaker=teamBHasTiebreaker,
+                                    matchupType=matchupType,
+                                    multiWeekMatchupId=multiWeekMatchupId,
+                                )
+                            )
+                    weeks.append(Week(weekNumber=weekNumber, matchups=matchups))
         return weeks
 
-    @staticmethod
-    def __isCompletedWeek(weekNumber: int, sleeperLeague: SleeperLeague) -> bool:
+    def __isCompletedWeek(self, weekNumber: int, sleeperLeague: SleeperLeague) -> bool:
         # see if this is the current year/week of the NFL
-        sportState = LeagueAPIClient.get_sport_state(sport=Sport.NFL)
+        sportState = self.__getSleeperSportState()
         return not (
             sportState.season == sleeperLeague.season
             and sportState.leg <= weekNumber
-            and sleeperLeague.status != SeasonStatus.COMPLETE
+            and sleeperLeague.status != SleeperSeasonStatus.COMPLETE
         )
 
     def __buildTeams(self, sleeperLeague: SleeperLeague) -> list[Team]:
         teams = list()
-        sleeperUsers = LeagueAPIClient.get_users_in_league(league_id=sleeperLeague.league_id)
+        sleeperUsers = self.__getSleeperUsers(sleeperLeague.league_id)
         sleeperRosters = LeagueAPIClient.get_rosters(league_id=sleeperLeague.league_id)
         for sleeperUser in sleeperUsers:
             # connect a sleeperUser to a sleeperRoster
             rosterId = None
             for sleeperRoster in sleeperRosters:
                 if sleeperRoster.owner_id == sleeperUser.user_id:
                     rosterId = sleeperRoster.roster_id
@@ -270,15 +318,15 @@
             team = Team(ownerId=owner.id, name=teamName)
             teams.append(team)
             self.__sleeperRosterIdToTeamMap[rosterId] = team
         return teams
 
     def __loadOwners(self, sleeperLeagues: list[SleeperLeague]) -> None:
         for sleeperLeague in sleeperLeagues:
-            sleeperUsers = LeagueAPIClient.get_users_in_league(league_id=sleeperLeague.league_id)
+            sleeperUsers = self.__getSleeperUsers(sleeperLeague.league_id)
             for sleeperUser in sleeperUsers:
                 ownerName = sleeperUser.display_name
                 # get general owner name if there is one
                 generalOwnerName = self._getGeneralOwnerNameFromGivenOwnerName(ownerName)
                 ownerName = generalOwnerName if generalOwnerName is not None else ownerName
                 self.__sleeperUserIdToOwnerMap[sleeperUser.user_id] = Owner(name=ownerName)
 
@@ -297,36 +345,40 @@
                 playoffRoundAndSleeperPlayoffMatchups[sleeperPlayoffMatchup.round] = [
                     sleeperPlayoffMatchup
                 ]
         numberOfPlayoffRounds = max(
             [playoffMatchup.round for playoffMatchup in sleeperPlayoffMatchups]
         )  # don't know a better way to determine this
         match sleeperLeague.settings.playoff_round_type_enum:
-            case PlayoffRoundType.ONE_WEEK_PER_ROUND:
+            case SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND:
                 return numberOfPlayoffRounds
-            case PlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND:
+            case SleeperPlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND:
                 return numberOfPlayoffRounds + 1
-            case PlayoffRoundType.TWO_WEEKS_PER_ROUND:
+            case SleeperPlayoffRoundType.TWO_WEEKS_PER_ROUND:
                 return numberOfPlayoffRounds * 2
+            case _:
+                raise LeagueLoaderException(
+                    f"PlayoffRoundType '{sleeperLeague.settings.playoff_round_type_enum}' is not supported."
+                )
 
     @staticmethod
     def __create_playoff_week_round_list(
         sleeperLeague: SleeperLeague, playoffWeeks: list, numberOfPlayoffRounds: int
     ) -> list[tuple[int, int]]:
         match sleeperLeague.settings.playoff_round_type_enum:
-            case PlayoffRoundType.ONE_WEEK_PER_ROUND:
+            case SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND:
                 return list(zip(playoffWeeks, range(1, numberOfPlayoffRounds + 1)))
-            case PlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND:
+            case SleeperPlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND:
                 return list(
                     itertools.zip_longest(
                         playoffWeeks,
                         range(1, numberOfPlayoffRounds + 1),
                         fillvalue=numberOfPlayoffRounds,
                     )
                 )
-            case PlayoffRoundType.TWO_WEEKS_PER_ROUND:
+            case SleeperPlayoffRoundType.TWO_WEEKS_PER_ROUND:
                 playoffRounds = [
                     playoffRound
                     for playoffRound in range(1, numberOfPlayoffRounds + 1)
-                    for i in range(1, numberOfPlayoffRounds + 1)
+                    for _ in range(1, numberOfPlayoffRounds + 1)
                 ]
                 return list(zip(playoffWeeks, playoffRounds))
```

### Comparing `leeger-2.3.0/leeger/league_loader/YahooLeagueLoader.py` & `leeger-2.4.0/leeger/league_loader/YahooLeagueLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import multiprocessing
 import subprocess
+from typing import Optional
 
-from yahoofantasy import Context
+from yahoofantasy import Context as YahooContext
 from yahoofantasy import League as YahooLeague
 from yahoofantasy import Matchup as YahooMatchup
 from yahoofantasy import Team as YahooTeam
 from yahoofantasy import Week as YahooWeek
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception.DoesNotExistException import DoesNotExistException
+from leeger.exception.LeagueLoaderException import LeagueLoaderException
 from leeger.league_loader.LeagueLoader import LeagueLoader
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
@@ -22,34 +24,39 @@
 class YahooLeagueLoader(LeagueLoader):
     """
     Responsible for loading a League from Yahoo Fantasy Football.
     https://football.fantasysports.yahoo.com/
     """
 
     __NFL = "nfl"
-    __LOGIN_TIMEOUT_SECONDS = 20
 
     def __init__(
-        self, leagueId: str, years: list[int], *, clientId: str, clientSecret: str, **kwargs
+        self,
+        mostRecentLeagueId: str,
+        years: list[int],
+        *,
+        clientId: str,
+        clientSecret: str,
+        loginTimeoutSeconds: Optional[int] = 20,
+        ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
     ):
         # validation
         try:
-            int(leagueId)
+            int(mostRecentLeagueId)
         except ValueError:
-            raise ValueError(f"League ID '{leagueId}' could not be turned into an int.")
-        super().__init__(leagueId, years, **kwargs)
+            raise ValueError(f"League ID '{mostRecentLeagueId}' could not be turned into an int.")
+        super().__init__(mostRecentLeagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
         self.__clientId = clientId
         self.__clientSecret = clientSecret
-        self.__timeoutSeconds = kwargs.pop("loginTimeoutSeconds", self.__LOGIN_TIMEOUT_SECONDS)
+        self.__loginTimeoutSeconds = loginTimeoutSeconds
         self.__yahooManagerIdToOwnerMap: dict[int, Owner] = dict()
         self.__yahooTeamIdToTeamMap: dict[str, Team] = dict()
         self.__yearToTeamIdHasLostInPlayoffs: dict[int, dict[int, bool]] = dict()
 
-    @classmethod
-    def login(cls, clientId: str, clientSecret: str) -> None:
+    def login(self, clientId: str, clientSecret: str) -> None:
         """
         Logs in via Yahoo OAuth.
         Will open up a browser window.
         """
         CLIENT_ID_OPTION = "--client-id"
         CLIENT_SECRET_OPTION = "--client-secret"
         subprocess.call(
@@ -64,43 +71,41 @@
         )
 
     def __getAllLeagues(self) -> list[YahooLeague]:
         loginProcess = multiprocessing.Process(
             target=self.login, args=(self.__clientId, self.__clientSecret)
         )
         loginProcess.start()
-        loginProcess.join(self.__timeoutSeconds)
+        loginProcess.join(self.__loginTimeoutSeconds)
         if loginProcess.is_alive():
             loginProcess.terminate()
             raise TimeoutError("Login to yahoofantasy timed out.")
-        ctx = Context()
+        yahooContext = YahooContext()
         yahooLeagues = list()
-        nextLeagueId = self._leagueId
-        remainingYears = self._years.copy()
-        foundYears = list()
-        while len(remainingYears) > 0 and nextLeagueId is not None:
+        # years from most -> least recent
+        remainingYears = sorted(self._years, reverse=True)
+        currentLeagueId = self._leagueId
+        previousLeagueId = None
+        for year in remainingYears:
+            foundLeagueForYear = False
             # get all leagues this user was in for this year
-            currentYear = remainingYears[0]
-            leagues = ctx.get_leagues(self.__NFL, currentYear)
-            # find the league ID we want
+            leagues = yahooContext.get_leagues(self.__NFL, year)
+            # find the league that we want (has a matching ID)
             for league in leagues:
-                if str(league.league_id) == nextLeagueId:
+                if str(league.league_id) == currentLeagueId:
                     yahooLeagues.append(league)
-                    foundYears.append(currentYear)
-                    nextLeagueId = league.renew
-                    if nextLeagueId is not None:
-                        nextLeagueId = str(nextLeagueId)[3:]
-                        break
-            remainingYears.pop(0)
-
-        if len(yahooLeagues) != len(self._years):
-            # TODO: Give a more descriptive // accurate error message
-            raise DoesNotExistException(
-                f"Found years {foundYears}, expected to find {self._years}."
-            )
+                    foundLeagueForYear = True
+                    previousLeagueId = league.past_league_id
+            if not foundLeagueForYear:
+                raise LeagueLoaderException(
+                    f"Could not find league for year {year} with ID {currentLeagueId}."
+                )
+            currentLeagueId = previousLeagueId
+
+        self._validateRetrievedLeagues(yahooLeagues)
         return yahooLeagues
 
     def getOwnerNames(self) -> dict[int, list[str]]:
         yearToOwnerNamesMap: dict[int, list[str]] = dict()
         yahooLeagues = self.__getAllLeagues()
         for yahooLeague in yahooLeagues:
             yearToOwnerNamesMap[yahooLeague.season] = list()
@@ -116,21 +121,23 @@
         if validate:
             # validate new league
             leagueValidation.runAllChecks(league)
         return league
 
     def __buildLeague(self, yahooLeagues: list[YahooLeague]) -> League:
         years = list()
-        leagueName = None
         for yahooLeague in yahooLeagues:
-            leagueName = yahooLeague.name if leagueName is None else leagueName
+            # save league name for each year
+            self._leagueNameByYear[yahooLeague.season] = yahooLeague.name
             self.__loadOwners(yahooLeague.teams())
             years.append(self.__buildYear(yahooLeague))
         return League(
-            name=leagueName, owners=list(self.__yahooManagerIdToOwnerMap.values()), years=years
+            name=self._getLeagueName(),
+            owners=list(self.__yahooManagerIdToOwnerMap.values()),
+            years=self._getValidYears(years),
         )
 
     def __buildYear(self, yahooLeague: YahooLeague) -> Year:
         self.__yearToTeamIdHasLostInPlayoffs[yahooLeague.season] = dict()
         teams = self.__buildTeams(yahooLeague.teams())
         weeks = self.__buildWeeks(yahooLeague)
         return Year(yearNumber=yahooLeague.season, teams=teams, weeks=weeks)
@@ -140,24 +147,24 @@
         for i in range(
             yahooLeague.current_week
         ):  # current week seems to be the last week in the league
             yahooWeek: YahooWeek = yahooLeague.weeks()[i]
             # get each teams matchup for that week
             matchups = list()
             # only get matchups that are completed
-            validMatchups = [m for m in yahooWeek.matchups if m.status == "postevent"]
-            for yahooMatchup in validMatchups:
+            validYahooMatchups = [m for m in yahooWeek.matchups if m.status == "postevent"]
+            for yahooMatchup in validYahooMatchups:
                 # team A is *this* team
-                yahooTeamA = yahooMatchup.team1
-                teamA = self.__yahooTeamIdToTeamMap[yahooMatchup.team1.team_id]
-                teamAScore = yahooMatchup.teams.team[0].team_points.total
+                yahooTeamA = yahooMatchup.teams.team[0]
+                teamA = self.__yahooTeamIdToTeamMap[yahooTeamA.team_id]
+                teamAScore = yahooTeamA.team_points.total
                 # team B is their opponent
-                yahooTeamB = yahooMatchup.team2
-                teamB = self.__yahooTeamIdToTeamMap[yahooMatchup.team2.team_id]
-                teamBScore = yahooMatchup.teams.team[1].team_points.total
+                yahooTeamB = yahooMatchup.teams.team[1]
+                teamB = self.__yahooTeamIdToTeamMap[yahooTeamB.team_id]
+                teamBScore = yahooTeamB.team_points.total
                 # figure out tiebreakers if there needs to be one
                 teamAHasTiebreaker = False
                 teamBHasTiebreaker = False
                 if yahooMatchup.is_tied == 0:
                     # non-tied matchup
                     teamAHasTiebreaker = yahooMatchup.winner_team_key == yahooTeamA.team_key
                     teamBHasTiebreaker = yahooMatchup.winner_team_key == yahooTeamB.team_key
@@ -174,44 +181,45 @@
                     )
                 )
             if len(matchups) > 0:
                 weeks.append(Week(weekNumber=i + 1, matchups=matchups))
         return weeks
 
     def __getMatchupType(self, yahooMatchup: YahooMatchup) -> MatchupType:
-        team1Id = yahooMatchup.team1.team_id
-        team2Id = yahooMatchup.team2.team_id
+        team1Id = yahooMatchup.teams.team[0].team_id
+        team2Id = yahooMatchup.teams.team[1].team_id
         # check if this is a playoff week
         if yahooMatchup.is_playoffs == 1:
             # figure out if this is the last week of playoffs (the championship week)
             if yahooMatchup.week == yahooMatchup.league.end_week:
                 # this is the championship week
-                # figure out if either team has lost in the playoffs yet
+                # figure out if either team has lost in the playoffs yet (or hasn't played in the playoffs yet, in case their first game is the championship)
                 if (
-                    team1Id in self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season]
-                    and not self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
+                    (
                         team1Id
-                    ]
-                    and team2Id in self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season]
-                    and not self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
+                        not in self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season]
+                        or not self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
+                            team1Id
+                        ]
+                    )
+                    and (
                         team2Id
-                    ]
+                        not in self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season]
+                        or not self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
+                            team2Id
+                        ]
+                    )
                     and yahooMatchup.is_consolation == 0
                 ):
                     return MatchupType.CHAMPIONSHIP
-            # update class dict with the team that lost
+            # update tracking dict with the team that lost
             for yahooTeamResult in yahooMatchup.teams.team:
-                if yahooTeamResult.win_probability == 0:
-                    self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
-                        yahooTeamResult.team_id
-                    ] = True
-                elif yahooTeamResult.win_probability == 1:
-                    self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
-                        yahooTeamResult.team_id
-                    ] = False
+                self.__yearToTeamIdHasLostInPlayoffs[yahooMatchup.league.season][
+                    yahooTeamResult.team_id
+                ] = (yahooTeamResult.team_key != yahooMatchup.winner_team_key)
             return MatchupType.PLAYOFF
         else:
             return MatchupType.REGULAR_SEASON
 
     def __buildTeams(self, yahooTeams: list[YahooTeam]) -> list[Team]:
         teams = list()
         for yahooTeam in yahooTeams:
```

### Comparing `leeger-2.3.0/leeger/model/abstract/UniqueId.py` & `leeger-2.4.0/leeger/model/abstract/UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/model/filter/AllTimeFilters.py` & `leeger-2.4.0/leeger/model/filter/AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/model/filter/YearFilters.py` & `leeger-2.4.0/leeger/model/filter/YearFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/model/league/League.py` & `leeger-2.4.0/leeger/model/league/League.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import copy
 from dataclasses import dataclass
 
 from leeger.exception import DoesNotExistException
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Year import Year
+from leeger.util.CustomLogger import CustomLogger
+from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
 
 
 @dataclass(kw_only=True, eq=False)
 class League(UniqueId, JSONSerializable, JSONDeserializable):
+    __LOGGER = CustomLogger.getLogger()
     name: str
     owners: list[Owner]
     years: list[Year]
 
     def __hash__(self):
         return hash(str(self.toJson()))
 
@@ -24,14 +27,22 @@
         """
         Checks if *this* League is the same as the given League.
         Does not check for equality of IDs, just values.
         """
         equal = self.name == otherLeague.name
         equal = equal and self.owners == otherLeague.owners
         equal = equal and self.years == otherLeague.years
+        if not equal:
+            differences = GeneralUtil.findDifferentFields(
+                self.toJson(),
+                otherLeague.toJson(),
+                parentKey="League",
+                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
+            )
+            self.__LOGGER.info(f"Differences: {differences}")
         return equal
 
     def __add__(self, otherLeague: League) -> League:
         """
         Combines *this* League with the given League.
         The combined League will be validated before it is returned.
```

### Comparing `leeger-2.3.0/leeger/model/league/Matchup.py` & `leeger-2.4.0/leeger/model/league/Matchup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception import DoesNotExistException
 from leeger.exception.InvalidMatchupFormatException import InvalidMatchupFormatException
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.model.league_helper.Performance import Performance
 from leeger.util.CustomLogger import CustomLogger
+from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
 
 
 @dataclass(kw_only=True, eq=False)
 class Matchup(UniqueId, JSONSerializable, JSONDeserializable):
     __LOGGER = CustomLogger.getLogger()
@@ -52,18 +53,28 @@
         # warn if this is going to return True but ID based fields are not equal
         if equal:
             notEqualStrings = list()
             if self.teamAId != otherMatchup.teamAId:
                 notEqualStrings.append("teamAId")
             if self.teamBId != otherMatchup.teamBId:
                 notEqualStrings.append("teamBId")
+            if self.multiWeekMatchupId != otherMatchup.multiWeekMatchupId:
+                notEqualStrings.append("multiWeekMatchupId")
             if len(notEqualStrings) > 0:
                 self.__LOGGER.warning(
                     f"Returning True for equality check when {notEqualStrings} are not equal."
                 )
+        else:
+            differences = GeneralUtil.findDifferentFields(
+                self.toJson(),
+                otherMatchup.toJson(),
+                parentKey="Matchup",
+                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
+            )
+            self.__LOGGER.info(f"Differences: {differences}")
         return equal
 
     def splitToPerformances(self) -> tuple[Performance, Performance]:
         """
         Splits this Matchup into 2 Performances.
         """
         performanceA = Performance(
```

### Comparing `leeger-2.3.0/leeger/model/league/Team.py` & `leeger-2.4.0/leeger/model/league/Team.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.util.CustomLogger import CustomLogger
+from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
 
 
 @dataclass(kw_only=True, eq=False)
 class Team(UniqueId, JSONSerializable, JSONDeserializable):
     __LOGGER = CustomLogger.getLogger()
@@ -18,19 +19,26 @@
         """
         Checks if *this* Team is the same as the given Team.
         Does not check for equality of IDs, just values.
         """
         equal = self.name == otherTeam.name
         # warn if this is going to return True but ID based fields are not equal
         if equal:
-            notEqualStrings = list()
             if self.ownerId != otherTeam.ownerId:
                 self.__LOGGER.warning(
                     f"Returning True for equality check when ownerIds are not equal."
                 )
+        else:
+            differences = GeneralUtil.findDifferentFields(
+                self.toJson(),
+                otherTeam.toJson(),
+                parentKey="Team",
+                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
+            )
+            self.__LOGGER.info(f"Differences: {differences}")
         return equal
 
     def toJson(self) -> dict:
         return {"id": self.id, "ownerId": self.ownerId, "name": self.name}
 
     @staticmethod
     def fromJson(d: dict) -> Team:
```

### Comparing `leeger-2.3.0/leeger/model/league/Week.py` & `leeger-2.4.0/leeger/model/league/Week.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,41 @@
 
 from dataclasses import dataclass
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception import DoesNotExistException
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.model.league.Matchup import Matchup
+from leeger.util.CustomLogger import CustomLogger
+from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
 
 
 @dataclass(kw_only=True, eq=False)
 class Week(UniqueId, JSONSerializable, JSONDeserializable):
+    __LOGGER = CustomLogger.getLogger()
     weekNumber: int
     matchups: list[Matchup]
 
     def __eq__(self, otherWeek: Week) -> bool:
         """
         Checks if *this* Week is the same as the given Week.
         Does not check for equality of IDs, just values.
         """
         equal = self.weekNumber == otherWeek.weekNumber
         equal = equal and self.matchups == otherWeek.matchups
+        if not equal:
+            differences = GeneralUtil.findDifferentFields(
+                self.toJson(),
+                otherWeek.toJson(),
+                parentKey="Week",
+                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
+            )
+            self.__LOGGER.info(f"Differences: {differences}")
         return equal
 
     @property
     def isPlayoffWeek(self) -> bool:
         isPlayoffWeek = False
         for matchup in self.matchups:
             if matchup.matchupType == MatchupType.PLAYOFF:
```

### Comparing `leeger-2.3.0/leeger/model/league/Year.py` & `leeger-2.4.0/leeger/model/league/Year.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 from typing import Optional
 
 from leeger.exception import DoesNotExistException
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.YearSettings import YearSettings
+from leeger.util.CustomLogger import CustomLogger
+from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
 
 
 @dataclass(kw_only=True, eq=False)
 class Year(UniqueId, JSONSerializable, JSONDeserializable):
+    __LOGGER = CustomLogger.getLogger()
     yearNumber: int
     teams: list[Team]
     weeks: list[Week]
     yearSettings: Optional[YearSettings] = None
 
     def __post_init__(self):
         if self.yearSettings is None:
@@ -31,14 +34,22 @@
         Checks if *this* Year is the same as the given Year.
         Does not check for equality of IDs, just values.
         """
         equal = self.yearNumber == otherYear.yearNumber
         equal = equal and self.teams == otherYear.teams
         equal = equal and self.weeks == otherYear.weeks
         equal = equal and self.yearSettings == otherYear.yearSettings
+        if not equal:
+            differences = GeneralUtil.findDifferentFields(
+                self.toJson(),
+                otherYear.toJson(),
+                parentKey="Year",
+                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
+            )
+            self.__LOGGER.info(f"Differences: {differences}")
         return equal
 
     def getTeamByName(self, teamName: str) -> Team:
         """
         Returns the Team with the given team name.
         """
         for team in self.teams:
```

### Comparing `leeger-2.3.0/leeger/model/league/YearSettings.py` & `leeger-2.4.0/leeger/model/league/YearSettings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
+from leeger.util.CustomLogger import CustomLogger
+from leeger.util.GeneralUtil import GeneralUtil
 
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
 
 
 @dataclass(kw_only=True, eq=False)
 class YearSettings(JSONSerializable, JSONDeserializable):
+    __LOGGER = CustomLogger.getLogger()
     leagueMedianGames: Optional[bool] = False
 
     def __post_init__(self):
         if self.leagueMedianGames is None:
             self.leagueMedianGames = False
 
     def __eq__(self, otherYearSettings: YearSettings) -> bool:
         """
         Checks if *this* YearSettings is the same as the given YearSettings.
         """
-        return self.leagueMedianGames == otherYearSettings.leagueMedianGames
+        equal = self.leagueMedianGames == otherYearSettings.leagueMedianGames
+        if not equal:
+            differences = GeneralUtil.findDifferentFields(
+                self.toJson(),
+                otherYearSettings.toJson(),
+                parentKey="YearSettings",
+                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
+            )
+            self.__LOGGER.info(f"Differences: {differences}")
+        return equal
 
     def toJson(self) -> dict:
         return {"leagueMedianGames": self.leagueMedianGames}
 
     @staticmethod
     def fromJson(d: dict) -> YearSettings:
         return YearSettings(leagueMedianGames=d.get("leagueMedianGames"))
```

### Comparing `leeger-2.3.0/leeger/model/league_helper/Performance.py` & `leeger-2.4.0/leeger/model/league_helper/Performance.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/model/stat/AllTimeStatSheet.py` & `leeger-2.4.0/leeger/model/stat/AllTimeStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/model/stat/YearStatSheet.py` & `leeger-2.4.0/leeger/model/stat/YearStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/CustomFormatter.py` & `leeger-2.4.0/leeger/util/CustomFormatter.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/CustomLogger.py` & `leeger-2.4.0/leeger/util/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/Deci.py` & `leeger-2.4.0/leeger/util/Deci.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/excel.py` & `leeger-2.4.0/leeger/util/excel.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/excel_helper.py` & `leeger-2.4.0/leeger/util/excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/navigator/LeagueNavigator.py` & `leeger-2.4.0/leeger/util/navigator/LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/navigator/MatchupNavigator.py` & `leeger-2.4.0/leeger/util/navigator/MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/navigator/WeekNavigator.py` & `leeger-2.4.0/leeger/util/navigator/WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/navigator/YearNavigator.py` & `leeger-2.4.0/leeger/util/navigator/YearNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/util/stat_sheet.py` & `leeger-2.4.0/leeger/util/stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/validate/leagueValidation.py` & `leeger-2.4.0/leeger/validate/leagueValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/validate/matchupValidation.py` & `leeger-2.4.0/leeger/validate/matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/validate/teamValidation.py` & `leeger-2.4.0/leeger/validate/teamValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/validate/weekValidation.py` & `leeger-2.4.0/leeger/validate/weekValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/leeger/validate/yearValidation.py` & `leeger-2.4.0/leeger/validate/yearValidation.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
                     multiWeekMatchupIdToCountAndMostRecentWeekMap[mwmid][0] += 1
                 else:
                     multiWeekMatchupIdToCountAndMostRecentWeekMap[mwmid] = [
                         1,
                         isMostRecentWeekInYear,
                     ]
 
-    for (mwmid, countAndMostRecentWeek) in multiWeekMatchupIdToCountAndMostRecentWeekMap.items():
+    for mwmid, countAndMostRecentWeek in multiWeekMatchupIdToCountAndMostRecentWeekMap.items():
         count, isMostRecentWeek = countAndMostRecentWeek
         if count == 1 and not isMostRecentWeek:
             raise InvalidYearFormatException(
                 f"Year {year.yearNumber} has multi-week matchup with ID '{mwmid}' that only occurs once and is not the most recent week."
             )
```

### Comparing `leeger-2.3.0/leeger.egg-info/PKG-INFO` & `leeger-2.4.0/leeger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.3.0
+Version: 2.4.0
 Summary: Instant stats for your fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
@@ -154,15 +154,15 @@
 found [here](https://github.com/joeyagreco/leeger/blob/main/example/league/combiningLeagues.py).
 ___
 **Q:**
 Can I disable validation on my League object?
 
 **A:**
 Yes. While it is not recommended that you disable this, as validation ensures the stats are calculated properly,
-disabling validation can be done by passing `validate=False` into any method that takes a League object.
+disabling validation can be done by passing `validate=False` into any method that takes a League object OR any `loadLeague()` method from a League Loader.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install.
 
 ```bash
 pip install leeger
@@ -203,14 +203,22 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Development
+
+### Formatting
+
+_Run these commands from the root folder (leeger) before committing._\
+**General Format:** `black --config=pyproject.toml . `\
+**Import/Variable Format:** `autoflake --config=pyproject.toml .`
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Credit
 
 - [ESPN API](https://github.com/cwendt94/espn-api)
```

### Comparing `leeger-2.3.0/leeger.egg-info/SOURCES.txt` & `leeger-2.4.0/leeger.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 leeger/__init__.py
 leeger/_version.py
 leeger.egg-info/PKG-INFO
 leeger.egg-info/SOURCES.txt
 leeger.egg-info/dependency_links.txt
@@ -127,14 +128,15 @@
 test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
 test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
 test/test_decorator/__init__.py
 test/test_decorator/test_validators.py
 test/test_league_loader/__init__.py
 test/test_league_loader/test_ESPNLeagueLoader.py
 test/test_league_loader/test_FleaflickerLeagueLoader.py
+test/test_league_loader/test_LeagueLoader.py
 test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
 test/test_league_loader/test_SleeperLeagueLoader.py
 test/test_league_loader/test_YahooLeagueLoader.py
 test/test_model/__init__.py
 test/test_model/test_abstract/__init__.py
 test/test_model/test_abstract/test_UniqueId.py
 test/test_model/test_filter/__init__.py
```

### Comparing `leeger-2.3.0/setup.py` & `leeger-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py` & `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py` & `leeger-2.4.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_decorator/test_validators.py` & `leeger-2.4.0/test/test_decorator/test_validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_abstract/test_UniqueId.py` & `leeger-2.4.0/test/test_model/test_abstract/test_UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_filter/test_AllTimeFilters.py` & `leeger-2.4.0/test/test_model/test_filter/test_AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_League.py` & `leeger-2.4.0/test/test_model/test_league/test_League.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_Matchup.py` & `leeger-2.4.0/test/test_model/test_league/test_Matchup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_Owner.py` & `leeger-2.4.0/test/test_model/test_league/test_Owner.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_Team.py` & `leeger-2.4.0/test/test_model/test_league/test_Team.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_Week.py` & `leeger-2.4.0/test/test_model/test_league/test_Week.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_Year.py` & `leeger-2.4.0/test/test_model/test_league/test_Year.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league/test_YearSettings.py` & `leeger-2.4.0/test/test_model/test_league/test_YearSettings.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_model/test_league_helper/test_Performance.py` & `leeger-2.4.0/test/test_model/test_league_helper/test_Performance.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_util/test_excel.py` & `leeger-2.4.0/test/test_util/test_excel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1759,15 +1759,14 @@
                         if isinstance(cell1Value, Decimal):
                             cell1Value = float(cell1Value)
                         if isinstance(cell2Value, Decimal):
                             cell2Value = float(cell2Value)
                         self.assertAlmostEqual(cell1Value, cell2Value)
 
     def test_leagueToExcel_leagueIsNone_raisesException(self):
-
         with self.assertRaises(ValueError) as context:
             leagueToExcel(None, "")
         self.assertEqual("'league' has not been set.", str(context.exception))
 
     def test_leagueToExcel_fileAlreadyExists_raisesException(self):
         owners, teams1 = getNDefaultOwnersAndTeams(2)
         teams1[0].name = "a"
```

### Comparing `leeger-2.3.0/test/test_util/test_excel_helper.py` & `leeger-2.4.0/test/test_util/test_excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_util/test_navigator/test_LeagueNavigator.py` & `leeger-2.4.0/test/test_util/test_navigator/test_LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_util/test_navigator/test_MatchupNavigator.py` & `leeger-2.4.0/test/test_util/test_navigator/test_MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_util/test_navigator/test_WeekNavigator.py` & `leeger-2.4.0/test/test_util/test_navigator/test_WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_util/test_navigator/test_YearNavigator.py` & `leeger-2.4.0/test/test_util/test_navigator/test_YearNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_util/test_stat_sheet.py` & `leeger-2.4.0/test/test_util/test_stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_leagueValidation.py` & `leeger-2.4.0/test/test_validate/test_leagueValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_matchupValidation.py` & `leeger-2.4.0/test/test_validate/test_matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_ownerValidation.py` & `leeger-2.4.0/test/test_validate/test_ownerValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_teamValidation.py` & `leeger-2.4.0/test/test_validate/test_teamValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_weekValidation.py` & `leeger-2.4.0/test/test_validate/test_weekValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_yearSettingsValidation.py` & `leeger-2.4.0/test/test_validate/test_yearSettingsValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.3.0/test/test_validate/test_yearValidation.py` & `leeger-2.4.0/test/test_validate/test_yearValidation.py`

 * *Files identical despite different names*

