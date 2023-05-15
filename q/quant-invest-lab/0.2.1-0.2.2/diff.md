# Comparing `tmp/quant_invest_lab-0.2.1.tar.gz` & `tmp/quant_invest_lab-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.1.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.2.tar", max compression
```

## Comparing `quant_invest_lab-0.2.1.tar` & `quant_invest_lab-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     4427 2023-05-14 20:28:40.324711 quant_invest_lab-0.2.1/README.md
--rw-r--r--   0        0        0      978 2023-05-14 20:22:51.144752 quant_invest_lab-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    18278 2023-05-14 17:42:39.234752 quant_invest_lab-0.2.1/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17111 2023-05-14 17:05:21.454752 quant_invest_lab-0.2.1/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26223 2023-05-14 20:20:38.384760 quant_invest_lab-0.2.1/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     8038 2023-05-14 15:47:17.294752 quant_invest_lab-0.2.1/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-14 20:17:42.054696 quant_invest_lab-0.2.1/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    20361 2023-05-14 18:09:36.804750 quant_invest_lab-0.2.1/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-14 17:30:20.244749 quant_invest_lab-0.2.1/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-14 17:22:27.984752 quant_invest_lab-0.2.1/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-14 17:21:39.694751 quant_invest_lab-0.2.1/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     5790 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.1/setup.py
--rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4427 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/README.md
+-rw-r--r--   0        0        0      978 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    18277 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17110 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0     8038 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    20461 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     1107 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.2/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.1/README.md` & `quant_invest_lab-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.1/pyproject.toml` & `quant_invest_lab-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quant-invest-lab"
-version = "0.2.1"
+version = "0.2.2"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 packages = [{include = "quant_invest_lab"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.2/quant_invest_lab/backtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "15min",
         "30min",
         "1hour",
         "2hour",
         "4hour",
         "12hour",
         "1day",
-    ] = "1day",
+    ],
     take_profit: float = np.inf,
     stop_loss: float = np.inf,
     initial_equity: int = 1000,
     maker_fees: Optional[float] = 0.001,
     taker_fees: Optional[float] = 0.001,
     get_trade_df: bool = False,
     get_returns_df: bool = False,
@@ -52,15 +52,15 @@
     ----
         df (pd.DataFrame): The dataframe containing the OHLC data.
 
         long_entry_function (Callable[[pd.Series, pd.Series], bool]): The long entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
 
         long_exit_function (Callable[[pd.Series, pd.Series, int], bool]): The long exit function, it should take 3 arguments, the current row, the previous row and the number of timeframe count since the last entry order, and return True or False depending on your strategy.
 
-        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ], optional): The timeframe granularity of the dataframe. Defaults to "1day".
+        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ]): The timeframe granularity of the dataframe.
 
         take_profit (float, optional): The percent of the buy price to add to create a stop order and take the profit associated. Defaults to np.inf.
 
         stop_loss (float, optional): The percent of the buy price to cut to create a stop order and stop the loss associated. Defaults to np.inf.
 
         initial_equity (int, optional): The initial capital. Defaults to 1000.
 
@@ -126,15 +126,18 @@
             "trade_return",
         ]
     )
 
     returns_df = pd.DataFrame(columns=["Returns"])
 
     for index, row in tqdm(
-        ohlcv_df[1:].iterrows(), desc="Backtesting...", total=ohlcv_df.shape[0] - 1
+        ohlcv_df[1:].iterrows(),
+        desc="Backtesting...",
+        total=ohlcv_df.shape[0] - 1,
+        leave=False,
     ):
         if position_opened is False and long_entry_function(row, previous_row) is True:
             position_opened = True
             current_trade["buy_date"] = index
             current_trade["buy_price"] = row.Close
             current_trade["buy_reason"] = "Entry position triggered"
             timeframe_count = 1
```

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.2/quant_invest_lab/data_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                 )
 
             df = df.sort_values(by="Timestamp")
             df.drop_duplicates(inplace=True)
             return df
 
     __kucoin_fetcher = KucoinDataFetcher()
-    __base_dir = "../data/"
+    __base_dir = "./data/"
     __absolute_start_date = "01-01-2017"
 
     def get_list_of_symbols(
         self, base_currency: Optional[str] = None, quote_currency: Optional[str] = None
     ) -> list[str]:
         """Return the list of symbol in the database's file.
         Args:
```

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.2/quant_invest_lab/indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
 
     Args:
         support_resistance_levels (list[float]): The support and resistance levels.
         open (pd.Series[float | int]): The open series from the OHLCV Data.
         low (pd.Series[float | int]): The low series from the OHLCV Data.
 
     Returns:
-        pd.Series: _description_
+        pd.Series: The S/R breakout rolling indicator.
     """
 
     def has_breakout(open_rows: pd.Series) -> int:
         """Base on the candle stick, detect a breakout or not.
 
         Args:
             open_rows (pd.Series): A series of 2 rolling open measures.
