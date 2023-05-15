# Comparing `tmp/rateslib-0.1.0.tar.gz` & `tmp/rateslib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateslib-0.1.0.tar", last modified: Mon Apr 24 18:45:31 2023, max compression
+gzip compressed data, was "rateslib-0.2.0.tar", last modified: Mon May 15 18:25:25 2023, max compression
```

## Comparing `rateslib-0.1.0.tar` & `rateslib-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.258394 rateslib-0.1.0/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.1.0/LICENSE
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-04-24 18:45:31.257970 rateslib-0.1.0/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.1.0/README.md
--rw-r--r--   0 Darbyshire   (501) staff       (20)      799 2023-04-24 18:27:13.000000 rateslib-0.1.0/pyproject.toml
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.091678 rateslib-0.1.0/rateslib/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     4576 2023-04-23 07:34:25.000000 rateslib-0.1.0/rateslib/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    22387 2023-03-31 16:14:49.000000 rateslib-0.1.0/rateslib/calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    53603 2023-04-24 18:22:38.000000 rateslib-0.1.0/rateslib/curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     3299 2023-04-17 18:48:46.000000 rateslib-0.1.0/rateslib/defaults.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23398 2023-04-17 18:48:46.000000 rateslib-0.1.0/rateslib/dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    64353 2023-04-19 18:21:10.000000 rateslib-0.1.0/rateslib/fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   207218 2023-04-24 15:23:12.000000 rateslib-0.1.0/rateslib/instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    65006 2023-04-24 04:46:29.000000 rateslib-0.1.0/rateslib/legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    52971 2023-04-24 17:06:01.000000 rateslib-0.1.0/rateslib/periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    45487 2023-03-31 17:09:16.000000 rateslib-0.1.0/rateslib/scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    66561 2023-04-24 16:41:08.000000 rateslib-0.1.0/rateslib/solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    16882 2023-03-31 16:24:01.000000 rateslib-0.1.0/rateslib/splines.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.101595 rateslib-0.1.0/rateslib.egg-info/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)      654 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/SOURCES.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/dependency_links.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)      142 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/requires.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/top_level.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-04-24 18:45:31.258464 rateslib-0.1.0/setup.cfg
--rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.1.0/setup.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.250350 rateslib-0.1.0/tests/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     8187 2023-03-05 18:52:18.000000 rateslib-0.1.0/tests/test_calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    18964 2023-03-31 16:52:57.000000 rateslib-0.1.0/tests/test_curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    22577 2023-04-17 18:48:46.000000 rateslib-0.1.0/tests/test_dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    28832 2023-04-24 16:35:20.000000 rateslib-0.1.0/tests/test_fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    63272 2023-04-17 18:48:46.000000 rateslib-0.1.0/tests/test_instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    27553 2023-04-01 10:40:19.000000 rateslib-0.1.0/tests/test_legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    32684 2023-04-17 18:48:46.000000 rateslib-0.1.0/tests/test_periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    24516 2023-03-20 17:46:32.000000 rateslib-0.1.0/tests/test_scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    32047 2023-04-24 17:06:01.000000 rateslib-0.1.0/tests/test_solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.1.0/tests/test_splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.126181 rateslib-0.2.0/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.2.0/LICENSE
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-05-15 18:25:25.125729 rateslib-0.2.0/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.2.0/README.md
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      779 2023-05-15 17:52:21.000000 rateslib-0.2.0/pyproject.toml
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.008758 rateslib-0.2.0/rateslib/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     4459 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/__init__.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23171 2023-05-15 17:59:17.000000 rateslib-0.2.0/rateslib/calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    57996 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     3536 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/default.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    25348 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    65162 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)   234743 2023-05-15 18:06:24.000000 rateslib-0.2.0/rateslib/instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    71323 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    62756 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    47001 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    67841 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    17008 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.026673 rateslib-0.2.0/rateslib.egg-info/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      653 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/SOURCES.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/dependency_links.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      129 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/requires.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/top_level.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-05-15 18:25:25.126276 rateslib-0.2.0/setup.cfg
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.2.0/setup.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.118447 rateslib-0.2.0/tests/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     8187 2023-03-05 18:52:18.000000 rateslib-0.2.0/tests/test_calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    25127 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23147 2023-05-06 20:57:27.000000 rateslib-0.2.0/tests/test_dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    28832 2023-04-24 16:35:20.000000 rateslib-0.2.0/tests/test_fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    88567 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    31919 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    43128 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    24515 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    34007 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.2.0/tests/test_splines.py
```

### Comparing `rateslib-0.1.0/LICENSE` & `rateslib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rateslib-0.1.0/PKG-INFO` & `rateslib-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
```

### Comparing `rateslib-0.1.0/README.md` & `rateslib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rateslib-0.1.0/pyproject.toml` & `rateslib-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateslib"
-version = "0.1.0"
+version = "0.2.0"
 description = "A fixed income library for trading interest rates"
 readme = "README.md"
 authors = [{ name = "J H M Darbyshire"}]
 license = { file = "LICENSE" }
 keywords = ["interest rate", "derivatives", "swaps", "bonds", "fixed income"]
 dependencies = [
     "numpy>=1.21.5",
-    "scipy>=1.8.0",
     "matplotlib>=3.5.1",
     "pandas>=1.4.1",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `rateslib-0.1.0/rateslib/__init__.py` & `rateslib-0.2.0/rateslib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 __docformat__ = "restructuredtext"
 
 # Let users know if they're missing any of our hard dependencies
-_hard_dependencies = ("pandas", "scipy", "matplotlib", "numpy")
+_hard_dependencies = ("pandas", "matplotlib", "numpy")
 _missing_dependencies = []
 
 for _dependency in _hard_dependencies:
     try:
         __import__(_dependency)
     except ImportError as _e:  # pragma: no cover
         raise ImportError(f"`rateslib` requires installation of {_dependency}: {_e}")
 
 from datetime import datetime as dt
 
-from rateslib.defaults import Defaults
+from rateslib.default import Defaults
+
 defaults = Defaults()
 
 from contextlib import ContextDecorator
+
+
 class default_context(ContextDecorator):
     """
     Context manager to temporarily set options in the `with` statement context.
 
     You need to invoke as ``option_context(pat, val, [(pat, val), ...])``.
 
     Examples
@@ -44,71 +47,43 @@
 
     def __exit__(self, *args) -> None:
         if self.undo:
             for pat, val in self.undo:
                 setattr(defaults, pat, val)
 
 
-from rateslib.dual import (
-    Dual,
-    Dual2,
-    dual_log,
-    dual_exp,
-    dual_solve
-)
+from rateslib.dual import Dual, Dual2, dual_log, dual_exp, dual_solve
 
-from rateslib.calendars import (
-    create_calendar,
-    get_calendar,
-    add_tenor,
-    dcf
-)
+from rateslib.calendars import create_calendar, get_calendar, add_tenor, dcf
 
-from rateslib.splines import (
-    bsplev_single,
-    bspldnev_single,
-    PPSpline
-)
+from rateslib.splines import bsplev_single, bspldnev_single, PPSpline
 
-from rateslib.scheduling import (
-    Schedule
-)
+from rateslib.scheduling import Schedule
 
-from rateslib.curves import (
-    Curve,
-    LineCurve,
-    interpolate,
-    index_left
-)
+from rateslib.curves import Curve, LineCurve, interpolate, index_left
 
 from rateslib.fx import (
     FXRates,
     FXForwards,
     ProxyCurve,
 )
 
-from rateslib.solver import (
-    Solver
-)
+from rateslib.solver import Solver
 
-from rateslib.periods import (
-    FixedPeriod,
-    FloatPeriod,
-    Cashflow
-)
+from rateslib.periods import FixedPeriod, FloatPeriod, Cashflow
 
 from rateslib.legs import (
     FixedLeg,
     FixedLegExchange,
     FixedLegExchangeMtm,
     FloatLeg,
     FloatLegExchange,
     FloatLegExchangeMtm,
     ZeroFloatLeg,
-    CustomLeg
+    CustomLeg,
 )
 
 from rateslib.instruments import (
     Value,
     Bill,
     FixedRateBond,
     FloatRateBond,
@@ -214,8 +189,8 @@
     "FixedFixedXCS",
     "FixedFloatXCS",
     "FloatFixedXCS",
     "XCS",
     "Spread",
     "Fly",
     "Portfolio",
-]
+]
```

### Comparing `rateslib-0.1.0/rateslib/calendars.py` & `rateslib-0.2.0/rateslib/calendars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,123 +1,151 @@
-from typing import Optional, Union
+from typing import Optional, Union, Dict, Any
 from math import floor
 from datetime import datetime, timedelta
 import calendar as calendar_mod
+
+from dateutil.relativedelta import MO, TH, FR
+
 from pandas.tseries.holiday import (
     AbstractHolidayCalendar,
     Holiday,
     next_monday,
-    DateOffset,
     next_monday_or_tuesday,
-    MO,
-    TH,
-    FR,
 )
-from pandas.tseries.offsets import CustomBusinessDay, Easter, Day
+from pandas.tseries.offsets import CustomBusinessDay, Easter, Day, DateOffset
 
+CalInput = Optional[Union[CustomBusinessDay, str]]
 
 # Generic holidays
-Epiphany = Holiday('Epiphany', month=1, day=6)
+Epiphany = Holiday("Epiphany", month=1, day=6)
 GoodFriday = Holiday("Good Friday", month=1, day=1, offset=[Easter(), Day(-2)])
 EasterMonday = Holiday("Easter Monday", month=1, day=1, offset=[Easter(), Day(1)])
-AscentionDay = Holiday('Ascention Day', month=1, day=1, offset=[Easter(), Day(39)])
+AscentionDay = Holiday("Ascention Day", month=1, day=1, offset=[Easter(), Day(39)])
 ChristmasEve = Holiday("Christmas Eve", month=12, day=24)
-ChristmasDay = Holiday('Christmas Day', month=12, day=25)
-ChristmasDayHoliday = Holiday("Christmas Day Holiday", month=12, day=25, observance=next_monday_or_tuesday)
-BoxingDay = Holiday('Boxing Day', month=12, day=26)
-BoxingDayHoliday = Holiday("Boxing Day Holiday", month=12, day=26, observance=next_monday_or_tuesday)
+ChristmasDay = Holiday("Christmas Day", month=12, day=25)
+ChristmasDayHoliday = Holiday(
+    "Christmas Day Holiday", month=12, day=25, observance=next_monday_or_tuesday
+)
+BoxingDay = Holiday("Boxing Day", month=12, day=26)
+BoxingDayHoliday = Holiday(
+    "Boxing Day Holiday", month=12, day=26, observance=next_monday_or_tuesday
+)
 NewYearsEve = Holiday("New Year's Eve", month=12, day=31)
 NewYearsDay = Holiday("New Year's Day", month=1, day=1)
-NewYearsDayHoliday = Holiday("New Year's Day Holiday", month=1, day=1, observance=next_monday)
+NewYearsDayHoliday = Holiday(
+    "New Year's Day Holiday", month=1, day=1, observance=next_monday
+)
 
 # US based
-USMartinLutherKingJr = Holiday('Dr. Martin Luther King Jr.', start_date=datetime(1986, 1, 1), month=1, day=1, offset=DateOffset(weekday=MO(3)))
-USPresidentsDay = Holiday('US President''s Day', month=2, day=1, offset=DateOffset(weekday=MO(3)))
-USMemorialDay = Holiday('US Memorial Day', month=5, day=31, offset=DateOffset(weekday=MO(-1)))
+USMartinLutherKingJr = Holiday(
+    "Dr. Martin Luther King Jr.",
+    start_date=datetime(1986, 1, 1),
+    month=1,
+    day=1,
+    offset=DateOffset(weekday=MO(3)),  # type: ignore[arg-type]
+)
+USPresidentsDay = Holiday(
+    "US President" "s Day", month=2, day=1, offset=DateOffset(weekday=MO(3))  # type: ignore[arg-type]
+)
+USMemorialDay = Holiday(
+    "US Memorial Day", month=5, day=31, offset=DateOffset(weekday=MO(-1))  # type: ignore[arg-type]
+)
 USIndependenceDay = Holiday("US Independence Day", month=7, day=4)
-USLabourDay = Holiday('US Labour Day', month=9, day=1, offset=DateOffset(weekday=MO(1)))
-USColumbusDay = Holiday('US Columbus Day', month=10, day=1, offset=DateOffset(weekday=MO(2)))
-USThanksgivingDay = Holiday('US Thanksgiving', month=11, day=1, offset=DateOffset(weekday=TH(4)))
+USLabourDay = Holiday("US Labour Day", month=9, day=1, offset=DateOffset(weekday=MO(1)))  # type: ignore[arg-type]
+USColumbusDay = Holiday(
+    "US Columbus Day", month=10, day=1, offset=DateOffset(weekday=MO(2))  # type: ignore[arg-type]
+)
+USThanksgivingDay = Holiday(
+    "US Thanksgiving", month=11, day=1, offset=DateOffset(weekday=TH(4))  # type: ignore[arg-type]
+)
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 # UK based
-UKEarlyMayBankHoliday = Holiday("UK Early May Bank Holiday", month=5, day=1, offset=DateOffset(weekday=MO(1)))
-UKSpringBankHoliday = Holiday("UK Spring Bank Holiday", month=5, day=31, offset=DateOffset(weekday=MO(-1)))
-UKSummerBankHoliday = Holiday("UK Summer Bank Holiday", month=8, day=31, offset=DateOffset(weekday=MO(-1)))
+UKEarlyMayBankHoliday = Holiday(
+    "UK Early May Bank Holiday", month=5, day=1, offset=DateOffset(weekday=MO(1))  # type: ignore[arg-type]
+)
+UKSpringBankHoliday = Holiday(
+    "UK Spring Bank Holiday", month=5, day=31, offset=DateOffset(weekday=MO(-1))  # type: ignore[arg-type]
+)
+UKSummerBankHoliday = Holiday(
+    "UK Summer Bank Holiday", month=8, day=31, offset=DateOffset(weekday=MO(-1))  # type: ignore[arg-type]
+)
 
 # EUR based
 EULabourDay = Holiday("EU Labour Day", month=5, day=1)
-SwedenNational = Holiday('Sweden National Day', month=6, day=6)
-MidsummerFriday = Holiday('Swedish Midsummer', month=6, day=25, offset=DateOffset(weekday=FR(-1)))
+SwedenNational = Holiday("Sweden National Day", month=6, day=6)
+MidsummerFriday = Holiday(
+    "Swedish Midsummer", month=6, day=25, offset=DateOffset(weekday=FR(-1))  # type: ignore[arg-type]
+)
 
-CALENDAR_RULES = {
+CALENDAR_RULES: Dict[str, list[Any]] = {
     "bus": [],
     "tgt": [
-      NewYearsDay,
-      GoodFriday,
-      EasterMonday,
-      EULabourDay,
-      ChristmasDay,
-      BoxingDay,
+        NewYearsDay,
+        GoodFriday,
+        EasterMonday,
+        EULabourDay,
+        ChristmasDay,
+        BoxingDay,
     ],
     "ldn": [
-      NewYearsDayHoliday,
-      GoodFriday,
-      EasterMonday,
-      UKEarlyMayBankHoliday,
-      UKSpringBankHoliday,
-      UKSummerBankHoliday,
-      ChristmasDayHoliday,
-      BoxingDayHoliday,
+        NewYearsDayHoliday,
+        GoodFriday,
+        EasterMonday,
+        UKEarlyMayBankHoliday,
+        UKSpringBankHoliday,
+        UKSummerBankHoliday,
+        ChristmasDayHoliday,
+        BoxingDayHoliday,
     ],
     "nyc": [
-      NewYearsDayHoliday,
-      GoodFriday,
-      EasterMonday,
-      UKEarlyMayBankHoliday,
-      UKSpringBankHoliday,
-      UKSummerBankHoliday,
-      ChristmasDayHoliday,
-      BoxingDayHoliday,
+        NewYearsDayHoliday,
+        GoodFriday,
+        EasterMonday,
+        UKEarlyMayBankHoliday,
+        UKSpringBankHoliday,
+        UKSummerBankHoliday,
+        ChristmasDayHoliday,
+        BoxingDayHoliday,
     ],
     "stk": [
-      NewYearsDay,
-      Epiphany,
-      GoodFriday,
-      EasterMonday,
-      EULabourDay,
-      AscentionDay,
-      SwedenNational,
-      MidsummerFriday,
-      ChristmasEve,
-      ChristmasDay,
-      BoxingDay,
-      NewYearsEve,
-     ],
+        NewYearsDay,
+        Epiphany,
+        GoodFriday,
+        EasterMonday,
+        EULabourDay,
+        AscentionDay,
+        SwedenNational,
+        MidsummerFriday,
+        ChristmasEve,
+        ChristmasDay,
+        BoxingDay,
+        NewYearsEve,
+    ],
     "osl": [
-      NewYearsDay,
-      Epiphany,
-      GoodFriday,
-      EasterMonday,
-      EULabourDay,
-      AscentionDay,
-      SwedenNational,
-      MidsummerFriday,
-      ChristmasEve,
-      ChristmasDay,
-      BoxingDay,
-      NewYearsEve,
-     ],
-  }
+        NewYearsDay,
+        Epiphany,
+        GoodFriday,
+        EasterMonday,
+        EULabourDay,
+        AscentionDay,
+        SwedenNational,
+        MidsummerFriday,
+        ChristmasEve,
+        ChristmasDay,
+        BoxingDay,
+        NewYearsEve,
+    ],
+}
 
 
-def create_calendar(rules: list, weekmask: str = None):
+def create_calendar(rules: list, weekmask: Optional[str] = None) -> CustomBusinessDay:
     """
     Create a calendar with specific business and holiday days defined.
 
     Parameters
     ----------
     rules : list[Holiday]
         A list of specific holiday dates defined by the
@@ -138,22 +166,28 @@
        TutsBday = Holiday("Tutankhamum Birthday", month=7, day=2)
        pyramid_builder = create_calendar(rules=[TutsBday], weekmask="Tue Wed Thu Fri Sat Sun")
        construction_days = date_range(dt(1999, 6, 25), dt(1999, 7, 5), freq=pyramid_builder)
        construction_days
 
     """
     weekmask = "Mon Tue Wed Thu Fri" if weekmask is None else weekmask
-    return CustomBusinessDay(calendar=AbstractHolidayCalendar(rules=rules), weekmask=weekmask)
+    return CustomBusinessDay(  # type: ignore[call-arg]
+        calendar=AbstractHolidayCalendar(rules=rules),
+        weekmask=weekmask,
+    )
+
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-def get_calendar(calendar: Optional[Union[CustomBusinessDay, str]], kind: bool = False):
+def get_calendar(
+    calendar: CalInput, kind: bool = False
+) -> Union[CustomBusinessDay, tuple[CustomBusinessDay, str]]:
     """
     Returns a calendar object either from an available set or a user defined input.
 
     Parameters
     ----------
     calendar : str, None, or CustomBusinessDay
         If `None` a blank calendar is returned containing no holidays.
@@ -185,25 +219,24 @@
 
     """
     if calendar is None:
         ret = (create_calendar([], weekmask="Mon Tue Wed Thu Fri Sat Sun"), "null")
     elif isinstance(calendar, str):
         calendars = calendar.lower().split(",")
         if len(calendars) == 1:  # only one named calendar is found
+            rules_: list[Any] = CALENDAR_RULES[calendars[0]]
             ret = (
-                create_calendar(
-                    CALENDAR_RULES[calendars[0]], weekmask="Mon Tue Wed Thu Fri"
-                ),
-                "named"
+                create_calendar(rules=rules_, weekmask="Mon Tue Wed Thu Fri"),
+                "named",
             )
         else:
-            rules = []
+            rules_ = []
             for c in calendars:
-                rules.extend(CALENDAR_RULES[c])
-            ret = (create_calendar(rules, weekmask="Mon Tue Wed Thu Fri"), "named")
+                rules_.extend(CALENDAR_RULES[c])
+            ret = (create_calendar(rules_, weekmask="Mon Tue Wed Thu Fri"), "named")
     else:  # calendar is a HolidayCalendar object
         ret = (calendar, "custom")
 
     return ret if kind else ret[0]
 
 
 def _is_holiday(date: datetime, calendar: CustomBusinessDay):
@@ -226,15 +259,15 @@
     else:
         return not (date + 0 * calendar == date)
 
 
 def _adjust_date(
     date: datetime,
     modifier: Optional[str],
-    calendar: Optional[Union[CustomBusinessDay, str]]
+    calendar: CalInput,
 ) -> datetime:
     """
     Modify a date under specific rule.
 
     Parameters
     ----------
     date : datetime
@@ -254,31 +287,31 @@
     modifier = modifier.upper()
     if modifier not in ["F", "MF", "P", "MP"]:
         raise ValueError("`modifier` must be in {None, 'F', 'MF', 'P', 'MP'}")
 
     (adj_op, mod_op) = (
         ("rollforward", "rollback") if "F" in modifier else ("rollback", "rollforward")
     )
-    calendar = get_calendar(calendar)
-
-    adjusted_date = getattr(calendar, adj_op)(date)
+    calendar_: CustomBusinessDay = get_calendar(calendar)  # type: ignore[assignment]
+    adjusted_date = getattr(calendar_, adj_op)(date)
     if adjusted_date.month != date.month and "M" in modifier:
-        adjusted_date = getattr(calendar, mod_op)(date)
+        adjusted_date = getattr(calendar_, mod_op)(date)
     return adjusted_date.to_pydatetime()
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 def add_tenor(
     start: datetime,
     tenor: str,
     modifier: Optional[str],
-    calendar: Optional[Union[CustomBusinessDay, str]],
+    calendar: CalInput,
 ) -> datetime:
     """
     Add a tenor to a given date under specific modification rules and holiday calendar.
 
     Note this function does **not** implement the `modified following month end` rule,
     where tenors starting on month end are adjusted to end on month end. For example
     a 3-month tenor starting 28th Feb 2022 would be adjusted to end on 31st May 2022.
@@ -301,19 +334,19 @@
 
     Examples
     --------
     .. ipython:: python
        :suppress:
 
        from rateslib.calendars import add_tenor, get_calendar, create_calendar, dcf
-       from rateslib.curves import Curve, LineCurve, interpolate, index_left
+       from rateslib.curves import Curve, LineCurve, interpolate, index_left, IndexCurve
        from rateslib.dual import Dual, Dual2
        from rateslib.periods import FixedPeriod, FloatPeriod, Cashflow
        from rateslib.legs import FixedLeg, FloatLeg, CustomLeg, FloatLegExchange, FixedLegExchange, FloatLegExchangeMtm, FixedLegExchangeMtm
-       from rateslib.instruments import FixedRateBond, FloatRateBond, Value, IRS, SBS, FRA, forward_fx, Spread, Fly
+       from rateslib.instruments import FixedRateBond, FloatRateBond, Value, IRS, SBS, FRA, forward_fx, Spread, Fly, BondFuture
        from rateslib.solver import Solver
        from rateslib.splines import bspldnev_single, PPSpline
        from datetime import datetime as dt
        from pandas import date_range, Series, DataFrame
 
     .. ipython:: python
 
@@ -321,31 +354,31 @@
        add_tenor(dt(2022, 12, 28), "4b", "F", get_calendar("ldn"))
        add_tenor(dt(2022, 12, 28), "4d", "F", get_calendar("ldn"))
     """
     tenor = tenor.upper()
     if "D" in tenor:
         return _add_days(start, int(tenor[:-1]), modifier, calendar)
     elif "B" in tenor:
-        calendar = get_calendar(calendar)
-        return (start + int(float(tenor[:-1])) * calendar).to_pydatetime()
+        calendar_: CustomBusinessDay = get_calendar(calendar)  # type: ignore[assignment]
+        return (start + int(float(tenor[:-1])) * calendar_).to_pydatetime()  # type: ignore[attr-defined]
     elif "Y" in tenor:
         return _add_months(start, int(float(tenor[:-1]) * 12), modifier, calendar)
     elif "M" in tenor:
         return _add_months(start, int(tenor[:-1]), modifier, calendar)
     else:
         raise ValueError(
             "`tenor` must identify frequency in {'B', 'D', 'M', 'Y'} e.g. '1Y'"
         )
 
 
 def _add_months(
     start: datetime,
     months: int,
     modifier: Optional[str],
-    cal: Optional[Union[CustomBusinessDay, str]],
+    cal: CalInput,
 ) -> datetime:
     """add a given number of months to an input date"""
     year_roll = floor((start.month + months - 1) / 12)
     month = (start.month + months) % 12
     month = 12 if month == 0 else month
     try:
         end = datetime(start.year + year_roll, month, start.day)
@@ -354,24 +387,25 @@
     return _adjust_date(end, modifier, cal)
 
 
 def _add_days(
     start: datetime,
     days: int,
     modifier: Optional[str],
-    cal: Optional[CustomBusinessDay],
+    cal: CalInput,
 ) -> datetime:
     end = start + timedelta(days=days)
     return _adjust_date(end, modifier, cal)
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _is_imm(date: datetime, hmuz=False) -> bool:
     """
     Test whether a given date is an IMM date, defined as third wednesday in month.
 
     Parameters
     ----------
     date : datetime,
@@ -436,14 +470,15 @@
 
     Returns
     -------
     int : Day
     """
     return datetime(year, month, calendar_mod.monthrange(year, month)[1])
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 def _is_som(date: datetime) -> bool:
     """
@@ -462,17 +497,19 @@
 
 
 def dcf(
     start: datetime,
     end: datetime,
     convention: str,
     termination: Optional[datetime] = None,  # required for 30E360ISDA and ActActICMA
-    frequency_months: Optional[int] = None,  # required for ActActICMA = ActActISMA = ActActBond
+    frequency_months: Optional[
+        int
+    ] = None,  # required for ActActICMA = ActActISMA = ActActBond
     stub: Optional[bool] = None,  # required for ActActICMA = ActActISMA = ActActBond
-):
+) -> float:
     """
     Calculate the day count fraction of a period.
 
     Parameters
     ----------
     start : datetime
         The adjusted start date of the calculation period.
@@ -572,32 +609,36 @@
         def _is_end_feb(date):
             if date.month == 2:
                 _, end_feb = calendar_mod.monthrange(date.year, 2)
                 return date.day == end_feb
             return False
 
         ds = 30 if (start.day == 31 or _is_end_feb(start)) else start.day
-        de = 30 if (end.day == 31 or (_is_end_feb(end) and end != termination)) else end.day
+        de = (
+            30
+            if (end.day == 31 or (_is_end_feb(end) and end != termination))
+            else end.day
+        )
         y, m = end.year - start.year, (end.month - start.month) / 12
         return y + m + (de - ds) / 360
     elif convention in ["ACTACT", "ACTACTISDA"]:
         if start == end:
             return 0.0
 
         start_date = datetime.combine(start, datetime.min.time())
         end_date = datetime.combine(end, datetime.min.time())
 
         year_1_diff = 366 if calendar_mod.isleap(start_date.year) else 365
         year_2_diff = 366 if calendar_mod.isleap(end_date.year) else 365
 
-        total_sum = end.year - start.year - 1
+        total_sum: float = end.year - start.year - 1
         total_sum += (datetime(start.year + 1, 1, 1) - start_date).days / year_1_diff
         total_sum += (end_date - datetime(end.year, 1, 1)).days / year_2_diff
         return total_sum
-    elif convention in ['ACTACTICMA', 'ACTACTISMA', 'ACTACTBOND']:
+    elif convention in ["ACTACTICMA", "ACTACTISMA", "ACTACTBOND"]:
         if frequency_months is None:
             raise ValueError(
                 "`frequency_months` must be supplied with specified `convention`."
             )
         if termination is None:
             raise ValueError(
                 "`termination` must be supplied with specified `convention`."
@@ -605,34 +646,39 @@
         if stub is None:
             raise ValueError("`stub` must be supplied with specified `convention`.")
         if not stub:
             return frequency_months / 12
         else:
             if end == termination:  # stub is a BACK stub:
                 fwd_end = _add_months(start, frequency_months, None, None)
-                fraction = 0
+                fraction = 0.0
                 if end > fwd_end:  # stub is LONG
                     fraction += 1
                     fraction += (end - fwd_end) / (
-                                _add_months(start, 2*frequency_months,
-                                                         None, None) - fwd_end)
+                        _add_months(start, 2 * frequency_months, None, None) - fwd_end
+                    )
                 else:
-                    fraction += (end - start) / (fwd_end-start)
+                    fraction += (end - start) / (fwd_end - start)
                 return fraction * frequency_months / 12
             else:  # stub is a FRONT stub
                 prev_start = _add_months(end, -frequency_months, None, None)
                 fraction = 0
                 if start < prev_start:  # stub is LONG
                     fraction += 1
-                    fraction += (prev_start - start) / (prev_start - _add_months(end, -2*frequency_months, None, None))
+                    fraction += (prev_start - start) / (
+                        prev_start - _add_months(end, -2 * frequency_months, None, None)
+                    )
                 else:
                     fraction += (end - start) / (end - prev_start)
                 return fraction * frequency_months / 12
     else:
-        raise ValueError("`convention` must be in {'Act365f', '1', 'Act360', "
-                         "'30360' '360360', 'BondBasis', '30E360', 'EuroBondBasis', "
-                         "'30E360ISDA', 'ActAct', 'ActActISDA', 'ActActICMA', "
-                         "'ActActISMA', 'ActActBond'}")
+        raise ValueError(
+            "`convention` must be in {'Act365f', '1', 'Act360', "
+            "'30360' '360360', 'BondBasis', '30E360', 'EuroBondBasis', "
+            "'30E360ISDA', 'ActAct', 'ActActISDA', 'ActActICMA', "
+            "'ActActISMA', 'ActActBond'}"
+        )
+
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
```

### Comparing `rateslib-0.1.0/rateslib/curves.py` & `rateslib-0.2.0/rateslib/curves.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 from uuid import uuid4
 import numpy as np
 import json
 from math import floor
 from rateslib import defaults
 from rateslib.dual import Dual, Dual2, dual_log, dual_exp
 from rateslib.splines import PPSpline
-from rateslib.defaults import plot
+from rateslib.default import plot
 from rateslib.calendars import create_calendar, get_calendar, add_tenor, dcf
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 class Serialize:
     """
     Methods mixin for serializing and solving :class:`Curve` or :class:`LineCurve` s.
     """
+
     def to_json(self):
         """
         Convert the parameters of the curve to JSON format.
 
         Returns
         -------
         str
@@ -42,39 +44,49 @@
         if self.t is None:
             t = None
         else:
             t = [t.strftime("%Y-%m-%d") for t in self.t]
 
         container = {
             "nodes": {dt.strftime("%Y-%m-%d"): v.real for dt, v in self.nodes.items()},
-            "interpolation": self.interpolation if isinstance(self.interpolation, str) else None,
+            "interpolation": self.interpolation
+            if isinstance(self.interpolation, str)
+            else None,
             "t": t,
             "c": self.spline.c if self.c_init else None,
             "id": self.id,
             "convention": self.convention,
             "endpoints": self.spline_endpoints,
             "modifier": self.modifier,
             "calendar_type": self.calendar_type,
             "ad": self.ad,
         }
+        if type(self) is IndexCurve:
+            container.update(
+                {"index_base": self.index_base, "index_lag": self.index_lag}
+            )
 
         if self.calendar_type == "null":
             container.update({"calendar": None})
         elif "named: " in self.calendar_type:
             container.update({"calendar": self.calendar_type[7:]})
         else:  # calendar type is custom
-            container.update({
-                "calendar": {
-                    "weekmask": self.calendar.weekmask,
-                    "holidays": [
-                        d.item().strftime("%Y-%m-%d")  # numpy/pandas timestamp to py
-                        for d in self.calendar.holidays
-                    ]
+            container.update(
+                {
+                    "calendar": {
+                        "weekmask": self.calendar.weekmask,
+                        "holidays": [
+                            d.item().strftime(
+                                "%Y-%m-%d"
+                            )  # numpy/pandas timestamp to py
+                            for d in self.calendar.holidays
+                        ],
+                    }
                 }
-            })
+            )
 
         return json.dumps(container, default=str)
 
     @classmethod
     def from_json(cls, curve, **kwargs):
         """
         Reconstitute a curve from JSON.
@@ -98,16 +110,15 @@
             # must load and construct a custom holiday calendar from serial dates
             parse = lambda d: Holiday("", year=d.year, month=d.month, day=d.day)
             dates = [
                 parse(datetime.strptime(d, "%Y-%m-%d"))
                 for d in serial["calendar"]["holidays"]
             ]
             serial["calendar"] = create_calendar(
-                rules=dates,
-                weekmask=serial["calendar"]["weekmask"]
+                rules=dates, weekmask=serial["calendar"]["weekmask"]
             )
 
         if serial["t"] is not None:
             serial["t"] = [datetime.strptime(t, "%Y-%m-%d") for t in serial["t"]]
         return cls(**{**serial, **kwargs})
 
     def copy(self):
@@ -145,24 +156,27 @@
             return None
         elif order == 1:
             self.ad, DualType = 1, Dual
         elif order == 2:
             self.ad, DualType = 2, Dual2
         else:
             raise ValueError("`order` can only be in {0, 1, 2} for auto diff calcs.")
-        self.nodes = {k: DualType(float(v), f"{self.id}{i}")
-                      for i, (k, v) in enumerate(self.nodes.items())}
+        self.nodes = {
+            k: DualType(float(v), f"{self.id}{i}")
+            for i, (k, v) in enumerate(self.nodes.items())
+        }
         self.csolve()
         return None
 
 
 class PlotCurve:
     """
     Methods mixin for plotting :class:`Curve` or :class:`LineCurve` s.
     """
+
     def plot(
         self,
         tenor: str,
         right: Optional[Union[datetime, str]] = None,
         left: Optional[Union[datetime, str]] = None,
         comparators: list[Curve] = [],
         difference: bool = False,
@@ -193,32 +207,32 @@
             length as number of plots.
 
         Returns
         -------
         (fig, ax, line) : Matplotlib.Figure, Matplotplib.Axes, Matplotlib.Lines2D
         """
         if left is None:
-            left_ : datetime = self.node_dates[0]
+            left_: datetime = self.node_dates[0]
         elif isinstance(left, str):
             left_ = add_tenor(self.node_dates[0], left, None, None)
         elif isinstance(left, datetime):
             left_ = left
         else:
             raise ValueError("`left` must be supplied as datetime or tenor string.")
 
         if right is None:
-            right_ : datetime = add_tenor(self.node_dates[-1], "-" + tenor, None, None)
+            right_: datetime = add_tenor(self.node_dates[-1], "-" + tenor, None, None)
         elif isinstance(right, str):
             right_ = add_tenor(self.node_dates[0], right, None, None)
         elif isinstance(right, datetime):
             right_ = right
         else:
             raise ValueError("`right` must be supplied as datetime or tenor string.")
 
-        points : int = (right_ - left_).days
+        points: int = (right_ - left_).days
         x = [left_ + timedelta(days=i) for i in range(points)]
         rates = [self.rate(_, tenor) for _ in x]
         if not difference:
             y = [rates]
             if comparators is not None:
                 for comparator in comparators:
                     y.append([comparator.rate(_, tenor) for _ in x])
@@ -237,14 +251,15 @@
         left: datetime = None,
         right: datetime = None,
         points: int = None,
     ):  # pragma: no cover
         """
         Debugging method?
         """
+
         def forward_fx(date, curve_domestic, curve_foreign, fx_rate, fx_settlement):
             _ = self[date] / curve_foreign[date]
             if fx_settlement is not None:
                 _ *= curve_foreign[fx_settlement] / curve_domestic[fx_settlement]
             _ *= fx_rate
             return _
 
@@ -287,20 +302,24 @@
     convention : str, optional, set by Default
         The convention of the curve for determining rates.
     modifier : str, optional
         The modification rule, in {"F", "MF", "P", "MP"}, for determining rates.
     calendar : calendar or str, optional
         The holiday calendar object to use. If str, looks up named calendar from
         static data. Used for determining rates.
+    index_base : float, optional
+        Set the initial, known value of the index. For typical use with RFR indexes and
+        inflation indexes, and if the :meth:`Curve.index_value` method is to be used.
     ad : int in {0, 1, 2}, optional
         Sets the automatic differentiation order. Defines whether to convert node
         values to float, :class:`~rateslib.dual.Dual` or
         :class:`~rateslib.dual.Dual2`. It is advised against
         using this setting directly. It is mainly used internally.
     """
+
     _op_exp = staticmethod(dual_exp)  # Curve is DF based: log-cubic spline is exp'ed
     _op_log = staticmethod(dual_log)  # Curve is DF based: spline is applied over log
     _ini_solve = 1  # Curve is assumed to have initial DF node at 1.0 as constraint
 
     def __init__(
         self,
         nodes: dict,
@@ -309,21 +328,23 @@
         c: Optional[list[float]] = None,
         endpoints: Optional[str] = None,
         id: Optional[str] = None,
         convention: Optional[str] = None,
         modifier: Optional[Union[str, bool]] = False,
         calendar: Optional[Union[CustomBusinessDay, str]] = None,
         ad: int = 0,
-        **kwargs
+        **kwargs,
     ):
         self.id = id or uuid4().hex[:5] + "_"  # 1 in a million clash
         self.nodes = nodes  # nodes.copy()
         self.node_dates = list(self.nodes.keys())
         self.n = len(self.node_dates)
-        self.interpolation = interpolation or defaults.interpolation[type(self).__name__]
+        self.interpolation = (
+            interpolation or defaults.interpolation[type(self).__name__]
+        )
 
         # Parameters for the rate derivation
         self.convention = convention or defaults.convention
         self.modifier = defaults.modifier if modifier is False else modifier
         self.calendar, self.calendar_type = get_calendar(calendar, kind=True)
         if self.calendar_type == "named":
             self.calendar_type = f"named: {calendar.lower()}"
@@ -353,31 +374,31 @@
         if self.spline is None or date <= self.t[0]:
             if isinstance(self.interpolation, Callable):
                 return self.interpolation(date, self.nodes.copy())
             return self._local_interp_(date)
         else:
             return self._op_exp(self.spline.ppev_single(date))
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def _local_interp_(self, date: datetime):
         if date < self.node_dates[0]:
             return 0  # then date is in the past and DF is zero
         l_index = index_left(self.node_dates, self.n, date)
-        node_left, node_right = self.node_dates[l_index], self.node_dates[l_index+1]
+        node_left, node_right = self.node_dates[l_index], self.node_dates[l_index + 1]
         return interpolate(
             date,
             node_left,
             self.nodes[node_left],
             node_right,
             self.nodes[node_right],
             self.interpolation,
-            self.node_dates[0]
+            self.node_dates[0],
         )
 
     # def plot(self, *args, **kwargs):
     #     return super().plot(*args, **kwargs)
 
     def rate(
         self,
@@ -561,51 +582,50 @@
                ],
            )
            spread_curve = curve.shift(25)
            fig, ax, line = curve.plot("1d", comparators=[spread_curve], labels=["orig", "shift"])
            plt.show()
 
         """
-
-        # TODO test whether need to lower AD order before adding spread
-
         v1v2 = [1.0] * (self.n - 1)
         n = [0] * (self.n - 1)
-        d = 1/365 if self.convention.upper() != "ACT360" else 1/360
+        d = 1 / 365 if self.convention.upper() != "ACT360" else 1 / 360
         v_new = [1.0] * (self.n)
         for i, (k, v) in enumerate(self.nodes.items()):
             if i == 0:
                 continue
-            n[i-1] = (k - self.node_dates[i-1]).days
-            v1v2[i-1] = (self.nodes[self.node_dates[i-1]] / v) ** (1 / n[i-1])
-            v_new[i] = v_new[i-1] / (v1v2[i-1] + d * spread / 10000) ** n[i-1]
+            n[i - 1] = (k - self.node_dates[i - 1]).days
+            v1v2[i - 1] = (self.nodes[self.node_dates[i - 1]] / v) ** (1 / n[i - 1])
+            v_new[i] = v_new[i - 1] / (v1v2[i - 1] + d * spread / 10000) ** n[i - 1]
 
         nodes = self.nodes.copy()
         for i, (k, v) in enumerate(nodes.items()):
             nodes[k] = v_new[i]
 
-        _ = Curve(
+        kwargs = {}
+        if type(self) is IndexCurve:
+            kwargs = {"index_base": self.index_base, "index_lag": self.index_lag}
+        _ = type(self)(
             nodes=nodes,
             interpolation=self.interpolation,
             t=self.t,
             c=None,
             endpoints=self.spline_endpoints,
             id=None,
             convention=self.convention,
             modifier=self.modifier,
             calendar=self.calendar,
-            ad=self.ad
+            ad=self.ad,
+            **kwargs,
         )
         return _
 
     def _translate_nodes(self, start: datetime):
         scalar = 1 / self[start]
-        new_nodes = {
-            k: scalar * v for k, v in self.nodes.items()
-        }
+        new_nodes = {k: scalar * v for k, v in self.nodes.items()}
 
         # re-organise the nodes on the new curve
         if start == self.node_dates[1]:
             del new_nodes[self.node_dates[1]]
         del new_nodes[self.node_dates[0]]
         new_nodes = {start: 1.0, **new_nodes}
         return new_nodes
@@ -757,25 +777,32 @@
                 for i in range(4):
                     new_t[i] = start  # adjust left side of t to start
         elif self.t and self.t[4] <= start:
             raise ValueError(
                 "Cannot translate spline knots for given `start`, review the docs."
             )
 
+        kwargs = {}
+        if type(self) is IndexCurve:
+            kwargs = {
+                "index_base": self.index_value(start),
+                "index_lag": self.index_lag,
+            }
         new_curve = type(self)(
             nodes=new_nodes,
             interpolation=self.interpolation,
             t=new_t,
             c=None,
             endpoints=self.spline_endpoints,
             modifier=self.modifier,
             calendar=self.calendar,
             convention=self.convention,
             id=None,
-            ad=self.ad
+            ad=self.ad,
+            **kwargs,
         )
         return new_curve
 
     def _roll_nodes(self, tenor: datetime, days: int):
         """
         Roll nodes by adding days to each one and scaling DF values.
 
@@ -793,23 +820,20 @@
         on_rate = self.rate(self.node_dates[0], "1d", None)
         d = 1 / 365 if self.convention.upper() != "ACT360" else 1 / 360
         scalar = 1 / ((1 + on_rate * d / 100) ** days)
         new_nodes = {
             k + timedelta(days=days): v * scalar for k, v in self.nodes.items()
         }
         if tenor > self.node_dates[0]:
-            new_nodes = {
-                self.node_dates[0]: 1.0,
-                **new_nodes
-            }
+            new_nodes = {self.node_dates[0]: 1.0, **new_nodes}
         return new_nodes
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def roll(self, tenor: Union[datetime, str]):
         """
         Create a new curve with its shape translated in time
 
         This curve adjustment is a simulation of a future state of the market where
         forward rates are assumed to have moved so that the present day's curve shape
@@ -903,15 +927,16 @@
             t=new_t,
             c=None,
             endpoints=self.spline_endpoints,
             modifier=self.modifier,
             calendar=self.calendar,
             convention=self.convention,
             id=None,
-            ad=self.ad
+            # TODO: design how to adjust the index_base on a rolled curve.
+            ad=self.ad,
         )
         if tenor > self.node_dates[0]:
             return new_curve
         else:  # tenor < self.node_dates[0]
             return new_curve.translate(self.node_dates[0])
 
 
@@ -934,26 +959,44 @@
     t : list[datetime], optional
         The knot locations for the B-spline cubic interpolation section of the
         curve. If *None* all interpolation will be done by the method specified in
         ``interpolation``.
     c : list[float], optional
         The B-spline coefficients used to define the cubic spline. If not given
         will use :meth:`csolve`.
+    endpoints : str or list, optional
+        The left and right endpoint constraint for the spline solution. Valid values are
+        in {"natural", "not_a_knot"}. If a list, supply the left endpoint then the
+        right endpoint.
     id : str, optional, set by Default
         The unique identifier to distinguish between curves in a multicurve framework.
     convention : str, optional,
-        This parameter is not used. It is included for signature consistency with
-        :class:`Curve`.
+        **This parameter is not used by :class:`LineCurve`**. It is included for
+        signature consistency with :class:`Curve`.
+    modifier : str, optional
+        **This parameter is not used by :class:`LineCurve`**. It is included for
+        signature consistency with :class:`Curve`.
+    calendar : calendar or str, optional
+        **This parameter is not used by :class:`LineCurve`**. It is included for
+        signature consistency with :class:`Curve`.
+    index_base : float, optional
+        **This parameter is not used by :class:`LineCurve`**. It is included for
+        signature consistency with :class:`Curve`.
     ad : int in {0, 1, 2}, optional
         Sets the automatic differentiation order. Defines whether to convert node
         values to float, :class:`Dual` or :class:`Dual2`. It is advised against
         using this setting directly. It is mainly used internally.
     """
-    _op_exp = staticmethod(lambda x: x)  # LineCurve spline is not log based so no exponent needed
-    _op_log = staticmethod(lambda x: x)  # LineCurve spline is not log based so no log needed
+
+    _op_exp = staticmethod(
+        lambda x: x
+    )  # LineCurve spline is not log based so no exponent needed
+    _op_log = staticmethod(
+        lambda x: x
+    )  # LineCurve spline is not log based so no log needed
     _ini_solve = 0  # No constraint placed on initial node in Solver
 
     def __init__(
         self,
         *args,
         **kwargs,
     ):
@@ -1047,42 +1090,41 @@
                ],
            )
            spread_curve = line_curve.shift(25)
            fig, ax, line = line_curve.plot("1d", comparators=[spread_curve])
            plt.show()
 
         """
-        # TODO test whether need to lower AD order before adding spread
         _ = LineCurve(
-            nodes={k: v + spread/100 for k, v in self.nodes.items()},
+            nodes={k: v + spread / 100 for k, v in self.nodes.items()},
             interpolation=self.interpolation,
             t=self.t,
             c=None,
             endpoints=self.spline_endpoints,
             id=None,
             convention=self.convention,
             modifier=self.modifier,
             calendar=self.calendar,
-            ad=self.ad
+            ad=self.ad,
         )
         return _
 
     def _translate_nodes(self, start: datetime):
         new_nodes = self.nodes.copy()
         # re-organise the nodes on the new curve
         del new_nodes[self.node_dates[0]]
         if start == self.node_dates[1]:
             pass
         else:
             new_nodes = {start: self[start], **new_nodes}
         return new_nodes
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def translate(self, start: datetime, t: bool = False):
         """
         Create a new curve with an initial node date moved forward keeping all else
         constant.
 
         This curve adjustment preserves forward curve expectations as time evolves.
@@ -1204,22 +1246,17 @@
            fig, ax, line = curve.plot("1d", left=dt(2022, 1, 15), comparators=[translated, translated2], labels=["orig", "translated", "translated2"])
            plt.show()
 
         """
         return super().translate(start, t)
 
     def _roll_nodes(self, tenor: datetime, days: int):
-        new_nodes = {
-            k + timedelta(days=days): v for k, v in self.nodes.items()
-        }
+        new_nodes = {k + timedelta(days=days): v for k, v in self.nodes.items()}
         if tenor > self.node_dates[0]:
-            new_nodes = {
-                self.node_dates[0]: self[self.node_dates[0]],
-                **new_nodes
-            }
+            new_nodes = {self.node_dates[0]: self[self.node_dates[0]], **new_nodes}
         return new_nodes
 
     def roll(self, tenor: Union[datetime, str]):
         """
         Create a new curve with its shape translated in time
 
         This curve adjustment is a simulation of a future state of the market where
@@ -1299,14 +1336,91 @@
            plt.show()
            plt.close()
 
         """
         return super().roll(tenor)
 
 
+class IndexCurve(Curve):
+    """
+    A :class:`Curve` designed for use with inflation secuities and derivatives.
+
+    Parameters
+    ----------
+    args : tuple
+        Position arguments required by :class:`Curve`.
+    inf_lag : int
+        Number of months of inflation lag this curve adopts. For example if the initial
+        curve node date is 1st Sep 2021 based on the inflation index published
+        17th June 2023 then the lag is 3 months.
+    kwargs : dict
+        Keyword arguments required by :class:`Curve`.
+    """
+
+    def __init__(
+        self,
+        *args,
+        index_base: Optional[float] = None,
+        index_lag: Optional[int] = None,
+        **kwargs,
+    ):
+        self.index_lag = defaults.index_lag if index_lag is None else index_lag
+        self.index_base = index_base
+        if self.index_base is None:
+            raise ValueError("`index_base` must be given for IndexCurve.")
+        super().__init__(*args, **kwargs)
+
+    def index_value(self, date: datetime, interpolation: str = "daily"):
+        """
+        Calculate the accrued value of the index from the ``index_base``.
+
+        Parameters
+        ----------
+        date : datetime
+            The date for which the index value will be returned.
+        interpolation : str in {"monthly", "daily"}
+            The method for returning the index value. Monthly returns the index value
+            for the start of the month and daily returns a value based on the
+            interpolation between nodes (which is recommended *"linear_index*) for
+            :class:`InflationCurve`.
+
+        Returns
+        -------
+        None, float, Dual, Dual2
+
+        Examples
+        --------
+        The SWESTR rate, for reference value date 6th Sep 2021, was published as
+        2.375% and the RFR index for that date was 100.73350964. Below we calculate
+        the value that was published for the RFR index on 7th Sep 2021 by the Riksbank.
+
+        .. ipython:: python
+
+           index_curve = IndexCurve(
+               nodes={
+                   dt(2021, 9, 6): 1.0,
+                   dt(2021, 9, 7): 1 / (1 + 2.375/36000)
+               },
+               index_base=100.73350964,
+               convention="Act360",
+           )
+           index_curve.rate(dt(2021, 9, 6), "1d")
+           index_curve.index_value(dt(2021, 9, 7))
+        """
+        if interpolation.lower() == "daily":
+            date_ = date
+        elif interpolation.lower() == "monthly":
+            date_ = datetime(date.year, date.month, 1)
+        else:
+            raise ValueError(
+                "`interpolation` for `index_value` must be in {'daily', 'monthly'}."
+            )
+        return self.index_base * 1 / self[date_]
+
+
 def interpolate(x, x_1, y_1, x_2, y_2, interpolation, start=None):
     """
     Perform local interpolation between two data points.
 
     Parameters
     ----------
     x : Any with topology
@@ -1340,14 +1454,17 @@
     .. ipython:: python
 
        interpolate(50, 0, 10, 100, 50, "linear")
        interpolate(dt(2000, 1, 6), dt(2000, 1, 1), 10, dt(2000, 1, 11), 50, "linear")
     """
     if interpolation == "linear":
         op = lambda z: z
+    elif interpolation == "linear_index":
+        op = lambda z: 1 / z
+        y_1, y_2 = 1 / y_1, 1 / y_2
     elif interpolation == "log_linear":
         op, y_1, y_2 = dual_exp, dual_log(y_1), dual_log(y_2)
     elif interpolation == "linear_zero_rate":
         # convention not used here since we just determine linear rate interpolation
         y_2 = dual_log(y_2) / ((start - x_2) / timedelta(days=365))
         if start == x_1:
             y_1 = y_2
@@ -1434,23 +1551,23 @@
         raise ValueError(
             "`index_left` designed for intervals. Cannot index list of length 1."
         )
 
     if list_length == 2:
         return left_count
 
-    split = floor((list_length-1)/2)
+    split = floor((list_length - 1) / 2)
     if list_length == 3 and value == list_input[split]:
         return left_count
 
     if value <= list_input[split]:
-        return index_left(list_input[:split+1], split+1, value, left_count)
+        return index_left(list_input[: split + 1], split + 1, value, left_count)
     else:
         return index_left(
-            list_input[split:], list_length-split, value, left_count + split
+            list_input[split:], list_length - split, value, left_count + split
         )
 
 
 # # ALTERNATIVE index_left: exhaustive search which is inferior to binary search
 # def index_left_exhaustive(list_input, value, left_count=0):
 #     if left_count == 0:
 #         if value > list_input[-1]:
```

### Comparing `rateslib-0.1.0/rateslib/defaults.py` & `rateslib-0.2.0/rateslib/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class Defaults:
     """
     Test docs
     """
+
     convention = "ACT360"
     notional = 1.0e6
     stub = "SHORTFRONT"
     stub_length = "SHORT"
     modifier = "MF"
+    index_lag = 3
     payment_lag = 2
     payment_lag_exchange = 0
     payment_lag_specific = {
         "IRS": 2,
         "ZCS": 2,
         "FXSwap": 0,
         "SBS": 2,
@@ -34,14 +36,15 @@
         "Bill": 0,
         "FRA": 0,
     }
     calendar = BusinessDay()
     interpolation = {
         "Curve": "log_linear",
         "LineCurve": "linear",
+        "IndexCurve": "linear_index",
     }
     endpoints = "natural"
     frequency_months = {
         "M": 1,
         "B": 2,
         "Q": 3,
         "T": 4,
@@ -77,40 +80,44 @@
         "currency": "Ccy",
         "rate": "Rate",
         "spread": "Spread",
         "npv": "NPV",
         "cashflow": "Cashflow",
         "fx": "FX Rate",
         "npv_fx": "NPV Ccy",
+        "real_cashflow": "Real Cashflow",
+        "index_value": "Index Val",
+        "index_ratio": "Index Ratio",
     }
     curve_not_in_solver = "ignore"
     no_fx_fixings_for_xcs = "warn"
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def reset_defaults(self):
         base = Defaults()
         for attr in [_ for _ in dir(self) if "__" != _[:2]]:
             setattr(self, attr, getattr(base, attr))
 
 
 def plot(x, y: list, labels=[]):
-    import matplotlib.pyplot as plt
-    import matplotlib.dates as mdates
+    import matplotlib.pyplot as plt  # type: ignore[import]
+    import matplotlib.dates as mdates  # type: ignore[import]
+
     fig, ax = plt.subplots(1, 1)
     lines = []
     for _y in y:
-        line, = ax.plot(x, _y)
+        (line,) = ax.plot(x, _y)
         lines.append(line)
     if labels and len(labels) == len(lines):
         ax.legend(lines, labels)
     years = mdates.YearLocator()  # every year
     months = mdates.MonthLocator()  # every month
-    yearsFmt = mdates.DateFormatter('%Y')
+    yearsFmt = mdates.DateFormatter("%Y")
     ax.xaxis.set_major_locator(years)
     ax.xaxis.set_major_formatter(yearsFmt)
     ax.xaxis.set_minor_locator(months)
     ax.grid(True)
     fig.autofmt_xdate()
-    return fig, ax, lines
+    return fig, ax, lines
```

### Comparing `rateslib-0.1.0/rateslib/dual.py` & `rateslib-0.2.0/rateslib/dual.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,95 @@
 from math import isclose
+from abc import abstractmethod, ABCMeta
+from typing import Union, Optional
 import math
 import numpy as np
 
 PRECISION = 1e-14
 FLOATS = (float, np.float16, np.float32, np.float64, np.float128)
 INTS = (int, np.int8, np.int16, np.int32, np.int32, np.int64)
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-class DualBase:
+class DualBase(metaclass=ABCMeta):
     """
     Base class for dual number implementation.
     """
 
+    dual: np.ndarray = np.zeros(0)
+    dual2: np.ndarray = np.zeros(0)
+
+    def __init__(self, real: float, vars: tuple[str, ...] = tuple()):
+        self.real: float = real
+        self.vars: tuple[str, ...] = vars
+
     def __float__(self):
         return float(self.real)
 
     def __abs__(self):
         return abs(self.real)
 
+    def __lt__(self, argument):
+        """Compare an argument by evaluating the size of the real."""
+        if not isinstance(argument, type(self)):
+            if not isinstance(argument, (*FLOATS, *INTS)):
+                raise TypeError(f"Cannot compare {type(self)} with incompatible type.")
+            argument = type(self)(float(argument))
+        if float(self) < float(argument):
+            return True
+        return False
+
+    def __gt__(self, argument):
+        """Compare an argument by evaluating the size of the real."""
+        if not isinstance(argument, type(self)):
+            if not isinstance(argument, (*FLOATS, *INTS)):
+                raise TypeError(f"Cannot compare {type(self)} with incompatible type.")
+            argument = type(self)(float(argument))
+        if float(self) > float(argument):
+            return True
+        return False
+
     def __eq__(self, argument):
         """Compare an argument with a Dual number for equality."""
         if not isinstance(argument, type(self)):
             if not isinstance(argument, (*FLOATS, *INTS)):
                 raise TypeError(f"Cannot compare {type(self)} with incompatible type.")
-            argument = type(self)(argument)
+            argument = type(self)(float(argument))
         if self.vars == argument.vars:
             return self.__eq_coeffs__(argument)
         else:
             self_, argument = self.__upcast_combined__(argument)
             return self_.__eq__(argument)
 
     def __eq_coeffs__(self, argument):
         """Compare the coefficients of two Dual numbers for equality."""
         if not isclose(self.real, argument.real, abs_tol=PRECISION):
             return False
         elif not np.all(np.isclose(self.dual, argument.dual, atol=PRECISION)):
             return False
-        elif getattr(self, "dual2", None) is not None:
+        if type(self) is Dual2 and type(argument) is Dual2:
             if not np.all(np.isclose(self.dual2, argument.dual2, atol=PRECISION)):
                 return False
+        elif type(self) is Dual2 or type(argument) is Dual2:
+            return False  # cannot compare Dual with Dual2
         return True
 
     def __upcast_combined__(self, arg):
         """Combines, and inserts, the vars of two Dual numbers to match each other."""
         new_vars = sorted(list(set(self.vars).union(set(arg.vars))))
         new_self = self if new_vars == self.vars else self.__upcast_vars__(new_vars)
         new_arg = arg if new_vars == arg.vars else arg.__upcast_vars__(new_vars)
         return new_self, new_arg
 
-    def __repr__(self):
-        dual2 = getattr(self, "dual2", None)
-        if dual2 is None:
-            name, final = "Dual", ""
-        else:
-            name, final = "Dual2", f", [[...]]"
-        return f"<{name}: {self.real:,.6f}, {self.vars}, {self.dual}{final}>"
-
-    def __str__(self):
-        output = f" val = {self.real:.8f}\n"
-        for i, tag in enumerate(self.vars):
-            output += f"  d{tag} = {self.dual[i]:.6f}\n"
-        if getattr(self, "dual2", None) is not None:
-            for i, ltag in enumerate(self.vars):
-                for j, rtag in enumerate(self.vars):
-                    if j >= i:
-                        output += f"d{ltag}d{rtag} = {2 * self.dual2[i,j]:.6f}\n"
-        return output
+    @abstractmethod
+    def __upcast_vars__(self, new_vars: list[str]):
+        pass
 
     def gradient(self, vars=None, order=1, keep_manifold=False):
         """
         Return derivatives of a dual number.
 
         Parameters
         ----------
@@ -115,14 +131,15 @@
             return ret
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 class Dual2(DualBase):
     """
     Dual number data type to perform second derivative automatic differentiation.
 
     Parameters
     ----------
     real : float, int
@@ -155,14 +172,28 @@
         else:
             self.vars = tuple(vars)
         n = len(self.vars)
         self.real = real
         self.dual = np.asarray(dual.copy()) if dual is not None else np.ones(n)
         self.dual2 = np.asarray(dual2.copy()) if dual2 is not None else np.zeros((n, n))
 
+    def __repr__(self):
+        name, final = "Dual2", f", [[...]]"
+        return f"<{name}: {self.real:,.6f}, {self.vars}, {self.dual}{final}>"
+
+    def __str__(self):
+        output = f" val = {self.real:.8f}\n"
+        for i, tag in enumerate(self.vars):
+            output += f"  d{tag} = {self.dual[i]:.6f}\n"
+        for i, ltag in enumerate(self.vars):
+            for j, rtag in enumerate(self.vars):
+                if j >= i:
+                    output += f"d{ltag}d{rtag} = {2 * self.dual2[i,j]:.6f}\n"
+        return output
+
     def __neg__(self):
         return Dual2(-self.real, self.vars, -self.dual, -self.dual2)
 
     def __add__(self, argument):
         if not isinstance(argument, Dual2):
             if isinstance(argument, np.ndarray):
                 return argument + self
@@ -204,27 +235,27 @@
             if isinstance(argument, np.ndarray):
                 return argument * self
             elif isinstance(argument, (*FLOATS, *INTS)):
                 return Dual2(
                     self.real * argument,
                     self.vars,
                     self.dual * argument,
-                    self.dual2 * argument
+                    self.dual2 * argument,
                 )
             raise TypeError("Dual2 operations defined between float, int or Dual2.")
 
         if self.vars == argument.vars:
             dual2 = self.dual2 * argument.real + argument.dual2 * self.real
-            _ = np.einsum('i,j', self.dual, argument.dual)
+            _ = np.einsum("i,j", self.dual, argument.dual)
             dual2 += (_ + _.T) / 2
             return Dual2(
                 self.real * argument.real,
                 self.vars,
                 self.dual * argument.real + argument.dual * self.real,
-                dual2
+                dual2,
             )
         else:
             self_, argument = self.__upcast_combined__(argument)
             return self_ * argument
 
     __rmul__ = __mul__
 
@@ -233,15 +264,15 @@
             if isinstance(argument, np.ndarray):
                 return argument.__rtruediv__(self)
             elif isinstance(argument, (*FLOATS, *INTS)):
                 return Dual2(
                     self.real / argument,
                     self.vars,
                     self.dual / argument,
-                    self.dual2 / argument
+                    self.dual2 / argument,
                 )
             raise TypeError("Dual2 operations defined between float, int or Dual2.")
 
         if self.vars == argument.vars:
             return self * argument**-1
         else:
             self_, argument = self.__upcast_combined__(argument)
@@ -255,123 +286,142 @@
         return numerator / self
 
     def __pow__(self, power):
         if isinstance(power, (*FLOATS, *INTS)):
             coeff = power * self.real ** (power - 1)
             coeff2 = power * (power - 1) * self.real ** (power - 2) * 0.5
             return Dual2(
-                self.real ** power,
+                self.real**power,
                 self.vars,
                 self.dual * coeff,
-                self.dual2 * coeff + np.einsum("i,j", self.dual, self.dual) * coeff2
+                self.dual2 * coeff + np.einsum("i,j", self.dual, self.dual) * coeff2,
             )
         elif isinstance(power, np.ndarray):
             return power.__rpow__(self)
         raise TypeError("Dual2 power defined only with float, int.")
 
     def __exp__(self):
         const = math.exp(self.real)
         return Dual2(
             const,
             self.vars,
             self.dual * const,
-            const * (self.dual2 + np.einsum("i,j", self.dual, self.dual) * 0.5 )
+            const * (self.dual2 + np.einsum("i,j", self.dual, self.dual) * 0.5),
         )
 
     def __log__(self):
         return Dual2(
             math.log(self.real),
             self.vars,
             self.dual / self.real,
-            self.dual2 / self.real - np.einsum("i,j", self.dual, self.dual) * 0.5 / self.real**2
+            self.dual2 / self.real
+            - np.einsum("i,j", self.dual, self.dual) * 0.5 / self.real**2,
         )
 
     def __upcast_vars__(self, new_vars):
         n = len(new_vars)
         dual, dual2 = np.zeros(n), np.zeros((n, n))
         ix_ = list(map(lambda x: new_vars.index(x), self.vars))
         dual[ix_], dual2[np.ix_(ix_, ix_)] = self.dual, self.dual2
         return Dual2(self.real, new_vars, dual, dual2)
 
     def __downcast_vars__(self):
         """removes variables where first and second order sensitivity is zero"""
         ix_ = np.where(np.isclose(self.dual, 0, atol=PRECISION) == False)[0]
-        ix2_ = np.where(np.isclose(self.dual2.sum(axis=0), 0, atol=PRECISION) == False)[0]
+        ix2_ = np.where(np.isclose(self.dual2.sum(axis=0), 0, atol=PRECISION) == False)[
+            0
+        ]
         ixu = np.union1d(ix_, ix2_)
         new_vars = [self.vars[i] for i in ixu]
-        return Dual2(
-            self.real, new_vars, self.dual[ixu], self.dual2[np.ix_(ixu, ixu)]
-        )
+        return Dual2(self.real, new_vars, self.dual[ixu], self.dual2[np.ix_(ixu, ixu)])
 
     def _set_order(self, order):
         if order == 1:
             return Dual(self.real, self.vars, self.dual)
         if order == 2:
             return Dual2(self.real, self.vars, self.dual, self.dual2)
         if order == 0:
             return float(self)
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 class Dual(DualBase):
     """
     Dual number data type to perform first derivative automatic differentiation.
 
     Parameters
     ----------
     real : float, int
         The real coefficient of the dual number
-    vars : list of str, optional
+    vars : tuple of str, optional
         The labels of the variables for which to record derivatives. If not given
         the dual number represents a constant, equivalent to an int or float.
     dual : 1d ndarray, optional
         First derivative information contained as coefficient of linear manifold.
         Defaults to an array of ones the length of ``vars`` if not given.
 
 
     Attributes
     ----------
     real : float, int
-    vars : str, list of str
+    vars : str, tuple of str
     dual : 1d ndarray
 
     See Also
     --------
     Dual2 : Dual number data type to perform second derivative automatic differentiation.
     """
 
-    def __init__(self, real, vars=(), dual=None):
-        self.real = real
+    def __init__(
+        self,
+        real: float,
+        vars: tuple[str, ...] = (),
+        dual: Optional[np.ndarray] = None,
+    ):
+        self.real: float = real
         if isinstance(vars, str):
-            self.vars = (vars,)
+            self.vars: tuple[str, ...] = (vars,)
         else:
             self.vars = tuple(vars)
         n = len(self.vars)
-        self.dual = np.asarray(dual.copy()) if dual is not None else np.ones(n)
+        self.dual: np.ndarray = (
+            np.asarray(dual.copy()) if dual is not None else np.ones(n)
+        )
+
+    @property
+    def dual2(self):
+        raise ValueError("`Dual` variable cannot possess `dual2` attribute")
+
+    def __repr__(self):
+        name, final = "Dual", ""
+        return f"<{name}: {self.real:,.6f}, {self.vars}, {self.dual}{final}>"
+
+    def __str__(self):
+        output = f" val = {self.real:.8f}\n"
+        for i, tag in enumerate(self.vars):
+            output += f"  d{tag} = {self.dual[i]:.6f}\n"
+        return output
 
     def __neg__(self):
         return Dual(-self.real, self.vars, -self.dual)
 
     def __add__(self, argument):
         if not isinstance(argument, Dual):
             if isinstance(argument, np.ndarray):
                 return argument + self
             elif isinstance(argument, (*FLOATS, *INTS)):
-                return Dual(self.real + argument, self.vars, self.dual)
+                return Dual(self.real + float(argument), self.vars, self.dual)
             raise TypeError("Dual operations defined between float, int or Dual.")
 
         if self.vars == argument.vars:
-            return Dual(
-                self.real + argument.real,
-                self.vars,
-                self.dual + argument.dual
-            )
+            return Dual(self.real + argument.real, self.vars, self.dual + argument.dual)
         else:
             self_, argument = self.__upcast_combined__(argument)
             return self_ + argument
 
     __radd__ = __add__
 
     def __sub__(self, argument):
@@ -381,54 +431,59 @@
         return -(self - argument)
 
     def __mul__(self, argument):
         if not isinstance(argument, Dual):
             if isinstance(argument, np.ndarray):
                 return argument * self
             elif isinstance(argument, (*FLOATS, *INTS)):
-                return Dual(self.real * argument, self.vars, self.dual * argument)
+                return Dual(
+                    self.real * float(argument), self.vars, self.dual * float(argument)
+                )
             raise TypeError("Dual operations defined between float, int or Dual.")
 
         if self.vars == argument.vars:
             return Dual(
                 self.real * argument.real,
                 self.vars,
-                self.dual * argument.real + argument.dual * self.real
+                self.dual * argument.real + argument.dual * self.real,
             )
         else:
             self_, argument = self.__upcast_combined__(argument)
             return self_ * argument
 
     __rmul__ = __mul__
 
     def __truediv__(self, argument):
         if not isinstance(argument, Dual):
             if isinstance(argument, np.ndarray):
                 return argument.__rtruediv__(self)
             if not isinstance(argument, (*FLOATS, *INTS)):
                 raise TypeError("Dual operations defined between float, int or Dual.")
-            return Dual(self.real / argument, self.vars, self.dual / argument)
+            return Dual(
+                self.real / float(argument), self.vars, self.dual / float(argument)
+            )
         if self.vars == argument.vars:
             return self * argument**-1
         else:
             self_, argument = self.__upcast_combined__(argument)
             return self_ * argument**-1
 
     def __rtruediv__(self, argument):
         if not isinstance(argument, (*FLOATS, *INTS)):
             raise TypeError("Dual operations defined between float, int or Dual.")
-        numerator = Dual(argument)
+        numerator = Dual(float(argument))
         return numerator / self
 
     def __pow__(self, power):
         if isinstance(power, (*FLOATS, *INTS)):
+            pow: float = float(power)
             return Dual(
-                self.real ** power,
+                self.real**pow,
                 self.vars,
-                self.dual * power * self.real ** (power - 1)
+                self.dual * pow * self.real ** (pow - 1),
             )
         elif isinstance(power, np.ndarray):
             return power.__rpow__(self)
         raise TypeError("Dual power defined only with float, int.")
 
     def __exp__(self):
         const = math.exp(self.real)
@@ -443,15 +498,15 @@
         ix_ = list(map(lambda x: new_vars.index(x), self.vars))
         dual[ix_] = self.dual
         return Dual(self.real, new_vars, dual)
 
     def __downcast_vars__(self):
         """removes variables where first order sensitivity is zero"""
         ix_ = np.where(np.isclose(self.dual, 0, atol=PRECISION) == False)[0]
-        new_vars = [self.vars[i] for i in ix_]
+        new_vars = tuple(self.vars[i] for i in ix_)
         return Dual(self.real, new_vars, self.dual[ix_])
 
     def _set_order(self, order):
         if order == 1:
             return Dual(self.real, self.vars, self.dual)
         if order == 2:
             return Dual2(self.real, self.vars, self.dual)
@@ -478,14 +533,15 @@
     -------
     float, Dual, Dual2
     """
     if isinstance(x, (Dual, Dual2)):
         return x.__exp__()
     return math.exp(x)
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 def dual_log(x, base=None):
     """
@@ -500,15 +556,15 @@
 
     Returns
     -------
     float, Dual, Dual2
     """
     if isinstance(x, (Dual, Dual2)):
         val = x.__log__()
-        return val if base is None else val * (1/math.log(base))
+        return val if base is None else val * (1 / math.log(base))
     return math.log(x) if base is None else math.log(x, base)
 
 
 def _pivot_matrix(A, method=1):
     """
     Returns the pivoting matrix for P, used in Doolittle's method.
 
@@ -535,14 +591,15 @@
     return P, PA
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _plu_decomp(A, method=1):
     """Performs an LU Decomposition of A (which must be square)
     into PA = LU. The function returns P, L and U. Uses Doolittle algorithm.
 
     `method` is passed to the pivoting technique.
     """
     if method == 3:
@@ -557,26 +614,26 @@
     # Perform the LU Decomposition
     try:
         for j in range(n):
             # All diagonal entries of L are set to unity
             L[j, j] = 1.0
 
             # LaTeX: u_{ij} = a_{ij} - \sum_{k=1}^{i-1} u_{kj} l_{ik}
-            for i in range(j+1):
+            for i in range(j + 1):
                 sx = np.matmul(L[i, :i], U[:i, j])
                 # s1 = sum(U[k][j] * L[i][k] for k in range(i))
                 U[i, j] = PA[i, j] - sx
 
             # LaTeX: l_{ij} = \frac{1}{u_{jj}} (a_{ij} - \sum_{k=1}^{j-1} u_{kj} l_{ik})
             for i in range(j, n):
                 sy = np.matmul(L[i, :j], U[:j, j])
                 # s2 = sum(U[k][j] * L[i][k] for k in range(j))
                 L[i, j] = (PA[i, j] - sy) / U[j, j]
     except ZeroDivisionError:
-        return _plu_decomp(A, method+1)  # retry with altered pivoting technique
+        return _plu_decomp(A, method + 1)  # retry with altered pivoting technique
 
     return P, L, U
 
 
 def _solve_lower_triangular_1d(L, b):
     """dual_solve the equation Lx = b, for L lower diagonal matrix, b is 1 dimension"""
     n = L.shape[0]
@@ -653,10 +710,13 @@
     float, int, Dual or Dual2
     """
     if isinstance(val, (*FLOATS, *INTS)):
         return val
     elif isinstance(val, (Dual, Dual2)):
         return val._set_order(order)
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+
+DualTypes = Union[float, Dual, Dual2]
```

### Comparing `rateslib-0.1.0/rateslib/fx.py` & `rateslib-0.2.0/rateslib/fx.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 from pandas.tseries.offsets import CustomBusinessDay
 from itertools import product
 import warnings
 from datetime import timedelta, datetime
 import json
 
 from rateslib import defaults
-from rateslib.dual import Dual, dual_solve, set_order
-from rateslib.defaults import plot
-from rateslib.calendars import add_tenor
+from rateslib.dual import Dual, dual_solve, set_order, DualTypes
+from rateslib.default import plot
+from rateslib.calendars import add_tenor, CalInput
 from rateslib.curves import Curve, LineCurve
+
 """
 .. ipython:: python
    :suppress:
 
    from rateslib.curves import Curve
    from datetime import datetime as dt
 """
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 class FXRates:
     """
     Object to store and calculate FX rates for a consistent settlement date.
 
     Parameters
     ----------
     fx_rates : dict
@@ -103,35 +105,39 @@
     fx_array : ndarray
     """
 
     def __init__(
         self,
         fx_rates: dict,
         settlement: Optional[datetime] = None,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         self._ad = 1
         self.settlement = settlement
 
         # covert all str to lowercase and values to Dual
         def _convert_dual(k, v):
             if isinstance(v, Dual):
                 return v
             return Dual(v, f"fx_{k.lower()}")
-        self.fx_rates = {
-            k.lower(): _convert_dual(k, v) for k, v in fx_rates.items()
-        }
+
+        self.fx_rates = {k.lower(): _convert_dual(k, v) for k, v in fx_rates.items()}
 
         # find currencies
         self.pairs = [k for k in self.fx_rates.keys()]
         self.variables = tuple(f"fx_{pair}" for pair in self.pairs)
         self.currencies = {
-            k: i for i, k in enumerate(list(
-            dict.fromkeys([p[:3] for p in self.pairs] + [p[3:6] for p in self.pairs])
-        ))
+            k: i
+            for i, k in enumerate(
+                list(
+                    dict.fromkeys(
+                        [p[:3] for p in self.pairs] + [p[3:6] for p in self.pairs]
+                    )
+                )
+            )
         }
         self.currencies_list = list(self.currencies.keys())
         if base is None:
             if defaults.base_currency in self.currencies_list:
                 self.base = defaults.base_currency
             else:
                 self.base = self.currencies_list[0]
@@ -152,24 +158,24 @@
         # solve FX vector in linear system
         A = np.zeros((self.q, self.q), dtype="object")
         b = np.ones(self.q, dtype="object")
         A[0, 0] = 1.0
         for i, pair in enumerate(self.pairs):
             domestic_idx = self.currencies[pair[:3]]
             foreign_idx = self.currencies[pair[3:]]
-            A[i+1, domestic_idx] = -1.0
-            A[i+1, foreign_idx] = 1 / self.fx_rates[pair]
-            b[i+1] = 0
+            A[i + 1, domestic_idx] = -1.0
+            A[i + 1, foreign_idx] = 1 / self.fx_rates[pair]
+            b[i + 1] = 0
         x = dual_solve(A, b[:, np.newaxis])[:, 0]
         self.fx_vector = x
 
         # solve fx_rates array
         self.fx_array = np.eye(self.q, dtype="object")
         for i in range(self.q):
-            for j in range(i+1, self.q):
+            for j in range(i + 1, self.q):
                 self.fx_array[i, j], self.fx_array[j, i] = x[j] / x[i], x[i] / x[j]
 
     def restate(self, pairs: list[str], keep_ad: bool = False):
         """
         Recreate an :class:`FXRates` class using other, derived currency pairs.
 
         This will redefine the pairs to which delta risks are expressed in ``Dual``
@@ -198,26 +204,28 @@
            fxr2 = fxr.restate(["eurusd", "gbpusd", "usdjpy"])
            fxr2.convert(100, "gbp", "usd")
         """
         if set(pairs) == set(self.pairs) and keep_ad:
             return self.copy()  # no restate needed but return new instance
 
         restated_fx_rates = FXRates(
-            {pair: self.rate(pair) if keep_ad else self.rate(pair).real
-             for pair in pairs},
-            self.settlement
+            {
+                pair: self.rate(pair) if keep_ad else self.rate(pair).real
+                for pair in pairs
+            },
+            self.settlement,
         )
         return restated_fx_rates
 
     def convert(
         self,
         value: Union[Dual, float],
         domestic: str,
         foreign: Optional[str] = None,
-        on_error: str = "ignore"
+        on_error: str = "ignore",
     ):
         """
         Convert an amount of a domestic currency into a foreign currency.
 
         Parameters
         ----------
         value : float or Dual
@@ -250,26 +258,26 @@
         for ccy in [domestic, foreign]:
             if ccy not in self.currencies:
                 if on_error == "ignore":
                     return None
                 elif on_error == "warn":
                     warnings.warn(
                         f"'{ccy}' not in FXRates.currencies: returning None.",
-                        UserWarning
+                        UserWarning,
                     )
                     return None
                 else:
                     raise ValueError(f"'{ccy}' not in FXRates.currencies.")
 
         i, j = self.currencies[domestic.lower()], self.currencies[foreign.lower()]
         return value * self.fx_array[i, j]
 
     def convert_positions(
         self,
-        array: Union[np.array, list],
+        array: Union[np.ndarray, list],
         base: Optional[str] = None,
     ):
         """
         Convert an array of currency cash positions into a single base currency.
 
         Parameters
         ----------
@@ -335,20 +343,15 @@
         )
         for pair in value.vars:
             if pair[:3] == "fx_":
                 delta = value.gradient(pair)[0]
                 _ += self._get_positions_from_delta(delta, pair[3:], base)
         return Series(_, index=self.currencies_list)
 
-    def _get_positions_from_delta(
-        self,
-        delta: float,
-        pair: str,
-        base: str
-    ):
+    def _get_positions_from_delta(self, delta: float, pair: str, base: str):
         """Return an array of cash positions determined from an FX pair delta risk."""
         b_idx = self.currencies[base]
         domestic, foreign = pair[:3], pair[3:]
         d_idx, f_idx = self.currencies[domestic], self.currencies[foreign]
         _ = np.zeros(self.q)
 
         # f_val = -delta * float(self.fx_array[b_idx, d_idx]) * float(self.fx_array[d_idx, f_idx])**2
@@ -489,15 +492,15 @@
 
         self._ad = order
         self.fx_vector = np.array([set_order(v, order) for v in self.fx_vector])
         x = self.fx_vector
         # solve fx_rates array
         self.fx_array = np.eye(self.q, dtype="object")
         for i in range(self.q):
-            for j in range(i+1, self.q):
+            for j in range(i + 1, self.q):
                 self.fx_array[i, j], self.fx_array[j, i] = x[j] / x[i], x[i] / x[j]
         for k, v in self.fx_rates.items():
             self.fx_rates[k] = set_order(v, order)
 
         return None
 
     def to_json(self):
@@ -525,17 +528,17 @@
         container = {
             "fx_rates": {k: float(v) for k, v in self.fx_rates.items()},
             "settlement": settlement,
             "base": self.base,
         }
         return json.dumps(container, default=str)
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     @classmethod
     def from_json(cls, fx_rates, **kwargs):
         """
         Load an FXRates object from a JSON string.
 
         This is usually required if a saved or transmitted object is to be recovered
@@ -580,17 +583,15 @@
         return True
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def copy(self):
         return FXRates(
-            fx_rates=self.fx_rates.copy(),
-            settlement=self.settlement,
-            base=self.base
+            fx_rates=self.fx_rates.copy(), settlement=self.settlement, base=self.base
         )
 
 
 class FXForwards:
     """
     Class for storing and calculating FX forward rates.
 
@@ -651,14 +652,15 @@
     currencies: dict
     q : int
     currencies_list : list
     transform : ndarray
     base : str
     fx_rates_immediate : FXRates
     """
+
     def update(
         self,
         fx_rates: Optional[Union[FXRates, list[FXRates]]] = None,
         fx_curves: Optional[dict] = None,
         base: Optional[str] = None,
     ):
         """
@@ -771,66 +773,64 @@
            fxf.update()
            fxf.rate("usdeur", dt(2022, 7, 15))
 
         """
         if isinstance(fx_curves, dict):
             self.fx_curves = {k.lower(): v for k, v in fx_curves.items()}
 
-            self.immediate = None
             self.terminal = datetime(2200, 1, 1)
-            for _, curve in self.fx_curves.items():
-                if self.immediate is None:
-                    self.immediate = curve.node_dates[0]
+            for flag, (_, curve) in enumerate(self.fx_curves.items()):
+                if flag == 0:
+                    self.immediate: datetime = curve.node_dates[0]
                 elif self.immediate != curve.node_dates[0]:
                     raise ValueError("`fx_curves` do not have the same initial date.")
                 if isinstance(curve, LineCurve):
                     raise TypeError("`fx_curves` must be DF based, not type LineCurve.")
                 if curve.node_dates[-1] < self.terminal:
                     self.terminal = curve.node_dates[-1]
 
         if fx_rates is not None:
             self.fx_rates = fx_rates
 
         if isinstance(self.fx_rates, list):
-            acyclic_fxf = None
-            for fx_rates_obj in self.fx_rates:
+            for flag, fx_rates_obj in enumerate(self.fx_rates):
                 # create sub FXForwards for each FXRates instance and re-combine.
                 # This reuses the arg validation of a single FXRates object and
                 # dependency of FXRates with fx_curves.
-                if acyclic_fxf is None:
+                if flag == 0:
                     sub_curves = self._get_curves_for_currencies(
                         self.fx_curves, fx_rates_obj.currencies_list
                     )
-                    acyclic_fxf = FXForwards(
+                    acyclic_fxf: FXForwards = FXForwards(
                         fx_rates=fx_rates_obj,
                         fx_curves=sub_curves,
                     )
                 else:
                     # calculate additional FX rates from previous objects
                     # in the same settlement frame.
                     pre_currencies = [
-                        ccy for ccy in acyclic_fxf.currencies_list
+                        ccy
+                        for ccy in acyclic_fxf.currencies_list
                         if ccy not in fx_rates_obj.currencies_list
                     ]
                     pre_rates = {
                         f"{fx_rates_obj.base}{ccy}": acyclic_fxf.rate(
                             f"{fx_rates_obj.base}{ccy}", fx_rates_obj.settlement
                         )
                         for ccy in pre_currencies
                     }
                     combined_fx_rates = FXRates(
                         fx_rates={**fx_rates_obj.fx_rates, **pre_rates},
-                        settlement=fx_rates_obj.settlement
+                        settlement=fx_rates_obj.settlement,
                     )
                     sub_curves = self._get_curves_for_currencies(
                         self.fx_curves, fx_rates_obj.currencies_list + pre_currencies
                     )
                     acyclic_fxf = FXForwards(
-                        fx_rates=combined_fx_rates,
-                        fx_curves=sub_curves
+                        fx_rates=combined_fx_rates, fx_curves=sub_curves
                     )
 
             if base is not None:
                 acyclic_fxf.base = base.lower()
 
             for attr in [
                 "currencies",
@@ -841,19 +841,19 @@
                 "fx_rates_immediate",
                 "pairs",
             ]:
                 setattr(self, attr, getattr(acyclic_fxf, attr))
         else:
             self.currencies = self.fx_rates.currencies
             self.q = len(self.currencies.keys())
-            self.currencies_list = list(self.currencies.keys())
+            self.currencies_list: list[str] = list(self.currencies.keys())
             self.transform = self._get_forwards_transformation_matrix(
                 self.q, self.currencies, self.fx_curves
             )
-            self.base = self.fx_rates.base if base is None else base
+            self.base: str = self.fx_rates.base if base is None else base
             self.pairs = self.fx_rates.pairs
             self.variables = tuple(f"fx_{pair}" for pair in self.pairs)
             self.fx_rates_immediate = self._update_fx_rates_immediate()
 
     def __init__(
         self,
         fx_rates: Union[FXRates, list[FXRates]],
@@ -862,15 +862,17 @@
     ):
         self._ad = 1
         self.update(fx_rates, fx_curves, base)
 
     @staticmethod
     def _get_curves_for_currencies(fx_curves, currencies):
         ps = product(currencies, currencies)
-        ret = {p[0]+p[1]: fx_curves[p[0]+p[1]] for p in ps if p[0]+p[1] in fx_curves}
+        ret = {
+            p[0] + p[1]: fx_curves[p[0] + p[1]] for p in ps if p[0] + p[1] in fx_curves
+        }
         return ret
 
     @staticmethod
     def _get_forwards_transformation_matrix(q, currencies, fx_curves):
         """
         Performs checks to ensure FX forwards can be generated from provided DF curves.
 
@@ -906,15 +908,15 @@
     @staticmethod
     def _get_recursive_chain(
         T: np.ndarray,
         start_idx: int,
         search_idx: int,
         traced_paths: list[int] = [],
         recursive_path: list[dict] = [],
-    ):
+    ) -> tuple[bool, list[dict]]:
         """
         Recursively calculate map from a cash currency to another via collateral curves.
 
         Parameters
         ----------
         T : ndarray
             The transformation mapping of cash and collateral currencies.
@@ -955,32 +957,32 @@
         if search_idx in row_paths:
             recursive_path.append({"row": search_idx})
             return True, recursive_path
         if search_idx in col_paths:
             recursive_path.append({"col": search_idx})
             return True, recursive_path
 
-        for (axis, paths) in [("row", row_paths), ("col", col_paths)]:
+        for axis, paths in [("row", row_paths), ("col", col_paths)]:
             for path_idx in paths:
                 if path_idx == start_idx:
                     pass
                 elif path_idx != search_idx and path_idx not in traced_paths:
                     recursive_path_app = recursive_path + [{axis: path_idx}]
                     traced_paths_app = traced_paths + [path_idx]
                     recursion = FXForwards._get_recursive_chain(
                         T, path_idx, search_idx, traced_paths_app, recursive_path_app
                     )
                     if recursion[0]:
                         return recursion
 
         return False, recursive_path
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def _update_fx_rates_immediate(self):
         """
         Find the immediate FX rates values.
 
         Notes
         -----
@@ -995,28 +997,28 @@
                     continue
                 cash_ccy = self.currencies_list[row]
                 coll_ccy = self.currencies_list[col]
                 settlement = self.fx_rates.settlement
                 v_i = self.fx_curves[f"{coll_ccy}{coll_ccy}"][settlement]
                 w_i = self.fx_curves[f"{cash_ccy}{coll_ccy}"][settlement]
                 pair = f"{cash_ccy}{coll_ccy}"
-                fx_rates_immediate.update({
-                   pair: self.fx_rates.fx_array[row, col] * v_i / w_i
-                })
+                fx_rates_immediate.update(
+                    {pair: self.fx_rates.fx_array[row, col] * v_i / w_i}
+                )
 
         fx_rates_immediate = FXRates(fx_rates_immediate, self.immediate)
         return fx_rates_immediate.restate(self.fx_rates.pairs, keep_ad=True)
 
     def rate(
         self,
         pair: str,
         settlement: Optional[datetime] = None,
         path: Optional[list[dict]] = None,
         return_path: bool = False,
-    ):
+    ) -> Union[DualTypes, tuple[DualTypes, list[dict]]]:
         """
         Return the fx forward rate for a currency pair.
 
         Parameters
         ----------
         pair : str
             The FX pair in usual domestic:foreign convention (6 digit code).
@@ -1051,36 +1053,40 @@
         given the available curves.
 
         .. math::
 
            f_{DOMFOR, i} = f_{DOMALT, i} ...  f_{ALTFOR, i}
 
         """
-        def _get_d_f_idx_and_path(pair, path: dict):
+
+        def _get_d_f_idx_and_path(pair, path: Optional[list[dict]]) \
+                -> tuple[int, int, list[dict]]:
             domestic, foreign = pair[:3].lower(), pair[3:].lower()
-            d_idx = self.fx_rates_immediate.currencies[domestic]
-            f_idx = self.fx_rates_immediate.currencies[foreign]
+            d_idx: int = self.fx_rates_immediate.currencies[domestic]
+            f_idx: int = self.fx_rates_immediate.currencies[foreign]
             if path is None:
                 path = self._get_recursive_chain(self.transform, f_idx, d_idx)[1]
             return d_idx, f_idx, path
 
         # perform a fast conversion if settlement aligns with known dates,
         if settlement is None:
             settlement = self.immediate
-        elif settlement < self.immediate:
+        elif settlement < self.immediate:  # type: ignore[operator]
             raise ValueError("`settlement` cannot be before immediate FX rate date.")
 
         if settlement == self.fx_rates_immediate.settlement:
             rate_ = self.fx_rates_immediate.rate(pair)
             if return_path:
                 _, _, path = _get_d_f_idx_and_path(pair, path)
                 return rate_, path
             return rate_
-        elif isinstance(self.fx_rates, FXRates) and \
-                settlement == self.fx_rates.settlement:
+        elif (
+            isinstance(self.fx_rates, FXRates)
+            and settlement == self.fx_rates.settlement
+        ):
             rate_ = self.fx_rates.rate(pair)
             if return_path:
                 _, _, path = _get_d_f_idx_and_path(pair, path)
                 return rate_, path
             return rate_
 
         # otherwise must rely on curves and path search which is slower
@@ -1104,20 +1110,15 @@
                 rate_ *= v_i / w_i
                 current_idx = route["row"]
 
         if return_path:
             return rate_, path
         return rate_
 
-    def positions(
-        self,
-        value,
-        base: Optional[str] = None,
-        aggregate: bool = False
-    ):
+    def positions(self, value, base: Optional[str] = None, aggregate: bool = False):
         """
         Convert a base value with FX rate sensitivities into an array of cash positions
         by settlement date.
 
         Parameters
         ----------
         value : float or Dual
@@ -1166,40 +1167,40 @@
             fx_rates = self.fx_rates
         else:
             fx_rates = [self.fx_rates]
 
         dates = list({fxr.settlement for fxr in fx_rates})
         if self.immediate not in dates:
             dates.insert(0, self.immediate)
-        df = DataFrame(0., index=self.currencies_list, columns=dates)
+        df = DataFrame(0.0, index=self.currencies_list, columns=dates)
         df.loc[base, self.immediate] = float(value)
         for pair in value.vars:
             if pair[:3] == "fx_":
                 dom_, for_ = pair[3:6], pair[6:9]
                 for fxr in fx_rates:
                     if dom_ in fxr.currencies_list and for_ in fxr.currencies_list:
                         delta = value.gradient(pair)[0]
                         _ = fxr._get_positions_from_delta(delta, pair[3:], base)
                         _ = Series(_, index=fxr.currencies_list, name=fxr.settlement)
-                        df = df.add(_.to_frame(), fill_value=0.)
+                        df = df.add(_.to_frame(), fill_value=0.0)
 
         if aggregate:
             return df.sum(axis=1)
         else:
             return df.sort_index(axis=1)
 
     def convert(
         self,
-        value: Union[Dual, float],
+        value: DualTypes,
         domestic: str,
         foreign: Optional[str] = None,
         settlement: Optional[datetime] = None,
         value_date: Optional[datetime] = None,
         collateral: Optional[str] = None,
-        on_error: str = "ignore"
+        on_error: str = "ignore",
     ):
         """
         Convert an amount of a domestic currency, as of a settlement date
         into a foreign currency, valued on another date.
 
         Parameters
         ----------
@@ -1254,73 +1255,90 @@
         for ccy in [domestic, foreign]:
             if ccy not in self.currencies:
                 if on_error == "ignore":
                     return None
                 elif on_error == "warn":
                     warnings.warn(
                         f"'{ccy}' not in FXForwards.currencies: returning None.",
-                        UserWarning
+                        UserWarning,
                     )
                     return None
                 else:
                     raise ValueError(f"'{ccy}' not in FXForwards.currencies.")
 
         if settlement is None:
             settlement = self.immediate
         if value_date is None:
             value_date = settlement
 
-        fx_rate = self.rate(domestic + foreign, settlement)
+        fx_rate: DualTypes = self.rate(domestic + foreign, settlement)
         if value_date == settlement:
             return fx_rate * value
         else:
             crv = self.curve(foreign, collateral)
             return fx_rate * value * crv[settlement] / crv[value_date]
 
     def convert_positions(
         self,
-        array: Union[np.array, list, DataFrame, Series],
+        array: Union[np.ndarray, list, DataFrame, Series],
         base: Optional[str] = None,
     ):
         """
         Convert an input of currency cash positions into a single base currency value.
 
         Parameters
         ----------
         array : list, 1d ndarray of floats, or Series, or DataFrame
-            The cash positions to simultaneously convert in the base currency. **Must**
-            be ordered by currency as defined in the attribute ``FXRates.currencies``.
-            XX TODO relabel this docstring correctly.
+            The cash positions to simultaneously convert to base currency value.
+            If a DataFrame, must be indexed by currencies (3-digit lowercase) and the
+            column headers must be settlement dates.
+            If a Series, must be indexed by currencies (3-digit lowercase).
+            If a 1d array or sequence, must
+            be ordered by currency as defined in the attribute ``FXForward.currencies``.
         base : str, optional
             The currency to convert to (3-digit code). Uses instance ``base`` if not
             given.
 
         Returns
         -------
         Dual
 
         Examples
         --------
 
         .. ipython:: python
 
-           fxr = FXRates({"usdnok": 8.0})
-           fxr.currencies
-           fxr.convert_positions([0, 1000000], "usd")
+           fxr = FXRates({"usdnok": 8.0}, settlement=dt(2022, 1, 1))
+           usdusd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99})
+           noknok = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.995})
+           fxf = FXForwards(fxr, {"usdusd": usdusd, "noknok": noknok, "nokusd": noknok})
+           fxf.currencies
+           fxf.convert_positions([0, 1000000], "usd")
+
+        .. ipython:: python
+
+           fxr.convert_positions(Series([1000000, 0], index=["nok", "usd"]), "usd")
+
+        .. ipython:: python
+
+           positions = DataFrame(index=["usd", "nok"], data={
+               dt(2022, 6, 2): [0, 1000000],
+               dt(2022, 9, 7): [0, -1000000],
+           })
+           fxf.convert_positions(positions, "usd")
         """
         base = self.base if base is None else base.lower()
 
         if isinstance(array, Series):
             array_ = array.to_frame(name=self.immediate)
         elif isinstance(array, DataFrame):
             array_ = array
         else:
             array_ = DataFrame(
-                {self.immediate: np.asarray(array)},
-                index=self.currencies_list
+                {self.immediate: np.asarray(array)}, index=self.currencies_list
             )
 
         # j = self.currencies[base]
         # return np.sum(array_ * self.fx_array[:, j])
         sum = 0
         for d in array_.columns:
             d_sum = 0
@@ -1333,15 +1351,15 @@
         return sum
 
     def swap(
         self,
         pair: str,
         settlements: list[datetime],
         path: Optional[list[dict]] = None,
-    ):
+    ) -> DualTypes:
         """
         Return the FXSwap mid-market rate for the given currency pair.
 
         Parameters
         ----------
         pair : str
             The FX pair in usual domestic:foreign convention (6-digit code).
@@ -1353,16 +1371,16 @@
             internal calculation to avoid repeatedly calculating the same path. Use of
             this argument in normal circumstances is not recommended.
 
         Returns
         -------
         Dual
         """
-        fx0 = self.rate(pair, settlements[0], path)
-        fx1 = self.rate(pair, settlements[1], path)
+        fx0: DualTypes = self.rate(pair, settlements[0], path)
+        fx1: DualTypes = self.rate(pair, settlements[1], path)
         return (fx1 - fx0) * 10000
 
     def _full_curve(self, cashflow: str, collateral: str):
         """
         Calculate a cash collateral curve.
 
         Parameters
@@ -1390,24 +1408,25 @@
         cash_ccy, coll_ccy = cashflow.lower(), collateral.lower()
         cash_idx, coll_idx = self.currencies[cash_ccy], self.currencies[coll_ccy]
         path = self._get_recursive_chain(self.transform, coll_idx, cash_idx)[1]
         end = list(self.fx_curves[f"{coll_ccy}{coll_ccy}"].nodes.keys())[-1]
         days = (end - self.immediate).days
         nodes = {
             k: (
-                self.rate(f"{cash_ccy}{coll_ccy}", k, path=path) /
-                self.fx_rates_immediate.fx_array[cash_idx, coll_idx] *
-                self.fx_curves[f"{coll_ccy}{coll_ccy}"][k]
-            ) for k in [self.immediate + timedelta(days=i) for i in range(days+1)]
+                self.rate(f"{cash_ccy}{coll_ccy}", k, path=path)
+                / self.fx_rates_immediate.fx_array[cash_idx, coll_idx]
+                * self.fx_curves[f"{coll_ccy}{coll_ccy}"][k]
+            )
+            for k in [self.immediate + timedelta(days=i) for i in range(days + 1)]
         }
         return Curve(nodes)
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def curve(
         self,
         cashflow: str,
         collateral: str,
         convention: Optional[str] = None,
         modifier: Optional[Union[str, bool]] = False,
@@ -1513,22 +1532,22 @@
         elif isinstance(right, str):
             right_ = add_tenor(self.immediate, right, None, None)
         elif isinstance(right, datetime):
             right_ = right
         else:
             raise ValueError("`right` must be supplied as datetime or tenor string.")
 
-        points : int = (right_ - left_).days
+        points: int = (right_ - left_).days
         x = [left_ + timedelta(days=i) for i in range(points)]
         _, path = self.rate(pair, x[0], return_path=True)
-        rates = [self.rate(pair, _, path=path) for _ in x]
+        rates: list[DualTypes] = [self.rate(pair, _, path=path) for _ in x]
         if not fx_swap:
-            y = [rates]
+            y: list[DualTypes] = [rates]
         else:
-            y = [(rate - rates[0])*10000 for rate in rates]
+            y = [(rate - rates[0]) * 10000 for rate in rates]
         return plot(x, y)
 
     def _set_ad_order(self, order):
         self._ad = order
         for curve in self.fx_curves.values():
             curve._set_ad_order(order)
 
@@ -1543,15 +1562,15 @@
         if isinstance(self.fx_rates, list):
             fx_rates = [_.to_json() for _ in self.fx_rates]
         else:
             fx_rates = self.fx_rates.to_json()
         container = {
             "base": self.base,
             "fx_rates": fx_rates,
-            "fx_curves": {k: v.to_json() for k, v in self.fx_curves.items()}
+            "fx_curves": {k: v.to_json() for k, v in self.fx_curves.items()},
         }
         return json.dumps(container, default=str)
 
     @classmethod
     def from_json(cls, fx_forwards, **kwargs):
         """
         Loads an FXForwards object from JSON.
@@ -1661,56 +1680,63 @@
 
        w_{dom:for,i} = \\frac{f_{DOMFOR,i}}{F_{DOMFOR,0}} v_{for:for,i}
 
     The returned curve contains contrived methods to calculate this dynamically and
     efficiently from the combination of curves and FX rates that are available within
     the given :class:`FXForwards` instance.
     """
+
     def __init__(
         self,
         cashflow: str,
         collateral: str,
         fx_forwards: FXForwards,
         convention: Optional[str] = None,
         modifier: Optional[Union[str, bool]] = False,
-        calendar: Optional[Union[CustomBusinessDay, bool]] = False,
+        calendar: Optional[Union[CalInput, bool]] = False,
     ):
         cash_ccy, coll_ccy = cashflow.lower(), collateral.lower()
         self._is_proxy = True
         self.fx_forwards = fx_forwards
         self.cash_currency = cash_ccy
         self.cash_pair = f"{cash_ccy}{cash_ccy}"
         self.cash_idx = self.fx_forwards.currencies[cash_ccy]
         self.coll_currency = coll_ccy
         self.coll_pair = f"{coll_ccy}{coll_ccy}"
         self.coll_idx = self.fx_forwards.currencies[coll_ccy]
         self.pair = f"{cash_ccy}{coll_ccy}"
         self.path = self.fx_forwards._get_recursive_chain(
             self.fx_forwards.transform, self.coll_idx, self.cash_idx
         )[1]
-        self.terminal = list(
-            self.fx_forwards.fx_curves[self.cash_pair].nodes.keys()
-        )[-1]
+        self.terminal = list(self.fx_forwards.fx_curves[self.cash_pair].nodes.keys())[
+            -1
+        ]
 
         default_curve = Curve(
             {},
-            convention=self.fx_forwards.fx_curves[self.cash_pair].convention if convention is None else convention,
-            modifier=self.fx_forwards.fx_curves[self.cash_pair].modifier if modifier is False else modifier,
-            calendar=self.fx_forwards.fx_curves[self.cash_pair].calendar if calendar is False else calendar,
+            convention=self.fx_forwards.fx_curves[self.cash_pair].convention
+            if convention is None
+            else convention,
+            modifier=self.fx_forwards.fx_curves[self.cash_pair].modifier
+            if modifier is False
+            else modifier,
+            calendar=self.fx_forwards.fx_curves[self.cash_pair].calendar
+            if calendar is False
+            else calendar,
         )
         self.convention = default_curve.convention
         self.modifier = default_curve.modifier
         self.calendar = default_curve.calendar
         self.node_dates = [self.fx_forwards.immediate, self.terminal]
 
     def __getitem__(self, date: datetime):
         return (
-            self.fx_forwards.rate(self.pair, date, path=self.path) /
-            self.fx_forwards.fx_rates_immediate.fx_array[self.cash_idx, self.coll_idx] *
-            self.fx_forwards.fx_curves[self.coll_pair][date]
+            self.fx_forwards.rate(self.pair, date, path=self.path)
+            / self.fx_forwards.fx_rates_immediate.fx_array[self.cash_idx, self.coll_idx]
+            * self.fx_forwards.fx_curves[self.coll_pair][date]
         )
 
     def to_json(self):  # pragma: no cover
         """
         Not implemented for :class:`~rateslib.fx.ProxyCurve` s.
         :return:
         """
@@ -1724,23 +1750,11 @@
 
     def _set_ad_order(self):  # pragma: no cover
         """
         Not implemented for :class:`~rateslib.fx.ProxyCurve` s.
         """
         return NotImplementedError("`set_ad_order` not available on proxy curve.")
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
-
-#####
-
-# TODO:
-
-# 1) PERFORMANCE:
-# Profiling shows that dual_solve for the determination of fx_vector is quite slow
-# due to the structure and sparsity of the matrix it should be possible to use a
-# more direct algorithm to determine the dual gradients of the fx vector components.
-
-# 2) UTILITY:
-# Consider allowing a to_json method for proxy curves to mediate exchange of info.
-# Or better yet just configure a to_json method for an FXForwards object.
```

### Comparing `rateslib-0.1.0/rateslib/instruments.py` & `rateslib-0.2.0/rateslib/instruments.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 """
 
 from abc import abstractmethod, ABCMeta
 from datetime import datetime
 from typing import Optional, Union
 import abc
 import warnings
+from math import sqrt
 
 import numpy as np
-from scipy.optimize import brentq
+
+# from scipy.optimize import brentq
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, concat, date_range, Series
 
 from rateslib import defaults
 from rateslib.calendars import add_tenor, _add_days, get_calendar, dcf
 from rateslib.scheduling import Schedule
 from rateslib.curves import Curve, index_left, LineCurve
@@ -76,14 +78,100 @@
                 elif defaults.curve_not_in_solver == "warn":
                     warnings.warn("`curve` not found in `solver`.", UserWarning)
                     return curve
                 else:
                     raise ValueError("`curve` must be in `solver`.")
 
 
+def _get_curves_and_fx_maybe_from_solver(
+    curves_attr: Optional[Union[Curve, str, list]],
+    solver: Optional[Solver],
+    curves: Optional[Union[Curve, str, list]],
+    fx: Optional[Union[float, FXRates, FXForwards]],
+):
+    """
+    Parses the ``solver``, ``curves`` and ``fx`` arguments in combination.
+
+    Parameters
+    ----------
+    curves_attr
+        The curves attribute attached to the class.
+    solver
+        The solver argument passed in the outer method.
+    curves
+        The curves argument passed in the outer method.
+    fx
+        The fx argument agrument passed in the outer method.
+
+    Returns
+    -------
+    tuple : (leg1 forecasting, leg1 discounting, leg2 forecasting, leg2 discounting), fx
+
+    Notes
+    -----
+    If only one curve is given this is used as all four curves.
+
+    If two curves are given the forecasting curve is used as the forecasting
+    curve on both legs and the discounting curve is used as the discounting
+    curve for both legs.
+
+    If three curves are given the single discounting curve is used as the
+    discounting curve for both legs.
+    """
+    if fx is None:
+        if solver is None:
+            fx_ = None
+            # fx_ = 1.0
+        elif solver is not None:
+            if solver.fx is None:
+                fx_ = None
+                # fx_ = 1.0
+            else:
+                fx_ = solver.fx
+    else:
+        fx_ = fx
+
+    if curves is None and curves_attr is None:
+        return (None, None, None, None), fx_
+    elif curves is None:
+        curves = curves_attr
+
+    if isinstance(curves, (Curve, str)):
+        curves = [curves]
+    if solver is None:
+
+        def check_curve(curve):
+            if isinstance(curve, str):
+                raise ValueError(
+                    "`curves` must contain Curve, not str, if `solver` not given."
+                )
+            return curve
+
+        curves_ = tuple(check_curve(curve) for curve in curves)
+    else:
+        try:
+            curves_ = tuple(_get_curve_from_solver(curve, solver) for curve in curves)
+        except KeyError:
+            raise ValueError(
+                "`curves` must contain str curve `id` s existing in `solver` "
+                "(or its associated `pre_solvers`)"
+            )
+
+    if len(curves_) == 1:
+        curves_ *= 4
+    elif len(curves_) == 2:
+        curves_ *= 2
+    elif len(curves_) == 3:
+        curves_ += (curves_[1],)
+    elif len(curves_) > 4:
+        raise ValueError("Can only supply a maximum of 4 `curves`.")
+
+    return curves_, fx_
+
+
 # def _get_curves_and_fx_maybe_from_solver(
 #     solver: Optional[Solver],
 #     curves: Union[Curve, str, list],
 #     fx: Optional[Union[float, FXRates, FXForwards]],
 # ):
 #     """
 #     Parses the ``solver``, ``curves`` and ``fx`` arguments in combination.
@@ -152,14 +240,15 @@
 
 
 class Sensitivities:
     """
     Base class to add risk sensitivity calculations to an object with an ``npv()``
     method.
     """
+
     def delta(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
@@ -250,15 +339,15 @@
 
 
 class BaseMixin:
     _fixed_rate_mixin = False
     _float_spread_mixin = False
     _leg2_fixed_rate_mixin = False
     _leg2_float_spread_mixin = False
-    _rate_scalar = 1.
+    _rate_scalar = 1.0
 
     @property
     def fixed_rate(self):
         """
         float or None : If set will also set the ``fixed_rate`` of the contained
         leg1.
 
@@ -325,89 +414,14 @@
     @leg2_float_spread.setter
     def leg2_float_spread(self, value):
         if not self._leg2_float_spread_mixin:
             raise AttributeError("Cannot set `leg2_float_spread` for this Instrument.")
         self._leg2_float_spread = value
         self.leg2.float_spread = value
 
-    def _get_curves_and_fx_maybe_from_solver(
-        self,
-        solver: Optional[Solver],
-        curves: Optional[Union[Curve, str, list]],
-        fx: Optional[Union[float, FXRates, FXForwards]],
-    ):
-        """
-        Parses the ``solver``, ``curves`` and ``fx`` arguments in combination.
-
-        Returns
-        -------
-        tuple : (leg1 forecasting, leg1 discounting, leg2 forecasting, leg2 discounting), fx
-
-        Notes
-        -----
-        If only one curve is given this is used as all four curves.
-
-        If two curves are given the forecasting curve is used as the forecasting
-        curve on both legs and the discounting curve is used as the discounting
-        curve for both legs.
-
-        If three curves are given the single discounting curve is used as the
-        discounting curve for both legs.
-        """
-        if fx is None:
-            if solver is None:
-                fx_ = None
-                # fx_ = 1.0
-            elif solver is not None:
-                if solver.fx is None:
-                    fx_ = None
-                    # fx_ = 1.0
-                else:
-                    fx_ = solver.fx
-        else:
-            fx_ = fx
-
-        if curves is None and getattr(self, "curves", None) is None:
-            return (None, None, None, None), fx_
-        elif curves is None:
-            curves = self.curves
-
-        if isinstance(curves, (Curve, str)):
-            curves = [curves]
-        if solver is None:
-            def check_curve(curve):
-                if isinstance(curve, str):
-                    raise ValueError(
-                        "`curves` must contain Curve, not str, if `solver` not given."
-                    )
-                return curve
-
-            curves_ = tuple(check_curve(curve) for curve in curves)
-        else:
-            try:
-                curves_ = tuple(
-                    _get_curve_from_solver(curve, solver) for curve in curves
-                )
-            except KeyError:
-                raise ValueError(
-                    "`curves` must contain str curve `id` s existing in `solver` "
-                    "(or its associated `pre_solvers`)"
-                )
-
-        if len(curves_) == 1:
-            curves_ *= 4
-        elif len(curves_) == 2:
-            curves_ *= 2
-        elif len(curves_) == 3:
-            curves_ += (curves_[1],)
-        elif len(curves_) > 4:
-            raise ValueError("Can only supply a maximum of 4 `curves`.")
-
-        return curves_, fx_
-
 
 class Value(BaseMixin):
     """
     A null instrument which can be used within a :class:`~rateslib.solver.Solver`
     to directly parametrise a node.
 
     Parameters
@@ -458,22 +472,322 @@
         base: Optional[str] = None,
     ):
         """
         Return the forecasting :class:`~rateslib.curves.Curve` or
         :class:`~rateslib.curves.LineCurve` value on the ``effective`` date of the
         instrument.
         """
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, None
+        )
         return curves[0][self.effective]
 
 
 ### Securities
 
 
-class FixedRateBond(Sensitivities, BaseMixin):
+class BondMixin:
+    def ex_div(self, settlement: datetime):
+        """
+        Return a boolean whether the security is ex-div on the settlement.
+
+        Parameters
+        ----------
+        settlement : datetime
+             The settlement date to test.
+
+        Returns
+        -------
+        bool
+        """
+        prev_a_idx = index_left(
+            self.leg1.schedule.aschedule,
+            len(self.leg1.schedule.aschedule),
+            settlement,
+        )
+        ex_div_date = add_tenor(
+            self.leg1.schedule.aschedule[prev_a_idx + 1],
+            f"{-self.ex_div_days}B",
+            None,  # modifier not required for business day tenor
+            self.leg1.schedule.calendar,
+        )
+        return True if settlement >= ex_div_date else False
+
+    def _accrued_frac(self, settlement: datetime):
+        """
+        Return the accrual fraction of period between last coupon and settlement and
+        coupon period left index
+        """
+        acc_idx = index_left(
+            self.leg1.schedule.aschedule,
+            len(self.leg1.schedule.aschedule),
+            settlement,
+        )
+        return (
+            (settlement - self.leg1.schedule.aschedule[acc_idx])
+            / (
+                self.leg1.schedule.aschedule[acc_idx + 1]
+                - self.leg1.schedule.aschedule[acc_idx]
+            )
+        ), acc_idx
+
+    def _npv_local(
+        self,
+        curve: Union[Curve, LineCurve],
+        disc_curve: Curve,
+        fx: Optional[Union[float, FXRates, FXForwards]],
+        base: Optional[str],
+        settlement: datetime,
+        projection: datetime,
+    ):
+        """
+        Return the NPV (local) of the security by summing cashflow valuations.
+
+        Parameters
+        ----------
+        curve : Curve or LineCurve
+            A curve used for projecting cashflows of floating rates.
+        disc_curve : Curve, str or list of such
+            A single :class:`Curve` for discounting cashflows.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+        settlement : datetime
+            The date of settlement of the bond which declares which cashflows are
+            unpaid and therefore valid for the calculation.
+        projection : datetime, optional
+           Curves discount cashflows to the initial node of the Curve. This parameter
+           allows the NPV to be projected forward to a future date under the appropriate
+           discounting mechanism. If *None* is not projected forward.
+
+        Returns
+        -------
+        float, Dual, Dual2
+
+        Notes
+        -----
+        The cashflows for determination (excluding an ``ex_div`` cashflow) are
+        evaluated by ``settlement``.
+
+        The date for which the PV is returned is by ``projection``, and not the
+        initial node date of the ``disc_curve``.
+        """
+        npv = self.leg1.npv(curve, disc_curve, fx, base)
+
+        # now must systematically deduct any cashflow between the initial node date
+        # and the settlement date, including the cashflow after settlement if ex_div.
+        initial_idx = index_left(
+            self.leg1.schedule.aschedule,
+            self.leg1.schedule.n_periods + 1,
+            disc_curve.node_dates[0],
+        )
+        settle_idx = index_left(
+            self.leg1.schedule.aschedule,
+            self.leg1.schedule.n_periods + 1,
+            settlement,
+        )
+
+        for period_idx in range(initial_idx, settle_idx):
+            # deduct coupon period
+            npv -= self.leg1.periods[period_idx].npv(curve, disc_curve, fx, base)
+
+        if self.ex_div(settlement):
+            # deduct coupon after settlement which is also unpaid
+            npv -= self.leg1.periods[settle_idx].npv(curve, disc_curve, fx, base)
+
+        if projection is None:
+            return npv
+        else:
+            return npv / disc_curve[projection]
+
+    def npv(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        local: bool = False,
+    ):
+        """
+        Return the NPV of the security by summing cashflow valuations.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+        local : bool, optional
+            If `True` will ignore the ``base`` request and return a dict identifying
+            local currency NPV.
+
+        Returns
+        -------
+        float, Dual, Dual2 or dict of such
+
+        Notes
+        -----
+        The ``settlement`` date of the bond is inferred from the objects ``settle``
+        days parameter and the initial date of the supplied ``curves``.
+        The NPV returned is for immediate settlement.
+
+        If **only one curve** is given this is used as all four curves.
+
+        If **two curves** are given the forecasting curve is used as the forecasting
+        curve on both legs and the discounting curve is used as the discounting
+        curve for both legs.
+        """
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        settlement = add_tenor(
+            curves[1].node_dates[0],
+            f"{self.settle}B",
+            None,
+            self.leg1.schedule.calendar,
+        )
+        base = self.leg1.currency if local else base
+        npv = self._npv_local(curves[0], curves[1], fx, base, settlement, None)
+        if local:
+            return {self.leg1.currency: npv}
+        else:
+            return npv
+
+    def analytic_delta(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Union[float, FXRates, FXForwards] = 1.0,
+        base: Optional[str] = None,
+    ):
+        """
+        Return the analytic delta of the security via summing all periods.
+
+        Parameters
+        ----------
+        curve : Curve
+            The forecasting curve object. Not used unless it is set equal to
+            ``disc_curve``.
+        disc_curve : Curve, optional
+            The discounting curve object used in calculations.
+            Set equal to ``curve`` if not given.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
+            object, converts from local currency into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
+            :class:`~rateslib.fx.FXForwards` object.
+
+        Returns
+        -------
+        float, Dual, Dual2
+        """
+        disc_curve = disc_curve or curve
+        settlement = add_tenor(
+            disc_curve.node_dates[0],
+            f"{self.settle}B",
+            None,
+            self.leg1.schedule.calendar,
+        )
+        a_delta = self.leg1.analytic_delta(curve, disc_curve, fx, base)
+        if self.ex_div(settlement):
+            # deduct the next coupon which has otherwise been included in valuation
+            current_period = index_left(
+                self.leg1.schedule.aschedule,
+                self.leg1.schedule.n_periods + 1,
+                settlement,
+            )
+            a_delta -= self.leg1.periods[current_period].analytic_delta(
+                curve, disc_curve, fx, base
+            )
+        return a_delta
+
+    def cashflows(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        settlement: datetime = None,
+    ):
+        """
+        Return the properties of the security used in calculating cashflows.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx_rate`` is an ``FXRates`` or ``FXForwards`` object.
+        settlement : datetime, optional
+            The settlement date of the security. If *None* adds the regular ``settle``
+            time to the initial node date of the given discount ``curves``.
+
+        Returns
+        -------
+        DataFrame
+        """
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        if settlement is None:
+            settlement = add_tenor(
+                curves[1].node_dates[0],
+                f"{self.settle}B",
+                None,
+                self.leg1.schedule.calendar,
+            )
+        cashflows = self.leg1.cashflows(curves[0], curves[1], fx, base)
+        if self.ex_div(settlement):
+            # deduct the next coupon which has otherwise been included in valuation
+            current_period = index_left(
+                self.leg1.schedule.aschedule,
+                self.leg1.schedule.n_periods + 1,
+                settlement,
+            )
+            cashflows.loc[current_period, defaults.headers["npv"]] = 0
+            cashflows.loc[current_period, defaults.headers["npv_fx"]] = 0
+        return cashflows
+
+
+class FixedRateBond(Sensitivities, BondMixin, BaseMixin):
     # TODO ensure calculations work for amortizing bonds.
     """
     Create a fixed rate bond security.
 
     Parameters
     ----------
     effective : datetime
@@ -578,42 +892,19 @@
             currency=currency,
             amortization=amortization,
             convention=convention,
             fixed_rate=fixed_rate,
             initial_exchange=False,
         )
         if self.leg1.amortization != 0:
+            # Note if amortization is added to FixedRateBonds must systematically
+            # go through and update all methods. Many rely on the quantity
+            # self.notional which is currently assumed to be a fixed quantity
             raise NotImplementedError("`amortization` for FixedRateBond must be zero.")
 
-    def ex_div(self, settlement: datetime):
-        """
-        Return a boolean whether the security is ex-div on the settlement.
-
-        Parameters
-        ----------
-        settlement : datetime
-             The settlement date to test.
-
-        Returns
-        -------
-        bool
-        """
-        prev_a_idx = index_left(
-            self.leg1.schedule.aschedule,
-            len(self.leg1.schedule.aschedule),
-            settlement,
-        )
-        ex_div_date = add_tenor(
-            self.leg1.schedule.aschedule[prev_a_idx+1],
-            f"{-self.ex_div_days}B",
-            None,  # modifier not required for business day tenor
-            self.leg1.schedule.calendar,
-        )
-        return True if settlement >= ex_div_date else False
-
     def accrued(self, settlement: datetime):
         """
         Calculate the accrued amount per nominal par value of 100.
 
         Parameters
         ----------
         settlement : datetime
@@ -627,38 +918,22 @@
 
            \\text{Accrued} = \\text{Coupon} \\times \\frac{\\text{Settle - Last Coupon}}{\\text{Next Coupon - Last Coupon}}
 
         """
         # TODO validate against effective and termination?
         frac, acc_idx = self._accrued_frac(settlement)
         if self.ex_div(settlement):
-            frac = (frac-1)  # accrued is negative in ex-div period
-        return (
-            frac * self.leg1.periods[acc_idx].cashflow / -self.leg1.notional * 100
-        )
+            frac = frac - 1  # accrued is negative in ex-div period
+        return frac * self.leg1.periods[acc_idx].cashflow / -self.leg1.notional * 100
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-    def _accrued_frac(self, settlement: datetime):
-        """
-        Return the accrual fraction of period between last coupon and settlement and
-        coupon period left index
-        """
-        acc_idx = index_left(
-            self.leg1.schedule.aschedule,
-            len(self.leg1.schedule.aschedule),
-            settlement,
-        )
-        return (
-            (settlement - self.leg1.schedule.aschedule[acc_idx]) /
-            (self.leg1.schedule.aschedule[acc_idx+1] -
-             self.leg1.schedule.aschedule[acc_idx])
-        ), acc_idx
+    # Analogue Methods
 
     def _price_from_ytm(self, ytm: float, settlement: datetime, dirty: bool = False):
         """
         Loop through all future cashflows and discount them with ``ytm`` to achieve
         correct price.
         """
         # TODO note this formula does not account for back stubs
@@ -671,26 +946,29 @@
         if self.leg1.periods[acc_idx].stub:
             # is a stub so must account for discounting in a different way.
             fd0 = self.leg1.periods[acc_idx].dcf * f * (1 - acc_frac)
         else:
             fd0 = 1 - acc_frac
 
         d = 0
-        for i, p_idx in enumerate(range(acc_idx, len(self.leg1.schedule.aschedule)-1)):
+        for i, p_idx in enumerate(
+            range(acc_idx, len(self.leg1.schedule.aschedule) - 1)
+        ):
             if i == 0 and self.ex_div(settlement):
                 continue
             else:
-                d += self.leg1.periods[p_idx].cashflow * v ** i
-        d += self.leg1.periods[-1].cashflow * v ** i
+                d += self.leg1.periods[p_idx].cashflow * v**i
+        d += self.leg1.periods[-1].cashflow * v**i
         p = v**fd0 * d / -self.leg1.notional * 100
         return p if dirty else p - self.accrued(settlement)
 
     def price(self, ytm: float, settlement: datetime, dirty: bool = False):
         """
-        Calculate the price of the security per nominal value of 100.
+        Calculate the price of the security per nominal value of 100, given
+        yield-to-maturity.
 
         Parameters
         ----------
         ytm : float
             The yield-to-maturity against which to determine the price.
         settlement : datetime
             The settlement date on which to determine the price.
@@ -822,15 +1100,15 @@
             _ = -self.price(Dual(float(ytm), "y"), settlement).gradient("y")[0]
         elif metric == "modified":
             price = -self.price(Dual(float(ytm), "y"), settlement, dirty=True)
             _ = -price.gradient("y")[0] / float(price) * 100
         elif metric == "duration":
             price = -self.price(Dual(float(ytm), "y"), settlement, dirty=True)
             f = 12 / defaults.frequency_months[self.leg1.schedule.frequency]
-            v = (1 + float(ytm) / (100 * f))
+            v = 1 + float(ytm) / (100 * f)
             _ = -price.gradient("y")[0] / float(price) * v * 100
         return _
 
     def convexity(self, ytm: float, settlement: datetime):
         """
         Return the second derivative of ``price`` w.r.t. ``ytm``.
 
@@ -916,156 +1194,214 @@
            )
            gilt.ytm(Dual(141.0701315, ["price", "a", "b"], [1, -0.5, 2]), dt(1999, 5, 27), True)
            gilt.ytm(Dual2(141.0701315, ["price", "a", "b"], [1, -0.5, 2]), dt(1999, 5, 27), True)
 
         """
 
         def root(y):
-            return self._price_from_ytm(y, settlement, dirty) - price
-        x = brentq(root, -99, 10000)
+            # we set this to work in float arithmetic for efficiency. Dual is added
+            # back below, see PR GH3
+            return self._price_from_ytm(y, settlement, dirty) - float(price)
+
+        # x = brentq(root, -99, 10000)  # remove dependence to scipy.optimize.brentq
+        # x, iters = _brents(root, -99, 10000)  # use own local brents code
+        x = _ytm_quadratic_converger2(root, -3.0, 2.0, 12.0)  # use special quad interp
 
         if isinstance(price, Dual):
             # use the inverse function theorem to express x as a Dual
             p = self._price_from_ytm(Dual(x, "y"), settlement, dirty)
             return Dual(x, price.vars, 1 / p.gradient("y")[0] * price.dual)
         elif isinstance(price, Dual2):
             # use the IFT in 2nd order to express x as a Dual2
             p = self._price_from_ytm(Dual2(x, "y"), settlement, dirty)
             dydP = 1 / p.gradient("y")[0]
-            d2ydP2 = - p.gradient("y", order=2)[0][0] * p.gradient("y")[0] ** -3
+            d2ydP2 = -p.gradient("y", order=2)[0][0] * p.gradient("y")[0] ** -3
             return Dual2(
                 x,
                 price.vars,
                 dydP * price.dual,
-                0.5 * (dydP * price.gradient(price.vars, order=2) +
-                d2ydP2 * np.matmul(price.dual[:, None], price.dual[None, :]))
+                0.5
+                * (
+                    dydP * price.gradient(price.vars, order=2)
+                    + d2ydP2 * np.matmul(price.dual[:, None], price.dual[None, :])
+                ),
             )
         else:
             return x
 
-    def rate(
+    def fwd_from_repo(
         self,
-        curves: Optional[Union[Curve, str, list]] = None,
-        solver: Optional[Solver] = None,
-        fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None,
-        metric="dirty_price",
+        price: Union[float, Dual, Dual2],
+        settlement: datetime,
+        forward_settlement: datetime,
+        repo_rate: Union[float, Dual, Dual2],
+        convention: Optional[str] = None,
+        dirty: bool = False,
     ):
         """
-        Return various pricing metrics of the security calculated from
-        :class:`~rateslib.curves.Curve` s.
+        Return a forward price implied by a given repo rate.
 
         Parameters
         ----------
-        curves : Curve, str or list of such
-            A single :class:`Curve` or id or a list of such. A list defines the
-            following curves in the order:
-
-              - Forecasting :class:`Curve` for ``leg1``.
-              - Discounting :class:`Curve` for ``leg1``.
-        solver : Solver, optional
-            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
-            instruments.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            ``FXRates`` or ``FXForwards`` object, converts from local currency
-            into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
-        metric : str in {"dirty_price", "clean_price", "ytm"}, optional
-            Metric returned by the method.
+        price : float, Dual, or Dual2
+            The initial price of the security at ``settlement``.
+        settlement : datetime
+            The settlement date of the bond
+        forward_settlement : datetime
+            The forward date for which to calculate the forward price.
+        repo_rate : float, Dual or Dual2
+            The rate which is used to calculate values.
+        convention : str, optional
+            The day count convention applied to the rate. If not given uses default
+            values.
+        dirty : bool, optional
+            Whether the input and output price are specified including accrued interest.
 
         Returns
         -------
-        float, Dual, Dual2
+        float, Dual or Dual2
+
+        Notes
+        -----
+        Any intermediate (non ex-dividend) cashflows between ``settlement`` and
+        ``forward_settlement`` will also be assumed to accrue at ``repo_rate``.
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        settlement = add_tenor(
-            curves[1].node_dates[0], f"{self.settle}B", None, self.leg1.schedule.calendar
+        convention = defaults.convention if convention is None else convention
+        dcf_ = dcf(settlement, forward_settlement, convention)
+        if not dirty:
+            d_price = price + self.accrued(settlement)
+        else:
+            d_price = price
+        if self.leg1.amortization != 0:
+            raise NotImplementedError(  # pragma: no cover
+                "method for forward price not available with amortization"
+            )
+        total_rtn = d_price * (1 + repo_rate * dcf_ / 100) * -self.leg1.notional / 100
+
+        # now systematically deduct coupons paid between settle and forward settle
+        settlement_idx = index_left(
+            self.leg1.schedule.aschedule,
+            self.leg1.schedule.n_periods + 1,
+            settlement,
+        )
+        fwd_settlement_idx = index_left(
+            self.leg1.schedule.aschedule,
+            self.leg1.schedule.n_periods + 1,
+            forward_settlement,
         )
-        npv = self.npv(curves, solver, fx, base)
 
-        # scale price to par 100 and make a fwd adjustment according to curve
-        dirty_price = npv * 100 / (-self.leg1.notional * curves[1][settlement])
+        # do not accrue a coupon not received
+        settlement_idx += 1 if self.ex_div(settlement) else 0
+        # deduct final coupon if received within period
+        fwd_settlement_idx += 1 if self.ex_div(forward_settlement) else 0
+
+        for p_idx in range(settlement_idx, fwd_settlement_idx):
+            # deduct accrued coupon from dirty price
+            dcf_ = dcf(self.leg1.periods[p_idx].payment, forward_settlement, convention)
+            accrued_coup = self.leg1.periods[p_idx].cashflow * (
+                1 + dcf_ * repo_rate / 100
+            )
+            total_rtn -= accrued_coup
 
-        if metric == "dirty_price":
-            return dirty_price
-        elif metric == "clean_price":
-            return dirty_price - self.accrued(settlement)
-        elif metric == "ytm":
-            return self.ytm(dirty_price, settlement, True)
-        raise ValueError("`metric` must be in {'dirty_price', 'clean_price', 'ytm'}.")
+        forward_price = total_rtn / -self.leg1.notional * 100
+        if dirty:
+            return forward_price
+        else:
+            return forward_price - self.accrued(forward_settlement)
 
-    def cashflows(
+    def repo_from_fwd(
         self,
-        curves: Optional[Union[Curve, str, list]] = None,
-        solver: Optional[Solver] = None,
-        fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None,
-        settlement: datetime = None
+        price: Union[float, Dual, Dual2],
+        settlement: datetime,
+        forward_settlement: datetime,
+        forward_price: Union[float, Dual, Dual2],
+        convention: Optional[str] = None,
+        dirty: bool = False,
     ):
         """
-        Return the properties of the security used in calculating cashflows.
+        Return an implied repo rate from a forward price.
 
         Parameters
         ----------
-        curves : Curve, str or list of such
-            A single :class:`Curve` or id or a list of such. A list defines the
-            following curves in the order:
-
-              - Forecasting :class:`Curve` for ``leg1``.
-              - Discounting :class:`Curve` for ``leg1``.
-        solver : Solver, optional
-            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
-            instruments.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            ``FXRates`` or ``FXForwards`` object, converts from local currency
-            into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx_rate`` is an ``FXRates`` or ``FXForwards`` object.
-        settlement : datetime, optional
-            The settlement date of the security. If *None* adds the regular ``settle``
-            time to the initial node date of the given discount ``curves``.
+        price : float, Dual, or Dual2
+            The initial price of the security at ``settlement``.
+        settlement : datetime
+            The settlement date of the bond
+        forward_settlement : datetime
+            The forward date for which to calculate the forward price.
+        forward_price : float, Dual or Dual2
+            The forward price which iplies the repo rate
+        convention : str, optional
+            The day count convention applied to the rate. If not given uses default
+            values.
+        dirty : bool, optional
+            Whether the input and output price are specified including accrued interest.
 
         Returns
         -------
-        DataFrame
+        float, Dual or Dual2
+
+        Notes
+        -----
+        Any intermediate (non ex-dividend) cashflows between ``settlement`` and
+        ``forward_settlement`` will also be assumed to accrue at ``repo_rate``.
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        if settlement is None:
-            settlement = add_tenor(
-                curves[1].node_dates[0], f"{self.settle}B", None, self.leg1.schedule.calendar
-            )
-        cashflows = self.leg1.cashflows(curves[0], curves[1], fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
+        convention = defaults.convention if convention is None else convention
+        # forward price from repo is linear in repo_rate so reverse calculate with AD
+        if not dirty:
+            p_t = forward_price + self.accrued(forward_settlement)
+            p_0 = price + self.accrued(settlement)
+        else:
+            p_t, p_0 = forward_price, price
+
+        dcf_ = dcf(settlement, forward_settlement, convention)
+        numerator = p_t - p_0
+        denominator = p_0 * dcf_
+
+        # now systematically deduct coupons paid between settle and forward settle
+        settlement_idx = index_left(
+            self.leg1.schedule.aschedule,
+            self.leg1.schedule.n_periods + 1,
+            settlement,
+        )
+        fwd_settlement_idx = index_left(
+            self.leg1.schedule.aschedule,
+            self.leg1.schedule.n_periods + 1,
+            forward_settlement,
+        )
+
+        # do not accrue a coupon not received
+        settlement_idx += 1 if self.ex_div(settlement) else 0
+        # deduct final coupon if received within period
+        fwd_settlement_idx += 1 if self.ex_div(forward_settlement) else 0
+
+        for p_idx in range(settlement_idx, fwd_settlement_idx):
+            # deduct accrued coupon from dirty price
+            dcf_ = dcf(self.leg1.periods[p_idx].payment, forward_settlement, convention)
+            numerator += 100 * self.leg1.periods[p_idx].cashflow / -self.leg1.notional
+            denominator -= (
+                100 * dcf_ * self.leg1.periods[p_idx].cashflow / -self.leg1.notional
             )
-            cashflows.loc[current_period, defaults.headers["npv"]] = 0
-            cashflows.loc[current_period, defaults.headers["npv_fx"]] = 0
-        return cashflows
 
-    def npv(
+        return numerator / denominator * 100
+
+    # Digital Methods
+
+    def rate(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-        local: bool = False,
+        metric: str = "clean_price",
+        forward_settlement: Optional[datetime] = None,
     ):
         """
-        Return the NPV of the security by summing cashflow valuations.
+        Return various pricing metrics of the security calculated from
+        :class:`~rateslib.curves.Curve` s.
 
         Parameters
         ----------
         curves : Curve, str or list of such
             A single :class:`Curve` or id or a list of such. A list defines the
             following curves in the order:
 
@@ -1078,134 +1414,68 @@
             The immediate settlement FX rate that will be used to convert values
             into another currency. A given `float` is used directly. If giving a
             ``FXRates`` or ``FXForwards`` object, converts from local currency
             into ``base``.
         base : str, optional
             The base currency to convert cashflows into (3-digit code), set by default.
             Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
-        local : bool, optional
-            If `True` will ignore the ``base`` request and return a dict identifying
-            local currency NPV.
-
-        Returns
-        -------
-        float, Dual, Dual2 or dict of such
-
-        Notes
-        -----
-        The ``settlement`` date of the bond is inferred from the objects ``settle``
-        days parameter and the initial date of the supplied ``curves``.
-        The NPV returned is for immediate settlement.
-
-        If **only one curve** is given this is used as all four curves.
-
-        If **two curves** are given the forecasting curve is used as the forecasting
-        curve on both legs and the discounting curve is used as the discounting
-        curve for both legs.
-        """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        settlement = add_tenor(
-            curves[1].node_dates[0], f"{self.settle}B", None, self.leg1.schedule.calendar
-        )
-        base = self.currency if local else base
-        npv = self.leg1.npv(curves[0], curves[1], fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
-            )
-            npv -= self.leg1.periods[current_period].npv(
-                curves[0], curves[1], fx, base
-            )
-        if local:
-            return {self.currency: npv}
-        else:
-            return npv
-
-    def analytic_delta(
-        self,
-        curve: Optional[Curve] = None,
-        disc_curve: Optional[Curve] = None,
-        fx: Union[float, FXRates, FXForwards] = 1.0,
-        base: Optional[str] = None,
-    ):
-        """
-        Return the analytic delta of the security via summing all periods.
-
-        Parameters
-        ----------
-        curve : Curve
-            The forecasting curve object. Not used unless it is set equal to
-            ``disc_curve``.
-        disc_curve : Curve, optional
-            The discounting curve object used in calculations.
-            Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
-            object, converts from local currency into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
-            :class:`~rateslib.fx.FXForwards` object.
+        metric : str, optional
+            Metric returned by the method. Available options are {"clean_price",
+            "dirty_price", "ytm", "fwd_clean_price", "fwd_dirty_price"}
+        forward_settlement : datetime
+            The forward settlement date, required if the metric is in
+            {"fwd_clean_price", "fwd_dirty_price"}.
 
         Returns
         -------
         float, Dual, Dual2
         """
-        # TODO make this ex-div compliant
-        disc_curve = disc_curve or curve
-        settlement = add_tenor(
-            disc_curve.node_dates[0], f"{self.settle}B", None,
-            self.leg1.schedule.calendar
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
         )
-        a_delta = self.leg1.analytic_delta(curve, disc_curve, fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
+
+        metric = metric.lower()
+        if metric in ["clean_price", "dirty_price", "ytm"]:
+            settlement = add_tenor(
+                curves[1].node_dates[0],
+                f"{self.settle}B",
+                None,
+                self.leg1.schedule.calendar,
             )
-            a_delta -= self.leg1.periods[current_period].analytic_delta(
-                curve, disc_curve, fx, base
+            npv = self._npv_local(
+                curves[0], curves[1], fx, base, settlement, settlement
             )
-        return a_delta
-
-    def forward_price(self, price, settlement, forward_settlement, disc_curve):
-        """
-        Calculate the forward price of the security.
-
-        Parameters
-        ----------
-        price : float, Dual, Dual2
-            The initial price of the security.
-        settlement : datetime
-            The settlement date associated with the ``price``.
-        forward_settlement : datetime
-            The forward settlement date for which to determine the price.
-        disc_curve : Curve
-            The rate which to discount cashflows, usually termed the repo rate.
+            # scale price to par 100 (npv is already projected forward to settlement)
+            dirty_price = npv * 100 / -self.leg1.notional
 
-        Returns
-        -------
-        float, Dual, Dual2
+            if metric == "dirty_price":
+                return dirty_price
+            elif metric == "clean_price":
+                return dirty_price - self.accrued(settlement)
+            elif metric == "ytm":
+                return self.ytm(dirty_price, settlement, True)
 
-        Notes
-        -----
-        This calculation only rolls a bond price forward accroding to the repo rate.
-        It does **not** account for cashflows or ex-dividend periods.
-        """
-        # TODO make this calculation accounting for forward historic coupons
-        multiplier = disc_curve[settlement] / disc_curve[forward_settlement]
-        return price * multiplier
+        elif metric in ["fwd_clean_price", "fwd_dirty_price"]:
+            if forward_settlement is None:
+                raise ValueError(
+                    "`forward_settlement` needed to determine forward price."
+                )
+            npv = self._npv_local(
+                curves[0], curves[1], fx, base, forward_settlement, forward_settlement
+            )
+            dirty_price = npv / -self.leg1.notional * 100
+            if metric == "fwd_dirty_price":
+                return dirty_price
+            elif metric == "fwd_clean_price":
+                return dirty_price - self.accrued(forward_settlement)
 
+        raise ValueError(
+            "`metric` must be in {'dirty_price', 'clean_price', 'ytm', "
+            "'fwd_clean_price', 'fwd_dirty_price'}."
+        )
 
     # def par_spread(self, *args, price, settlement, dirty, **kwargs):
     #     """
     #     The spread to the fixed rate added to value the security at par valued from
     #     the given :class:`~rateslib.curves.Curve` s.
     #
     #     Parameters
@@ -1261,25 +1531,25 @@
 
     Attributes
     ----------
     leg1 : FixedLegExchange
     """
 
     def __init__(
-            self,
-            effective: datetime,
-            termination: Union[datetime, str] = None,
-            frequency: str = None,
-            modifier: Optional[str] = False,
-            calendar: Optional[Union[CustomBusinessDay, str]] = None,
-            payment_lag: Optional[int] = None,
-            notional: Optional[float] = None,
-            currency: Optional[str] = None,
-            convention: Optional[str] = None,
-            settle: int = 1,
+        self,
+        effective: datetime,
+        termination: Union[datetime, str] = None,
+        frequency: str = None,
+        modifier: Optional[str] = False,
+        calendar: Optional[Union[CustomBusinessDay, str]] = None,
+        payment_lag: Optional[int] = None,
+        notional: Optional[float] = None,
+        currency: Optional[str] = None,
+        convention: Optional[str] = None,
+        settle: int = 1,
     ):
         if payment_lag is None:
             payment_lag = defaults.payment_lag_specific[type(self).__name__]
         super().__init__(
             effective=effective,
             termination=termination,
             frequency=frequency,
@@ -1334,22 +1604,29 @@
         metric : str in {"price", "discount_rate", "ytm", "simple_rate"}
             Metric returned by the method.
 
         Returns
         -------
         float, Dual, Dual2
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         settlement = add_tenor(
-            curves[1].node_dates[0], f"{self.settle}B", None,
-            self.leg1.schedule.calendar
+            curves[1].node_dates[0],
+            f"{self.settle}B",
+            None,
+            self.leg1.schedule.calendar,
         )
         # scale price to par 100 and make a fwd adjustment according to curve
-        price = self.npv(curves, solver, fx, base) * 100 / \
-            (-self.leg1.notional * curves[1][settlement])
+        price = (
+            self.npv(curves, solver, fx, base)
+            * 100
+            / (-self.leg1.notional * curves[1][settlement])
+        )
         if metric == "price":
             return price
         elif metric == "discount_rate":
             return self.discount_rate(price, settlement)
         elif metric == "simple_rate":
             return self.simple_rate(price, settlement)
         elif metric == "ytm":
@@ -1381,20 +1658,21 @@
         Returns
         -------
         float, Dual, Dual2
         """
         dcf = (1 - self._accrued_frac(settlement)[0]) * self.leg1.periods[0].dcf
         return 100 - discount_rate * dcf
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-class FloatRateBond(Sensitivities, BaseMixin):
+class FloatRateBond(Sensitivities, BondMixin, BaseMixin):
     """
     Create a floating rate bond security.
 
     Parameters
     ----------
     effective : datetime
         The adjusted or unadjusted effective date.
@@ -1470,14 +1748,15 @@
         `ex_div` period of at maximum 1.
 
     Attributes
     ----------
     ex_div_days : int
     leg1 : FloatLegExchange
     """
+
     _float_spread_mixin = True
 
     def __init__(
         self,
         effective: datetime,
         termination: Union[datetime, str] = None,
         frequency: str = None,
@@ -1538,83 +1817,64 @@
             if self.ex_div_days > self.leg1.method_param:
                 raise ValueError(
                     "For RFR FRNs `ex_div` must be less than or equal to `method_param`"
                     " otherwise negative accrued payments cannot be explicitly "
                     "determined due to unknown fixings."
                 )
 
-    def ex_div(self, settlement: datetime):
-        """
-        Return a boolean whether the security is ex-div on the settlement.
-
-        Parameters
-        ----------
-        settlement : datetime
-             The settlement date to test.
-
-        Returns
-        -------
-        bool
-        """
-        prev_a_idx = index_left(
-            self.leg1.schedule.aschedule,
-            len(self.leg1.schedule.aschedule),
-            settlement,
-        )
-        ex_div_date = add_tenor(
-            self.leg1.schedule.aschedule[prev_a_idx+1],
-            f"{-self.ex_div_days}B",
-            None,  # modifier not required for business day tenor
-            self.leg1.schedule.calendar,
-        )
-        return True if settlement >= ex_div_date else False
-
-    def _accrued_frac(self, settlement: datetime):
-        """
-        Return the accrual fraction of period between last coupon and settlement and
-        coupon period left index
-        """
-        acc_idx = index_left(
-            self.leg1.schedule.aschedule,
-            len(self.leg1.schedule.aschedule),
-            settlement,
-        )
-        return (
-            (settlement - self.leg1.schedule.aschedule[acc_idx]) /
-            (self.leg1.schedule.aschedule[acc_idx+1] -
-             self.leg1.schedule.aschedule[acc_idx])
-        ), acc_idx
-
-    def accrued(self, settlement: datetime):
+    def accrued(
+        self,
+        settlement: datetime,
+        forecast: bool = False,
+        curve: Curve = None,
+    ):
         """
         Calculate the accrued amount per nominal par value of 100.
 
         Parameters
         ----------
         settlement : datetime
             The settlement date which to measure accrued interest against.
+        forecast : bool, optional
+            Whether to use a curve to forecast future fixings.
+        curve : Curve, optional
+            If ``forecast`` is *True* and fixings are future based then must provide
+            a forecast curve.
 
         Notes
         -----
+        The settlement of an FRN will always be a definite amount. The
+        ``fixing_method``, ``method_param`` and ``ex_div`` will contain a
+        valid combination of parameters such that when payments need to be
+        cleared these definitive amounts can be calculated
+        via previously published fixings.
+
         If the coupon is IBOR based then the accrued
         fractionally apportions the coupon payment based on calendar days, including
-        negative accrued during ex div periods.
+        negative accrued during ex div periods. This rarely poses a problem since
+        IBOR is fixed well in advance of settlement.
 
         .. math::
 
            \\text{Accrued} = \\text{Coupon} \\times \\frac{\\text{Settle - Last Coupon}}{\\text{Next Coupon - Last Coupon}}
 
-        If the coupon is based in RFR rates then the accrued is calculated upto the
-        settlement date by compounding known fixing rates. Negative accrued is
-        extrapolated by evaluating the number of remaining days in the ex div period
-        and comparing them to the number of days in the existing accrual period.
-        Negative accrued **may need to be forecast** if fixings within the ex-div
-        period are unpublished (i.e. when a combination of ``settle``, ``ex_div`` days
-        and ``method_param`` are sufficient). If a forecast is required the last known
-        given fixing is repeated.
+        With RFR rates, however, and since ``settlement`` typically occurs
+        in the future, e.g. T+2, it may be
+        possible, particularly if the bond is *ex-div* that some fixings are not known
+        today, but they will be known by ``settlement``. This is also true if we
+        wish to calculate the forward dirty price of a bond and need to forecast
+        the accrued amount (and also for a forecast IBOR period).
+
+        Thus, there are two options:
+
+        - In the analogue mode where very few fixings might be missing, and we require
+          these values to calculate negative accrued in an ex-div period we do not
+          require a ``curve`` but repeat the last historic fixing.
+        - In the digital mode where the ``settlement`` may be well in the future we
+          use a ``curve`` to forecast rates,
 
         Examples
         --------
         An RFR based FRN where the fixings are known up to the end of period.
 
         .. ipython:: python
 
@@ -1649,31 +1909,37 @@
                fixings=fixings,
                fixing_method="ibor",
                method_param=2,
            )
            frn.accrued(dt(2000, 3, 27))
            frn.accrued(dt(2000, 6, 4))
         """
-        # TODO validate against effective and termination?
         if self.leg1.fixing_method == "ibor":
             frac, acc_idx = self._accrued_frac(settlement)
             if self.ex_div(settlement):
-                frac = (frac - 1)  # accrued is negative in ex-div period
-            rate = self.leg1.periods[acc_idx].rate(
-                Curve({
-                    self.leg1.periods[acc_idx].start: 1.0,
-                    self.leg1.periods[acc_idx].end: 1.0
-                })
-            )
-            cashflow = -self.leg1.periods[acc_idx].notional * \
-                       self.leg1.periods[acc_idx].dcf * \
-                       rate / 100
-            return (
-                frac * cashflow / -self.leg1.notional * 100
+                frac = frac - 1  # accrued is negative in ex-div period
+
+            if forecast:
+                curve = curve
+            else:
+                curve = Curve(
+                    {  # create a dummy curve. rate() will return the fixing
+                        self.leg1.periods[acc_idx].start: 1.0,
+                        self.leg1.periods[acc_idx].end: 1.0,
+                    }
+                )
+            rate = self.leg1.periods[acc_idx].rate(curve)
+
+            cashflow = (
+                -self.leg1.periods[acc_idx].notional
+                * self.leg1.periods[acc_idx].dcf
+                * rate
+                / 100
             )
+            return frac * cashflow / -self.leg1.notional * 100
         else:  # is "rfr"
             acc_idx = index_left(
                 self.leg1.schedule.aschedule,
                 len(self.leg1.schedule.aschedule),
                 settlement,
             )
             p = FloatPeriod(
@@ -1686,186 +1952,893 @@
                 convention=self.leg1.convention,
                 termination=self.leg1.schedule.aschedule[acc_idx + 1],
                 stub=True,
                 float_spread=self.float_spread,
                 fixing_method=self.leg1.fixing_method,
                 fixings=self.leg1.fixings[acc_idx],
                 method_param=self.leg1.method_param,
-                spread_compound_method=self.leg1.spread_compound_method
+                spread_compound_method=self.leg1.spread_compound_method,
             )
 
-            # For negative accrued in ex-div we need to forecast unpublished rates.
-            # Build a curve which replicates the last known fixing value from fixings
-            try:
-                last_fixing = p.fixings[-1]
-            except TypeError:
-                # then rfr fixing cannot be fetched from attribute
-                if acc_idx == 0 and p.start == self.leg1.schedule.aschedule[0]:
-                    # bond settles on issue date of bond, fixing may not be available.
-                    accrued_to_settle = 0.
-                else:
-                    raise TypeError(
-                        "`fixings` are not available for RFR float period. Must be a "
-                        f"Series or list, {p.fixings} was given."
-                    )
+            if forecast:
+                curve = curve
             else:
-                _crv = LineCurve({
-                    self.leg1.periods[acc_idx].start: last_fixing,
-                    self.leg1.periods[acc_idx].end: last_fixing,
-                })
-                # Otherwise rate to settle is determined fully by known fixings.
-                rate_to_settle = float(p.rate(_crv))
-                accrued_to_settle = 100 * p.dcf * rate_to_settle / 100
+                try:
+                    last_fixing = p.fixings[-1]
+                    # For negative accr in ex-div we need to forecast unpublished rates.
+                    # Build a curve which replicates the last fixing value from fixings.
+                except TypeError:
+                    # then rfr fixing cannot be fetched from attribute
+
+                    # if acc_idx == 0 and p.start == self.leg1.schedule.aschedule[0]:
+                    #     # bond settles on issue date of bond, fixing may not be available.
+                    #     accrued_to_settle = 0.
+
+                    if p.dcf < 1e-10:
+                        # then settlement is same as period.start so no rate necessary
+                        # create a dummy curve
+                        last_fixing = 0.0
+                    else:
+                        raise TypeError(
+                            "`fixings` are not available for RFR float period. Must be a "
+                            f"Series or list, {p.fixings} was given."
+                        )
+                curve = LineCurve(
+                    {
+                        self.leg1.periods[acc_idx].start: last_fixing,
+                        self.leg1.periods[acc_idx].end: last_fixing,
+                    }
+                )
+
+            # Otherwise rate to settle is determined fully by known fixings.
+            if p.dcf < 1e-10:
+                rate_to_settle = 0.0  # there are no fixings in the period.
+            else:
+                rate_to_settle = float(p.rate(curve))
+            accrued_to_settle = 100 * p.dcf * rate_to_settle / 100
 
             if self.ex_div(settlement):
-                rate_to_end = self.leg1.periods[acc_idx].rate(_crv)
-                accrued_to_end = 100 * self.leg1.periods[acc_idx].dcf * rate_to_end / 100
+                rate_to_end = self.leg1.periods[acc_idx].rate(curve)
+                accrued_to_end = (
+                    100 * self.leg1.periods[acc_idx].dcf * rate_to_end / 100
+                )
                 return accrued_to_settle - accrued_to_end
             else:
                 return accrued_to_settle
 
     def rate(
         self,
         curves: Union[Curve, str, list],
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-        settlement=None,
-        metric="dirty_price",
+        metric="clean_price",
+        forward_settlement: Optional[datetime] = None,
     ):
         """
-        TODO
+        Return various pricing metrics of the security calculated from
+        :class:`~rateslib.curves.Curve` s.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+        metric : str, optional
+            Metric returned by the method. Available options are {"clean_price",
+            "dirty_price", "spread", "fwd_clean_price", "fwd_dirty_price"}
+        forward_settlement : datetime
+            The forward settlement date, required if the metric is in
+            {"fwd_clean_price", "fwd_dirty_price"}.
+
+        Returns
+        -------
+        float, Dual, Dual2
+
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        npv = self.npv(curves, solver, fx, base, False, settlement)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
 
-        # scale price to par 100 and make a fwd adjustment according to curve
-        dirty_price = npv * 100 / (-self.leg1.notional * curves[1][settlement])
+        metric = metric.lower()
+        if metric in ["clean_price", "dirty_price", "spread"]:
+            settlement = add_tenor(
+                curves[1].node_dates[0],
+                f"{self.settle}B",
+                None,
+                self.leg1.schedule.calendar,
+            )
+            npv = self._npv_local(
+                curves[0], curves[1], fx, base, settlement, settlement
+            )
+            # scale price to par 100 (npv is already projected forward to settlement)
+            dirty_price = npv * 100 / -self.leg1.notional
 
-        if metric == "dirty_price":
-            return dirty_price
-        elif metric == "clean_price":
-            return dirty_price - self.accrued(settlement)
-        elif metric == "spread":
-            if "rfr" in self.leg1.fixing_method and \
-                    self.leg1.spread_compound_method != "none_simple":
-                # This code replicates BaseLeg._spread for an FRN accounting for ex-div
-                # via FRN.npv().
-
-                _fs = self.float_spread
-                self.float_spread = Dual2(0. if _fs is None else float(_fs), "spread_z")
-
-                fore_curve, disc_curve = curves[0], curves[1]
-
-                fore_ad = fore_curve.ad
-                fore_curve._set_ad_order(2)
-
-                disc_ad = disc_curve.ad
-                disc_curve._set_ad_order(2)
-
-                if isinstance(fx, (FXRates, FXForwards)):
-                    _fx = None if fx is None else fx._ad
-                    fx._set_ad_order(2)
+            if metric == "dirty_price":
+                return dirty_price
+            elif metric == "clean_price":
+                return dirty_price - self.accrued(settlement)
+            elif metric == "spread":
+                if (
+                    "rfr" in self.leg1.fixing_method
+                    and self.leg1.spread_compound_method != "none_simple"
+                ):
+                    # This code replicates BaseLeg._spread for an FRN accounting for ex-div
+                    # via FRN.npv().
+
+                    _fs = self.float_spread
+                    self.float_spread = Dual2(
+                        0.0 if _fs is None else float(_fs), "spread_z"
+                    )
 
-                npv = self.npv(
-                    [fore_curve, disc_curve], None, fx, base, False, settlement
-                )
-                b = npv.gradient("spread_z", order=1)[0]
-                a = 0.5 * npv.gradient("spread_z", order=2)[0][0]
-                c = npv + self.leg1.notional
-
-                _1 = -c / b
-                if abs(a) > 1e-14:
-                    _2 = (-b - (b**2 - 4*a*c)**0.5) / (2*a)
-                    # _2a = (-b + (b**2 - 4*a*c)**0.5) / (2*a)  # alt quadratic soln
-                    _ = _2
+                    fore_curve, disc_curve = curves[0], curves[1]
+
+                    fore_ad = fore_curve.ad
+                    fore_curve._set_ad_order(2)
+
+                    disc_ad = disc_curve.ad
+                    disc_curve._set_ad_order(2)
+
+                    if isinstance(fx, (FXRates, FXForwards)):
+                        _fx = None if fx is None else fx._ad
+                        fx._set_ad_order(2)
+
+                    npv = self.npv([fore_curve, disc_curve], None, fx, base, False)
+                    b = npv.gradient("spread_z", order=1)[0]
+                    a = 0.5 * npv.gradient("spread_z", order=2)[0][0]
+                    c = npv + self.leg1.notional
+
+                    _1 = -c / b
+                    if abs(a) > 1e-14:
+                        _2a = (-b - (b**2 - 4 * a * c) ** 0.5) / (2 * a)
+                        _2b = (-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)  # alt soln
+                        if abs(_1 - _2a) < abs(_1 - _2b):
+                            _ = _2a
+                        else:
+                            _ = _2b  # select quadratic soln
+                    else:  # pragma: no cover
+                        # this is to avoid div by zero err and return an approximation
+                        _ = _1
+                        warnings.warn(
+                            "Divide by zero encountered and the spread is approximated "
+                            "to first order.",
+                            UserWarning,
+                        )
+                    _ += 0.0 if _fs is None else _fs
+
+                    self.float_spread = _fs
+                    fore_curve._set_ad_order(fore_ad)
+                    disc_curve._set_ad_order(disc_ad)
+                    if isinstance(fx, (FXRates, FXForwards)):
+                        fx._set_ad_order(_fx)
+                    return set_order(_, disc_ad)  # use disc_ad: cred spd from disc crv
                 else:
-                    _ = _1
-                _ += 0. if _fs is None else _fs
+                    # NPV calc is efficient and requires no additional ingenuity.
+                    _ = (npv + self.leg1.notional) / self.analytic_delta(
+                        curves[0], curves[1], fx, base
+                    )
+                    _ += self.float_spread
+                    return _
+
+        elif metric in ["fwd_clean_price", "fwd_dirty_price"]:
+            if forward_settlement is None:
+                raise ValueError(
+                    "`forward_settlement` needed to determine forward price."
+                )
+            npv = self._npv_local(
+                curves[0], curves[1], fx, base, forward_settlement, forward_settlement
+            )
+            dirty_price = npv / -self.leg1.notional * 100
+            if metric == "fwd_dirty_price":
+                return dirty_price
+            elif metric == "fwd_clean_price":
+                return dirty_price - self.accrued(forward_settlement, True, curves[0])
 
-                self.float_spread = _fs
-                fore_curve._set_ad_order(fore_ad)
-                disc_curve._set_ad_order(disc_ad)
-                if isinstance(fx, (FXRates, FXForwards)):
-                    fx._set_ad_order(_fx)
-                return set_order(_, disc_ad)  # use disc_ad: cred spread from disc curve
-            else:
-                # NPV calc is efficient and requires no additional ingenuity.
-                _ = (npv + self.leg1.notional) / \
-                    self.analytic_delta(curves[0], curves[1], fx, base)
-                _ += self.float_spread
-                return _
         raise ValueError(
             "`metric` must be in {'dirty_price', 'clean_price', 'spread'}."
         )
 
-    def cashflows(
+
+### Single currency derivatives
+
+
+class BondFuture(Sensitivities):
+    """
+    Create a bond future derivative.
+
+    Parameters
+    ----------
+    coupon: float
+        The nominal coupon rate set on the contract specifications.
+    delivery: datetime or 2-tuple of datetimes
+        The delivery window first and last delivery day, or a single delivery day.
+    basket: tuple of FixedRateBond
+        The bonds that are available as deliverables.
+    last_trading: int, optional
+        The number of business days before the final delivery day when trading
+        will cease.
+    nominal: float, optional
+        The nominal amount of the contract.
+    calendar: str, optional
+        The calendar to define delivery days within the delivery window.
+    """
+
+    def __init__(
         self,
-        curves: Union[Curve, str, list],
+        coupon: float,
+        delivery: Union[datetime, tuple[datetime, datetime]],
+        basket: tuple[FixedRateBond],
+        # last_trading: Optional[int] = None,
+        nominal: Optional[float] = None,
+        contracts: Optional[int] = None,
+        calendar: Optional[str] = None,
+        currency: Optional[str] = None,
+    ):
+        self.currency = defaults.base_currency if currency is None else currency.lower()
+        self.coupon = coupon
+        if isinstance(delivery, datetime):
+            self.delivery = (delivery, delivery)
+        else:
+            self.delivery = tuple(delivery)
+        self.basket = tuple(basket)
+        self.calendar = get_calendar(calendar)
+        # self.last_trading = delivery[1] if last_trading is None else
+        self.nominal = defaults.notional if nominal is None else nominal
+        self.contracts = 1 if contracts is None else contracts
+        self._cfs = None
+
+    @property
+    def notional(self):
+        """
+        Return the notional as number of contracts multiplied by contract nominal.
+
+        Returns
+        -------
+        float
+        """
+        return self.nominal * self.contracts * -1  # long positions is negative notn
+
+    @property
+    def cfs(self):
+        """
+        Return the conversion factors for each bond in the ordered ``basket``.
+
+        Returns
+        -------
+        tuple
+
+        Notes
+        -----
+        This method uses the traditional calculation of obtaining a clean price
+        for each bond on the **first delivery date** assuming the **yield-to-maturity**
+        is set as the nominal coupon of the bond future, and scaled to 100.
+
+        .. warning::
+
+           Some exchanges, such as EUREX, specify their own conversion factors' formula
+           which differs slightly in the definition of yield-to-maturity than the
+           implementation offered by *rateslib*. This results in small differences and
+           is *potentially* explained in the way dates, holidays and DCFs are handled
+           by each calculator.
+
+        For ICE-LIFFE and gilt futures the methods between the exchange and *rateslib*
+        align which results in accurate values. Official values can be validated
+        against the document
+        :download:`ICE-LIFFE Jun23 Long Gilt<_static/long_gilt_initial_jun23.pdf>`.
+
+        For an equivalent comparison with values which do not exactly align see
+        :download:`EUREX Jun23 Bond Futures<_static/eurex_bond_conversion_factors.csv>`.
+
+        Examples
+        --------
+
+        .. ipython:: python
+
+           kws = dict(
+               stub="ShortFront",
+               frequency="S",
+               calendar="ldn",
+               currency="gbp",
+               convention="ActActICMA",
+               ex_div=7,
+               settle=1,
+           )
+           bonds = [
+               FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+               FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+               FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+               FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+           ]
+           future = BondFuture(
+               delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
+           )
+           future.cfs
+
+        """
+        if self._cfs is None:
+            self._cfs = self._conversion_factors()
+        return self._cfs
+
+    def _conversion_factors(self):
+        return tuple(
+            bond.price(self.coupon, self.delivery[0]) / 100 for bond in self.basket
+        )
+
+    def dlv(
+        self,
+        future_price: Union[float, Dual, Dual2],
+        prices: list[float, Dual, Dual2],
+        repo_rate: Union[float, Dual, Dual2, list, tuple],
+        settlement: datetime,
+        delivery: Optional[datetime] = None,
+        convention: Optional[str] = None,
+        dirty: bool = False,
+    ):
+        """
+        Return an aggregated DataFrame of metrics similar to the Bloomberg DLV function.
+
+        Parameters
+        ----------
+        future_price: float, Dual, Dual2
+            The price of the future.
+        prices: sequence of float, Dual, Dual2
+            The prices of the bonds in the deliverable basket (ordered).
+        repo_rate: float, Dual, Dual2 or list/tuple of such
+            The repo rates of the bonds to delivery.
+        settlement: datetime
+            The settlement date of the bonds, required only if ``dirty`` is *True*.
+        delivery: datetime, optional
+            The date of the futures delivery. If not given uses the final delivery
+            day.
+        convention: str, optional
+            The day count convention applied to the repo rates.
+        dirty: bool
+            Whether the bond prices are given including accrued interest.
+
+        Returns
+        -------
+        DataFrame
+
+        Examples
+        --------
+        This example replicates the Bloomberg screen print in the publication
+        *The Futures Bond Basis: Second Edition (p77)* by Moorad Choudhry. To replicate
+        that publication exactly no calendar has been provided. A more modern
+        Bloomberg would probably consider the London business day calendar and
+        this would affect the metrics of the third bond to a small degree (i.e.
+        set `calendar="ldn"`)
+
+        .. ipython:: python
+
+           kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
+           bonds = [
+               FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+               FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+               FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+               FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+           ]
+           future = BondFuture(
+               delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
+           )
+           future.dlv(
+               future_price=112.98,
+               prices=[102.732, 131.461, 107.877, 134.455],
+               repo_rate=6.24,
+               settlement=dt(2000, 3, 16),
+               convention="Act365f",
+           )
+        """
+        if not isinstance(repo_rate, (tuple, list)):
+            r_ = (repo_rate,) * len(self.basket)
+        else:
+            r_ = tuple(repo_rate)
+
+        df = DataFrame(
+            columns=[
+                "Bond",
+                "Price",
+                "YTM",
+                "C.Factor",
+                "Gross Basis",
+                "Implied Repo",
+                "Actual Repo",
+                "Net Basis",
+            ],
+            index=range(len(self.basket)),
+        )
+        df["Price"] = prices
+        df["YTM"] = [
+            bond.ytm(prices[i], settlement, dirty=dirty)
+            for i, bond in enumerate(self.basket)
+        ]
+        df["C.Factor"] = self.cfs
+        df["Gross Basis"] = self.gross_basis(
+            future_price, prices, settlement, dirty=dirty
+        )
+        df["Implied Repo"] = self.implied_repo(
+            future_price, prices, settlement, delivery, convention, dirty=dirty
+        )
+        df["Actual Repo"] = r_
+        df["Net Basis"] = self.net_basis(
+            future_price, prices, r_, settlement, delivery, convention, dirty=dirty
+        )
+        df["Bond"] = [
+            f"{bond.fixed_rate:,.3f}% "
+            f"{bond.leg1.schedule.termination.strftime('%d-%m-%Y')}"
+            for bond in self.basket
+        ]
+        return df
+
+    def gross_basis(
+        self,
+        future_price: Union[float, Dual, Dual2],
+        prices: list[float, Dual, Dual2],
+        settlement: datetime = None,
+        dirty: bool = False,
+    ):
+        """
+        Calculate the implied repo of each bond in the basket using the proceeds
+        method.
+
+        Parameters
+        ----------
+        future_price: float, Dual, Dual2
+            The price of the future.
+        prices: sequence of float, Dual, Dual2
+            The prices of the bonds in the deliverable basket (ordered).
+        settlement: datetime
+            The settlement date of the bonds, required only if ``dirty`` is *True*.
+        dirty: bool
+            Whether the bond prices are given including accrued interest.
+
+        Returns
+        -------
+        tuple
+
+        Examples
+        --------
+
+        .. ipython:: python
+
+           future.gross_basis(112.98, [102.732, 131.461, 107.877, 134.455])
+        """
+        if dirty:
+            prices_ = tuple(
+                prices[i] - bond.accrued(settlement)
+                for i, bond in enumerate(self.basket)
+            )
+        else:
+            prices_ = prices
+        return tuple(
+            prices_[i] - self.cfs[i] * future_price for i in range(len(self.basket))
+        )
+
+    def net_basis(
+        self,
+        future_price: Union[float, Dual, Dual2],
+        prices: list[float, Dual, Dual2],
+        repo_rate: Union[float, Dual, Dual2, list, tuple],
+        settlement: datetime,
+        delivery: Optional[datetime] = None,
+        convention: Optional[str] = None,
+        dirty: bool = False,
+    ):
+        """
+        Calculate the implied repo of each bond in the basket using the proceeds
+        method.
+
+        Parameters
+        ----------
+        future_price: float, Dual, Dual2
+            The price of the future.
+        prices: sequence of float, Dual, Dual2
+            The prices of the bonds in the deliverable basket (ordered).
+        repo_rate: float, Dual, Dual2 or list/tuple of such
+            The repo rates of the bonds to delivery.
+        settlement: datetime
+            The settlement date of the bonds, required only if ``dirty`` is *True*.
+        delivery: datetime, optional
+            The date of the futures delivery. If not given uses the final delivery
+            day.
+        convention: str, optional
+            The day count convention applied to the repo rates.
+        dirty: bool
+            Whether the bond prices are given including accrued interest.
+
+        Returns
+        -------
+        tuple
+
+        Examples
+        --------
+
+        .. ipython:: python
+
+           future.net_basis(
+               future_price=112.98,
+               prices=[102.732, 131.461, 107.877, 134.455],
+               repo_rate=6.24,
+               settlement=dt(2000, 3, 16),
+               delivery=dt(2000, 6, 30),
+               convention="Act365f"
+           )
+        """
+        if delivery is None:
+            f_settlement = self.delivery[1]
+        else:
+            f_settlement = delivery
+
+        if not isinstance(repo_rate, (list, tuple)):
+            r_ = (repo_rate,) * len(self.basket)
+        else:
+            r_ = repo_rate
+
+        net_basis_ = tuple(
+            bond.fwd_from_repo(
+                prices[i], settlement, f_settlement, r_[i], convention, dirty=dirty
+            )
+            - self.cfs[i] * future_price
+            for i, bond in enumerate(self.basket)
+        )
+        return net_basis_
+
+    def implied_repo(
+        self,
+        future_price: Union[float, Dual, Dual2],
+        prices: list[float, Dual, Dual2],
+        settlement: datetime,
+        delivery: Optional[datetime] = None,
+        convention: Optional[str] = None,
+        dirty: bool = False,
+    ):
+        """
+        Calculate the implied repo of each bond in the basket using the proceeds
+        method.
+
+        Parameters
+        ----------
+        future_price: float, Dual, Dual2
+            The price of the future.
+        prices: sequence of float, Dual, Dual2
+            The prices of the bonds in the deliverable basket (ordered).
+        settlement: datetime
+            The settlement date of the bonds.
+        delivery: datetime, optional
+            The date of the futures delivery. If not given uses the final delivery
+            day.
+        convention: str, optional
+            The day count convention used in the rate.
+        dirty: bool
+            Whether the bond prices are given including accrued interest.
+
+        Returns
+        -------
+        tuple
+
+        Examples
+        --------
+
+        .. ipython:: python
+
+           future.implied_repo(
+               112.98, [102.732, 131.461, 107.877, 134.455], dt(2000, 3, 16)
+           )
+        """
+        if delivery is None:
+            f_settlement = self.delivery[1]
+        else:
+            f_settlement = delivery
+
+        implied_repos = tuple()
+        for i, bond in enumerate(self.basket):
+            invoice_price = future_price * self.cfs[i]
+            implied_repos += (
+                bond.repo_from_fwd(
+                    price=prices[i],
+                    settlement=settlement,
+                    forward_settlement=f_settlement,
+                    forward_price=invoice_price,
+                    convention=convention,
+                    dirty=dirty,
+                ),
+            )
+        return implied_repos
+
+    def ytm(
+        self,
+        future_price: Union[float, Dual, Dual2],
+        delivery: Optional[datetime] = None,
+    ):
+        """
+        Calculate the yield-to-maturity of the bond future.
+
+        Parameters
+        ----------
+        future_price : float, Dual, Dual2
+            The price of the future.
+        delivery : datetime, optional
+            The future delivery day on which to calculate the yield. If not given aligns
+            with the last delivery day specified on the future.
+
+        Returns
+        -------
+        tuple
+
+        Examples
+        --------
+
+        .. ipython:: python
+
+           future.ytm(112.98)
+        """
+        if delivery is None:
+            settlement = self.delivery[1]
+        else:
+            settlement = delivery
+        adjusted_prices = [future_price * cf for cf in self.cfs]
+        yields = tuple(
+            bond.ytm(adjusted_prices[i], settlement)
+            for i, bond in enumerate(self.basket)
+        )
+        return yields
+
+    def duration(
+        self,
+        future_price: float,
+        metric: str = "risk",
+        delivery: Optional[datetime] = None,
+    ):
+        """
+        Return the (negated) derivative of ``price`` w.r.t. ``ytm``.
+
+        Parameters
+        ----------
+        future_price : float
+            The price of the future.
+        metric : str
+            The specific duration calculation to return. See notes.
+        delivery : datetime, optional
+            The delivery date of the contract.
+
+        Returns
+        -------
+        float
+
+        See Also
+        --------
+        FixedRateBond.duration: Calculation the risk of a FixedRateBond.
+
+        Example
+        -------
+        .. ipython:: python
+
+           risk = future.duration(112.98)
+           risk
+
+        The difference in yield is shown to be 1bp for the CTD (index: 0)
+        when the futures price is adjusted by the risk amount.
+
+        .. ipython:: python
+
+           future.ytm(112.98)
+           future.ytm(112.98 + risk[0] / 100)
+        """
+        if delivery is None:
+            f_settlement = self.delivery[1]
+        else:
+            f_settlement = delivery
+
+        _ = ()
+        for i, bond in enumerate(self.basket):
+            invoice_price = future_price * self.cfs[i]
+            ytm = bond.ytm(invoice_price, f_settlement)
+            if metric == "risk":
+                _ += (bond.duration(ytm, f_settlement, "risk") / self.cfs[i],)
+            else:
+                _ += (bond.duration(ytm, f_settlement, metric),)
+        return _
+
+    def convexity(
+        self,
+        future_price: float,
+        delivery: Optional[datetime] = None,
+    ):
+        """
+        Return the second derivative of ``price`` w.r.t. ``ytm``.
+
+        Parameters
+        ----------
+        future_price : float
+            The price of the future.
+        delivery : datetime, optional
+            The delivery date of the contract. If not given uses the last delivery day
+            in the delivery window.
+
+        Returns
+        -------
+        float
+
+        See Also
+        --------
+        FixedRateBond.convexity: Calculate the convexity of a FixedRateBond.
+
+        Example
+        -------
+        .. ipython:: python
+
+           risk = future.duration(112.98)
+           convx = future.convexity(112.98)
+           convx
+
+        Observe the change in risk duration when the prices is increased by 1bp.
+
+        .. ipython:: python
+
+           future.duration(112.98)
+           future.duration(112.98 + risk[0] / 100)
+        """
+        if delivery is None:
+            f_settlement = self.delivery[1]
+        else:
+            f_settlement = delivery
+
+        _ = ()
+        for i, bond in enumerate(self.basket):
+            invoice_price = future_price * self.cfs[i]
+            ytm = bond.ytm(invoice_price, f_settlement)
+            _ += (bond.convexity(ytm, f_settlement) / self.cfs[i],)
+        return _
+
+    def ctd_index(
+        self,
+        future_price: float,
+        prices: Union[list, tuple],
+        settlement: datetime,
+        delivery: Optional[datetime] = None,
+        dirty: bool = False,
+    ):
+        """
+        Determine the index of the CTD in the basket from implied repo rate.
+
+        Parameters
+        ----------
+        future_price : float
+            The price of the future.
+        prices : list or tuple of float, Dual, Dual2, optional
+            The prices of the bonds to determine the CTD. Not used is ``ctd_index``
+            is given.
+        settlement : datetime
+            The settlement date of the bonds' ``prices``. Only required if ``prices``
+            are given.
+        delivery : datetime, optional
+            The delivery date of the contract.
+        dirty : bool
+            Whether the ``prices`` given include accrued interest or not.
+
+        Returns
+        -------
+        int
+        """
+        implied_repo = self.implied_repo(
+            future_price, prices, settlement, delivery, "Act365F", dirty
+        )
+        ctd_index_ = implied_repo.index(max(implied_repo))
+        return ctd_index_
+
+    # Digital Methods
+
+    def rate(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-        settlement: datetime = None,
+        metric: str = "future_price",
+        delivery: Optional[datetime] = None,
     ):
         """
-        TODO
+        Return various pricing metrics of the security calculated from
+        :class:`~rateslib.curves.Curve` s.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+        metric : str in {"future_price", "ytm"}, optional
+            Metric returned by the method.
+        delivery: datetime, optional
+            The date of the futures delivery. If not given uses the final delivery
+            day.
+
+        Returns
+        -------
+        float, Dual, Dual2
+
+        Notes
+        -----
+        This method determines the *'futures_price'* and *'ytm'*  by assuming a net
+        basis of zero and pricing from the cheapest to delivery (CTD).
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        if settlement is None:
-            settlement = curves[1].node_dates[0]
-        cashflows = self.leg1.cashflows(curves[0], curves[1], fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
+        metric = metric.lower()
+        if metric not in ["future_price", "ytm"]:
+            raise ValueError("`metric` must be in {'future_price', 'ytm'}.")
+
+        if delivery is None:
+            f_settlement = self.delivery[1]
+        else:
+            f_settlement = delivery
+        prices_ = [
+            bond.rate(curves, solver, fx, base, "fwd_clean_price", f_settlement)
+            for bond in self.basket
+        ]
+        future_prices_ = [price / self.cfs[i] for i, price in enumerate(prices_)]
+        future_price = min(future_prices_)
+        ctd_index = future_prices_.index(min(future_prices_))
+
+        if metric == "future_price":
+            return future_price
+        elif metric == "ytm":
+            return self.basket[ctd_index].ytm(
+                future_price * self.cfs[ctd_index], f_settlement
             )
-            cashflows.loc[current_period, defaults.headers["npv"]] = 0
-            cashflows.loc[current_period, defaults.headers["npv_fx"]] = 0
-        return cashflows
 
     def npv(
         self,
-        curves: Union[Curve, str, list],
+        curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
-        settlement: datetime = None,
     ):
         """
-        TODO
+        Determine the monetary value of the bond future position.
+
+        This method is mainly included to calculate risk sensitivities. The
+        monetary value of bond futures is not usually a metric worth considering.
+        The profit or loss of a position based on entry level is a more common
+        metric, however the initial value of the position does not affect the risk.
+
+        See :meth:`BaseDerivative.npv`.
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        if settlement is None:
-            settlement = curves[1].node_dates[0]
-        base = self.currency if local else base
-        npv = self.leg1.npv(curves[0], curves[1], fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
-            )
-            npv -= self.leg1.periods[current_period].npv(
-                curves[0], curves[1], fx, base
-            )
+        future_price = self.rate(curves, solver, fx, base, "future_price")
+        fx, base = _get_fx_and_base(self.currency, fx, base)
+        npv_ = future_price / 100 * -self.notional
         if local:
-            return {self.currency: npv}
+            return {self.currency: npv_}
         else:
-            return npv
-
-    def analytic_delta(self, *args, **kwargs):
-        # TODO make this ex-div compliant
-        return self.leg1.analytic_delta(*args, **kwargs)
-
-
-### Single currency derivatives
+            return npv_ * fx
 
 
 class BaseDerivative(Sensitivities, BaseMixin, metaclass=ABCMeta):
     """
     Abstract base class with common parameters for many ``Derivative`` subclasses.
 
     Parameters
@@ -1973,15 +2946,15 @@
         currency: Optional[str] = None,
         amortization: Optional[float] = None,
         convention: Optional[str] = None,
         leg2_effective: Optional[datetime] = "inherit",
         leg2_termination: Optional[Union[datetime, str]] = "inherit",
         leg2_frequency: Optional[int] = "inherit",
         leg2_stub: Optional[str] = "inherit",
-        leg2_front_stub: Optional[datetime] ="inherit",
+        leg2_front_stub: Optional[datetime] = "inherit",
         leg2_back_stub: Optional[datetime] = "inherit",
         leg2_roll: Optional[Union[str, int]] = "inherit",
         leg2_eom: Optional[bool] = "inherit",
         leg2_modifier: Optional[str] = "inherit",
         leg2_calendar: Optional[Union[CustomBusinessDay, str]] = "inherit",
         leg2_payment_lag: Optional[int] = "inherit",
         leg2_notional: Optional[float] = "inherit_negate",
@@ -1991,17 +2964,29 @@
         curves: Optional[Union[list, str, Curve]] = None,
     ):
         self.curves = curves
         notional = defaults.notional if notional is None else notional
         if payment_lag is None:
             payment_lag = defaults.payment_lag_specific[type(self).__name__]
         for attribute in [
-            "effective", "termination", "frequency", "stub", "front_stub",
-            "back_stub", "roll", "eom", "modifier", "calendar", "payment_lag",
-            "convention", "notional", "amortization", "currency",
+            "effective",
+            "termination",
+            "frequency",
+            "stub",
+            "front_stub",
+            "back_stub",
+            "roll",
+            "eom",
+            "modifier",
+            "calendar",
+            "payment_lag",
+            "convention",
+            "notional",
+            "amortization",
+            "currency",
         ]:
             leg2_val, val = vars()[f"leg2_{attribute}"], vars()[attribute]
             if leg2_val == "inherit":
                 _ = val
             elif leg2_val == "inherit_negate":
                 _ = None if val is None else val * -1
             else:
@@ -2106,19 +3091,23 @@
 
         Examples
         --------
         .. ipython:: python
 
            irs.cashflows([curve], None, fxr)
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
-        return concat([
-            self.leg1.cashflows(curves[0], curves[1], fx, base),
-            self.leg2.cashflows(curves[2], curves[3], fx, base),
-            ], keys=["leg1", "leg2"],
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        return concat(
+            [
+                self.leg1.cashflows(curves[0], curves[1], fx, base),
+                self.leg2.cashflows(curves[2], curves[3], fx, base),
+            ],
+            keys=["leg1", "leg2"],
         )
 
     @abc.abstractmethod
     def npv(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
@@ -2179,20 +3168,24 @@
         --------
         .. ipython:: python
 
            irs.npv(curve)
            irs.npv([curve], None, fxr)
            irs.npv([curve], None, fxr, "gbp")
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         leg1_npv = self.leg1.npv(curves[0], curves[1], fx, base, local)
         leg2_npv = self.leg2.npv(curves[2], curves[3], fx, base, local)
         if local:
-            return {k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
-                    for k in set(leg1_npv) | set(leg2_npv)}
+            return {
+                k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
+                for k in set(leg1_npv) | set(leg2_npv)
+            }
         else:
             return leg1_npv + leg2_npv
 
     @abc.abstractmethod
     def rate(self, *args, **kwargs):
         """
         Return the `rate` or typical `price` for a derivative instrument.
@@ -2262,14 +3255,15 @@
     leg2_fixing_method : str, optional
         The method by which floating rates are determined, set by default. See notes.
     leg2_method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseDerivative`.
     """
+
     _fixed_rate_mixin = True
     _leg2_float_spread_mixin = True
 
     def __init__(
         self,
         *args,
         fixed_rate: Optional[float] = None,
@@ -2423,15 +3417,17 @@
 
         Examples
         --------
         .. ipython:: python
 
            irs.rate([forecasting_curve, discounting_curve])
         """
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         leg2_npv = self.leg2.npv(curves[2], curves[3])
         return self.leg1._spread(-leg2_npv, curves[0], curves[1]) / 100
         # leg1_analytic_delta = self.leg1.analytic_delta(curves[0], curves[1])
         # return leg2_npv / (leg1_analytic_delta * 100)
 
     def cashflows(
         self,
@@ -2450,17 +3446,17 @@
         .. ipython:: python
 
            fxr = FXRates({"gbpusd": 2.0})
            irs.cashflows([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
         return super().cashflows(curves, solver, fx, base)
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def spread(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
@@ -2533,28 +3529,29 @@
         The ``leg2_float_spread`` is determined through NPV differences. If the difference
         is small since the defined spread is already quite close to the solution the
         approximation is much more accurate. This is shown above where the second call
         to ``irs.spread`` is different to the previous call.
         """
         irs_npv = self.npv(curves, solver)
         specified_spd = 0 if self.leg2.float_spread is None else self.leg2.float_spread
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         return self.leg2._spread(-irs_npv, curves[2], curves[3]) + specified_spd
         # leg2_analytic_delta = self.leg2.analytic_delta(curves[2], curves[3])
         # return irs_npv / leg2_analytic_delta + specified_spd
 
 
 class Swap(IRS):
     """
     Alias for :class:`~rateslib.instruments.IRS`.
     """
 
 
 class ZCS(BaseDerivative):
-
     _fixed_rate_mixin = True
     _leg2_float_spread_mixin = True
 
     def __init__(
         self,
         *args,
         fixed_rate: Optional[float] = None,
@@ -2702,15 +3699,17 @@
         float, Dual or Dual2
 
         Notes
         -----
         The arguments ``fx`` and ``base`` are unused by single currency derivatives
         rates calculations.
         """
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         leg2_npv = self.leg2.npv(curves[2], curves[3])
         return self.leg1._spread(-leg2_npv, curves[0], curves[1]) / 100
         # leg1_analytic_delta = self.leg1.analytic_delta(curves[0], curves[1])
         # return leg2_npv / (leg1_analytic_delta * 100)
 
     def cashflows(
         self,
@@ -2781,17 +3780,18 @@
     leg2_fixing_method : str, optional
         The method by which floating rates are determined, set by default. See notes.
     leg2_method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseDerivative`.
     """
+
     _float_spread_mixin = True
     _leg2_float_spread_mixin = True
-    _rate_scalar = 100.
+    _rate_scalar = 100.0
 
     def __init__(
         self,
         *args,
         float_spread: Optional[float] = None,
         spread_compound_method: Optional[str] = None,
         fixings: Optional[Union[float, list, Series]] = None,
@@ -2880,15 +3880,15 @@
            )
            sbs.analytic_delta(forecasting_curve, discounting_curve, leg=1)
         """
         return super().analytic_delta(*args, **kwargs)
 
     def cashflows(
         self,
-        curves: Optional[Union[Curve, str, list]]= None,
+        curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
         """
         Return the properties of all legs used in calculating cashflows.
 
@@ -2900,15 +3900,15 @@
 
            sbs.cashflows([forecasting_curve, discounting_curve, forecasting_curve2])
         """
         return super().cashflows(curves, solver, fx, base)
 
     def npv(
         self,
-        curves: Optional[Union[Curve, str, list]]= None,
+        curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
         """
         Return the NPV of the derivative object by summing legs.
@@ -2921,15 +3921,15 @@
 
            sbs.npv([forecasting_curve, discounting_curve, forecasting_curve2])
         """
         return super().npv(curves, solver, fx, base, local)
 
     def rate(
         self,
-        curves: Optional[Union[Curve, str, list]]= None,
+        curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         leg: int = 1,
     ):
         """
         Return the mid-market float spread on the specified leg of the SBS.
@@ -2957,15 +3957,17 @@
         --------
         .. ipython:: python
 
            sbs.rate([forecasting_curve, discounting_curve, forecasting_curve2], leg=1)
            sbs.rate([forecasting_curve, discounting_curve, forecasting_curve2], leg=2)
         """
         irs_npv = self.npv(curves, solver)
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         if leg == 1:
             leg_obj, args = self.leg1, (curves[0], curves[1])
         else:
             leg_obj, args = self.leg2, (curves[2], curves[3])
 
         specified_spd = 0 if leg_obj.float_spread is None else leg_obj.float_spread
         return leg_obj._spread(-irs_npv, *args) + specified_spd
@@ -3025,14 +4027,15 @@
     Notes
     -----
     FRAs are a legacy derivative whose ``fixing_method`` is set to *"ibor"*.
 
     ``effective`` and ``termination`` are not adjusted prior to initialising
     ``Periods``. Care should be taken to enter these exactly.
     """
+
     _fixed_rate_mixin = True
 
     def __init__(
         self,
         effective: datetime,
         termination: Union[datetime, str],
         frequency: str,
@@ -3158,15 +4161,15 @@
 
     def npv(
         self,
         curves: Optional[Union[str, list, Curve]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-        local: bool = False
+        local: bool = False,
     ):
         """
         Return the NPV of the derivative.
 
         See :meth:`BaseDerivative.npv`.
 
         Examples
@@ -3176,15 +4179,17 @@
            fra.npv([forecasting_curve, discounting_curve])
 
         .. ipython:: python
 
            fxr = FXRates({"gbpusd": 2.0})
            fra.npv([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = self.cashflow(curves[0]) * curves[1][self.payment]
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
@@ -3220,15 +4225,17 @@
 
         Examples
         --------
         .. ipython:: python
 
            fra.rate(forecasting_curve)
         """
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         return self.leg2.rate(curves[0])
 
     def cashflow(self, curve: Union[Curve, LineCurve]):
         """
         Calculate the local currency cashflow on the FRA from current floating rate
         and fixed rate.
 
@@ -3247,15 +4254,15 @@
 
            fra.cashflow(forecasting_curve)
         """
         if self.fixed_rate is None:
             return 0  # set the fixed rate = to floating rate netting to zero
         rate = self.leg2.rate(curve)
         cf = self.notional * self.leg1.dcf * (rate - self.fixed_rate) / 100
-        cf /= (1 + self.leg1.dcf * rate / 100)
+        cf /= 1 + self.leg1.dcf * rate / 100
         return cf
 
     def cashflows(
         self,
         curves: Optional[Union[str, list, Curve]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -3278,15 +4285,17 @@
         Examples
         --------
         .. ipython:: python
 
            fxr = FXRates({"gbpusd": 2.0})
            fra.cashflows([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
-        curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         cf = float(self.cashflow(curves[0]))
         npv_local = self.cashflow(curves[0]) * curves[1][self.payment]
 
         _spread = None if self.fixed_rate is None else -float(self.fixed_rate) * 100
         cfs = self.leg1.cashflows(curves[0], curves[1], fx, base)
         cfs[defaults.headers["type"]] = "FRA"
@@ -3303,14 +4312,15 @@
 ### Multi-currency derivatives
 
 
 class BaseXCS(BaseDerivative):
     """
     Base class with common methods for multi-currency ``Derivatives``.
     """
+
     _is_mtm = False
 
     def __init__(
         self,
         *args,
         **kwargs,
     ):
@@ -3334,15 +4344,16 @@
         if not self._is_mtm:
             self.pair = self.leg1.currency + self.leg2.currency
             # if self.fx_fixing is None this indicates the swap is unfixed and will be set
             # later. If a fixing is given this means the notional is fixed without any
             # further sensitivity, hence the downcast to a float below.
             if isinstance(fx_fixings, FXForwards):
                 self.fx_fixings = float(
-                    fx_fixings.rate(self.pair, self.leg2.periods[0].payment))
+                    fx_fixings.rate(self.pair, self.leg2.periods[0].payment)
+                )
             elif isinstance(fx_fixings, FXRates):
                 self.fx_fixings = float(fx_fixings.rate(self.pair))
             elif isinstance(fx_fixings, (float, Dual, Dual2)):
                 self.fx_fixings = float(fx_fixings)
             else:
                 self._fx_fixings = None
 
@@ -3365,21 +4376,18 @@
                     else:
                         fx_fixing = 1.0
                         if defaults.no_fx_fixings_for_xcs.lower() == "warn":
                             warnings.warn(
                                 "Using 1.0 for FX, no `fx` or `fx_fixing` given and "
                                 "rateslib option `no_fx_fixings_for_xcs` is set to "
                                 "'warn'.",
-                                UserWarning
+                                UserWarning,
                             )
                 else:
-                    fx_fixing = fx.rate(
-                        self.pair,
-                        self.leg2.periods[0].payment
-                    )
+                    fx_fixing = fx.rate(self.pair, self.leg2.periods[0].payment)
                 self._set_leg2_notional(fx_fixing)
         else:
             self._set_leg2_notional(fx)
 
     def _set_leg2_notional(self, fx_arg: Union[float, FXForwards]):
         """
         Update the notional on leg2 (foreign leg) if the initial fx rate is unfixed.
@@ -3406,27 +4414,29 @@
 
     def npv(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[FXForwards] = None,
         base: Optional[str] = None,
-        local: bool = False
+        local: bool = False,
     ):
         """
         Return the NPV of the derivative by summing legs.
 
         .. warning::
 
            If ``fx_fixing`` has not been set for the instrument requires
            ``fx`` as an FXForwards object to dynamically determine this.
 
         See :meth:`BaseDerivative.npv`.
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         base = self.leg1.currency if base is None else base
         self._set_fx_fixings(fx)
         if self._is_mtm:
             self.leg2._do_not_repeat_set_periods = True
 
         if "Fixed" in type(self.leg1).__name__ and self.fixed_rate is None:
             mid_market_rate = self.rate(curves, solver, fx, leg=1)
@@ -3486,60 +4496,62 @@
         the fixed rate used
         for calculation is the implied mid-market rate including the
         current ``float_spread`` parameter.
 
         Examples
         --------
         """
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
 
         if leg == 1:
             tgt_fore_curve, tgt_disc_curve = curves[0], curves[1]
             alt_fore_curve, alt_disc_curve = curves[2], curves[3]
         else:
             tgt_fore_curve, tgt_disc_curve = curves[2], curves[3]
             alt_fore_curve, alt_disc_curve = curves[0], curves[1]
 
         leg2 = 1 if leg == 2 else 2
         tgt_str, alt_str = "" if leg == 1 else "leg2_", "" if leg2 == 1 else "leg2_"
-        tgt_leg, alt_leg = getattr(self, f"leg{leg}"),  getattr(self, f"leg{leg2}")
+        tgt_leg, alt_leg = getattr(self, f"leg{leg}"), getattr(self, f"leg{leg2}")
         base = tgt_leg.currency
 
         _is_float_tgt_leg = "Float" in type(tgt_leg).__name__
         _is_float_alt_leg = "Float" in type(alt_leg).__name__
         if not _is_float_alt_leg and getattr(self, f"{alt_str}fixed_rate") is None:
             raise ValueError(
                 "Cannot solve for a `fixed_rate` or `float_spread` where the "
                 "`fixed_rate` on the non-solvable leg is None."
             )
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+        # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+        # Commercial use of this code, and/or copying and redistribution is prohibited.
+        # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
         if tgt_leg._is_linear:
-
             if not _is_float_tgt_leg and getattr(self, f"{tgt_str}fixed_rate") is None:
                 # set the target fixed leg to a null fixed rate for calculation
-                tgt_leg.fixed_rate = 0.
+                tgt_leg.fixed_rate = 0.0
 
             self._set_fx_fixings(fx)
             if self._is_mtm:
                 self.leg2._do_not_repeat_set_periods = True
 
             tgt_leg_npv = tgt_leg.npv(tgt_fore_curve, tgt_disc_curve, fx, base)
             alt_leg_npv = alt_leg.npv(alt_fore_curve, alt_disc_curve, fx, base)
             fx_a_delta = 1.0 if not tgt_leg._is_mtm else fx
             _ = tgt_leg._spread(
-                -(tgt_leg_npv+alt_leg_npv), tgt_fore_curve, tgt_disc_curve, fx_a_delta
+                -(tgt_leg_npv + alt_leg_npv), tgt_fore_curve, tgt_disc_curve, fx_a_delta
             )
 
-            specified_spd = 0.
-            if _is_float_tgt_leg and \
-                    not(getattr(self, f"{tgt_str}float_spread") is None):
+            specified_spd = 0.0
+            if _is_float_tgt_leg and not (
+                getattr(self, f"{tgt_str}float_spread") is None
+            ):
                 specified_spd = tgt_leg.float_spread
             elif not _is_float_tgt_leg:
                 specified_spd = tgt_leg.fixed_rate * 100
 
             _ += specified_spd
 
             if self._is_mtm:
@@ -3564,15 +4576,17 @@
     def cashflows(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[FXForwards] = None,
         base: Optional[str] = None,
     ):
-        curves, fx = self._get_curves_and_fx_maybe_from_solver(solver, curves, fx)
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
         self._set_fx_fixings(fx)
         if self._is_mtm:
             self.leg2._do_not_repeat_set_periods = True
 
         ret = super().cashflows(curves, solver, fx, base)
         if self._is_mtm:
             self.leg2._do_not_repeat_set_periods = False  # reset the mtm calc
@@ -3641,17 +4655,18 @@
     .. note::
 
        Although non-MTM XCSs have an ``fx_fixing`` argument, which consists of a single,
        initial FX fixing, this is internally mapped to the ``fx_fixings`` attribute,
        which, for MTM XCSs, provides all the FX fixings throughout the swap.
 
     """
+
     _float_spread_mixin = True
     _leg2_float_spread_mixin = True
-    _rate_scalar = 100.
+    _rate_scalar = 100.0
 
     def __init__(
         self,
         *args,
         fx_fixing: Optional[Union[float, FXRates, FXForwards]] = None,
         float_spread: Optional[float] = None,
         fixings: Optional[Union[float, list]] = None,
@@ -3754,36 +4769,38 @@
         """
         npv = self.npv(
             curve_domestic,
             disc_curve_domestic,
             curve_foreign,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
         )
         f_0 = forward_fx(
             disc_curve_domestic.node_dates[0],
             disc_curve_domestic,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
+        )
+        leg1_analytic_delta = f_0 * self.leg1.analytic_delta(
+            curve_domestic, disc_curve_domestic
         )
-        leg1_analytic_delta = f_0 * self.leg1.analytic_delta(curve_domestic, disc_curve_domestic)
         spread = npv / leg1_analytic_delta
         return spread
 
     def _npv2(
         self,
         curve_domestic: Curve,
         disc_curve_domestic: Curve,
         curve_foreign: Curve,
         disc_curve_foreign: Curve,
         fx_rate: Union[float, Dual],
         fx_settlement: Optional[datetime] = None,
-        base: str = None
+        base: str = None,
     ):  # pragma: no cover
         """
         Return the NPV of the non-mtm XCS.
 
         Parameters
         ----------
         curve_domestic : Curve
@@ -3805,15 +4822,15 @@
         """
         base = defaults.fx_swap_base if base is None else base
         f_0 = forward_fx(
             disc_curve_domestic.node_dates[0],
             disc_curve_domestic,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
         )
         fx = forward_fx(
             self.effective,
             disc_curve_domestic,
             disc_curve_foreign,
             f_0,
         )
@@ -3865,28 +4882,30 @@
         DataFrame
         """
         f_0 = forward_fx(
             disc_curve_domestic.node_dates[0],
             disc_curve_domestic,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
         )
         base = defaults.fx_swap_base if base is None else base
         if base == "foreign":
             d_fx, f_fx = f_0, 1.0
         elif base == "domestic":
-            d_fx, f_fx = 1.0,  1.0 / f_0
+            d_fx, f_fx = 1.0, 1.0 / f_0
         else:
             raise ValueError('`base` should be either "domestic" or "foreign".')
         self._set_leg2_notional(f_0)
-        return concat([
-            self.leg1.cashflows(curve_domestic, disc_curve_domestic, d_fx),
-            self.leg2.cashflows(curve_foreign, disc_curve_foreign, f_fx),
-        ], keys=["leg1", "leg2"],
+        return concat(
+            [
+                self.leg1.cashflows(curve_domestic, disc_curve_domestic, d_fx),
+                self.leg2.cashflows(curve_foreign, disc_curve_foreign, f_fx),
+            ],
+            keys=["leg1", "leg2"],
         )
 
 
 class NonMtmFixedFloatXCS(BaseXCS):
     """
     Create a non-mark-to-market cross currency swap (XCS) derivative composing a
     :class:`~rateslib.legs.FixedLegExchange` and a
@@ -3930,14 +4949,15 @@
 
     Notes
     -----
     Non-mtm cross currency swaps create identical yet opposite currency exchanges at
     the effective date and the payment termination date of the swap. There are no
     intermediate currency exchanges.
     """
+
     _fixed_rate_mixin = True
     _leg2_float_spread_mixin = True
 
     def __init__(
         self,
         *args,
         fx_fixing: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -4033,14 +5053,15 @@
 
     Notes
     -----
     Non-mtm cross currency swaps create identical yet opposite currency exchanges at
     the effective date and the payment termination date of the swap. There are no
     intermediate currency exchanges.
     """
+
     _fixed_rate_mixin = True
     _leg2_fixed_rate_mixin = True
 
     def __init__(
         self,
         *args,
         fx_fixing: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -4091,14 +5112,15 @@
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
         )
         self._initialise_fx_fixings(fx_fixing)
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class XCS(BaseXCS):
     """
@@ -4159,18 +5181,19 @@
     Mtm cross currency swaps create notional exchanges on the foreign leg throughout
     the life of the derivative and adjust the notional on which interest is accrued.
 
     .. warning::
 
        ``Amortization`` is not used as an argument by ``XCS``.
     """
+
     _float_spread_mixin = True
     _leg2_float_spread_mixin = True
     _is_mtm = True
-    _rate_scalar = 100.
+    _rate_scalar = 100.0
 
     def __init__(
         self,
         *args,
         fx_fixings: Union[list, float, Dual, Dual2] = [],
         float_spread: Optional[float] = None,
         fixings: Optional[Union[float, list]] = None,
@@ -4249,15 +5272,15 @@
         self,
         curve_domestic: Curve,
         disc_curve_domestic: Curve,
         curve_foreign: Curve,
         disc_curve_foreign: Curve,
         fx_rate: Union[float, Dual],
         fx_settlement: Optional[datetime] = None,
-        base: str = None
+        base: str = None,
     ):  # pragma: no cover
         """
         Return the NPV of the non-mtm XCS.
 
         Parameters
         ----------
         curve_domestic : Curve
@@ -4279,15 +5302,15 @@
         """
         base = defaults.fx_swap_base if base is None else base
         f_0 = forward_fx(
             disc_curve_domestic.node_dates[0],
             disc_curve_domestic,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
         )
         fx = forward_fx(
             self.effective,
             disc_curve_domestic,
             disc_curve_foreign,
             f_0,
         )
@@ -4336,24 +5359,26 @@
         """
         npv = self.npv(
             curve_domestic,
             disc_curve_domestic,
             curve_foreign,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
         )
         f_0 = forward_fx(
             disc_curve_domestic.node_dates[0],
             disc_curve_domestic,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
+        )
+        leg1_analytic_delta = f_0 * self.leg1.analytic_delta(
+            curve_domestic, disc_curve_domestic
         )
-        leg1_analytic_delta = f_0 * self.leg1.analytic_delta(curve_domestic, disc_curve_domestic)
         spread = npv / leg1_analytic_delta
         return spread
 
     def _cashflows2(
         self,
         curve_domestic: Optional[Curve] = None,
         disc_curve_domestic: Optional[Curve] = None,
@@ -4390,49 +5415,51 @@
         DataFrame
         """
         f_0 = forward_fx(
             disc_curve_domestic.node_dates[0],
             disc_curve_domestic,
             disc_curve_foreign,
             fx_rate,
-            fx_settlement
+            fx_settlement,
         )
         base = defaults.fx_swap_base if base is None else base
         if base == "foreign":
             d_fx, f_fx = f_0, 1.0
         elif base == "domestic":
-            d_fx, f_fx = 1.0,  1.0 / f_0
+            d_fx, f_fx = 1.0, 1.0 / f_0
         else:
             raise ValueError('`base` should be either "domestic" or "foreign".')
         self._set_leg2_notional(f_0)
-        return concat([
-            self.leg1.cashflows(curve_domestic, disc_curve_domestic, d_fx),
-            self.leg2.cashflows(curve_foreign, disc_curve_foreign, f_fx),
-        ], keys=["leg1", "leg2"],
+        return concat(
+            [
+                self.leg1.cashflows(curve_domestic, disc_curve_domestic, d_fx),
+                self.leg2.cashflows(curve_foreign, disc_curve_foreign, f_fx),
+            ],
+            keys=["leg1", "leg2"],
         )
 
 
 class FixedFloatXCS(BaseXCS):
     _fixed_rate_mixin = True
     _leg2_float_spread_mixin = True
     _is_mtm = True
 
     def __init__(
-            self,
-            *args,
-            fx_fixings: Union[list, float, Dual, Dual2] = [],
-            fixed_rate: Optional[float] = None,
-            payment_lag_exchange: Optional[int] = None,
-            leg2_float_spread: Optional[float] = None,
-            leg2_fixings: Optional[Union[float, list]] = None,
-            leg2_fixing_method: Optional[str] = None,
-            leg2_method_param: Optional[int] = None,
-            leg2_spread_compound_method: Optional[str] = None,
-            leg2_payment_lag_exchange: Optional[int] = "inherit",
-            **kwargs,
+        self,
+        *args,
+        fx_fixings: Union[list, float, Dual, Dual2] = [],
+        fixed_rate: Optional[float] = None,
+        payment_lag_exchange: Optional[int] = None,
+        leg2_float_spread: Optional[float] = None,
+        leg2_fixings: Optional[Union[float, list]] = None,
+        leg2_fixing_method: Optional[str] = None,
+        leg2_method_param: Optional[int] = None,
+        leg2_spread_compound_method: Optional[str] = None,
+        leg2_payment_lag_exchange: Optional[int] = "inherit",
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if leg2_payment_lag_exchange == "inherit":
             leg2_payment_lag_exchange = payment_lag_exchange
         if fx_fixings is None:
             raise ValueError(
                 "`fx_fixings` for MTM XCS should be entered as an empty list, not None."
@@ -4488,22 +5515,22 @@
 
 class FixedFixedXCS(BaseXCS):
     _fixed_rate_mixin = True
     _leg2_fixed_rate_mixin = True
     _is_mtm = True
 
     def __init__(
-            self,
-            *args,
-            fx_fixings: Union[list, float, Dual, Dual2] = [],
-            fixed_rate: Optional[float] = None,
-            payment_lag_exchange: Optional[int] = None,
-            leg2_fixed_rate: Optional[float] = None,
-            leg2_payment_lag_exchange: Optional[int] = "inherit",
-            **kwargs,
+        self,
+        *args,
+        fx_fixings: Union[list, float, Dual, Dual2] = [],
+        fixed_rate: Optional[float] = None,
+        payment_lag_exchange: Optional[int] = None,
+        leg2_fixed_rate: Optional[float] = None,
+        leg2_payment_lag_exchange: Optional[int] = "inherit",
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if leg2_payment_lag_exchange == "inherit":
             leg2_payment_lag_exchange = payment_lag_exchange
         if fx_fixings is None:
             raise ValueError(
                 "`fx_fixings` for MTM XCS should be entered as an empty list, not None."
@@ -4553,29 +5580,29 @@
         )
 
 
 class FloatFixedXCS(BaseXCS):
     _float_spread_mixin = True
     _leg2_fixed_rate_mixin = True
     _is_mtm = True
-    _rate_scalar = 100.
+    _rate_scalar = 100.0
 
     def __init__(
-            self,
-            *args,
-            fx_fixings: Union[list, float, Dual, Dual2] = [],
-            float_spread: Optional[float] = None,
-            fixings: Optional[Union[float, list]] = None,
-            fixing_method: Optional[str] = None,
-            method_param: Optional[int] = None,
-            spread_compound_method: Optional[str] = None,
-            payment_lag_exchange: Optional[int] = None,
-            leg2_fixed_rate: Optional[float] = None,
-            leg2_payment_lag_exchange: Optional[int] = "inherit",
-            **kwargs,
+        self,
+        *args,
+        fx_fixings: Union[list, float, Dual, Dual2] = [],
+        float_spread: Optional[float] = None,
+        fixings: Optional[Union[float, list]] = None,
+        fixing_method: Optional[str] = None,
+        method_param: Optional[int] = None,
+        spread_compound_method: Optional[str] = None,
+        payment_lag_exchange: Optional[int] = None,
+        leg2_fixed_rate: Optional[float] = None,
+        leg2_payment_lag_exchange: Optional[int] = "inherit",
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if leg2_payment_lag_exchange == "inherit":
             leg2_payment_lag_exchange = payment_lag_exchange
         if fx_fixings is None:
             raise ValueError(
                 "`fx_fixings` for MTM XCS should be entered as an empty list, not None."
@@ -4701,17 +5728,17 @@
             payment_lag_exchange=leg2_payment_lag_exchange,
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             convention=self.leg2_convention,
         )
         self._initialise_fx_fixings(fx_fixing)
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def rate(
         self,
         curves: Union[Curve, str, list],
         solver: Optional[Solver] = None,
         fx: Optional[FXForwards] = None,
         fixed_rate: bool = False,
@@ -4762,320 +5789,14 @@
         # ini_fx = self.leg2.notional / -self.leg1.notional
         ## TODO decide how to price mid-market rates when ini fx is struck but
         ## there is no fixed points, i,e the FXswap is sem-determined, which is
         ## not a real instrument.
         return (cf / -self.leg1.notional) * 10000
 
 
-# class FXSwap(BaseDerivative):
-#     """
-#     Create an FX Swap instrument.
-#
-#     ``FXSwap`` is a multi-currency derivative. Must supply the ``currency`` and
-#     ``leg2_currency`` as 3-digit codes, for consistent pricing.
-#
-#     Parameters
-#     ----------
-#     args : tuple
-#         Required positional args to :class:`BaseDerivative`.
-#     fx_fixing_points: tuple(float or Dual,), optional
-#        A tuple of two floats (or Duals): the FX rate for the initial exchange applied to
-#        ``notional`` to directly set ``leg2_notional``, and the fx swap points (in
-#        10,000ths) which will directly set the foreign cashflow at termination.
-#
-#        .. warning::
-#
-#           Do not set ``leg2_notional`` directly as an input. Use ``fx_fixing_points`` to
-#           determine the foreign leg notional and cashflows at the settlement dates.
-#
-#     kwargs : dict
-#         Required keyword arguments to :class:`BaseDerivative`.
-#
-#     Notes
-#     -----
-#
-#     **Pricing Parameters**
-#
-#     Although an FX swap contains only 4 cashflows, its definition and operation are
-#     made more complex by allowing pricing parameters to be set or unset at
-#     initialisation. There are 2 possible initialisation states:
-#
-#       - Fixing ``fx0`` and ``points``: this is the common initialisation
-#         for an executed FX swap trade. All pricing parameters are set and determined.
-#       - Not fixing ``fx0`` or ``points``: this is the common initialisation for an
-#         interbank trade. The instrument is defined except for its pricing parameters
-#         which can be priced subject to other variables. Upon execution these parameters
-#         would then be set.
-#
-#     **Cashflow Settlement**
-#
-#     The date generation for FXSwaps used the :class:`Schedule` generator. For FXSwaps
-#     the default ``payment_lag`` is 0 days meaning payment dates align with accrual
-#     start and end dates, so the ``effective`` and ``termination`` date will define the
-#     payment dates (except if they are adjusted under a holiday calendar modification).
-#     The settlement dates for FXSwap cashflows are determined from
-#     the ``schedule.pschedule`` (payment day schedule) attribute of each leg.
-#     """
-#     def __init__(
-#         self,
-#         *args,
-#         fx_fixing_points: Optional[tuple] = None,
-#         **kwargs,
-#     ):
-#         super().__init__(*args, **kwargs)
-#         if self.currency is None or self.leg2_currency is None:
-#             raise ValueError("Must supply `currency` and `leg2_currency` to `FXSwap`.")
-#         self.leg1, self.leg2 = CustomLeg([]), CustomLeg([])
-#         self.leg1.currency,  self.leg2.currency = self.currency, self.leg2_currency
-#         self.pair = self.currency + self.leg2_currency
-#
-#         self.leg1.schedule = Schedule(
-#             effective=self.effective,
-#             termination=self.termination,
-#             frequency="Z",
-#             modifier=self.modifier,
-#             calendar=self.calendar,
-#             payment_lag=self.payment_lag,
-#         )
-#         self.leg2.schedule = Schedule(
-#             effective=self.leg2_effective,
-#             termination=self.leg2_termination,
-#             frequency="Z",
-#             modifier=self.leg2_modifier,
-#             calendar=self.leg2_calendar,
-#             payment_lag=self.leg2_payment_lag,
-#         )
-#         self._fx_fixing_points = fx_fixing_points
-#
-#         if self.notional != -self.leg2_notional:
-#             Warning("`leg2_notional` is not used in the FXSwap class.")
-#         self.leg1.periods = [
-#             Cashflow(
-#                 notional=self.notional,
-#                 payment=self.leg1.schedule.pschedule[0],
-#                 currency=self.leg1.currency
-#             ),
-#             Cashflow(
-#                 notional=-self.notional,
-#                 payment=self.leg1.schedule.pschedule[1],
-#                 currency=self.leg1.currency
-#             )
-#         ]
-#         self.fx_fixing_points = fx_fixing_points  # sets leg2
-#
-#     @property
-#     def fx_fixing_points(self):
-#         """Sets the FX fixing and the swap points to define the cashflows."""
-#         return self._fx_fixing_points
-#
-#     @fx_fixing_points.setter
-#     def fx_fixing_points(self, value):
-#         """Will reset leg2 notional and cashflows. Only called if not set at init."""
-#         self._fx_fixing_points = value
-#         if value is None:
-#             fx0, points = 1.0, 0.0
-#         else:
-#             fx0, points = value[0], value[1]
-#         self._set_cashflows(fx0, points)
-#
-#     def _set_cashflows(self, fx0, points):
-#         self.leg2_notional = -self.notional * fx0
-#         self.leg2.periods = [
-#             Cashflow(notional=self.leg2_notional,
-#                      payment=self.leg2.schedule.pschedule[0],
-#                      currency=self.leg2.currency),
-#             Cashflow(notional=self.notional * (fx0 + points / 10000),
-#                      payment=self.leg2.schedule.pschedule[1],
-#                      currency=self.leg2.currency)
-#         ]
-#
-#     def npv(
-#         self,
-#         fx: Optional[FXForwards] = None,
-#         solver: Optional[Solver] = None,
-#         collateral: Optional[str] = None,
-#         base: Optional[str] = None,
-#     ):
-#         """
-#         Return the NPV of the FXSwap.
-#
-#         An ``FXSwap`` is a multi-currency derivative so an
-#         :class:`~rateslib.fx.FXForwards` object is required for pricing which
-#         contains all the necessary cross-currency discount factors.
-#
-#         Parameters
-#         ----------
-#         fx
-#         solver
-#         collateral
-#         base
-#
-#         Returns
-#         -------
-#         float, Dual or Dual2
-#         """
-#         if fx is None:
-#             if solver is None or solver.fx is None:
-#                 raise ValueError("`fx` or `solver.fx` must be supplied")
-#             elif solver.fx is not None:
-#                 fx = solver.fx
-#
-#         base = fx.base if base is None else base.lower()
-#         if self.fx_fixing_points is None:
-#             fx0 = fx.rate(self.pair, self.leg1.schedule.aschedule[0])
-#             points = self.rate(fx)
-#             self._set_cashflows(float(fx0), float(points))
-#
-#         leg1_npv = (
-#             fx.curve(self.leg1.currency, collateral)[self.leg1.periods[0].payment] *
-#             self.leg1.periods[0].notional + self.leg1.periods[1].notional *
-#             fx.curve(self.leg1.currency, collateral)[self.leg1.periods[1].payment]
-#         )
-#         leg2_npv = (
-#             fx.curve(self.leg2.currency, collateral)[self.leg2.periods[0].payment] *
-#             self.leg2.periods[0].notional + self.leg2.periods[1].notional *
-#             fx.curve(self.leg2.currency, collateral)[self.leg2.periods[1].payment]
-#         )
-#
-#         return (
-#             fx.rate(self.leg1.currency + base) * leg1_npv +
-#             fx.rate(self.leg2.currency + base) * leg2_npv
-#         )
-#
-#     def _npv_alt(
-#         self,
-#         curve_domestic: Curve,
-#         curve_foreign: Curve,
-#         fx_rate: Union[float, Dual],
-#         fx_settlement: Optional[datetime] = None,
-#         base: str = None
-#     ):
-#         """
-#         Return the NPV of the FX swap.
-#
-#         Parameters
-#         ----------
-#         curve_domestic : Curve
-#             The discounting :class:`Curve` for domestic currency cashflows.
-#         curve_foreign : Curve
-#             The discounting :class:`Curve` for foreign currency cashflows.
-#         fx_rate : float, optional
-#             The FX rate for valuing cashflows.
-#         fx_settlement : datetime, optional
-#             The date for settlement of ``fx_rate``. If spot then should be input as T+2.
-#             If `None`, is assumed to be immediate settlement.
-#         base : str, optional
-#             The base currency to express the NPV, either `"domestic"` or `"foreign"`.
-#             Set by default.
-#         """
-#         base = defaults.fx_swap_base if base is None else base
-#         f_0 = forward_fx(
-#             curve_domestic.node_dates[0],
-#             curve_domestic,
-#             curve_foreign,
-#             fx_rate,
-#             fx_settlement
-#         )
-#         if self.fx_fixing_points is None:
-#             args = (curve_domestic, curve_foreign, f_0)
-#             fx = forward_fx(self.leg2.schedule.aschedule[0], *args)
-#             points = self._rate_alt(*args)
-#             self._set_cashflows(fx, points)
-#         leg1_npv = self.leg1.npv(curve_domestic)
-#         leg2_npv = self.leg2.npv(curve_foreign)
-#
-#         if base == "foreign":
-#             return leg1_npv * f_0 + leg2_npv
-#         elif base == "domestic":
-#             return leg1_npv + leg2_npv / f_0
-#         else:
-#             raise ValueError('`base` should be either "domestic" or "foreign".')
-#
-#     def rate(
-#         self,
-#         fx: Optional[FXForwards] = None,
-#         solver: Optional[Solver] = None,
-#     ):
-#         if fx is None:
-#             if solver is None or solver.fx is None:
-#                 raise ValueError("`fx` or `solver.fx` must be supplied")
-#             elif solver.fx is not None:
-#                 fx = solver.fx
-#
-#         fx0 = fx.rate(self.pair, settlement=self.leg1.periods[0].payment)
-#         fx1 = fx.rate(self.pair, settlement=self.leg1.periods[1].payment)
-#         return (fx1 - fx0) * 10000
-#
-#     def _rate_alt(
-#         self,
-#         curve_domestic: Curve,
-#         curve_foreign: Curve,
-#         fx_rate: Optional[Union[float, Dual]] = None,
-#         fx_settlement: Optional[datetime] = None,
-#     ):
-#         """
-#         Return the mid-market rate in points of the FX swap.
-#
-#         Parameters
-#         ----------
-#         curve_domestic : Curve
-#             The discounting :class:`Curve` for domestic currency cashflows.
-#         curve_foreign : Curve
-#             The discounting :class:`Curve` for foreign currency cashflows.
-#         fx_rate : float or Dual, optional
-#             The FX rate for valuing cashflows.
-#         fx_settlement : datetime, optional
-#             The date for settlement of ``fx_rate``. If spot then should be input as T+2.
-#             If `None`, is assumed to be immediate settlement.
-#
-#         Returns
-#         -------
-#         Dual
-#
-#         Notes
-#         -----
-#
-#         .. math::
-#
-#            z_{fx} = f_{i-1} \\left ( \\frac{v_{i-1}-v_i}{v_i} \\right ) + F_0 \\left ( \\frac{w_j^* - w_{j-1}^*}{v_i} \\right )
-#
-#         where, :math:`v_{i-1}, v_i` denote DFs on the dates of exchange of the foreign
-#         currency, and, :math:`w_j^*, w_{j-1}^*` denote dates of exchange of the
-#         domestic currency, which in an FX swap should align.
-#         """
-#         f_0 = forward_fx(
-#             curve_domestic.node_dates[0],
-#             curve_domestic,
-#             curve_foreign,
-#             fx_rate,
-#             fx_settlement
-#         )
-#         args = (curve_domestic, curve_foreign, f_0)
-#         f_i_1 = forward_fx(self.leg2.periods[0].payment, *args)
-#         v_i_1 = curve_foreign[self.leg2.periods[0].payment]
-#         v_i = curve_foreign[self.leg2.periods[1].payment]
-#         w_j_1 = curve_domestic[self.leg1.periods[0].payment]
-#         w_j = curve_domestic[self.leg1.periods[1].payment]
-#         _ = (f_i_1 * (v_i_1 - v_i) + f_0 * (w_j - w_j_1)) / v_i
-#         return _ * 10000
-#
-#     # TODO make FXSwap cashflow arguments consistent with theme
-#     def cashflows(self, curve_domestic, curve_foreign):
-#         return super().cashflows(None, curve_domestic, None, curve_foreign)
-#
-#     def delta(
-#         self,
-#         solver: Optional[Solver] = None,
-#         collateral: Optional[str] = None,
-#         base: Optional[str] = None,
-#     ):
-#         npv = self.npv(None, collateral, solver, base)
-#         return solver.delta(npv)
-
-
 ### Generic Instruments
 
 
 class Spread(Sensitivities):
     """
     A spread instrument defined as the difference in rate between two ``Instruments``.
 
@@ -5119,15 +5840,16 @@
        irs1 = IRS(dt(2022, 1, 1), "3M", "Q", curves=curve1)
        irs2 = IRS(dt(2022, 1, 1), "6M", "Q", curves=curve2)
        spread = Spread(irs1, irs2)
        spread.npv()
        spread.rate()
        spread.cashflows()
     """
-    _rate_scalar = 1.
+
+    _rate_scalar = 1.0
 
     def __init__(self, instrument1, instrument2):
         self.instrument1 = instrument1
         self.instrument2 = instrument2
 
     def npv(self, *args, **kwargs):
         """
@@ -5145,16 +5867,18 @@
         Returns
         -------
         float, Dual or Dual2
         """
         leg1_npv = self.instrument1.npv(*args, **kwargs)
         leg2_npv = self.instrument2.npv(*args, **kwargs)
         if kwargs.get("local", False):
-            return {k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
-                    for k in set(leg1_npv) | set(leg2_npv)}
+            return {
+                k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
+                for k in set(leg1_npv) | set(leg2_npv)
+            }
         else:
             return leg1_npv + leg2_npv
 
     # def npv(self, *args, **kwargs):
     #     if len(args) == 0:
     #         args1 = (kwargs.get("curve1", None), kwargs.get("disc_curve1", None))
     #         args2 = (kwargs.get("curve2", None), kwargs.get("disc_curve2", None))
@@ -5191,18 +5915,20 @@
     #         args2 = (kwargs.get("curve2", None), kwargs.get("disc_curve2", None))
     #     else:
     #         args1 = args
     #         args2 = args
     #     return self.instrument2.rate(*args2) - self.instrument1.rate(*args1)
 
     def cashflows(self, *args, **kwargs):
-        return concat([
-            self.instrument1.cashflows(*args, **kwargs),
-            self.instrument2.cashflows(*args, **kwargs),
-            ], keys=["instrument1", "instrument2"],
+        return concat(
+            [
+                self.instrument1.cashflows(*args, **kwargs),
+                self.instrument2.cashflows(*args, **kwargs),
+            ],
+            keys=["instrument1", "instrument2"],
         )
 
 
 # class SpreadX:
 #     pass
 
 
@@ -5228,15 +5954,16 @@
     with shared pricing arguments for their methods. If this is not true
     consider using the :class:`FlyX`, cross ``Instrument``.
 
     Examples
     --------
     See examples for :class:`Spread` for similar functionality.
     """
-    _rate_scalar = 1.
+
+    _rate_scalar = 1.0
 
     def __init__(self, instrument1, instrument2, instrument3):
         self.instrument1 = instrument1
         self.instrument2 = instrument2
         self.instrument3 = instrument3
 
     def npv(self, *args, **kwargs):
@@ -5256,16 +5983,18 @@
         -------
         float, Dual or Dual2
         """
         leg1_npv = self.instrument1.npv(*args, **kwargs)
         leg2_npv = self.instrument2.npv(*args, **kwargs)
         leg3_npv = self.instrument3.npv(*args, **kwargs)
         if kwargs.get("local", False):
-            return {k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
-                    for k in set(leg1_npv) | set(leg2_npv)}
+            return {
+                k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
+                for k in set(leg1_npv) | set(leg2_npv)
+            }
         else:
             return leg1_npv + leg2_npv + leg3_npv
 
     def rate(self, *args, **kwargs):
         """
         Return the mid-market rate of the composited via the difference of instrument
         rates.
@@ -5285,19 +6014,21 @@
         """
         leg1_rate = self.instrument1.rate(*args, **kwargs)
         leg2_rate = self.instrument2.rate(*args, **kwargs)
         leg3_rate = self.instrument3.rate(*args, **kwargs)
         return -leg3_rate + 2 * leg2_rate - leg1_rate
 
     def cashflows(self, *args, **kwargs):
-        return concat([
-            self.instrument1.cashflows(*args, **kwargs),
-            self.instrument2.cashflows(*args, **kwargs),
-            self.instrument3.cashflows(*args, **kwargs),
-            ], keys=["instrument1", "instrument2", "instrument3"],
+        return concat(
+            [
+                self.instrument1.cashflows(*args, **kwargs),
+                self.instrument2.cashflows(*args, **kwargs),
+                self.instrument3.cashflows(*args, **kwargs),
+            ],
+            keys=["instrument1", "instrument2", "instrument3"],
         )
 
 
 # class FlyX:
 #     """
 #     A butterly instrument which is the spread of two spread instruments
 #     """
@@ -5326,15 +6057,14 @@
 #             args1 = args
 #             args2 = args
 #             args3 = args
 #         return 2 * self.instrument2.rate(*args2) - self.instrument1.rate(*args1) - self.instrument3.rate(*args3)
 
 
 class Portfolio(Sensitivities):
-
     def __init__(self, instruments):
         self.instruments = instruments
 
     def npv(self, *args, **kwargs):
         # TODO do not permit a mixing of currencies.
         # TODO look at legs.npv where args len is used.
         if kwargs.get("local", False):
@@ -5449,10 +6179,166 @@
 
     _ = curve_domestic[date] / curve_foreign[date]
     if fx_settlement is not None:
         _ *= curve_foreign[fx_settlement] / curve_domestic[fx_settlement]
     _ *= fx_rate
     return _
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+
+
+# def _ytm_quadratic_converger(f, y0, y1, y2, tol=1e-9):
+#     """
+#     Convert a price from yield function `f` into a quadratic approximation and
+#     determine the root, yield, which matches the target price.
+#     """
+#     _A = np.array([[y0**2, y0, 1], [y1**2, y1, 1], [y2**2, y2, 1]])
+#     _b = np.array([f(y0), f(y1), f(y2)])[:, None]
+#
+#     # check tolerance from previous recursive estimations
+#     if abs(_b[1, 0]) < tol:
+#         return y1
+#
+#     c = np.linalg.solve(_A, _b)
+#
+#     yield1 = ((-c[1] + sqrt(c[1]**2 - 4 * c[0] * c[2])) / (2 * c[0]))[0]
+#     yield2 = ((-c[1] - sqrt(c[1]**2 - 4 * c[0] * c[2])) / (2 * c[0]))[0]
+#     z1, z2 = f(yield1), f(yield2)
+#
+#     # make a linear guess at new quadratic solution
+#     approx_yield = yield1 - (yield2 - yield1) * z1 / (z2 - z1)
+#     if abs(z1) < abs(z2):
+#         soln_yield = yield1
+#         if abs(z1) < tol:
+#             return soln_yield
+#     else:
+#         soln_yield = yield2
+#         if abs(z2) < tol:
+#             return soln_yield
+#     return _ytm_quadratic_converger(
+#         f,
+#         approx_yield - max(10 * (approx_yield - soln_yield), 0.001),
+#         approx_yield,
+#         approx_yield + max(10 * (approx_yield - soln_yield), 0.001),
+#         tol
+#     )
+
+
+def _ytm_quadratic_converger2(f, y0, y1, y2, f0=None, f1=None, f2=None, tol=1e-9):
+    """
+    Convert a price from yield function `f` into a quadratic approximation and
+    determine the root, yield, which matches the target price.
+    """
+    # allow function values to be passed recursively to avoid re-calculation
+    f0 = f(y0) if f0 is None else f0
+    f1 = f(y1) if f1 is None else f1
+    f2 = f(y2) if f2 is None else f2
+
+    if f0 < 0 and f1 < 0 and f2 < 0:
+        # reassess initial values
+        return _ytm_quadratic_converger2(
+            f, 2 * y0 - y2, y1 - y2 + y0, y0, None, None, f0, tol
+        )
+    elif f0 > 0 and f1 > 0 and f2 > 0:
+        return _ytm_quadratic_converger2(
+            f, y2, y1 + 1 * (y2 - y0), y2 + 2 * (y2 - y0), f2, None, None, tol
+        )
+
+    _b = np.array([y0, y1, y2])[:, None]
+    # check tolerance from previous recursive estimations
+    for i, f_ in enumerate([f0, f1, f2]):
+        if abs(f_) < tol:
+            return _b[i, 0]
+
+    _A = np.array([[f0**2, f0, 1], [f1**2, f1, 1], [f2**2, f2, 1]])
+    c = np.linalg.solve(_A, _b)
+    y = c[2, 0]
+    f_ = f(y)
+
+    pad = min(tol * 1e8, 0.0001, abs(f_ * 1e4))  # avoids singular matrix error
+    if y <= y0:
+        return _ytm_quadratic_converger2(
+            f, 2 * y - y0 - pad, y, y0 + pad, None, f_, None, tol
+        )
+    elif y0 < y <= y1:
+        if (y - y0) < (y1 - y):
+            return _ytm_quadratic_converger2(
+                f, y0 - pad, y, 2 * y - y0 + pad, None, f_, None, tol
+            )
+        else:
+            return _ytm_quadratic_converger2(
+                f, 2 * y - y1 - pad, y, y1 + pad, None, f_, None, tol
+            )
+    elif y1 < y <= y2:
+        if (y - y1) < (y2 - y):
+            return _ytm_quadratic_converger2(
+                f, y1 - pad, y, 2 * y - y1 + pad, None, f_, None, tol
+            )
+        else:
+            return _ytm_quadratic_converger2(
+                f, 2 * y - y2 - pad, y, y2 + pad, None, f_, None, tol
+            )
+    else:  # y2 < y:
+        return _ytm_quadratic_converger2(
+            f, y2 - pad, y, 2 * y - y2 + pad, None, f_, None, tol
+        )
+
+
+# def _brents(f, x0, x1, max_iter=50, tolerance=1e-9):
+#     fx0 = f(x0)
+#     fx1 = f(x1)
+#
+#     if float(fx0 * fx1) > 0:
+#         raise ValueError(
+#             "`brents` must initiate from function values with opposite signs.")
+#
+#     if abs(fx0) < abs(fx1):
+#         x0, x1 = x1, x0
+#         fx0, fx1 = fx1, fx0
+#
+#     x2, fx2 = x0, fx0
+#
+#     mflag = True
+#     steps_taken = 0
+#
+#     while steps_taken < max_iter and abs(x1 - x0) > tolerance:
+#         fx0 = f(x0)
+#         fx1 = f(x1)
+#         fx2 = f(x2)
+#
+#         if fx0 != fx2 and fx1 != fx2:
+#             L0 = (x0 * fx1 * fx2) / ((fx0 - fx1) * (fx0 - fx2))
+#             L1 = (x1 * fx0 * fx2) / ((fx1 - fx0) * (fx1 - fx2))
+#             L2 = (x2 * fx1 * fx0) / ((fx2 - fx0) * (fx2 - fx1))
+#             new = L0 + L1 + L2
+#
+#         else:
+#             new = x1 - ((fx1 * (x1 - x0)) / (fx1 - fx0))
+#
+#         if ((float(new) < float((3 * x0 + x1) / 4) or float(new) > float(x1)) or
+#                 (mflag == True and (abs(new - x1)) >= (abs(x1 - x2) / 2)) or
+#                 (mflag == False and (abs(new - x1)) >= (abs(x2 - d) / 2)) or
+#                 (mflag == True and (abs(x1 - x2)) < tolerance) or
+#                 (mflag == False and (abs(x2 - d)) < tolerance)):
+#             new = (x0 + x1) / 2
+#             mflag = True
+#
+#         else:
+#             mflag = False
+#
+#         fnew = f(new)
+#         d, x2 = x2, x1
+#
+#         if float(fx0 * fnew) < 0:
+#             x1 = new
+#         else:
+#             x0 = new
+#
+#         if abs(fx0) < abs(fx1):
+#             x0, x1 = x1, x0
+#
+#         steps_taken += 1
+#
+#     return x1, steps_taken
```

### Comparing `rateslib-0.1.0/rateslib/legs.py` & `rateslib-0.2.0/rateslib/legs.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 from pandas import DataFrame, Series
 
 from rateslib import defaults
 from rateslib.calendars import add_tenor
 from rateslib.scheduling import Schedule
 from rateslib.curves import Curve
 from rateslib.periods import (
+    IndexFixedPeriod,
     FixedPeriod,
     FloatPeriod,
     Cashflow,
+    IndexCashflow,
     _validate_float_args,
-    _get_fx_and_base
+    _get_fx_and_base,
 )
 from rateslib.dual import Dual, Dual2, set_order
 from rateslib.fx import FXForwards, FXRates
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
@@ -238,15 +240,18 @@
         should typically be avoided anyway.
 
         Returns
         -------
         bool
         """
         if "Float" in type(self).__name__:
-            if "rfr" in self.fixing_method and self.spread_compound_method != "none_simple":
+            if (
+                "rfr" in self.fixing_method
+                and self.spread_compound_method != "none_simple"
+            ):
                 return False
         return True
 
     def _spread(self, target_npv, fore_curve, disc_curve, fx=None):
         """
         Calculates an adjustment to the ``fixed_rate`` or ``float_spread`` to match
         a specific target NPV.
@@ -283,21 +288,20 @@
         Examples
         --------
         """
         if self._is_linear:
             a_delta = self.analytic_delta(fore_curve, disc_curve, fx, self.currency)
             return -target_npv / a_delta
         else:
-            # raise NotImplementedError("needs development XXXXX")
             # This method creates a dual2 variable for float spread.
             _fs = self.float_spread
-            self.float_spread = Dual2(0. if _fs is None else float(_fs), "spread_z")
+            self.float_spread = Dual2(0.0 if _fs is None else float(_fs), "spread_z")
 
             # This method uses ad-hoc AD to solve a specific problem for which
-            # there is no close form solution. Calculating NPV is very inefficient
+            # there is no closed form solution. Calculating NPV is very inefficient
             # so, we only do this once as opposed to using a root solver algo
             # which would otherwise converge to the exact solution but is
             # practically not workable.
 
             fore_ad = fore_curve.ad
             fore_curve._set_ad_order(2)
 
@@ -311,26 +315,27 @@
             npv = self.npv(fore_curve, disc_curve, fx, self.currency)
             b = npv.gradient("spread_z", order=1)[0]
             a = 0.5 * npv.gradient("spread_z", order=2)[0][0]
             c = -target_npv
 
             _1 = -c / b
             if abs(a) > 1e-14:
-                _2a = (-b - (b**2 - 4*a*c)**0.5) / (2*a)
-                _2b = (-b + (b**2 - 4*a*c)**0.5) / (2*a)  # alt quadratic soln
+                _2a = (-b - (b**2 - 4 * a * c) ** 0.5) / (2 * a)
+                _2b = (-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)  # alt quadratic soln
                 if abs(_1 - _2a) < abs(_1 - _2b):
                     _ = _2a
                 else:
                     _ = _2b  # select quadratic soln
             else:  # pragma: no cover
                 # this is to avoid divide by zero errors and return an approximation
                 _ = _1
                 warnings.warn(
                     "Divide by zero encountered and the spread is approximated to "
-                    "first order.", UserWarning
+                    "first order.",
+                    UserWarning,
                 )
 
             self.float_spread = _fs
             fore_curve._set_ad_order(fore_ad)
             disc_curve._set_ad_order(disc_ad)
             if isinstance(fx, (FXRates, FXForwards)):
                 fx._set_ad_order(_fx)
@@ -370,37 +375,40 @@
         Required positional args to :class:`BaseLeg`.
     fixed_rate : float, optional
         The rate applied to determine cashflows. Can be set to `None` and designated
         later, perhaps after a mid-market rate for all periods has been calculated.
     kwargs : dict
         Required keyword arguments to :class:`BaseLeg`.
     """
-    def __init__(self, *args,  fixed_rate: Optional[float] = None, **kwargs):
+
+    def __init__(self, *args, fixed_rate: Optional[float] = None, **kwargs):
         self._fixed_rate = fixed_rate
         super().__init__(*args, **kwargs)
         self.periods = [
             FixedPeriod(
                 fixed_rate=self.fixed_rate,
                 start=period[defaults.headers["a_acc_start"]],
                 end=period[defaults.headers["a_acc_end"]],
                 payment=period[defaults.headers["payment"]],
                 notional=self.notional - self.amortization * i,
                 currency=self.currency,
                 convention=self.convention,
                 termination=self.schedule.termination,
                 frequency=self.schedule.frequency,
-                stub=True if period[defaults.headers["stub_type"]] == "Stub" else False
-            ) for i, period in self.schedule.table.to_dict(orient="index").items()
+                stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 class FloatLegMixin:
     """
     Add the functionality to add and retrieve ``float_spread`` on
     :class:`~rateslib.periods.FloatPeriod` s and a :meth:`fixings_table`.
     """
 
     def _set_fixings(
@@ -421,15 +429,15 @@
                 # fixing_method in ["rfr_lookback", "rfr_observation_shift", "ibor"]:
                 adj_days = self.method_param
             first_required_day = [
                 add_tenor(
                     self.schedule.aschedule[i],
                     f"-{adj_days}B",
                     None,
-                    self.schedule.calendar
+                    self.schedule.calendar,
                 )
                 for i in range(self.schedule.n_periods)
             ]
             fixings = [
                 fixings if last_fixing >= day else None for day in first_required_day
             ]
         elif not isinstance(fixings, list):
@@ -588,27 +596,31 @@
            frequency="M",
            fixings=[[1.19, 1.19, -8.81]],
            currency="SEK",
        )
        float_leg.cashflows(curve)
        float_leg.fixings_table(curve)[dt(2022,12,28):dt(2023,1,4)]
     """
+
     def __init__(
         self,
         *args,
         float_spread: Optional[float] = None,
         fixings: Optional[Union[float, list, Series]] = None,
         fixing_method: Optional[str] = None,
         method_param: Optional[int] = None,
         spread_compound_method: Optional[str] = None,
-        **kwargs
+        **kwargs,
     ):
         self._float_spread = float_spread
-        self.fixing_method, self.method_param, self.spread_compound_method = \
-            _validate_float_args(fixing_method, method_param, spread_compound_method)
+        (
+            self.fixing_method,
+            self.method_param,
+            self.spread_compound_method,
+        ) = _validate_float_args(fixing_method, method_param, spread_compound_method)
 
         super().__init__(*args, **kwargs)
 
         self._set_fixings(fixings)
         self.periods = [
             FloatPeriod(
                 float_spread=self.float_spread,
@@ -620,16 +632,17 @@
                 convention=self.convention,
                 termination=self.schedule.termination,
                 frequency=self.schedule.frequency,
                 stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
                 fixing_method=self.fixing_method,
                 fixings=self.fixings[i],
                 method_param=self.method_param,
-                spread_compound_method=self.spread_compound_method
-            ) for i, period in self.schedule.table.to_dict(orient="index").items()
+                spread_compound_method=self.spread_compound_method,
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
 
     # @property
     # def _is_complex(self):
     #     """
     #     A complex float leg is one which is RFR based and for which each individual
     #     RFR fixing is required is order to calculate correctly. This occurs in the
@@ -701,27 +714,31 @@
        the leg is acceptable, i.e. a leg calendar of *"nyc,ldn,tgt"* and a curve
        calendar of *"ldn"* is valid, whereas only *"nyc,tgt"* may give errors.
 
     Examples
     --------
     TODO
     """
+
     def __init__(
         self,
         *args,
         float_spread: Optional[float] = None,
         fixings: Optional[Union[float, list, Series]] = None,
         fixing_method: Optional[str] = None,
         method_param: Optional[int] = None,
         spread_compound_method: Optional[str] = None,
-        **kwargs
+        **kwargs,
     ):
         self._float_spread = float_spread
-        self.fixing_method, self.method_param, self.spread_compound_method = \
-            _validate_float_args(fixing_method, method_param, spread_compound_method)
+        (
+            self.fixing_method,
+            self.method_param,
+            self.spread_compound_method,
+        ) = _validate_float_args(fixing_method, method_param, spread_compound_method)
 
         super().__init__(*args, **kwargs)
         if abs(float(self.amortization)) > 1e-2:
             raise NotImplementedError("`ZeroFloatLeg` cannot accept `amortization`.")
 
         self._set_fixings(fixings)
         self.periods = [
@@ -735,53 +752,22 @@
                 convention=self.convention,
                 termination=self.schedule.termination,
                 frequency=self.schedule.frequency,
                 stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
                 fixing_method=self.fixing_method,
                 fixings=self.fixings[i],
                 method_param=self.method_param,
-                spread_compound_method=self.spread_compound_method
-            ) for i, period in self.schedule.table.to_dict(orient="index").items()
+                spread_compound_method=self.spread_compound_method,
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
 
-    # @property
-    # def _is_complex(self):
-    #     """
-    #     A complex float leg is one which is RFR based and for which each individual
-    #     RFR fixing is required is order to calculate correctly. This occurs in the
-    #     following cases:
-    #
-    #     1) The ``fixing_method`` is *"lookback"* - since fixing have arbitrary
-    #        weightings misaligned with their standard weightings due to
-    #        arbitrary shifts.
-    #     2) The ``spread_compound_method`` is not *"none_simple"* - this is because the
-    #        float spread is compounded alongside the rates so there is a non-linear
-    #        relationship. Note if spread is zero this is negated and can be ignored.
-    #     3) The ``fixing_method`` is *"lockout"* - technically this could be made semi
-    #        efficient by splitting calculations into two parts. As of now it
-    #        remains within the inefficient complex section.
-    #     4) ``fixings`` are given which need to be incorporated into the calculation.
-    #
-    #
-    #     """
-    #     if self.fixing_method in ["rfr_payment_delay", "rfr_observation_shift"]:
-    #         if self.fixings is not None:
-    #             return True
-    #         elif abs(self.float_spread) < 1e-9 or \
-    #                 self.spread_compound_method == "none_simple":
-    #             return False
-    #         else:
-    #             return True
-    #     elif self.fixing_method == "ibor":
-    #         return False
-    #     return True
-
     @property
     def dcf(self):
-        _ = 0.
+        _ = 0.0
         for period in self.periods:
             _ += period.dcf
         return _
 
     def rate(self, curve):
         """
         Calculating the floating rate for the zero coupon leg.
@@ -791,52 +777,56 @@
         curve : Curve, LineCurve
             The forecasting curve object.
 
         Returns
         -------
         float, Dual, Dual2
         """
-        compounded_rate, total_dcf = 1., 0.
+        compounded_rate, total_dcf = 1.0, 0.0
         for period in self.periods:
             compounded_rate *= 1 + period.dcf * period.rate(curve) / 100
             total_dcf += period.dcf
-        return 100 * (compounded_rate - 1.) / total_dcf
+        return 100 * (compounded_rate - 1.0) / total_dcf
 
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = (
-                self.rate(curve) / 100 * self.dcf * disc_curve[
-            self.schedule.pschedule[-1]] * -self.notional
+            self.rate(curve)
+            / 100
+            * self.dcf
+            * disc_curve[self.schedule.pschedule[-1]]
+            * -self.notional
         )
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
     def fixings_table(self, curve: Curve):
         # TODO: fixing table for ZeroFloatLeg
         raise NotImplementedError("fixings table on ZeroFloatLeg.")
 
     def analytic_delta(self, *args, **kwargs):
+        # TODO: a delta for ZeroFloatLeg
         raise NotImplementedError("analytic delta on ZeroFloatLeg.")
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         """
         Return the properties of the leg used in calculating cashflows.
 
         Parameters
         ----------
         curve : Curve, optional
@@ -859,42 +849,45 @@
         Returns
         -------
         DataFrame
         """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
         rate = None if curve is None else float(self.rate(curve))
-        cashflow = None if rate is None else -float(
-            self.notional * self.dcf * rate / 100
+        cashflow = (
+            None if rate is None else -float(self.notional * self.dcf * rate / 100)
         )
         if disc_curve is None or rate is None:
             npv, npv_fx = None, None
         else:
             npv = float(self.npv(curve, disc_curve))
             npv_fx = npv * float(fx)
-        spread = 0. if self.float_spread is None else float(self.float_spread)
-        seq= [{
-            defaults.headers["type"]: type(self).__name__,
-            defaults.headers["stub_type"]: None,
-            defaults.headers["currency"]: self.currency.upper(),
-            defaults.headers["a_acc_start"]: self.schedule.aschedule[0],
-            defaults.headers["a_acc_end"]: self.schedule.aschedule[-1],
-            defaults.headers["payment"]: self.schedule.pschedule[-1],
-            defaults.headers["convention"]: self.convention,
-            defaults.headers["dcf"]: self.dcf,
-            defaults.headers["notional"]: float(self.notional),
-            defaults.headers["df"]: None if disc_curve is None else float(
-                disc_curve[self.schedule.pschedule[-1]]),
-            defaults.headers["rate"]: rate,
-            defaults.headers["spread"]: spread,
-            defaults.headers["cashflow"]: cashflow,
-            defaults.headers["npv"]: npv,
-            defaults.headers["fx"]: float(fx),
-            defaults.headers["npv_fx"]: npv_fx,
-        }]
+        spread = 0.0 if self.float_spread is None else float(self.float_spread)
+        seq = [
+            {
+                defaults.headers["type"]: type(self).__name__,
+                defaults.headers["stub_type"]: None,
+                defaults.headers["currency"]: self.currency.upper(),
+                defaults.headers["a_acc_start"]: self.schedule.aschedule[0],
+                defaults.headers["a_acc_end"]: self.schedule.aschedule[-1],
+                defaults.headers["payment"]: self.schedule.pschedule[-1],
+                defaults.headers["convention"]: self.convention,
+                defaults.headers["dcf"]: self.dcf,
+                defaults.headers["notional"]: float(self.notional),
+                defaults.headers["df"]: None
+                if disc_curve is None
+                else float(disc_curve[self.schedule.pschedule[-1]]),
+                defaults.headers["rate"]: rate,
+                defaults.headers["spread"]: spread,
+                defaults.headers["cashflow"]: cashflow,
+                defaults.headers["npv"]: npv,
+                defaults.headers["fx"]: float(fx),
+                defaults.headers["npv_fx"]: npv_fx,
+            }
+        ]
         return DataFrame.from_records(seq)
 
 
 class BaseLegExchange(BaseLeg):
     """
     Abstract base class with common parameters for all ``LegExchange`` subclasses.
 
@@ -912,27 +905,29 @@
 
     See Also
     --------
     FixedLegExchange : Create a fixed leg with additional notional exchanges.
     FloatLegExchange : Create a floating leg with additional notional exchanges.
     BaseLegExchangeMtm : Base class for legs with additional MTM notional exchanges.
     """
+
     _is_mtm = False
 
     def __init__(
         self,
         *args,
         initial_exchange: bool = True,
         payment_lag_exchange: Optional[int] = None,
         **kwargs,
     ):
         self._no_base_notional = True
         self.payment_lag_exchange = (
-             defaults.payment_lag_exchange if payment_lag_exchange is None
-             else payment_lag_exchange
+            defaults.payment_lag_exchange
+            if payment_lag_exchange is None
+            else payment_lag_exchange
         )
         self.initial_exchange = initial_exchange
         super().__init__(*args, **kwargs)
 
     @property
     def notional(self):
         return self._notional
@@ -956,15 +951,16 @@
         pass  # pragma: no cover
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-class FixedLegExchange(BaseLegExchange, FixedLegMixin):
+
+class FixedLegExchange(FixedLegMixin, BaseLegExchange):
     """
     Create a leg of :class:`~rateslib.periods.FixedPeriod` s and initial and final
     :class:`~rateslib.periods.Cashflow` s.
 
     Parameters
     ----------
     args : dict
@@ -985,81 +981,259 @@
     The final cashflow notional is set as the notional. The payment date is set equal
     to the final accrual date adjusted by ``payment_lag_exchange``.
 
     If ``amortization`` is specified an exchanged notional equivalent to the
     amortization amount is added to the list of periods. For similar examples see
     :class:`~rateslib.legs.FloatLegExchange`.
     """
-    def __init__(
-        self,
-        *args,
-        fixed_rate: Optional[float] = None,
-        **kwargs
-    ):
+
+    def __init__(self, *args, fixed_rate: Optional[float] = None, **kwargs) -> None:
         self._fixed_rate = fixed_rate
         super().__init__(*args, **kwargs)
         self._set_periods()
 
-    def _set_periods(self):
+    def _set_periods(self) -> None:
         # initial exchange
-        self.periods = [Cashflow(
-            -self.notional,
-            add_tenor(
-                self.schedule.aschedule[0],
-                f"{self.payment_lag_exchange}B",
-                None,
-                self.schedule.calendar
-            ),
-            self.currency,
-            "Exchange",
-        )] if self.initial_exchange else []
+        self.periods = (
+            [
+                Cashflow(
+                    -self.notional,
+                    add_tenor(
+                        self.schedule.aschedule[0],
+                        f"{self.payment_lag_exchange}B",
+                        None,
+                        self.schedule.calendar,
+                    ),
+                    self.currency,
+                    "Exchange",
+                )
+            ]
+            if self.initial_exchange
+            else []
+        )
 
         regular_periods = [
             FixedPeriod(
                 fixed_rate=self.fixed_rate,
                 start=period[defaults.headers["a_acc_start"]],
                 end=period[defaults.headers["a_acc_end"]],
                 payment=period[defaults.headers["payment"]],
                 notional=self.notional - self.amortization * i,
                 convention=self.convention,
                 currency=self.currency,
                 termination=self.schedule.termination,
                 frequency=self.schedule.frequency,
-                stub=True if period[defaults.headers["stub_type"]] == "Stub" else False
-            ) for i, period in self.schedule.table.to_dict(orient="index").items()
+                stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
         if self.amortization != 0:
             amortization = [
                 Cashflow(
                     self.amortization,
                     self.schedule.pschedule[1 + i],
                     self.currency,
                     "Amortization",
-                ) for i in range(self.schedule.n_periods - 1)
+                )
+                for i in range(self.schedule.n_periods - 1)
+            ]
+            interleaved_periods = [
+                val for pair in zip(regular_periods, amortization) for val in pair
+            ]
+            interleaved_periods.append(regular_periods[-1])  # add last regular period
+        else:
+            interleaved_periods = regular_periods
+        self.periods.extend(interleaved_periods)
+
+        # final cashflow
+        self.periods.append(
+            Cashflow(
+                self.notional - self.amortization * (self.schedule.n_periods - 1),
+                add_tenor(
+                    self.schedule.aschedule[-1],
+                    f"{self.payment_lag_exchange}B",
+                    None,
+                    self.schedule.calendar,
+                ),
+                self.currency,
+                "Exchange",
+            )
+        )
+
+
+class IndexFixedLegExchange(FixedLegMixin, BaseLegExchange):
+    """
+    Create a leg of :class:`~rateslib.periods.IndexFixedPeriod` s and initial and
+    final :class:`~rateslib.periods.IndexCashflow` s.
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`BaseLegExchange`.
+    index_base : float or None, optional
+        The base index to determine the cashflow.
+    index_fixings : float, or Series, optional
+        If a float scalar, will be applied as the index fixing for the whole
+        period. If a datetime indexed ``Series`` will use the
+        fixings that are available in that object, and derive the rest from the
+        ``curve``.
+    index_method : str
+        Whether the indexing uses a daily measure for settlement or the most recently
+        monthly data taken from the first day of month.
+    fixed_rate : float or None
+        The fixed rate applied to determine cashflows. Can be set to `None` and
+        designated later, perhaps after a mid-market rate for all periods has been
+        calculated.
+    kwargs : dict
+        Required keyword arguments to :class:`BaseLegExchange`.
+
+    Notes
+    -----
+    The initial cashflow notional is set as the negative of the notional. The payment
+    date is set equal to the accrual start date adjusted by
+    the ``payment_lag_exchange``.
+
+    The final cashflow notional is set as the notional. The payment date is set equal
+    to the final accrual date adjusted by ``payment_lag_exchange``.
+
+    If ``amortization`` is specified an exchanged notional equivalent to the
+    amortization amount is added to the list of periods. For similar examples see
+    :class:`~rateslib.legs.FloatLegExchange`.
+    """
+
+    def __init__(
+        self,
+        *args,
+        index_base: float,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: str = "daily",
+        fixed_rate: Optional[float] = None,
+        **kwargs
+    ) -> None:
+        self._fixed_rate = fixed_rate
+        self.index_base = index_base
+        self.index_method = index_method.lower()
+        if self.index_method not in ["daily", "monthly"]:
+            raise ValueError("`index_method` must be in {'daily', 'monthly'}.")
+        super().__init__(*args, **kwargs)
+        self._set_index_fixings(index_fixings)
+        self._set_periods()
+
+    def _set_index_fixings(
+        self,
+        index_fixings: Optional[Union[float, list, Series]]
+    ) -> None:
+        """
+        Re-organises the ``index_fixings`` input to list structure for each period.
+        Requires a ``schedule`` object and ``index_args``.
+        """
+        if index_fixings is None:
+            index_fixings_: list = []
+        elif isinstance(index_fixings, Series):
+            last_fixing = index_fixings.index[-1]
+            required_day = self.schedule.pschedule[:self.schedule.n_periods]
+            if self.index_method == "monthly":
+                required_day = [
+                    datetime(d.year, d.month, 1) for d in required_day
+                ]
+            index_fixings_ = [
+                index_fixings if last_fixing >= d else None for d in required_day
+            ]
+        elif not isinstance(index_fixings, list):
+            index_fixings_ = [index_fixings]
+        else:
+            index_fixings_ = index_fixings
+
+        self.index_fixings = (
+            index_fixings_ + [None] * (self.schedule.n_periods - len(index_fixings_))
+        )
+        return None
+
+    def _set_periods(self) -> None:
+        # initial exchange
+        self.periods = (
+            [
+                IndexCashflow(
+                    notional=-self.notional,
+                    payment=add_tenor(
+                        self.schedule.aschedule[0],
+                        f"{self.payment_lag_exchange}B",
+                        None,
+                        self.schedule.calendar,
+                    ),
+                    currency=self.currency,
+                    stub_type="Exchange",
+                    rate=None,
+                    index_base=self.index_base,
+                    index_fixings=self.index_fixings[0],
+                    index_method=self.index_method
+                )
+            ]
+            if self.initial_exchange
+            else []
+        )
+
+        regular_periods = [
+            IndexFixedPeriod(
+                fixed_rate=self.fixed_rate,
+                start=period[defaults.headers["a_acc_start"]],
+                end=period[defaults.headers["a_acc_end"]],
+                payment=period[defaults.headers["payment"]],
+                notional=self.notional - self.amortization * i,
+                convention=self.convention,
+                currency=self.currency,
+                termination=self.schedule.termination,
+                frequency=self.schedule.frequency,
+                stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
+                index_base=self.index_base,
+                index_method=self.index_method,
+                index_fixings=self.index_fixings[i]
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
+        ]
+        if self.amortization != 0:
+            amortization = [
+                IndexCashflow(
+                    notional=self.amortization,
+                    payment=self.schedule.pschedule[1 + i],
+                    currency=self.currency,
+                    stub_type="Amortization",
+                    rate=None,
+                    index_base=self.index_base,
+                    index_fixings=self.index_fixings[1 + i],
+                    index_method=self.index_method
+                )
+                for i in range(self.schedule.n_periods - 1)
             ]
             interleaved_periods = [
                 val for pair in zip(regular_periods, amortization) for val in pair
             ]
             interleaved_periods.append(regular_periods[-1])  # add last regular period
         else:
             interleaved_periods = regular_periods
         self.periods.extend(interleaved_periods)
 
         # final cashflow
-        self.periods.append(Cashflow(
-            self.notional - self.amortization * (self.schedule.n_periods - 1),
-            add_tenor(
-                self.schedule.aschedule[-1],
-                f"{self.payment_lag_exchange}B",
-                None,
-                self.schedule.calendar
-            ),
-            self.currency,
-            "Exchange",
-        ))
+        self.periods.append(
+            IndexCashflow(
+                notional=self.notional - self.amortization * (self.schedule.n_periods - 1),
+                payment=add_tenor(
+                    self.schedule.aschedule[-1],
+                    f"{self.payment_lag_exchange}B",
+                    None,
+                    self.schedule.calendar,
+                ),
+                currency=self.currency,
+                stub_type="Exchange",
+                rate=None,
+                index_base=self.index_base,
+                index_fixings=self.index_fixings[-1],
+                index_method=self.index_method
+            )
+        )
 
 
 class FloatLegExchange(BaseLegExchange, FloatLegMixin):
     """
     Create a leg of :class:`~rateslib.periods.FloatPeriod` s and initial and
     final :class:`~rateslib.periods.Cashflow` s.
 
@@ -1110,46 +1284,56 @@
        float_leg_exch.cashflows(curve)
 
     .. ipython:: python
 
        float_leg_exch = FloatLegExchange(dt(2022, 1, 1), "9M", "Q", notional=1000000, amortization=200000)
        float_leg_exch.cashflows(curve)
     """
+
     def __init__(
         self,
         *args,
         float_spread: Union[float, None] = None,
         fixings: Optional[Union[float, list, Series]] = None,
         fixing_method: Optional[str] = None,
         method_param: Optional[int] = None,
         spread_compound_method: Optional[str] = None,
-        **kwargs
+        **kwargs,
     ):
         self._float_spread = float_spread
-        self.fixing_method, self.method_param, self.spread_compound_method = \
-            _validate_float_args(fixing_method, method_param, spread_compound_method)
+        (
+            self.fixing_method,
+            self.method_param,
+            self.spread_compound_method,
+        ) = _validate_float_args(fixing_method, method_param, spread_compound_method)
 
         super().__init__(*args, **kwargs)
 
         self._set_fixings(fixings)
         self._set_periods()
 
     def _set_periods(self):
         # initial exchange
-        self.periods = [Cashflow(
-            -self.notional,
-            add_tenor(
-                self.schedule.aschedule[0],
-                f"{self.payment_lag_exchange}B",
-                None,
-                self.schedule.calendar
-            ),
-            self.currency,
-            "Exchange",
-        )] if self.initial_exchange else []
+        self.periods = (
+            [
+                Cashflow(
+                    -self.notional,
+                    add_tenor(
+                        self.schedule.aschedule[0],
+                        f"{self.payment_lag_exchange}B",
+                        None,
+                        self.schedule.calendar,
+                    ),
+                    self.currency,
+                    "Exchange",
+                )
+            ]
+            if self.initial_exchange
+            else []
+        )
 
         regular_periods = [
             FloatPeriod(
                 float_spread=self.float_spread,
                 start=period[defaults.headers["a_acc_start"]],
                 end=period[defaults.headers["a_acc_end"]],
                 payment=period[defaults.headers["payment"]],
@@ -1158,46 +1342,50 @@
                 currency=self.currency,
                 convention=self.convention,
                 termination=self.schedule.termination,
                 stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
                 fixings=self.fixings[i],
                 fixing_method=self.fixing_method,
                 method_param=self.method_param,
-                spread_compound_method=self.spread_compound_method
-            ) for i, period in self.schedule.table.to_dict(orient="index").items()
+                spread_compound_method=self.spread_compound_method,
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
         if self.amortization != 0:
             amortization = [
                 Cashflow(
                     self.amortization,
                     self.schedule.pschedule[1 + i],
                     self.currency,
                     "Amortization",
-                ) for i in range(self.schedule.n_periods - 1)
+                )
+                for i in range(self.schedule.n_periods - 1)
             ]
             interleaved_periods = [
                 val for pair in zip(regular_periods, amortization) for val in pair
             ]
             interleaved_periods.append(regular_periods[-1])  # add last regular period
         else:
             interleaved_periods = regular_periods
         self.periods.extend(interleaved_periods)
 
         # final cashflow
-        self.periods.append(Cashflow(
-            self.notional - self.amortization * (self.schedule.n_periods - 1),
-            add_tenor(
-                self.schedule.aschedule[-1],
-                f"{self.payment_lag_exchange}B",
-                None,
-                self.schedule.calendar
-            ),
-            self.currency,
-            "Exchange",
-        ))
+        self.periods.append(
+            Cashflow(
+                self.notional - self.amortization * (self.schedule.n_periods - 1),
+                add_tenor(
+                    self.schedule.aschedule[-1],
+                    f"{self.payment_lag_exchange}B",
+                    None,
+                    self.schedule.calendar,
+                ),
+                self.currency,
+                "Exchange",
+            )
+        )
 
 
 class BaseLegExchangeMtm(BaseLegExchange, metaclass=ABCMeta):
     _do_not_repeat_set_periods = False
     _is_mtm = True
 
     """
@@ -1239,15 +1427,15 @@
         self.alt_currency = alt_currency.lower()
         self.alt_notional = defaults.notional if alt_notional is None else alt_notional
         super().__init__(*args, **kwargs)
         if self.amortization != 0:
             raise ValueError(
                 "`amortization` cannot be supplied to a `FixedLegExchangeMtm` type."
             )
-        self.fx_fixings = fx_fixings  # calls the setter and sets self.periods
+        self.fx_fixings = fx_fixings  # calls the setter
 
     @property
     def notional(self):
         return self._notional
 
     @notional.setter
     def notional(self, value):
@@ -1270,17 +1458,17 @@
             self._fx_fixings = [value]
         else:
             raise TypeError("`fx_fixings` should be scalar value or list of such")
 
         # if self._initialised:
         #     self._set_periods(None)
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def _get_fx_fixings(self, fx):
         """
         Return the calculated FX fixings.
 
         Initialise with the fx fixings already provided statically.
         Use an FXForwards object to determine the additionally required fixings.
@@ -1289,28 +1477,28 @@
 
         Parameters
         ----------
         fx : FXForwards, optional
             The object to derive FX fixings that are not otherwise given in
             ``fx_fixings``.
         """
-        n_given, n_req = len(self.fx_fixings),  self.schedule.n_periods
+        n_given, n_req = len(self.fx_fixings), self.schedule.n_periods
         fx_fixings = self.fx_fixings.copy()
 
         if isinstance(fx, FXForwards):
             for i in range(n_given, n_req):
                 fx_fixings.append(
                     fx.rate(
                         self.alt_currency + self.currency,
                         add_tenor(
                             self.schedule.aschedule[i],
                             f"{self.payment_lag_exchange}B",
                             None,
-                            self.schedule.calendar
-                        )
+                            self.schedule.calendar,
+                        ),
                     )
                 )
         elif n_req > 0:  # only check if unknown fixings are required
             if defaults.no_fx_fixings_for_xcs.lower() == "raise":
                 raise ValueError(
                     "`fx` is required when `fx_fixings` are not pre-set and "
                     "if rateslib option `no_fx_fixings_for_xcs` is set to "
@@ -1318,52 +1506,56 @@
                 )
             if n_given == 0:
                 if defaults.no_fx_fixings_for_xcs.lower() == "warn":
                     warnings.warn(
                         "Using 1.0 for FX, no `fx` or `fx_fixing` given and "
                         "rateslib option `no_fx_fixings_for_xcs` is set to "
                         "'warn'.",
-                        UserWarning
+                        UserWarning,
                     )
                 fx_fixings = [1.0] * n_req
             else:
                 if defaults.no_fx_fixings_for_xcs.lower() == "warn":
                     warnings.warn(
                         "Using final FX fixing given for missing periods, "
                         "rateslib option `no_fx_fixings_for_xcs` is set to "
                         "'warn'.",
-                        UserWarning
+                        UserWarning,
                     )
                 fx_fixings.extend([fx_fixings[-1]] * (n_req - n_given))
         return fx_fixings
 
     @abc.abstractmethod
     def _regular_period(self, *args, **kwargs):
         pass  # pragma: no cover
 
     def _set_periods(self, fx):
         fx_fixings = self._get_fx_fixings(fx)
         self.notional = fx_fixings[0] * self.alt_notional
-        notionals = [
-            self.alt_notional * fx_fixings[i] for i in range(len(fx_fixings))
-        ]
+        notionals = [self.alt_notional * fx_fixings[i] for i in range(len(fx_fixings))]
 
         # initial exchange
-        self.periods = [Cashflow(
-            -self.notional,
-            add_tenor(
-                self.schedule.aschedule[0],
-                f"{self.payment_lag_exchange}B",
-                None,
-                self.schedule.calendar
-            ),
-            self.currency,
-            "Exchange",
-            fx_fixings[0]
-        )] if self.initial_exchange else []
+        self.periods = (
+            [
+                Cashflow(
+                    -self.notional,
+                    add_tenor(
+                        self.schedule.aschedule[0],
+                        f"{self.payment_lag_exchange}B",
+                        None,
+                        self.schedule.calendar,
+                    ),
+                    self.currency,
+                    "Exchange",
+                    fx_fixings[0],
+                )
+            ]
+            if self.initial_exchange
+            else []
+        )
 
         regular_periods = [
             self._regular_period(
                 start=period[defaults.headers["a_acc_start"]],
                 end=period[defaults.headers["a_acc_end"]],
                 payment=period[defaults.headers["payment"]],
                 stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
@@ -1375,40 +1567,43 @@
         mtm_flows = [
             Cashflow(
                 -notionals[i + 1] + notionals[i],
                 add_tenor(
                     self.schedule.aschedule[i + 1],
                     f"{self.payment_lag_exchange}B",
                     None,
-                    self.schedule.calendar
+                    self.schedule.calendar,
                 ),
                 self.currency,
                 "Mtm",
                 fx_fixings[i + 1],
-            ) for i in range(len(fx_fixings) - 1)
+            )
+            for i in range(len(fx_fixings) - 1)
         ]
         interleaved_periods = [
             val for pair in zip(regular_periods, mtm_flows) for val in pair
         ]
         interleaved_periods.append(regular_periods[-1])
         self.periods.extend(interleaved_periods)
 
         # final cashflow
-        self.periods.append(Cashflow(
-            notionals[-1],
-            add_tenor(
-                self.schedule.aschedule[-1],
-                f"{self.payment_lag_exchange}B",
-                None,
-                self.schedule.calendar
-            ),
-            self.currency,
-            "Exchange",
-            fx_fixings[-1],
-        ))
+        self.periods.append(
+            Cashflow(
+                notionals[-1],
+                add_tenor(
+                    self.schedule.aschedule[-1],
+                    f"{self.payment_lag_exchange}B",
+                    None,
+                    self.schedule.calendar,
+                ),
+                self.currency,
+                "Exchange",
+                fx_fixings[-1],
+            )
+        )
 
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
@@ -1438,28 +1633,28 @@
         return ret
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         if not self._do_not_repeat_set_periods:
             self._set_periods(fx)
         ret = super().cashflows(curve, disc_curve, fx, base)
         # self._is_set_periods_fx = False
         return ret
 
     def analytic_delta(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         if not self._do_not_repeat_set_periods:
             self._set_periods(fx)
         ret = super().analytic_delta(curve, disc_curve, fx, base)
         # self._is_set_periods_fx = False
         return ret
 
@@ -1505,37 +1700,38 @@
 
     The final cashflow notional is set as the notional. The payment date is set equal
     to the final period payment date (i.e. the end accrual date plus payment lag).
 
     If ``amortization`` is specified an exchanged notional equivalent to the
     amortization amount is added to the list of periods.
     """
+
     def __init__(
         self,
         *args,
         fixed_rate: Optional[float] = None,
         fx_fixings: Optional[Union[list, float, Dual, Dual2]] = None,
         alt_currency: Optional[str] = None,
         alt_notional: Optional[float] = None,
-        **kwargs
+        **kwargs,
     ):
         self._fixed_rate = fixed_rate
         # self._initialised = False
         super().__init__(
             *args,
             fx_fixings=fx_fixings,
             alt_currency=alt_currency,
             alt_notional=alt_notional,
-            **kwargs
+            **kwargs,
         )
         # self._initialised = True
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def _regular_period(
         self,
         start: datetime,
         end: datetime,
         payment: datetime,
         notional: float,
@@ -1639,43 +1835,45 @@
            currency="eur",
            alt_currency="usd",
            alt_notional=1000000,
        )
        float_leg_exch_mtm.cashflows(curve, None, fxf)
 
     """
+
     def __init__(
         self,
         *args,
         float_spread: Union[float, None] = None,
         fixings: Optional[Union[float, list]] = None,
         fixing_method: Optional[str] = None,
         method_param: Optional[int] = None,
         spread_compound_method: Optional[str] = None,
         fx_fixings: Optional[Union[list, float, Dual, Dual2]] = None,
         alt_currency: Optional[str] = None,
         alt_notional: Optional[float] = None,
-        **kwargs
+        **kwargs,
     ):
         self._float_spread = float_spread
-        self.fixing_method, self.method_param, self.spread_compound_method = \
-            _validate_float_args(fixing_method, method_param, spread_compound_method)
+        (
+            self.fixing_method,
+            self.method_param,
+            self.spread_compound_method,
+        ) = _validate_float_args(fixing_method, method_param, spread_compound_method)
         # self._initialised = False  # flag for not calling fx_fixings in super()
 
         super().__init__(
             *args,
             fx_fixings=fx_fixings,
             alt_currency=alt_currency,
             alt_notional=alt_notional,
-            **kwargs
+            **kwargs,
         )
 
         self._set_fixings(fixings)
-
-        # TODO check the ordering here of the next two lines: periods are not set here but will be at price time
         self.fx_fixings = fx_fixings  # sets fx_fixings and periods after initialising
         # self._initialised = True  # once rates fixings are set can set periods
 
     def _regular_period(
         self,
         start: datetime,
         end: datetime,
@@ -1694,15 +1892,15 @@
             currency=self.currency,
             convention=self.convention,
             termination=self.schedule.termination,
             stub=stub,
             fixings=self.fixings[iterator],
             fixing_method=self.fixing_method,
             method_param=self.method_param,
-            spread_compound_method=self.spread_compound_method
+            spread_compound_method=self.spread_compound_method,
         )
 
 
 class CustomLeg(BaseLeg):
     """
     Create a leg contained of user specified ``Periods``.
 
@@ -1724,18 +1922,22 @@
 
        fp1 = FixedPeriod(dt(2021,1,1), dt(2021,7,1), dt(2021,7,2), "Q", 1e6, "Act365F", fixed_rate=2.10)
        fp2 = FixedPeriod(dt(2021,3,7), dt(2021,9,7), dt(2021,9,8), "Q", -5e6, "Act365F", fixed_rate=3.10)
        custom_leg = CustomLeg(periods=[fp1, fp2])
        custom_leg.cashflows(curve)
 
     """
+
     def __init__(self, periods):
-        if not all(isinstance(p, (FixedPeriod, FloatPeriod, Cashflow)) for p in periods):
+        if not all(
+            isinstance(p, (FixedPeriod, FloatPeriod, Cashflow)) for p in periods
+        ):
             raise ValueError(
                 "Each object in `periods` must be of type {FixedPeriod, FloatPeriod, "
                 "Cashflow}."
             )
         self.periods = periods
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
```

### Comparing `rateslib-0.1.0/rateslib/periods.py` & `rateslib-0.2.0/rateslib/periods.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,28 +21,30 @@
 """
 
 from abc import abstractmethod, ABCMeta
 from datetime import datetime
 from typing import Optional, Union
 import warnings
 
+import numpy as np
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, date_range, Series, NA, isna
 
 from rateslib import defaults
 from rateslib.calendars import add_tenor, get_calendar, dcf
-from rateslib.curves import Curve, LineCurve
-from rateslib.dual import Dual, Dual2
+from rateslib.curves import Curve, LineCurve, IndexCurve
+from rateslib.dual import Dual, Dual2, DualTypes
 from rateslib.fx import FXForwards, FXRates
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _get_fx_and_base(
     currency: str,
     fx: Optional[Union[float, FXRates, FXForwards]] = None,
     base: Optional[str] = None,
 ):
     if isinstance(fx, (FXRates, FXForwards)):
         base = fx.base if base is None else base.lower()
@@ -112,29 +114,31 @@
         self.currency = defaults.base_currency if currency is None else currency.lower()
         self.convention = defaults.convention if convention is None else convention
         self.termination = termination
         self.freq_months = defaults.frequency_months[self.frequency]
         self.stub = stub
 
     def __repr__(self):
-        return f"<{type(self).__name__}: {self.start.strftime('%Y-%m-%d')}->" \
-               f"{self.end.strftime('%Y-%m-%d')},{self.notional},{self.convention}>"
+        return (
+            f"<{type(self).__name__}: {self.start.strftime('%Y-%m-%d')}->"
+            f"{self.end.strftime('%Y-%m-%d')},{self.notional},{self.convention}>"
+        )
 
     @property
     def dcf(self):
         """
         float : Calculated with appropriate ``convention`` over the period.
         """
         return dcf(
             self.start,
             self.end,
             self.convention,
             self.termination,
             self.freq_months,
-            self.stub
+            self.stub,
         )
 
     @abstractmethod
     def analytic_delta(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
@@ -222,25 +226,26 @@
                currency="gbp",
                fixed_rate=4.00,
            )
            period.analytic_delta(curve, curve)
            period.analytic_delta(curve, curve, fxr)
            period.analytic_delta(curve, curve, fxr, "gbp")
         """
-        disc_curve = disc_curve or curve
+        disc_curve_: Curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
-        return fx * self.notional * self.dcf * disc_curve[self.payment] / 10000
+        _ = fx * self.notional * self.dcf * disc_curve_[self.payment] / 10000
+        return _
 
     @abstractmethod
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         """
         Return the properties of the period used in calculating cashflows.
 
         Parameters
         ----------
         curve : Curve, optional
@@ -277,16 +282,17 @@
             defaults.headers["currency"]: self.currency.upper(),
             defaults.headers["a_acc_start"]: self.start,
             defaults.headers["a_acc_end"]: self.end,
             defaults.headers["payment"]: self.payment,
             defaults.headers["convention"]: self.convention,
             defaults.headers["dcf"]: self.dcf,
             defaults.headers["notional"]: float(self.notional),
-            defaults.headers["df"]: None if disc_curve is None else float(
-                disc_curve[self.payment]),
+            defaults.headers["df"]: None
+            if disc_curve is None
+            else float(disc_curve[self.payment]),
         }
 
     @abstractmethod
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
@@ -359,49 +365,50 @@
         return super().analytic_delta(*args, **kwargs)
 
     @property
     def cashflow(self):
         """
         float, Dual or Dual2 : The calculated value from rate, dcf and notional.
         """
-        return None if self.fixed_rate is None \
+        return (
+            None
+            if self.fixed_rate is None
             else -self.notional * self.dcf * self.fixed_rate / 100
+        )
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-        local: bool = False
+        local: bool = False,
     ):
         disc_curve = disc_curve or curve
         if disc_curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
         fx, base = _get_fx_and_base(self.currency, fx, base)
-        value = (
-            self.fixed_rate / 100 * self.dcf * disc_curve[self.payment] * -self.notional
-        )
+        value = self.cashflow * disc_curve[self.payment]
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
         if disc_curve is None or self.fixed_rate is None:
             npv = None
             npv_fx = None
@@ -420,15 +427,15 @@
             defaults.headers["npv_fx"]: npv_fx,
         }
 
 
 def _validate_float_args(
     fixing_method: Optional[str],
     method_param: Optional[int],
-    spread_compound_method: Optional[str]
+    spread_compound_method: Optional[str],
 ):
     """
     Validate the argument input to float periods.
 
     Returns
     -------
     tuple
@@ -446,36 +453,39 @@
         raise ValueError(
             "`fixing_method` must be in {'rfr_payment_delay', "
             "'rfr_observation_shift', 'rfr_lockout', 'rfr_lookback', 'ibor'}, "
             f"got '{fixing_method_}'."
         )
 
     method_param_ = (
-        defaults.fixing_method_param[fixing_method_] if method_param is None
+        defaults.fixing_method_param[fixing_method_]
+        if method_param is None
         else method_param
     )
     if method_param_ != 0 and fixing_method_ == "rfr_payment_delay":
         raise ValueError(
             "`method_param` should not be used (or a value other than 0) when "
             f"using a `fixing_method` of 'rfr_payment_delay', got {method_param_}. "
             f"Configure the `payment_lag` option instead to have the "
             f"appropriate effect."
         )
     elif fixing_method_ == "rfr_lockout" and method_param_ < 1:
         raise ValueError(
             f'`method_param` must be >0 for "rfr_lockout" `fixing_method`, '
-            f'got {method_param_}'
+            f"got {method_param_}"
         )
 
     if spread_compound_method is None:
-        spread_compound_method_:str = defaults.spread_compound_method
+        spread_compound_method_: str = defaults.spread_compound_method
     else:
         spread_compound_method_ = spread_compound_method.lower()
     if spread_compound_method_ not in [
-        "none_simple", "isda_compounding", "isda_flat_compounding"
+        "none_simple",
+        "isda_compounding",
+        "isda_flat_compounding",
     ]:
         raise ValueError(
             "`spread_compound_method` must be in {'none_simple', "
             "'isda_compounding', 'isda_flat_compounding'}, "
             f"got {spread_compound_method_}"
         )
     return fixing_method_, method_param_, spread_compound_method_
@@ -707,74 +717,81 @@
         self,
         *args,
         float_spread: Optional[float] = None,
         fixings: Optional[Union[float, list, Series]] = None,
         fixing_method: Optional[str] = None,
         method_param: Optional[int] = None,
         spread_compound_method: Optional[str] = None,
-        **kwargs
+        **kwargs,
     ):
         self.float_spread = 0 if float_spread is None else float_spread
 
-        self.fixing_method, self.method_param, self.spread_compound_method = \
-            _validate_float_args(fixing_method, method_param, spread_compound_method)
+        (
+            self.fixing_method,
+            self.method_param,
+            self.spread_compound_method,
+        ) = _validate_float_args(fixing_method, method_param, spread_compound_method)
 
         self.fixings = fixings
         if isinstance(self.fixings, list) and self.fixing_method == "ibor":
             raise ValueError(
                 "`fixings` can only be a single value, not list, under 'ibor' method."
             )
 
         # self.calendar = get_calendar(calendar)
         # self.modifier = modifier
         super().__init__(*args, **kwargs)
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def analytic_delta(
         self,
-        curve: Curve,
+        curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
     ):
         if self.spread_compound_method == "none_simple" or self.float_spread == 0:
             # then analytic_delta is not impacted by float_spread compounding
             dr_dz = 1.0
-
-        else:
+        elif isinstance(curve, Curve):
             _ = self.float_spread
             DualType = Dual if curve.ad in [0, 1] else Dual2
             self.float_spread = DualType(float(_), "z_float_spread")
             rate = self.rate(curve)
             dr_dz = rate.gradient("z_float_spread")[0] * 100
             self.float_spread = _
+        else:
+            raise TypeError(
+                "`curve` must be supplied for given `spread_compound_method`"
+            )
 
         return dr_dz * super().analytic_delta(curve, disc_curve, fx, base)
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ):
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
         rate = None if curve is None else float(self.rate(curve))
         if disc_curve is None or rate is None:
             npv, npv_fx = None, None
         else:
             npv = float(self.npv(curve, disc_curve))
             npv_fx = npv * float(fx)
-        cashflow = None if rate is None else -float(
-            self.notional * self.dcf * rate / 100)
+        cashflow = (
+            None if rate is None else -float(self.notional * self.dcf * rate / 100)
+        )
 
         return {
             **super().cashflows(curve, disc_curve, fx, base),
             defaults.headers["rate"]: rate,
             defaults.headers["spread"]: float(self.float_spread),
             defaults.headers["cashflow"]: cashflow,
             defaults.headers["npv"]: npv,
@@ -791,17 +808,23 @@
         local: bool = False,
     ):
         disc_curve = disc_curve or curve
         if disc_curve is None or curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
+        if self.payment < disc_curve.node_dates[0]:
+            return 0.0  # payment date is in the past avoid issues with fixings or rates
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = (
-            self.rate(curve)/100 * self.dcf * disc_curve[self.payment] * -self.notional
+            self.rate(curve)
+            / 100
+            * self.dcf
+            * disc_curve[self.payment]
+            * -self.notional
         )
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
     def rate(self, curve: Union[Curve, LineCurve]):
@@ -821,21 +844,27 @@
         --------
         .. ipython:: python
 
            period.rate(curve)
         """
         if isinstance(self.fixings, (float, Dual, Dual2)):
             # if fixings is a single value then return that value (curve unused)
-            if self.spread_compound_method in [
-                "isda_compounding", "isda_flat_compounding"
-            ] and self.float_spread != 0 and "rfr" in self.fixing_method:
-                warnings.warn("Unless the RFR period is a 1-day tenor, "
-                              "a single scalar fixing will not be compounded correctly"
-                              "with the given `spread_compound_method`, and "
-                              "`float_spread`", UserWarning)
+            if (
+                self.spread_compound_method
+                in ["isda_compounding", "isda_flat_compounding"]
+                and self.float_spread != 0
+                and "rfr" in self.fixing_method
+            ):
+                warnings.warn(
+                    "Unless the RFR period is a 1-day tenor, "
+                    "a single scalar fixing will not be compounded correctly"
+                    "with the given `spread_compound_method`, and "
+                    "`float_spread`",
+                    UserWarning,
+                )
 
             # this ignores spread_compound_type
             return self.fixings + self.float_spread / 100
         # else next calculations made based on fixings in (None, list, Series)
 
         if type(curve) is Curve:
             if "rfr" in self.fixing_method:
@@ -896,17 +925,17 @@
                 pass
         return curve[fixing_date] + self.float_spread / 100
 
     def _rfr_rate_from_line_curve(self, curve: LineCurve):
         return self._rfr_fixings_array(curve, fixing_exposure=False)[0]
 
     def _rfr_fixings_array(
-            self,
-            curve: Union[Curve, LineCurve],
-            fixing_exposure: bool = False,
+        self,
+        curve: Union[Curve, LineCurve],
+        fixing_exposure: bool = False,
     ):
         """
         Calculate the rate of a period via extraction and combination of every fixing.
 
         This method of calculation is used when either:
 
         - known fixings needs to be combined with unknown fixings,
@@ -938,117 +967,131 @@
         elif self.fixing_method == "rfr_observation_shift":
             start_obs = add_tenor(
                 self.start, f"-{self.method_param}b", "P", curve.calendar
             )
             end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
             start_dcf, end_dcf = start_obs, end_obs
         elif self.fixing_method == "rfr_lookback":
-            start_obs = add_tenor(self.start, f"-{self.method_param}b", "P",
-                                  curve.calendar)
+            start_obs = add_tenor(
+                self.start, f"-{self.method_param}b", "P", curve.calendar
+            )
             end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
             start_dcf, end_dcf = self.start, self.end
         else:
             raise NotImplementedError(
                 "`fixing_method` should be in {'rfr_payment_delay', 'rfr_lockout', "
                 "'rfr_lookback', 'rfr_observation_shift'}"
             )
 
-        obs_dates = Series(date_range(  # dates of the fixing observation period
-            start=start_obs,
-            end=end_obs,
-            freq=curve.calendar
-        ))
-        dcf_dates = Series(date_range(  # dates for the dcf weights period
-            start=start_dcf,
-            end=end_dcf,
-            freq=curve.calendar
-        ))
+        obs_dates = Series(
+            date_range(  # dates of the fixing observation period
+                start=start_obs, end=end_obs, freq=curve.calendar
+            )
+        )
+        dcf_dates = Series(
+            date_range(  # dates for the dcf weights period
+                start=start_dcf, end=end_dcf, freq=curve.calendar
+            )
+        )
         if len(dcf_dates) != len(obs_dates):
             # this should never be true since dates should be adjusted under the
             # curve calendar which is consistent in all above execution statements.
             raise ValueError(  # pragma: no cover
                 "Observation and dcf dates do not align, possible `calendar` issue."
             )
 
-        dcf_vals = Series([  # calculate the dcf values from the dcf dates
-            dcf(dcf_dates[i], dcf_dates[i + 1], curve.convention)
-            for i in range(len(dcf_dates.index) - 1)
-        ])
+        dcf_vals = Series(
+            [  # calculate the dcf values from the dcf dates
+                dcf(dcf_dates[i], dcf_dates[i + 1], curve.convention)
+                for i in range(len(dcf_dates.index) - 1)
+            ]
+        )
 
         rates = Series(NA, index=obs_dates[:-1])
         if self.fixings is not None:
             # then fixings will be a list or Series, scalars are already processed.
             if isinstance(self.fixings, list):
-                rates.iloc[:len(self.fixings)] = self.fixings
+                rates.iloc[: len(self.fixings)] = self.fixings
             elif isinstance(self.fixings, Series):
                 if not self.fixings.index.is_monotonic_increasing:
                     raise ValueError(
                         "`fixings` as a Series must have a monotonically increasing "
                         "datetimeindex."
                     )
-                fixing_rates = self.fixings.loc[obs_dates.iloc[0]:obs_dates.iloc[-2]]
+                fixing_rates = self.fixings.loc[obs_dates.iloc[0] : obs_dates.iloc[-2]]  # type: ignore[misc]
                 rates.loc[fixing_rates.index] = fixing_rates
 
                 # basic error checking for missing fixings and provide warning.
                 try:
                     first_forecast_date = rates[isna(rates)].index[0]
                     if rates[~isna(rates)].index[-1] > first_forecast_date:
                         # then a missing fixing exists
-                        warnings.warn(f"`fixings` has missed a calendar value "
-                                      f"({first_forecast_date}) which "
-                                      "has been inferred from the curve. Subsequent "
-                                      "fixings have been detected", UserWarning)
+                        warnings.warn(
+                            f"`fixings` has missed a calendar value "
+                            f"({first_forecast_date}) which "
+                            "has been inferred from the curve. Subsequent "
+                            "fixings have been detected",
+                            UserWarning,
+                        )
                 except (KeyError, IndexError):
                     pass
             else:
                 raise TypeError(  # pragma: no cover
                     "`fixings` should be of type scalar, None, list or Series."
                 )
 
-        # TODO document the difference between LineCurves for RFR and IBOR where an
-        # IBOR curve should return rates by publication date and RFR curves should
-        # return rates by reference value date.
-
         # reindex the rates series getting missing values from the curves
-        rates = Series({
-            k: curve.rate(k, "1b") if isna(v) else v for k, v in rates.items()
-        })
+        rates = Series(
+            {k: curve.rate(k, "1b") if isna(v) else v for k, v in rates.items()}
+        )
 
         if fixing_exposure:
             # need to calculate the dcfs associated with the rates (unshifted)
             if self.fixing_method in [
-                "rfr_payment_delay", "rfr_observation_shift", "rfr_lockout"
+                "rfr_payment_delay",
+                "rfr_observation_shift",
+                "rfr_lockout",
             ]:  # for all these methods there is no shift
                 dcf_of_r = dcf_vals.copy()
             elif self.fixing_method == "rfr_lookback":
-                dcf_of_r = Series([
-                    dcf(obs_dates[i], obs_dates[i + 1], curve.convention)
-                    for i in range(len(dcf_dates.index) - 1)
-                ])
+                dcf_of_r = Series(
+                    [
+                        dcf(obs_dates[i], obs_dates[i + 1], curve.convention)
+                        for i in range(len(dcf_dates.index) - 1)
+                    ]
+                )
 
         if self.fixing_method == "rfr_lockout":
             # adjust the final rates values of the lockout arrays according to param
             try:
-                rates.iloc[-self.method_param:] = rates.iloc[-self.method_param - 1]
+                rates.iloc[-self.method_param :] = rates.iloc[-self.method_param - 1]
             except IndexError:
                 raise ValueError(
                     "period has too few dates for `rfr_lockout` param to function."
                 )
 
         if fixing_exposure:
-            rates_dual = Series([
-                Dual(float(r), f"fixing_{i}") for i, (k, r) in enumerate(rates.items())
-            ], index=rates.index)
+            rates_dual = Series(
+                [
+                    Dual(float(r), f"fixing_{i}")
+                    for i, (k, r) in enumerate(rates.items())
+                ],
+                index=rates.index,
+            )
             if self.fixing_method == "rfr_lockout":
-                rates_dual.iloc[-self.method_param:] = \
-                    rates_dual.iloc[-self.method_param - 1]
+                rates_dual.iloc[-self.method_param :] = rates_dual.iloc[
+                    -self.method_param - 1
+                ]
             rate = self._isda_compounded_rate_with_spread(rates_dual, dcf_vals)
-            notional_exposure = Series([
-                rate.gradient(f"fixing_{i}")[0] for i in range(len(dcf_dates.index)-1)
-            ])
+            notional_exposure = Series(
+                [
+                    rate.gradient(f"fixing_{i}")[0]
+                    for i in range(len(dcf_dates.index) - 1)
+                ]
+            )
             notional_exposure *= -self.notional * self.dcf / dcf_of_r
             extra_cols = {
                 "obs_dcf": dcf_of_r,
                 "notional": notional_exposure.apply(float, convert_dtype=float),
             }
         else:
             rate = self._isda_compounded_rate_with_spread(rates, dcf_vals)
@@ -1057,21 +1100,23 @@
         if rates.isna().any():
             raise ValueError(
                 "RFRs could not be calculated, have you missed providing `fixings` or "
                 "does the `Curve` begin after the start of a `FloatPeriod` including"
                 "the `method_param` adjustment?"
             )
 
-        return rate, DataFrame({
-            "obs_dates": obs_dates,
-            "dcf_dates": dcf_dates,
-            "dcf": dcf_vals,
-            "rates": rates.apply(float, convert_dtype=float).reset_index(drop=True),
-            **extra_cols
-        })
+        return rate, DataFrame(
+            {
+                "obs_dates": obs_dates,
+                "dcf_dates": dcf_dates,
+                "dcf": dcf_vals,
+                "rates": rates.apply(float, convert_dtype=float).reset_index(drop=True),
+                **extra_cols,
+            }
+        )
 
     def _isda_compounded_rate_with_spread(self, rates, dcf_vals):
         """
         Calculate all in rates with float spread under different compounding methods.
 
         Parameters
         ----------
@@ -1083,40 +1128,39 @@
         Returns
         -------
         float, Dual, Dual2
         """
         dcf_vals = dcf_vals.set_axis(rates.index)
         if self.float_spread == 0 or self.spread_compound_method == "none_simple":
             return (
-                ((1 + dcf_vals * rates / 100).prod() - 1) * 100
-                / dcf_vals.sum()
-                + self.float_spread / 100
-            )
+                (1 + dcf_vals * rates / 100).prod() - 1
+            ) * 100 / dcf_vals.sum() + self.float_spread / 100
         elif self.spread_compound_method == "isda_compounding":
             return (
                 ((1 + dcf_vals * (rates / 100 + self.float_spread / 10000)).prod() - 1)
-                * 100 / dcf_vals.sum()
+                * 100
+                / dcf_vals.sum()
             )
         elif self.spread_compound_method == "isda_flat_compounding":
             sub_cashflows = (rates / 100 + self.float_spread / 10000) * dcf_vals
             for i in range(1, len(sub_cashflows)):
-                k, k_ = rates.index[i], rates.index[i-1]
+                k, k_ = rates.index[i], rates.index[i - 1]
                 sub_cashflows[k] += sub_cashflows[k_] * rates[k] / 100 * dcf_vals[k]
             total_cashflow = sub_cashflows.sum()
             return total_cashflow * 100 / dcf_vals.sum()
         else:
             # this path not generally hit due to validation at initialisation
             raise ValueError(
                 "`spread_compound_method` must be in {'none_simple', "
                 "'isda_compounding', 'isda_flat_compounding'}."
             )
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     @property
     def _is_complex(self):
         """
         A complex float leg is one which is RFR based and for which each individual
         RFR fixing is required is order to calculate correctly. This occurs in the
         following cases:
@@ -1130,16 +1174,15 @@
            efficient by splitting calculations into two parts. As of now it
            remains within the inefficient section.
         4) ``fixings`` are given which need to be incorporated into the calculation
         """
         if self.fixing_method in ["rfr_payment_delay", "rfr_observation_shift"]:
             if self.fixings is not None:
                 return True
-            elif self.float_spread == 0 or \
-                    self.spread_compound_method == "none_simple":
+            elif self.float_spread == 0 or self.spread_compound_method == "none_simple":
                 return False
             else:
                 return True
         elif self.fixing_method == "ibor":
             return False
         return True
 
@@ -1253,25 +1296,29 @@
                "method_param": 2,
             })
            period.fixings_table(ibor_curve)
         """
         if "rfr" in self.fixing_method:
             rate, table = self._rfr_fixings_array(curve, fixing_exposure=True)
             table = table.iloc[:-1]
-            return table[["obs_dates", "notional", "dcf", "rates"]].set_index("obs_dates")
+            return table[["obs_dates", "notional", "dcf", "rates"]].set_index(
+                "obs_dates"
+            )
         elif "ibor" in self.fixing_method:
             fixing_date = add_tenor(
                 self.start, f"-{self.method_param}b", "P", curve.calendar
             )
-            return DataFrame({
-                "obs_dates": [fixing_date],
-                "notional": -self.notional,
-                "dcf": [None],
-                "rates": [self.rate(curve)],
-            }).set_index("obs_dates")
+            return DataFrame(
+                {
+                    "obs_dates": [fixing_date],
+                    "notional": -self.notional,
+                    "dcf": [None],
+                    "rates": [self.rate(curve)],
+                }
+            ).set_index("obs_dates")
 
 
 class Cashflow:
     """
     Create a single cashflow amount on a payment date (effectively a CustomPeriod).
 
     Parameters
@@ -1288,15 +1335,14 @@
         An associated rate to relate to the cashflow, e.g. an FX fixing.
 
     Attributes
     ----------
     notional : float
     payment : Datetime
     stub_type : str
-    rate : float
 
     Notes
     -----
     Other common :class:`BasePeriod` parameters not required for single cashflows are
     set to *None*.
     """
 
@@ -1307,15 +1353,21 @@
         currency: Optional[str] = None,
         stub_type: Optional[str] = None,
         rate: Optional[float] = None,
     ):
         self.notional, self.payment = notional, payment
         self.currency = defaults.base_currency if currency is None else currency.lower()
         self.stub_type = stub_type
-        self.rate = rate if rate is None else float(rate)
+        self.rate_ = rate if rate is None else float(rate)
+
+    def rate(self):
+        """
+        The rate of the cashflow (nominal only - not used in calculations)
+        """
+        return self.rate_
 
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
@@ -1323,51 +1375,57 @@
     ):
         disc_curve = disc_curve or curve
         if disc_curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
         fx, base = _get_fx_and_base(self.currency, fx, base)
-        value = (self.cashflow * disc_curve[self.payment])
+        value = self.cashflow * disc_curve[self.payment]
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None
+        base: Optional[str] = None,
     ) -> dict:
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
         if disc_curve is None:
             npv, npv_fx = None, None
         else:
             npv = float(self.npv(curve, disc_curve))
             npv_fx = npv * float(fx)
 
+        try:
+            cashflow_ = float(self.cashflow)
+        except TypeError:  # cashflow in superclass not a property
+            cashflow_ = None
+
         return {
             defaults.headers["type"]: type(self).__name__,
             defaults.headers["stub_type"]: self.stub_type,
             defaults.headers["currency"]: self.currency.upper(),
             defaults.headers["a_acc_start"]: None,
             defaults.headers["a_acc_end"]: None,
             defaults.headers["payment"]: self.payment,
             defaults.headers["convention"]: None,
             defaults.headers["dcf"]: None,
             defaults.headers["notional"]: float(self.notional),
-            defaults.headers["df"]: None if disc_curve is None else float(
-                disc_curve[self.payment]),
-            defaults.headers["rate"]: self.rate,
+            defaults.headers["df"]: None
+            if disc_curve is None
+            else float(disc_curve[self.payment]),
+            defaults.headers["rate"]: self.rate(),
             defaults.headers["spread"]: None,
-            defaults.headers["cashflow"]: float(self.cashflow),
+            defaults.headers["cashflow"]: cashflow_,
             defaults.headers["npv"]: npv,
             defaults.headers["fx"]: float(fx),
             defaults.headers["npv_fx"]: npv_fx,
         }
 
     @property
     def cashflow(self):
@@ -1378,10 +1436,259 @@
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
         return 0
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+
+
+class IndexMixin(metaclass=ABCMeta):
+    index_base: float = 0.0
+    index_method: str = ""
+    index_fixings: Optional[Union[float, Series]] = None
+    payment: datetime = datetime(1990, 1, 1)
+    currency: str = ""
+
+    def cashflow(self, curve: Optional[IndexCurve] = None) -> Optional[DualTypes]:
+        """
+        float, Dual or Dual2 : The calculated value from rate, dcf and notional,
+        adjusted for the index.
+        """
+        if self.real_cashflow is None:
+            return None
+        if self.rate(curve) is None:
+            return None
+        _ = self.real_cashflow * self.rate(curve) / self.index_base
+        return _
+
+    def rate(self, curve: Optional[IndexCurve] = None) -> Optional[DualTypes]:
+        """
+        Project an index rate for the cashflow payment date.
+
+        Parameters
+        ----------
+        curve : IndexCurve
+
+        Returns
+        -------
+        float, Dual, Dual2
+        """
+        if self.index_fixings is None:
+            if curve is None:
+                return None
+            # forecast inflation index from curve
+            return curve.index_value(self.payment, self.index_method)
+        else:
+            if isinstance(self.index_fixings, Series):
+                if self.index_method == "daily":
+                    adj_date = self.payment
+                else:  # index_method == "monthly"
+                    adj_date = datetime(self.payment.year, self.payment.month, 1)
+
+                try:
+                    return self.index_fixings[adj_date]
+                except KeyError:
+                    s = self.index_fixings.copy()
+                    s.loc[adj_date] = np.NaN  # type: ignore[call-overload]
+                    return s.sort_index().interpolate("linear")[adj_date]
+            else:
+                return self.index_fixings
+
+    def npv(
+        self,
+        curve: IndexCurve,
+        disc_curve: Optional[Curve] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        local: bool = False,
+    ):
+        disc_curve = disc_curve or curve
+        if disc_curve is None:
+            raise TypeError(
+                "`curves` have not been supplied correctly. NoneType has been detected."
+            )
+        fx, base = _get_fx_and_base(self.currency, fx, base)
+        value = self.cashflow(curve) * disc_curve[self.payment]
+        if local:
+            return {self.currency: value}
+        else:
+            return fx * value
+
+    @property
+    @abstractmethod
+    def real_cashflow(self):
+        pass  # pragma: no cover
+
+
+class IndexFixedPeriod(IndexMixin, FixedPeriod):  # type: ignore[misc]
+    """
+    Create a period defined with a real rate adjusted by an index.
+
+    When used with inflation products this defines a real coupon period with a
+    cashflow adjusted upwards by the inflation index.
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`FixedPeriod`.
+    index_base : float or None, optional
+        The base index to determine the cashflow.
+    index_fixings : float, or Series, optional
+        If a float scalar, will be applied as the index fixing for the whole
+        period. If a datetime indexed ``Series`` will use the
+        fixings that are available in that object, and derive the rest from the
+        ``curve``.
+    index_method : str
+        Whether the indexing uses a daily measure for settlement or the most recently
+        monthly data taken from the first day of month.
+    kwargs : dict
+        Required keyword arguments to :class:`FixedPeriod`.
+    """
+
+    def __init__(
+        self,
+        *args,
+        index_base: float,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: str = "daily",
+        **kwargs,
+    ):
+        self.index_base = index_base
+        self.index_fixings = index_fixings
+        self.index_method = index_method.lower()
+        if self.index_method not in ["daily", "monthly"]:
+            raise ValueError("`index_method` must be in {'daily', 'monthly'}.")
+        super(IndexMixin, self).__init__(*args, **kwargs)
+
+    def analytic_delta(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Union[float, FXRates, FXForwards] = 1.0,
+        base: Optional[str] = None,
+    ):
+        real_a_delta = super().analytic_delta(curve, disc_curve, fx, base)
+        _ = real_a_delta * self.rate(curve) / self.index_base
+        return _
+
+    @property
+    def real_cashflow(self):
+        """
+        float, Dual or Dual2 : The calculated real value from rate, dcf and notional.
+        """
+        return (
+            None
+            if self.fixed_rate is None
+            else -self.notional * self.dcf * self.fixed_rate / 100
+        )
+
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere
+
+    def cashflows(
+        self,
+        curve: Optional[IndexCurve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+    ):
+        disc_curve = disc_curve or curve
+        fx, base = _get_fx_and_base(self.currency, fx, base)
+
+        if disc_curve is None or self.fixed_rate is None:
+            npv = None
+            npv_fx = None
+        else:
+            npv = float(self.npv(curve, disc_curve))
+            npv_fx = npv * float(fx)
+
+        cashflow_ = self.cashflow(curve)
+        cashflow_ = None if cashflow_ is None else float(cashflow_)
+
+        index_ = self.rate(curve)
+        if index_ is None:
+            index_ratio_ = None
+        else:
+            index_ratio_ = index_ /self.index_base
+
+        return {
+            **super(FixedPeriod, self).cashflows(curve, disc_curve, fx, base),
+            defaults.headers["rate"]: self.fixed_rate,
+            defaults.headers["spread"]: None,
+            defaults.headers["real_cashflow"]: self.real_cashflow,
+            defaults.headers["index_value"]: index_,
+            defaults.headers["index_ratio"]: index_ratio_,
+            defaults.headers["cashflow"]: cashflow_,
+            defaults.headers["npv"]: npv,
+            defaults.headers["fx"]: float(fx),
+            defaults.headers["npv_fx"]: npv_fx,
+        }
+
+
+class IndexCashflow(IndexMixin, Cashflow):  # type: ignore[misc]
+    """
+    Create a cashflow defined with a real rate adjusted by an index.
+
+    When used with inflation products this defines a real redemption with a
+    cashflow adjusted upwards by the inflation index.
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`Cashflow`.
+    index_base : float or None, optional
+        The base index to determine the cashflow.
+    index_fixings : float, or Series, optional
+        If a float scalar, will be applied as the index fixing for the whole
+        period. If a datetime indexed ``Series`` will use the
+        fixings that are available in that object, and derive the rest from the
+        ``curve``.
+    index_method : str
+        Whether the indexing uses a daily measure for settlement or the most recently
+        monthly data taken from the first day of month.
+    kwargs : dict
+        Required keyword arguments to :class:`Cashflow`.
+    """
+    def __init__(
+        self,
+        *args,
+        index_base: float,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: str = "daily",
+        **kwargs,
+    ):
+        self.index_base = index_base
+        self.index_fixings = index_fixings
+        self.index_method = index_method.lower()
+        super(IndexMixin, self).__init__(*args, **kwargs)
+
+    @property
+    def real_cashflow(self):
+        return -self.notional
+
+    def cashflows(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+    ) -> dict:
+
+        index_ = self.rate(curve)
+        if index_ is None:
+            index_ratio_ = None
+        else:
+            index_ratio_ = index_ / self.index_base
+
+        return {
+            **super(IndexMixin, self).cashflows(curve, disc_curve, fx, base),
+            defaults.headers["real_cashflow"]: self.real_cashflow,
+            defaults.headers["index_value"]: index_,
+            defaults.headers["index_ratio"]: index_ratio_,
+            defaults.headers["cashflow"]: self.cashflow(curve),
+        }
```

### Comparing `rateslib-0.1.0/rateslib/scheduling.py` & `rateslib-0.2.0/rateslib/scheduling.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 )
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 class Schedule:
     """
     Generate a schedule of dates according to a regular pattern and calendar inference.
 
     Parameters
     ----------
     effective : datetime
@@ -223,20 +224,22 @@
         frequency = frequency.upper()
         if frequency not in ["M", "B", "Q", "T", "S", "A", "Z"]:
             raise ValueError("`frequency` must be in {M, B, Q, T, S, A, Z}.")
         self.frequency = frequency
 
         if isinstance(termination, str):
             # if termination is string the end date is calculated as unadjusted
-            termination = add_tenor(effective, termination, None, None)
+            termination_: datetime = add_tenor(effective, termination, None, None)
+        else:
+            termination_ = termination
 
-        if termination <= effective:
+        if termination_ <= effective:
             raise ValueError("`termination` must be after `effective`.")
-        self.effective : datetime = effective
-        self.termination : datetime = termination
+        self.effective: datetime = effective
+        self.termination: datetime = termination_
 
         if frequency == "Z":
             self.ueffective = None
             self.utermination = None
             self.stub = None
             self.front_stub = None
             self.back_stub = None
@@ -259,58 +262,88 @@
             if front_stub is None:
                 if back_stub is None:
                     raise ValueError(
                         "Must supply at least one stub date with dual sided stub type."
                     )
                 else:
                     valid, parsed_args = _infer_stub_date(
-                        effective, termination, frequency, stub, front_stub, back_stub,
-                        self.modifier, eom, roll, self.calendar
+                        effective,
+                        termination_,
+                        frequency,
+                        stub,
+                        front_stub,
+                        back_stub,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         self.ueffective = parsed_args["ueffective"]
                         self.utermination = parsed_args["utermination"]
                         self.front_stub = parsed_args["front_stub"]
                         self.back_stub = parsed_args["back_stub"]
                         self.roll = parsed_args["roll"]
             else:
                 if back_stub is None:
                     valid, parsed_args = _infer_stub_date(
-                        effective, termination, frequency, stub, front_stub, back_stub,
-                        self.modifier, eom, roll, self.calendar
+                        effective,
+                        termination_,
+                        frequency,
+                        stub,
+                        front_stub,
+                        back_stub,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         self.ueffective = parsed_args["ueffective"]
                         self.utermination = parsed_args["utermination"]
                         self.front_stub = parsed_args["front_stub"]
                         self.back_stub = parsed_args["back_stub"]
                         self.roll = parsed_args["roll"]
                 else:
                     # check regular swap and populate attributes
                     valid, parsed_args = _check_regular_swap(
-                        front_stub, back_stub, frequency, self.modifier, eom, roll, self.calendar
+                        front_stub,
+                        back_stub,
+                        frequency,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         self.ueffective = effective
-                        self.utermination = termination
+                        self.utermination = termination_
                         self.front_stub = parsed_args["ueffective"]
                         self.back_stub = parsed_args["utermination"]
                         self.roll = parsed_args["roll"]
         elif "FRONT" in stub:
             if front_stub is None:
                 if back_stub is None:
                     valid, parsed_args = _infer_stub_date(
-                        effective, termination, frequency, stub, front_stub, back_stub,
-                        self.modifier, eom, roll, self.calendar
+                        effective,
+                        termination_,
+                        frequency,
+                        stub,
+                        front_stub,
+                        back_stub,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         self.ueffective = parsed_args["ueffective"]
                         self.utermination = parsed_args["utermination"]
                         self.front_stub = parsed_args["front_stub"]
@@ -318,16 +351,21 @@
                         self.roll = parsed_args["roll"]
                 else:
                     raise ValueError("`stub` is front sided but `back_stub` given.")
             else:
                 if back_stub is None:
                     # check regular swap and populate attibutes
                     valid, parsed_args = _check_regular_swap(
-                        front_stub, termination, frequency, self.modifier, eom, roll,
-                        self.calendar
+                        front_stub,
+                        termination_,
+                        frequency,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         # stub inference is not required, no stubs are necessary
                         self.ueffective = effective
                         self.utermination = parsed_args["utermination"]
@@ -336,55 +374,71 @@
                         self.roll = parsed_args["roll"]
                 else:
                     raise ValueError("`stub` is front sided but `back_stub` given.")
         elif "BACK" in stub:
             if front_stub is None:
                 if back_stub is None:
                     valid, parsed_args = _infer_stub_date(
-                        effective, termination, frequency, stub, front_stub, back_stub,
-                        self.modifier, eom, roll, self.calendar
+                        effective,
+                        termination_,
+                        frequency,
+                        stub,
+                        front_stub,
+                        back_stub,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         self.ueffective = parsed_args["ueffective"]
                         self.utermination = parsed_args["utermination"]
                         self.front_stub = parsed_args["front_stub"]
                         self.back_stub = parsed_args["back_stub"]
                         self.roll = parsed_args["roll"]
                 else:
                     # check regular swap and populate attributes
                     valid, parsed_args = _check_regular_swap(
-                        effective, back_stub, frequency, self.modifier, eom, roll, self.calendar
+                        effective,
+                        back_stub,
+                        frequency,
+                        self.modifier,
+                        eom,
+                        roll,
+                        self.calendar,
                     )
                     if not valid:
                         raise ValueError("date, stub and roll inputs are invalid")
                     else:
                         self.ueffective = parsed_args["ueffective"]
-                        self.utermination = termination
+                        self.utermination = termination_
                         self.front_stub = None
                         self.back_stub = parsed_args["utermination"]
                         self.roll = parsed_args["roll"]
             else:
                 raise ValueError("`stub` is only back sided but `front_stub` given.")
         else:
             raise ValueError(
                 "`stub` should be combinations of {'SHORT', 'LONG'} with "
                 "{'FRONT', 'BACK'}."
             )
 
         self.uschedule = [
-            dt for dt in _generate_irregular_schedule_unadjusted(
+            dt
+            for dt in _generate_irregular_schedule_unadjusted(
                 self.ueffective,
                 self.utermination,
                 self.frequency,
                 self.roll,
                 self.front_stub,
-                self.back_stub
-            )]
+                self.back_stub,
+            )
+        ]
         self._attribute_schedules()
 
         return None
 
     def _attribute_schedules(self):
         """Attributes additional schedules according to date adjust and payment lag."""
         self.aschedule = [
@@ -397,45 +451,52 @@
         self.stubs = [False] * (len(self.uschedule) - 1)
         if self.front_stub is not None:
             self.stubs[0] = True
         if self.back_stub is not None:
             self.stubs[-1] = True
 
     def __repr__(self):
-        str = f"freq: {self.frequency},  stub: {self.stub},  roll: {self.roll}" \
-              f",  pay lag: {self.payment_lag},  modifier: {self.modifier}\n"
+        str = (
+            f"freq: {self.frequency},  stub: {self.stub},  roll: {self.roll}"
+            f",  pay lag: {self.payment_lag},  modifier: {self.modifier}\n"
+        )
         return str + self.table.__repr__()
 
     @property
     def table(self):
         """
         DataFrame : Rows of schedule dates and information.
         """
-        df = DataFrame({
-            defaults.headers["stub_type"]: ["Stub" if _ else "Regular" for _ in self.stubs],
-            defaults.headers["u_acc_start"]: self.uschedule[:-1],
-            defaults.headers["u_acc_end"]: self.uschedule[1:],
-            defaults.headers["a_acc_start"]: self.aschedule[:-1],
-            defaults.headers["a_acc_end"]: self.aschedule[1:],
-            defaults.headers["payment"]: self.pschedule[1:],
-        })
+        df = DataFrame(
+            {
+                defaults.headers["stub_type"]: [
+                    "Stub" if _ else "Regular" for _ in self.stubs
+                ],
+                defaults.headers["u_acc_start"]: self.uschedule[:-1],
+                defaults.headers["u_acc_end"]: self.uschedule[1:],
+                defaults.headers["a_acc_start"]: self.aschedule[:-1],
+                defaults.headers["a_acc_end"]: self.aschedule[1:],
+                defaults.headers["payment"]: self.pschedule[1:],
+            }
+        )
         return df
 
     @property
     def n_periods(self):
         """
         int : Number of periods contained in the schedule.
         """
         return len(self.aschedule[1:])
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _is_divisible_months(date1: datetime, date2: datetime, frequency_months: int):
     """
     Test whether two dates' months define a period divisible by frequency months.
 
     Parameters
     ----------
     date1 : datetime,
@@ -524,14 +585,15 @@
         return non_eom_map[e_cat][t_cat]
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _get_date_category(date: datetime):
     """
     Assign a date to a specific category for roll parsing.
 
     Parameters
     ----------
     date : Datetime
@@ -613,15 +675,15 @@
     """
     frequency_months = defaults.frequency_months[frequency.upper()]
     freq_check = _is_divisible_months(ueffective, utermination, frequency_months)
     if not freq_check:
         return False, "Months date separation not aligned with frequency."
 
     roll = "eom" if roll == 31 else roll
-    for (roll_, _is_roll) in [("eom", _is_eom), ("imm", _is_imm), ("som", _is_som)]:
+    for roll_, _is_roll in [("eom", _is_eom), ("imm", _is_imm), ("som", _is_som)]:
         if str(roll).lower() == roll_:
             if not _is_roll(ueffective):
                 return False, f"Non-{roll_} effective date with {roll_} rolls."
             if not _is_roll(utermination):
                 return False, f"Non-{roll_} termination date with {roll_} rolls."
 
     if isinstance(roll, int):
@@ -657,15 +719,15 @@
 def _check_regular_swap(
     effective: datetime,
     termination: datetime,
     frequency: str,
     modifier: Optional[str],
     eom: bool,
     roll: Optional[Union[str, int]],
-    calendar: Optional[CustomBusinessDay],
+    calendar: CustomBusinessDay,
 ):
     """
     Tests whether the given the parameters define a regular leg schedule without stubs.
 
     Parameters
     ----------
     effective : datetime
@@ -715,38 +777,39 @@
     consistent framework with which to hedge using par tenors so we adopt the second
     in this method.
     """
     _ueffectives = _get_unadjusted_date_alternatives(effective, modifier, calendar)
     _uterminations = _get_unadjusted_date_alternatives(termination, modifier, calendar)
 
     err_str = ""
-    for (_ueff, _uterm) in product(_ueffectives, _uterminations):
+    for _ueff, _uterm in product(_ueffectives, _uterminations):
         ret = _check_unadjusted_regular_swap(_ueff, _uterm, frequency, eom, roll)
         if ret[0]:
             return ret
         else:
             err_str += ret[1] + "\n"
     return False, f"All unadjusted date combinations exhuasted:\n{err_str}"
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _infer_stub_date(
     effective: datetime,
     termination: datetime,
     frequency: str,
     stub: str,
     front_stub: Optional[datetime],
     back_stub: Optional[datetime],
     modifier: Optional[str],
     eom: bool,
     roll: Optional[Union[str, int]],
-    calendar: Optional[CustomBusinessDay],
+    calendar: CustomBusinessDay,
 ) -> tuple[bool, Any]:
     """
     Attempts to infer either a front or back stub in an unspecified schedule.
 
     Parameters
     ----------
     effective : datetime
@@ -784,26 +847,27 @@
       - ``front_stub``: when ``stub`` is front sided only and ``back_stub`` is *None*.
       - ``front_stub``: when ``stub`` is dual sided and ``back_stub`` is specified.
       - ``back_stub``: when ``stub`` is back sided only and ``front_stub`` is *None*.
       - ``back_stub``: when ``stub`` is dual sided and ``front_stub`` is specified.
     """
     if "FRONT" in stub and "BACK" in stub:  # stub is dual sided
         if front_stub is None:
+            assert isinstance(back_stub, datetime)
             valid, parsed_args = _check_regular_swap(
                 effective, back_stub, frequency, modifier, eom, roll, calendar
             )
             if valid:  # no front stub is required
                 return True, {
                     "ueffective": parsed_args["ueffective"],
                     "utermination": termination,
                     "front_stub": None,
                     "back_stub": parsed_args["utermination"],
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
-                    "eom": parsed_args["eom"]
+                    "eom": parsed_args["eom"],
                 }
             else:
                 stub_ = _get_default_stub("FRONT", stub)
                 front_stub = _get_unadjusted_stub_date(
                     effective, back_stub, frequency, stub_, eom, roll
                 )
         else:
@@ -814,15 +878,15 @@
                 return True, {
                     "ueffective": effective,
                     "utermination": parsed_args["utermination"],
                     "front_stub": parsed_args["ueffective"],
                     "back_stub": None,
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
-                    "eom": parsed_args["eom"]
+                    "eom": parsed_args["eom"],
                 }
             else:
                 stub_ = _get_default_stub("BACK", stub)
                 back_stub = _get_unadjusted_stub_date(
                     front_stub, termination, frequency, stub_, eom, roll
                 )
         valid, parsed_args = _check_regular_swap(
@@ -834,29 +898,29 @@
             return True, {
                 "ueffective": effective,
                 "utermination": termination,
                 "front_stub": parsed_args["ueffective"],
                 "back_stub": parsed_args["utermination"],
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
-                "eom": parsed_args["eom"]
+                "eom": parsed_args["eom"],
             }
     elif "FRONT" in stub:
         valid, parsed_args = _check_regular_swap(
             effective, termination, frequency, modifier, eom, roll, calendar
         )
         if valid:  # no front stub is required
             return True, {
                 "ueffective": parsed_args["ueffective"],
                 "utermination": parsed_args["utermination"],
                 "front_stub": None,
                 "back_stub": None,
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
-                "eom": parsed_args["eom"]
+                "eom": parsed_args["eom"],
             }
         else:
             stub_ = _get_default_stub("FRONT", stub)
             front_stub = _get_unadjusted_stub_date(
                 effective, termination, frequency, stub_, eom, roll
             )
             valid, parsed_args = _check_regular_swap(
@@ -868,29 +932,29 @@
                 return True, {
                     "ueffective": effective,
                     "utermination": parsed_args["utermination"],
                     "front_stub": parsed_args["ueffective"],
                     "back_stub": None,
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
-                    "eom": parsed_args["eom"]
+                    "eom": parsed_args["eom"],
                 }
     else:  # schedule is "BACK" sided
         valid, parsed_args = _check_regular_swap(
             effective, termination, frequency, modifier, eom, roll, calendar
         )
         if valid:  # no back stub is required
             return True, {
                 "ueffective": parsed_args["ueffective"],
                 "utermination": parsed_args["utermination"],
                 "front_stub": None,
                 "back_stub": None,
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
-                "eom": parsed_args["eom"]
+                "eom": parsed_args["eom"],
             }
         else:
             stub_ = _get_default_stub("BACK", stub)
             back_stub = _get_unadjusted_stub_date(
                 effective, termination, frequency, stub_, eom, roll
             )
             valid, parsed_args = _check_regular_swap(
@@ -902,15 +966,15 @@
                 return True, {
                     "ueffective": parsed_args["ueffective"],
                     "utermination": termination,
                     "front_stub": None,
                     "back_stub": parsed_args["utermination"],
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
-                    "eom": parsed_args["eom"]
+                    "eom": parsed_args["eom"],
                 }
 
 
 def _get_default_stub(side: str, stub: str) -> str:
     if f"SHORT{side}" in stub:
         return f"SHORT{side}"
     elif f"LONG{side}" in stub:
@@ -958,22 +1022,23 @@
 
     return _get_unadjusted_short_stub_date(
         ueffective,
         utermination,
         frequency,
         "FRONT" if "FRONT" in stub else "BACK",
         eom,
-        roll
+        roll,
     )
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+
 def _get_unadjusted_short_stub_date(
     ueffective: datetime,
     utermination: datetime,
     frequency: str,
     stub_side: str,
     eom: bool,
     roll: Optional[Union[int, str]] = None,
@@ -1005,22 +1070,26 @@
     else:  # stub_side == "BACK":
         stub_side_dt, reg_side_dt, direction = utermination, ueffective, -1
 
     if roll is None:
         roll = "eom" if (eom and _is_eom(reg_side_dt)) else reg_side_dt.day
 
     frequency_months = defaults.frequency_months[frequency]
-    if (_is_divisible_months(ueffective, utermination, frequency_months) and
-        ueffective.day < utermination.day):
+    if (
+        _is_divisible_months(ueffective, utermination, frequency_months)
+        and ueffective.day < utermination.day
+    ):
         if stub_side == "FRONT":
             stub_date = _get_roll(ueffective.month, ueffective.year, roll)
         else:
             stub_date = _get_roll(utermination.month, utermination.year, roll)
-    elif (_is_divisible_months(ueffective, utermination, frequency_months) and
-        ueffective.day >= utermination.day):
+    elif (
+        _is_divisible_months(ueffective, utermination, frequency_months)
+        and ueffective.day >= utermination.day
+    ):
         stub_date = _add_months(stub_side_dt, frequency_months * direction, None, None)
         stub_date = _get_roll(stub_date.month, stub_date.year, roll)
     else:
         for month_offset in range(1, 12):
             stub_date = _add_months(stub_side_dt, month_offset * direction, None, None)
             if _is_divisible_months(stub_date, reg_side_dt, frequency_months):
                 break
@@ -1116,24 +1185,24 @@
         yield _
 
 
 # Utility Functions
 
 
 def _get_unadjusted_date_alternatives(
-    date: datetime, modifier: str, cal: CustomBusinessDay
+    date: datetime, modifier: Optional[str], cal: CustomBusinessDay
 ):
     """
     Return all possible unadjusted dates that result in given date under modifier/cal.
 
     Parameters
     ----------
     date : Datetime
         Date to test.
-    modifier : str
+    modifier : str, optional
         |modifier|
     calendar : Calendar
         |calendar|
 
     Returns
     -------
     list : of valid unadjusted dates
@@ -1197,15 +1266,17 @@
         date = _get_eom(month, year)
     elif roll == "som":
         date = datetime(year, month, 1)
     elif roll == "imm":
         date = _get_imm(month, year)
     else:
         try:
+            assert isinstance(roll, int)
             date = datetime(year, month, roll)
         except ValueError:  # day is out of range for month, i.e. 30 or 31
             date = _get_eom(month, year)
     return date
 
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
```

### Comparing `rateslib-0.1.0/rateslib/solver.py` & `rateslib-0.2.0/rateslib/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from rateslib.fx import FXForwards
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-# TODO: validate solver_id are unique in pre_solver_chain
 class Gradients:
     """
     A catalogue of all the gradients used in optimisation routines and risk
     sensitivties.
     """
 
     @property
@@ -40,15 +39,15 @@
         return self._J
 
     @property
     def grad_v_rT(self):
         """
         Alias of ``J``.
         """
-        return self.J
+        return self.J  # pragma: no cover
 
     @property
     def J2(self):
         """
         3d array of second derivatives of calibrating instrument rates with
         respect to curve variables, of size (n, n, m);
 
@@ -72,15 +71,15 @@
         return self._J2
 
     @property
     def grad_v_v_rT(self):
         """
         Alias of ``J2``.
         """
-        return self.J2
+        return self.J2  # pragma: no cover
 
     @property
     def grad_s_vT(self):
         """
         2d Jacobian array of curve variables with respect to calibrating instruments,
         of size (m, n);
 
@@ -228,15 +227,17 @@
                     f"{self._ad}."
                 )
 
             J2 = np.zeros(shape=(self.pre_n, self.pre_n, self.pre_m))
             i, j = 0, 0
             for pre_slvr in self.pre_solvers:
                 J2[
-                    i : i+pre_slvr.pre_n, i : i+pre_slvr.pre_n, j : j+pre_slvr.pre_m
+                    i : i + pre_slvr.pre_n,
+                    i : i + pre_slvr.pre_n,
+                    j : j + pre_slvr.pre_m,
                 ] = pre_slvr.J2_pre
                 i, j = i + pre_slvr.pre_n, j + pre_slvr.pre_m
 
             rates = np.array([_[0].rate(*_[1], **_[2]) for _ in self.instruments])
             # solver is passed in order to extract curves as string
             _ = np.array([r.gradient(self.pre_variables, order=2) for r in rates])
             J2[:, :, -self.m :] = np.transpose(_, (1, 2, 0))
@@ -254,21 +255,24 @@
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities.
         """
         # FX sensitivity requires reverting through all pre-solvers rates.
-        rates_pre= []
+        rates_pre = []
         for solver in self.pre_solvers:
             rates_pre += [rate for rate in solver.r]
         rates_pre += [rate for rate in self.r]
 
         all_gradients = np.array(
-            [rate.gradient(self.pre_variables + tuple(fx_vars), order=2) for rate in rates_pre]
+            [
+                rate.gradient(self.pre_variables + tuple(fx_vars), order=2)
+                for rate in rates_pre
+            ]
         ).swapaxes(0, 2)
 
         grad_f_v_rT = all_gradients[self.pre_n :, : self.pre_n, :]
         return grad_f_v_rT
 
     def grad_f_f_rT_pre(self, fx_vars):
         """
@@ -315,15 +319,15 @@
         return self._grad_s_s_vT_pre
 
     @property
     def grad_v_v_rT_pre(self):
         """
         Alias of ``J2_pre``.
         """
-        return self.J2_pre
+        return self.J2_pre  # pragma: no cover
 
     def grad_f_s_vT_pre(self, fx_vars):
         """
         3d array of second derivatives of curve variables with respect to
         FX rates and calibrating instrument rates, of size (len(fx_vars), pre_m, pre_n);
 
         .. math::
@@ -332,15 +336,15 @@
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities.
         """
         # FX sensitivity requires reverting through all pre-solvers rates.
-        _ = - np.tensordot(
+        _ = -np.tensordot(
             self.grad_f_v_rT_pre(fx_vars), self.grad_s_vT_pre, (1, 1)
         ).swapaxes(1, 2)
         _ = np.tensordot(_, self.grad_s_vT_pre, (2, 0))
         grad_f_s_vT = _
         return grad_f_s_vT
 
     def grad_f_f_vT_pre(self, fx_vars):
@@ -354,15 +358,15 @@
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities.
         """
         # FX sensitivity requires reverting through all pre-solvers rates.
-        _ = - np.tensordot(self.grad_f_f_rT_pre(fx_vars), self.grad_s_vT_pre, (2, 0))
+        _ = -np.tensordot(self.grad_f_f_rT_pre(fx_vars), self.grad_s_vT_pre, (2, 0))
         _ -= np.tensordot(
             self.grad_f_rT_pre(fx_vars), self.grad_f_s_vT_pre(fx_vars), (1, 1)
         )
         grad_f_f_vT = _
         return grad_f_f_vT
 
     def grad_f_vT_pre(self, fx_vars):
@@ -425,23 +429,23 @@
         if self._grad_s_vT_pre is None:
             grad_s_vT = np.zeros(shape=(self.pre_m, self.pre_n))
 
             i, j = 0, 0
             for pre_solver in self.pre_solvers:
                 # create the left side block matrix
                 m, n = pre_solver.pre_m, pre_solver.pre_n
-                grad_s_vT[i:i+m, j:j+n] = pre_solver.grad_s_vT_pre
+                grad_s_vT[i : i + m, j : j + n] = pre_solver.grad_s_vT_pre
 
                 # create the right column dependencies
                 grad_v_r = np.array(
                     [r.gradient(pre_solver.pre_variables) for r in self.r]
                 ).T
                 block = np.matmul(grad_v_r, self.grad_s_vT)
                 block = -1 * np.matmul(pre_solver.grad_s_vT_pre, block)
-                grad_s_vT[i:i+m, -self.m :] = block
+                grad_s_vT[i : i + m, -self.m :] = block
 
                 i, j = i + m, j + n
 
             # create bottom right block
             grad_s_vT[-self.m :, -self.m :] = self.grad_s_vT
             self._grad_s_vT_pre = grad_s_vT
         return self._grad_s_vT_pre
@@ -456,17 +460,15 @@
            [\\nabla_\mathbf{s} f_{loc:bas}]_{i} = \\frac{\\partial f}{\\partial s_i}
 
         Parameters
         ----------
         f : Dual or Dual2
             The value of the local to base FX conversion rate.
         """
-        _ = np.tensordot(
-            self.grad_s_vT_pre, f.gradient(self.pre_variables), (1, 0)
-        )
+        _ = np.tensordot(self.grad_s_vT_pre, f.gradient(self.pre_variables), (1, 0))
         grad_s_f = _
         return grad_s_f
 
     def grad_s_sT_f_pre(self, f):
         """
         2d array of derivatives of FX conversion rate with respect to
         calibrating instruments, of size (pre_m, pre_m);
@@ -505,15 +507,15 @@
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities
         """
         grad_s_vT = self.grad_s_vT_pre
         grad_v_f = f.gradient(self.pre_variables)
         grad_f_sT_v = self.grad_f_s_vT_pre(fx_vars)
         _ = f.gradient(self.pre_variables + tuple(fx_vars), order=2)
-        grad_v_vT_f = _[: self.pre_n,: self.pre_n]
+        grad_v_vT_f = _[: self.pre_n, : self.pre_n]
         grad_f_vT_f = _[self.pre_n :, : self.pre_n]
         # grad_f_fT_f = _[self.pre_n :, self.pre_n :]
         grad_f_vT = self.grad_f_vT_pre(fx_vars)
 
         _ = np.tensordot(grad_f_sT_v, grad_v_f, (2, 0))
         _ += np.tensordot(grad_f_vT_f, grad_s_vT, (1, 1))
 
@@ -540,15 +542,15 @@
             The variable name tags for the FX rate sensitivities
         """
         # grad_s_vT = self.grad_s_vT_pre
         grad_v_f = f.gradient(self.pre_variables)
         # grad_f_sT_v = self.grad_f_s_vT_pre(fx_vars)
         _ = f.gradient(self.pre_variables + tuple(fx_vars), order=2)
         grad_v_vT_f = _[: self.pre_n, : self.pre_n]
-        grad_f_vT_f = _[self.pre_n:, : self.pre_n]
+        grad_f_vT_f = _[self.pre_n :, : self.pre_n]
         grad_f_fT_f = _[self.pre_n :, self.pre_n :]
         grad_f_vT = self.grad_f_vT_pre(fx_vars)
         grad_f_fT_v = self.grad_f_f_vT_pre(fx_vars)
 
         _ = grad_f_fT_f
         _ += 2.0 * np.tensordot(grad_f_vT_f, grad_f_vT, (1, 1))
         _ += np.tensordot(grad_f_fT_v, grad_v_f, (2, 0))
@@ -712,15 +714,17 @@
             npv : Dual2
                 A local currency NPV of a period of a leg.
             fx_vars : list or tuple of str
                 The variable tags for automatic differentiation of FX rate sensitivity
         """
         # fx_rate-instrument cross gamma:
         _ = np.tensordot(
-            self.grad_f_vT_pre(fx_vars), npv.gradient(self.pre_variables, order=2), (1, 0)
+            self.grad_f_vT_pre(fx_vars),
+            npv.gradient(self.pre_variables, order=2),
+            (1, 0),
         )
         _ += self.gradp_f_vT_Ploc(npv, fx_vars)
         _ = np.tensordot(_, self.grad_s_vT_pre, (1, 1))
         _ += np.tensordot(
             self.grad_f_s_vT_pre(fx_vars), npv.gradient(self.pre_variables), (2, 0)
         )
         grad_f_sT_Ploc = _
@@ -963,17 +967,30 @@
         func_tol: float = 1e-11,
         conv_tol: float = 1e-14,
     ) -> None:
         self.algorithm, self.m = algorithm, len(instruments)
         self.func_tol, self.conv_tol, self.max_iter = func_tol, conv_tol, max_iter
         self.id = id or uuid4().hex[:5] + "_"  # 1 in a million clash
         self.pre_solvers = tuple(pre_solvers)
+
+        # validate `id`s so that DataFrame indexing does not share duplicated keys.
+        if len(set([self.id] + [p.id for p in self.pre_solvers])) < 1 + len(
+            self.pre_solvers
+        ):
+            raise ValueError(
+                "Solver `id`s must be unique when supplying `pre_solvers`, "
+                f"got ids: {[self.id] + [p.id for p in self.pre_solvers]}"
+            )
+
+        # validate `s` and `instruments` with a naive length comparison
         if len(s) != len(instruments):
             raise ValueError("`instrument_rates` must be same length as `instruments`.")
         self.s = np.asarray(s)
+
+        # validate `instrument_labels` if given is same length as `m`
         if instrument_labels is not None:
             if self.m != len(instrument_labels):
                 raise ValueError("`instrument_labels` must have length `instruments`.")
             else:
                 self.instrument_labels = tuple(instrument_labels)
         else:
             self.instrument_labels = tuple(f"{self.id}{i}" for i in range(self.m))
@@ -1017,15 +1034,17 @@
             if curve1.id == curve2.id:
                 raise ValueError(
                     "`curves` must each have their own unique `id`. If using "
                     "pre-solvers as part of a dependency chain a curve can only be "
                     "specified as a variable in one solver."
                 )
         self.pre_variables += self.variables
-        self.pre_instrument_labels += tuple((self.id, lbl) for lbl in self.instrument_labels)
+        self.pre_instrument_labels += tuple(
+            (self.id, lbl) for lbl in self.instrument_labels
+        )
 
         # Final elements
         self._ad = 1
         self.fx = fx
         self.instruments = tuple((self._parse_instrument(inst) for inst in instruments))
         self.rate_scalars = tuple((inst[0]._rate_scalar for inst in self.instruments))
         self.pre_rate_scalars += self.rate_scalars
@@ -1178,26 +1197,26 @@
         """
         s = None
         for pre_solver in self.pre_solvers:
             _ = Series(
                 pre_solver.x.astype(float) * 100 / self.rate_scalars,
                 index=MultiIndex.from_tuples(
                     [(pre_solver.id, inst) for inst in pre_solver.instrument_labels]
-                )
+                ),
             )
             if s is None:
                 s = _
             else:
                 s = concat([s, _])
 
         _ = Series(
             self.x.astype(float) * 100 / self.rate_scalars,
             index=MultiIndex.from_tuples(
                 [(self.id, inst) for inst in self.instrument_labels]
-            )
+            ),
         )
         if s is None:
             s = _
         else:
             s = concat([s, _])
         return s
 
@@ -1247,17 +1266,21 @@
             v_1 = self.v + delta
         # elif algorithm == "gradient_descent_final":
         #     _ = np.matmul(self.Jkm, np.matmul(self.W, self.x[:, np.newaxis]))
         #     y = 2 * np.matmul(self.Jkm.transpose(), _)[:, 0]
         #     alpha = np.dot(y, self.weights * self.x) / np.dot(y, self.weights * y)
         #     v_1 = self.v - 2 * alpha * _[:, 0]
         elif algorithm == "gauss_newton_final":
-            # TODO deal with square and not square matrices here.
-            A = self.J.transpose()
-            b = -self.x[:, np.newaxis]
+            if self.J.shape[0] == self.J.shape[1]:  # square system
+                A = self.J.transpose()
+                b = -self.x[:, np.newaxis]
+            else:
+                A = np.matmul(self.J, np.matmul(self.W, self.J.transpose()))
+                b = -np.matmul(np.matmul(self.J, self.W), self.x[:, np.newaxis])
+
             delta = dual_solve(A, b)[:, 0]
             v_1 = self.v + delta
         else:
             raise NotImplementedError(f"`algorithm`: {algorithm} (spelled correctly?)")
         return v_1
 
     def _update_fx(self):
@@ -1287,15 +1310,17 @@
         self.g_prev, self.g_list, self.lambd = 1e10, [], 1000
         self._reset_properties_()
         self._update_fx()
         t0 = time()
         for i in range(self.max_iter):
             g_val = self.g.real
             self.g_list.append(g_val)
-            # TODO check whether less than or equal to is correct in below condition
+            # condition is set to less than to avoid the case where a null update
+            # results in the same solution and this is erroneously categorised
+            # as a converged solution.
             if (
                 self.g.real < self.g_prev
                 and (self.g_prev - self.g.real) < self.conv_tol
             ):
                 print(
                     f"SUCCESS: `conv_tol` reached after {i} iterations "
                     f"({self.algorithm}), `f_val`: {self.g.real}, "
@@ -1414,48 +1439,52 @@
         fx_scalar = 0.0001
         container = {}
         for ccy in npv:
             container[("instruments", ccy, ccy)] = (
                 self.grad_s_Ploc(npv[ccy]) * inst_scalar
             )
             container[("fx", ccy, ccy)] = (
-                    self.grad_f_Ploc(npv[ccy], fx_vars) * fx_scalar
+                self.grad_f_Ploc(npv[ccy], fx_vars) * fx_scalar
             )
 
             if base is not None and base != ccy:
                 # extend the derivatives
                 f = fx.rate(f"{ccy}{base}")
-                container[("instruments", ccy, base)] = self.grad_s_Pbase(
-                    npv[ccy], container[("instruments", ccy, ccy)] / inst_scalar, f
-                ) * inst_scalar
-                container[("fx", ccy, base)] = self.grad_f_Pbase(
-                    npv[ccy], container[("fx", ccy, ccy)] / fx_scalar, f, fx_vars
-                ) * fx_scalar
+                container[("instruments", ccy, base)] = (
+                    self.grad_s_Pbase(
+                        npv[ccy], container[("instruments", ccy, ccy)] / inst_scalar, f
+                    )
+                    * inst_scalar
+                )
+                container[("fx", ccy, base)] = (
+                    self.grad_f_Pbase(
+                        npv[ccy], container[("fx", ccy, ccy)] / fx_scalar, f, fx_vars
+                    )
+                    * fx_scalar
+                )
 
         # construct the DataFrame from container with hierarchical indexes
         inst_idx = MultiIndex.from_tuples(
             [("instruments",) + label for label in self.pre_instrument_labels],
-            names=["type", "solver", "label"]
+            names=["type", "solver", "label"],
         )
         fx_idx = MultiIndex.from_tuples(
-            [("fx", "fx", f[3:]) for f in fx_vars],
-            names=["type", "solver", "label"]
+            [("fx", "fx", f[3:]) for f in fx_vars], names=["type", "solver", "label"]
         )
-        indexes = {
-            "instruments": inst_idx,
-            "fx": fx_idx
-        }
+        indexes = {"instruments": inst_idx, "fx": fx_idx}
         r_idx = inst_idx.append(fx_idx)
         c_idx = MultiIndex.from_tuples([], names=["local_ccy", "display_ccy"])
         df = DataFrame(None, index=r_idx, columns=c_idx)
         for key, array in container.items():
             df.loc[indexes[key[0]], (key[1], key[2])] = array
 
         if base is not None:
-            df.loc[r_idx, ("all", base)] = df.loc[r_idx, (slice(None), base)].sum(axis=1)
+            df.loc[r_idx, ("all", base)] = df.loc[r_idx, (slice(None), base)].sum(
+                axis=1
+            )
 
         sorted_cols = df.columns.sort_values()
         return df.loc[:, sorted_cols]
 
     def _get_base_and_fx(self, base, fx):
         if base is not None and self.fx is None and fx is None:
             raise ValueError(
@@ -1465,15 +1494,17 @@
         elif fx is None:
             fx = self.fx
         elif fx is not None and self.fx is not None:
             if id(fx) != id(self.fx):
                 warnings.warn(
                     "Solver contains an `fx` attribute but an `fx` argument has been "
                     "supplied which is not the same. This can lead to risk sensitivity "
-                    "inconsistencies, mathematically.", UserWarning)
+                    "inconsistencies, mathematically.",
+                    UserWarning,
+                )
         if base is not None:
             base = base.lower()
         return base, fx
 
     def gamma(self, npv, base=None, fx=None):
         """
         Calculate the cross-gamma risk sensitivity of an instrument's NPV to the
@@ -1532,96 +1563,98 @@
         fx_vars = tuple() if fx is None else fx.variables
 
         inst_scalar = np.array(self.pre_rate_scalars) / 100  # instruments scalar
         fx_scalar = np.ones(len(fx_vars)) * 0.0001
         container = {}
         for ccy in npv:
             container[(ccy, ccy)] = {}
-            container[(ccy, ccy)]["instruments", "instruments"] = (
-                self.grad_s_sT_Ploc(npv[ccy]) *
-                np.matmul(inst_scalar[:, None], inst_scalar[None, :])
-            )
-            container[(ccy, ccy)]["fx", "instruments"] = (
-                self.grad_f_sT_Ploc(npv[ccy], fx_vars) *
-                np.matmul(fx_scalar[:, None], inst_scalar[None, :])
-            )
-            container[(ccy, ccy)]["instruments", "fx"] = (
-                container[(ccy, ccy)][("fx", "instruments")].T
-            )
-            container[(ccy, ccy)]["fx", "fx"] = (
-                self.grad_f_fT_Ploc(npv[ccy], fx_vars) *
-                np.matmul(fx_scalar[:, None], fx_scalar[None, :])
-            )
+            container[(ccy, ccy)]["instruments", "instruments"] = self.grad_s_sT_Ploc(
+                npv[ccy]
+            ) * np.matmul(inst_scalar[:, None], inst_scalar[None, :])
+            container[(ccy, ccy)]["fx", "instruments"] = self.grad_f_sT_Ploc(
+                npv[ccy], fx_vars
+            ) * np.matmul(fx_scalar[:, None], inst_scalar[None, :])
+            container[(ccy, ccy)]["instruments", "fx"] = container[(ccy, ccy)][
+                ("fx", "instruments")
+            ].T
+            container[(ccy, ccy)]["fx", "fx"] = self.grad_f_fT_Ploc(
+                npv[ccy], fx_vars
+            ) * np.matmul(fx_scalar[:, None], fx_scalar[None, :])
 
             if base is not None and base != ccy:
                 # extend the derivatives
                 f = fx.rate(f"{ccy}{base}")
                 container[(ccy, base)] = {}
-                container[(ccy, base)]["instruments", "instruments"] = (
-                        self.grad_s_sT_Pbase(
-                            npv[ccy],
-                            container[(ccy, ccy)]["instruments", "instruments"]
-                            / np.matmul(inst_scalar[:, None], inst_scalar[None, :]),
-                            f
-                        ) * np.matmul(inst_scalar[:, None], inst_scalar[None, :])
-                )
-                # TODO fix the zero arrays
-                container[(ccy, base)]["fx", "instruments"] = (
-                        self.grad_f_sT_Pbase(
-                            npv[ccy],
-                            container[(ccy, ccy)]["fx", "instruments"]
-                            / np.matmul(fx_scalar[:, None], inst_scalar[None, :]),
-                            f,
-                            fx_vars
-                        ) * np.matmul(fx_scalar[:, None], inst_scalar[None, :])
-                )
-                container[(ccy, base)]["instruments", "fx"] = (
-                    container[(ccy, base)][("fx", "instruments")].T
-                )
-                container[(ccy, base)]["fx", "fx"] = (
-                        self.grad_f_fT_Pbase(
-                            npv[ccy],
-                            container[(ccy, ccy)]["fx", "fx"]
-                            / np.matmul(fx_scalar[:, None], fx_scalar[None, :]),
-                            f,
-                            fx_vars
-                        ) * np.matmul(fx_scalar[:, None], fx_scalar[None, :])
+                container[(ccy, base)][
+                    "instruments", "instruments"
+                ] = self.grad_s_sT_Pbase(
+                    npv[ccy],
+                    container[(ccy, ccy)]["instruments", "instruments"]
+                    / np.matmul(inst_scalar[:, None], inst_scalar[None, :]),
+                    f,
+                ) * np.matmul(
+                    inst_scalar[:, None], inst_scalar[None, :]
                 )
+                container[(ccy, base)]["fx", "instruments"] = self.grad_f_sT_Pbase(
+                    npv[ccy],
+                    container[(ccy, ccy)]["fx", "instruments"]
+                    / np.matmul(fx_scalar[:, None], inst_scalar[None, :]),
+                    f,
+                    fx_vars,
+                ) * np.matmul(fx_scalar[:, None], inst_scalar[None, :])
+                container[(ccy, base)]["instruments", "fx"] = container[(ccy, base)][
+                    ("fx", "instruments")
+                ].T
+                container[(ccy, base)]["fx", "fx"] = self.grad_f_fT_Pbase(
+                    npv[ccy],
+                    container[(ccy, ccy)]["fx", "fx"]
+                    / np.matmul(fx_scalar[:, None], fx_scalar[None, :]),
+                    f,
+                    fx_vars,
+                ) * np.matmul(fx_scalar[:, None], fx_scalar[None, :])
 
         # construct the DataFrame from container with hierarchical indexes
         currencies = list(npv.keys())
         local_keys = [(ccy, ccy) for ccy in currencies]
         base_keys = [] if base is None else [(ccy, base) for ccy in currencies]
-        all_keys = sorted(list(set(local_keys+base_keys)))
+        all_keys = sorted(list(set(local_keys + base_keys)))
         inst_keys = [("instruments",) + label for label in self.pre_instrument_labels]
         fx_keys = [("fx", "fx", f[3:]) for f in fx_vars]
-        idx_tuples = [
-            c + l for c in all_keys for l in inst_keys + fx_keys
-        ]
+        idx_tuples = [c + l for c in all_keys for l in inst_keys + fx_keys]
         ridx = MultiIndex.from_tuples(
             [key for key in idx_tuples],
-            names=["local_ccy", "display_ccy", "type", "solver", "label"]
+            names=["local_ccy", "display_ccy", "type", "solver", "label"],
         )
+        if base is not None:
+            ridx = ridx.append(
+                MultiIndex.from_tuples([("all", base) + l for l in inst_keys + fx_keys])
+            )
         cidx = MultiIndex.from_tuples(
-            [l for l in inst_keys + fx_keys],
-            names=["type", "solver", "label"]
+            [l for l in inst_keys + fx_keys], names=["type", "solver", "label"]
         )
         df = DataFrame(None, index=ridx, columns=cidx)
         for key, d in container.items():
-            array = np.block([
-                [d[("instruments", "instruments")], d[("instruments", "fx")]],
-                [d[("fx", "instruments")], d[("fx", "fx")]]
-            ])
+            array = np.block(
+                [
+                    [d[("instruments", "instruments")], d[("instruments", "fx")]],
+                    [d[("fx", "instruments")], d[("fx", "fx")]],
+                ]
+            )
             locator = key + (slice(None), slice(None), slice(None))
             df.loc[locator, :] = array
 
         if base is not None:
-            pass
-            # TODO implement a sum
-            # df.loc[r_idx, ("all", base)] = df.loc[r_idx, (slice(None), base)].sum(axis=1)
+            # sum over all the base rows to aggregate
+            gdf = (
+                df.loc[(currencies, base, slice(None), slice(None), slice(None)), :]
+                .groupby(level=[2, 3, 4])
+                .sum()
+            )
+            gdf.index = MultiIndex.from_tuples([("all", base) + l for l in gdf.index])
+            df.loc[("all", base, slice(None), slice(None), slice(None))] = gdf
 
         return df
 
     def _pnl_explain(self, npv, ds, dfx=None, base=None, fx=None, order=1):
         """
         Calculate PnL from market movements over delta and, optionally, gamma.
```

### Comparing `rateslib-0.1.0/rateslib/splines.py` & `rateslib-0.2.0/rateslib/splines.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,23 +59,27 @@
     ## Right side endpoint support
     org_k = org_k or k  # original_k adds support for derivative recursion
     if x == t[-1] and i >= (len(t) - org_k - 1):
         return 1
 
     ## Recursion
     if k == 1:
-        if t[i] <= x < t[i+1]:
+        if t[i] <= x < t[i + 1]:
             return 1
         return 0
     else:
         left, right = 0, 0
-        if t[i] != t[i+k-1]:
-            left = (x - t[i]) / (t[i+k-1] - t[i]) * bsplev_single(x, i, k-1, t)
-        if t[i+1] != t[i+k]:
-            right = (t[i+k] - x) / (t[i+k] - t[i+1]) * bsplev_single(x, i+1, k-1, t)
+        if t[i] != t[i + k - 1]:
+            left = (x - t[i]) / (t[i + k - 1] - t[i]) * bsplev_single(x, i, k - 1, t)
+        if t[i + 1] != t[i + k]:
+            right = (
+                (t[i + k] - x)
+                / (t[i + k] - t[i + 1])
+                * bsplev_single(x, i + 1, k - 1, t)
+            )
         return left + right
 
 
 def bspldnev_single(x, i, k, t, m, org_k=None):
     """
     Calculate the `m` th order derivative from the right of an indexed b-spline at `x`.
 
@@ -151,15 +155,15 @@
     """
     if m == 0:
         return bsplev_single(x, i, k, t)
     elif k == 1 or m >= k:
         return 0
 
     org_k = org_k or k
-    r, div1, div2 = 0, t[i+k-1] - t[i], t[i+k] - t[i+1]
+    r, div1, div2 = 0, t[i + k - 1] - t[i], t[i + k] - t[i + 1]
     if isinstance(div1, timedelta):
         div1 = div1 / timedelta(days=1)
     if isinstance(div2, timedelta):
         div2 = div2 / timedelta(days=1)
 
     if m == 1:
         if div1 != 0:
@@ -206,17 +210,17 @@
 
     where :math:`B_{i,k,\mathbf{t}}(x)` is one of the *n* b-splines, of order *k* over
     knot sequence :math:`\mathbf{t}`, evaluated at *x*,
     and :math:`c_i` is the coefficient of the *i*'th b-spline for this specific
     piecewise polynomial.
     """
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def __init__(self, k, t, c=None):
         self.t = t
         self.k = k
         self.n = len(t) - k
         self.c = c
 
@@ -233,16 +237,17 @@
             if self.t[i] != other.t[i]:
                 return False
         for attr in ["k", "n"]:
             if getattr(self, attr, None) != getattr(other, attr, None):
                 return False
         if self.c is None and other.c is None:
             return True
-        elif (self.c is None and other.c is not None) or \
-                (self.c is not None and other.c is None):
+        elif (self.c is None and other.c is not None) or (
+            self.c is not None and other.c is None
+        ):
             return False
         elif not all(self.c == other.c):
             return False
         return True
 
     def bsplev(self, x, i, otypes=["float64"]):
         """
@@ -385,17 +390,17 @@
             )
         y = np.asarray(y)
         B_ji = self.bsplmatrix(tau, left_n, right_n)
         c = dual_solve(B_ji, y[:, np.newaxis], allow_lsq=allow_lsq)
         self.c = c[:, 0]
         return None
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def ppev_single(self, x):
         """
         Evaluate a single `x` coordinate on the piecewise polynomial spline.
 
         Parameters
         ----------
```

### Comparing `rateslib-0.1.0/rateslib.egg-info/PKG-INFO` & `rateslib-0.2.0/rateslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
```

### Comparing `rateslib-0.1.0/rateslib.egg-info/SOURCES.txt` & `rateslib-0.2.0/rateslib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 rateslib/__init__.py
 rateslib/calendars.py
 rateslib/curves.py
-rateslib/defaults.py
+rateslib/default.py
 rateslib/dual.py
 rateslib/fx.py
 rateslib/instruments.py
 rateslib/legs.py
 rateslib/periods.py
 rateslib/scheduling.py
 rateslib/solver.py
```

### Comparing `rateslib-0.1.0/tests/test_calendars.py` & `rateslib-0.2.0/tests/test_calendars.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.1.0/tests/test_curves.py` & `rateslib-0.2.0/tests/test_curves.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datetime import datetime as dt
 from pandas import DataFrame
 import numpy as np
 from math import log, exp
 
 import context
-from rateslib.curves import Curve, LineCurve, index_left, interpolate
+from rateslib.curves import Curve, LineCurve, index_left, interpolate, IndexCurve
 from rateslib.dual import Dual, Dual2
 from rateslib.calendars import get_calendar
 
 
 @pytest.fixture()
 def curve():
     return Curve(
@@ -33,14 +33,28 @@
         },
         interpolation="linear",
         id="v",
         ad=1,
     )
 
 
+@pytest.fixture()
+def index_curve():
+    return IndexCurve(
+        nodes={
+            dt(2022, 3, 1): 1.00,
+            dt(2022, 3, 31): 0.999,
+        },
+        interpolation="linear_index",
+        id="v",
+        ad=1,
+        index_base=110.0,
+    )
+
+
 @pytest.mark.parametrize("method", ["flat_forward", "flat_backward"])
 def test_flat_interp(method):
     assert interpolate(1, 1, 5, 2, 10, method) == 5
     assert interpolate(2, 1, 5, 2, 10, method) == 10
     assert interpolate(1.5, 1, 5, 2, 10, "flat_forward") == 5
     assert interpolate(1.5, 1, 5, 2, 10, "flat_backward") == 10
 
@@ -118,23 +132,27 @@
         '"convention": "Act360", "endpoints": ["natural", "natural"], "modifier": "MF", '
         '"calendar_type": "null", "ad": 1, "calendar": null}'
     )
     result = curve.to_json()
     assert result == expected
 
 
-def test_serialization_round_trip(curve, line_curve):
+def test_serialization_round_trip(curve, line_curve, index_curve):
     serial = curve.to_json()
     constructed = Curve.from_json(serial)
     assert constructed == curve
 
     serial = line_curve.to_json()
     constructed = LineCurve.from_json(serial)
     assert constructed == line_curve
 
+    serial = index_curve.to_json()
+    constructed = IndexCurve.from_json(serial)
+    assert constructed == index_curve
+
 
 def test_serialization_round_trip_spline():
     curve = Curve(
         nodes={
             dt(2022, 3, 1): 1.00,
             dt(2022, 3, 31): 0.99,
             dt(2022, 5, 1): 0.98,
@@ -376,15 +394,42 @@
 
 
 def test_index_left_raises():
     with pytest.raises(ValueError, match="`index_left` designed for intervals."):
         index_left([1], 1, 100)
 
 
-def test_curve_shift():
+# def test_curve_shift():
+#     curve = Curve(
+#         nodes={
+#             dt(2022, 1, 1): 1.0,
+#             dt(2023, 1, 1): 0.988,
+#             dt(2024, 1, 1): 0.975,
+#             dt(2025, 1, 1): 0.965,
+#             dt(2026, 1, 1): 0.955,
+#             dt(2027, 1, 1): 0.9475
+#         },
+#         t=[
+#             dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+#             dt(2025, 1, 1),
+#             dt(2026, 1, 1),
+#             dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+#         ],
+#     )
+#     result_curve = curve.shift(25)
+#     diff = np.array([
+#         result_curve.rate(_, "1D") - curve.rate(_, "1D") - 0.25 for _ in [
+#             dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
+#         ]
+#     ])
+#     assert np.all(np.abs(diff) < 1e-7)
+
+
+@pytest.mark.parametrize("ad_order", [0, 1, 2])
+def test_curve_shift_ad_order(ad_order):
     curve = Curve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.988,
             dt(2024, 1, 1): 0.975,
             dt(2025, 1, 1): 0.965,
             dt(2026, 1, 1): 0.955,
@@ -392,25 +437,53 @@
         },
         t=[
             dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
             dt(2025, 1, 1),
             dt(2026, 1, 1),
             dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
         ],
+        ad=ad_order,
     )
     result_curve = curve.shift(25)
     diff = np.array([
         result_curve.rate(_, "1D") - curve.rate(_, "1D") - 0.25 for _ in [
             dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
         ]
     ])
     assert np.all(np.abs(diff) < 1e-7)
 
 
-def test_linecurve_shift():
+def test_curve_shift_dual_input():
+    curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.988,
+            dt(2024, 1, 1): 0.975,
+            dt(2025, 1, 1): 0.965,
+            dt(2026, 1, 1): 0.955,
+            dt(2027, 1, 1): 0.9475
+        },
+        t=[
+            dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+            dt(2025, 1, 1),
+            dt(2026, 1, 1),
+            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+        ],
+    )
+    result_curve = curve.shift(Dual(25, "z"))
+    diff = np.array([
+        result_curve.rate(_, "1D") - curve.rate(_, "1D") - 0.25 for _ in [
+            dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
+        ]
+    ])
+    assert np.all(np.abs(diff) < 1e-7)
+
+
+@pytest.mark.parametrize("ad_order", [0, 1, 2])
+def test_linecurve_shift(ad_order):
     curve = LineCurve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.988,
             dt(2024, 1, 1): 0.975,
             dt(2025, 1, 1): 0.965,
             dt(2026, 1, 1): 0.955,
@@ -418,24 +491,111 @@
         },
         t=[
             dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
             dt(2025, 1, 1),
             dt(2026, 1, 1),
             dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
         ],
+        ad=ad_order
     )
     result_curve = curve.shift(25)
     diff = np.array([
         result_curve[_] - curve[_] - 0.25 for _ in [
             dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
         ]
     ])
     assert np.all(np.abs(diff) < 1e-7)
 
 
+def test_linecurve_shift_dual_input():
+    curve = LineCurve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.988,
+            dt(2024, 1, 1): 0.975,
+            dt(2025, 1, 1): 0.965,
+            dt(2026, 1, 1): 0.955,
+            dt(2027, 1, 1): 0.9475,
+        },
+        t=[
+            dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+            dt(2025, 1, 1),
+            dt(2026, 1, 1),
+            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+        ],
+    )
+    result_curve = curve.shift(Dual(25, "z"))
+    diff = np.array([
+        result_curve[_] - curve[_] - 0.25 for _ in [
+            dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
+        ]
+    ])
+    assert np.all(np.abs(diff) < 1e-7)
+
+
+@pytest.mark.parametrize("ad_order", [0, 1, 2])
+def test_indexcurve_shift(ad_order):
+    curve = IndexCurve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.988,
+            dt(2024, 1, 1): 0.975,
+            dt(2025, 1, 1): 0.965,
+            dt(2026, 1, 1): 0.955,
+            dt(2027, 1, 1): 0.9475,
+        },
+        t=[
+            dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+            dt(2025, 1, 1),
+            dt(2026, 1, 1),
+            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+        ],
+        ad=ad_order,
+        index_base=110.,
+        interpolation="log_linear",
+    )
+    result_curve = curve.shift(25)
+    diff = np.array([
+        result_curve.rate(_, "1D") - curve.rate(_, "1D") - 0.25 for _ in [
+            dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
+        ]
+    ])
+    assert np.all(np.abs(diff) < 1e-7)
+    assert result_curve.index_base == curve.index_base
+
+
+def test_indexcurve_shift_dual_input():
+    curve = IndexCurve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.988,
+            dt(2024, 1, 1): 0.975,
+            dt(2025, 1, 1): 0.965,
+            dt(2026, 1, 1): 0.955,
+            dt(2027, 1, 1): 0.9475,
+        },
+        t=[
+            dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+            dt(2025, 1, 1),
+            dt(2026, 1, 1),
+            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+        ],
+        index_base=110.0,
+        interpolation="log_linear",
+    )
+    result_curve = curve.shift(Dual(25, "z"))
+    diff = np.array([
+        result_curve.rate(_, "1D") - curve.rate(_, "1D") - 0.25 for _ in [
+            dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
+        ]
+    ])
+    assert np.all(np.abs(diff) < 1e-7)
+    assert result_curve.index_base == curve.index_base
+
+
 @pytest.mark.parametrize("crv, t, tol", [
     (Curve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.988,
             dt(2024, 1, 1): 0.975,
             dt(2025, 1, 1): 0.965,
@@ -445,14 +605,31 @@
         t=[
             dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
             dt(2025, 1, 1),
             dt(2026, 1, 1),
             dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
         ],
     ), False, 1e-8),
+    (IndexCurve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.988,
+            dt(2024, 1, 1): 0.975,
+            dt(2025, 1, 1): 0.965,
+            dt(2026, 1, 1): 0.955,
+            dt(2027, 1, 1): 0.9475
+        },
+        t=[
+            dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+            dt(2025, 1, 1),
+            dt(2026, 1, 1),
+            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+        ],
+        index_base=110.,
+    ), False, 1e-8),
     (LineCurve(
         nodes={
             dt(2022, 1, 1): 1.7,
             dt(2023, 1, 1): 1.65,
             dt(2024, 1, 1): 1.4,
             dt(2025, 1, 1): 1.3,
             dt(2026, 1, 1): 1.25,
@@ -488,14 +665,16 @@
     result_curve = crv.translate(dt(2023, 1, 1), t=t)
     diff = np.array([
         result_curve.rate(_, "1D") - crv.rate(_, "1D") for _ in [
             dt(2023, 1, 25), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
         ]
     ])
     assert np.all(np.abs(diff) < tol)
+    if type(crv) is IndexCurve:
+        assert result_curve.index_base == crv.index_value(dt(2023, 1, 1))
 
 
 @pytest.mark.parametrize("crv", [
     Curve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.988,
@@ -576,14 +755,33 @@
            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
         ],
     )
     with pytest.raises(ValueError, match="Cannot translate spline knots for given"):
         curve.translate(dt(2022, 12, 15))
 
 
+def test_curve_index_linear_daily_interp():
+    curve = IndexCurve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2022, 1, 5): 0.9999},
+        index_base=200.0,
+    )
+    result = curve.index_value(dt(2022, 1, 5))
+    expected = 200.020002002
+    assert abs(result - expected) < 1e-7
+
+    result = curve.index_value(dt(2022, 1, 3))
+    expected = 200.010001001  # value is linearly interpolated between index values.
+    assert abs(result - expected) < 1e-7
+
+
+def test_indexcurve_raises():
+    with pytest.raises(ValueError, match="`index_base` must be given"):
+        curve = IndexCurve({dt(2022, 1, 1): 1.0})
+
+
 class TestPlotCurve:
 
     def test_plot_curve(self, curve):
         fig, ax, lines = curve.plot("1d")
         result = lines[0].get_data()
         assert result[0][0] == dt(2022, 3, 1)
         assert abs(result[1][0].real - 12.004001333774994) < 1e-6
```

### Comparing `rateslib-0.1.0/tests/test_dual.py` & `rateslib-0.2.0/tests/test_dual.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,14 +175,38 @@
     assert y_1 != Dual2(1, vars=["v2", "v1"], dual=np.array([1, 2]))
     # non-matching dual2
     assert y_2 != Dual2(
         1, vars=["v0", "v1"], dual=np.array([1, 2]), dual2=np.ones((2, 2)) * 2
     )
 
 
+def test_lt():
+    assert Dual(1, "x") < Dual(2, "y")
+    assert Dual2(1, "z") < Dual2(2, "x")
+    assert Dual(1, "x") < 10
+    assert not Dual(1, "x") < 0
+
+
+def test_lt_raises():
+    with pytest.raises(TypeError, match="Cannot compare"):
+        assert Dual(1, "x") < Dual2(2, "y")
+
+
+def test_gt():
+    assert Dual(2, "x") > Dual(1, "y")
+    assert Dual2(2, "z") > Dual2(1, "x")
+    assert Dual(1, "x") > 0
+    assert not Dual(1, "x") > 10
+
+
+def test_gt_raises():
+    with pytest.raises(TypeError, match="Cannot compare"):
+        assert Dual(2, "x") > Dual2(1, "y")
+
+
 def test_dual2_abs_float(x_1, y_1, y_2):
     assert abs(x_1) == 1
     assert abs(y_1) == 1
     assert abs(y_2) == 1
     assert float(x_1) == float(1)
     assert float(y_1) == float(1)
     assert float(y_2) == float(1)
```

### Comparing `rateslib-0.1.0/tests/test_fx.py` & `rateslib-0.2.0/tests/test_fx.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.1.0/tests/test_instruments.py` & `rateslib-0.2.0/tests/test_instruments.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from pandas.testing import assert_frame_equal
 import numpy as np
 
 import context
 from rateslib import defaults, default_context
 from rateslib.instruments import (
     IRS, forward_fx, SBS, FXSwap, NonMtmXCS, FixedRateBond, Bill, Value,
-    _get_curve_from_solver, BaseMixin, FloatRateBond, FRA,
+    _get_curve_from_solver, BaseMixin, FloatRateBond, FRA, BondFuture,
     NonMtmFixedFloatXCS, NonMtmFixedFixedXCS, XCS, FixedFloatXCS, FixedFixedXCS, FloatFixedXCS,
-    Portfolio, Spread, Fly
+    Portfolio, Spread, Fly, _get_curves_and_fx_maybe_from_solver
 )
 from rateslib.dual import Dual, Dual2
 from rateslib.calendars import dcf
 from rateslib.curves import Curve
 from rateslib.fx import FXRates, FXForwards
 from rateslib.solver import Solver
 
@@ -106,17 +106,16 @@
         }
     )
     solver = Solver(
         [curve], inst, [0.975], fx=fxfs if fxf else None
     ) if solver else None
     curve = curve if crv else None
 
-    a = BaseMixin()
-    crv_result, fx_result = a._get_curves_and_fx_maybe_from_solver(
-        solver, curve, fx
+    crv_result, fx_result = _get_curves_and_fx_maybe_from_solver(
+        None, solver, curve, fx
     )
 
     # check the fx results. If fx is specified directly it is returned
     # otherwsie it is returned from a solver object if it is available.
     if fx is not None:
         assert fx_result == 2.0
     elif solver is None:
@@ -129,38 +128,36 @@
 
     assert crv_result == (curve, curve, curve, curve)
 
 
 def test_get_curves_and_fx_from_solver_raises():
     from rateslib.solver import Solver
 
-    a = BaseMixin()
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
     inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
     solver = Solver([curve], inst, [0.975])
 
     with pytest.raises(ValueError, match="`curves` must contain Curve, not str, if"):
-        a._get_curves_and_fx_maybe_from_solver(None, "tagged", None)
+        _get_curves_and_fx_maybe_from_solver(None, None, "tagged", None)
 
     with pytest.raises(ValueError, match="`curves` must contain str curve `id` s"):
-        a._get_curves_and_fx_maybe_from_solver(solver, "bad_id", None)
+        _get_curves_and_fx_maybe_from_solver(None, solver, "bad_id", None)
 
     with pytest.raises(ValueError, match="Can only supply a maximum of 4 `curves`"):
-        a._get_curves_and_fx_maybe_from_solver(solver, ["tagged"] * 5, None)
+        _get_curves_and_fx_maybe_from_solver(None, solver, ["tagged"] * 5, None)
 
 
 @pytest.mark.parametrize("num", [1, 2, 3, 4])
 def test_get_curves_from_solver_multiply(num):
     from rateslib.solver import Solver
 
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
     inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
     solver = Solver([curve], inst, [0.975])
-    a = BaseMixin()
-    result, _ = a._get_curves_and_fx_maybe_from_solver(solver, ["tagged"] * num, None)
+    result, _ = _get_curves_and_fx_maybe_from_solver(None, solver, ["tagged"] * num, None)
     assert result == (curve, curve, curve, curve)
 
 
 class TestIRS:
 
     @pytest.mark.parametrize("float_spread, fixed_rate, expected", [
         (0, 4.03, 4.03637780),
@@ -278,28 +275,28 @@
             payment_lag=2,
             notional=1e9,
             convention="Act360",
             frequency="Q",
             stub="ShortFront",
         )
         result = irs.npv(curve)
-        assert abs(result) < 1e-9
+        assert abs(result) < 1e-8
 
         irs.fixed_rate = 1.0  # pay fixed low rate implies positive NPV
         assert irs.npv(curve) > 1
 
         irs.fixed_rate = None  # fixed rate set back to initial
-        assert abs(irs.npv(curve)) < 1e-9
+        assert abs(irs.npv(curve)) < 1e-8
 
         irs.fixed_rate = float(irs.rate(curve))
         irs.leg2_float_spread = 100
         assert irs.npv(curve) > 1
 
         irs.leg2_float_spread = None
-        assert abs(irs.npv(curve)) < 1e-9
+        assert abs(irs.npv(curve)) < 1e-8
 
     def test_sbs_float_spread_raises(self, curve):
         irs = IRS(dt(2022, 1, 1), "9M", "Q")
         with pytest.raises(AttributeError, match="Cannot set `float_spread`"):
             irs.float_spread = 1.0
 
 
@@ -1015,14 +1012,24 @@
         bond = FixedRateBond(dt(1997, 1, 1), dt(2004, 11, 26), "S", convention="ActActICMA",
                              fixed_rate=6.75, ex_div=7, calendar="ldn")
         assert bond.ytm(108., dt(1999, 5, 10), True) - 5.7009527 < 1e-6
         assert bond.ytm(108., dt(1999, 5, 17), True) - 5.7253361 < 1e-6
         assert bond.ytm(108., dt(1999, 5, 18), True) - 5.0413308 < 1e-6
         assert bond.ytm(108., dt(1999, 5, 26), True) - 5.0652248 < 1e-6
 
+    def test_fixed_rate_bond_yield_domains(self):
+        bond = FixedRateBond(dt(1995, 1, 1), dt(2015, 12, 7), "S",
+                             convention="ActActICMA",
+                             fixed_rate=8, ex_div=7, calendar="ldn")
+        assert bond.ytm(500., dt(1999, 5, 24), True) + 5.86484231333 < 1e-8
+        assert bond.ytm(200, dt(1999, 5, 24), True) - 1.4366895440550 < 1e-8
+        assert bond.ytm(100, dt(1999, 5, 24), True) - 8.416909601459 < 1e-8
+        assert bond.ytm(50, dt(1999, 5, 24), True) - 18.486840866431 < 1e-6
+        assert bond.ytm(1, dt(1999, 5, 24), True) - 13421775210.82037 < 1e-3
+
     def test_fixed_rate_bond_ytm_duals(self):
         bond = FixedRateBond(dt(1995, 1, 1), dt(2015, 12, 7), "S", convention="ActActICMA",
                              fixed_rate=8, ex_div=7, calendar="ldn")
 
         dPdy = bond.duration(4, dt(1995, 1, 1))
         P = bond.price(4, dt(1995, 1, 1))
         result = bond.ytm(Dual(P, ["a", "b"], [1, -0.5]), dt(1995, 1, 1))
@@ -1114,28 +1121,32 @@
             calendar="ldn",
             currency="gbp",
             convention="ActActICMA",
             ex_div=7,
             fixed_rate=8.0,
             settle=0,
         )
-        curve = Curve({dt(1998, 12, 7): 1.0, dt(2015, 12, 7): 0.50})
-        dirty_price = gilt.rate(curve)
-
-        assert (
-            gilt.rate(curve, metric="clean_price")
-            ==
-            dirty_price - gilt.accrued(dt(1998, 12, 7))
+        curve = Curve({dt(1998, 12, 9): 1.0, dt(2015, 12, 7): 0.50})
+        clean_price = gilt.rate(curve, metric="clean_price")
+        result = gilt.rate(
+            curve, metric="fwd_clean_price", forward_settlement=dt(1998, 12, 9)
         )
+        assert abs(result - clean_price) < 1e-8
 
-        assert (
-            gilt.rate(curve, metric="ytm")
-            ==
-            gilt.ytm(dirty_price, dt(1998, 12, 7), True)
+        result = gilt.rate(curve, metric="dirty_price")
+        expected = clean_price + gilt.accrued(dt(1998, 12, 9))
+        assert result == expected
+        result = gilt.rate(
+            curve, metric="fwd_dirty_price", forward_settlement=dt(1998, 12, 9)
         )
+        assert abs(result - clean_price - gilt.accrued(dt(1998, 12, 9))) < 1e-8
+
+        result = gilt.rate(curve, metric="ytm")
+        expected = gilt.ytm(clean_price, dt(1998, 12, 9), False)
+        assert abs(result - expected) < 1e-8
 
     def test_fixed_rate_bond_npv(self):
         gilt = FixedRateBond(
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
@@ -1152,14 +1163,42 @@
         assert abs(result - expected) < 1e-6
 
         gilt.settle = 1
         result = gilt.npv(curve)  # bond is ex div on settlement 26th Nov 2010
         expected = 109.229489312983  # bond has dropped a coupon payment of 4.
         assert abs(result - expected) < 1e-6
 
+        result = gilt.npv(curve, local=True)
+        assert abs(result["gbp"] - expected) < 1e-6
+
+    def test_fixed_rate_bond_npv_private(self):
+        # this test shadows 'fixed_rate_bond_npv' but extends it for projection
+        curve = Curve({
+            dt(2004, 11, 25): 1.0,
+            dt(2010, 11, 25): 1.0,
+            dt(2015, 12, 7): 0.75}
+        )
+        gilt = FixedRateBond(
+            effective=dt(1998, 12, 7),
+            termination=dt(2015, 12, 7),
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="ActActICMA",
+            ex_div=7,
+            fixed_rate=8.0,
+            notional=-100,
+            settle=0,
+        )
+        result = gilt._npv_local(
+            None, curve, None, None, dt(2010, 11, 26), dt(2010, 11, 25)
+        )
+        expected = 109.229489312983  # npv should match associated test
+        assert abs(result - expected) < 1e-6
+
     def test_fixed_rate_bond_analytic_delta(self):
         gilt = FixedRateBond(
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
             currency="gbp",
@@ -1217,14 +1256,17 @@
             fixed_rate=8.0,
             notional=-100,
         )
         curve = Curve({dt(1998, 12, 7): 1.0, dt(2015, 12, 7): 0.50})
         with pytest.raises(ValueError, match="`metric` must be in"):
             gilt.rate(curve, metric="bad_metric")
 
+        with pytest.raises(ValueError, match="`forward_settlement` needed to"):
+            gilt.rate(curve, metric="fwd_clean_price")
+
     def test_fixed_rate_bond_no_amortization(self):
         with pytest.raises(NotImplementedError, match="`amortization` for"):
             gilt = FixedRateBond(
                 effective=dt(1998, 12, 7),
                 termination=dt(2015, 12, 7),
                 frequency="S",
                 calendar="ldn",
@@ -1232,14 +1274,120 @@
                 convention="ActActICMA",
                 ex_div=7,
                 fixed_rate=8.0,
                 notional=-100,
                 amortization=100
             )
 
+    @pytest.mark.parametrize("f_s, exp", [
+        (dt(2001, 12, 31), 99.997513754),  # compounding of mid year coupon
+        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
+    ])
+    def test_fixed_rate_bond_forward_price_analogue(self, f_s, exp):
+        gilt = FixedRateBond(
+            effective=dt(2001, 1, 1),
+            termination=dt(2002, 1, 1),
+            frequency="S",
+            calendar=None,
+            currency="gbp",
+            convention="Act365f",
+            ex_div=0,
+            fixed_rate=1.0,
+            notional=-100,
+            settle=0,
+        )
+        result = gilt.fwd_from_repo(100.0, dt(2001, 1, 1), f_s, 1.0, "act365f")
+        assert abs(result - exp) < 1e-6
+
+    @pytest.mark.parametrize("f_s, exp", [
+        (dt(2001, 12, 31), 100.49888361793),  # compounding of mid year coupon
+        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
+    ])
+    def test_fixed_rate_bond_forward_price_analogue_dirty(self, f_s, exp):
+        gilt = FixedRateBond(
+            effective=dt(2001, 1, 1),
+            termination=dt(2002, 1, 1),
+            frequency="S",
+            calendar=None,
+            currency="gbp",
+            convention="Act365f",
+            ex_div=0,
+            fixed_rate=1.0,
+            notional=-100,
+            settle=0,
+        )
+        result = gilt.fwd_from_repo(
+            100.0, dt(2001, 1, 1), f_s, 1.0, "act365f", dirty=True
+        )
+        assert abs(result - exp) < 1e-6
+
+    @pytest.mark.parametrize("s, f_s, exp", [
+        (dt(2010, 11, 25), dt(2011, 11, 25), 99.9975000187),
+        (dt(2010, 11, 28), dt(2011, 11, 28), 99.9975000187),
+        (dt(2010, 11, 28), dt(2011, 11, 25), 99.997419419),
+        (dt(2010, 11, 25), dt(2011, 11, 28), 99.997579958),
+    ])
+    def test_fixed_rate_bond_forward_price_analogue_ex_div(self, s, f_s, exp):
+        gilt = FixedRateBond(
+            effective=dt(1998, 12, 7),
+            termination=dt(2015, 12, 7),
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="act365f",
+            ex_div=7,
+            fixed_rate=1.0,
+            notional=-100,
+            settle=0,
+        )
+        result = gilt.fwd_from_repo(100.0, s, f_s, 1.0, "act365f")
+        assert abs(result - exp) < 1e-6
+
+    @pytest.mark.parametrize("f_s, f_p", [
+        (dt(2001, 12, 31), 99.997513754),  # compounding of mid year coupon
+        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
+    ])
+    def test_fixed_rate_bond_implied_repo(self, f_s, f_p):
+        gilt = FixedRateBond(
+            effective=dt(2001, 1, 1),
+            termination=dt(2002, 1, 1),
+            frequency="S",
+            calendar=None,
+            currency="gbp",
+            convention="Act365f",
+            ex_div=0,
+            fixed_rate=1.0,
+            notional=-100,
+            settle=0,
+        )
+        result = gilt.repo_from_fwd(100.0, dt(2001, 1, 1), f_s, f_p, "act365f")
+        assert abs(result - 1.00) < 1e-8
+
+    @pytest.mark.parametrize("f_s, f_p", [
+        (dt(2001, 12, 31), 100.49888361793),  # compounding of mid year coupon
+        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
+    ])
+    def test_fixed_rate_bond_implied_repo_analogue_dirty(self, f_s, f_p):
+        gilt = FixedRateBond(
+            effective=dt(2001, 1, 1),
+            termination=dt(2002, 1, 1),
+            frequency="S",
+            calendar=None,
+            currency="gbp",
+            convention="Act365f",
+            ex_div=0,
+            fixed_rate=1.0,
+            notional=-100,
+            settle=0,
+        )
+        result = gilt.repo_from_fwd(
+            100.0, dt(2001, 1, 1), f_s, f_p, "act365f", dirty=True
+        )
+        assert abs(result - 1.0) < 1e-8
+
 
 class TestBill:
 
     def test_bill_discount_rate(self):
         # test pricing functions against Treasury Bill Example from US Treasury
         bill = Bill(
             effective=dt(2004, 1, 22),
@@ -1249,15 +1397,15 @@
             currency="usd",
             convention="Act360",
         )
 
         assert bill.discount_rate(99.93777, dt(2004, 1, 22)) == 0.8000999999999543
         assert bill.price(0.800, dt(2004, 1, 22)) == 99.93777777777778
         # this YTM is equivalent to the FixedRateBond ytm with coupon of 0.0
-        assert bill.ytm(99.937778, dt(2004, 1, 22)) == 0.8034566609543146
+        assert abs(bill.ytm(99.937778, dt(2004, 1, 22)) - 0.8034566609543146) < 1e-9
 
         d = dcf(dt(2004, 1, 22), dt(2004, 2, 19), "Act360")
         expected = 100 * (1 / (1-0.0080009999999*d) - 1) / d  # floating point truncation
         expected = 100 * (100 / 99.93777777777778 - 1) / d
         result = bill.simple_rate(99.93777777777778, dt(2004, 1, 22))
         assert abs(result - expected) < 1e-6
 
@@ -1359,34 +1507,66 @@
 
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=0,
+            settle=0,
             float_spread=float_spd,
             spread_compound_method=method,
         )
         curve = Curve({
             dt(2007, 1, 1): 1.0,
             dt(2017, 1, 1): 0.9
         }, convention="Act365f"
         )
         disc_curve = curve.shift(curve_spd)
         result = bond.rate(
             [curve, disc_curve],
-            settlement=dt(2007, 1, 1),
             metric="spread"
         )
         assert abs(result - expected) < 1e-4
 
         bond.float_spread = result
         validate = bond.npv([curve, disc_curve])
         assert abs(validate + bond.leg1.notional) < 0.30 * abs(curve_spd)
 
+    @pytest.mark.parametrize("curve_spd, method, float_spd, expected", [
+        (10, "isda_compounding", 0, 10.00000120),
+    ])
+    def test_float_rate_bond_rate_spread_fx(self, curve_spd, method, float_spd, expected):
+        bond = FloatRateBond(
+            effective=dt(2007, 1, 1),
+            termination=dt(2017, 1, 1),
+            frequency="S",
+            convention="Act365f",
+            ex_div=0,
+            settle=0,
+            float_spread=float_spd,
+            spread_compound_method=method,
+        )
+        curve = Curve({
+            dt(2007, 1, 1): 1.0,
+            dt(2017, 1, 1): 0.9
+        }, convention="Act365f"
+        )
+        disc_curve = curve.shift(curve_spd)
+        fxr = FXRates({"usdnok": 10.0}, settlement=dt(2007, 1, 1))
+        result = bond.rate(
+            [curve, disc_curve],
+            metric="spread",
+            fx=fxr,
+        )
+        assert abs(result - expected) < 1e-4
+
+        bond.float_spread = result
+        validate = bond.npv([curve, disc_curve], fx=fxr)
+        assert abs(validate + bond.leg1.notional) < 0.30 * abs(curve_spd)
+
     def test_float_rate_bond_accrued(self):
         fixings = Series(2.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 1)))
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
@@ -1397,14 +1577,62 @@
             method_param=5,
             spread_compound_method="none_simple",
         )
         result = bond.accrued(dt(2010, 3, 3))
         expected = 0.5019275497883  # approx 2 / 12 * 3%
         assert abs(result - expected) < 1e-8
 
+    @pytest.mark.parametrize("metric, spd, exp", [
+        ("clean_price", 0., 100.),
+        ("dirty_price", 0., 100.),
+        ("clean_price", 10., 99.99982764447981),  # compounding diff between shift
+        ("dirty_price", 10., 100.0165399732469),
+    ])
+    def test_float_rate_bond_rate_metric(self, metric, spd, exp):
+        fixings = Series(0.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 1)))
+        bond = FloatRateBond(
+            effective=dt(2007, 1, 1),
+            termination=dt(2017, 1, 1),
+            frequency="S",
+            convention="Act365f",
+            ex_div=3,
+            float_spread=spd,
+            fixing_method="rfr_observation_shift",
+            fixings=fixings,
+            method_param=5,
+            spread_compound_method="none_simple",
+            settle=2
+        )
+        curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 1.0}, convention="act365f")
+        disc_curve = curve.shift(spd)
+
+        result = bond.rate(curves=[curve, disc_curve], metric=metric)
+        assert abs(result - exp) < 1e-8
+
+    @pytest.mark.parametrize("settlement, expected", [
+        (dt(2010, 3, 3), 0.501369863013698),
+        (dt(2010, 12, 30), -0.005479452054)
+    ])
+    def test_float_rate_bond_accrued_ibor(self, settlement, expected):
+        fixings = Series(2.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 1)))
+        bond = FloatRateBond(
+            effective=dt(2007, 1, 1),
+            termination=dt(2017, 1, 1),
+            frequency="S",
+            convention="Act365f",
+            ex_div=3,
+            float_spread=100,
+            fixing_method="ibor",
+            fixings=fixings,
+            method_param=2,
+            spread_compound_method="none_simple",
+        )
+        result = bond.accrued(settlement)
+        assert abs(result - expected) < 1e-8
+
     def test_float_rate_bond_raise_frequency(self):
         with pytest.raises(ValueError, match="FloatRateBond `frequency`"):
             bond = FloatRateBond(
                 effective=dt(2007, 1, 1),
                 termination=dt(2017, 1, 1),
                 frequency="Z",
                 convention="Act365f",
@@ -1483,14 +1711,438 @@
             method_param=0,
             spread_compound_method="none_simple",
             calendar=None,
         )
         result = bond.accrued(dt(2010, 3, 16))
         assert result == 0.
 
+    def test_float_rate_bond_analytic_delta(self):
+        frn = FloatRateBond(
+            effective=dt(2010, 6, 7),
+            termination=dt(2015, 12, 7),
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="ActActICMA",
+            ex_div=7,
+            float_spread=100,
+            notional=-1000000,
+            settle=0,
+            fixing_method="ibor",
+            fixings=2.0
+        )
+        curve = Curve({dt(2010, 11, 25): 1.0, dt(2015, 12, 7): 1.0})
+        result = frn.analytic_delta(curve)
+        expected = -550.0
+        assert abs(result - expected) < 1e-6
+
+        frn.settle = 1
+        result = frn.analytic_delta(curve)  # bond is ex div on settle 26th Nov 2010
+        expected = -500.0  # bond has dropped a 6m coupon payment
+        assert abs(result - expected) < 1e-6
+
+    @pytest.mark.parametrize("metric, spd, exp", [
+        ("fwd_clean_price", 0., 100),
+        ("fwd_dirty_price", 0., 100),
+        ("fwd_clean_price", 50., 99.99602155150806),
+        ("fwd_dirty_price", 50., 100.03848730493272),
+    ])
+    def test_float_rate_bond_forward_prices(self, metric, spd, exp):
+        bond = FloatRateBond(
+            effective=dt(2007, 1, 1),
+            termination=dt(2017, 1, 1),
+            frequency="S",
+            convention="Act365f",
+            ex_div=3,
+            float_spread=spd,
+            fixing_method="rfr_observation_shift",
+            method_param=5,
+            spread_compound_method="none_simple",
+            settle=2
+        )
+        curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 1.0}, convention="act365f")
+        disc_curve = curve.shift(spd)
+
+        result = bond.rate(
+            curves=[curve, disc_curve],
+            metric=metric,
+            forward_settlement=dt(2010, 8, 1)
+        )
+        assert abs(result - exp) < 1e-8
+
+    def test_float_rate_bond_forward_accrued(self):
+        bond = FloatRateBond(
+            effective=dt(2007, 1, 1),
+            termination=dt(2017, 1, 1),
+            frequency="S",
+            convention="Act365f",
+            ex_div=3,
+            float_spread=0,
+            fixing_method="rfr_observation_shift",
+            method_param=5,
+            spread_compound_method="none_simple",
+            settle=2
+        )
+        curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 0.9}, convention="act365f")
+        disc_curve = curve.shift(0)
+        result = bond.accrued(dt(2010, 8, 1), forecast=True, curve=curve)
+        expected = 0.13083715795372267
+        assert abs(result - expected) < 1e-8
+
+    def test_rate_raises(self):
+        bond = FloatRateBond(
+            effective=dt(2007, 1, 1),
+            termination=dt(2017, 1, 1),
+            frequency="S",
+            convention="Act365f",
+            ex_div=3,
+            float_spread=0.,
+            fixing_method="rfr_observation_shift",
+            method_param=5,
+            spread_compound_method="none_simple",
+            settle=2
+        )
+        with pytest.raises(ValueError, match="`forward_settlement` needed to "):
+            bond.rate(None, metric="fwd_clean_price", forward_settlement=None)
+
+        with pytest.raises(ValueError, match="`metric` must be in"):
+            bond.rate(None, metric="BAD")
+
+
+class TestBondFuture:
+
+    @pytest.mark.parametrize("delivery, mat, coupon, exp", [
+        (dt(2023, 6, 12), dt(2032, 2, 15), 0.0, 0.603058),
+        (dt(2023, 6, 12), dt(2032, 8, 15), 1.7, 0.703125),
+        (dt(2023, 6, 12), dt(2033, 2, 15), 2.3, 0.733943),
+        (dt(2023, 9, 11), dt(2032, 8, 15), 1.7, 0.709321),
+        (dt(2023, 9, 11), dt(2033, 2, 15), 2.3, 0.739087),
+        (dt(2023, 12, 11), dt(2032, 8, 15), 1.7, 0.715464),
+        (dt(2023, 12, 11), dt(2033, 2, 15), 2.3, 0.744390),
+    ])
+    def test_conversion_factors_eurex_bund(self, delivery, mat, coupon, exp):
+        # The expected results are downloaded from the EUREX website
+        # regarding precalculated conversion factors.
+        # this test allows for an error in the cf < 1e-4.
+        kwargs = dict(
+            effective=dt(2020, 1, 1),
+            stub="ShortFront",
+            frequency="A",
+            calendar="tgt",
+            currency="eur",
+            convention="ActActICMA"
+        )
+        bond1 = FixedRateBond(termination=mat, fixed_rate=coupon, **kwargs)
+
+        fut = BondFuture(
+            delivery=delivery,
+            coupon=6.0,
+            basket=[bond1]
+        )
+        result = fut.cfs
+        assert abs(result[0]-exp) < 1e-4
+
+    @pytest.mark.parametrize("mat, coupon, exp", [
+        (dt(2032, 6, 7), 4.25, 1.0187757),
+        (dt(2033, 7, 31), 0.875, 0.7410593),
+        (dt(2034, 9, 7), 4.5, 1.0449380),
+        (dt(2035, 7, 31), 0.625, 0.6773884),
+        (dt(2036, 3, 7), 4.25, 1.0247516),
+    ])
+    def test_conversion_factors_ice_gilt(self, mat, coupon, exp):
+        # The expected results are downloaded from the ICE LIFFE website
+        # regarding precalculated conversion factors.
+        # this test allows for an error in the cf < 1e-6.
+        kwargs = dict(
+            effective=dt(2020, 1, 1),
+            stub="ShortFront",
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="ActActICMA",
+            ex_div=7,
+        )
+        bond1 = FixedRateBond(termination=mat, fixed_rate=coupon, **kwargs)
+
+        fut = BondFuture(
+            delivery=(dt(2023, 6, 1), dt(2023, 6, 30)),
+            coupon=4.0,
+            basket=[bond1]
+        )
+        result = fut.cfs
+        assert abs(result[0] - exp) < 1e-6
+
+    def test_dlv_screen_print(self):
+        kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        future = BondFuture(
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
+        )
+        result = future.dlv(
+            future_price=112.98,
+            prices=[102.732, 131.461, 107.877, 134.455],
+            repo_rate=6.24,
+            settlement=dt(2000, 3, 16),
+            convention="Act365f",
+        )
+        expected = DataFrame({
+            "Bond": [
+                "5.750% 07-12-2009",
+                "9.000% 12-07-2011",
+                "6.250% 25-11-2010",
+                "9.000% 06-08-2012",
+            ],
+            "Price": [102.732, 131.461, 107.877, 134.455],
+            "YTM": [5.384243, 5.273217, 5.275481, 5.193851],
+            "C.Factor": [0.914225, 1.152571, 0.944931, 1.161956],
+            "Gross Basis": [-0.557192, 1.243582, 1.118677, 3.177230],
+            "Implied Repo": [7.381345, 3.564685, 2.199755, -1.414670],
+            "Actual Repo": [6.24, 6.24, 6.24, 6.24],
+            "Net Basis": [-0.343654, 1.033668, 1.275866, 3.010371],
+        })
+        assert_frame_equal(result, expected)
+
+        result2 = future.dlv(
+            future_price=112.98,
+            prices=[102.732, 131.461, 107.877, 134.455],
+            repo_rate=[6.24, 6.24, 6.24, 6.24],  # test individual repo input
+            settlement=dt(2000, 3, 16),
+            convention="Act365f",
+        )
+        assert_frame_equal(result2, expected)
+
+    def test_notional(self):
+        future = BondFuture(
+            coupon=0,
+            delivery=dt(2000, 6, 1),
+            basket=[],
+            nominal=100000,
+            contracts=10
+        )
+        assert future.notional == -1e6
+
+    def test_dirty_in_methods(self):
+        kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        future = BondFuture(
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
+        )
+        prices = [102.732, 131.461, 107.877, 134.455]
+        dirty_prices = [
+            price + future.basket[i].accrued(dt(2000, 3, 16))
+            for i, price in enumerate(prices)
+        ]
+        result = future.gross_basis(112.98, dirty_prices, dt(2000, 3, 16), True)
+        expected = future.gross_basis(112.98, prices, dt(2000, 3, 16), False)
+        assert result == expected
+
+    def test_delivery_in_methods(self):
+        kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        future = BondFuture(
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
+        )
+        prices = [102.732, 131.461, 107.877, 134.455]
+        expected = future.net_basis(112.98, prices, 6.24, dt(2000, 3, 16))
+        result = future.net_basis(112.98, prices, 6.24, dt(2000, 3, 16), delivery=dt(2000, 6, 30))
+        assert result == expected
+
+        expected = future.implied_repo(112.98, prices, dt(2000, 3, 16))
+        result = future.implied_repo(112.98, prices, dt(2000, 3, 16), delivery=dt(2000, 6, 30))
+        assert result == expected
+
+        expected = future.ytm(112.98)
+        result = future.ytm(112.98, delivery=dt(2000, 6, 30))
+        assert result == expected
+
+        expected = future.duration(112.98)
+        result = future.duration(112.98, delivery=dt(2000, 6, 30))
+        assert result == expected
+
+    def test_ctd_index(self):
+        kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        future = BondFuture(
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
+        )
+        prices = [102.732, 131.461, 107.877, 134.455]
+        assert future.ctd_index(112.98, prices, dt(2000, 3, 16)) == 0
+
+    @pytest.mark.parametrize("metric, expected", [
+        ("future_price", 112.98),
+        ("ytm", 5.301975)
+    ])
+    @pytest.mark.parametrize("delivery", [None, dt(2000, 6, 30)])
+    def test_futures_rates(self, metric, expected, delivery):
+        curve = Curve(
+            nodes={
+                dt(2000, 3, 15): 1.0,
+                dt(2000, 6, 30): 1.0,
+                dt(2009,  12, 7): 1.0,
+                dt(2010, 11, 25): 1.0,
+                dt(2011, 7, 12): 1.0,
+                dt(2012, 8, 6): 1.0
+            },
+            id="gilt_curve",
+            convention="act365f",
+        )
+        kws = dict(
+            ex_div=7,
+            frequency="S",
+            convention="ActActICMA",
+            calendar=None,
+            settle=1,
+            curves="gilt_curve",
+        )
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        solver = Solver(
+            curves=[curve],
+            instruments=[
+                IRS(dt(2000, 3, 15), dt(2000, 6, 30), "A", convention="act365f", curves="gilt_curve")
+            ] + bonds,
+            s=[7.381345, 102.732, 131.461, 107.877, 134.455],
+        )  # note the repo rate as defined by 'gilt_curve' is set to analogue implied
+        future = BondFuture(
+            coupon=7.0,
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
+            basket=bonds,
+        )
+        result = future.rate(None, solver, metric=metric, delivery=delivery)
+        assert abs(result - expected) < 1e-3
+
+    def test_future_rate_raises(self):
+        kws = dict(
+            ex_div=7,
+            frequency="S",
+            convention="ActActICMA",
+            calendar=None,
+            settle=1,
+            curves="gilt_curve",
+        )
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        future = BondFuture(
+            coupon=7.0,
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
+            basket=bonds,
+        )
+        with pytest.raises(ValueError, match="`metric`"):
+            result = future.rate(metric="badstr")
+
+    def test_futures_npv(self):
+        curve = Curve(
+            nodes={
+                dt(2000, 3, 15): 1.0,
+                dt(2000, 6, 30): 1.0,
+                dt(2009,  12, 7): 1.0,
+                dt(2010, 11, 25): 1.0,
+                dt(2011, 7, 12): 1.0,
+                dt(2012, 8, 6): 1.0
+            },
+            id="gilt_curve",
+            convention="act365f",
+        )
+        kws = dict(
+            ex_div=7,
+            frequency="S",
+            convention="ActActICMA",
+            calendar=None,
+            settle=1,
+            curves="gilt_curve",
+            currency="gbp",
+        )
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        solver = Solver(
+            curves=[curve],
+            instruments=[
+                IRS(dt(2000, 3, 15), dt(2000, 6, 30), "A", convention="act365f", curves="gilt_curve")
+            ] + bonds,
+            s=[7.381345, 102.732, 131.461, 107.877, 134.455],
+        )  # note the repo rate as defined by 'gilt_curve' is set to analogue implied
+        future = BondFuture(
+            coupon=7.0,
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
+            basket=bonds,
+            nominal=100000,
+            contracts=10,
+            currency="gbp",
+        )
+        result = future.npv(None, solver, local=False)
+        expected = 1129798.770872
+        assert abs(result - expected) < 1e-5
+
+        result2 = future.npv(None, solver, local=True)
+        assert abs(result2["gbp"] - expected) < 1e-5
+
+    @pytest.mark.parametrize("delivery", [None, dt(2000, 6, 30)])
+    def test_futures_duration_and_convexity(self, delivery):
+        kws = dict(
+            ex_div=7,
+            frequency="S",
+            convention="ActActICMA",
+            calendar=None,
+            settle=1,
+            curves="gilt_curve",
+        )
+        bonds = [
+            FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+            FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+        ]
+        future = BondFuture(
+            coupon=7.0,
+            delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
+            basket=bonds,
+        )
+        result = future.duration(112.98, delivery=delivery)[0]
+        expected = 8.20178546111
+        assert abs(result - expected) < 1e-3
+
+        expected = (
+            future.duration(112.98, delivery=delivery)[0]
+            - future.duration(112.98-result/100, delivery=delivery)[0]
+        )
+        result2 = future.convexity(112.98, delivery=delivery)[0]
+        assert abs(result2 - expected*100) < 1e-3
+
 
 class TestPricingMechanism:
 
     def test_value(self, curve):
         ob = Value(dt(2022, 1, 28), curves=curve)
         ob.rate()
```

### Comparing `rateslib-0.1.0/tests/test_legs.py` & `rateslib-0.2.0/tests/test_legs.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 import context
 from rateslib import default_context
 from rateslib.legs import (
     FixedLeg,
     FloatLeg,
     FloatPeriod,
+    ZeroFloatLeg,
     FixedPeriod,
     CustomLeg,
     FloatLegExchange,
     FixedLegExchange,
+    IndexFixedLegExchange,
     FloatLegExchangeMtm,
     FixedLegExchangeMtm,
     Cashflow,
 )
 from rateslib.fx import FXRates, FXForwards
-from rateslib.defaults import Defaults
-from rateslib.curves import Curve
+from rateslib.default import Defaults
+from rateslib.curves import Curve, IndexCurve
 
 
 @pytest.fixture()
 def curve():
     nodes = {
         dt(2022, 1, 1): 1.00,
         dt(2022, 4, 1): 0.99,
@@ -313,14 +315,127 @@
             assert leg.periods[i].__repr__() == expected[i].__repr__()
 
     def test_spread_compound_method_raises(self):
         with pytest.raises(ValueError, match="`spread_compound_method`"):
             FloatLeg(dt(2022, 2, 1), "9M", "Q", spread_compound_method="bad")
 
 
+class TestZeroFloatLeg:
+
+    def test_zero_float_leg_set_float_spread(self, curve):
+        float_leg = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+        )
+        assert float_leg.float_spread is None
+        assert float_leg.periods[0].float_spread == 0
+
+        float_leg.float_spread = 2.0
+        assert float_leg.float_spread == 2.0
+        assert float_leg.periods[0].float_spread == 2.0
+
+    def test_zero_float_leg_amort_raise(self):
+        with pytest.raises(NotImplementedError, match="`ZeroFloatLeg` cannot accept"):
+            float_leg = ZeroFloatLeg(
+                effective=dt(2022, 1, 1),
+                termination=dt(2022, 6, 1),
+                payment_lag=2,
+                notional=-1e9,
+                convention="Act360",
+                frequency="Q",
+                amortization=1,
+            )
+
+    def test_zero_float_leg_dcf(self):
+        ftl = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+        )
+        result = ftl.dcf
+        expected = ftl.periods[0].dcf + ftl.periods[1].dcf
+        assert result == expected
+
+    def test_zero_float_leg_rate(self, curve):
+        ftl = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+            float_spread=500,
+        )
+        result = ftl.rate(curve)
+        expected = (1+ftl.periods[0].dcf * ftl.periods[0].rate(curve)/100)
+        expected *= (1+ftl.periods[1].dcf * ftl.periods[1].rate(curve)/100)
+        expected = (expected - 1) / ftl.dcf * 100
+        assert result == expected
+
+    def test_zero_float_leg_cashflows(self, curve):
+        ftl = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+            float_spread=500,
+        )
+        result = ftl.cashflows(curve)
+        expected = DataFrame(
+            {
+                "Type": ["ZeroFloatLeg"],
+                 "Acc Start": [dt(2022, 1, 1)],
+                 "Acc End": [dt(2022, 6, 1)],
+                 "DCF": [0.419444444444444],
+                 "Spread": [500.]
+             }
+        )
+        assert_frame_equal(
+            result[["Type", "Acc Start", "Acc End", "DCF", "Spread"]],
+            expected
+        )
+
+    def test_zero_float_leg_npv(self, curve):
+        ftl = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+        )
+        result = ftl.npv(curve)
+        expected = 16710778.891147703
+        assert abs(result - expected) < 1e-2
+        result2 = ftl.npv(curve, local=True)
+        assert abs(result2["usd"] - expected) < 1e-2
+
+    def test_cashflows_none(self):
+        ftl = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+        )
+        result = ftl.cashflows()
+        assert result.iloc[0].to_dict()[Defaults.headers["npv"]] is None
+        assert result.iloc[0].to_dict()[Defaults.headers["npv_fx"]] is None
+
+
 class TestFloatLegExchange:
 
     def test_float_leg_exchange_notional_setter(self):
         float_leg_exc = FloatLegExchange(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
@@ -459,64 +574,91 @@
         assert fixed_leg.periods[0].fixed_rate is None
 
         fixed_leg.fixed_rate = 2.0
         assert fixed_leg.fixed_rate == 2.0
         assert fixed_leg.periods[0].fixed_rate == 2.0
 
 
-class TestFixedLegExchange:
+class TestIndexFixedLegExchange:
 
-    def test_fixed_leg_exchange_notional_setter(self):
-        fixed_leg_exc = FixedLegExchange(
-            effective=dt(2022, 1, 1),
-            termination=dt(2022, 6, 1),
-            payment_lag=2,
-            notional=-1e9,
-            convention="Act360",
-            frequency="Q",
+    @pytest.mark.parametrize("i_fixings", [
+        None,
+        [2.1, 2.2, 2.3],
+        2.1,
+        Series(
+            [2.1, 2.2, 2.3],
+            index=[dt(2022, 6, 15), dt(2022, 9, 15), dt(2022, 12, 15)]
         )
-        fixed_leg_exc.notional = 200
-        assert fixed_leg_exc.notional == 200
-
-    def test_fixed_leg_exchange_amortization_setter(self):
-        fixed_leg_exc = FixedLegExchange(
-            effective=dt(2022, 1, 1),
-            termination=dt(2022, 10, 1),
-            payment_lag=2,
-            notional=-1000,
-            convention="Act360",
-            frequency="Q",
-        )
-        fixed_leg_exc.amortization = -200
-
-        cashflows = [2, 4, 6]
-        cash_notionals = [None, -200, None, -200, None, -600]
-        fixed_notionals = [None, -1000, None, -800, None, -600]
-        for i in cashflows:
-            assert isinstance(fixed_leg_exc.periods[i], Cashflow)
-            assert fixed_leg_exc.periods[i].notional == cash_notionals[i - 1]
-
-            assert isinstance(fixed_leg_exc.periods[i - 1], FixedPeriod)
-            assert fixed_leg_exc.periods[i - 1].notional == fixed_notionals[i - 1]
-
-    def test_fixed_leg_exchange_set_fixed_rate(self):
-        fixed_leg_exc = FixedLegExchange(
-            effective=dt(2022, 1, 1),
-            termination=dt(2022, 10, 1),
-            payment_lag=2,
-            notional=-1000,
-            convention="Act360",
+    ])
+    def test_idx_leg_cashflows(self, i_fixings):
+        leg = IndexFixedLegExchange(
+            effective=dt(2022, 3, 15),
+            termination="9M",
             frequency="Q",
-        )
-        assert fixed_leg_exc.fixed_rate is None
-        fixed_leg_exc.fixed_rate = 2.0
-        assert fixed_leg_exc.fixed_rate == 2.0
-        for period in fixed_leg_exc.periods:
-            if isinstance(period, FixedPeriod):
-                period.fixed_rate == 2.0
+            convention="ActActICMA",
+            payment_lag=0,
+            notional=40e6,
+            fixed_rate=5.0,
+            index_base=200.0,
+            index_fixings=i_fixings,
+            initial_exchange=False,
+        )
+        index_curve = IndexCurve(
+            nodes={
+                dt(2022, 3, 15): 1.0,
+                dt(2022, 6, 15): 1.0 / 1.05,
+                dt(2022, 9, 15): 1.0 / 1.10,
+                dt(2022, 12, 15): 1.0 / 1.15,
+            },
+            index_base=200.0
+        )
+        disc_curve = Curve({dt(2022, 3, 15): 1.0, dt(2022, 12, 15): 1.0})
+        flows = leg.cashflows(curve=index_curve, disc_curve=disc_curve)
+
+        def equals_with_tol(a, b):
+            if isinstance(a, str):
+                return a == b
+            else:
+                return abs(a-b) < 1e-7
+
+        expected = {
+            "Type": "IndexFixedPeriod",
+            "DCF": 0.250,
+            "Notional": 40e6,
+            "Rate": 5.0,
+            "Real Cashflow": -500e3,
+            "Index Val": 230.0,
+            "Index Ratio": 1.15,
+            "Cashflow": -575000,
+        }
+        flow = flows.iloc[2].to_dict()
+        for key in set(expected.keys()) & set(flow.keys()):
+            assert equals_with_tol(expected[key], flow[key])
+
+        final_flow = flows.iloc[3].to_dict()
+        expected = {
+            "Type": "IndexCashflow",
+            "Notional": 40e6,
+            "Real Cashflow": -40e6,
+            "Index Val": 230.0,
+            "Index Ratio": 1.15,
+            "Cashflow": -46e6,
+        }
+        for key in set(expected.keys()) & set(final_flow.keys()):
+            assert equals_with_tol(expected[key], final_flow[key])
+
+    def test_args_raises(self):
+        with pytest.raises(ValueError, match="`index_method` must be in"):
+            leg = IndexFixedLegExchange(
+                effective=dt(2022, 3, 15),
+                termination="9M",
+                frequency="Q",
+                index_base=200.0,
+                index_method="BAD"
+            )
 
 
 class TestFloatLegExchangeMtm:
 
     @pytest.mark.parametrize("fx_fixings, exp", [
         (None, [None, None, None]),
         ([1.5], [1.5, None, None]),
```

### Comparing `rateslib-0.1.0/tests/test_periods.py` & `rateslib-0.2.0/tests/test_periods.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pytest
 from datetime import datetime as dt
+from datetime import timedelta
 from pandas.testing import assert_frame_equal
 from pandas import DataFrame, Series
 import numpy as np
 
 import context
 from rateslib.periods import (
-    Cashflow, FixedPeriod, FloatPeriod,
+    Cashflow, FixedPeriod, FloatPeriod, IndexFixedPeriod, IndexCashflow
 )
 from rateslib.fx import FXRates
-from rateslib.defaults import Defaults
-from rateslib.curves import Curve, LineCurve
+from rateslib.default import Defaults
+from rateslib.curves import Curve, LineCurve, IndexCurve
 
 
 @pytest.fixture()
 def curve():
     nodes = {
         dt(2022, 1, 1): 1.00,
         dt(2022, 4, 1): 0.99,
@@ -708,14 +709,38 @@
                 payment=dt(2022, 4, 4),
                 frequency="Q",
                 fixing_method="rfr_lockout",
                 method_param=0,
                 fixings=[1.00]
             )
 
+        with pytest.raises(ValueError, match="`method_param` should not be used"):
+            float_period = FloatPeriod(
+                start=dt(2022, 1, 4),
+                end=dt(2022, 4, 4),
+                payment=dt(2022, 4, 4),
+                frequency="Q",
+                fixing_method="rfr_payment_delay",
+                method_param=2,
+                fixings=[1.00]
+            )
+
+    def test_analytic_delta_no_curve_raises(self):
+        float_period = FloatPeriod(
+            start=dt(2022, 12, 28),
+            end=dt(2023, 1, 2),
+            payment=dt(2023, 1, 2),
+            frequency="M",
+            fixings=[1.19, 1.19, -8.81],
+            spread_compound_method="isda_compounding",
+            float_spread=1.0
+        )
+        with pytest.raises(TypeError, match="`curve` must be supplied"):
+            float_period.analytic_delta()
+
 
 class TestFixedPeriod:
 
     def test_fixed_period_analytic_delta(self, curve, fxr):
         fixed_period = FixedPeriod(
             start=dt(2022, 1, 1),
             end=dt(2022, 4, 1),
@@ -728,15 +753,14 @@
         )
         result = fixed_period.analytic_delta(curve)
         assert abs(result - 24744.478172244584) < 1e-7
 
         result = fixed_period.analytic_delta(curve, curve, fxr, "nok")
         assert abs(result - 247444.78172244584) < 1e-7
 
-
     def test_fixed_period_analytic_delta_fxr_base(self, curve, fxr):
         fixed_period = FixedPeriod(
             start=dt(2022, 1, 1),
             end=dt(2022, 4, 1),
             payment=dt(2022, 4, 3),
             notional=1e9,
             convention="Act360",
@@ -777,18 +801,18 @@
             Defaults.headers["notional"]: 1e9,
             Defaults.headers["currency"]: "USD",
             Defaults.headers["convention"]: "Act360",
             Defaults.headers["dcf"]: fixed_period.dcf,
             Defaults.headers["df"]: 0.9897791268897856 if crv else None,
             Defaults.headers["rate"]: rate,
             Defaults.headers["spread"]: None,
-            Defaults.headers["npv"]: -9897791.268897858 if crv else None,
+            Defaults.headers["npv"]: -9897791.268897856 if crv else None,
             Defaults.headers["cashflow"]: cashflow,
             Defaults.headers["fx"]: fx,
-            Defaults.headers["npv_fx"]: -9897791.268897858 * fx if crv else None,
+            Defaults.headers["npv_fx"]: -9897791.268897855 * fx if crv else None,
         }
         result = fixed_period.cashflows(
             curve if crv else None,
             fx=(2 if fx == 2 else fxr),
             base="_" if fx == 2 else "nok",
         )
         assert result == expected
@@ -807,22 +831,36 @@
         )
         result = fixed_period.npv(curve)
         assert abs(result + 9897791.268897833) < 1e-7
 
         result = fixed_period.npv(curve, curve, fxr, "nok")
         assert abs(result + 98977912.68897833) < 1e-6
 
+    def test_fixed_period_npv_raises(self):
+        fixed_period = FixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+        )
+        with pytest.raises(TypeError, match="`curves` have not been"):
+            fixed_period.npv(None)
+
 
 class TestCashflow:
 
     def test_cashflow_analytic_delta(self, curve):
         cashflow = Cashflow(notional=1e6, payment=dt(2022, 1, 1))
         assert cashflow.analytic_delta(curve) == 0
 
-
     @pytest.mark.parametrize("crv, fx", [
         (True, 2.0),
         (False, 2.0),
         (True, 10.0),
         (False, 10.0),
     ])
     def test_cashflow_cashflows(self, curve, fxr, crv, fx):
@@ -849,12 +887,274 @@
         result = cashflow.cashflows(
             curve if crv else None,
             fx=(2 if fx == 2 else fxr),
             base="_" if fx == 2 else "nok",
         )
         assert result == expected
 
+    def test_cashflow_npv_raises(self, curve):
+        with pytest.raises(TypeError, match="`curves` have not been supplied"):
+            cashflow = Cashflow(notional=1e6, payment=dt(2022, 1, 1))
+            cashflow.npv(None)
+        cashflow = Cashflow(notional=1e6, payment=dt(2022, 1, 1))
+        assert cashflow.analytic_delta(curve) == 0
+
+    def test_cashflow_npv_local(self, curve):
+        cashflow = Cashflow(notional=1e9, payment=dt(2022, 4, 3), currency="nok")
+        result = cashflow.npv(curve, local=True)
+        expected = {"nok": -989779126.8897856}
+        assert result == expected
+
+
+class TestIndexFixedPeriod:
+
+    @pytest.mark.parametrize("method, expected", [
+        ("daily", 201.00502512562812), ("monthly", 200.98317675333183)
+    ])
+    def test_period_rate(self, method, expected):
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+            index_method=method,
+        )
+        index_curve = IndexCurve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
+            index_base=200.,
+        )
+        result = index_period.rate(index_curve)
+        assert abs(result - expected) < 1e-8
+
+    def test_period_cashflow(self):
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+        )
+        index_curve = IndexCurve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
+            index_base=200.,
+        )
+        result = index_period.real_cashflow
+        expected = -1e7 * ((dt(2022, 4, 1) - dt(2022, 1, 1)) / timedelta(days=360)) * 4
+        assert abs(result - expected) < 1e-8
+
+        result = index_period.cashflow(index_curve)
+        expected = expected * index_curve.index_value(dt(2022, 4, 3)) / 100.
+        assert abs(result - expected) < 1e-8
+
+    def test_period_analytic_delta(self, fxr, curve):
+        index_curve = IndexCurve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
+            index_base=200.,
+        )
+        fixed_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            currency="usd",
+            index_base=200.0,
+            index_fixings=300.0,
+        )
+        result = fixed_period.analytic_delta(index_curve, curve)
+        assert abs(result - 24744.478172244584 * 300. / 200.) < 1e-7
+
+        result = fixed_period.analytic_delta(index_curve, curve, fxr, "nok")
+        assert abs(result - 247444.78172244584 * 300. / 200.) < 1e-7
+
+    @pytest.mark.parametrize("fixings, method", [
+        (300.0, "daily"),
+        (
+            Series([1, 300, 5], index=[dt(2022, 4, 2), dt(2022, 4, 3), dt(2022, 4, 4)]),
+            "daily",
+        ),
+        (Series([100., 500], index=[dt(2022, 4, 2), dt(2022, 4, 4)]), "daily"),
+        (Series([300., 500], index=[dt(2022, 4, 1), dt(2022, 4, 5)]), "monthly"),
+    ])
+    def test_period_fixings_series(self, fixings, method, curve):
+        fixed_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            currency="usd",
+            index_base=200.0,
+            index_fixings=fixings,
+            index_method=method,
+        )
+        result = fixed_period.analytic_delta(None, curve)
+        assert abs(result - 24744.478172244584 * 300. / 200.) < 1e-7
+
+    def test_period_raises(self):
+        with pytest.raises(ValueError, match="`index_method` must be "):
+            fixed_period = IndexFixedPeriod(
+                start=dt(2022, 1, 1),
+                end=dt(2022, 4, 1),
+                payment=dt(2022, 4, 3),
+                notional=1e9,
+                convention="Act360",
+                termination=dt(2022, 4, 1),
+                frequency="Q",
+                currency="usd",
+                index_base=200.0,
+                index_method="BAD",
+            )
+
+    def test_period_npv(self, curve):
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+        )
+        index_curve = IndexCurve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
+            index_base=200.,
+        )
+        result = index_period.npv(index_curve, curve)
+        expected = -19895057.826930363
+        assert abs(result - expected) < 1e-8
+
+        result = index_period.npv(index_curve, curve, local=True)
+        assert abs(result["usd"] - expected) < 1e-8
+
+    def test_period_npv_raises(self):
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+        )
+        with pytest.raises(TypeError, match="`curves` have not been supplied"):
+            index_period.npv(None)
+
+    @pytest.mark.parametrize("curve_", [True, False])
+    def test_period_cashflows(self, curve, curve_):
+        curve = curve if curve_ else None
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+            index_fixings=200.,
+        )
+        result = index_period.cashflows(curve)
+        expected = {
+            "Type": "IndexFixedPeriod",
+            "Period": "Regular",
+            "Ccy": "USD",
+            "Acc Start": dt(2022, 1, 1),
+            "Acc End": dt(2022, 4, 1),
+            "Payment": dt(2022, 4, 3),
+            "Convention": "Act360",
+            "DCF": 0.25,
+            "DF": 0.9897791268897856 if curve_ else None,
+            "Notional": 1e9,
+            "Rate": 4.0,
+            "Spread": None,
+            "Cashflow": -20000000.0,
+            "Real Cashflow": -10e6,
+            "Index Val": 200.0,
+            "Index Ratio": 2.0,
+            "NPV": -19795582.53779571 if curve_ else None,
+            "FX Rate": 1.0,
+            "NPV Ccy": -19795582.53779571 if curve_ else None,
+        }
+        assert result == expected
+
+    def test_cashflow_returns_none(self):
+        i_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 2, 1),
+            payment=dt(2022, 2, 1),
+            frequency="M",
+            index_base=100.0,
+        )
+        assert i_period.cashflow() is None
+        assert i_period.real_cashflow is None
+
+    def test_cashflow_no_index_rate(self):
+        i_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 2, 1),
+            payment=dt(2022, 2, 1),
+            frequency="M",
+            index_base=100.0,
+        )
+        result = i_period.cashflows()
+        assert result[Defaults.headers["index_ratio"]] is None
+
+
+class TestIndexCashflow:
+
+    def test_cashflow_analytic_delta(self, curve):
+        cashflow = IndexCashflow(
+            notional=1e6, payment=dt(2022, 1, 1), index_base=100
+        )
+        assert cashflow.analytic_delta(curve) == 0
+
+    def test_index_cashflow(self):
+        cf = IndexCashflow(
+            notional=1e6, payment=dt(2022, 1, 1), index_base=100, index_fixings=200
+        )
+        assert cf.real_cashflow == -1e6
+
+        assert cf.cashflow(None) == -2e6
+
+    def test_index_cashflow_npv(self, curve):
+        cf = IndexCashflow(
+            notional=1e6, payment=dt(2022, 1, 1), index_base=100, index_fixings=200
+        )
+        assert abs(cf.npv(curve) + 2e6) < 1e-6
+
+    def test_cashflow_no_index_rate(self):
+        i_period = IndexCashflow(
+            notional=200.0,
+            payment=dt(2022, 2, 1),
+            index_base=100.0,
+        )
+        result = i_period.cashflows()
+        assert result[Defaults.headers["index_ratio"]] is None
 
 
 def test_base_period_dates_raise():
     with pytest.raises(ValueError):
         _ = FixedPeriod(dt(2023, 1, 1), dt(2022, 1, 1), dt(2024, 1, 1), "Q")
```

### Comparing `rateslib-0.1.0/tests/test_scheduling.py` & `rateslib-0.2.0/tests/test_scheduling.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from pandas import DatetimeIndex, date_range, DataFrame
 from pandas.tseries.holiday import Holiday
 from pandas.testing import assert_index_equal
 from datetime import datetime as dt
 
 import context
-from rateslib.defaults import Defaults
+from rateslib.default import Defaults
 from rateslib.calendars import create_calendar
 from rateslib.scheduling import (
     _check_unadjusted_regular_swap,
     _check_regular_swap,
     _is_divisible_months,
     _get_date_category,
     _get_default_stub,
```

### Comparing `rateslib-0.1.0/tests/test_solver.py` & `rateslib-0.2.0/tests/test_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pandas import DataFrame, MultiIndex
 from pandas.testing import assert_frame_equal
 import numpy as np
 from numpy.testing import assert_allclose
 from math import log, exp
 
 import context
-from rateslib import defaults, default_context
+from rateslib import default_context
 from rateslib.curves import Curve, index_left, LineCurve
 from rateslib.solver import Solver
 from rateslib.dual import Dual
 from rateslib.instruments import IRS, Value, FloatRateBond, Portfolio, XCS
 from rateslib.fx import FXRates, FXForwards
 
 
@@ -548,14 +548,50 @@
     grad_s_vT_fixed_point_iter = solver.grad_s_vT
 
     assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_final_iter_anal, atol=1e-12)
     assert_allclose(grad_s_vT_fixed_point_iter, grad_s_vT_final_iter_anal, atol=1e-12)
     assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_fixed_point_iter, atol=1e-12)
 
 
+def test_solver_grad_s_vT_methods_equivalent_overspecified_curve():
+    curve = Curve(nodes={
+        dt(2022, 1, 1): 1.0,
+        dt(2023, 1, 1): 1.0,
+        dt(2024, 1, 1): 1.0,
+        dt(2025, 1, 1): 1.0,
+        # dt(2026, 1, 1): 1.0,
+        dt(2027, 1, 1): 1.0,
+    })
+    instruments = [
+        (IRS(dt(2022, 1, 1), "2Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "1Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "2Y", "A"), (curve,), {}),
+        (IRS(dt(2022, 5, 1), "4Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "4Y", "A"), (curve,), {}),
+    ]
+    s = [1.2, 1.4, 1.6, 1.7, 1.9]
+    solver = Solver([curve], instruments, s)
+
+    solver._grad_s_vT_method = "_grad_s_vT_final_iteration_analytical"
+    grad_s_vT_final_iter_anal = solver.grad_s_vT
+
+    solver._grad_s_vT_method = "_grad_s_vT_final_iteration_dual"
+    solver._grad_s_vT_final_iteration_algo = "gauss_newton_final"
+    solver._reset_properties_()
+    grad_s_vT_final_iter_dual = solver.grad_s_vT
+
+    solver._grad_s_vT_method = "_grad_s_vT_fixed_point_iteration"
+    solver._reset_properties_()
+    grad_s_vT_fixed_point_iter = solver.grad_s_vT
+
+    assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_final_iter_anal, atol=1e-6)
+    assert_allclose(grad_s_vT_fixed_point_iter, grad_s_vT_final_iter_anal, atol=1e-6)
+    assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_fixed_point_iter, atol=1e-6)
+
+
 def test_solver_second_order_vars_raise_on_first_order():
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
     solver = Solver(
         curves=[curve],
         instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
         s=[1]
     )
@@ -610,20 +646,20 @@
         dt(2022, 7, 1): 0.94,
         dt(2023, 1, 1): 0.92,
         dt(2024, 1, 1): 0.9,
     }, id="credit")
     f_c = d_c.copy()
     f_c.id = "rfr"
     instruments = [
-        (FloatRateBond(dt(2022, 1, 1), "6M", "Q", spread_compound_method="isda_compounding"),
-         ([f_c, d_c],), {"metric": "spread", "settlement": dt(2022, 1, 3)}),
-        (FloatRateBond(dt(2022, 1, 1), "1y", "Q", spread_compound_method="isda_compounding"),
-         ([f_c, d_c],), {"metric": "spread", "settlement": dt(2022, 1, 3)}),
-        (FloatRateBond(dt(2022, 1, 1), "18m", "Q", spread_compound_method="isda_compounding"),
-         ([f_c, d_c],), {"metric": "spread", "settlement": dt(2022, 1, 3)}),
+        (FloatRateBond(dt(2022, 1, 1), "6M", "Q", spread_compound_method="isda_compounding", settle=2),
+         ([f_c, d_c],), {"metric": "spread"}),
+        (FloatRateBond(dt(2022, 1, 1), "1y", "Q", spread_compound_method="isda_compounding", settle=2),
+         ([f_c, d_c],), {"metric": "spread"}),
+        (FloatRateBond(dt(2022, 1, 1), "18m", "Q", spread_compound_method="isda_compounding", settle=2),
+         ([f_c, d_c],), {"metric": "spread"}),
     ]
     solver = Solver([d_c], instruments, [25, 25, 25])
     result = d_c.rate(dt(2022, 7, 1), "1D")
     expected = f_c.rate(dt(2022, 7, 1), "1D") + 0.25
     assert abs(result - expected) < 1e-5
 
 
@@ -959,7 +995,26 @@
             IRS(dt(2022, 1, 1), "12M", "A", curves="curve1"),
         ],
         s=[2.0, 2.2, 2.3, 2.4, 2.45, 2.55],
         id="rates",
     )
     result = solver_with_error.error
     assert abs(result.loc[("rates", "rates0")] - 22.798) < 1e-2
+
+
+def test_solver_non_unique_id_raises():
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    solver = Solver(
+        curves=[curve],
+        instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
+        s=[1],
+        id="bad"
+    )
+    curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="B")
+    with pytest.raises(ValueError, match="Solver `id`s must be unique"):
+        solver2 = Solver(
+            curves=[curve2],
+            instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve2,), {})],
+            s=[1],
+            id="bad",
+            pre_solvers=[solver]
+        )
```

### Comparing `rateslib-0.1.0/tests/test_splines.py` & `rateslib-0.2.0/tests/test_splines.py`

 * *Files identical despite different names*

