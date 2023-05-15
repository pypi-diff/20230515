# Comparing `tmp/risingwave-0.0.5.tar.gz` & `tmp/risingwave-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risingwave-0.0.5.tar", last modified: Wed Apr 12 11:25:21 2023, max compression
+gzip compressed data, was "risingwave-0.0.6.tar", last modified: Mon May 15 09:47:01 2023, max compression
```

## Comparing `risingwave-0.0.5.tar` & `risingwave-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-12 11:25:21.415539 risingwave-0.0.5/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-04-12 11:25:21.415375 risingwave-0.0.5/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.5/README.md
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-12 11:25:21.412151 risingwave-0.0.5/risingwave/
--rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.5/risingwave/__init__.py
--rw-r--r--   0 wangrunji   (501) staff       (20)    10275 2023-04-12 11:24:37.000000 risingwave-0.0.5/risingwave/udf.py
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-12 11:25:21.415120 risingwave-0.0.5/risingwave.egg-info/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)      228 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        8 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/requires.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/top_level.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-04-12 11:25:21.415583 risingwave-0.0.5/setup.cfg
--rw-r--r--   0 wangrunji   (501) staff       (20)      605 2023-04-12 11:25:01.000000 risingwave-0.0.5/setup.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-15 09:47:01.778306 risingwave-0.0.6/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-05-15 09:47:01.778167 risingwave-0.0.6/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.6/README.md
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-15 09:47:01.777324 risingwave-0.0.6/risingwave/
+-rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.6/risingwave/__init__.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)    11869 2023-05-15 09:45:39.000000 risingwave-0.0.6/risingwave/udf.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-15 09:47:01.777966 risingwave-0.0.6/risingwave.egg-info/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)      228 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        8 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/requires.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/top_level.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-05-15 09:47:01.778342 risingwave-0.0.6/setup.cfg
+-rw-r--r--   0 wangrunji   (501) staff       (20)      606 2023-05-15 09:45:39.000000 risingwave-0.0.6/setup.py
```

### Comparing `risingwave-0.0.5/PKG-INFO` & `risingwave-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.5
+Version: 0.0.6
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `risingwave-0.0.5/README.md` & `risingwave-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `risingwave-0.0.5/risingwave/udf.py` & `risingwave-0.0.6/risingwave/udf.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,136 +7,177 @@
 import json
 
 
 class UserDefinedFunction:
     """
     Base interface for user-defined function.
     """
+
     _name: str
     _input_schema: pa.Schema
     _result_schema: pa.Schema
 
-    def eval_batch(self, batch: pa.RecordBatch) -> pa.RecordBatch:
+    def eval_batch(self, batch: pa.RecordBatch) -> Iterator[pa.RecordBatch]:
         """
         Apply the function on a batch of inputs.
         """
-        pass
+        return iter([])
 
 
 class ScalarFunction(UserDefinedFunction):
     """
     Base interface for user-defined scalar function. A user-defined scalar functions maps zero, one,
     or multiple scalar values to a new scalar value.
     """
 
     def eval(self, *args) -> Any:
         """
         Method which defines the logic of the scalar function.
         """
         pass
 
-    def eval_batch(self, batch: pa.RecordBatch) -> pa.RecordBatch:
+    def eval_batch(self, batch: pa.RecordBatch) -> Iterator[pa.RecordBatch]:
         # parse value from json string for jsonb columns
         inputs = [[v.as_py() for v in array] for array in batch]
         inputs = [
             _process_input_array(array, type)
-            for array, type in zip(inputs, self._input_schema.types)]
+            for array, type in zip(inputs, self._input_schema.types)
+        ]
 
         # evaluate the function for each row
-        column = [self.eval(*[col[i] for col in inputs])
-                  for i in range(batch.num_rows)]
+        column = [self.eval(*[col[i] for col in inputs]) for i in range(batch.num_rows)]
 
         # convert value to json for jsonb columns
         if self._result_schema.types[0] == pa.large_string():
-            column = [(json.dumps(v) if v is not None else None)
-                      for v in column]
+            column = [(json.dumps(v) if v is not None else None) for v in column]
         array = pa.array(column, type=self._result_schema.types[0])
-        return pa.RecordBatch.from_arrays([array], schema=self._result_schema)
+        yield pa.RecordBatch.from_arrays([array], schema=self._result_schema)
 
 
 def _process_input_array(array: list, type: pa.DataType) -> list:
     if pa.types.is_list(type):
