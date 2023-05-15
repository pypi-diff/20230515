# Comparing `tmp/types-openpyxl-3.1.0.7.tar.gz` & `tmp/types-openpyxl-3.1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-openpyxl-3.1.0.7.tar", last modified: Wed May 10 15:21:15 2023, max compression
+gzip compressed data, was "types-openpyxl-3.1.0.8.tar", last modified: Mon May 15 12:30:39 2023, max compression
```

## Comparing `types-openpyxl-3.1.0.7.tar` & `types-openpyxl-3.1.0.8.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-10 15:21:14.000000 types-openpyxl-3.1.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:14.000000 types-openpyxl-3.1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.499220 types-openpyxl-3.1.0.7/openpyxl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:21:14.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/_constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.499220 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/rich_text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/cell/text.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.503220 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/area_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/bar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/bubble_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/chartspace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/data_source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/error_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/legend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/line_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/marker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/pie_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/pivot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/plotarea.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/radar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/scatter_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/series.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/series_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/shapes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/stock_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/surface_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/title.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/trendline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chart/updown_bars.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.503220 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/chartsheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/publish.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.507220 types-openpyxl-3.1.0.7/openpyxl-stubs/comments/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/comments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/comments/author.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/comments/comment_sheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/comments/comments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/comments/shape_writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.507220 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/product.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/singleton.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/compat/strings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.507220 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/nested.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/serialisable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/slots.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.511220 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/connector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/effect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/fill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/graphic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/line.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18284 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/xdr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.511220 types-openpyxl-3.1.0.7/openpyxl-stubs/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/formatting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/formatting/formatting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/formatting/rule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.511220 types-openpyxl-3.1.0.7/openpyxl-stubs/formula/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/formula/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/formula/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/formula/translate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.511220 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/extended.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/interface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/relationship.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.511220 types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34488 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.511220 types-openpyxl-3.1.0.7/openpyxl-stubs/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/reader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/reader/drawings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/reader/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/reader/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/reader/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.515220 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/alignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/borders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/cell_style.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/differential.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/fills.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/named_styles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/styleable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/stylesheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/styles/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.515220 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/bound_dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/dataframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/escape.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/formulas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/indexed_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/inference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/utils/units.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.519220 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/child.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/defined_name.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.519220 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/external_link/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/external_link/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/external_link/external.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/external_reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/function_group.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/smart_tags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/web.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_write_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/cell_range.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/cell_watch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/controls.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/copier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/datavalidation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/dimensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/formula.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/header_footer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/hyperlink.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/ole.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/page.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/pagebreak.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/related.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/scenario.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/smart_tag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/worksheet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/openpyxl-stubs/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/writer/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/writer/theme.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/openpyxl-stubs/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/xml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/xml/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 15:19:44.000000 types-openpyxl-3.1.0.7/openpyxl-stubs/xml/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-10 15:21:14.000000 types-openpyxl-3.1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:15.523220 types-openpyxl-3.1.0.7/types_openpyxl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:21:15.000000 types-openpyxl-3.1.0.7/types_openpyxl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-10 15:21:15.000000 types-openpyxl-3.1.0.7/types_openpyxl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:15.000000 types-openpyxl-3.1.0.7/types_openpyxl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:21:15.000000 types-openpyxl-3.1.0.7/types_openpyxl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.743408 types-openpyxl-3.1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-15 12:30:39.743408 types-openpyxl-3.1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.723408 types-openpyxl-3.1.0.8/openpyxl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/_constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.723408 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/rich_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/text.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/area_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bubble_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/chartspace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/data_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/error_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/line_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/marker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pie_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pivot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/plotarea.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/radar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/scatter_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/series.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/series_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/shapes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/stock_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/surface_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/title.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/trendline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/updown_bars.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/chartsheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/publish.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/author.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/comment_sheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/comments.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/shape_writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/singleton.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/strings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/nested.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/serialisable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/slots.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/connector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/effect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/fill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/graphic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/xdr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/formatting.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/rule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/translate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/extended.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/interface.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/relationship.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/record.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/drawings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/alignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/borders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/cell_style.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/differential.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fills.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/named_styles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/styleable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/stylesheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/bound_dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/dataframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/escape.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/formulas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/indexed_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/inference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/units.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/child.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/defined_name.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_link/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_link/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_link/external.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/function_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/smart_tags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/web.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_write_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/cell_range.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/cell_watch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/controls.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/copier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/datavalidation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/dimensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/formula.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/header_footer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/hyperlink.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/ole.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/page.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/pagebreak.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/scenario.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/smart_tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/worksheet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/theme.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:30:39.743408 types-openpyxl-3.1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/top_level.txt
```

### Comparing `types-openpyxl-3.1.0.7/CHANGELOG.md` & `types-openpyxl-3.1.0.8/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.1.0.8 (2023-05-15)
+
+openpyxl: Type MetaSerialisable dunders (#10170)
+
+Typed `Serialisable.__attrs__`, `Serialisable.__nested__`, `Serialisable.__elements__`, and `Serialisable.__namespaced__` ClassVars.
+
 ## 3.1.0.7 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 3.1.0.6 (2023-05-10)
 
 [openpyxl] Complete base descriptors (#10001)
```

### Comparing `types-openpyxl-3.1.0.7/PKG-INFO` & `types-openpyxl-3.1.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.7
+Version: 3.1.0.8
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `2d5dafadb75f122e0c2aeced09a5b72232373f40`.
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/cell/cell.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/cell/read_only.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/cell/rich_text.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/rich_text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/cell/text.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/text.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Alias, Integer, NoneSet, Typed, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.fonts import Font
 
 _PhoneticPropertiesType: TypeAlias = Literal["halfwidthKatakana", "fullwidthKatakana", "Hiragana", "noConversion"]
@@ -43,15 +44,15 @@
     condense: Incomplete
     extend: Incomplete
     color: Incomplete
     sz: Incomplete
     u: Incomplete
     vertAlign: Incomplete
     scheme: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         rFont: Incomplete | None = None,
         charset: Incomplete | None = None,
         family: Incomplete | None = None,
         b: Incomplete | None = None,
         i: Incomplete | None = None,
@@ -69,24 +70,24 @@
 
 class RichText(Serialisable):
     tagname: str
     rPr: Typed[InlineFont, Literal[True]]
     font: Alias
     t: Incomplete
     text: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rPr: InlineFont | None = None, t: Incomplete | None = None) -> None: ...
 
 class Text(Serialisable):
     tagname: str
     t: Incomplete
     plain: Alias
     r: Incomplete
     formatted: Alias
     rPh: Incomplete
     phonetic: Alias
     phoneticPr: Typed[_PhoneticProperties, Literal[True]]
     PhoneticProperties: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, t: Incomplete | None = None, r=(), rPh=(), phoneticPr: _PhoneticProperties | None = None) -> None: ...
     @property
     def content(self): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/_3d.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_3d.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
@@ -16,15 +17,15 @@
     rotY: Incomplete
     y_rotation: Alias
     depthPercent: Incomplete
     rAngAx: Incomplete
     right_angle_axes: Alias
     perspective: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         rotX: int = 15,
         hPercent: Incomplete | None = None,
         rotY: int = 20,
         depthPercent: Incomplete | None = None,
         rAngAx: bool = True,
