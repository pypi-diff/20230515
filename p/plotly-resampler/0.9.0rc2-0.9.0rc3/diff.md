# Comparing `tmp/plotly_resampler-0.9.0rc2.tar.gz` & `tmp/plotly_resampler-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.9.0rc2.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.0rc3.tar", max compression
```

## Comparing `plotly_resampler-0.9.0rc2.tar` & `plotly_resampler-0.9.0rc3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1115 2023-05-03 12:32:58.928306 plotly_resampler-0.9.0rc2/LICENSE
--rw-r--r--   0        0        0     9540 2023-05-09 09:35:41.332034 plotly_resampler-0.9.0rc2/README.md
--rw-r--r--   0        0        0      853 2023-05-11 09:37:41.902449 plotly_resampler-0.9.0rc2/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      796 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     6934 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    11877 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0     3048 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handler_interface.py
--rw-r--r--   0        0        0     3179 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handlers.py
--rw-r--r--   0        0        0     7933 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/plotly_aggregator_parser.py
--rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    23690 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    61317 2023-05-11 09:36:04.273826 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13669 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     5376 2023-05-07 09:13:04.096399 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc2/plotly_resampler/registering.py
--rw-r--r--   0        0        0     2857 2023-05-11 09:37:23.139098 plotly_resampler-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-05-03 12:32:58.928306 plotly_resampler-0.9.0rc3/LICENSE
+-rw-r--r--   0        0        0    11180 2023-05-15 07:29:18.434096 plotly_resampler-0.9.0rc3/README.md
+-rw-r--r--   0        0        0      853 2023-05-15 07:29:43.141241 plotly_resampler-0.9.0rc3/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     6934 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    11877 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3048 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3179 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     8088 2023-05-15 07:29:18.434096 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    23690 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    62492 2023-05-15 07:10:55.600245 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13669 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     5376 2023-05-14 08:02:19.170287 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc3/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     2857 2023-05-15 07:29:29.573711 plotly_resampler-0.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    13126 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc3/PKG-INFO
```

### Comparing `plotly_resampler-0.9.0rc2/LICENSE` & `plotly_resampler-0.9.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/README.md` & `plotly_resampler-0.9.0rc3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 > `plotly_resampler`: visualize large sequential data by **adding resampling functionality to Plotly figures**
 
 [Plotly](https://github.com/plotly/plotly.py) is an awesome interactive visualization library, however it can get pretty slow when a lot of data points are visualized (100 000+ datapoints). This library solves this by downsampling (aggregating) the data respective to the view and then plotting the aggregated points. When you interact with the plot (panning, zooming, ...), callbacks are used to aggregate data and update the figure.
 
 ![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/basic_example.gif)
 
-
 In [this Plotly-Resampler demo](https://github.com/predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over `110,000,000` data points are visualized!
 
 <!-- These dynamic aggregation callbacks are realized with: -->
 <!-- * [Dash](https://github.com/plotly/dash) when a `go.Figure` object is wrapped with dynamic aggregation functionality, see example ⬆️. -->
 <!-- * The [FigureWidget.layout.on_change](https://plotly.com/python-api-reference/generated/plotly.html?highlight=on_change#plotly.basedatatypes.BasePlotlyType.on_change) method, when a `go.FigureWidget` is used within a `.ipynb` environment. -->
 
 <!-- #### Useful links -->
@@ -35,14 +34,33 @@
 
 ### Installation
 
 | [**pip**](https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
 | ---| ----|
 <!-- | [**conda**](https://anaconda.org/conda-forge/plotly_resampler/) | `conda install -c conda-forge plotly_resampler` | -->
 
+<br>
+<details><summary><b>What is the difference between plotly-resampler figures and plain plotly figures?</b></summary>
+
+`plotly-resampler` can be thought of as wrapper around plain plotly figures which adds visualization scalability to line-charts by dynamically aggregating the data w.r.t. the front-end view. `plotly-resampler` thus adds dynamic aggregation functionality to plain plotly figures.
+
+**Important to know**:
+
+* ``show`` *always* returns a static html view of the figure, i.e., no dynamic aggregation can be performed on that view.
+* To have dynamic aggregation:
+
+  * with ``FigureResampler``, you need to call ``show_dash`` (or output the object in a cell via ``IPython.display``) -> which spawns a dash-web app, and the dynamic aggregation is realized with dash callback.
+  * with ``FigureWidgetResampler``, you need to use ``IPython.display`` on the object, which uses widget-events to realize dynamic aggregation (via the running IPython kernel).
+
+**Other changes of plotly-resampler figures w.r.t. vanilla plotly**:
+
+* **double-clicking** within a line-chart area **does not Reset Axes**, as it results in an “Autoscale” event. We decided to implement an Autoscale event as updating your y-range such that it shows all the data that is in your x-range.
+   * **Note**: vanilla Plotly figures their Autoscale result in Reset Axes behavior, in our opinion this did not make a lot of sense. It is therefore that we have overriden this behavior in plotly-resampler.
+</details><br>
+
 ### Features :tada:
 
   * **Convenient** to use:
     * just add either
       * `register_plotly_resampler` function to your notebook with the best suited `mode` argument.
       * `FigureResampler` decorator around a plotly Figure and call `.show_dash()`
       * `FigureWidgetResampler` decorator around a plotly Figure and output the instance in a cell
@@ -136,34 +154,34 @@
 * When running the code on a server, you should forward the port of the `FigureResampler.show_dash()` method to your local machine.<br>
   **Note** that you can add dynamic aggregation to plotly figures with the `FigureWidgetResampler` wrapper without needing to forward a port!
 * The `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation functionality, so when this main thread is occupied, no resampling logic can be executed. For example; if you perform long computations within your notebook, the kernel will be occupied during these computations, and will only execute the resampling operations that take place during these computations after finishing that computation.
 * In general, when using downsampling one should be aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing) effects.
   The <b style="color:orange">[R]</b> in the legend indicates when the corresponding trace is being resampled (and thus possibly distorted) or not. Additionally, the `~<range>` suffix represent the mean aggregation bin size in terms of the sequence index.
 * The plotly **autoscale** event (triggered by the autoscale button or a double-click within the graph), **does not reset the axes but autoscales the current graph-view** of plotly-resampler figures. This design choice was made as it seemed more intuitive for the developers to support this behavior with double-click than the default axes-reset behavior. The graph axes can ofcourse be resetted by using the `reset_axis` button.  If you want to give feedback and discuss this further with the developers, see issue [#49](https://github.com/predict-idlab/plotly-resampler/issues/49).
 
-## Cite
-
-Paper (preprint): https://arxiv.org/abs/2206.08703
+## Citation and papers
 
+The paper about the plotly-resampler toolkit itself (preprint): https://arxiv.org/abs/2206.08703
 ```bibtex
 @inproceedings{van2022plotly,
   title={Plotly-resampler: Effective visual analytics for large time series},
   author={Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
   booktitle={2022 IEEE Visualization and Visual Analytics (VIS)},
   pages={21--25},
   year={2022},
   organization={IEEE}
 }
 ```
 
-## Future work 🔨
+**Related papers**:
+- **Visual representativeness** of time series data point selection algorithms (preprint): https://arxiv.org/abs/2304.00900 <br>
+  code: https://github.com/predict-idlab/ts-datapoint-selection-vis
+-  **MinMaxLTTB** - an efficient data point selection algorithm (preprint): https://arxiv.org/abs/2305.00332 <br>
+  code: https://github.com/predict-idlab/MinMaxLTTB
 
-- [x] Support `.add_traces()` (currently only `.add_trace` is supported)
-- [x] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
-- [x] Integrate with [tsdownsample](https://github.com/predict-idlab/tsdownsample) :racehorse:
 
 <br>
 
 ---
 
 <p align="center">
 👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>
```

#### html2text {}

```diff
@@ -21,15 +21,35 @@
 interact with the plot (panning, zooming, ...), callbacks are used to aggregate
 data and update the figure. ![basic example gif](https://
 raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/
 _static/basic_example.gif) In [this Plotly-Resampler demo](https://github.com/
 predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
 `110,000,000` data points are visualized!       ### Installation | [**pip**]
 (https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
-| ---| ----|  ### Features :tada: * **Convenient** to use: * just add either *
+| ---| ----|
+What is the difference between plotly-resampler figures and plain plotly
+figures? `plotly-resampler` can be thought of as wrapper around plain plotly
+figures which adds visualization scalability to line-charts by dynamically
+aggregating the data w.r.t. the front-end view. `plotly-resampler` thus adds
+dynamic aggregation functionality to plain plotly figures. **Important to
+know**: * ``show`` *always* returns a static html view of the figure, i.e., no
+dynamic aggregation can be performed on that view. * To have dynamic
+aggregation: * with ``FigureResampler``, you need to call ``show_dash`` (or
+output the object in a cell via ``IPython.display``) -> which spawns a dash-web
+app, and the dynamic aggregation is realized with dash callback. * with
+``FigureWidgetResampler``, you need to use ``IPython.display`` on the object,
+which uses widget-events to realize dynamic aggregation (via the running
+IPython kernel). **Other changes of plotly-resampler figures w.r.t. vanilla
+plotly**: * **double-clicking** within a line-chart area **does not Reset
+Axes**, as it results in an âAutoscaleâ event. We decided to implement an
+Autoscale event as updating your y-range such that it shows all the data that
+is in your x-range. * **Note**: vanilla Plotly figures their Autoscale result
+in Reset Axes behavior, in our opinion this did not make a lot of sense. It is
+therefore that we have overriden this behavior in plotly-resampler.
+### Features :tada: * **Convenient** to use: * just add either *
 `register_plotly_resampler` function to your notebook with the best suited
 `mode` argument. * `FigureResampler` decorator around a plotly Figure and call
 `.show_dash()` * `FigureWidgetResampler` decorator around a plotly Figure and
 output the instance in a cell * allows all other plotly figure construction
 flexibility to be used! * **Environment-independent** * can be used in Jupyter,
 vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as
 application (on a server) * Interface for **various aggregation algorithms**: *
@@ -89,19 +109,22 @@
 **autoscale** event (triggered by the autoscale button or a double-click within
 the graph), **does not reset the axes but autoscales the current graph-view**
 of plotly-resampler figures. This design choice was made as it seemed more
 intuitive for the developers to support this behavior with double-click than
 the default axes-reset behavior. The graph axes can ofcourse be resetted by
 using the `reset_axis` button. If you want to give feedback and discuss this
 further with the developers, see issue [#49](https://github.com/predict-idlab/
-plotly-resampler/issues/49). ## Cite Paper (preprint): https://arxiv.org/abs/
-2206.08703 ```bibtex @inproceedings{van2022plotly, title={Plotly-resampler:
-Effective visual analytics for large time series}, author={Van Der Donckt,
-Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
-booktitle={2022 IEEE Visualization and Visual Analytics (VIS)}, pages={21--25},
-year={2022}, organization={IEEE} } ``` ## Future work ð¨ - [x] Support
-`.add_traces()` (currently only `.add_trace` is supported) - [x] Support
-`hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/
-plotly-resampler/pull/148) - [x] Integrate with [tsdownsample](https://
-github.com/predict-idlab/tsdownsample) :racehorse:
+plotly-resampler/issues/49). ## Citation and papers The paper about the plotly-
+resampler toolkit itself (preprint): https://arxiv.org/abs/2206.08703 ```bibtex
+@inproceedings{van2022plotly, title={Plotly-resampler: Effective visual
+analytics for large time series}, author={Van Der Donckt, Jonas and Van Der
+Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie}, booktitle={2022 IEEE
+Visualization and Visual Analytics (VIS)}, pages={21--25}, year={2022},
+organization={IEEE} } ``` **Related papers**: - **Visual representativeness**
+of time series data point selection algorithms (preprint): https://arxiv.org/
+abs/2304.00900
+code: https://github.com/predict-idlab/ts-datapoint-selection-vis -
+**MinMaxLTTB** - an efficient data point selection algorithm (preprint): https:
+//arxiv.org/abs/2305.00332
+code: https://github.com/predict-idlab/MinMaxLTTB
 ---
         ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/__init__.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.9.0rc2"
+__version__ = "0.9.0rc3"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
     "MinMaxLTTB",
     "LTTB",
```

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregation_interface.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregation_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregators.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregators.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handler_interface.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handler_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handlers.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handlers.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/plotly_aggregator_parser.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/plotly_aggregator_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,46 +34,50 @@
         ts: Union[pd.Timestamp, None], reference_tz: Union[pytz.BaseTzInfo, None]
     ) -> Union[pd.Timestamp, None]:
         """Adjust `ts` its timezone to the `reference_tz`."""
         if ts is None:
             return None
         elif reference_tz is not None:
             if ts.tz is not None:
-                assert ts.tz.zone == reference_tz.zone
+                assert ts.tz.__str__() == reference_tz.__str__()
                 return ts
             else:  # localize -> time remains the same
                 return ts.tz_localize(reference_tz)
         elif reference_tz is None and ts.tz is not None:
             return ts.tz_localize(None)
         return ts
 
     @staticmethod
-    def get_start_end_indices(hf_trace_data, start, end) -> Tuple[int, int]:
+    def get_start_end_indices(hf_trace_data, axis_type, start, end) -> Tuple[int, int]:
         """Get the start & end indices of the high-frequency data."""
         # Base case: no hf data, or both start & end are None
         if not len(hf_trace_data["x"]):
             return 0, 0
         elif start is None and end is None:
             return 0, len(hf_trace_data["x"])
 
         # NOTE: as we use bisect right for the end index, we do not need to add a
         #      small epsilon to the end value
         start = hf_trace_data["x"][0] if start is None else start
         end = hf_trace_data["x"][-1] if end is None else end
 
+        # NOTE: we must verify this before check if the x is a range-index
+        if axis_type == "log":
+            start, end = 10**start, 10**end
+
         # We can compute the start & end indices directly when it is a RangeIndex
         if isinstance(hf_trace_data["x"], pd.RangeIndex):
             x_start = hf_trace_data["x"].start
             x_step = hf_trace_data["x"].step
             start_idx = int(max((start - x_start) // x_step, 0))
             end_idx = int((end - x_start) // x_step)
             return start_idx, end_idx
         # TODO: this can be performed as-well for a fixed frequency range-index w/ freq
 
-        if hf_trace_data["axis_type"] == "date":
+        if axis_type == "date":
             start, end = pd.to_datetime(start), pd.to_datetime(end)
             # convert start & end to the same timezone
             if isinstance(hf_trace_data["x"], pd.DatetimeIndex):
                 tz = hf_trace_data["x"].tz
                 assert start.tz == end.tz
                 start = PlotlyAggregatorParser.to_same_tz(start, tz)
                 end = PlotlyAggregatorParser.to_same_tz(end, tz)
```

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,27 +322,39 @@
         # Parse trace data (necessary when updating the trace data)
         for k in _hf_data_container._fields:
             if isinstance(
                 hf_trace_data[k], (np.ndarray, pd.RangeIndex, pd.DatetimeIndex)
             ):
                 # is faster to escape the loop here than check inside the hasattr if
                 continue
-            if hasattr(hf_trace_data[k], "values"):
+            elif pd.core.dtypes.common.is_datetime64tz_dtype(hf_trace_data[k]):
+                # When we use the .values method, timezone information is lost
+                # so convert it to pd.DatetimeIndex, which preserves the tz-info
+                hf_trace_data[k] = pd.Index(hf_trace_data[k])
+            elif hasattr(hf_trace_data[k], "values"):
                 # when not a range index or datetime index
                 hf_trace_data[k] = hf_trace_data[k].values
 
         # Also check if the y-data is empty, if so, return an empty trace
         if len(hf_trace_data["y"]) == 0:
             trace["x"] = []
             trace["y"] = []
             trace["name"] = hf_trace_data["name"]
             return trace
 
+        # Leverage the axis type to get the start and end indices
+        # Note: the axis type specified in the figure layout takes precedence over the
+        # the axis type which is inferred from the data (and stored in hf_trace_data)
+        # TODO: verify if we need to use `axis`of anchor as key to determing axis type
+        axis = trace.get("xaxis", "x")
+        axis_type = self.layout._props.get(axis[:1] + "axis" + axis[1:], {}).get(
+            "type", hf_trace_data["axis_type"]
+        )
         start_idx, end_idx = PlotlyAggregatorParser.get_start_end_indices(
-            hf_trace_data, start, end
+            hf_trace_data, axis_type, start, end
         )
 
         # Return an invisible, single-point, trace when the sliced hf_series doesn't
         # contain any data in the current view
         if end_idx == start_idx:
             trace["x"] = [hf_trace_data["x"][0]]
             trace["y"] = [None]
@@ -578,21 +590,25 @@
         Returns
         -------
         _hf_data_container
             A namedtuple which serves as a datacontainer.
 
         """
         hf_x: np.ndarray = (
+            # fmt: off
             (np.asarray(trace["x"]) if trace["x"] is not None else None)
             if hasattr(trace, "x") and hf_x is None
-            else hf_x.values
-            if isinstance(hf_x, pd.Series)
-            else hf_x
-            if isinstance(hf_x, pd.Index)
+            # If we cast a tz-aware datetime64 array to `.values` we lose the tz-info 
+            # and the UTC time will be displayed instead of the tz-localized time, 
+            # hence we cast to a pd.DatetimeIndex, which preserves the tz-info
+            else pd.Index(hf_x) if pd.core.dtypes.common.is_datetime64tz_dtype(hf_x)
+            else hf_x.values if isinstance(hf_x, pd.Series)
+            else hf_x if isinstance(hf_x, pd.Index)
             else np.asarray(hf_x)
+            # fmt: on
         )
 
         hf_y = (
             trace["y"]
             if hasattr(trace, "y") and hf_y is None
             else hf_y.values
             if isinstance(hf_y, (pd.Series, pd.Index))
```

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/utils.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/plotly_resampler/registering.py` & `plotly_resampler-0.9.0rc3/plotly_resampler/registering.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc2/pyproject.toml` & `plotly_resampler-0.9.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.9.0rc2"
+version = "0.9.0rc3"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
 documentation = "https://predict-idlab.github.io/plotly-resampler"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
```

### Comparing `plotly_resampler-0.9.0rc2/PKG-INFO` & `plotly_resampler-0.9.0rc3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotly-resampler
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: Visualizing large time series with plotly
 Home-page: https://github.com/predict-idlab/plotly-resampler
 License: MIT
 Keywords: time-series,visualization,resampling,plotly,plotly-dash
 Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,15 +60,14 @@
 
 > `plotly_resampler`: visualize large sequential data by **adding resampling functionality to Plotly figures**
 
 [Plotly](https://github.com/plotly/plotly.py) is an awesome interactive visualization library, however it can get pretty slow when a lot of data points are visualized (100 000+ datapoints). This library solves this by downsampling (aggregating) the data respective to the view and then plotting the aggregated points. When you interact with the plot (panning, zooming, ...), callbacks are used to aggregate data and update the figure.
 
 ![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/basic_example.gif)
 
-
 In [this Plotly-Resampler demo](https://github.com/predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over `110,000,000` data points are visualized!
 
 <!-- These dynamic aggregation callbacks are realized with: -->
 <!-- * [Dash](https://github.com/plotly/dash) when a `go.Figure` object is wrapped with dynamic aggregation functionality, see example ⬆️. -->
 <!-- * The [FigureWidget.layout.on_change](https://plotly.com/python-api-reference/generated/plotly.html?highlight=on_change#plotly.basedatatypes.BasePlotlyType.on_change) method, when a `go.FigureWidget` is used within a `.ipynb` environment. -->
 
 <!-- #### Useful links -->
@@ -78,14 +77,33 @@
 
 ### Installation
 
 | [**pip**](https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
 | ---| ----|
 <!-- | [**conda**](https://anaconda.org/conda-forge/plotly_resampler/) | `conda install -c conda-forge plotly_resampler` | -->
 
+<br>
+<details><summary><b>What is the difference between plotly-resampler figures and plain plotly figures?</b></summary>
+
+`plotly-resampler` can be thought of as wrapper around plain plotly figures which adds visualization scalability to line-charts by dynamically aggregating the data w.r.t. the front-end view. `plotly-resampler` thus adds dynamic aggregation functionality to plain plotly figures.
+
+**Important to know**:
+
+* ``show`` *always* returns a static html view of the figure, i.e., no dynamic aggregation can be performed on that view.
+* To have dynamic aggregation:
+
+  * with ``FigureResampler``, you need to call ``show_dash`` (or output the object in a cell via ``IPython.display``) -> which spawns a dash-web app, and the dynamic aggregation is realized with dash callback.
+  * with ``FigureWidgetResampler``, you need to use ``IPython.display`` on the object, which uses widget-events to realize dynamic aggregation (via the running IPython kernel).
+
+**Other changes of plotly-resampler figures w.r.t. vanilla plotly**:
+
+* **double-clicking** within a line-chart area **does not Reset Axes**, as it results in an “Autoscale” event. We decided to implement an Autoscale event as updating your y-range such that it shows all the data that is in your x-range.
+   * **Note**: vanilla Plotly figures their Autoscale result in Reset Axes behavior, in our opinion this did not make a lot of sense. It is therefore that we have overriden this behavior in plotly-resampler.
+</details><br>
+
 ### Features :tada:
 
   * **Convenient** to use:
     * just add either
       * `register_plotly_resampler` function to your notebook with the best suited `mode` argument.
       * `FigureResampler` decorator around a plotly Figure and call `.show_dash()`
       * `FigureWidgetResampler` decorator around a plotly Figure and output the instance in a cell
@@ -179,34 +197,34 @@
 * When running the code on a server, you should forward the port of the `FigureResampler.show_dash()` method to your local machine.<br>
   **Note** that you can add dynamic aggregation to plotly figures with the `FigureWidgetResampler` wrapper without needing to forward a port!
 * The `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation functionality, so when this main thread is occupied, no resampling logic can be executed. For example; if you perform long computations within your notebook, the kernel will be occupied during these computations, and will only execute the resampling operations that take place during these computations after finishing that computation.
 * In general, when using downsampling one should be aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing) effects.
   The <b style="color:orange">[R]</b> in the legend indicates when the corresponding trace is being resampled (and thus possibly distorted) or not. Additionally, the `~<range>` suffix represent the mean aggregation bin size in terms of the sequence index.
 * The plotly **autoscale** event (triggered by the autoscale button or a double-click within the graph), **does not reset the axes but autoscales the current graph-view** of plotly-resampler figures. This design choice was made as it seemed more intuitive for the developers to support this behavior with double-click than the default axes-reset behavior. The graph axes can ofcourse be resetted by using the `reset_axis` button.  If you want to give feedback and discuss this further with the developers, see issue [#49](https://github.com/predict-idlab/plotly-resampler/issues/49).
 
-## Cite
-
-Paper (preprint): https://arxiv.org/abs/2206.08703
+## Citation and papers
 
+The paper about the plotly-resampler toolkit itself (preprint): https://arxiv.org/abs/2206.08703
 ```bibtex
 @inproceedings{van2022plotly,
   title={Plotly-resampler: Effective visual analytics for large time series},
   author={Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
   booktitle={2022 IEEE Visualization and Visual Analytics (VIS)},
   pages={21--25},
   year={2022},
   organization={IEEE}
 }
 ```
 
-## Future work 🔨
+**Related papers**:
+- **Visual representativeness** of time series data point selection algorithms (preprint): https://arxiv.org/abs/2304.00900 <br>
+  code: https://github.com/predict-idlab/ts-datapoint-selection-vis
+-  **MinMaxLTTB** - an efficient data point selection algorithm (preprint): https://arxiv.org/abs/2305.00332 <br>
+  code: https://github.com/predict-idlab/MinMaxLTTB
 
-- [x] Support `.add_traces()` (currently only `.add_trace` is supported)
-- [x] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
-- [x] Integrate with [tsdownsample](https://github.com/predict-idlab/tsdownsample) :racehorse:
 
 <br>
 
 ---
 
 <p align="center">
 👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc2 Summary:
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc3 Summary:
 Visualizing large time series with plotly Home-page: https://github.com/
 predict-idlab/plotly-resampler License: MIT Keywords: time-
 series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
@@ -48,15 +48,35 @@
 interact with the plot (panning, zooming, ...), callbacks are used to aggregate
 data and update the figure. ![basic example gif](https://
 raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/
 _static/basic_example.gif) In [this Plotly-Resampler demo](https://github.com/
 predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
 `110,000,000` data points are visualized!       ### Installation | [**pip**]
 (https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
-| ---| ----|  ### Features :tada: * **Convenient** to use: * just add either *
+| ---| ----|
+What is the difference between plotly-resampler figures and plain plotly
+figures? `plotly-resampler` can be thought of as wrapper around plain plotly
+figures which adds visualization scalability to line-charts by dynamically
+aggregating the data w.r.t. the front-end view. `plotly-resampler` thus adds
+dynamic aggregation functionality to plain plotly figures. **Important to
+know**: * ``show`` *always* returns a static html view of the figure, i.e., no
+dynamic aggregation can be performed on that view. * To have dynamic
+aggregation: * with ``FigureResampler``, you need to call ``show_dash`` (or
+output the object in a cell via ``IPython.display``) -> which spawns a dash-web
+app, and the dynamic aggregation is realized with dash callback. * with
+``FigureWidgetResampler``, you need to use ``IPython.display`` on the object,
+which uses widget-events to realize dynamic aggregation (via the running
+IPython kernel). **Other changes of plotly-resampler figures w.r.t. vanilla
+plotly**: * **double-clicking** within a line-chart area **does not Reset
+Axes**, as it results in an âAutoscaleâ event. We decided to implement an
+Autoscale event as updating your y-range such that it shows all the data that
+is in your x-range. * **Note**: vanilla Plotly figures their Autoscale result
+in Reset Axes behavior, in our opinion this did not make a lot of sense. It is
+therefore that we have overriden this behavior in plotly-resampler.
+### Features :tada: * **Convenient** to use: * just add either *
 `register_plotly_resampler` function to your notebook with the best suited
 `mode` argument. * `FigureResampler` decorator around a plotly Figure and call
 `.show_dash()` * `FigureWidgetResampler` decorator around a plotly Figure and
 output the instance in a cell * allows all other plotly figure construction
 flexibility to be used! * **Environment-independent** * can be used in Jupyter,
 vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as
 application (on a server) * Interface for **various aggregation algorithms**: *
@@ -116,19 +136,22 @@
 **autoscale** event (triggered by the autoscale button or a double-click within
 the graph), **does not reset the axes but autoscales the current graph-view**
 of plotly-resampler figures. This design choice was made as it seemed more
 intuitive for the developers to support this behavior with double-click than
 the default axes-reset behavior. The graph axes can ofcourse be resetted by
 using the `reset_axis` button. If you want to give feedback and discuss this
 further with the developers, see issue [#49](https://github.com/predict-idlab/
-plotly-resampler/issues/49). ## Cite Paper (preprint): https://arxiv.org/abs/
-2206.08703 ```bibtex @inproceedings{van2022plotly, title={Plotly-resampler:
-Effective visual analytics for large time series}, author={Van Der Donckt,
-Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
-booktitle={2022 IEEE Visualization and Visual Analytics (VIS)}, pages={21--25},
-year={2022}, organization={IEEE} } ``` ## Future work ð¨ - [x] Support
-`.add_traces()` (currently only `.add_trace` is supported) - [x] Support
-`hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/
-plotly-resampler/pull/148) - [x] Integrate with [tsdownsample](https://
-github.com/predict-idlab/tsdownsample) :racehorse:
+plotly-resampler/issues/49). ## Citation and papers The paper about the plotly-
+resampler toolkit itself (preprint): https://arxiv.org/abs/2206.08703 ```bibtex
+@inproceedings{van2022plotly, title={Plotly-resampler: Effective visual
+analytics for large time series}, author={Van Der Donckt, Jonas and Van Der
+Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie}, booktitle={2022 IEEE
+Visualization and Visual Analytics (VIS)}, pages={21--25}, year={2022},
+organization={IEEE} } ``` **Related papers**: - **Visual representativeness**
+of time series data point selection algorithms (preprint): https://arxiv.org/
+abs/2304.00900
+code: https://github.com/predict-idlab/ts-datapoint-selection-vis -
+**MinMaxLTTB** - an efficient data point selection algorithm (preprint): https:
+//arxiv.org/abs/2305.00332
+code: https://github.com/predict-idlab/MinMaxLTTB
 ---
         ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