-        return [(_process_input_array(v, type.value_type)
-                if v is not None else None)
-                for v in array]
+        return [
+            (_process_input_array(v, type.value_type) if v is not None else None)
+            for v in array
+        ]
     if pa.types.is_large_string(type):
-        return [(json.loads(v) if v is not None else None)
-                for v in array]
+        return [(json.loads(v) if v is not None else None) for v in array]
     return array
 
 
 class TableFunction(UserDefinedFunction):
     """
     Base interface for user-defined table function. A user-defined table functions maps zero, one,
-    or multiple table values to a new table value.
+    or multiple scalar values to a new table value.
     """
 
+    BATCH_SIZE = 1024
+
     def eval(self, *args) -> Iterator:
         """
         Method which defines the logic of the table function.
         """
         yield
 
-    def eval_batch(self, batch: pa.RecordBatch) -> pa.RecordBatch:
-        result_rows = []
+    def eval_batch(self, batch: pa.RecordBatch) -> Iterator[pa.RecordBatch]:
+        class RecordBatchBuilder:
+            """A utility class for constructing Arrow RecordBatch by row."""
+
+            schema: pa.Schema
+            columns: List[List]
+
+            def __init__(self, schema: pa.Schema):
+                self.schema = schema
+                self.columns = [[] for _ in self.schema.types]
+
+            def len(self) -> int:
+                """Returns the number of rows in the RecordBatch being built."""
+                return len(self.columns[0])
+
+            def append(self, index: int, args: Tuple):
+                """Appends a new row to the RecordBatch being built."""
+                self.columns[0].append(index)
+                for column, val in zip(self.columns[1:], args):
+                    column.append(val)
+
+            def build(self) -> pa.RecordBatch:
+                """Builds the RecordBatch from the accumulated data and clears the state."""
+                # Convert the columns to arrow arrays
+                arrays = [
+                    pa.array(col, type)
+                    for col, type in zip(self.columns, self.schema.types)
+                ]
+                # Reset columns
+                self.columns = [[] for _ in self.schema.types]
+                return pa.RecordBatch.from_arrays(arrays, schema=self.schema)
+
+        builder = RecordBatchBuilder(self._result_schema)
+
         # Iterate through rows in the input RecordBatch
         for row_index in range(batch.num_rows):
             row = tuple(column[row_index].as_py() for column in batch)
-            result_rows.extend(self.eval(*row))
-
-        result_columns = zip(
-            *result_rows) if len(self._result_schema) > 1 else [result_rows]
-
-        # Convert the result columns to arrow arrays
-        arrays = [
-            pa.array(col, type) for col, type in zip(result_columns, self._result_schema.types)
-        ]
-        return pa.RecordBatch.from_arrays(arrays, schema=self._result_schema)
+            for result_row in self.eval(*row):
+                if not isinstance(result_row, tuple):
+                    result_row = (result_row,)
+                builder.append(row_index, result_row)
+                if builder.len() == self.BATCH_SIZE:
+                    yield builder.build()
+        if builder.len() != 0:
+            yield builder.build()
 
 
 class UserDefinedScalarFunctionWrapper(ScalarFunction):
     """
     Base Wrapper for Python user-defined scalar function.
     """
+
     _func: Callable
 
     def __init__(self, func, input_types, result_type, name=None):
         self._func = func
-        self._input_schema = pa.schema(zip(
-            inspect.getfullargspec(func)[0],
-            [_to_data_type(t) for t in _to_list(input_types)]
-        ))
-        self._result_schema = pa.schema(
-            [('output', _to_data_type(result_type))])
+        self._input_schema = pa.schema(
+            zip(
+                inspect.getfullargspec(func)[0],
+                [_to_data_type(t) for t in _to_list(input_types)],
+            )
+        )
+        self._result_schema = pa.schema([("output", _to_data_type(result_type))])
         self._name = name or (
-            func.__name__ if hasattr(func, '__name__') else func.__class__.__name__)
+            func.__name__ if hasattr(func, "__name__") else func.__class__.__name__
+        )
 
     def __call__(self, *args):
         return self._func(*args)
 
     def eval(self, *args):
         return self._func(*args)
 
 
 class UserDefinedTableFunctionWrapper(TableFunction):
     """
     Base Wrapper for Python user-defined table function.
     """
+
     _func: Callable
 
     def __init__(self, func, input_types, result_types, name=None):
         self._func = func