@@ -35,15 +36,15 @@
 class Surface(Serialisable):
     tagname: str
     thickness: Incomplete
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     pictureOptions: Typed[PictureOptions, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         thickness: Incomplete | None = None,
         spPr: GraphicalProperties | None = None,
         pictureOptions: PictureOptions | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/__init__.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_chart.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.legend import Legend
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.descriptors.base import Alias, Bool, Integer, MinMax, Set, Typed, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
@@ -28,15 +29,15 @@
     title: Incomplete
     anchor: str
     width: int
     height: float
     style: MinMax[float, Literal[True]]
     mime_type: str
     graphical_properties: Typed[GraphicalProperties, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     plot_area: Incomplete
     pivotSource: Incomplete
     pivotFormats: Incomplete
     idx_base: int
     def __init__(self, axId=(), **kw: Unused) -> None: ...
     def __hash__(self) -> int: ...
     def __iadd__(self, other): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/area_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bubble_chart.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,37 @@
 from _typeshed import Incomplete, Unused
-from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
+from openpyxl.chart.axis import NumericAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 
 from ._chart import ChartBase
 
-class _AreaChartBase(ChartBase):
-    grouping: Incomplete
+class BubbleChart(ChartBase):
+    tagname: str
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
-    dropLines: Typed[ChartLines, Literal[True]]
-    __elements__: Incomplete
+    bubble3D: Incomplete
+    bubbleScale: Incomplete
+    showNegBubbles: Incomplete
+    sizeRepresents: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[NumericAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        grouping: str = "standard",
         varyColors: Incomplete | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
-        dropLines: ChartLines | None = None,
+        bubble3D: Incomplete | None = None,
+        bubbleScale: Incomplete | None = None,
+        showNegBubbles: Incomplete | None = None,
+        sizeRepresents: Incomplete | None = None,
+        extLst: Unused = None,
+        **kw,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
-
-class AreaChart(_AreaChartBase):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    x_axis: Typed[TextAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, axId: Unused = None, extLst: Unused = None, **kw) -> None: ...
-
-class AreaChart3D(AreaChart):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    gapDepth: Incomplete
-    x_axis: Typed[TextAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
-    z_axis: Typed[SeriesAxis, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, gapDepth: Incomplete | None = None, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/axis.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/axis.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText, Text
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
@@ -18,15 +19,15 @@
 class Scaling(Serialisable):
     tagname: str
     logBase: Incomplete
     orientation: Incomplete
     max: Incomplete
     min: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         logBase: Incomplete | None = None,
         orientation: str = "minMax",
         max: Incomplete | None = None,
         min: Incomplete | None = None,
         extLst: Unused = None,
@@ -48,15 +49,15 @@
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textProperties: Alias
     crossAx: Incomplete
     crosses: Incomplete
     crossesAt: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         axId: Incomplete | None = None,
         scaling: Scaling | None = None,
         delete: Incomplete | None = None,
         axPos: str = "l",
         majorGridlines: ChartLines | None = None,
@@ -81,30 +82,30 @@
     layout: Typed[Layout, Literal[True]]
     tx: Typed[Text, Literal[True]]
     text: Alias
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textPropertes: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         layout: Layout | None = None,
         tx: Text | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
     ) -> None: ...
 
 class DisplayUnitsLabelList(Serialisable):
     tagname: str
     custUnit: Incomplete
     builtInUnit: Incomplete
     dispUnitsLbl: Typed[DisplayUnitsLabel, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         custUnit: Incomplete | None = None,
         builtInUnit: Incomplete | None = None,
         dispUnitsLbl: DisplayUnitsLabel | None = None,
         extLst: Unused = None,
     ) -> None: ...
@@ -128,15 +129,15 @@
     crosses: Incomplete
     crossesAt: Incomplete
     crossBetween: Incomplete
     majorUnit: Incomplete
     minorUnit: Incomplete
     dispUnits: Typed[DisplayUnitsLabelList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         crossBetween: Incomplete | None = None,
         majorUnit: Incomplete | None = None,
         minorUnit: Incomplete | None = None,
         dispUnits: DisplayUnitsLabelList | None = None,
         extLst: Unused = None,
@@ -166,15 +167,15 @@
     auto: Incomplete
     lblAlgn: Incomplete
     lblOffset: Incomplete
     tickLblSkip: Incomplete
     tickMarkSkip: Incomplete
     noMultiLvlLbl: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         auto: Incomplete | None = None,
         lblAlgn: Incomplete | None = None,
         lblOffset: int = 100,
         tickLblSkip: Incomplete | None = None,
         tickMarkSkip: Incomplete | None = None,
@@ -205,15 +206,15 @@
     lblOffset: Incomplete
     baseTimeUnit: Incomplete
     majorUnit: Incomplete
     majorTimeUnit: Incomplete
     minorUnit: Incomplete
     minorTimeUnit: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         auto: Incomplete | None = None,
         lblOffset: Incomplete | None = None,
         baseTimeUnit: Incomplete | None = None,
         majorUnit: Incomplete | None = None,
         majorTimeUnit: Incomplete | None = None,
@@ -240,11 +241,11 @@
     txPr: Incomplete
     crossAx: Incomplete
     crosses: Incomplete
     crossesAt: Incomplete
     tickLblSkip: Incomplete
     tickMarkSkip: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, tickLblSkip: Incomplete | None = None, tickMarkSkip: Incomplete | None = None, extLst: Unused = None, **kw
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/bar_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bar_chart.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 
@@ -14,15 +15,15 @@
     barDir: Incomplete
     type: Alias
     grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         barDir: str = "col",
         grouping: str = "clustered",
         varyColors: Incomplete | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
@@ -41,15 +42,15 @@
     dLbls: Incomplete
     gapWidth: Incomplete
     overlap: Incomplete
     serLines: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     legend: Incomplete
     def __init__(
         self,
         gapWidth: int = 150,
         overlap: Incomplete | None = None,
         serLines: ChartLines | None = None,
         extLst: Unused = None,
@@ -71,15 +72,15 @@
     gapDepth: Incomplete
     shape: Incomplete
     serLines: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
     z_axis: Typed[SeriesAxis, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         gapWidth: int = 150,
         gapDepth: int = 150,
         shape: Incomplete | None = None,
         serLines: ChartLines | None = None,
         extLst: Unused = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/bubble_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/record.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import NumericAxis
-from openpyxl.chart.label import DataLabelList
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.serialisable import Serialisable
 
-from ._chart import ChartBase
-
-class BubbleChart(ChartBase):
+class Record(Serialisable):
     tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Typed[DataLabelList, Literal[True]]
-    dataLabels: Alias
-    bubble3D: Incomplete
-    bubbleScale: Incomplete
-    showNegBubbles: Incomplete
-    sizeRepresents: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[NumericAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
-    __elements__: Incomplete
+    m: Incomplete
+    n: Incomplete
+    b: Incomplete
+    e: Incomplete
+    s: Incomplete
+    d: Incomplete
+    x: Incomplete
     def __init__(
         self,
-        varyColors: Incomplete | None = None,
-        ser=(),
-        dLbls: DataLabelList | None = None,
-        bubble3D: Incomplete | None = None,
-        bubbleScale: Incomplete | None = None,
-        showNegBubbles: Incomplete | None = None,
-        sizeRepresents: Incomplete | None = None,
-        extLst: Unused = None,
-        **kw,
+        _fields=(),
+        m: Incomplete | None = None,
+        n: Incomplete | None = None,
+        b: Incomplete | None = None,
+        e: Incomplete | None = None,
+        s: Incomplete | None = None,
+        d: Incomplete | None = None,
+        x: Incomplete | None = None,
     ) -> None: ...
+
+class RecordList(Serialisable):
+    mime_type: str
+    rel_type: str
+    tagname: str
+    r: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
+    def __init__(self, count: Unused = None, r=(), extLst: ExtensionList | None = None) -> None: ...
+    @property
+    def count(self): ...
+    def to_tree(self): ...
+    @property
+    def path(self): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/chartspace.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/chartspace.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
 from openpyxl.chart.legend import Legend
 from openpyxl.chart.pivot import PivotSource
 from openpyxl.chart.plotarea import PlotArea
 from openpyxl.chart.print_settings import PrintSettings
 from openpyxl.chart.shapes import GraphicalProperties
@@ -25,15 +25,15 @@
     backWall: Incomplete
     plotArea: Typed[PlotArea, Literal[False]]
     legend: Typed[Legend, Literal[True]]
     plotVisOnly: Incomplete
     dispBlanksAs: Incomplete
     showDLblsOverMax: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         title: Title | None = None,
         autoTitleDeleted: Incomplete | None = None,
         pivotFmts=(),
         view3D: Incomplete | None = None,
         floor: Incomplete | None = None,
@@ -50,15 +50,15 @@
 class Protection(Serialisable):
     tagname: str
     chartObject: Incomplete
     data: Incomplete
     formatting: Incomplete
     selection: Incomplete
     userInterface: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         chartObject: Incomplete | None = None,
         data: Incomplete | None = None,
         formatting: Incomplete | None = None,
         selection: Incomplete | None = None,
         userInterface: Incomplete | None = None,
@@ -87,15 +87,15 @@
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textProperties: Alias
     externalData: Typed[ExternalData, Literal[True]]
     printSettings: Typed[PrintSettings, Literal[True]]
     userShapes: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         date1904: Incomplete | None = None,
         lang: Incomplete | None = None,
         roundedCorners: Incomplete | None = None,
         style: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/data_source.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/data_source.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import NoReturn, overload
+from typing import ClassVar, NoReturn, overload
 from typing_extensions import Literal
 
 from openpyxl.descriptors import Strict
 from openpyxl.descriptors.base import Alias, Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
@@ -25,74 +25,74 @@
     def __init__(self, idx: _ConvertibleToInt, formatCode: Incomplete | None = None, v: Incomplete | None = None) -> None: ...
 
 class NumData(Serialisable):
     formatCode: Incomplete
     ptCount: Incomplete
     pt: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, formatCode: Incomplete | None = None, ptCount: Incomplete | None = None, pt=(), extLst: Unused = None
     ) -> None: ...
 
 class NumRef(Serialisable):
     f: Incomplete
     ref: Alias
     numCache: Typed[NumData, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, f: Incomplete | None = None, numCache: NumData | None = None, extLst: Unused = None) -> None: ...
 
 class StrVal(Serialisable):
     tagname: str
     idx: Integer[Literal[False]]
     v: Incomplete
     def __init__(self, idx: _ConvertibleToInt = 0, v: Incomplete | None = None) -> None: ...
 
 class StrData(Serialisable):
     tagname: str
     ptCount: Incomplete
     pt: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, ptCount: Incomplete | None = None, pt=(), extLst: Unused = None) -> None: ...
 
 class StrRef(Serialisable):
     tagname: str
     f: Incomplete
     strCache: Typed[StrData, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, f: Incomplete | None = None, strCache: StrData | None = None, extLst: Unused = None) -> None: ...
 
 class NumDataSource(Serialisable):
     numRef: Typed[NumRef, Literal[True]]
     numLit: Typed[NumData, Literal[True]]
     def __init__(self, numRef: NumRef | None = None, numLit: NumData | None = None) -> None: ...
 
 class Level(Serialisable):
     tagname: str
     pt: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, pt=()) -> None: ...
 
 class MultiLevelStrData(Serialisable):
     tagname: str
     ptCount: Integer[Literal[True]]
     lvl: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, ptCount: _ConvertibleToInt | None = None, lvl=(), extLst: Unused = None) -> None: ...
 
 class MultiLevelStrRef(Serialisable):
     tagname: str
     f: Incomplete
     multiLvlStrCache: Typed[MultiLevelStrData, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, f: Incomplete | None = None, multiLvlStrCache: MultiLevelStrData | None = None, extLst: Unused = None
     ) -> None: ...
 
 class AxDataSource(Serialisable):
     tagname: str
     numRef: Typed[NumRef, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/descriptors.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/descriptors.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/error_bar.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/error_bar.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.data_source import NumDataSource
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
@@ -18,15 +19,15 @@
     noEndCap: Incomplete
     plus: Typed[NumDataSource, Literal[True]]
     minus: Typed[NumDataSource, Literal[True]]
     val: Incomplete
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         errDir: Incomplete | None = None,
         errBarType: str = "both",
         errValType: str = "fixedVal",
         noEndCap: Incomplete | None = None,
         plus: NumDataSource | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/label.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/label.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable as Serialisable
@@ -21,15 +22,15 @@
     showCatName: Incomplete
     showSerName: Incomplete
     showPercent: Incomplete
     showBubbleSize: Incomplete
     showLeaderLines: Incomplete
     separator: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         numFmt: Incomplete | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
         dLblPos: Incomplete | None = None,
         showLegendKey: Incomplete | None = None,
@@ -58,15 +59,15 @@
     showCatName: Incomplete
     showSerName: Incomplete
     showPercent: Incomplete
     showBubbleSize: Incomplete
     showLeaderLines: Incomplete
     separator: Incomplete
     extLst: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, idx: int = 0, **kw) -> None: ...
 
 class DataLabelList(_DataLabelBase):
     tagname: str
     dLbl: Incomplete
     delete: Incomplete
     numFmt: Incomplete
@@ -78,9 +79,9 @@
     showCatName: Incomplete
     showSerName: Incomplete
     showPercent: Incomplete
     showBubbleSize: Incomplete
     showLeaderLines: Incomplete
     separator: Incomplete
     extLst: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, dLbl=(), delete: Incomplete | None = None, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/layout.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pivot.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
+from openpyxl.chart.label import DataLabel as _DataLabel
+from openpyxl.chart.marker import Marker
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class ManualLayout(Serialisable):
+class PivotSource(Serialisable):
     tagname: str
-    layoutTarget: Incomplete
-    xMode: Incomplete
-    yMode: Incomplete
-    wMode: Incomplete
-    hMode: Incomplete
-    x: Incomplete
-    y: Incomplete
-    w: Incomplete
-    width: Alias
-    h: Incomplete
-    height: Alias
+    name: Incomplete
+    fmtId: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, name: str | None = None, fmtId: Incomplete | None = None, extLst: Unused = None) -> None: ...
+
+class PivotFormat(Serialisable):
+    tagname: str
+    idx: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    TextBody: Alias
+    marker: Typed[Marker, Literal[True]]
+    dLbl: Typed[_DataLabel, Literal[True]]
+    DataLabel: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        layoutTarget: Incomplete | None = None,
-        xMode: Incomplete | None = None,
-        yMode: Incomplete | None = None,
-        wMode: str = "factor",
-        hMode: str = "factor",
-        x: Incomplete | None = None,
-        y: Incomplete | None = None,
-        w: Incomplete | None = None,
-        h: Incomplete | None = None,
+        idx: int = 0,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        marker: Marker | None = None,
+        dLbl: _DataLabel | None = None,
         extLst: Unused = None,
     ) -> None: ...
-
-class Layout(Serialisable):
-    tagname: str
-    manualLayout: Typed[ManualLayout, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, manualLayout: ManualLayout | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/legend.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/legend.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
@@ -10,30 +11,30 @@
 
 class LegendEntry(Serialisable):
     tagname: str
     idx: Incomplete
     delete: Incomplete
     txPr: Typed[RichText, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, idx: int = 0, delete: bool = False, txPr: RichText | None = None, extLst: Unused = None) -> None: ...
 
 class Legend(Serialisable):
     tagname: str
     legendPos: Incomplete
     position: Alias
     legendEntry: Incomplete
     layout: Typed[Layout, Literal[True]]
     overlay: Incomplete
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         legendPos: str = "r",
         legendEntry=(),
         layout: Layout | None = None,
         overlay: Incomplete | None = None,
         spPr: GraphicalProperties | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/line_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/plotarea.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,73 @@
 from _typeshed import Incomplete, Unused
-from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import ChartLines, NumericAxis, _BaseAxis
-from openpyxl.chart.label import DataLabelList
-from openpyxl.chart.updown_bars import UpDownBars
+from openpyxl.chart.layout import Layout
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.serialisable import Serialisable
 
-from ._chart import ChartBase
-
-class _LineChartBase(ChartBase):
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Typed[DataLabelList, Literal[True]]
-    dataLabels: Alias
-    dropLines: Typed[ChartLines, Literal[True]]
-    __elements__: Incomplete
-    def __init__(
-        self,
-        grouping: str = "standard",
-        varyColors: Incomplete | None = None,
-        ser=(),
-        dLbls: DataLabelList | None = None,
-        dropLines: ChartLines | None = None,
-        **kw,
-    ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
-
-class LineChart(_LineChartBase):
+class DataTable(Serialisable):
     tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    hiLowLines: Typed[ChartLines, Literal[True]]
-    upDownBars: Typed[UpDownBars, Literal[True]]
-    marker: Incomplete
-    smooth: Incomplete
+    showHorzBorder: Incomplete
+    showVertBorder: Incomplete
+    showOutline: Incomplete
+    showKeys: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[_BaseAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        hiLowLines: ChartLines | None = None,
-        upDownBars: UpDownBars | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
+        showHorzBorder: Incomplete | None = None,
+        showVertBorder: Incomplete | None = None,
+        showOutline: Incomplete | None = None,
+        showKeys: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
         extLst: Unused = None,
-        **kw,
     ) -> None: ...
 
-class LineChart3D(_LineChartBase):
+class PlotArea(Serialisable):
     tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    gapDepth: Incomplete
-    hiLowLines: Typed[ChartLines, Literal[True]]
-    upDownBars: Typed[UpDownBars, Literal[True]]
-    marker: Incomplete
-    smooth: Incomplete
+    layout: Typed[Layout, Literal[True]]
+    dTable: Typed[DataTable, Literal[True]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[ExtensionList, Literal[False]]
-    y_axis: Typed[ExtensionList, Literal[False]]
-    z_axis: Typed[ExtensionList, Literal[False]]
-    __elements__: Incomplete
+    areaChart: Incomplete
+    area3DChart: Incomplete
+    lineChart: Incomplete
+    line3DChart: Incomplete
+    stockChart: Incomplete
+    radarChart: Incomplete
+    scatterChart: Incomplete
+    pieChart: Incomplete
+    pie3DChart: Incomplete
+    doughnutChart: Incomplete
+    barChart: Incomplete
+    bar3DChart: Incomplete
+    ofPieChart: Incomplete
+    surfaceChart: Incomplete
+    surface3DChart: Incomplete
+    bubbleChart: Incomplete
+    valAx: Incomplete
+    catAx: Incomplete
+    dateAx: Incomplete
+    serAx: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        gapDepth: Incomplete | None = None,
-        hiLowLines: ChartLines | None = None,
-        upDownBars: UpDownBars | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
-        **kw,
+        layout: Layout | None = None,
+        dTable: DataTable | None = None,
+        spPr: GraphicalProperties | None = None,
+        _charts=(),
+        _axes=(),
+        extLst: Unused = None,
     ) -> None: ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    @classmethod
+    def from_tree(cls, node): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/marker.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/marker.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
@@ -10,15 +11,15 @@
 class Marker(Serialisable):
     tagname: str
     symbol: Incomplete
     size: Incomplete
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         symbol: Incomplete | None = None,
         size: Incomplete | None = None,
         spPr: GraphicalProperties | None = None,
         extLst: Unused = None,
     ) -> None: ...
@@ -30,15 +31,15 @@
     marker: Typed[Marker, Literal[True]]
     bubble3D: Incomplete
     explosion: Incomplete
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     pictureOptions: Typed[PictureOptions, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         idx: Incomplete | None = None,
         invertIfNegative: Incomplete | None = None,
         marker: Marker | None = None,
         bubble3D: Incomplete | None = None,
         explosion: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/picture.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/picture.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 
 from openpyxl.descriptors.serialisable import Serialisable
 
 class PictureOptions(Serialisable):
     tagname: str
     applyToFront: Incomplete
     applyToSides: Incomplete
     applyToEnd: Incomplete
     pictureFormat: Incomplete
     pictureStackUnit: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         applyToFront: Incomplete | None = None,
         applyToSides: Incomplete | None = None,
         applyToEnd: Incomplete | None = None,
         pictureFormat: Incomplete | None = None,
         pictureStackUnit: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/pie_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/line_chart.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import ChartLines
+from openpyxl.chart.axis import ChartLines, NumericAxis, _BaseAxis
 from openpyxl.chart.label import DataLabelList
+from openpyxl.chart.updown_bars import UpDownBars
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.serialisable import Serialisable
 
 from ._chart import ChartBase
 
-class _PieChartBase(ChartBase):
+class _LineChartBase(ChartBase):
+    grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
-    __elements__: Incomplete
-    def __init__(self, varyColors: bool = True, ser=(), dLbls: DataLabelList | None = None) -> None: ...
+    dropLines: Typed[ChartLines, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
+        self,
+        grouping: str = "standard",
+        varyColors: Incomplete | None = None,
+        ser=(),
+        dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
+        **kw,
+    ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
-class PieChart(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    firstSliceAng: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, firstSliceAng: int = 0, extLst: Unused = None, **kw) -> None: ...
-
-class PieChart3D(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-
-class DoughnutChart(_PieChartBase):
+class LineChart(_LineChartBase):
     tagname: str
+    grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
-    firstSliceAng: Incomplete
-    holeSize: Incomplete
+    dropLines: Incomplete
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
+    marker: Incomplete
+    smooth: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, firstSliceAng: int = 0, holeSize: int = 10, extLst: Unused = None, **kw) -> None: ...
-
-class CustomSplit(Serialisable):
-    tagname: str
-    secondPiePt: Incomplete
-    __elements__: Incomplete
-    def __init__(self, secondPiePt=()) -> None: ...
+    x_axis: Typed[_BaseAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
+        self,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
+        marker: Incomplete | None = None,
+        smooth: Incomplete | None = None,
+        extLst: Unused = None,
+        **kw,
+    ) -> None: ...
 
-class ProjectedPieChart(_PieChartBase):
+class LineChart3D(_LineChartBase):
     tagname: str
+    grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
-    ofPieType: Incomplete
-    type: Alias
-    gapWidth: Incomplete
-    splitType: Incomplete
-    splitPos: Incomplete
-    custSplit: Typed[CustomSplit, Literal[True]]
-    secondPieSize: Incomplete
-    serLines: Typed[ChartLines, Literal[True]]
-    join_lines: Alias
+    dropLines: Incomplete
+    gapDepth: Incomplete
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
+    marker: Incomplete
+    smooth: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    x_axis: Typed[ExtensionList, Literal[False]]
+    y_axis: Typed[ExtensionList, Literal[False]]
+    z_axis: Typed[ExtensionList, Literal[False]]
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        ofPieType: str = "pie",
-        gapWidth: Incomplete | None = None,
-        splitType: str = "auto",
-        splitPos: Incomplete | None = None,
-        custSplit: CustomSplit | None = None,
-        secondPieSize: int = 75,
-        serLines: ChartLines | None = None,
-        extLst: Unused = None,
+        gapDepth: Incomplete | None = None,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
+        marker: Incomplete | None = None,
+        smooth: Incomplete | None = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/pivot.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/title.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.label import DataLabel as _DataLabel
-from openpyxl.chart.marker import Marker
+from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.chart.text import RichText, Text
+from openpyxl.descriptors import Strict, Typed
+from openpyxl.descriptors.base import Alias
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class PivotSource(Serialisable):
+class Title(Serialisable):
     tagname: str
-    name: Incomplete
-    fmtId: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, name: str | None = None, fmtId: Incomplete | None = None, extLst: Unused = None) -> None: ...
-
-class PivotFormat(Serialisable):
-    tagname: str
-    idx: Incomplete
+    tx: Typed[Text, Literal[True]]
+    text: Alias
+    layout: Typed[Layout, Literal[True]]
+    overlay: Incomplete
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
-    TextBody: Alias
-    marker: Typed[Marker, Literal[True]]
-    dLbl: Typed[_DataLabel, Literal[True]]
-    DataLabel: Alias
+    body: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        idx: int = 0,
+        tx: Text | None = None,
+        layout: Layout | None = None,
+        overlay: Incomplete | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
-        marker: Marker | None = None,
-        dLbl: _DataLabel | None = None,
         extLst: Unused = None,
     ) -> None: ...
+
+def title_maker(text): ...
+
+class TitleDescriptor(Typed[Title, Incomplete]):
+    expected_type: type[Title]
+    allow_none: Literal[True]
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/plotarea.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/shapes.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,47 @@
 from _typeshed import Incomplete, Unused
-from typing_extensions import Literal
+from typing import ClassVar
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.chart.layout import Layout
-from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Alias, NoneSet, Typed
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
+from openpyxl.drawing.geometry import CustomGeometry2D, PresetGeometry2D, Scene3D, Shape3D, Transform2D
+from openpyxl.drawing.line import LineProperties
 
-class DataTable(Serialisable):
-    tagname: str
-    showHorzBorder: Incomplete
-    showVertBorder: Incomplete
-    showOutline: Incomplete
-    showKeys: Incomplete
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    txPr: Typed[RichText, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(
-        self,
-        showHorzBorder: Incomplete | None = None,
-        showVertBorder: Incomplete | None = None,
-        showOutline: Incomplete | None = None,
-        showKeys: Incomplete | None = None,
-        spPr: GraphicalProperties | None = None,
-        txPr: RichText | None = None,
-        extLst: Unused = None,
-    ) -> None: ...
+_GraphicalPropertiesBwMode: TypeAlias = Literal[
+    "clr", "auto", "gray", "ltGray", "invGray", "grayWhite", "blackGray", "blackWhite", "black", "white", "hidden"
+]
 
-class PlotArea(Serialisable):
+class GraphicalProperties(Serialisable):
     tagname: str
-    layout: Typed[Layout, Literal[True]]
-    dTable: Typed[DataTable, Literal[True]]
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    extLst: Typed[ExtensionList, Literal[True]]
-    areaChart: Incomplete
-    area3DChart: Incomplete
-    lineChart: Incomplete
-    line3DChart: Incomplete
-    stockChart: Incomplete
-    radarChart: Incomplete
-    scatterChart: Incomplete
-    pieChart: Incomplete
-    pie3DChart: Incomplete
-    doughnutChart: Incomplete
-    barChart: Incomplete
-    bar3DChart: Incomplete
-    ofPieChart: Incomplete
-    surfaceChart: Incomplete
-    surface3DChart: Incomplete
-    bubbleChart: Incomplete
-    valAx: Incomplete
-    catAx: Incomplete
-    dateAx: Incomplete
-    serAx: Incomplete
-    __elements__: Incomplete
+    bwMode: NoneSet[_GraphicalPropertiesBwMode]
+    xfrm: Typed[Transform2D, Literal[True]]
+    transform: Alias
+    custGeom: Typed[CustomGeometry2D, Literal[True]]
+    prstGeom: Typed[PresetGeometry2D, Literal[True]]
+    noFill: Incomplete
+    solidFill: Incomplete
+    gradFill: Typed[GradientFillProperties, Literal[True]]
+    pattFill: Typed[PatternFillProperties, Literal[True]]
+    ln: Typed[LineProperties, Literal[True]]
+    line: Alias
+    scene3d: Typed[Scene3D, Literal[True]]
+    sp3d: Typed[Shape3D, Literal[True]]
+    shape3D: Alias
+    extLst: Typed[Incomplete, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        layout: Layout | None = None,
-        dTable: DataTable | None = None,
-        spPr: GraphicalProperties | None = None,
-        _charts=(),
-        _axes=(),
+        bwMode: _GraphicalPropertiesBwMode | Literal["none"] | None = None,
+        xfrm: Transform2D | None = None,
+        noFill: Incomplete | None = None,
+        solidFill: Incomplete | None = None,
+        gradFill: GradientFillProperties | None = None,
+        pattFill: PatternFillProperties | None = None,
+        ln: Incomplete | None = None,
+        scene3d: Scene3D | None = None,
+        custGeom: CustomGeometry2D | None = None,
+        prstGeom: PresetGeometry2D | None = None,
+        sp3d: Shape3D | None = None,
         extLst: Unused = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
-    @classmethod
-    def from_tree(cls, node): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/print_settings.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/print_settings.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Alias, Float, Typed, _ConvertibleToFloat
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.header_footer import HeaderFooter
 from openpyxl.worksheet.page import PrintPageSetup
 
@@ -29,14 +29,14 @@
     ) -> None: ...
 
 class PrintSettings(Serialisable):
     tagname: str
     headerFooter: Typed[HeaderFooter, Literal[True]]
     pageMargins: Typed[PageMargins, Literal[True]]
     pageSetup: Typed[PrintPageSetup, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         headerFooter: HeaderFooter | None = None,
         pageMargins: PageMargins | None = None,
         pageSetup: PrintPageSetup | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/radar_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/scatter_chart.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.axis import NumericAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 
-from ._chart import ChartBase
+from ._chart import ChartBase as ChartBase
 
-class RadarChart(ChartBase):
+class ScatterChart(ChartBase):
     tagname: str
-    radarStyle: Incomplete
-    type: Alias
+    scatterStyle: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[TextAxis, Literal[False]]
+    x_axis: Typed[NumericAxis | TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        radarStyle: str = "standard",
+        scatterStyle: Incomplete | None = None,
         varyColors: Incomplete | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/reference.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/reference.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/scatter_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/stock_chart.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import NumericAxis, TextAxis
+from openpyxl.chart.axis import ChartLines, NumericAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
+from openpyxl.chart.updown_bars import UpDownBars
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 
-from ._chart import ChartBase as ChartBase
+from ._chart import ChartBase
 
-class ScatterChart(ChartBase):
+class StockChart(ChartBase):
     tagname: str
-    scatterStyle: Incomplete
-    varyColors: Incomplete
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
+    dropLines: Typed[ChartLines, Literal[True]]
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[NumericAxis | TextAxis, Literal[False]]
+    x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        scatterStyle: Incomplete | None = None,
-        varyColors: Incomplete | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/series.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/series.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.data_source import AxDataSource, NumDataSource, StrRef
 from openpyxl.chart.error_bar import ErrorBars
 from openpyxl.chart.label import DataLabelList
 from openpyxl.chart.marker import Marker
 from openpyxl.chart.picture import PictureOptions
@@ -15,15 +16,15 @@
 attribute_mapping: Incomplete
 
 class SeriesLabel(Serialisable):
     tagname: str
     strRef: Typed[StrRef, Literal[True]]
     v: Incomplete
     value: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, strRef: StrRef | None = None, v: Incomplete | None = None) -> None: ...
 
 class Series(Serialisable):
     tagname: str
     idx: Incomplete
     order: Incomplete
     tx: Typed[SeriesLabel, Literal[True]]
@@ -47,15 +48,15 @@
     yVal: Typed[NumDataSource, Literal[True]]
     bubbleSize: Typed[NumDataSource, Literal[True]]
     zVal: Alias
     bubble3D: Incomplete
     marker: Typed[Marker, Literal[True]]
     smooth: Incomplete
     explosion: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         idx: int = 0,
         order: int = 0,
         tx: SeriesLabel | None = None,
         spPr: GraphicalProperties | None = None,
         pictureOptions: PictureOptions | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/shapes.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/defined_name.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,70 @@
-from _typeshed import Incomplete, Unused
-from typing_extensions import Literal, TypeAlias
+from _typeshed import Incomplete
+from collections import defaultdict
+from collections.abc import Generator
+from re import Pattern
+from typing_extensions import Literal
 
-from openpyxl.descriptors.base import Alias, NoneSet, Typed
+from openpyxl.descriptors import Sequence
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
-from openpyxl.drawing.geometry import CustomGeometry2D, PresetGeometry2D, Scene3D, Shape3D, Transform2D
-from openpyxl.drawing.line import LineProperties
 
-_GraphicalPropertiesBwMode: TypeAlias = Literal[
-    "clr", "auto", "gray", "ltGray", "invGray", "grayWhite", "blackGray", "blackWhite", "black", "white", "hidden"
-]
+RESERVED: frozenset[str]
+RESERVED_REGEX: Pattern[str]
 
-class GraphicalProperties(Serialisable):
+class DefinedName(Serialisable):
     tagname: str
-    bwMode: NoneSet[_GraphicalPropertiesBwMode]
-    xfrm: Typed[Transform2D, Literal[True]]
-    transform: Alias
-    custGeom: Typed[CustomGeometry2D, Literal[True]]
-    prstGeom: Typed[PresetGeometry2D, Literal[True]]
-    noFill: Incomplete
-    solidFill: Incomplete
-    gradFill: Typed[GradientFillProperties, Literal[True]]
-    pattFill: Typed[PatternFillProperties, Literal[True]]
-    ln: Typed[LineProperties, Literal[True]]
-    line: Alias
-    scene3d: Typed[Scene3D, Literal[True]]
-    sp3d: Typed[Shape3D, Literal[True]]
-    shape3D: Alias
-    extLst: Typed[Incomplete, Literal[True]]
-    __elements__: Incomplete
+    name: String[Literal[False]]
+    comment: String[Literal[True]]
+    customMenu: String[Literal[True]]
+    description: String[Literal[True]]
+    help: String[Literal[True]]
+    statusBar: String[Literal[True]]
+    localSheetId: Integer[Literal[True]]
+    hidden: Bool[Literal[True]]
+    function: Bool[Literal[True]]
+    vbProcedure: Bool[Literal[True]]
+    xlm: Bool[Literal[True]]
+    functionGroupId: Integer[Literal[True]]
+    shortcutKey: String[Literal[True]]
+    publishToServer: Bool[Literal[True]]
+    workbookParameter: Bool[Literal[True]]
+    attr_text: Incomplete
+    value: Alias
     def __init__(
         self,
-        bwMode: _GraphicalPropertiesBwMode | Literal["none"] | None = None,
-        xfrm: Transform2D | None = None,
-        noFill: Incomplete | None = None,
-        solidFill: Incomplete | None = None,
-        gradFill: GradientFillProperties | None = None,
-        pattFill: PatternFillProperties | None = None,
-        ln: Incomplete | None = None,
-        scene3d: Scene3D | None = None,
-        custGeom: CustomGeometry2D | None = None,
-        prstGeom: PresetGeometry2D | None = None,
-        sp3d: Shape3D | None = None,
-        extLst: Unused = None,
+        name: str,
+        comment: str | None = None,
+        customMenu: str | None = None,
+        description: str | None = None,
+        help: str | None = None,
+        statusBar: str | None = None,
+        localSheetId: _ConvertibleToInt | None = None,
+        hidden: _ConvertibleToBool | None = None,
+        function: _ConvertibleToBool | None = None,
+        vbProcedure: _ConvertibleToBool | None = None,
+        xlm: _ConvertibleToBool | None = None,
+        functionGroupId: _ConvertibleToInt | None = None,
+        shortcutKey: str | None = None,
+        publishToServer: _ConvertibleToBool | None = None,
+        workbookParameter: _ConvertibleToBool | None = None,
+        attr_text: Incomplete | None = None,
     ) -> None: ...
+    @property
+    def type(self): ...
+    @property
+    def destinations(self) -> Generator[Incomplete, None, None]: ...
+    @property
+    def is_reserved(self): ...
+    @property
+    def is_external(self): ...
+    def __iter__(self): ...
+
+class DefinedNameDict(dict[str, DefinedName]):
+    def add(self, value: DefinedName) -> None: ...
+
+class DefinedNameList(Serialisable):
+    tagname: str
+    definedName: Sequence
+    def __init__(self, definedName=()) -> None: ...
+    def by_sheet(self) -> defaultdict[int, DefinedNameDict]: ...
+    def __len__(self) -> int: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/stock_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/layout.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import ChartLines, NumericAxis, TextAxis
-from openpyxl.chart.label import DataLabelList
-from openpyxl.chart.updown_bars import UpDownBars
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.serialisable import Serialisable
 
-from ._chart import ChartBase
-
-class StockChart(ChartBase):
+class ManualLayout(Serialisable):
     tagname: str
-    ser: Incomplete
-    dLbls: Typed[DataLabelList, Literal[True]]
-    dataLabels: Alias
-    dropLines: Typed[ChartLines, Literal[True]]
-    hiLowLines: Typed[ChartLines, Literal[True]]
-    upDownBars: Typed[UpDownBars, Literal[True]]
+    layoutTarget: Incomplete
+    xMode: Incomplete
+    yMode: Incomplete
+    wMode: Incomplete
+    hMode: Incomplete
+    x: Incomplete
+    y: Incomplete
+    w: Incomplete
+    width: Alias
+    h: Incomplete
+    height: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[TextAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        ser=(),
-        dLbls: DataLabelList | None = None,
-        dropLines: ChartLines | None = None,
-        hiLowLines: ChartLines | None = None,
-        upDownBars: UpDownBars | None = None,
+        layoutTarget: Incomplete | None = None,
+        xMode: Incomplete | None = None,
+        yMode: Incomplete | None = None,
+        wMode: str = "factor",
+        hMode: str = "factor",
+        x: Incomplete | None = None,
+        y: Incomplete | None = None,
+        w: Incomplete | None = None,
+        h: Incomplete | None = None,
         extLst: Unused = None,
-        **kw,
     ) -> None: ...
+
+class Layout(Serialisable):
+    tagname: str
+    manualLayout: Typed[ManualLayout, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, manualLayout: ManualLayout | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/surface_chart.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/area_chart.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import NumericAxis, SeriesAxis, TextAxis
-from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
+from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.serialisable import Serialisable
 
-from ._3d import _3DBase
 from ._chart import ChartBase
 
-class BandFormat(Serialisable):
-    tagname: str
-    idx: Incomplete
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    __elements__: Incomplete
-    def __init__(self, idx: int = 0, spPr: GraphicalProperties | None = None) -> None: ...
-
-class BandFormatList(Serialisable):
-    tagname: str
-    bandFmt: Incomplete
-    __elements__: Incomplete
-    def __init__(self, bandFmt=()) -> None: ...
-
-class _SurfaceChartBase(ChartBase):
-    wireframe: Incomplete
+class _AreaChartBase(ChartBase):
+    grouping: Incomplete
+    varyColors: Incomplete
     ser: Incomplete
-    bandFmts: Typed[BandFormatList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, wireframe: Incomplete | None = None, ser=(), bandFmts: BandFormatList | None = None, **kw) -> None: ...
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
+    dropLines: Typed[ChartLines, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
+        self,
+        grouping: str = "standard",
+        varyColors: Incomplete | None = None,
+        ser=(),
+        dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
+    ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
-class SurfaceChart3D(_SurfaceChartBase, _3DBase):
+class AreaChart(_AreaChartBase):
     tagname: str
-    wireframe: Incomplete
+    grouping: Incomplete
+    varyColors: Incomplete
     ser: Incomplete
-    bandFmts: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
+    dLbls: Incomplete
+    dropLines: Incomplete
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
-    z_axis: Typed[SeriesAxis, Literal[False]]
-    __elements__: Incomplete
-    def __init__(self, **kw) -> None: ...
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, axId: Unused = None, extLst: Unused = None, **kw) -> None: ...
 
-class SurfaceChart(SurfaceChart3D):
+class AreaChart3D(AreaChart):
     tagname: str
-    wireframe: Incomplete
+    grouping: Incomplete
+    varyColors: Incomplete
     ser: Incomplete
-    bandFmts: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    def __init__(self, **kw) -> None: ...
+    dLbls: Incomplete
+    dropLines: Incomplete
+    gapDepth: Incomplete
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    z_axis: Typed[SeriesAxis, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, gapDepth: Incomplete | None = None, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/text.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/text.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.data_source import StrRef
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.text import ListStyle, RichTextProperties
 
 class RichText(Serialisable):
     tagname: str
     bodyPr: Typed[RichTextProperties, Literal[False]]
     properties: Alias
     lstStyle: Typed[ListStyle, Literal[True]]
     p: Incomplete
     paragraphs: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, bodyPr: RichTextProperties | None = None, lstStyle: ListStyle | None = None, p: Incomplete | None = None
     ) -> None: ...
 
 class Text(Serialisable):
     tagname: str
     strRef: Typed[StrRef, Literal[True]]
     rich: Typed[RichText, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, strRef: StrRef | None = None, rich: RichText | None = None) -> None: ...
     def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/trendline.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/trendline.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.data_source import NumFmt
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText, Text
 from openpyxl.descriptors.base import Alias, String, Typed
@@ -15,15 +16,15 @@
     tx: Typed[Text, Literal[True]]
     numFmt: Typed[NumFmt, Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         layout: Layout | None = None,
         tx: Text | None = None,
         numFmt: NumFmt | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
@@ -41,15 +42,15 @@
     forward: Incomplete
     backward: Incomplete
     intercept: Incomplete
     dispRSqr: Incomplete
     dispEq: Incomplete
     trendlineLbl: Typed[ExtensionList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         name: str | None = None,
         spPr: ExtensionList | None = None,
         trendlineType: str = "linear",
         order: Incomplete | None = None,
         period: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chart/updown_bars.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/updown_bars.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.axis import ChartLines
 from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class UpDownBars(Serialisable):
     tagname: str
     gapWidth: Incomplete
     upBars: Typed[ChartLines, Literal[True]]
     downBars: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, gapWidth: int = 150, upBars: ChartLines | None = None, downBars: ChartLines | None = None, extLst: Unused = None
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/chartsheet.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/chartsheet.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.chartsheet.custom import CustomChartsheetViews
 from openpyxl.chartsheet.properties import ChartsheetProperties
 from openpyxl.chartsheet.protection import ChartsheetProtection
 from openpyxl.chartsheet.publish import WebPublishItems
 from openpyxl.chartsheet.relation import DrawingHF, SheetBackgroundPicture
@@ -30,16 +31,16 @@
     drawingHF: Typed[DrawingHF, Literal[True]]
     picture: Typed[SheetBackgroundPicture, Literal[True]]
     webPublishItems: Typed[WebPublishItems, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     sheet_state: Set[_ChartsheetSheetState]
     headerFooter: Typed[_HeaderFooter, Literal[False]]
     HeaderFooter: Alias
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         sheetPr: ChartsheetProperties | None = None,
         sheetViews: ChartsheetViewList | None = None,
         sheetProtection: ChartsheetProtection | None = None,
         customSheetViews: CustomChartsheetViews | None = None,
         pageMargins: PageMargins | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/custom.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/custom.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, Set, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.header_footer import HeaderFooter
 from openpyxl.worksheet.page import PageMargins, PrintPageSetup
 
@@ -14,15 +14,15 @@
     guid: Incomplete
     scale: Integer[Literal[False]]
     state: Set[_CustomChartsheetViewState]
     zoomToFit: Bool[Literal[True]]
     pageMargins: Typed[PageMargins, Literal[True]]
     pageSetup: Typed[PrintPageSetup, Literal[True]]
     headerFooter: Typed[HeaderFooter, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         guid: Incomplete | None = None,
         *,
         scale: _ConvertibleToInt,
         state: _CustomChartsheetViewState = "visible",
@@ -42,9 +42,9 @@
         pageSetup: PrintPageSetup | None = None,
         headerFooter: HeaderFooter | None = None,
     ) -> None: ...
 
 class CustomChartsheetViews(Serialisable):
     tagname: str
     customSheetView: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, customSheetView: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/properties.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/properties.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable as Serialisable
 from openpyxl.styles.colors import Color
 
 class ChartsheetProperties(Serialisable):
     tagname: str
     published: Bool[Literal[True]]
     codeName: String[Literal[True]]
     tabColor: Typed[Color, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, published: _ConvertibleToBool | None = None, codeName: str | None = None, tabColor: Color | None = None
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/protection.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/protection.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.protection import _Protected
 
 class ChartsheetProtection(Serialisable, _Protected):
     tagname: str
     algorithmName: String[Literal[True]]
     hashValue: Incomplete
     saltValue: Incomplete
     spinCount: Integer[Literal[True]]
     content: Bool[Literal[True]]
     objects: Bool[Literal[True]]
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     password: Incomplete
     def __init__(
         self,
         content: _ConvertibleToBool | None = None,
         objects: _ConvertibleToBool | None = None,
         hashValue: Incomplete | None = None,
         spinCount: _ConvertibleToInt | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/publish.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/publish.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, Set, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 _WebPublishItemSourceType: TypeAlias = Literal[
     "sheet", "printArea", "autoFilter", "range", "chart", "pivotTable", "query", "label"
@@ -45,9 +45,9 @@
         autoRepublish: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class WebPublishItems(Serialisable):
     tagname: str
     count: Integer[Literal[True]]
     webPublishItem: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt | None = None, webPublishItem: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/relation.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/relation.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/chartsheet/views.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/views.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class ChartsheetView(Serialisable):
     tagname: str
     tabSelected: Bool[Literal[True]]
     zoomScale: Integer[Literal[True]]
     workbookViewId: Integer[Literal[False]]
     zoomToFit: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         tabSelected: _ConvertibleToBool | None = None,
         zoomScale: _ConvertibleToInt | None = None,
         workbookViewId: _ConvertibleToInt = 0,
         zoomToFit: _ConvertibleToBool | None = True,
         extLst: Unused = None,
     ) -> None: ...
 
 class ChartsheetViewList(Serialisable):
     tagname: str
     sheetView: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, sheetView: Incomplete | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/comments/comment_sheet.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/comments/comment_sheet.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from _typeshed import Incomplete, Unused
 from collections.abc import Generator
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.cell.text import Text
 from openpyxl.comments.author import AuthorList
 from openpyxl.descriptors.base import Bool, Integer, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
@@ -25,15 +25,15 @@
     textHAlign: Set[_PropertiesTextHAlign]
     textVAlign: Set[_PropertiesTextVAlign]
     lockText: Bool[Literal[True]]
     justLastX: Bool[Literal[True]]
     autoScale: Bool[Literal[True]]
     rowHidden: Bool[Literal[True]]
     colHidden: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     anchor: ObjectAnchor | None
     @overload
     def __init__(
         self,
         locked: _ConvertibleToBool | None = None,
         defaultSize: _ConvertibleToBool | None = None,
         _print: _ConvertibleToBool | None = None,
@@ -78,16 +78,16 @@
     ref: String[Literal[False]]
     authorId: Integer[Literal[False]]
     guid: Incomplete
     shapeId: Integer[Literal[True]]
     text: Typed[Text, Literal[False]]
     commentPr: Typed[Properties, Literal[True]]
     author: String[Literal[True]]
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     height: Incomplete
     width: Incomplete
     def __init__(
         self,
         ref: str = "",
         authorId: _ConvertibleToInt = 0,
         guid: Incomplete | None = None,
@@ -105,15 +105,15 @@
 
 class CommentSheet(Serialisable):
     tagname: str
     authors: Typed[AuthorList, Literal[False]]
     commentList: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     mime_type: str
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, authors: AuthorList, commentList: Incomplete | None = None, extLst: Unused = None) -> None: ...
     def to_tree(self): ...
     @property
     def comments(self) -> Generator[Incomplete, None, None]: ...
     @classmethod
     def from_comments(cls, comments): ...
     def write_shapes(self, vml: Incomplete | None = None): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/base.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/base.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/excel.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/nested.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/nested.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/descriptors/sequence.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/sequence.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/colors.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/colors.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors import Strict, Typed
 from openpyxl.descriptors.base import Alias, Integer, MinMax, Set, _ConvertibleToFloat, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
@@ -96,15 +96,15 @@
     blue: Incomplete
     blueOff: Incomplete
     blueMod: Incomplete
     gamma: Typed[Transform, Literal[True]]
     invGamma: Typed[Transform, Literal[True]]
     val: Set[_SystemColorVal]
     lastClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         val: _SystemColorVal = "windowText",
         lastClr: Incomplete | None = None,
         tint: Incomplete | None = None,
         shade: Incomplete | None = None,
         comp: Transform | None = None,
@@ -179,15 +179,15 @@
     greenMod: Incomplete
     blue: Incomplete
     blueOff: Incomplete
     blueMod: Incomplete
     gamma: Incomplete
     invGamma: Incomplete
     val: Set[_SchemeColorVal]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         tint: Incomplete | None = None,
         shade: Incomplete | None = None,
         comp: Incomplete | None = None,
         inv: Incomplete | None = None,
@@ -259,15 +259,15 @@
     RGBPercent: Alias
     srgbClr: Incomplete
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SystemColor, Literal[True]]
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         scrgbClr: _RGBPercent | None = None,
         srgbClr: Incomplete | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SystemColor | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/connector.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/connector.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
 from openpyxl.descriptors import Typed
 from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
@@ -32,15 +31,15 @@
         endCxn: Connection | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class ConnectorNonVisual(Serialisable):
     cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
     cNvCxnSpPr: Typed[NonVisualConnectorProperties, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cNvPr: NonVisualDrawingProps, cNvCxnSpPr: NonVisualConnectorProperties) -> None: ...
 
 class ConnectorShape(Serialisable):
     tagname: str
     nvCxnSpPr: Typed[ConnectorNonVisual, Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[False]]
     style: Typed[ShapeStyle, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/drawing.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/effect.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/effect.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Bool,
     Float,
     Integer,
     Set,
@@ -119,28 +119,28 @@
     rad: Float[Literal[False]]
     scrgbClr: Incomplete
     srgbClr: Incomplete
     hslClr: Incomplete
     sysClr: Incomplete
     schemeClr: Incomplete
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rad: _ConvertibleToFloat, **kw) -> None: ...
 
 class InnerShadowEffect(ColorChoice):
     blurRad: Float[Literal[False]]
     dist: Float[Literal[False]]
     dir: Integer[Literal[False]]
     scrgbClr: Incomplete
     srgbClr: Incomplete
     hslClr: Incomplete
     sysClr: Incomplete
     schemeClr: Incomplete
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, blurRad: _ConvertibleToFloat, dist: _ConvertibleToFloat, dir: _ConvertibleToInt, **kw) -> None: ...
 
 class OuterShadow(ColorChoice):
     tagname: str
     blurRad: Float[Literal[True]]
     dist: Float[Literal[True]]
     dir: Integer[Literal[True]]
@@ -152,15 +152,15 @@
     rotWithShape: Bool[Literal[True]]
     scrgbClr: Incomplete
     srgbClr: Incomplete
     hslClr: Incomplete
     sysClr: Incomplete
     schemeClr: Incomplete
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         blurRad: _ConvertibleToFloat | None = None,
         dist: _ConvertibleToFloat | None = None,
         dir: _ConvertibleToInt | None = None,
         sx: _ConvertibleToInt | None = None,
@@ -193,15 +193,15 @@
     dir: Integer[Literal[False]]
     scrgbClr: Incomplete
     srgbClr: Incomplete
     hslClr: Incomplete
     sysClr: Incomplete
     schemeClr: Incomplete
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, prst: _PresetShadowEffectPrst, dist: _ConvertibleToFloat, dir: _ConvertibleToInt, **kw) -> None: ...
 
 class ReflectionEffect(Serialisable):
     blurRad: Float[Literal[False]]
     stA: Integer[Literal[False]]
     stPos: Integer[Literal[False]]
     endA: Integer[Literal[False]]
@@ -242,15 +242,15 @@
     fillOverlay: Typed[FillOverlayEffect, Literal[True]]
     glow: Typed[GlowEffect, Literal[True]]
     innerShdw: Typed[InnerShadowEffect, Literal[True]]
     outerShdw: Typed[OuterShadow, Literal[True]]
     prstShdw: Typed[PresetShadowEffect, Literal[True]]
     reflection: Typed[ReflectionEffect, Literal[True]]
     softEdge: Typed[SoftEdgesEffect, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         blur: BlurEffect | None = None,
         fillOverlay: FillOverlayEffect | None = None,
         glow: GlowEffect | None = None,
         innerShdw: InnerShadowEffect | None = None,
         outerShdw: OuterShadow | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/fill.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/fill.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     Integer,
     MinMax,
@@ -102,15 +103,15 @@
     namespace: Incomplete
     prst: NoneSet[_PatternFillPropertiesPrst]
     preset: Alias
     fgClr: Typed[ColorChoice, Literal[True]]
     foreground: Alias
     bgClr: Typed[ColorChoice, Literal[True]]
     background: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         prst: _PatternFillPropertiesPrst | Literal["none"] | None = None,
         fgClr: ColorChoice | None = None,
         bgClr: ColorChoice | None = None,
     ) -> None: ...
 
@@ -143,15 +144,15 @@
     RGBPercent: Alias
     srgbClr: Incomplete
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SchemeColor, Literal[True]]
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         pos: _ConvertibleToFloat | None = None,
         scrgbClr: _RGBPercent | None = None,
         srgbClr: Incomplete | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
@@ -180,15 +181,15 @@
     rotWithShape: Bool[Literal[True]]
     gsLst: Incomplete
     stop_list: Alias
     lin: Typed[LinearShadeProperties, Literal[True]]
     linear: Alias
     path: Typed[PathShadeProperties, Literal[True]]
     tileRect: Typed[RelativeRect, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         flip: _PropertiesFlip | Literal["none"] | None = None,
         rotWithShape: _ConvertibleToBool | None = None,
         gsLst=(),
         lin: LinearShadeProperties | None = None,
         path: PathShadeProperties | None = None,
@@ -201,15 +202,15 @@
     RGBPercent: Alias
     srgbClr: Incomplete
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SchemeColor, Literal[True]]
     prstClr: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         scrgbClr: _RGBPercent | None = None,
         srgbClr: Incomplete | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SchemeColor | None = None,
@@ -246,15 +247,15 @@
     clrRepl: Typed[ColorReplaceEffect, Literal[True]]
     duotone: Typed[DuotoneEffect, Literal[True]]
     fillOverlay: Typed[FillOverlayEffect, Literal[True]]
     grayscl: Typed[GrayscaleEffect, Literal[True]]
     hsl: Typed[HSLEffect, Literal[True]]
     lum: Typed[LuminanceEffect, Literal[True]]
     tint: Typed[TintEffect, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         cstate: _BlipCstate | Literal["none"] | None = None,
         embed: Incomplete | None = None,
         link: Incomplete | None = None,
         noGrp: _ConvertibleToBool | None = None,
         noSelect: _ConvertibleToBool | None = None,
@@ -308,15 +309,15 @@
     tagname: str
     dpi: Integer[Literal[True]]
     rotWithShape: Bool[Literal[True]]
     blip: Typed[Blip, Literal[True]]
     srcRect: Typed[RelativeRect, Literal[True]]
     tile: Typed[TileInfoProperties, Literal[True]]
     stretch: Typed[StretchInfoProperties, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         dpi: _ConvertibleToInt | None = None,
         rotWithShape: _ConvertibleToBool | None = None,
         blip: Blip | None = None,
         tile: TileInfoProperties | None = None,
         stretch: StretchInfoProperties = ...,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/geometry.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/geometry.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     Float,
     Integer,
@@ -359,15 +359,15 @@
     rot: Integer[Literal[True]]
     flipH: Bool[Literal[True]]
     flipV: Bool[Literal[True]]
     off: Typed[Point2D, Literal[True]]
     ext: Typed[PositiveSize2D, Literal[True]]
     chOff: Typed[Point2D, Literal[True]]
     chExt: Typed[PositiveSize2D, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         rot: _ConvertibleToInt | None = None,
         flipH: _ConvertibleToBool | None = None,
         flipV: _ConvertibleToBool | None = None,
         off: Point2D | None = None,
         ext: PositiveSize2D | None = None,
@@ -381,15 +381,15 @@
     rot: Integer[Literal[True]]
     flipH: Bool[Literal[True]]
     flipV: Bool[Literal[True]]
     off = Typed(expected_type=Point2D, allow_none=True)
     ext = Typed(expected_type=PositiveSize2D, allow_none=True)
     chOff = Typed(expected_type=Point2D, allow_none=True)
     chExt = Typed(expected_type=PositiveSize2D, allow_none=True)
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         rot: _ConvertibleToInt | None = 0,
         flipH: _ConvertibleToBool | None = None,
         flipV: _ConvertibleToBool | None = None,
         off: Point2D | None = None,
         ext: PositiveSize2D | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/graphic.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/graphic.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Alias, Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.picture import PictureFrame
 from openpyxl.drawing.properties import GroupShapeProperties, NonVisualGroupShape
@@ -34,15 +35,15 @@
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(self, graphicFrameLocks: GraphicFrameLocking | None = None, extLst: ExtensionList | None = None) -> None: ...
 
 class NonVisualGraphicFrame(Serialisable):
     tagname: str
     cNvPr: Typed[ExtensionList, Literal[False]]
     cNvGraphicFramePr: Typed[ExtensionList, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cNvPr: Incomplete | None = None, cNvGraphicFramePr: Incomplete | None = None) -> None: ...
 
 class GraphicData(Serialisable):
     tagname: str
     namespace: Incomplete
     uri: String[Literal[False]]
     chart: Typed[ChartRelation, Literal[True]]
@@ -57,15 +58,15 @@
 class GraphicFrame(Serialisable):
     tagname: str
     nvGraphicFramePr: Typed[NonVisualGraphicFrame, Literal[False]]
     xfrm: Typed[XDRTransform2D, Literal[False]]
     graphic: Typed[GraphicObject, Literal[False]]
     macro: String[Literal[True]]
     fPublished: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         nvGraphicFramePr: NonVisualGraphicFrame | None = None,
         xfrm: XDRTransform2D | None = None,
         graphic: GraphicObject | None = None,
         macro: str | None = None,
         fPublished: _ConvertibleToBool | None = None,
@@ -73,11 +74,12 @@
 
 class GroupShape(Serialisable):
     nvGrpSpPr: Typed[NonVisualGroupShape, Literal[False]]
     nonVisualProperties: Alias
     grpSpPr: Typed[GroupShapeProperties, Literal[False]]
     visualProperties: Alias
     pic: Typed[PictureFrame, Literal[True]]
-    __elements__: Incomplete
+    # Source incorrectly uses a list here instead of a tuple
+    __elements__: ClassVar[list[str]]  # type: ignore[assignment]
     def __init__(
         self, nvGrpSpPr: NonVisualGroupShape, grpSpPr: GroupShapeProperties, pic: PictureFrame | None = None
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/line.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/line.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Alias, Integer, MinMax, NoneSet, Typed, _ConvertibleToFloat, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
 
@@ -55,15 +56,15 @@
     custDash: Typed[DashStop, Literal[True]]
     round: Incomplete
     bevel: Incomplete
     miter: Incomplete
     headEnd: Typed[LineEndProperties, Literal[True]]
     tailEnd: Typed[LineEndProperties, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         w: _ConvertibleToFloat | None = None,
         cap: _LinePropertiesCap | Literal["none"] | None = None,
         cmpd: _LinePropertiesCmpd | Literal["none"] | None = None,
         algn: _LinePropertiesAlgn | Literal["none"] | None = None,
         noFill: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/picture.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/picture.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.descriptors.base import Alias, Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.fill import BlipFillProperties
@@ -20,15 +21,15 @@
     noMove: Bool[Literal[True]]
     noResize: Bool[Literal[True]]
     noEditPoints: Bool[Literal[True]]
     noAdjustHandles: Bool[Literal[True]]
     noChangeArrowheads: Bool[Literal[True]]
     noChangeShapeType: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         noCrop: _ConvertibleToBool | None = None,
         noGrp: _ConvertibleToBool | None = None,
         noSelect: _ConvertibleToBool | None = None,
         noRot: _ConvertibleToBool | None = None,
         noChangeAspect: _ConvertibleToBool | None = None,
@@ -42,38 +43,38 @@
     ) -> None: ...
 
 class NonVisualPictureProperties(Serialisable):
     tagname: str
     preferRelativeResize: Bool[Literal[True]]
     picLocks: Typed[PictureLocking, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, preferRelativeResize: _ConvertibleToBool | None = None, picLocks: Incomplete | None = None, extLst: Unused = None
     ) -> None: ...
 
 class PictureNonVisual(Serialisable):
     tagname: str
     cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
     cNvPicPr: Typed[NonVisualPictureProperties, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, cNvPr: NonVisualDrawingProps | None = None, cNvPicPr: NonVisualPictureProperties | None = None
     ) -> None: ...
 
 class PictureFrame(Serialisable):
     tagname: str
     macro: String[Literal[True]]
     fPublished: Bool[Literal[True]]
     nvPicPr: Typed[PictureNonVisual, Literal[False]]
     blipFill: Typed[BlipFillProperties, Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[False]]
     graphicalProperties: Alias
     style: Typed[ShapeStyle, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         macro: str | None = None,
         fPublished: _ConvertibleToBool | None = None,
         nvPicPr: PictureNonVisual | None = None,
         blipFill: BlipFillProperties | None = None,
         spPr: GraphicalProperties | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/properties.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/properties.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, NoneSet, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.geometry import GroupTransform2D, Scene3D
 from openpyxl.drawing.text import Hyperlink
@@ -37,15 +37,15 @@
     noMove: Bool[Literal[True]]
     noResize: Bool[Literal[True]]
     noChangeArrowheads: Bool[Literal[True]]
     noEditPoints: Bool[Literal[True]]
     noAdjustHandles: Bool[Literal[True]]
     noChangeShapeType: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         noGrp: _ConvertibleToBool | None = None,
         noUngrp: _ConvertibleToBool | None = None,
         noSelect: _ConvertibleToBool | None = None,
         noRot: _ConvertibleToBool | None = None,
         noChangeAspect: _ConvertibleToBool | None = None,
@@ -58,23 +58,23 @@
         extLst: Unused = None,
     ) -> None: ...
 
 class NonVisualGroupDrawingShapeProps(Serialisable):
     tagname: str
     grpSpLocks: Typed[GroupLocking, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, grpSpLocks: Incomplete | None = None, extLst: Unused = None) -> None: ...
 
 class NonVisualDrawingShapeProps(Serialisable):
     tagname: str
     spLocks: Typed[GroupLocking, Literal[True]]
     txBax: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     txBox: Incomplete
     def __init__(
         self, spLocks: Incomplete | None = None, txBox: _ConvertibleToBool | None = None, extLst: Unused = None
     ) -> None: ...
 
 class NonVisualDrawingProps(Serialisable):
     tagname: str
@@ -82,15 +82,16 @@
     name: String[Literal[False]]
     descr: String[Literal[True]]
     hidden: Bool[Literal[True]]
     title: String[Literal[True]]
     hlinkClick: Typed[Hyperlink, Literal[True]]
     hlinkHover: Typed[Hyperlink, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    # Source incorrectly uses a list here instead of a tuple
+    __elements__: ClassVar[list[str]]  # type: ignore[assignment]
     @overload
     def __init__(
         self,
         id: Incomplete | None = None,
         *,
         name: str,
         descr: str | None = None,
@@ -113,9 +114,9 @@
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class NonVisualGroupShape(Serialisable):
     tagname: str
     cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
     cNvGrpSpPr: Typed[NonVisualGroupDrawingShapeProps, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cNvPr: NonVisualDrawingProps, cNvGrpSpPr: NonVisualGroupDrawingShapeProps) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/spreadsheet_drawing.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/spreadsheet_drawing.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.connector import Shape
 from openpyxl.drawing.graphic import GraphicFrame, GroupShape
 from openpyxl.drawing.picture import PictureFrame
@@ -32,15 +33,15 @@
     groupShape: Alias
     graphicFrame: Typed[GraphicFrame, Literal[True]]
     cxnSp: Typed[Shape, Literal[True]]
     connectionShape: Alias
     pic: Typed[PictureFrame, Literal[True]]
     contentPart: Incomplete
     clientData: Typed[AnchorClientData, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         clientData: AnchorClientData | None = None,
         sp: Shape | None = None,
         grpSp: GroupShape | None = None,
         graphicFrame: GraphicFrame | None = None,
         cxnSp: Shape | None = None,
@@ -55,44 +56,44 @@
     sp: Incomplete
     grpSp: Incomplete
     graphicFrame: Incomplete
     cxnSp: Incomplete
     pic: Incomplete
     contentPart: Incomplete
     clientData: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, pos: XDRPoint2D | None = None, ext: XDRPositiveSize2D | None = None, **kw) -> None: ...
 
 class OneCellAnchor(_AnchorBase):
     tagname: str
     _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
     ext: Typed[XDRPositiveSize2D, Literal[False]]
     sp: Incomplete
     grpSp: Incomplete
     graphicFrame: Incomplete
     cxnSp: Incomplete
     pic: Incomplete
     contentPart: Incomplete
     clientData: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, _from: AnchorMarker | None = None, ext: XDRPositiveSize2D | None = None, **kw) -> None: ...
 
 class TwoCellAnchor(_AnchorBase):
     tagname: str
     editAs: NoneSet[_TwoCellAnchorEditAs]
     _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
     to: Typed[AnchorMarker, Literal[False]]
     sp: Incomplete
     grpSp: Incomplete
     graphicFrame: Incomplete
     cxnSp: Incomplete
     pic: Incomplete
     contentPart: Incomplete
     clientData: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         editAs: _TwoCellAnchorEditAs | Literal["none"] | None = None,
         _from: AnchorMarker | None = None,
         to: AnchorMarker | None = None,
         **kw,
     ) -> None: ...
@@ -100,15 +101,15 @@
 class SpreadsheetDrawing(Serialisable):
     tagname: str
     mime_type: str
     PartName: str
     twoCellAnchor: Incomplete
     oneCellAnchor: Incomplete
     absoluteAnchor: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     charts: Incomplete
     images: Incomplete
     def __init__(self, twoCellAnchor=(), oneCellAnchor=(), absoluteAnchor=()) -> None: ...
     def __hash__(self) -> int: ...
     def __bool__(self) -> bool: ...
     @property
     def path(self): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/drawing/text.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/text.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     Integer,
     MinMax,
@@ -152,15 +153,15 @@
     tooltip: String[Literal[True]]
     history: Bool[Literal[True]]
     highlightClick: Bool[Literal[True]]
     endSnd: Bool[Literal[True]]
     snd: Typed[EmbeddedWAVAudioFile, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     id: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         invalidUrl: str | None = None,
         action: str | None = None,
         tgtFrame: str | None = None,
         tooltip: str | None = None,
         history: _ConvertibleToBool | None = None,
@@ -226,15 +227,15 @@
     grpFill: Incomplete
     effectLst: Typed[EffectList, Literal[True]]
     effectDag: Typed[EffectContainer, Literal[True]]
     uLnTx: Incomplete
     uLn: Typed[LineProperties, Literal[True]]
     uFillTx: Incomplete
     uFill: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         kumimoji: _ConvertibleToBool | None = None,
         lang: str | None = None,
         altLang: str | None = None,
         sz: _ConvertibleToFloat | None = None,
         b: _ConvertibleToBool | None = None,
@@ -284,15 +285,15 @@
 class TabStopList(Serialisable):
     tab: Typed[TabStop, Literal[True]]
     def __init__(self, tab: Incomplete | None = None) -> None: ...
 
 class Spacing(Serialisable):
     spcPct: Incomplete
     spcPts: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, spcPct: Incomplete | None = None, spcPts: Incomplete | None = None) -> None: ...
 
 class AutonumberBullet(Serialisable):
     type: Set[_AutonumberBulletType]
     startAt: Integer[Literal[False]]
     def __init__(self, type: _AutonumberBulletType, startAt: _ConvertibleToInt) -> None: ...
 
@@ -323,15 +324,15 @@
     buSzPts: Incomplete
     buFontTx: Incomplete
     buFont: Typed[Font, Literal[True]]
     buNone: Incomplete
     buAutoNum: Incomplete
     buChar: Incomplete
     buBlip: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         marL: _ConvertibleToInt | None = None,
         marR: _ConvertibleToInt | None = None,
         lvl: _ConvertibleToInt | None = None,
         indent: _ConvertibleToInt | None = None,
         algn: _ParagraphPropertiesAlgn | Literal["none"] | None = None,
@@ -370,15 +371,15 @@
     lvl4pPr: Typed[ParagraphProperties, Literal[True]]
     lvl5pPr: Typed[ParagraphProperties, Literal[True]]
     lvl6pPr: Typed[ParagraphProperties, Literal[True]]
     lvl7pPr: Typed[ParagraphProperties, Literal[True]]
     lvl8pPr: Typed[ParagraphProperties, Literal[True]]
     lvl9pPr: Typed[ParagraphProperties, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         defPPr: ParagraphProperties | None = None,
         lvl1pPr: ParagraphProperties | None = None,
         lvl2pPr: ParagraphProperties | None = None,
         lvl3pPr: ParagraphProperties | None = None,
         lvl4pPr: ParagraphProperties | None = None,
@@ -393,31 +394,31 @@
 class RegularTextRun(Serialisable):
     tagname: str
     namespace: Incomplete
     rPr: Typed[CharacterProperties, Literal[True]]
     properties: Alias
     t: Incomplete
     value: Alias
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rPr: CharacterProperties | None = None, t: str = "") -> None: ...
 
 class LineBreak(Serialisable):
     tagname: str
     namespace: Incomplete
     rPr: Typed[CharacterProperties, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rPr: CharacterProperties | None = None) -> None: ...
 
 class TextField(Serialisable):
     id: String[Literal[False]]
     type: String[Literal[True]]
     rPr: Typed[CharacterProperties, Literal[True]]
     pPr: Typed[CharacterProperties, Literal[True]]
     t: String[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         id: str,
         type: str | None = None,
         rPr: CharacterProperties | None = None,
         pPr: CharacterProperties | None = None,
         t: str | None = None,
@@ -429,15 +430,15 @@
     pPr: Typed[ParagraphProperties, Literal[True]]
     properties: Alias
     endParaRPr: Typed[CharacterProperties, Literal[True]]
     r: Incomplete
     text: Alias
     br: Typed[LineBreak, Literal[True]]
     fld: Typed[TextField, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         pPr: ParagraphProperties | None = None,
         endParaRPr: CharacterProperties | None = None,
         r: Incomplete | None = None,
         br: LineBreak | None = None,
         fld: TextField | None = None,
@@ -487,15 +488,15 @@
     prstTxWarp: Typed[PresetTextShape, Literal[True]]
     scene3d: Typed[Scene3D, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     noAutofit: Incomplete
     normAutofit: Incomplete
     spAutoFit: Incomplete
     flatTx: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         rot: _ConvertibleToInt | None = None,
         spcFirstLastPara: _ConvertibleToBool | None = None,
         vertOverflow: _RichTextPropertiesVertOverflow | Literal["none"] | None = None,
         horzOverflow: _RichTextPropertiesHorzOverflow | Literal["none"] | None = None,
         vert: _RichTextPropertiesVert | Literal["none"] | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/formatting/formatting.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/formatting.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/formatting/rule.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/rule.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors import Float, Strict
 from openpyxl.descriptors.base import Bool, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.differential import DifferentialStyle
@@ -71,29 +72,29 @@
 
 class FormatObject(Serialisable):
     tagname: str
     type: Set[_FormatObjectType]
     val: Incomplete
     gte: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, type: _FormatObjectType, val: Incomplete | None = None, gte: _ConvertibleToBool | None = None, extLst: Unused = None
     ) -> None: ...
 
 class RuleType(Serialisable):
     cfvo: Incomplete
 
 class IconSet(RuleType):
     tagname: str
     iconSet: NoneSet[_IconSetIconSet]
     showValue: Bool[Literal[True]]
     percent: Bool[Literal[True]]
     reverse: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     cfvo: Incomplete
     def __init__(
         self,
         iconSet: _IconSetIconSet | Literal["none"] | None = None,
         showValue: _ConvertibleToBool | None = None,
         percent: _ConvertibleToBool | None = None,
         reverse: _ConvertibleToBool | None = None,
@@ -102,29 +103,29 @@
 
 class DataBar(RuleType):
     tagname: str
     minLength: Integer[Literal[True]]
     maxLength: Integer[Literal[True]]
     showValue: Bool[Literal[True]]
     color: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     cfvo: Incomplete
     def __init__(
         self,
         minLength: _ConvertibleToInt | None = None,
         maxLength: _ConvertibleToInt | None = None,
         showValue: _ConvertibleToBool | None = None,
         cfvo: Incomplete | None = None,
         color: Incomplete | None = None,
     ) -> None: ...
 
 class ColorScale(RuleType):
     tagname: str
     color: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     cfvo: Incomplete
     def __init__(self, cfvo: Incomplete | None = None, color: Incomplete | None = None) -> None: ...
 
 class Rule(Serialisable):
     tagname: str
     type: Set[_RuleType]
     dxfId: Integer[Literal[True]]
@@ -141,16 +142,16 @@
     equalAverage: Bool[Literal[True]]
     formula: Incomplete
     colorScale: Typed[ColorScale, Literal[True]]
     dataBar: Typed[DataBar, Literal[True]]
     iconSet: Typed[IconSet, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     dxf: Typed[DifferentialStyle, Literal[True]]
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         type: _RuleType,
         dxfId: _ConvertibleToInt | None = None,
         priority: _ConvertibleToInt = 0,
         stopIfTrue: _ConvertibleToBool | None = None,
         aboveAverage: _ConvertibleToBool | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/formula/tokenizer.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/formula/tokenizer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/formula/translate.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/formula/translate.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/core.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/core.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 
 from openpyxl.descriptors import DateTime
 from openpyxl.descriptors.base import Alias
 from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 
 # Does not reimplement the relevant methods, so runtime also has incompatible supertypes
@@ -32,15 +33,15 @@
     title: Incomplete
     creator: Incomplete
     description: Incomplete
     identifier: Incomplete
     language: Incomplete
     created: Incomplete
     modified: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         category: Incomplete | None = None,
         contentStatus: Incomplete | None = None,
         keywords: Incomplete | None = None,
         lastModifiedBy: Incomplete | None = None,
         lastPrinted: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/custom.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/custom.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/manifest.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/manifest.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete
 from collections.abc import Generator
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import String
 from openpyxl.descriptors.serialisable import Serialisable
 
 mimetypes: Incomplete
 
@@ -23,15 +24,15 @@
 DEFAULT_OVERRIDE: Incomplete
 
 class Manifest(Serialisable):
     tagname: str
     Default: Incomplete
     Override: Incomplete
     path: str
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, Default=(), Override=()) -> None: ...
     @property
     def filenames(self): ...
     @property
     def extensions(self): ...
     def to_tree(self): ...
     def __contains__(self, content_type): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/relationship.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/relationship.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/packaging/workbook.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/workbook.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.workbook.defined_name import DefinedNameList
 from openpyxl.workbook.function_group import FunctionGroupList
@@ -68,15 +69,15 @@
     smartTagPr: Typed[SmartTagProperties, Literal[True]]
     smartTagTypes: Typed[SmartTagList, Literal[True]]
     webPublishing: Typed[WebPublishing, Literal[True]]
     fileRecoveryPr: Typed[FileRecoveryProperties, Literal[True]]
     webPublishObjects: Typed[WebPublishObjectList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     Ignorable: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         conformance: _WorkbookPackageConformance | Literal["none"] | None = None,
         fileVersion: FileVersion | None = None,
         fileSharing: FileSharing | None = None,
         workbookPr: WorkbookProperties | None = None,
         workbookProtection: WorkbookProtection | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/cache.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/cache.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from _typeshed import Incomplete, Unused
 from datetime import datetime
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Bool,
     DateTime,
     Float,
     Integer,
@@ -52,15 +52,15 @@
     mdx: String[Literal[False]]
     memberName: String[Literal[False]]
     hierarchy: String[Literal[False]]
     parent: String[Literal[False]]
     solveOrder: Integer[Literal[False]]
     set: Bool[Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         name: str,
         mdx: str,
         memberName: str,
         hierarchy: str,
         parent: str,
@@ -71,15 +71,15 @@
 
 class CalculatedItem(Serialisable):
     tagname: str
     field: Integer[Literal[True]]
     formula: String[Literal[False]]
     pivotArea: Typed[PivotArea, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self, field: _ConvertibleToInt | None = None, *, formula: str, pivotArea: PivotArea, extLst: Incomplete | None = None
     ) -> None: ...
     @overload
     def __init__(
         self, field: _ConvertibleToInt | None, formula: str, pivotArea: PivotArea, extLst: Incomplete | None = None
@@ -90,79 +90,79 @@
     culture: String[Literal[True]]
     format: String[Literal[True]]
     def __init__(self, culture: str | None = None, format: str | None = None) -> None: ...
 
 class ServerFormatList(Serialisable):
     tagname: str
     serverFormat: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, serverFormat: Incomplete | None = None) -> None: ...
     @property
     def count(self): ...
 
 class Query(Serialisable):
     tagname: str
     mdx: String[Literal[False]]
     tpls: Typed[TupleList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, mdx: str, tpls: TupleList | None = None) -> None: ...
 
 class QueryCache(Serialisable):
     tagname: str
     count: Integer[Literal[False]]
     query: Typed[Query, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, query: Query) -> None: ...
 
 class OLAPSet(Serialisable):
     tagname: str
     count: Integer[Literal[False]]
     maxRank: Integer[Literal[False]]
     setDefinition: String[Literal[False]]
     sortType: Incomplete
     queryFailed: Bool[Literal[False]]
     tpls: Typed[TupleList, Literal[True]]
     sortByTuple: Typed[TupleList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         count: _ConvertibleToInt,
         maxRank: _ConvertibleToInt,
         setDefinition: str,
         sortType: Incomplete | None = None,
         queryFailed: _ConvertibleToBool = None,
         tpls: TupleList | None = None,
         sortByTuple: TupleList | None = None,
     ) -> None: ...
 
 class OLAPSets(Serialisable):
     count: Integer[Literal[False]]
     set: Typed[OLAPSet, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, set: OLAPSet) -> None: ...
 
 class PCDSDTCEntries(Serialisable):
     tagname: str
     count: Integer[Literal[False]]
     m: Typed[Missing, Literal[False]]
     n: Typed[Number, Literal[False]]
     e: Typed[Error, Literal[False]]
     s: Typed[Text, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, m: Missing, n: Number, e: Error, s: Text) -> None: ...
 
 class TupleCache(Serialisable):
     tagname: str
     entries: Typed[PCDSDTCEntries, Literal[True]]
     sets: Typed[OLAPSets, Literal[True]]
     queryCache: Typed[QueryCache, Literal[True]]
     serverFormats: Typed[ServerFormatList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         entries: PCDSDTCEntries | None = None,
         sets: OLAPSets | None = None,
         queryCache: QueryCache | None = None,
         serverFormats: ServerFormatList | None = None,
         extLst: ExtensionList | None = None,
@@ -218,71 +218,71 @@
     uniqueName: String[Literal[False]]
     group: Bool[Literal[False]]
     def __init__(self, uniqueName: str, group: _ConvertibleToBool = None) -> None: ...
 
 class GroupMembers(Serialisable):
     count: Integer[Literal[False]]
     groupMember: Typed[GroupMember, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, groupMember: GroupMember) -> None: ...
 
 class LevelGroup(Serialisable):
     tagname: str
     name: String[Literal[False]]
     uniqueName: String[Literal[False]]
     caption: String[Literal[False]]
     uniqueParent: String[Literal[False]]
     id: Integer[Literal[False]]
     groupMembers: Typed[GroupMembers, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, name: str, uniqueName: str, caption: str, uniqueParent: str, id: _ConvertibleToInt, groupMembers: GroupMembers
     ) -> None: ...
 
 class Groups(Serialisable):
     tagname: str
     count: Integer[Literal[False]]
     group: Typed[LevelGroup, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, group: LevelGroup) -> None: ...
 
 class GroupLevel(Serialisable):
     tagname: str
     uniqueName: String[Literal[False]]
     caption: String[Literal[False]]
     user: Bool[Literal[False]]
     customRollUp: Bool[Literal[False]]
     groups: Typed[Groups, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         uniqueName: str,
         caption: str,
         user: _ConvertibleToBool = None,
         customRollUp: _ConvertibleToBool = None,
         groups: Groups | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class GroupLevels(Serialisable):
     count: Integer[Literal[False]]
     groupLevel: Typed[GroupLevel, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, groupLevel: GroupLevel) -> None: ...
 
 class FieldUsage(Serialisable):
     tagname: str
     x: Integer[Literal[False]]
     def __init__(self, x: _ConvertibleToInt) -> None: ...
 
 class FieldsUsage(Serialisable):
     count: Integer[Literal[False]]
     fieldUsage: Typed[FieldUsage, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, fieldUsage: FieldUsage | None = None) -> None: ...
 
 class CacheHierarchy(Serialisable):
     tagname: str
     uniqueName: String[Literal[False]]
     caption: String[Literal[True]]
     measure: Bool[Literal[False]]
@@ -304,15 +304,15 @@
     memberValueDatatype: Integer[Literal[True]]
     unbalanced: Bool[Literal[True]]
     unbalancedGroup: Bool[Literal[True]]
     hidden: Bool[Literal[False]]
     fieldsUsage: Typed[FieldsUsage, Literal[True]]
     groupLevels: Typed[GroupLevels, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         uniqueName: str = "",
         caption: str | None = None,
         measure: _ConvertibleToBool = None,
         set: _ConvertibleToBool = None,
@@ -373,25 +373,25 @@
     tagname: str
     m: Incomplete
     n: Incomplete
     b: Incomplete
     e: Incomplete
     s: Incomplete
     d: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, m=(), n=(), b=(), e=(), s=(), d=()) -> None: ...
     @property
     def count(self): ...
 
 class DiscretePr(Serialisable):
     tagname: str
     count: Integer[Literal[False]]
     x: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, x: Incomplete | None = None) -> None: ...
 
 class RangePr(Serialisable):
     tagname: str
     autoStart: Bool[Literal[True]]
     autoEnd: Bool[Literal[True]]
     groupBy: Set[_RangePrGroupBy]
@@ -415,15 +415,15 @@
 class FieldGroup(Serialisable):
     tagname: str
     par: Integer[Literal[True]]
     base: Integer[Literal[True]]
     rangePr: Typed[RangePr, Literal[True]]
     discretePr: Typed[DiscretePr, Literal[True]]
     groupItems: Typed[GroupItems, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         par: _ConvertibleToInt | None = None,
         base: _ConvertibleToInt | None = None,
         rangePr: RangePr | None = None,
         discretePr: DiscretePr | None = None,
         groupItems: GroupItems | None = None,
@@ -446,15 +446,15 @@
     containsNumber: Bool[Literal[True]]
     containsInteger: Bool[Literal[True]]
     minValue: Float[Literal[True]]
     maxValue: Float[Literal[True]]
     minDate: DateTime[Literal[True]]
     maxDate: DateTime[Literal[True]]
     longText: Bool[Literal[True]]
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         _fields=(),
         containsSemiMixedTypes: _ConvertibleToBool | None = None,
         containsNonDate: _ConvertibleToBool | None = None,
         containsDate: _ConvertibleToBool | None = None,
         containsString: _ConvertibleToBool | None = None,
@@ -487,15 +487,15 @@
     formula: String[Literal[True]]
     sqlType: Integer[Literal[True]]
     hierarchy: Integer[Literal[True]]
     level: Integer[Literal[True]]
     databaseField: Bool[Literal[True]]
     mappingCount: Integer[Literal[True]]
     memberPropertyField: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         sharedItems: SharedItems | None = None,
         fieldGroup: FieldGroup | None = None,
         mpMap: Incomplete | None = None,
         extLst: ExtensionList | None = None,
@@ -573,25 +573,25 @@
     tagname: str
     name: String[Literal[False]]
     def __init__(self, name: str) -> None: ...
 
 class Page(Serialisable):
     tagname: str
     pageItem: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, pageItem: Incomplete | None = None) -> None: ...
     @property
     def count(self): ...
 
 class Consolidation(Serialisable):
     tagname: str
     autoPage: Bool[Literal[True]]
     pages: Incomplete
     rangeSets: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, autoPage: _ConvertibleToBool | None = None, pages=(), rangeSets=()) -> None: ...
 
 class WorksheetSource(Serialisable):
     tagname: str
     ref: String[Literal[True]]
     name: String[Literal[True]]
     sheet: String[Literal[True]]
@@ -600,15 +600,15 @@
 class CacheSource(Serialisable):
     tagname: str
     type: Set[_CacheSourceType]
     connectionId: Integer[Literal[True]]
     worksheetSource: Typed[WorksheetSource, Literal[True]]
     consolidation: Typed[Consolidation, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         type: _CacheSourceType,
         connectionId: _ConvertibleToInt | None = None,
         worksheetSource: WorksheetSource | None = None,
         consolidation: Consolidation | None = None,
         extLst: ExtensionList | None = None,
@@ -644,15 +644,15 @@
     calculatedItems: Incomplete
     calculatedMembers: Incomplete
     dimensions: Incomplete
     measureGroups: Incomplete
     maps: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     id: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         invalid: _ConvertibleToBool | None = None,
         saveData: _ConvertibleToBool | None = None,
         refreshOnLoad: _ConvertibleToBool | None = None,
         optimizeMemory: _ConvertibleToBool | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/fields.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/fields.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from _typeshed import Incomplete
 from datetime import datetime
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import (
     Bool,
     DateTime,
     Float,
     Integer,
@@ -26,15 +26,15 @@
     hier: Integer[Literal[False]]
     item: Integer[Literal[False]]
     def __init__(self, fld: _ConvertibleToInt, hier: _ConvertibleToInt, item: _ConvertibleToInt) -> None: ...
 
 class TupleList(Serialisable):
     c: Integer[Literal[True]]
     tpl: Typed[Tuple, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(self, c: _ConvertibleToInt | None = None, *, tpl: Tuple) -> None: ...
     @overload
     def __init__(self, c: _ConvertibleToInt | None, tpl: Tuple) -> None: ...
 
 class Missing(Serialisable):
     tagname: str
@@ -47,15 +47,15 @@
     _in: Integer[Literal[True]]  # Not private. Avoids name clash
     bc: Incomplete
     fc: Incomplete
     i: Bool[Literal[True]]
     un: Bool[Literal[True]]
     st: Bool[Literal[True]]
     b: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         tpls=(),
         x=(),
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
@@ -81,15 +81,15 @@
     _in: Integer[Literal[True]]  # Not private. Avoids name clash
     bc: Incomplete
     fc: Incomplete
     i: Bool[Literal[True]]
     un: Bool[Literal[True]]
     st: Bool[Literal[True]]
     b: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         tpls=(),
         x=(),
         *,
         v: _ConvertibleToFloat,
@@ -136,15 +136,15 @@
     _in: Integer[Literal[True]]  # Not private. Avoids name clash
     bc: Incomplete
     fc: Incomplete
     i: Bool[Literal[True]]
     un: Bool[Literal[True]]
     st: Bool[Literal[True]]
     b: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         tpls: TupleList | None = None,
         x=(),
         *,
         v: str,
@@ -183,15 +183,15 @@
     tagname: str
     x: Incomplete
     v: Bool[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         x=(),
         v: _ConvertibleToBool = None,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
@@ -210,15 +210,15 @@
     _in: Integer[Literal[True]]  # Not private. Avoids name clash
     bc: Incomplete
     fc: Incomplete
     i: Bool[Literal[True]]
     un: Bool[Literal[True]]
     st: Bool[Literal[True]]
     b: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         tpls=(),
         x=(),
         v: Incomplete | None = None,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
@@ -237,15 +237,15 @@
     tagname: str
     x: Incomplete
     v: DateTime[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         x=(),
         v: datetime | str | None = None,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/pivot/table.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/table.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.filters import AutoFilter
 
@@ -109,25 +109,25 @@
     tagname: str
     hierarchyUsage: Integer[Literal[False]]
     def __init__(self, hierarchyUsage: _ConvertibleToInt) -> None: ...
 
 class ColHierarchiesUsage(Serialisable):
     tagname: str
     colHierarchyUsage: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, colHierarchyUsage=()) -> None: ...
     @property
     def count(self): ...
 
 class RowHierarchiesUsage(Serialisable):
     tagname: str
     rowHierarchyUsage: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, rowHierarchyUsage=()) -> None: ...
     @property
     def count(self): ...
 
 class PivotFilter(Serialisable):
     tagname: str
     fld: Integer[Literal[False]]
@@ -139,15 +139,15 @@
     iMeasureFld: Integer[Literal[True]]
     name: String[Literal[True]]
     description: String[Literal[True]]
     stringValue1: String[Literal[True]]
     stringValue2: String[Literal[True]]
     autoFilter: Typed[AutoFilter, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         fld: _ConvertibleToInt,
         mpFld: _ConvertibleToInt | None = None,
         *,
         type: _PivotFilterType,
@@ -179,15 +179,15 @@
         autoFilter: AutoFilter,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class PivotFilters(Serialisable):
     count: Integer[Literal[False]]
     filter: Typed[PivotFilter, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: _ConvertibleToInt, filter: PivotFilter | None = None) -> None: ...
 
 class PivotTableStyle(Serialisable):
     tagname: str
     name: String[Literal[True]]
     showRowHeaders: Bool[Literal[False]]
     showColHeaders: Bool[Literal[False]]
@@ -204,15 +204,15 @@
         showLastColumn: _ConvertibleToBool = None,
     ) -> None: ...
 
 class MemberList(Serialisable):
     tagname: str
     level: Integer[Literal[True]]
     member: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, level: _ConvertibleToInt | None = None, member=()) -> None: ...
     @property
     def count(self): ...
 
 class MemberProperty(Serialisable):
     tagname: str
     name: String[Literal[True]]
@@ -264,15 +264,15 @@
     dragToData: Bool[Literal[False]]
     dragOff: Bool[Literal[False]]
     includeNewItemsInFilter: Bool[Literal[False]]
     caption: String[Literal[True]]
     mps: Incomplete
     members: Typed[MemberList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         outline: _ConvertibleToBool = None,
         multipleItemSelectionAllowed: _ConvertibleToBool = None,
         subtotalTop: _ConvertibleToBool = None,
         showInFieldList: _ConvertibleToBool = None,
         dragToRow: _ConvertibleToBool = None,
@@ -303,15 +303,15 @@
     countSubtotal: Bool[Literal[True]]
     stdDevSubtotal: Bool[Literal[True]]
     stdDevPSubtotal: Bool[Literal[True]]
     varSubtotal: Bool[Literal[True]]
     varPSubtotal: Bool[Literal[True]]
     x: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         field: _ConvertibleToInt | None = None,
         count: Unused = None,
         selected: _ConvertibleToBool | None = None,
         byPosition: _ConvertibleToBool | None = None,
         relative: _ConvertibleToBool | None = None,
@@ -345,15 +345,15 @@
     grandCol: Bool[Literal[True]]
     cacheIndex: Bool[Literal[True]]
     outline: Bool[Literal[True]]
     offset: String[Literal[True]]
     collapsedLevelsAreSubtotals: Bool[Literal[True]]
     axis: NoneSet[_PivotAxis]
     fieldPosition: Integer[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         references=(),
         extLst: ExtensionList | None = None,
         field: _ConvertibleToInt | None = None,
         type: _PivotAreaType | Literal["none"] | None = "normal",
         dataOnly: _ConvertibleToBool | None = True,
@@ -370,15 +370,15 @@
 
 class ChartFormat(Serialisable):
     tagname: str
     chart: Integer[Literal[False]]
     format: Integer[Literal[False]]
     series: Bool[Literal[False]]
     pivotArea: Typed[PivotArea, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self, chart: _ConvertibleToInt, format: _ConvertibleToInt, series: _ConvertibleToBool = None, *, pivotArea: PivotArea
     ) -> None: ...
     @overload
     def __init__(
         self, chart: _ConvertibleToInt, format: _ConvertibleToInt, series: _ConvertibleToBool, pivotArea: PivotArea
@@ -387,15 +387,15 @@
 class ConditionalFormat(Serialisable):
     tagname: str
     scope: Set[_ConditionalFormatScope]
     type: NoneSet[_ConditionalFormatType]
     priority: Integer[Literal[False]]
     pivotAreas: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         scope: _ConditionalFormatScope = "selection",
         type: _ConditionalFormatType | Literal["none"] | None = None,
         *,
         priority: _ConvertibleToInt,
@@ -411,28 +411,28 @@
         pivotAreas=(),
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class ConditionalFormatList(Serialisable):
     tagname: str
     conditionalFormat: Incomplete
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, conditionalFormat=..., count: Incomplete | None = ...) -> None: ...
     def by_priority(self): ...
     @property
     def count(self): ...
     def to_tree(self, tagname: Incomplete | None = ...): ...  # type: ignore[override]
 
 class Format(Serialisable):
     tagname: str
     action: NoneSet[_FormatAction]
     dxfId: Integer[Literal[True]]
     pivotArea: Typed[PivotArea, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         action: _FormatAction | Literal["none"] | None = "formatting",
         dxfId: _ConvertibleToInt | None = None,
         *,
         pivotArea: PivotArea,
@@ -453,15 +453,15 @@
     fld: Integer[Literal[False]]
     subtotal: Set[_DataFieldSubtotal]
     showDataAs: Set[_DataFieldShowDataAs]
     baseField: Integer[Literal[False]]
     baseItem: Integer[Literal[False]]
     numFmtId: Integer[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         name: str | None = None,
         *,
         fld: _ConvertibleToInt,
         subtotal: str = "sum",
@@ -488,15 +488,15 @@
     tagname: str
     fld: Integer[Literal[False]]
     item: Integer[Literal[True]]
     hier: Integer[Literal[True]]
     name: String[Literal[True]]
     cap: String[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         fld: _ConvertibleToInt,
         item: _ConvertibleToInt | None = None,
         hier: _ConvertibleToInt | None = None,
         name: str | None = None,
         cap: str | None = None,
@@ -505,25 +505,25 @@
 
 class RowColItem(Serialisable):
     tagname: str
     t: Set[_ItemType]
     r: Integer[Literal[False]]
     i: Integer[Literal[False]]
     x: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, t: _ItemType = "data", r: _ConvertibleToInt = 0, i: _ConvertibleToInt = 0, x=()) -> None: ...
 
 class RowColField(Serialisable):
     tagname: str
     x: Integer[Literal[False]]
     def __init__(self, x: _ConvertibleToInt) -> None: ...
 
 class AutoSortScope(Serialisable):
     pivotArea: Typed[PivotArea, Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, pivotArea: PivotArea) -> None: ...
 
 class FieldItem(Serialisable):
     tagname: str
     n: String[Literal[True]]
     t: Set[_ItemType]
     h: Bool[Literal[True]]
@@ -599,15 +599,15 @@
     stdDevPSubtotal: Bool[Literal[True]]
     varSubtotal: Bool[Literal[True]]
     varPSubtotal: Bool[Literal[True]]
     showPropCell: Bool[Literal[True]]
     showPropTip: Bool[Literal[True]]
     showPropAsCaption: Bool[Literal[True]]
     defaultAttributeDrillState: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         items=(),
         autoSortScope: AutoSortScope | None = None,
         name: str | None = None,
         axis: _PivotAxis | Literal["none"] | None = None,
         dataField: _ConvertibleToBool | None = None,
@@ -764,15 +764,15 @@
     pivotHierarchies: Incomplete
     pivotTableStyleInfo: Typed[PivotTableStyle, Literal[True]]
     filters: Incomplete
     rowHierarchiesUsage: Typed[RowHierarchiesUsage, Literal[True]]
     colHierarchiesUsage: Typed[ColHierarchiesUsage, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     id: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         name: str,
         cacheId: _ConvertibleToInt,
         dataOnRows: _ConvertibleToBool = False,
         dataPosition: _ConvertibleToInt | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/reader/excel.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/reader/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/reader/workbook.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/reader/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/__init__.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/alignment.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/alignment.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/borders.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/borders.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _SideStyle: TypeAlias = Literal[
     "dashDot",
@@ -46,15 +47,15 @@
         color: Incomplete | None = None,
         border_style: Incomplete | None = None,
     ) -> None: ...
 
 class Border(Serialisable):
     tagname: str
     __fields__: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     start: Typed[Side, Literal[True]]
     end: Typed[Side, Literal[True]]
     left: Typed[Side, Literal[True]]
     right: Typed[Side, Literal[True]]
     top: Typed[Side, Literal[True]]
     bottom: Typed[Side, Literal[True]]
     diagonal: Typed[Side, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/builtins.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/builtins.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/cell_style.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/cell_style.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete, Unused
 from array import array
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors import Strict
 from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.alignment import Alignment
@@ -46,16 +47,16 @@
     applyBorder: Bool[Literal[True]]
     # Overwritten by properties below
     # applyAlignment: Bool[Literal[True]]
     # applyProtection: Bool[Literal[True]]
     alignment: Typed[Alignment, Literal[True]]
     protection: Typed[Protection, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         numFmtId: _ConvertibleToInt = 0,
         fontId: _ConvertibleToInt = 0,
         fillId: _ConvertibleToInt = 0,
         borderId: _ConvertibleToInt = 0,
         xfId: _ConvertibleToInt | None = None,
@@ -77,18 +78,18 @@
     @property
     def applyProtection(self): ...
     @property
     def applyAlignment(self): ...
 
 class CellStyleList(Serialisable):
     tagname: str
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     # Overwritten by property below
     # count: Integer
     xf: Incomplete
     alignment: Incomplete
     protection: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, xf=()) -> None: ...
     @property
     def count(self): ...
     def __getitem__(self, idx): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/colors.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/colors.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors import Strict, Typed
 from openpyxl.descriptors.base import Bool, Integer, MinMax, String, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 COLOR_INDEX: Incomplete
@@ -51,12 +52,12 @@
     rgb: Incomplete
     def __init__(self, rgb: Incomplete | None = None) -> None: ...
 
 class ColorList(Serialisable):
     tagname: str
     indexedColors: Incomplete
     mruColors: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, indexedColors=(), mruColors=()) -> None: ...
     def __bool__(self) -> bool: ...
     @property
     def index(self): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/differential.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/differential.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles import Alignment, Border, Fill, Font, Protection
 from openpyxl.styles.numbers import NumberFormat
 
 class DifferentialStyle(Serialisable):
     tagname: str
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     font: Typed[Font, Literal[True]]
     numFmt: Typed[NumberFormat, Literal[True]]
     fill: Typed[Fill, Literal[True]]
     alignment: Typed[Alignment, Literal[True]]
     border: Typed[Border, Literal[True]]
     protection: Typed[Protection, Literal[True]]
     extLst: ExtensionList | None
@@ -28,15 +29,15 @@
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class DifferentialStyleList(Serialisable):
     tagname: str
     dxf: Incomplete
     styles: Alias
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, dxf=(), count: Incomplete | None = None) -> None: ...
     def append(self, dxf) -> None: ...
     def add(self, dxf): ...
     def __bool__(self) -> bool: ...
     def __getitem__(self, idx): ...
     @property
     def count(self): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/fills.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fills.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Final, Literal, TypeAlias
 
 from openpyxl.descriptors import Sequence
 from openpyxl.descriptors.base import Alias, Float, MinMax, NoneSet, Set, _ConvertibleToFloat
 from openpyxl.descriptors.serialisable import Serialisable
 
 FILL_NONE: Final = "none"
@@ -52,15 +53,15 @@
 class Fill(Serialisable):
     tagname: str
     @classmethod
     def from_tree(cls, el): ...
 
 class PatternFill(Fill):
     tagname: str
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     patternType: NoneSet[_FillsType]
     fill_type: Alias
     fgColor: Incomplete
     start_color: Alias
     bgColor: Incomplete
     end_color: Alias
     def __init__(
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/fonts.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fonts.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 
 from openpyxl.descriptors.base import Alias
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Font(Serialisable):
     UNDERLINE_DOUBLE: str
     UNDERLINE_DOUBLE_ACCOUNTING: str
@@ -25,15 +26,15 @@
     extend: Incomplete
     u: Incomplete
     underline: Alias
     vertAlign: Incomplete
     color: Incomplete
     scheme: Incomplete
     tagname: str
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         name: Incomplete | None = None,
         sz: Incomplete | None = None,
         b: Incomplete | None = None,
         i: Incomplete | None = None,
         charset: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/named_styles.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/named_styles.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.alignment import Alignment
 from openpyxl.styles.borders import Border
@@ -55,15 +56,15 @@
     name: String[Literal[False]]
     xfId: Integer[Literal[False]]
     builtinId: Integer[Literal[True]]
     iLevel: Integer[Literal[True]]
     hidden: Bool[Literal[True]]
     customBuiltin: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         name: str,
         xfId: _ConvertibleToInt,
         builtinId: _ConvertibleToInt | None = None,
         iLevel: _ConvertibleToInt | None = None,
         hidden: _ConvertibleToBool | None = None,
@@ -72,13 +73,13 @@
     ) -> None: ...
 
 class _NamedCellStyleList(Serialisable):
     tagname: str
     # Overwritten by property below
     # count: Integer
     cellStyle: Incomplete
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, cellStyle=()) -> None: ...
     @property
     def count(self): ...
     @property
     def names(self): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/numbers.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/numbers.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors import Strict, String
 from openpyxl.descriptors.base import Integer, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 BUILTIN_FORMATS: Incomplete
@@ -63,13 +64,13 @@
     formatCode: String[Literal[False]]
     def __init__(self, numFmtId: _ConvertibleToInt, formatCode: str) -> None: ...
 
 class NumberFormatList(Serialisable):
     # Overwritten by property below
     # count: Integer
     numFmt: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, numFmt=()) -> None: ...
     @property
     def count(self): ...
     def __getitem__(self, idx): ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/styleable.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/styleable.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/stylesheet.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/stylesheet.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.cell_style import CellStyleList
 from openpyxl.styles.colors import ColorList
@@ -19,15 +20,15 @@
     cellStyleXfs: Typed[CellStyleList, Literal[False]]
     cellXfs: Typed[CellStyleList, Literal[False]]
     cellStyles: Typed[_NamedCellStyleList, Literal[False]]
     dxfs: Incomplete
     tableStyles: Typed[TableStyleList, Literal[True]]
     colors: Typed[ColorList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     number_formats: Incomplete
     cell_styles: Incomplete
     alignments: Incomplete
     protections: Incomplete
     named_styles: Incomplete
     def __init__(
         self,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/styles/table.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/table.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, Set, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 _TableStyleElementType: TypeAlias = Literal[
     "wholeTable",
@@ -47,31 +48,31 @@
 class TableStyle(Serialisable):
     tagname: str
     name: String[Literal[False]]
     pivot: Bool[Literal[True]]
     table: Bool[Literal[True]]
     count: Integer[Literal[True]]
     tableStyleElement: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         name: str,
         pivot: _ConvertibleToBool | None = None,
         table: _ConvertibleToBool | None = None,
         count: _ConvertibleToInt | None = None,
         tableStyleElement=(),
     ) -> None: ...
 
 class TableStyleList(Serialisable):
     tagname: str
     defaultTableStyle: String[Literal[True]]
     defaultPivotStyle: String[Literal[True]]
     tableStyle: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         count: Unused = None,
         defaultTableStyle: str | None = "TableStyleMedium9",
         defaultPivotStyle: str | None = "PivotStyleLight16",
         tableStyle=(),
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/utils/cell.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/utils/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/utils/datetime.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/utils/datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/utils/units.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/utils/units.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/_writer.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/child.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/child.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/defined_name.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/protection.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 from _typeshed import Incomplete
-from collections import defaultdict
-from collections.abc import Generator
-from re import Pattern
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.descriptors import Sequence
 from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
-RESERVED: frozenset[str]
-RESERVED_REGEX: Pattern[str]
-
-class DefinedName(Serialisable):
+class WorkbookProtection(Serialisable):
     tagname: str
-    name: String[Literal[False]]
-    comment: String[Literal[True]]
-    customMenu: String[Literal[True]]
-    description: String[Literal[True]]
-    help: String[Literal[True]]
-    statusBar: String[Literal[True]]
-    localSheetId: Integer[Literal[True]]
-    hidden: Bool[Literal[True]]
-    function: Bool[Literal[True]]
-    vbProcedure: Bool[Literal[True]]
-    xlm: Bool[Literal[True]]
-    functionGroupId: Integer[Literal[True]]
-    shortcutKey: String[Literal[True]]
-    publishToServer: Bool[Literal[True]]
-    workbookParameter: Bool[Literal[True]]
-    attr_text: Incomplete
-    value: Alias
+    workbook_password: Alias
+    workbookPasswordCharacterSet: String[Literal[True]]
+    revision_password: Alias
+    revisionsPasswordCharacterSet: String[Literal[True]]
+    lockStructure: Bool[Literal[True]]
+    lock_structure: Alias
+    lockWindows: Bool[Literal[True]]
+    lock_windows: Alias
+    lockRevision: Bool[Literal[True]]
+    lock_revision: Alias
+    revisionsAlgorithmName: String[Literal[True]]
+    revisionsHashValue: Incomplete
+    revisionsSaltValue: Incomplete
+    revisionsSpinCount: Integer[Literal[True]]
+    workbookAlgorithmName: String[Literal[True]]
+    workbookHashValue: Incomplete
+    workbookSaltValue: Incomplete
+    workbookSpinCount: Integer[Literal[True]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        name: str,
-        comment: str | None = None,
-        customMenu: str | None = None,
-        description: str | None = None,
-        help: str | None = None,
-        statusBar: str | None = None,
-        localSheetId: _ConvertibleToInt | None = None,
-        hidden: _ConvertibleToBool | None = None,
-        function: _ConvertibleToBool | None = None,
-        vbProcedure: _ConvertibleToBool | None = None,
-        xlm: _ConvertibleToBool | None = None,
-        functionGroupId: _ConvertibleToInt | None = None,
-        shortcutKey: str | None = None,
-        publishToServer: _ConvertibleToBool | None = None,
-        workbookParameter: _ConvertibleToBool | None = None,
-        attr_text: Incomplete | None = None,
+        workbookPassword: Incomplete | None = None,
+        workbookPasswordCharacterSet: str | None = None,
+        revisionsPassword: Incomplete | None = None,
+        revisionsPasswordCharacterSet: str | None = None,
+        lockStructure: _ConvertibleToBool | None = None,
+        lockWindows: _ConvertibleToBool | None = None,
+        lockRevision: _ConvertibleToBool | None = None,
+        revisionsAlgorithmName: str | None = None,
+        revisionsHashValue: Incomplete | None = None,
+        revisionsSaltValue: Incomplete | None = None,
+        revisionsSpinCount: _ConvertibleToInt | None = None,
+        workbookAlgorithmName: str | None = None,
+        workbookHashValue: Incomplete | None = None,
+        workbookSaltValue: Incomplete | None = None,
+        workbookSpinCount: _ConvertibleToInt | None = None,
     ) -> None: ...
+    def set_workbook_password(self, value: str = "", already_hashed: bool = False) -> None: ...
     @property
-    def type(self): ...
-    @property
-    def destinations(self) -> Generator[Incomplete, None, None]: ...
-    @property
-    def is_reserved(self): ...
+    def workbookPassword(self): ...
+    @workbookPassword.setter
+    def workbookPassword(self, value) -> None: ...
+    def set_revisions_password(self, value: str = "", already_hashed: bool = False) -> None: ...
     @property
-    def is_external(self): ...
-    def __iter__(self): ...
+    def revisionsPassword(self): ...
+    @revisionsPassword.setter
+    def revisionsPassword(self, value) -> None: ...
+    @classmethod
+    def from_tree(cls, node): ...
 
-class DefinedNameDict(dict[str, DefinedName]):
-    def add(self, value: DefinedName) -> None: ...
+DocumentSecurity = WorkbookProtection
 
-class DefinedNameList(Serialisable):
+class FileSharing(Serialisable):
     tagname: str
-    definedName: Sequence
-    def __init__(self, definedName=()) -> None: ...
-    def by_sheet(self) -> defaultdict[int, DefinedNameDict]: ...
-    def __len__(self) -> int: ...
+    readOnlyRecommended: Bool[Literal[True]]
+    userName: String[Literal[True]]
+    reservationPassword: Incomplete
+    algorithmName: String[Literal[True]]
+    hashValue: Incomplete
+    saltValue: Incomplete
+    spinCount: Integer[Literal[True]]
+    def __init__(
+        self,
+        readOnlyRecommended: _ConvertibleToBool | None = None,
+        userName: str | None = None,
+        reservationPassword: Incomplete | None = None,
+        algorithmName: str | None = None,
+        hashValue: Incomplete | None = None,
+        saltValue: Incomplete | None = None,
+        spinCount: _ConvertibleToInt | None = None,
+    ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/external_link/external.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/controls.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,65 @@
-from _typeshed import Incomplete, Unused
-from typing_extensions import Literal, TypeAlias
+from _typeshed import Incomplete
+from typing import ClassVar, overload
+from typing_extensions import Literal
 
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.packaging.relationship import Relationship
+from openpyxl.worksheet.ole import ObjectAnchor
 
-_ExternalCellType: TypeAlias = Literal["b", "d", "n", "e", "s", "str", "inlineStr"]
-
-class ExternalCell(Serialisable):
-    r: String[Literal[False]]
-    t: NoneSet[_ExternalCellType]
-    vm: Integer[Literal[True]]
-    v: Incomplete
-    def __init__(
-        self,
-        r: str,
-        t: _ExternalCellType | Literal["none"] | None = None,
-        vm: _ConvertibleToInt | None = None,
-        v: Incomplete | None = None,
-    ) -> None: ...
-
-class ExternalRow(Serialisable):
-    r: Integer[Literal[False]]
-    cell: Incomplete
-    __elements__: Incomplete
-    def __init__(self, r: _ConvertibleToInt, cell: Incomplete | None = None) -> None: ...
-
-class ExternalSheetData(Serialisable):
-    sheetId: Integer[Literal[False]]
-    refreshError: Bool[Literal[True]]
-    row: Incomplete
-    __elements__: Incomplete
-    def __init__(self, sheetId: _ConvertibleToInt, refreshError: _ConvertibleToBool | None = None, row=()) -> None: ...
-
-class ExternalSheetDataSet(Serialisable):
-    sheetData: Incomplete
-    __elements__: Incomplete
-    def __init__(self, sheetData: Incomplete | None = None) -> None: ...
-
-class ExternalSheetNames(Serialisable):
-    sheetName: Incomplete
-    __elements__: Incomplete
-    def __init__(self, sheetName=()) -> None: ...
-
-class ExternalDefinedName(Serialisable):
+class ControlProperty(Serialisable):
     tagname: str
-    name: String[Literal[False]]
-    refersTo: String[Literal[True]]
-    sheetId: Integer[Literal[True]]
-    def __init__(self, name: str, refersTo: str | None = None, sheetId: _ConvertibleToInt | None = None) -> None: ...
-
-class ExternalBook(Serialisable):
-    tagname: str
-    sheetNames: Typed[ExternalSheetNames, Literal[True]]
-    definedNames: Incomplete
-    sheetDataSet: Typed[ExternalSheetDataSet, Literal[True]]
+    anchor: Typed[ObjectAnchor, Literal[False]]
+    locked: Bool[Literal[True]]
+    defaultSize: Bool[Literal[True]]
+    _print: Bool[Literal[True]]  # Not private. Avoids name clash
+    disabled: Bool[Literal[True]]
+    recalcAlways: Bool[Literal[True]]
+    uiObject: Bool[Literal[True]]
+    autoFill: Bool[Literal[True]]
+    autoLine: Bool[Literal[True]]
+    autoPict: Bool[Literal[True]]
+    macro: String[Literal[True]]
+    altText: String[Literal[True]]
+    linkedCell: String[Literal[True]]
+    listFillRange: String[Literal[True]]
+    cf: String[Literal[True]]
     id: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        sheetNames: ExternalSheetNames | None = None,
-        definedNames=(),
-        sheetDataSet: ExternalSheetDataSet | None = None,
+        anchor: ObjectAnchor,
+        locked: _ConvertibleToBool | None = True,
+        defaultSize: _ConvertibleToBool | None = True,
+        _print: _ConvertibleToBool | None = True,
+        disabled: _ConvertibleToBool | None = False,
+        recalcAlways: _ConvertibleToBool | None = False,
+        uiObject: _ConvertibleToBool | None = False,
+        autoFill: _ConvertibleToBool | None = True,
+        autoLine: _ConvertibleToBool | None = True,
+        autoPict: _ConvertibleToBool | None = True,
+        macro: str | None = None,
+        altText: str | None = None,
+        linkedCell: str | None = None,
+        listFillRange: str | None = None,
+        cf: str | None = "pict",
         id: Incomplete | None = None,
     ) -> None: ...
 
-class ExternalLink(Serialisable):
+class Control(Serialisable):
     tagname: str
-    mime_type: str
-    externalBook: Typed[ExternalBook, Literal[True]]
-    file_link: Typed[Relationship, Literal[True]]
-    __elements__: Incomplete
+    controlPr: Typed[ControlProperty, Literal[True]]
+    shapeId: Integer[Literal[False]]
+    name: String[Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    @overload
     def __init__(
-        self, externalBook: ExternalBook | None = None, ddeLink: Unused = None, oleLink: Unused = None, extLst: Unused = None
+        self, controlPr: ControlProperty | None = None, *, shapeId: _ConvertibleToInt, name: str | None = None
     ) -> None: ...
-    def to_tree(self): ...
-    @property
-    def path(self): ...
+    @overload
+    def __init__(self, controlPr: ControlProperty | None, shapeId: _ConvertibleToInt, name: str | None = None) -> None: ...
 
-def read_external_link(archive, book_path): ...
+class Controls(Serialisable):
+    tagname: str
+    control: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, control=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/function_group.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/function_group.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Integer, String, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 class FunctionGroup(Serialisable):
     tagname: str
     name: String[Literal[False]]
     def __init__(self, name: str) -> None: ...
 
 class FunctionGroupList(Serialisable):
     tagname: str
     builtInGroupCount: Integer[Literal[True]]
     functionGroup: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, builtInGroupCount: _ConvertibleToInt | None = 16, functionGroup=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/properties.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/protection.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/scenario.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,96 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
-from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import (
+    Bool,
+    Convertible,
+    Integer,
+    String,
+    _ConvertibleToBool,
+    _ConvertibleToInt,
+    _ConvertibleToMultiCellRange,
+)
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.worksheet.cell_range import MultiCellRange
 
-class WorkbookProtection(Serialisable):
+class InputCells(Serialisable):
     tagname: str
-    workbook_password: Alias
-    workbookPasswordCharacterSet: String[Literal[True]]
-    revision_password: Alias
-    revisionsPasswordCharacterSet: String[Literal[True]]
-    lockStructure: Bool[Literal[True]]
-    lock_structure: Alias
-    lockWindows: Bool[Literal[True]]
-    lock_windows: Alias
-    lockRevision: Bool[Literal[True]]
-    lock_revision: Alias
-    revisionsAlgorithmName: String[Literal[True]]
-    revisionsHashValue: Incomplete
-    revisionsSaltValue: Incomplete
-    revisionsSpinCount: Integer[Literal[True]]
-    workbookAlgorithmName: String[Literal[True]]
-    workbookHashValue: Incomplete
-    workbookSaltValue: Incomplete
-    workbookSpinCount: Integer[Literal[True]]
-    __attrs__: Incomplete
+    r: String[Literal[False]]
+    deleted: Bool[Literal[True]]
+    undone: Bool[Literal[True]]
+    val: String[Literal[False]]
+    numFmtId: Integer[Literal[True]]
+
+    @overload
     def __init__(
         self,
-        workbookPassword: Incomplete | None = None,
-        workbookPasswordCharacterSet: str | None = None,
-        revisionsPassword: Incomplete | None = None,
-        revisionsPasswordCharacterSet: str | None = None,
-        lockStructure: _ConvertibleToBool | None = None,
-        lockWindows: _ConvertibleToBool | None = None,
-        lockRevision: _ConvertibleToBool | None = None,
-        revisionsAlgorithmName: str | None = None,
-        revisionsHashValue: Incomplete | None = None,
-        revisionsSaltValue: Incomplete | None = None,
-        revisionsSpinCount: _ConvertibleToInt | None = None,
-        workbookAlgorithmName: str | None = None,
-        workbookHashValue: Incomplete | None = None,
-        workbookSaltValue: Incomplete | None = None,
-        workbookSpinCount: _ConvertibleToInt | None = None,
+        r: str,
+        deleted: _ConvertibleToBool | None = False,
+        undone: _ConvertibleToBool | None = False,
+        *,
+        val: str,
+        numFmtId: _ConvertibleToInt | None = None,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        r: str,
+        deleted: _ConvertibleToBool | None,
+        undone: _ConvertibleToBool | None,
+        val: str,
+        numFmtId: _ConvertibleToInt | None = None,
     ) -> None: ...
-    def set_workbook_password(self, value: str = "", already_hashed: bool = False) -> None: ...
-    @property
-    def workbookPassword(self): ...
-    @workbookPassword.setter
-    def workbookPassword(self, value) -> None: ...
-    def set_revisions_password(self, value: str = "", already_hashed: bool = False) -> None: ...
-    @property
-    def revisionsPassword(self): ...
-    @revisionsPassword.setter
-    def revisionsPassword(self, value) -> None: ...
-    @classmethod
-    def from_tree(cls, node): ...
 
-DocumentSecurity = WorkbookProtection
+class Scenario(Serialisable):
+    tagname: str
+    inputCells: Incomplete
+    name: String[Literal[False]]
+    locked: Bool[Literal[True]]
+    hidden: Bool[Literal[True]]
+    user: String[Literal[True]]
+    comment: String[Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
+    @overload
+    def __init__(
+        self,
+        inputCells=(),
+        *,
+        name: str,
+        locked: _ConvertibleToBool | None = False,
+        hidden: _ConvertibleToBool | None = False,
+        count: Unused = None,
+        user: str | None = None,
+        comment: str | None = None,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        inputCells,
+        name: str,
+        locked: _ConvertibleToBool | None = False,
+        hidden: _ConvertibleToBool | None = False,
+        count: Unused = None,
+        user: str | None = None,
+        comment: str | None = None,
+    ) -> None: ...
+    @property
+    def count(self): ...
 
-class FileSharing(Serialisable):
+class ScenarioList(Serialisable):
     tagname: str
-    readOnlyRecommended: Bool[Literal[True]]
-    userName: String[Literal[True]]
-    reservationPassword: Incomplete
-    algorithmName: String[Literal[True]]
-    hashValue: Incomplete
-    saltValue: Incomplete
-    spinCount: Integer[Literal[True]]
+    scenario: Incomplete
+    current: Integer[Literal[True]]
+    show: Integer[Literal[True]]
+    sqref: Convertible[MultiCellRange, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        readOnlyRecommended: _ConvertibleToBool | None = None,
-        userName: str | None = None,
-        reservationPassword: Incomplete | None = None,
-        algorithmName: str | None = None,
-        hashValue: Incomplete | None = None,
-        saltValue: Incomplete | None = None,
-        spinCount: _ConvertibleToInt | None = None,
+        scenario=(),
+        current: _ConvertibleToInt | None = None,
+        show: _ConvertibleToInt | None = None,
+        sqref: _ConvertibleToMultiCellRange | None = None,
     ) -> None: ...
+    def append(self, scenario) -> None: ...
+    def __bool__(self) -> bool: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/smart_tags.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/smart_tags.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, NoneSet, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _SmartTagPropertiesShow: TypeAlias = Literal["all", "noIndicator"]
 
@@ -12,15 +13,15 @@
     name: String[Literal[True]]
     url: String[Literal[True]]
     def __init__(self, namespaceUri: str | None = None, name: str | None = None, url: str | None = None) -> None: ...
 
 class SmartTagList(Serialisable):
     tagname: str
     smartTagType: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, smartTagType=()) -> None: ...
 
 class SmartTagProperties(Serialisable):
     tagname: str
     embed: Bool[Literal[True]]
     show: NoneSet[_SmartTagPropertiesShow]
     def __init__(
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/views.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/views.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 _BookViewVilibility: TypeAlias = Literal["visible", "hidden", "veryHidden"]
@@ -22,15 +22,15 @@
     windowWidth: Integer[Literal[True]]
     windowHeight: Integer[Literal[True]]
     tabRatio: Integer[Literal[True]]
     firstSheet: Integer[Literal[True]]
     activeTab: Integer[Literal[True]]
     autoFilterDateGrouping: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         visibility: _BookViewVilibility | Literal["none"] | None = "visible",
         minimized: _ConvertibleToBool | None = False,
         showHorizontalScroll: _ConvertibleToBool | None = True,
         showVerticalScroll: _ConvertibleToBool | None = True,
         showSheetTabs: _ConvertibleToBool | None = True,
@@ -68,15 +68,15 @@
     tabRatio: Integer[Literal[True]]
     activeSheetId: Integer[Literal[False]]
     showFormulaBar: Bool[Literal[True]]
     showStatusbar: Bool[Literal[True]]
     showComments: NoneSet[_CustomWorkbookViewShowComments]
     showObjects: NoneSet[_CustomWorkbookViewShowObjects]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         name: str,
         guid: Incomplete | None = None,
         autoUpdate: _ConvertibleToBool | None = None,
         mergeInterval: _ConvertibleToInt | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/web.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/web.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 _WebPublishingTargetScreenSize: TypeAlias = Literal[
     "544x376",
@@ -50,15 +50,15 @@
     ) -> None: ...
 
 class WebPublishObjectList(Serialisable):
     tagname: str
     # Overwritten by property below
     # count: Integer
     webPublishObject: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, webPublishObject=()) -> None: ...
     @property
     def count(self): ...
 
 class WebPublishing(Serialisable):
     tagname: str
     css: Bool[Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/workbook/workbook.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_read_only.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_reader.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_reader.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_write_only.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_write_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/_writer.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/cell_range.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/cell_range.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/controls.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/header_footer.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors import Strict
+from openpyxl.descriptors.base import Alias, Bool, Integer, MatchPattern, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.ole import ObjectAnchor
 
-class ControlProperty(Serialisable):
-    tagname: str
-    anchor: Typed[ObjectAnchor, Literal[False]]
-    locked: Bool[Literal[True]]
-    defaultSize: Bool[Literal[True]]
-    _print: Bool[Literal[True]]  # Not private. Avoids name clash
-    disabled: Bool[Literal[True]]
-    recalcAlways: Bool[Literal[True]]
-    uiObject: Bool[Literal[True]]
-    autoFill: Bool[Literal[True]]
-    autoLine: Bool[Literal[True]]
-    autoPict: Bool[Literal[True]]
-    macro: String[Literal[True]]
-    altText: String[Literal[True]]
-    linkedCell: String[Literal[True]]
-    listFillRange: String[Literal[True]]
-    cf: String[Literal[True]]
-    id: Incomplete
-    __elements__: Incomplete
+FONT_PATTERN: str
+COLOR_PATTERN: str
+SIZE_REGEX: str
+FORMAT_REGEX: Incomplete
+
+class _HeaderFooterPart(Strict):
+    text: String[Literal[True]]
+    font: String[Literal[True]]
+    size: Integer[Literal[True]]
+    RGB: str
+    color: MatchPattern[str, Literal[True]]
     def __init__(
-        self,
-        anchor: ObjectAnchor,
-        locked: _ConvertibleToBool | None = True,
-        defaultSize: _ConvertibleToBool | None = True,
-        _print: _ConvertibleToBool | None = True,
-        disabled: _ConvertibleToBool | None = False,
-        recalcAlways: _ConvertibleToBool | None = False,
-        uiObject: _ConvertibleToBool | None = False,
-        autoFill: _ConvertibleToBool | None = True,
-        autoLine: _ConvertibleToBool | None = True,
-        autoPict: _ConvertibleToBool | None = True,
-        macro: str | None = None,
-        altText: str | None = None,
-        linkedCell: str | None = None,
-        listFillRange: str | None = None,
-        cf: str | None = "pict",
-        id: Incomplete | None = None,
+        self, text: str | None = None, font: str | None = None, size: _ConvertibleToInt | None = None, color: str | None = None
     ) -> None: ...
+    def __bool__(self) -> bool: ...
+    @classmethod
+    def from_str(cls, text): ...
 
-class Control(Serialisable):
-    tagname: str
-    controlPr: Typed[ControlProperty, Literal[True]]
-    shapeId: Integer[Literal[False]]
-    name: String[Literal[True]]
-    __elements__: Incomplete
-    @overload
+class HeaderFooterItem(Strict):
+    left: Typed[_HeaderFooterPart, Literal[False]]
+    center: Typed[_HeaderFooterPart, Literal[False]]
+    centre: Alias
+    right: Typed[_HeaderFooterPart, Literal[False]]
     def __init__(
-        self, controlPr: ControlProperty | None = None, *, shapeId: _ConvertibleToInt, name: str | None = None
+        self,
+        left: _HeaderFooterPart | None = None,
+        right: _HeaderFooterPart | None = None,
+        center: _HeaderFooterPart | None = None,
     ) -> None: ...
-    @overload
-    def __init__(self, controlPr: ControlProperty | None, shapeId: _ConvertibleToInt, name: str | None = None) -> None: ...
+    def __bool__(self) -> bool: ...
+    def to_tree(self, tagname): ...
+    @classmethod
+    def from_tree(cls, node): ...
 
-class Controls(Serialisable):
+class HeaderFooter(Serialisable):
     tagname: str
-    control: Incomplete
-    __elements__: Incomplete
-    def __init__(self, control=()) -> None: ...
+    differentOddEven: Bool[Literal[True]]
+    differentFirst: Bool[Literal[True]]
+    scaleWithDoc: Bool[Literal[True]]
+    alignWithMargins: Bool[Literal[True]]
+    oddHeader: Typed[HeaderFooterItem, Literal[True]]
+    oddFooter: Typed[HeaderFooterItem, Literal[True]]
+    evenHeader: Typed[HeaderFooterItem, Literal[True]]
+    evenFooter: Typed[HeaderFooterItem, Literal[True]]
+    firstHeader: Typed[HeaderFooterItem, Literal[True]]
+    firstFooter: Typed[HeaderFooterItem, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
+        self,
+        differentOddEven: _ConvertibleToBool | None = None,
+        differentFirst: _ConvertibleToBool | None = None,
+        scaleWithDoc: _ConvertibleToBool | None = None,
+        alignWithMargins: _ConvertibleToBool | None = None,
+        oddHeader: HeaderFooterItem | None = None,
+        oddFooter: HeaderFooterItem | None = None,
+        evenHeader: HeaderFooterItem | None = None,
+        evenFooter: HeaderFooterItem | None = None,
+        firstHeader: HeaderFooterItem | None = None,
+        firstFooter: HeaderFooterItem | None = None,
+    ) -> None: ...
+    def __bool__(self) -> bool: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/datavalidation.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/datavalidation.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     Convertible,
     Integer,
@@ -83,16 +84,16 @@
 
 class DataValidationList(Serialisable):
     tagname: str
     disablePrompts: Bool[Literal[True]]
     xWindow: Integer[Literal[True]]
     yWindow: Integer[Literal[True]]
     dataValidation: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         disablePrompts: _ConvertibleToBool | None = None,
         xWindow: _ConvertibleToInt | None = None,
         yWindow: _ConvertibleToInt | None = None,
         count: Incomplete | None = None,
         dataValidation=(),
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/dimensions.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/dimensions.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/errors.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/errors.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Extension(Serialisable):
     tagname: str
     uri: String[Literal[True]]
     def __init__(self, uri: str | None = None) -> None: ...
 
 class ExtensionList(Serialisable):
     tagname: str
     ext: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, ext=()) -> None: ...
 
 class IgnoredError(Serialisable):
     tagname: str
     sqref: Incomplete
     evalError: Bool[Literal[True]]
     twoDigitTextYear: Bool[Literal[True]]
@@ -41,9 +42,9 @@
         calculatedColumn: _ConvertibleToBool | None = False,
     ) -> None: ...
 
 class IgnoredErrors(Serialisable):
     tagname: str
     ignoredError: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, ignoredError=(), extLst: ExtensionList | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/filters.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/filters.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from _typeshed import Incomplete, Unused
 from datetime import datetime
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     DateTime,
     Float,
@@ -123,15 +123,15 @@
     tagname: str
     columnSort: Bool[Literal[True]]
     caseSensitive: Bool[Literal[True]]
     sortMethod: NoneSet[_SortStateSortMethod]
     ref: Incomplete
     sortCondition: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         columnSort: _ConvertibleToBool | None = None,
         caseSensitive: _ConvertibleToBool | None = None,
         sortMethod: _SortStateSortMethod | Literal["none"] | None = None,
         ref: Incomplete | None = None,
         sortCondition=(),
@@ -175,15 +175,15 @@
         self, operator: _CustomFilterOperator | Literal["none"] | None = None, val: Incomplete | None = None
     ) -> None: ...
 
 class CustomFilters(Serialisable):
     tagname: str
     _and: Bool[Literal[True]]  # Not private. Avoids name clash
     customFilter: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, _and: _ConvertibleToBool | None = False, customFilter=()) -> None: ...
 
 class Top10(Serialisable):
     tagname: str
     top: Bool[Literal[True]]
     percent: Bool[Literal[True]]
     val: Float[Literal[False]]
@@ -241,15 +241,15 @@
 
 class Filters(Serialisable):
     tagname: str
     blank: Bool[Literal[True]]
     calendarType: NoneSet[_FiltersCalendarType]
     filter: Incomplete
     dateGroupItem: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         blank: _ConvertibleToBool | None = None,
         calendarType: _FiltersCalendarType | Literal["none"] | None = None,
         filter=(),
         dateGroupItem=(),
     ) -> None: ...
@@ -263,15 +263,15 @@
     filters: Typed[Filters, Literal[True]]
     top10: Typed[Top10, Literal[True]]
     customFilters: Typed[CustomFilters, Literal[True]]
     dynamicFilter: Typed[DynamicFilter, Literal[True]]
     colorFilter: Typed[ColorFilter, Literal[True]]
     iconFilter: Typed[IconFilter, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         colId: _ConvertibleToInt,
         hiddenButton: _ConvertibleToBool | None = False,
         showButton: _ConvertibleToBool | None = True,
         filters: Filters | None = None,
         top10: Top10 | None = None,
@@ -286,14 +286,14 @@
 
 class AutoFilter(Serialisable):
     tagname: str
     ref: Incomplete
     filterColumn: Incomplete
     sortState: Typed[SortState, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, ref: Incomplete | None = None, filterColumn=(), sortState: SortState | None = None, extLst: Unused = None
     ) -> None: ...
     def __bool__(self) -> bool: ...
     def add_filter_column(self, col_id, vals, blank: bool = False) -> None: ...
     def add_sort_condition(self, ref, descending: bool = False) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/formula.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/formula.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/hyperlink.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/hyperlink.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import String
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Hyperlink(Serialisable):
     tagname: str
     ref: String[Literal[False]]
     location: String[Literal[True]]
     tooltip: String[Literal[True]]
     display: String[Literal[True]]
     id: Incomplete
     target: String[Literal[True]]
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         ref: str,
         location: str | None = None,
         tooltip: str | None = None,
         display: str | None = None,
         id: Incomplete | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/ole.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/ole.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Bool, Integer, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.spreadsheet_drawing import AnchorMarker
 
 _OleObjectDvAspect: TypeAlias = Literal["DVASPECT_CONTENT", "DVASPECT_ICON"]
@@ -35,15 +35,15 @@
     uiObject: Bool[Literal[True]]
     autoFill: Bool[Literal[True]]
     autoLine: Bool[Literal[True]]
     autoPict: Bool[Literal[True]]
     macro: String[Literal[False]]
     altText: String[Literal[True]]
     dde: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         anchor: ObjectAnchor,
         locked: _ConvertibleToBool | None = None,
         defaultSize: _ConvertibleToBool | None = None,
         _print: _ConvertibleToBool | None = None,
@@ -79,15 +79,15 @@
     objectPr: Typed[ObjectPr, Literal[True]]
     progId: String[Literal[True]]
     dvAspect: Set[_OleObjectDvAspect]
     link: String[Literal[True]]
     oleUpdate: Set[_OleObjectOleUpdate]
     autoLoad: Bool[Literal[True]]
     shapeId: Integer[Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         objectPr: ObjectPr | None = None,
         progId: str | None = None,
         dvAspect: _OleObjectDvAspect = "DVASPECT_CONTENT",
         link: str | None = None,
@@ -107,9 +107,9 @@
         autoLoad: _ConvertibleToBool | None,
         shapeId: _ConvertibleToInt,
     ) -> None: ...
 
 class OleObjects(Serialisable):
     tagname: str
     oleObject: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, oleObject=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/page.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/page.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/pagebreak.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/pagebreak.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, Integer, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Break(Serialisable):
     tagname: str
@@ -22,16 +23,16 @@
 
 class RowBreak(Serialisable):
     tagname: str
     # Overwritten by properties below
     # count: Integer
     # manualBreakCount: Integer
     brk: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, manualBreakCount: Unused = None, brk=()) -> None: ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int: ...
     @property
     def count(self): ...
     @property
     def manualBreakCount(self): ...
@@ -42,8 +43,8 @@
 class ColBreak(RowBreak):
     tagname: str
     @property
     def count(self): ...
     @property
     def manualBreakCount(self): ...
     brk: Incomplete
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/print_settings.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/print_settings.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/properties.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/properties.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Outline(Serialisable):
     tagname: str
@@ -34,15 +35,15 @@
     syncRef: String[Literal[True]]
     syncVertical: Bool[Literal[True]]
     transitionEvaluation: Bool[Literal[True]]
     transitionEntry: Bool[Literal[True]]
     tabColor: Incomplete
     outlinePr: Typed[Outline, Literal[True]]
     pageSetUpPr: Typed[PageSetupProperties, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         codeName: str | None = None,
         enableFormatConditionsCalculation: _ConvertibleToBool | None = None,
         filterMode: _ConvertibleToBool | None = None,
         published: _ConvertibleToBool | None = None,
         syncHorizontal: _ConvertibleToBool | None = None,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/protection.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/protection.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 class _Protected:
     def set_password(self, value: str = "", already_hashed: bool = False) -> None: ...
@@ -30,15 +31,15 @@
     sort: Bool[Literal[False]]
     autoFilter: Bool[Literal[False]]
     pivotTables: Bool[Literal[False]]
     saltValue: Incomplete
     spinCount: Integer[Literal[True]]
     algorithmName: String[Literal[True]]
     hashValue: Incomplete
-    __attrs__: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     password: Incomplete
     def __init__(
         self,
         sheet: _ConvertibleToBool = False,
         objects: _ConvertibleToBool = False,
         scenarios: _ConvertibleToBool = False,
         formatCells: _ConvertibleToBool = True,
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/smart_tag.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/smart_tag.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
 from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
 class CellSmartTagPr(Serialisable):
     tagname: str
@@ -13,15 +13,15 @@
 
 class CellSmartTag(Serialisable):
     tagname: str
     cellSmartTagPr: Incomplete
     type: Integer[Literal[False]]
     deleted: Bool[Literal[True]]
     xmlBased: Bool[Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         cellSmartTagPr=(),
         *,
         type: _ConvertibleToInt,
         deleted: _ConvertibleToBool | None = False,
@@ -36,15 +36,15 @@
         xmlBased: _ConvertibleToBool | None = False,
     ) -> None: ...
 
 class CellSmartTags(Serialisable):
     tagname: str
     cellSmartTag: Incomplete
     r: String[Literal[False]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cellSmartTag, r: str) -> None: ...
 
 class SmartTags(Serialisable):
     tagname: str
     cellSmartTags: Incomplete
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cellSmartTags=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/table.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/table.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete, Unused
-from typing import overload
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors import Strict, String
 from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.filters import AutoFilter, SortState
@@ -35,15 +35,15 @@
 class XMLColumnProps(Serialisable):
     tagname: str
     mapId: Integer[Literal[False]]
     xpath: String[Literal[False]]
     denormalized: Bool[Literal[True]]
     xmlDataType: String[Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         mapId: _ConvertibleToInt,
         xpath: str,
         denormalized: _ConvertibleToBool | None = None,
         *,
@@ -81,15 +81,15 @@
     headerRowCellStyle: String[Literal[True]]
     dataCellStyle: String[Literal[True]]
     totalsRowCellStyle: String[Literal[True]]
     calculatedColumnFormula: Typed[TableFormula, Literal[True]]
     totalsRowFormula: Typed[TableFormula, Literal[True]]
     xmlColumnPr: Typed[XMLColumnProps, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         id: _ConvertibleToInt,
         uniqueName: str | None = None,
         *,
         name: str,
@@ -160,15 +160,15 @@
     totalsRowCellStyle: String[Literal[True]]
     connectionId: Integer[Literal[True]]
     autoFilter: Typed[AutoFilter, Literal[True]]
     sortState: Typed[SortState, Literal[True]]
     tableColumns: Incomplete
     tableStyleInfo: Typed[TableStyleInfo, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         id: _ConvertibleToInt = 1,
         displayName: Incomplete | None = None,
         ref: Incomplete | None = None,
         name: str | None = None,
         comment: str | None = None,
@@ -202,16 +202,16 @@
     def column_names(self): ...
 
 class TablePartList(Serialisable):
     tagname: str
     # Overwritten by property below
     # count: Integer
     tablePart: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, tablePart=()) -> None: ...
     def append(self, part) -> None: ...
     @property
     def count(self): ...
     def __bool__(self) -> bool: ...
 
 class TableList(dict[Incomplete, Incomplete]):
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/views.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/views.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, Unused
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Bool,
     Float,
     Integer,
     NoneSet,
@@ -98,9 +99,9 @@
         pane: Pane | None = None,
     ) -> None: ...
 
 class SheetViewList(Serialisable):
     tagname: str
     sheetView: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, sheetView: Incomplete | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/worksheet/worksheet.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/worksheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/openpyxl-stubs/xml/constants.pyi` & `types-openpyxl-3.1.0.8/openpyxl-stubs/xml/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.7/setup.py` & `types-openpyxl-3.1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `2d5dafadb75f122e0c2aeced09a5b72232373f40`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.1.0.7",
+      version="3.1.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md",
```

### Comparing `types-openpyxl-3.1.0.7/types_openpyxl.egg-info/PKG-INFO` & `types-openpyxl-3.1.0.8/types_openpyxl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.7
+Version: 3.1.0.8
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `2d5dafadb75f122e0c2aeced09a5b72232373f40`.
```

### Comparing `types-openpyxl-3.1.0.7/types_openpyxl.egg-info/SOURCES.txt` & `types-openpyxl-3.1.0.8/types_openpyxl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

