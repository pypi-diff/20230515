# Comparing `tmp/quant_invest_lab-0.2.3.tar.gz` & `tmp/quant_invest_lab-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.3.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.4.tar", max compression
```

## Comparing `quant_invest_lab-0.2.3.tar` & `quant_invest_lab-0.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4427 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/README.md
--rw-r--r--   0        0        0      978 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    18277 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17110 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26301 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     8038 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    20461 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4427 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/README.md
+-rw-r--r--   0        0        0      978 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    32590 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17110 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0     9477 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    20461 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     1107 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.4/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.3/README.md` & `quant_invest_lab-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/pyproject.toml` & `quant_invest_lab-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quant-invest-lab"
-version = "0.2.3"
+version = "0.2.4"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 packages = [{include = "quant_invest_lab"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.4/quant_invest_lab/backtest.py`

 * *Files 24% similar despite different names*

```diff
@@ -113,50 +113,52 @@
     previous_row = ohlcv_df.iloc[0]
     position_opened = False
     timeframe_count = 0
     current_trade: dict[str, float | datetime | int | str | pd.Timestamp] = {}
 
     trades_df = pd.DataFrame(
         columns=[
-            "buy_date",
-            "buy_price",
-            "buy_reason",
-            "sell_date",
-            "sell_price",
-            "sell_reason",
+            "entry_date",
+            "entry_price",
+            "entry_reason",
+            "exit_date",
+            "exit_price",
+            "exit_reason",
             "trade_return",
         ]
     )
 
     returns_df = pd.DataFrame(columns=["Returns"])
 
     for index, row in tqdm(
         ohlcv_df[1:].iterrows(),
         desc="Backtesting...",
         total=ohlcv_df.shape[0] - 1,
         leave=False,
     ):
         if position_opened is False and long_entry_function(row, previous_row) is True:
             position_opened = True
-            current_trade["buy_date"] = index
-            current_trade["buy_price"] = row.Close
-            current_trade["buy_reason"] = "Entry position triggered"
+            current_trade["entry_date"] = index
+            current_trade["entry_price"] = row.Close
+            current_trade["entry_reason"] = "Entry position triggered"
             timeframe_count = 1
-            buy_price = row.Close
+            entry_price = row.Close
         elif (
             position_opened is True
-            and current_trade["buy_price"] * (1 + take_profit) <= row.High
+            and current_trade["entry_price"] * (1 + take_profit) <= row.High
         ):
             position_opened = False
-            current_trade["sell_date"] = index
-            current_trade["sell_price"] = current_trade["buy_price"] * (1 + take_profit)
-            current_trade["sell_reason"] = "Take profit triggered"
+            current_trade["exit_date"] = index
+            current_trade["exit_price"] = current_trade["entry_price"] * (
+                1 + take_profit
+            )
+            current_trade["exit_reason"] = "Take profit triggered"
 
             rets = ohlcv_df.loc[
-                current_trade["buy_date"] : current_trade["sell_date"]
+                current_trade["entry_date"] : current_trade["exit_date"]
             ].Returns
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
             current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
 
             trades_df = pd.concat(
@@ -167,25 +169,25 @@
                 ignore_index=False,
             )
             timeframe_count = 0
 
             current_trade = {}
         elif (
             position_opened is True
-            and current_trade["buy_price"] * (1 - stop_loss) >= row.Low
+            and current_trade["entry_price"] * (1 - stop_loss) >= row.Low
         ):
             position_opened = False
-            current_trade["sell_date"] = index
-            current_trade["sell_price"] = float(current_trade["buy_price"]) * (
+            current_trade["exit_date"] = index
+            current_trade["exit_price"] = float(current_trade["entry_price"]) * (
                 1 - stop_loss
             )
-            current_trade["sell_reason"] = "Stop loss triggered"
+            current_trade["exit_reason"] = "Stop loss triggered"
 
             rets = ohlcv_df.loc[
-                current_trade["buy_date"] : current_trade["sell_date"]
+                current_trade["entry_date"] : current_trade["exit_date"]
             ].Returns
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
             current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
 
             trades_df = pd.concat(
@@ -198,20 +200,20 @@
             timeframe_count = 0
             current_trade = {}
         elif (
             position_opened is True
             and long_exit_function(row, previous_row, timeframe_count) is True
         ):
             position_opened = False
-            current_trade["sell_date"] = index
-            current_trade["sell_price"] = row.Close
-            current_trade["sell_reason"] = "Exit position triggered"
+            current_trade["exit_date"] = index
+            current_trade["exit_price"] = row.Close
+            current_trade["exit_reason"] = "Exit position triggered"
 
             rets = ohlcv_df.loc[
-                current_trade["buy_date"] : current_trade["sell_date"]
+                current_trade["entry_date"] : current_trade["exit_date"]
             ].Returns
 
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
 
             current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
@@ -235,15 +237,15 @@
     ohlcv_df["Drawdown"] = drawdown(df["Returns"])
     if parameter_optimization is True:
         if len(trades_df) > 0:
             return returns_df["Cum_Returns"].iloc[-1]
         return 0.0
 
     assert len(trades_df) > 0, "No trades were generated"
-    trades_df["trade_duration"] = trades_df["sell_date"] - trades_df["buy_date"]
+    trades_df["trade_duration"] = trades_df["exit_date"] - trades_df["entry_date"]
 
     good_trades = trades_df.loc[trades_df["trade_return"] > 0]
     bad_trades = trades_df.loc[trades_df["trade_return"] < 0]
     total_trades = len(trades_df)
 
     print(f"{'  Initial informations  ':-^50}")
     print(f"Period: [{str(ohlcv_df.index[0])}] -> [{str(ohlcv_df.index[-1])}]")
@@ -316,34 +318,366 @@
 
     print(f"\n  Total good trades: {len(good_trades)}")
     print(f"  Mean good trades return: {100*good_trades['trade_return'].mean():.2f} %")
     print(
         f"  Median good trades return: {100*good_trades['trade_return'].median():.2f} %"
     )
     print(
-        f"  Best trades return: {100*trades_df['trade_return'].max():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmax()]['sell_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmax()]['trade_duration']}"
+        f"  Best trades return: {100*trades_df['trade_return'].max():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmax()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmax()]['trade_duration']}"
     )
     print(
         f"  Mean good trade duration: {str((good_trades['trade_duration']).mean()).split('.')[0]}"
     )
     print(f"\n  Total bad trades: {len(bad_trades)}")
     print(f"  Mean bad trades return: {100*bad_trades['trade_return'].mean():.2f} %")
     print(
         f"  Median bad trades return: {100*bad_trades['trade_return'].median():.2f} %"
     )
     print(
-        f"  Worst trades return: {100*trades_df['trade_return'].min():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmin()]['sell_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmin()]['trade_duration']}"
+        f"  Worst trades return: {100*trades_df['trade_return'].min():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmin()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmin()]['trade_duration']}"
     )
     print(
         f"  Mean bad trade duration: {str((bad_trades['trade_duration']).mean()).split('.')[0]}"
     )
 
     print(f"\nExit reasons repartition: ")
     for reason, val in zip(
-        trades_df.sell_reason.value_counts().index, trades_df.sell_reason.value_counts()
+        trades_df.exit_reason.value_counts().index, trades_df.exit_reason.value_counts()
+    ):
+        print(f"- {reason}: {val}")
+    if plot_result is True:
+        plot_from_trade_df(trades_df, ohlcv_df, returns_df)
+    if get_returns_df and get_trade_df:
+        return trades_df, returns_df
+    if get_trade_df:
+        return trades_df
+    if get_returns_df:
+        return returns_df
+
+
+def ohlc_short_only_backtester(
+    df: pd.DataFrame,
+    short_entry_function: Callable[[pd.Series, pd.Series], bool],
+    short_exit_function: Callable[[pd.Series, pd.Series, int], bool],
+    timeframe: Literal[
+        "1min",
+        "2min",
+        "5min",
+        "15min",
+        "30min",
+        "1hour",
+        "2hour",
+        "4hour",
+        "12hour",
+        "1day",
+    ],
+    take_profit: float = np.inf,
+    stop_loss: float = np.inf,
+    initial_equity: int = 1000,
+    maker_fees: Optional[float] = 0.001,
+    taker_fees: Optional[float] = 0.001,
+    get_trade_df: bool = False,
+    get_returns_df: bool = False,
+    parameter_optimization: bool = False,
+    plot_result: bool = True,
+) -> Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]:
+    """Run a backtest with short only position on a OHLC dataset.
+
+    Args:
+    ----
+        df (pd.DataFrame): The dataframe containing the OHLC data.
+
+        short_entry_function (Callable[[pd.Series, pd.Series], bool]): The short entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
+
+        short_exit_function (Callable[[pd.Series, pd.Series, int], bool]): The short exit function, it should take 3 arguments, the current row, the previous row and the number of timeframe count since the last entry order, and return True or False depending on your strategy.
+
+        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ]): The timeframe granularity of the dataframe.
+
+        take_profit (float, optional): The percent of the buy price to add to create a stop order and take the profit associated. Defaults to np.inf.
+
+        stop_loss (float, optional): The percent of the buy price to cut to create a stop order and stop the loss associated. Defaults to np.inf.
+
+        initial_equity (int, optional): The initial capital. Defaults to 1000.
+
+        maker_fees (Optional[float], optional): The fees applied, here maker for limit orders (not yet implemented). Defaults to 0.001.
+
+        taker_fees (Optional[float], optional): The fees applied, here taker for spot orders. Defaults to 0.001.
+
+        get_trade_df (bool, optional): Whether or not to return the trade dataframe (summary of trades) . Defaults to False.
+
+        get_returns_df (bool, optional): Whether or not to return the strategy returns dataframe. Defaults to False.
+
+        parameter_optimization (bool, optional): This parameter is useful when running fitting/optimization it prints nothing but the final strategy return. Defaults to False.
+
+        plot_result (bool, optional): Plot equity, price, drawdown, distribution of the strategy. Defaults to True.
+
+    Returns:
+    -----
+        Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]: Nothing or the strategy total return or the trade_df or the return_df or the trade_df and the return_df.
+    """
+    assert timeframe in [
+        "1min",
+        "2min",
+        "5min",
+        "15min",
+        "30min",
+        "1hour",
+        "2hour",
+        "4hour",
+        "12hour",
+        "1day",
+    ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
+    assert df.shape[0] > 1, "Dataframe must have at least 2 rows"
+    assert set({"Open", "High", "Low", "Close", "Returns"}).issubset(
+        df.columns
+    ), "Dataframe must have columns Open, High, Low, Close, Returns"
+    timeframe_annualized = {
+        "1min": int(365 * 24 / 1 * 60),
+        "2min": int(365 * 24 / 1 * 30),
+        "5min": int(365 * 24 / 1 * 12),
+        "15min": int(365 * 24 / 1 * 4),
+        "30min": int(365 * 24 / 1 * 2),
+        "1hour": int(365 * 24 / 1),
+        "2hour": int(365 * 24 / 2),
+        "4hour": int(365 * 24 / 4),
+        "12hour": int(365 * 24 / 12),
+        "1day": 365,
+    }
+    N = timeframe_annualized[timeframe]
+    ohlcv_df = df.copy()
+    previous_row = ohlcv_df.iloc[0]
+    position_opened = False
+    timeframe_count = 0
+    current_trade: dict[str, float | datetime | int | str | pd.Timestamp] = {}
+
+    trades_df = pd.DataFrame(
+        columns=[
+            "entry_date",
+            "entry_price",
+            "entry_reason",
+            "exit_date",
+            "exit_price",
+            "exit_reason",
+            "trade_return",
+        ]
+    )
+
+    returns_df = pd.DataFrame(columns=["Returns"])
+
+    for index, row in tqdm(
+        ohlcv_df[1:].iterrows(),
+        desc="Backtesting...",
+        total=ohlcv_df.shape[0] - 1,
+        leave=False,
+    ):
+        if position_opened is False and short_entry_function(row, previous_row) is True:
+            position_opened = True
+            current_trade["entry_date"] = index
+            current_trade["entry_price"] = row.Close
+            current_trade["entry_reason"] = "Entry position triggered"
+            timeframe_count = 1
+            entry_price = row.Close
+        elif (
+            position_opened is True
+            and current_trade["entry_price"] * (1 + stop_loss) <= row.High
+        ):
+            position_opened = False
+            current_trade["exit_date"] = index
+            current_trade["exit_price"] = current_trade["entry_price"] * (1 + stop_loss)
+            current_trade["exit_reason"] = "Stop loss triggered"
+
+            rets = -ohlcv_df.loc[
+                current_trade["entry_date"] : current_trade["exit_date"]
+            ].Returns
+            if isinstance(taker_fees, float) and taker_fees > 0:
+                rets.iloc[0] = rets.iloc[0] - taker_fees
+                rets.iloc[-1] = rets.iloc[-1] - taker_fees
+            current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
+
+            trades_df = pd.concat(
+                [trades_df, pd.DataFrame([current_trade])], ignore_index=True
+            )
+            returns_df = pd.concat(
+                [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
+                ignore_index=False,
+            )
+            timeframe_count = 0
+
+            current_trade = {}
+        elif (
+            position_opened is True
+            and current_trade["entry_price"] * (1 - take_profit) >= row.Low
+        ):
+            position_opened = False
+            current_trade["exit_date"] = index
+            current_trade["exit_price"] = float(current_trade["entry_price"]) * (
+                1 - take_profit
+            )
+            current_trade["exit_reason"] = "Take profit triggered"
+
+            rets = -ohlcv_df.loc[
+                current_trade["entry_date"] : current_trade["exit_date"]
+            ].Returns
+            if isinstance(taker_fees, float) and taker_fees > 0:
+                rets.iloc[0] = rets.iloc[0] - taker_fees
+                rets.iloc[-1] = rets.iloc[-1] - taker_fees
+            current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
+
+            trades_df = pd.concat(
+                [trades_df, pd.DataFrame([current_trade])], ignore_index=True
+            )
+            returns_df = pd.concat(
+                [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
+                ignore_index=False,
+            )
+            timeframe_count = 0
+            current_trade = {}
+        elif (
+            position_opened is True
+            and short_exit_function(row, previous_row, timeframe_count) is True
+        ):
+            position_opened = False
+            current_trade["exit_date"] = index
+            current_trade["exit_price"] = row.Close
+            current_trade["exit_reason"] = "Exit position triggered"
+
+            rets = -ohlcv_df.loc[
+                current_trade["entry_date"] : current_trade["exit_date"]
+            ].Returns
+
+            if isinstance(taker_fees, float) and taker_fees > 0:
+                rets.iloc[0] = rets.iloc[0] - taker_fees
+                rets.iloc[-1] = rets.iloc[-1] - taker_fees
+
+            current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
+
+            trades_df = pd.concat(
+                [trades_df, pd.DataFrame([current_trade])], ignore_index=True
+            )
+            returns_df = pd.concat(
+                [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
+                ignore_index=False,
+            )
+            timeframe_count = 0
+            current_trade = {}
+        else:
+            timeframe_count += 1
+        previous_row = row
+
+    returns_df["Cum_Returns"] = (returns_df["Returns"] + 1).cumprod()
+    returns_df["Drawdown"] = drawdown(returns_df["Returns"])
+    ohlcv_df["Cum_Returns"] = (df["Returns"] + 1).cumprod()
+    ohlcv_df["Drawdown"] = drawdown(df["Returns"])
+    if parameter_optimization is True:
+        if len(trades_df) > 0:
+            return returns_df["Cum_Returns"].iloc[-1]
+        return 0.0
+
+    assert len(trades_df) > 0, "No trades were generated"
+    trades_df["trade_duration"] = trades_df["exit_date"] - trades_df["entry_date"]
+
+    good_trades = trades_df.loc[trades_df["trade_return"] > 0]
+    bad_trades = trades_df.loc[trades_df["trade_return"] < 0]
+    total_trades = len(trades_df)
+
+    print(f"{'  Initial informations  ':-^50}")
+    print(f"Period: [{str(ohlcv_df.index[0])}] -> [{str(ohlcv_df.index[-1])}]")
+    print(f"Intial balance: {initial_equity:.2f} $")
+    if taker_fees is not None and maker_fees is not None:
+        print(
+            f"Taker fees: {taker_fees*100:.2f} %, Maker fees: {maker_fees*100:.2f} %, All the metrics will be calculated considering these fees"
+        )
+    else:
+        print("No fees considered here.")
+
+    print(f"\n{'  Strategy performances  ':-^50}")
+
+    print(
+        f'Strategy final net balance: {returns_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, return: {(returns_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
+    )
+    print(
+        f'Buy & Hold final net balance: {ohlcv_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, returns: {(ohlcv_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
+    )
+    print(f"Strategy winrate ratio: {100 * len(good_trades) / total_trades:.2f} %")
+    print(
+        f"Strategy profit factor ratio: {abs(good_trades['trade_return'].mean()/bad_trades['trade_return'].mean()):.2f}"
+    )
+
+    print(f"\n{'  Returns statistical information  ':-^50}")
+
+    print(
+        f"Expected return : {100*returns_df['Returns'].mean():.2f} %, annuzalized: {100*returns_df['Returns'].mean()*N:.2f} %"
+    )
+    print(
+        f"Median return : {100*returns_df['Returns'].median():.2f} %, annuzalized: {100*returns_df['Returns'].median()*N:.2f} %"
+    )
+    print(
+        f'Expected volatility: {100*returns_df["Returns"].std():.2f} %, annualized: {100*returns_df["Returns"].std()*(N**0.5):.2f} %'
+    )
+    print(
+        f'Skewness: {skew(returns_df["Returns"].values):.2f}, <0 = left tail, >0 = right tail -> the higher the better'
+    )
+    print(
+        f'Kurtosis: {kurtosis(returns_df["Returns"].values):.2f}',
+        ", >3 = fat tails, <3 = thin tails -> the lower the better",
+    )
+    print(f"{timeframe}-95%-VaR: {100*value_at_risk(returns_df['Returns']):.2f} %")
+    print(
+        f"{timeframe}-95%-CVaR: {100*conditional_value_at_risk(returns_df['Returns']):.2f} %"
+    )
+
+    print(f"\n{'  Strategy statistical information  ':-^50}")
+    print(f"Max drawdown: {100*max_drawdown(returns_df['Returns']):.2f} %")
+    print(f"Kelly criterion: {100*kelly_criterion(returns_df.Returns):.2f} %")
+    print(
+        f"Sharpe ratio (annualized): {sharpe_ratio(returns_df['Returns'], N,risk_free_rate=N*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
+    )
+    print(
+        f"Sortino ratio (annualized): {sortino_ratio(returns_df['Returns'], N,risk_free_rate=N*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
+    )
+    print(
+        f"Calmar ratio (annualized): {calmar_ratio(returns_df['Returns'], N):.2f} (risk free rate = buy and hold)"
+    )
+
+    print(f"\n{'  Trades informations  ':-^50}")
+    print(f"Mean trade return : {100*trades_df['trade_return'].mean():.2f} %")
+    print(f"Median trade return : {100*trades_df['trade_return'].median():.2f} %")
+    print(f'Mean trade volatility: {100*trades_df["trade_return"].std():.2f} %')
+    print(
+        f"Mean trade duration: {str((trades_df['trade_duration']).mean()).split('.')[0]}"
+    )
+
+    print(f"Total trades: {total_trades}")
+
+    print(f"\n  Total good trades: {len(good_trades)}")
+    print(f"  Mean good trades return: {100*good_trades['trade_return'].mean():.2f} %")
+    print(
+        f"  Median good trades return: {100*good_trades['trade_return'].median():.2f} %"
+    )
+    print(
+        f"  Best trades return: {100*trades_df['trade_return'].max():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmax()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmax()]['trade_duration']}"
+    )
+    print(
+        f"  Mean good trade duration: {str((good_trades['trade_duration']).mean()).split('.')[0]}"
+    )
+    print(f"\n  Total bad trades: {len(bad_trades)}")
+    print(f"  Mean bad trades return: {100*bad_trades['trade_return'].mean():.2f} %")
+    print(
+        f"  Median bad trades return: {100*bad_trades['trade_return'].median():.2f} %"
+    )
+    print(
+        f"  Worst trades return: {100*trades_df['trade_return'].min():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmin()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmin()]['trade_duration']}"
+    )
+    print(
+        f"  Mean bad trade duration: {str((bad_trades['trade_duration']).mean()).split('.')[0]}"
+    )
+
+    print(f"\nExit reasons repartition: ")
+    for reason, val in zip(
+        trades_df.exit_reason.value_counts().index, trades_df.exit_reason.value_counts()
     ):
         print(f"- {reason}: {val}")
     if plot_result is True:
         plot_from_trade_df(trades_df, ohlcv_df, returns_df)
     if get_returns_df and get_trade_df:
         return trades_df, returns_df
     if get_trade_df:
@@ -386,33 +720,33 @@
         ),
         row=1,
         col=1,
     )
     fig.update_yaxes(title_text="Historical price (USDT)", row=1, col=1)
     fig.update_xaxes(title_text="Datetime", row=1, col=1)
     trades = trade_df.copy()
-    trades["date"] = trades["sell_date"]
+    trades["date"] = trades["exit_date"]
     trades = trades.set_index("date")
 
     fig.add_trace(
         go.Scatter(
             name="Buy and hold cumulative return",
             x=price_df.index,
             y=price_df["Cum_Returns"],
-            line={"shape": "hv"},
+            line={"shape": "hv", "color": "violet"},
         ),
         row=2,
         col=1,
     )
     fig.add_trace(
         go.Scatter(
             name="Strategy cumulative return",
             x=returns_df.index,
             y=returns_df["Cum_Returns"],
-            line={"shape": "hv"},
+            line={"shape": "hv", "color": "salmon"},
         ),
         row=2,
         col=1,
     )
     fig.update_yaxes(type="log", row=2, col=1)
     fig.update_yaxes(title_text="Log cumulative returns", row=2, col=1)
     fig.update_xaxes(title_text="Datetime", row=2, col=1)
@@ -439,35 +773,35 @@
         ),
         row=3,
         col=1,
     )
 
     fig.update_yaxes(title_text="Drawdown", row=3, col=1)
     fig.update_xaxes(title_text="Datetime", row=3, col=1)
-
+    distplot_bench = ff.create_distplot(
+        [price_df["Returns"]],
+        ["Benchmark Returns"],
+        colors=["violet"],
+        curve_type="kde",
+        bin_size=3.5
+        * price_df["Returns"].std()
+        / (len(price_df["Returns"]) ** (1 / 3)),
+    )
+    fig.add_trace(distplot_bench["data"][0], row=4, col=1)
     distplot = ff.create_distplot(
         [returns_df["Returns"]],
         ["Strategy Returns"],
         colors=["salmon"],
         curve_type="kde",
         bin_size=3.5
         * returns_df["Returns"].std()
         / (len(returns_df["Returns"]) ** (1 / 3)),
     )
     fig.add_trace(distplot["data"][0], row=4, col=1)
 
-    distplot_bench = ff.create_distplot(
-        [price_df["Returns"]],
-        ["Benchmark Returns"],
-        curve_type="kde",
-        bin_size=3.5
-        * price_df["Returns"].std()
-        / (len(price_df["Returns"]) ** (1 / 3)),
-    )
-    fig.add_trace(distplot_bench["data"][0], row=4, col=1)
     fig.update_xaxes(title_text="Returns", row=4, col=1)
     fig.update_yaxes(title_text="Density", row=4, col=1)
     fig.update_layout(
         xaxis_rangeslider_visible=False,
         showlegend=True,
         title_text="Historical price, strategy equity evolution/drawdown and returns distribution",
         height=1000,
```

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.4/quant_invest_lab/data_provider.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.4/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.4/quant_invest_lab/metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -134,14 +134,50 @@
     Returns:
     ----
         float: The max drawdown.
     """
     return drawdown(returns).min()
 
 
+def information_ratio(
+    portfolio_returns: pd.Series, benchmark_returns: pd.Series
+) -> float:
+    """The information ratio (IR) is a measurement of portfolio returns beyond the returns of a benchmark, usually an index, compared to the volatility of those returns. The information ratio (IR) measures a portfolio manager's ability to generate excess returns relative to a benchmark but also attempts to identify the consistency of the investor.
+
+    Args:
+    -----
+        portfolio_returns (pd.Series): The strategy or portfolio not cumulative returns.
+
+        benchmark_returns (pd.Series): The strategy or portfolio benchmark not cumulative returns.
+
+    Returns:
+    -----
+        float: The annualized information ratio.
+    """
+    return (portfolio_returns - benchmark_returns).mean() / tracking_error(
+        portfolio_returns, benchmark_returns
+    )
+
+
+def tracking_error(portfolio_returns: pd.Series, benchmark_returns: pd.Series) -> float:
+    """Tracking error is the divergence between the price behavior of a position or a portfolio and the price behavior of a benchmark.
+
+    Args:
+    -----
+        portfolio_returns (pd.Series): The strategy or portfolio not cumulative returns.
+
+        benchmark_returns (pd.Series): The strategy or portfolio benchmark not cumulative returns.
+
+    Returns:
+    -----
+        float: The annualized tracking error.
+    """
+    return (portfolio_returns - benchmark_returns).std()
+
+
 def kelly_criterion(returns: pd.Series) -> float:
     p = (returns > 0).mean()
     q = 1 - p
     win = returns[returns > 0].mean()
     loss = returns[returns < 0].mean()
     r = win / abs(loss)
     return float((p * r - q) / r)
```

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.4/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.4/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.4/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.4/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.4/quant_invest_lab/utils.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.3/PKG-INFO` & `quant_invest_lab-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.3
+Version: 0.2.4
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
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.3 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.4 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
 for that and sharing it as open source project. Author: BaptisteZloch Author-
 email: bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