-        self._input_schema = pa.schema(zip(
-            inspect.getfullargspec(func)[0],
-            [_to_data_type(t) for t in _to_list(input_types)]
-        ))
+        self._input_schema = pa.schema(
+            zip(
+                inspect.getfullargspec(func)[0],
+                [_to_data_type(t) for t in _to_list(input_types)],
+            )
+        )
         self._result_schema = pa.schema(
-            [('', _to_data_type(t)) for t in _to_list(result_types)])
+            [("row_index", pa.int64())]
+            + [("", _to_data_type(t)) for t in _to_list(result_types)]
+        )
         self._name = name or (
-            func.__name__ if hasattr(func, '__name__') else func.__class__.__name__)
+            func.__name__ if hasattr(func, "__name__") else func.__class__.__name__
+        )
 
     def __call__(self, *args):
         return self._func(*args)
 
     def eval(self, *args):
         return self._func(*args)
 
@@ -144,17 +185,19 @@
 def _to_list(x):
     if isinstance(x, list):
         return x
     else:
         return [x]
 
 
-def udf(input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
-        result_type: Union[str, pa.DataType],
-        name: Optional[str] = None,) -> Callable:
+def udf(
+    input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
+    result_type: Union[str, pa.DataType],
+    name: Optional[str] = None,
+) -> Callable:
     """
     Annotation for creating a user-defined scalar function.
 
     Parameters:
     - input_types: A list of strings or Arrow data types that specifies the input data types.
     - result_type: A string or an Arrow data type that specifies the return value type.
     - name: An optional string specifying the function name. If not provided, the original name will be used.
@@ -168,17 +211,19 @@
         return x
     ```
     """
 
     return lambda f: UserDefinedScalarFunctionWrapper(f, input_types, result_type, name)
 
 
-def udtf(input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
-         result_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
-         name: Optional[str] = None,) -> Callable:
+def udtf(
+    input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
+    result_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
+    name: Optional[str] = None,
+) -> Callable:
     """
     Annotation for creating a user-defined table function.
 
     Parameters:
     - input_types: A list of strings or Arrow data types that specifies the input data types.
     - result_types A list of strings or Arrow data types that specifies the return value types.
     - name: An optional string specifying the function name. If not provided, the original name will be used.
@@ -202,55 +247,64 @@
     Example:
     ```
     server = UdfServer(location="0.0.0.0:8815")
     server.add_function(my_udf)
     server.serve()
     ```
     """
+
     # UDF server based on Apache Arrow Flight protocol.
     # Reference: https://arrow.apache.org/cookbook/py/flight.html#simple-parquet-storage-service-with-arrow-flight
 
+    _location: str
     _functions: Dict[str, UserDefinedFunction]
 
     def __init__(self, location="0.0.0.0:8815", **kwargs):
-        super(UdfServer, self).__init__('grpc://' + location, **kwargs)
+        super(UdfServer, self).__init__("grpc://" + location, **kwargs)
+        self._location = location
         self._functions = {}
 
     def get_flight_info(self, context, descriptor):
         """Return the result schema of a function."""
-        udf = self._functions[descriptor.path[0].decode('utf-8')]
+        udf = self._functions[descriptor.path[0].decode("utf-8")]
         # return the concatenation of input and output schema
-        full_schema = pa.schema(
-            list(udf._input_schema) + list(udf._result_schema))
+        full_schema = pa.schema(list(udf._input_schema) + list(udf._result_schema))
         # we use `total_records` to indicate the number of input arguments
-        return pa.flight.FlightInfo(schema=full_schema, descriptor=descriptor, endpoints=[], total_records=len(udf._input_schema), total_bytes=0)
+        return pa.flight.FlightInfo(
+            schema=full_schema,
+            descriptor=descriptor,
+            endpoints=[],
+            total_records=len(udf._input_schema),
+            total_bytes=0,
+        )
 
     def add_function(self, udf: UserDefinedFunction):
         """Add a function to the server."""
         name = udf._name
         if name in self._functions:
-            raise ValueError('Function already exists: ' + name)
-        print('added function:', name)
+            raise ValueError("Function already exists: " + name)
+        print("added function:", name)
         self._functions[name] = udf
 
     def do_exchange(self, context, descriptor, reader, writer):
         """Call a function from the client."""
-        udf = self._functions[descriptor.path[0].decode('utf-8')]
+        udf = self._functions[descriptor.path[0].decode("utf-8")]
         writer.begin(udf._result_schema)
-        for chunk in reader:
-            # print(pa.Table.from_batches([chunk.data]))
-            try:
-                result = udf.eval_batch(chunk.data)
-            except Exception as e:
-                print(traceback.print_exc())
-                raise e
-            writer.write_batch(result)
+        try:
+            for batch in reader:
+                # print(pa.Table.from_batches([batch.data]))
+                for output_batch in udf.eval_batch(batch.data):
+                    writer.write_batch(output_batch)
+        except Exception as e:
+            print(traceback.print_exc())
+            raise e
 
     def serve(self):
         """Start the server."""