@@ -340,16 +340,16 @@
     window: int = 26,
 ) -> pd.Series:
     """ZLEMA is an abbreviation of Zero Lag Exponential Moving Average. It was developed by John Ehlers and Rick Way.
     ZLEMA is a kind of Exponential moving average but its main idea is to eliminate the lag arising from the very nature of the moving averages
     and other trend following indicators. As it follows price closer, it also provides better price averaging and responds better to price swings.
 
     Args:
-        close (pd.Series): _description_
-        window (int, optional): _description_. Defaults to 26.
+        close (pd.Series): The close series from the OHLCV Data.
+        window (int, optional): The window to calculate the zlema on a period. Defaults to 26.
 
     Returns:
         pd.Series: The ZLEMA indicator
     """
     return (close + (close.diff((window - 1) // 2))).ewm(span=window).mean()
```

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.2/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.2/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.2/quant_invest_lab/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,46 +40,49 @@
         weights: npt.NDArray | Iterable,
         assets: npt.NDArray | list[str] | tuple[str] | pd.Index,
     ) -> None:
         """Plot the allocation of the portfolio in  a pie chart.
 
         Args:
         -----
-            weights (npt.NDArray | Iterable): _description_
-            assets (npt.NDArray | list[str] | tuple[str]): _description_
+            weights (npt.NDArray | Iterable): The weights for each asset in the portfolio between 0 and 1.
+            assets (npt.NDArray | list[str] | tuple[str]): The assets (their names) in the portfolio.
         """
         res = [(p, float(w)) for p, w in zip(assets, weights)]
         res.sort(key=lambda x: x[1], reverse=True)
         res = np.array(res)
-        fig = go.Figure(
-            go.Pie(
-                labels=res[:, 0].tolist(),
-                values=res[:, -1],
-                hole=0.4,
-                text=[f"{p}: {float(w):.2f} %" for p, w in res],
-                textinfo="label+percent",
-                hoverinfo="label+value",
-                marker=dict(colors=px.colors.qualitative.Pastel1),
-            )
-        )
-
-        fig.update_layout(
-            title={
-                "text": "Asset allocation",
-                "x": 0.5,
-                "y": 0.95,
-                "xanchor": "center",
-                "yanchor": "top",
-            },
-            showlegend=False,
-            height=600,
-            width=600,
-        )
+        plt.title("Asset allocation")
+        plt.pie(res[:, -1], labels=res[:, 0].tolist(), autopct="%1.1f%%")
+        plt.show()
+        # fig = go.Figure(
+        #     go.Pie(
+        #         labels=res[:, 0].tolist(),
+        #         values=res[:, -1],
+        #         hole=0.4,
+        #         text=[f"{p}: {float(w):.2f} %" for p, w in res],
+        #         textinfo="label+percent",
+        #         hoverinfo="label+value",
+        #         marker=dict(colors=px.colors.qualitative.Pastel1),
+        #     )
+        # )
+
+        # fig.update_layout(
+        #     title={
+        #         "text": "Asset allocation",
+        #         "x": 0.5,
+        #         "y": 0.95,
+        #         "xanchor": "center",
+        #         "yanchor": "top",
+        #     },
+        #     showlegend=False,
+        #     height=600,
+        #     width=600,
+        # )
 
-        fig.show()
+        # fig.show()
 
     def _compute_metrics(
         self,
         weights: npt.NDArray,
     ) -> dict[str, float | int]:
         """Given an array of weights, compute the Sharpe ratio, the risk and the return of the portfolio. This method in used it the optimization functions of the portfolio optimization models.
 
@@ -335,18 +338,14 @@
         """
         self.__all_weights = np.zeros((n_portfolios, len(self._returns.columns)))
         self.__ret_arr = np.zeros(n_portfolios)
         self.__vol_arr = np.zeros(n_portfolios)
         self.__sharpe_arr = np.zeros(n_portfolios)
 
         for x in tqdm(range(n_portfolios)):
-            # Weights
-            # weights = np.array(
-            #     np.random.uniform(size=len(self._returns.columns)), dtype=np.float64
-            # )
             weights = np.array(
                 np.random.rand(len(self._returns.columns)), dtype=np.float64
             )
             weights = weights / np.sum(weights)
 
             # Save weights
             self.__all_weights[x, :] = weights
@@ -522,15 +521,15 @@
         isinstance(full_dataframe, pd.DataFrame)
         and full_dataframe.shape[0] != 0
         and full_dataframe.shape[1] > 1
     ), "full_dataframe must be a pandas DataFrame containing at least 2 columns and 1 row"
     assert (
         target_explained_variance > 0 and target_explained_variance < 1
     ), "target_explained_variance must be a float between 0 and 1"
-    X = full_dataframe.values
+    X = full_dataframe.to_numpy()
     match mode:
         case "pca":
             calibration_pca = PCA()
             calibration_pca.fit(X)
 
             d = (
                 np.argmax(
```

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.2/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.2/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.1/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.2/quant_invest_lab/utils.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.1/PKG-INFO` & `quant_invest_lab-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.1 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.2 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
 for that and sharing it as open source project. Author: BaptisteZloch Author-
 email: bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

