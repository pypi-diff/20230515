# Comparing `tmp/cvxsimulator-0.3.1.tar.gz` & `tmp/cvxsimulator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.3.2.tar", max compression
```

## Comparing `cvxsimulator-0.3.1.tar` & `cvxsimulator-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1102 2023-05-10 05:02:56.377078 cvxsimulator-0.3.1/LICENSE
--rw-r--r--   0        0        0     4907 2023-05-10 05:02:56.377078 cvxsimulator-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     3796 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1163 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1341 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/month.py
--rw-r--r--   0        0        0     3549 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      596 2023-05-10 05:03:54.213931 cvxsimulator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-15 16:53:35.626777 cvxsimulator-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4907 2023-05-15 16:53:35.626777 cvxsimulator-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     3796 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1163 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1341 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/month.py
+-rw-r--r--   0        0        0     4307 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-15 16:53:35.654777 cvxsimulator-0.3.2/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      596 2023-05-15 16:53:59.707195 cvxsimulator-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.2/PKG-INFO
```

### Comparing `cvxsimulator-0.3.1/LICENSE` & `cvxsimulator-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.1/README.md` & `cvxsimulator-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.1/cvx/simulator/builder.py` & `cvxsimulator-0.3.2/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.1/cvx/simulator/metrics.py` & `cvxsimulator-0.3.2/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.1/cvx/simulator/month.py` & `cvxsimulator-0.3.2/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.3.2/cvx/simulator/portfolio.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,27 +18,41 @@
         assert self.stocks.index.is_unique
 
         assert set(self.stocks.index).issubset(set(self.prices.index))
         assert set(self.stocks.columns).issubset(set(self.prices.columns))
 
     @property
     def index(self):
+        """
+        The timestamps in the portfolio (index in prices frame)
+
+        Returns:
+             Index of timestamps
+        """
         return self.prices.index
 
     @property
     def assets(self):
+        """
+        The assets in the portfolio (columns in prices frame)
+
+        Returns:
+            Index of assets.
+        """
         return self.prices.columns
 
     @property
     def weights(self):
+        """
+        Frame of relative weights (e.g. value / nav)
+        """
         return self.equity / self.nav
 
-    def __getitem__(self, item):
-        assert item in self.index
-        return self.stocks.loc[item]
+    def __getitem__(self, time):
+        return self.stocks.loc[time]
 
     @property
     def trading_costs(self):
         # return a frame of all zeros
         if self.trading_cost_model is None:
             return 0.0 * self.prices
 
@@ -72,14 +86,34 @@
         """
         Profit
         """
         price_changes = self.prices.ffill().diff()
         previous_stocks = self.stocks.shift(1).fillna(0.0)
         return (previous_stocks * price_changes).dropna(axis=0, how="all").sum(axis=1)
 
+    @property
+    def highwater(self) -> pd.Series:
+        """
+        Highwater mark.
+
+        Returns:
+            The High-Water Mark, e.g. a moving max.
+        """
+        return self.nav.expanding(min_periods=1).max()
+
+    @property
+    def drawdown(self) -> pd.Series:
+        """
+        The drawdown relative to HWM.
+
+        Returns:
+            Relative drawdown series.
+        """
+        return 1.0 - self.nav / self.highwater
+
     def __mul__(self, scalar):
         """
         Multiplies positions by a scalar
         """
         return EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar, initial_cash=self.initial_cash * scalar, trading_cost_model=self.trading_cost_model)
 
     def __rmul__(self, scalar):
```

### Comparing `cvxsimulator-0.3.1/pyproject.toml` & `cvxsimulator-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.1"
+version = "v0.3.2"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.3.1/PKG-INFO` & `cvxsimulator-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