+        print(f"listening on {self._location}")
         super(UdfServer, self).serve()
 
 
 def _to_data_type(t: Union[str, pa.DataType]) -> pa.DataType:
     """
     Convert a string or pyarrow.DataType to pyarrow.DataType.
     """
@@ -258,47 +312,47 @@
         return _string_to_data_type(t)
     else:
         return t
 
 
 def _string_to_data_type(type_str: str):
     type_str = type_str.upper()
-    if type_str in ('BOOLEAN', 'BOOL'):
+    if type_str in ("BOOLEAN", "BOOL"):
         return pa.bool_()
-    elif type_str in ('SMALLINT', 'INT2'):
+    elif type_str in ("SMALLINT", "INT2"):
         return pa.int16()
-    elif type_str in ('INT', 'INTEGER', 'INT4'):
+    elif type_str in ("INT", "INTEGER", "INT4"):
         return pa.int32()
-    elif type_str in ('BIGINT', 'INT8'):
+    elif type_str in ("BIGINT", "INT8"):
         return pa.int64()
-    elif type_str in ('FLOAT4', 'REAL'):
+    elif type_str in ("FLOAT4", "REAL"):
         return pa.float32()
-    elif type_str in ('FLOAT8', 'DOUBLE PRECISION'):
+    elif type_str in ("FLOAT8", "DOUBLE PRECISION"):
         return pa.float64()
-    elif type_str.startswith('DECIMAL') or type_str.startswith('NUMERIC'):
+    elif type_str.startswith("DECIMAL") or type_str.startswith("NUMERIC"):
         return pa.decimal128(28)
-    elif type_str in ('DATE'):
+    elif type_str in ("DATE"):
         return pa.date32()
-    elif type_str in ('TIME', 'TIME WITHOUT TIME ZONE'):
-        return pa.time32('ms')
-    elif type_str in ('TIMESTAMP', 'TIMESTAMP WITHOUT TIME ZONE'):
-        return pa.timestamp('ms')
-    elif type_str.startswith('INTERVAL'):
-        return pa.duration('us')
-    elif type_str in ('VARCHAR'):
+    elif type_str in ("TIME", "TIME WITHOUT TIME ZONE"):
+        return pa.time32("ms")
+    elif type_str in ("TIMESTAMP", "TIMESTAMP WITHOUT TIME ZONE"):
+        return pa.timestamp("ms")
+    elif type_str.startswith("INTERVAL"):
+        return pa.duration("us")
+    elif type_str in ("VARCHAR"):
         return pa.string()
-    elif type_str in ('JSONB'):
+    elif type_str in ("JSONB"):
         return pa.large_string()
-    elif type_str in ('BYTEA'):
+    elif type_str in ("BYTEA"):
         return pa.binary()
-    elif type_str.endswith('[]'):
+    elif type_str.endswith("[]"):
         return pa.list_(_string_to_data_type(type_str[:-2]))
-    elif type_str.startswith('STRUCT'):
+    elif type_str.startswith("STRUCT"):
         # extract 'STRUCT<INT, VARCHAR, ...>'
-        type_list = type_str[6:].strip('<>')
+        type_list = type_str[6:].strip("<>")
         fields = []
-        for type_str in type_list.split(','):
+        for type_str in type_list.split(","):
             type_str = type_str.strip()
-            fields.append(pa.field('', _string_to_data_type(type_str)))
+            fields.append(pa.field("", _string_to_data_type(type_str)))
         return pa.struct(fields)
 
-    raise ValueError(f'Unsupported type: {type_str}')
+    raise ValueError(f"Unsupported type: {type_str}")
```

### Comparing `risingwave-0.0.5/risingwave.egg-info/PKG-INFO` & `risingwave-0.0.6/risingwave.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.5
+Version: 0.0.6
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `risingwave-0.0.5/setup.py` & `risingwave-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="risingwave",
-    version="0.0.5",
+    version="0.0.6",
     author="RisingWave Labs",
     description="RisingWave Python API",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     url="https://github.com/risingwavelabs/risingwave",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
-        "License :: OSI Approved :: Apache Software License"
+        "License :: OSI Approved :: Apache Software License",
     ],
     python_requires=">=3.8",
-    install_requires=['pyarrow'],
+    install_requires=["pyarrow"],
 )
```

