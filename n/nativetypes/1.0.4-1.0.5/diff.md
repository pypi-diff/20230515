# Comparing `tmp/nativetypes-1.0.4-py2.py3-none-any.whl.zip` & `tmp/nativetypes-1.0.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6623 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      466 b- defN 17-Jun-10 21:40 nativetypes/__init__.py
--rw-rw-rw-  2.0 fat     7994 b- defN 17-Jun-25 17:44 nativetypes/native_float.py
--rw-rw-rw-  2.0 fat     9226 b- defN 20-May-14 08:01 nativetypes/native_int.py
--rw-rw-rw-  2.0 fat     1100 b- defN 20-May-14 08:08 nativetypes-1.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1108 b- defN 20-May-14 08:08 nativetypes-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 20-May-14 08:08 nativetypes-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 20-May-14 08:08 nativetypes-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      652 b- defN 20-May-14 08:08 nativetypes-1.0.4.dist-info/RECORD
-8 files, 20674 bytes uncompressed, 5485 bytes compressed:  73.5%
+Zip file size: 6579 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      447 b- defN 23-May-15 16:58 nativetypes/__init__.py
+-rw-rw-r--  2.0 unx     7762 b- defN 23-May-15 16:58 nativetypes/native_float.py
+-rw-rw-r--  2.0 unx     9019 b- defN 23-May-15 17:04 nativetypes/native_int.py
+-rw-rw-r--  2.0 unx     1079 b- defN 23-May-15 17:12 nativetypes-1.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1138 b- defN 23-May-15 17:12 nativetypes-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-15 17:12 nativetypes-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-15 17:12 nativetypes-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      652 b- defN 23-May-15 17:12 nativetypes-1.0.5.dist-info/RECORD
+8 files, 20219 bytes uncompressed, 5441 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: nativetypes/native_float.py
 Comment: 
 
 Filename: nativetypes/native_int.py
 Comment: 
 
-Filename: nativetypes-1.0.4.dist-info/LICENSE
+Filename: nativetypes-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: nativetypes-1.0.4.dist-info/METADATA
+Filename: nativetypes-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: nativetypes-1.0.4.dist-info/WHEEL
+Filename: nativetypes-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: nativetypes-1.0.4.dist-info/top_level.txt
+Filename: nativetypes-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: nativetypes-1.0.4.dist-info/RECORD
+Filename: nativetypes-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nativetypes/__init__.py

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Native types.
-"""
-
-# Imports
-from .native_int import *
-from .native_float import *
-
-# Prevent polluting namespace
-del native_int
-del native_float
-
-def reinterpret_cast(dst, src):
-    assert (isinstance(dst(), nint) or isinstance(dst(), nfloat)) and \
-           (isinstance(src, nint) or isinstance(src, nfloat))
-    byteorder = 'big'
-    return dst.from_bytes(src.to_bytes(byteorder), byteorder)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+Native types.
+"""
+
+# Imports
+from .native_int import *
+from .native_float import *
+
+# Prevent polluting namespace
+del native_int
+del native_float
+
+def reinterpret_cast(dst, src):
+    assert (isinstance(dst(), nint) or isinstance(dst(), nfloat)) and \
+           (isinstance(src, nint) or isinstance(src, nfloat))
+    byteorder = 'big'
+    return dst.from_bytes(src.to_bytes(byteorder), byteorder)
```

## nativetypes/native_float.py

 * *Ordering differences only*

```diff
@@ -1,232 +1,232 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Native types.
-"""
-
-import operator
-import struct
-
-from .native_int import *
-
-# Helpers
-def ensure_native(lhs, rhs):
-    assert isinstance(lhs, nfloat) or isinstance(rhs, nfloat)
-    if not isinstance(lhs, nfloat):
-        lhs = nfloat(lhs, rhs.e, rhs.m)
-    if not isinstance(rhs, nfloat):
-        rhs = nfloat(rhs, lhs.e, lhs.m)
-    return lhs, rhs
-
-# Promotions
-def promote_exponent(lhs, rhs):
-    return max(lhs.e, rhs.e)
-def promote_mantissa(lhs, rhs):
-    return max(lhs.m, rhs.m)
-
-# Operators
-def op_unary(value, op):
-    exponent = value.e
-    mantissa = value.m
-    result = op(float(value))
-    return nfloat(result, exponent, mantissa)
-
-def op_binary(lhs, rhs, op):
-    lhs, rhs = ensure_native(lhs, rhs)
-    exponent = promote_exponent(lhs, rhs)
-    mantissa = promote_mantissa(lhs, rhs)
-    result = op(float(lhs), float(rhs))
-    return nfloat(result, exponent, mantissa)
-
-def op_relational(lhs, rhs, op):
-    lhs, rhs = ensure_native(lhs, rhs)
-    exponent = promote_exponent(lhs, rhs)
-    mantissa = promote_mantissa(lhs, rhs)
-    return op(float(lhs), float(rhs))
-
-# Native Float
-class nfloat(object):
-    def __init__(self, value=0.0, exponent=8, mantissa=23):
-        assert exponent <= 11, 'Support up to float64 only'
-        assert mantissa <= 52, 'Support up to float64 only'
-        self.e = exponent
-        self.m = mantissa
-        # Value
-        self.vs = nint(bits=1)
-        self.ve = nint(bits=exponent, signed=False)
-        self.vm = nint(bits=mantissa, signed=False)
-        self.set(value)
-
-    # Bytes conversion
-    @staticmethod
-    def from_bytes(data, byteorder, exponent, mantissa):
-        bits = 1 + exponent + mantissa
-        value = int(nint.from_bytes(data, byteorder, bits=bits, signed=False))
-        result = nfloat(0.0, exponent, mantissa)
-        result.vs.set(value >> (mantissa + exponent))
-        result.ve.set(value >> (mantissa))
-        result.vm.set(value)
-        return result
-
-    def to_bytes(self, byteorder):
-        value = 0
-        value |= int(self.vm)
-        value |= int(self.ve) << (self.m)
-        value |= int(self.vs) << (self.m + self.e)
-        bits = 1 + self.e + self.m
-        return nint(value, bits=bits, signed=False).to_bytes(byteorder)
-
-    def set(self, value):
-        assert isinstance(value, float)
-        value = struct.pack('d', value)
-        value = struct.unpack('Q', value)[0]
-        self.vs.set(value >> (63))
-        # Exponent
-        ve = (value >> 52) & 0x7FF
-        if not ve:
-            self.ve.set(0)
-        else:
-            src_bits = 11
-            dst_bits = self.e
-            exp_min = - 2 ** (dst_bits - 1) + 2
-            exp_max = + 2 ** (dst_bits - 1) + 0
-            ve -= (2 ** (src_bits - 1)) - 1
-            ve = min(max(ve, exp_min), exp_max)
-            ve += (2 ** (dst_bits - 1)) - 1
-            self.ve.set(ve)
-        # Mantissa
-        self.vm.set(value >> (52 - self.m))
-        self.vm |= (value >> (51 - min(51, self.m))) & 1
-
-    def __str__(self):
-        return str(float(self))
-    def __repr__(self):
-        typename = type(self).__name__
-        return '%s(%s)' % (typename, self)
-    def __format__(self, format_spec):
-        template = '{{:{}}}'.format(format_spec)
-        return template.format(float(self))
-    def __int__(self):
-        return int(float(self))
-    def __bool__(self):
-        return bool(float(self))
-    def __nonzero__(self):
-        return bool(float(self))
-    def __float__(self):
-        sign = (-1) ** self.vs.v
-        # Non-numbers
-        if self.ve == self.ve.max():
-            if self.vm == 0:
-                return float('inf') * sign
-            return float('nan')
-        denormalized = (self.ve == 0)
-        # Exponent
-        exponent = -(2 ** (self.e - 1)) + 2
-        if not denormalized:
-            exponent += self.ve.v - 1
-        # Mantissa
-        mantissa = 0.0 if denormalized else 1.0
-        for i in range(1, self.m + 1):
-            mantissa += ((self.vm.v >> (self.m - i)) & 1) * (2 ** (-i))
-        # Value
-        value = mantissa * (2 ** exponent)
-        return sign * value
-
-    def op_binary_inplace(self, value, op):
-        result_float = op(float(self), float(value))
-        self.set(result_float)
-        return self
-
-    # Unary operations
-    def __abs__(self):
-        return op_unary(self, operator.__abs__)
-    def __pos__(self):
-        return op_unary(self, operator.__pos__)
-    def __neg__(self):
-        return op_unary(self, operator.__neg__)
-
-    # Binary operations
-    def __add__(self, rhs):
-        return op_binary(self, rhs, operator.__add__)
-    def __sub__(self, rhs):
-        return op_binary(self, rhs, operator.__sub__)
-    def __mul__(self, rhs):
-        return op_binary(self, rhs, operator.__mul__)
-    def __div__(self, rhs):
-        return op_binary(self, rhs, operator.__div__)
-    def __floordiv__(self, rhs):
-        return op_binary(self, rhs, operator.__floordiv__)
-    def __truediv__(self, rhs):
-        return op_binary(self, rhs, operator.__truediv__)
-    def __mod__(self, rhs):
-        return op_binary(self, rhs, operator.__mod__)
-    def __pow__(self, rhs):
-        return op_binary(self, rhs, operator.__pow__)
-
-    # Reflected binary operation
-    def __radd__(self, lhs):
-        return op_binary(lhs, self, operator.__add__)
-    def __rsub__(self, lhs):
-        return op_binary(lhs, self, operator.__sub__)
-    def __rmul__(self, lhs):
-        return op_binary(lhs, self, operator.__mul__)
-    def __rdiv__(self, lhs):
-        return op_binary(lhs, self, operator.__div__)
-    def __rfloordiv__(self, lhs):
-        return op_binary(lhs, self, operator.__floordiv__)
-    def __rtruediv__(self, lhs):
-        return op_binary(lhs, self, operator.__truediv__)
-    def __rmod__(self, lhs):
-        return op_binary(lhs, self, operator.__mod__)
-    def __rpow__(self, lhs):
-        return op_binary(lhs, self, operator.__pow__)
-
-    # In-place operations
-    def __iadd__(self, v):
-        return self.op_binary_inplace(v, operator.__add__)
-    def __isub__(self, v):
-        return self.op_binary_inplace(v, operator.__sub__)
-    def __imul__(self, v):
-        return self.op_binary_inplace(v, operator.__mul__)
-    def __idiv__(self, v):
-        return self.op_binary_inplace(v, operator.__div__)
-    def __ifloordiv__(self, v):
-        return self.op_binary_inplace(v, operator.__floordiv__)
-    def __itruediv__(self, v):
-        return self.op_binary_inplace(v, operator.__truediv__)
-    def __imod__(self, v):
-        return self.op_binary_inplace(v, operator.__mod__)
-    def __ipow__(self, v):
-        return self.op_binary_inplace(v, operator.__pow__)
-
-    # Boolean operations
-    def __eq__(self, rhs):
-        return op_relational(self, rhs, operator.__eq__)
-    def __ne__(self, rhs):
-        return op_relational(self, rhs, operator.__ne__)
-    def __lt__(self, rhs):
-        return op_relational(self, rhs, operator.__lt__)
-    def __le__(self, rhs):
-        return op_relational(self, rhs, operator.__le__)
-    def __ge__(self, rhs):
-        return op_relational(self, rhs, operator.__ge__)
-    def __gt__(self, rhs):
-        return op_relational(self, rhs, operator.__gt__)
-
-
-# Aliases
-def nfloat_type(name, exponent, mantissa):
-    def __init__(self, value=0.0):
-        nfloat.__init__(self, value, exponent, mantissa)
-    @staticmethod
-    def from_bytes(data, byteorder):
-        return nfloat.from_bytes(data, byteorder, exponent, mantissa)
-    return type(name, (nfloat,), {
-        "__init__": __init__,
-        "from_bytes": from_bytes
-    })
-
-# Shorthands
-float16 = nfloat_type('float16', exponent=5,  mantissa=10)
-float32 = nfloat_type('float32', exponent=8,  mantissa=23)
-float64 = nfloat_type('float64', exponent=11, mantissa=52)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+Native types.
+"""
+
+import operator
+import struct
+
+from .native_int import *
+
+# Helpers
+def ensure_native(lhs, rhs):
+    assert isinstance(lhs, nfloat) or isinstance(rhs, nfloat)
+    if not isinstance(lhs, nfloat):
+        lhs = nfloat(lhs, rhs.e, rhs.m)
+    if not isinstance(rhs, nfloat):
+        rhs = nfloat(rhs, lhs.e, lhs.m)
+    return lhs, rhs
+
+# Promotions
+def promote_exponent(lhs, rhs):
+    return max(lhs.e, rhs.e)
+def promote_mantissa(lhs, rhs):
+    return max(lhs.m, rhs.m)
+
+# Operators
+def op_unary(value, op):
+    exponent = value.e
+    mantissa = value.m
+    result = op(float(value))
+    return nfloat(result, exponent, mantissa)
+
+def op_binary(lhs, rhs, op):
+    lhs, rhs = ensure_native(lhs, rhs)
+    exponent = promote_exponent(lhs, rhs)
+    mantissa = promote_mantissa(lhs, rhs)
+    result = op(float(lhs), float(rhs))
+    return nfloat(result, exponent, mantissa)
+
+def op_relational(lhs, rhs, op):
+    lhs, rhs = ensure_native(lhs, rhs)
+    exponent = promote_exponent(lhs, rhs)
+    mantissa = promote_mantissa(lhs, rhs)
+    return op(float(lhs), float(rhs))
+
+# Native Float
+class nfloat(object):
+    def __init__(self, value=0.0, exponent=8, mantissa=23):
+        assert exponent <= 11, 'Support up to float64 only'
+        assert mantissa <= 52, 'Support up to float64 only'
+        self.e = exponent
+        self.m = mantissa
+        # Value
+        self.vs = nint(bits=1)
+        self.ve = nint(bits=exponent, signed=False)
+        self.vm = nint(bits=mantissa, signed=False)
+        self.set(value)
+
+    # Bytes conversion
+    @staticmethod
+    def from_bytes(data, byteorder, exponent, mantissa):
+        bits = 1 + exponent + mantissa
+        value = int(nint.from_bytes(data, byteorder, bits=bits, signed=False))
+        result = nfloat(0.0, exponent, mantissa)
+        result.vs.set(value >> (mantissa + exponent))
+        result.ve.set(value >> (mantissa))
+        result.vm.set(value)
+        return result
+
+    def to_bytes(self, byteorder):
+        value = 0
+        value |= int(self.vm)
+        value |= int(self.ve) << (self.m)
+        value |= int(self.vs) << (self.m + self.e)
+        bits = 1 + self.e + self.m
+        return nint(value, bits=bits, signed=False).to_bytes(byteorder)
+
+    def set(self, value):
+        assert isinstance(value, float)
+        value = struct.pack('d', value)
+        value = struct.unpack('Q', value)[0]
+        self.vs.set(value >> (63))
+        # Exponent
+        ve = (value >> 52) & 0x7FF
+        if not ve:
+            self.ve.set(0)
+        else:
+            src_bits = 11
+            dst_bits = self.e
+            exp_min = - 2 ** (dst_bits - 1) + 2
+            exp_max = + 2 ** (dst_bits - 1) + 0
+            ve -= (2 ** (src_bits - 1)) - 1
+            ve = min(max(ve, exp_min), exp_max)
+            ve += (2 ** (dst_bits - 1)) - 1
+            self.ve.set(ve)
+        # Mantissa
+        self.vm.set(value >> (52 - self.m))
+        self.vm |= (value >> (51 - min(51, self.m))) & 1
+
+    def __str__(self):
+        return str(float(self))
+    def __repr__(self):
+        typename = type(self).__name__
+        return '%s(%s)' % (typename, self)
+    def __format__(self, format_spec):
+        template = '{{:{}}}'.format(format_spec)
+        return template.format(float(self))
+    def __int__(self):
+        return int(float(self))
+    def __bool__(self):
+        return bool(float(self))
+    def __nonzero__(self):
+        return bool(float(self))
+    def __float__(self):
+        sign = (-1) ** self.vs.v
+        # Non-numbers
+        if self.ve == self.ve.max():
+            if self.vm == 0:
+                return float('inf') * sign
+            return float('nan')
+        denormalized = (self.ve == 0)
+        # Exponent
+        exponent = -(2 ** (self.e - 1)) + 2
+        if not denormalized:
+            exponent += self.ve.v - 1
+        # Mantissa
+        mantissa = 0.0 if denormalized else 1.0
+        for i in range(1, self.m + 1):
+            mantissa += ((self.vm.v >> (self.m - i)) & 1) * (2 ** (-i))
+        # Value
+        value = mantissa * (2 ** exponent)
+        return sign * value
+
+    def op_binary_inplace(self, value, op):
+        result_float = op(float(self), float(value))
+        self.set(result_float)
+        return self
+
+    # Unary operations
+    def __abs__(self):
+        return op_unary(self, operator.__abs__)
+    def __pos__(self):
+        return op_unary(self, operator.__pos__)
+    def __neg__(self):
+        return op_unary(self, operator.__neg__)
+
+    # Binary operations
+    def __add__(self, rhs):
+        return op_binary(self, rhs, operator.__add__)
+    def __sub__(self, rhs):
+        return op_binary(self, rhs, operator.__sub__)
+    def __mul__(self, rhs):
+        return op_binary(self, rhs, operator.__mul__)
+    def __div__(self, rhs):
+        return op_binary(self, rhs, operator.__div__)
+    def __floordiv__(self, rhs):
+        return op_binary(self, rhs, operator.__floordiv__)
+    def __truediv__(self, rhs):
+        return op_binary(self, rhs, operator.__truediv__)
+    def __mod__(self, rhs):
+        return op_binary(self, rhs, operator.__mod__)
+    def __pow__(self, rhs):
+        return op_binary(self, rhs, operator.__pow__)
+
+    # Reflected binary operation
+    def __radd__(self, lhs):
+        return op_binary(lhs, self, operator.__add__)
+    def __rsub__(self, lhs):
+        return op_binary(lhs, self, operator.__sub__)
+    def __rmul__(self, lhs):
+        return op_binary(lhs, self, operator.__mul__)
+    def __rdiv__(self, lhs):
+        return op_binary(lhs, self, operator.__div__)
+    def __rfloordiv__(self, lhs):
+        return op_binary(lhs, self, operator.__floordiv__)
+    def __rtruediv__(self, lhs):
+        return op_binary(lhs, self, operator.__truediv__)
+    def __rmod__(self, lhs):
+        return op_binary(lhs, self, operator.__mod__)
+    def __rpow__(self, lhs):
+        return op_binary(lhs, self, operator.__pow__)
+
+    # In-place operations
+    def __iadd__(self, v):
+        return self.op_binary_inplace(v, operator.__add__)
+    def __isub__(self, v):
+        return self.op_binary_inplace(v, operator.__sub__)
+    def __imul__(self, v):
+        return self.op_binary_inplace(v, operator.__mul__)
+    def __idiv__(self, v):
+        return self.op_binary_inplace(v, operator.__div__)
+    def __ifloordiv__(self, v):
+        return self.op_binary_inplace(v, operator.__floordiv__)
+    def __itruediv__(self, v):
+        return self.op_binary_inplace(v, operator.__truediv__)
+    def __imod__(self, v):
+        return self.op_binary_inplace(v, operator.__mod__)
+    def __ipow__(self, v):
+        return self.op_binary_inplace(v, operator.__pow__)
+
+    # Boolean operations
+    def __eq__(self, rhs):
+        return op_relational(self, rhs, operator.__eq__)
+    def __ne__(self, rhs):
+        return op_relational(self, rhs, operator.__ne__)
+    def __lt__(self, rhs):
+        return op_relational(self, rhs, operator.__lt__)
+    def __le__(self, rhs):
+        return op_relational(self, rhs, operator.__le__)
+    def __ge__(self, rhs):
+        return op_relational(self, rhs, operator.__ge__)
+    def __gt__(self, rhs):
+        return op_relational(self, rhs, operator.__gt__)
+
+
+# Aliases
+def nfloat_type(name, exponent, mantissa):
+    def __init__(self, value=0.0):
+        nfloat.__init__(self, value, exponent, mantissa)
+    @staticmethod
+    def from_bytes(data, byteorder):
+        return nfloat.from_bytes(data, byteorder, exponent, mantissa)
+    return type(name, (nfloat,), {
+        "__init__": __init__,
+        "from_bytes": from_bytes
+    })
+
+# Shorthands
+float16 = nfloat_type('float16', exponent=5,  mantissa=10)
+float32 = nfloat_type('float32', exponent=8,  mantissa=23)
+float64 = nfloat_type('float64', exponent=11, mantissa=52)
```

## nativetypes/native_int.py

```diff
@@ -1,276 +1,276 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Native types.
-"""
-
-import operator
-import sys
-
-# Helpers
-def get_value(value, bits, signed):
-    if isinstance(value, nint):
-        value = value.v
-    mask = 2**bits - 1
-    if signed and value & (1 << (bits - 1)):
-        return value | ~mask
-    else:
-        return value & mask
-
-def ensure_native(lhs, rhs):
-    assert isinstance(lhs, nint) or isinstance(rhs, nint)
-    if not isinstance(lhs, nint):
-        lhs = nint(lhs, rhs.b, rhs.s)
-    if not isinstance(rhs, nint):
-        rhs = nint(rhs, lhs.b, lhs.s)
-    return lhs, rhs
-
-# Promotions
-def promote_bits(lhs, rhs):
-    return max(lhs.b, rhs.b)
-def promote_signed(lhs, rhs):
-    return lhs.s & rhs.s
-
-# Helpers
-def op_div(lhs, rhs):
-    return int(operator.truediv(lhs, rhs))
-def op_mod(lhs, rhs):
-    return lhs - op_div(lhs, rhs) * rhs
-
-# Operators
-def op_unary(value, op):
-    bits = value.b
-    signed = value.s
-    result = op(get_value(value, bits, signed))
-    return nint(result, bits, signed)
-
-def op_binary(lhs, rhs, op):
-    lhs, rhs = ensure_native(lhs, rhs)
-    bits = promote_bits(lhs, rhs)
-    signed = promote_signed(lhs, rhs)
-    result = op(
-        get_value(lhs, bits, signed),
-        get_value(rhs, bits, signed))
-    return nint(result, bits, signed)
-
-def op_relational(lhs, rhs, op):
-    lhs, rhs = ensure_native(lhs, rhs)
-    bits = promote_bits(lhs, rhs)
-    signed = promote_signed(lhs, rhs)
-    return op(
-        get_value(lhs, bits, signed),
-        get_value(rhs, bits, signed))
-
-# Native Integer
-class nint(object):
-    def __init__(self, value=0, bits=32, signed=True):
-        assert bits >= 1, 'Support down to int1 only'
-        self.b = bits
-        self.s = signed
-        self.m = (1 << bits) - 1
-        self.set(value)
-
-    # Bytes conversion
-    @staticmethod
-    def from_bytes(data, byteorder, bits, signed):
-        if sys.version_info[0] < 3:
-            if byteorder == 'little':
-                data = data[::-1]
-            value = int(data.encode('hex'), 16)
-        else:
-            value = int.from_bytes(data, byteorder)
-        return nint(value, bits, signed)
-
-    def to_bytes(self, byteorder):
-        length = (self.b + 7) // 8
-        if sys.version_info[0] < 3:
-            data = '%x' % int(self)
-            data = ('0' * (len(data) % 2) + data)
-            data = data.zfill(length * 2).decode('hex')
-            if byteorder == 'little':
-                data = data[::-1]
-            return data
-        else:
-            return int(self).to_bytes(length, byteorder)
-
-    def set(self, value):
-        if self.s and value & (1 << (self.b - 1)):
-            self.v = value | ~self.m
-        else:
-            self.v = value & self.m
-
-    def op_binary_inplace(self, value, op):
-        result_int = op(self.v, value)
-        self.set(result_int)
-        return self
-
-    # Utilities
-    def min(self):
-        return -(2 ** (self.b - 1)) * int(self.s)
-
-    def max(self):
-        return (2 ** (self.b - int(self.s))) - 1
-
-    # Slicing
-    def __getitem__(self, key):
-        if isinstance(key, int):
-            assert 0 <= key < self.b
-            return bool((int(self) >> key) & 1)
-        if isinstance(key, slice):
-            assert 0 <= key.start < self.b
-            assert 0 <= key.stop <= self.b
-            assert key.start < key.stop
-            bits = key.stop - key.start
-            value = int(self) >> key.start
-            return nint(value, bits, signed=False)
-
-    # Conversion operations
-    def __str__(self):
-        return str(int(self))
-    def __repr__(self):
-        typename = type(self).__name__
-        return '%s(%s)' % (typename, self)
-    def __format__(self, format_spec):
-        template = '{{:{}}}'.format(format_spec)
-        return template.format(int(self))
-    def __int__(self):
-        return int(self.v)
-    def __bool__(self):
-        return bool(self.v)
-    def __nonzero__(self):
-        return bool(self.v)
-    def __float__(self):
-        return float(self.v)
-    def __index__(self):
-        return self.v.__index__()
-
-    # Unary operations
-    def __abs__(self):
-        return op_unary(self, operator.__abs__)
-    def __pos__(self):
-        return op_unary(self, operator.__pos__)
-    def __neg__(self):
-        return op_unary(self, operator.__neg__)
-    def __invert__(self):
-        return op_unary(self, operator.__invert__)
-
-    # Binary operations
-    def __add__(self, rhs):
-        return op_binary(self, rhs, operator.__add__)
-    def __sub__(self, rhs):
-        return op_binary(self, rhs, operator.__sub__)
-    def __mul__(self, rhs):
-        return op_binary(self, rhs, operator.__mul__)
-    def __div__(self, rhs):
-        return op_binary(self, rhs, op_div)
-    def __floordiv__(self, rhs):
-        return op_binary(self, rhs, op_div)
-    def __truediv__(self, rhs):
-        return op_binary(self, rhs, op_div)
-    def __mod__(self, rhs):
-        return op_binary(self, rhs, op_mod)
-    def __pow__(self, rhs):
-        return op_binary(self, rhs, operator.__pow__)
-    def __and__(self, rhs):
-        return op_binary(self, rhs, operator.__and__)
-    def __or__(self, rhs):
-        return op_binary(self, rhs, operator.__or__)
-    def __xor__(self, rhs):
-        return op_binary(self, rhs, operator.__xor__)
-    def __lshift__(self, rhs):
-        return op_binary(self, rhs, operator.__lshift__)
-    def __rshift__(self, rhs):
-        return op_binary(self, rhs, operator.__rshift__)
-
-    # Reflected binary operation
-    def __radd__(self, lhs):
-        return op_binary(lhs, self, operator.__add__)
-    def __rsub__(self, lhs):
-        return op_binary(lhs, self, operator.__sub__)
-    def __rmul__(self, lhs):
-        return op_binary(lhs, self, operator.__mul__)
-    def __rdiv__(self, lhs):
-        return op_binary(lhs, self, op_div)
-    def __rfloordiv__(self, lhs):
-        return op_binary(lhs, self, op_div)
-    def __rtruediv__(self, lhs):
-        return op_binary(lhs, self, op_div)
-    def __rmod__(self, lhs):
-        return op_binary(lhs, self, op_mod)
-    def __rpow__(self, lhs):
-        return op_binary(lhs, self, operator.__pow__)
-    def __rand__(self, lhs):
-        return op_binary(lhs, self, operator.__and__)
-    def __ror__(self, lhs):
-        return op_binary(lhs, self, operator.__or__)
-    def __rxor__(self, lhs):
-        return op_binary(lhs, self, operator.__xor__)
-    def __rlshift__(self, lhs):
-        return op_binary(lhs, self, operator.__lshift__)
-    def __rrshift__(self, lhs):
-        return op_binary(lhs, self, operator.__rshift__)
-
-    # In-place operations
-    def __iadd__(self, v):
-        return self.op_binary_inplace(v, operator.__add__)
-    def __isub__(self, v):
-        return self.op_binary_inplace(v, operator.__sub__)
-    def __imul__(self, v):
-        return self.op_binary_inplace(v, operator.__mul__)
-    def __idiv__(self, v):
-        return self.op_binary_inplace(v, op_div)
-    def __ifloordiv__(self, v):
-        return self.op_binary_inplace(v, op_div)
-    def __itruediv__(self, v):
-        return self.op_binary_inplace(v, op_div)
-    def __imod__(self, v):
-        return self.op_binary_inplace(v, op_mod)
-    def __ipow__(self, v):
-        return self.op_binary_inplace(v, operator.__pow__)
-    def __iand__(self, v):
-        return self.op_binary_inplace(v, operator.__and__)
-    def __ior__(self, v):
-        return self.op_binary_inplace(v, operator.__or__)
-    def __ixor__(self, v):
-        return self.op_binary_inplace(v, operator.__xor__)
-    def __ilshift__(self, v):
-        return self.op_binary_inplace(v, operator.__lshift__)
-    def __irshift__(self, v):
-        return self.op_binary_inplace(v, operator.__rshift__)
-
-    # Boolean operations
-    def __eq__(self, rhs):
-        return op_relational(self, rhs, operator.__eq__)
-    def __ne__(self, rhs):
-        return op_relational(self, rhs, operator.__ne__)
-    def __lt__(self, rhs):
-        return op_relational(self, rhs, operator.__lt__)
-    def __le__(self, rhs):
-        return op_relational(self, rhs, operator.__le__)
-    def __ge__(self, rhs):
-        return op_relational(self, rhs, operator.__ge__)
-    def __gt__(self, rhs):
-        return op_relational(self, rhs, operator.__gt__)
-
-
-# Aliases
-def nint_type(name, bits, signed):
-    def __init__(self, value=0):
-        nint.__init__(self, value, bits, signed)
-    @staticmethod
-    def from_bytes(data, byteorder):
-        return nint.from_bytes(data, byteorder, bits, signed)
-    return type(name, (nint,), {
-        "__init__": __init__,
-        "from_bytes": from_bytes
-    })
-
-# Shorthands
-int8   = nint_type('int8',   bits=8,  signed=True)
-int16  = nint_type('int16',  bits=16, signed=True)
-int32  = nint_type('int32',  bits=32, signed=True)
-int64  = nint_type('int64',  bits=64, signed=True)
-uint8  = nint_type('uint8',  bits=8,  signed=False)
-uint16 = nint_type('uint16', bits=16, signed=False)
-uint32 = nint_type('uint32', bits=32, signed=False)
-uint64 = nint_type('uint64', bits=64, signed=False)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+Native types.
+"""
+
+import operator
+import sys
+
+# Helpers
+def get_value(value, bits, signed):
+    if isinstance(value, nint):
+        value = value.v
+    mask = 2**bits - 1
+    if signed and value & (1 << (bits - 1)):
+        return value | ~mask
+    else:
+        return value & mask
+
+def ensure_native(lhs, rhs):
+    assert isinstance(lhs, nint) or isinstance(rhs, nint)
+    if not isinstance(lhs, nint):
+        lhs = nint(lhs, rhs.b, rhs.s)
+    if not isinstance(rhs, nint):
+        rhs = nint(rhs, lhs.b, lhs.s)
+    return lhs, rhs
+
+# Promotions
+def promote_bits(lhs, rhs):
+    return max(lhs.b, rhs.b)
+def promote_signed(lhs, rhs):
+    return lhs.s & rhs.s
+
+# Helpers
+def op_div(lhs, rhs):
+    return int(operator.truediv(lhs, rhs))
+def op_mod(lhs, rhs):
+    return lhs - op_div(lhs, rhs) * rhs
+
+# Operators
+def op_unary(value, op):
+    bits = value.b
+    signed = value.s
+    result = op(get_value(value, bits, signed))
+    return nint(result, bits, signed)
+
+def op_binary(lhs, rhs, op):
+    lhs, rhs = ensure_native(lhs, rhs)
+    bits = promote_bits(lhs, rhs)
+    signed = promote_signed(lhs, rhs)
+    result = op(
+        get_value(lhs, bits, signed),
+        get_value(rhs, bits, signed))
+    return nint(result, bits, signed)
+
+def op_relational(lhs, rhs, op):
+    lhs, rhs = ensure_native(lhs, rhs)
+    bits = promote_bits(lhs, rhs)
+    signed = promote_signed(lhs, rhs)
+    return op(
+        get_value(lhs, bits, signed),
+        get_value(rhs, bits, signed))
+
+# Native Integer
+class nint(object):
+    def __init__(self, value=0, bits=32, signed=True):
+        assert bits >= 1, 'Support down to int1 only'
+        self.b = bits
+        self.s = signed
+        self.m = (1 << bits) - 1
+        self.set(value)
+
+    # Bytes conversion
+    @staticmethod
+    def from_bytes(data, byteorder, bits, signed):
+        if sys.version_info[0] < 3:
+            if byteorder == 'little':
+                data = data[::-1]
+            value = int(data.encode('hex'), 16)
+        else:
+            value = int.from_bytes(data, byteorder)
+        return nint(value, bits, signed)
+
+    def to_bytes(self, byteorder):
+        length = (self.b + 7) // 8
+        if sys.version_info[0] < 3:
+            data = '%x' % int(self)
+            data = ('0' * (len(data) % 2) + data)
+            data = data.zfill(length * 2).decode('hex')
+            if byteorder == 'little':
+                data = data[::-1]
+            return data
+        else:
+            return int(self).to_bytes(length, byteorder, signed=self.s)
+
+    def set(self, value):
+        if self.s and value & (1 << (self.b - 1)):
+            self.v = value | ~self.m
+        else:
+            self.v = value & self.m
+
+    def op_binary_inplace(self, value, op):
+        result_int = op(self.v, value)
+        self.set(result_int)
+        return self
+
+    # Utilities
+    def min(self):
+        return -(2 ** (self.b - 1)) * int(self.s)
+
+    def max(self):
+        return (2 ** (self.b - int(self.s))) - 1
+
+    # Slicing
+    def __getitem__(self, key):
+        if isinstance(key, int):
+            assert 0 <= key < self.b
+            return bool((int(self) >> key) & 1)
+        if isinstance(key, slice):
+            assert 0 <= key.start < self.b
+            assert 0 <= key.stop <= self.b
+            assert key.start < key.stop
+            bits = key.stop - key.start
+            value = int(self) >> key.start
+            return nint(value, bits, signed=False)
+
+    # Conversion operations
+    def __str__(self):
+        return str(int(self))
+    def __repr__(self):
+        typename = type(self).__name__
+        return '%s(%s)' % (typename, self)
+    def __format__(self, format_spec):
+        template = '{{:{}}}'.format(format_spec)
+        return template.format(int(self))
+    def __int__(self):
+        return int(self.v)
+    def __bool__(self):
+        return bool(self.v)
+    def __nonzero__(self):
+        return bool(self.v)
+    def __float__(self):
+        return float(self.v)
+    def __index__(self):
+        return self.v.__index__()
+
+    # Unary operations
+    def __abs__(self):
+        return op_unary(self, operator.__abs__)
+    def __pos__(self):
+        return op_unary(self, operator.__pos__)
+    def __neg__(self):
+        return op_unary(self, operator.__neg__)
+    def __invert__(self):
+        return op_unary(self, operator.__invert__)
+
+    # Binary operations
+    def __add__(self, rhs):
+        return op_binary(self, rhs, operator.__add__)
+    def __sub__(self, rhs):
+        return op_binary(self, rhs, operator.__sub__)
+    def __mul__(self, rhs):
+        return op_binary(self, rhs, operator.__mul__)
+    def __div__(self, rhs):
+        return op_binary(self, rhs, op_div)
+    def __floordiv__(self, rhs):
+        return op_binary(self, rhs, op_div)
+    def __truediv__(self, rhs):
+        return op_binary(self, rhs, op_div)
+    def __mod__(self, rhs):
+        return op_binary(self, rhs, op_mod)
+    def __pow__(self, rhs):
+        return op_binary(self, rhs, operator.__pow__)
+    def __and__(self, rhs):
+        return op_binary(self, rhs, operator.__and__)
+    def __or__(self, rhs):
+        return op_binary(self, rhs, operator.__or__)
+    def __xor__(self, rhs):
+        return op_binary(self, rhs, operator.__xor__)
+    def __lshift__(self, rhs):
+        return op_binary(self, rhs % self.b, operator.__lshift__)
+    def __rshift__(self, rhs):
+        return op_binary(self, rhs % self.b, operator.__rshift__)
+
+    # Reflected binary operation
+    def __radd__(self, lhs):
+        return op_binary(lhs, self, operator.__add__)
+    def __rsub__(self, lhs):
+        return op_binary(lhs, self, operator.__sub__)
+    def __rmul__(self, lhs):
+        return op_binary(lhs, self, operator.__mul__)
+    def __rdiv__(self, lhs):
+        return op_binary(lhs, self, op_div)
+    def __rfloordiv__(self, lhs):
+        return op_binary(lhs, self, op_div)
+    def __rtruediv__(self, lhs):
+        return op_binary(lhs, self, op_div)
+    def __rmod__(self, lhs):
+        return op_binary(lhs, self, op_mod)
+    def __rpow__(self, lhs):
+        return op_binary(lhs, self, operator.__pow__)
+    def __rand__(self, lhs):
+        return op_binary(lhs, self, operator.__and__)
+    def __ror__(self, lhs):
+        return op_binary(lhs, self, operator.__or__)
+    def __rxor__(self, lhs):
+        return op_binary(lhs, self, operator.__xor__)
+    def __rlshift__(self, lhs):
+        return op_binary(lhs, self % self.b, operator.__lshift__)
+    def __rrshift__(self, lhs):
+        return op_binary(lhs, self % self.b, operator.__rshift__)
+
+    # In-place operations
+    def __iadd__(self, v):
+        return self.op_binary_inplace(v, operator.__add__)
+    def __isub__(self, v):
+        return self.op_binary_inplace(v, operator.__sub__)
+    def __imul__(self, v):
+        return self.op_binary_inplace(v, operator.__mul__)
+    def __idiv__(self, v):
+        return self.op_binary_inplace(v, op_div)
+    def __ifloordiv__(self, v):
+        return self.op_binary_inplace(v, op_div)
+    def __itruediv__(self, v):
+        return self.op_binary_inplace(v, op_div)
+    def __imod__(self, v):
+        return self.op_binary_inplace(v, op_mod)
+    def __ipow__(self, v):
+        return self.op_binary_inplace(v, operator.__pow__)
+    def __iand__(self, v):
+        return self.op_binary_inplace(v, operator.__and__)
+    def __ior__(self, v):
+        return self.op_binary_inplace(v, operator.__or__)
+    def __ixor__(self, v):
+        return self.op_binary_inplace(v, operator.__xor__)
+    def __ilshift__(self, v):
+        return self.op_binary_inplace(v % self.b, operator.__lshift__)
+    def __irshift__(self, v):
+        return self.op_binary_inplace(v % self.b, operator.__rshift__)
+
+    # Boolean operations
+    def __eq__(self, rhs):
+        return op_relational(self, rhs, operator.__eq__)
+    def __ne__(self, rhs):
+        return op_relational(self, rhs, operator.__ne__)
+    def __lt__(self, rhs):
+        return op_relational(self, rhs, operator.__lt__)
+    def __le__(self, rhs):
+        return op_relational(self, rhs, operator.__le__)
+    def __ge__(self, rhs):
+        return op_relational(self, rhs, operator.__ge__)
+    def __gt__(self, rhs):
+        return op_relational(self, rhs, operator.__gt__)
+
+
+# Aliases
+def nint_type(name, bits, signed):
+    def __init__(self, value=0):
+        nint.__init__(self, value, bits, signed)
+    @staticmethod
+    def from_bytes(data, byteorder):
+        return nint.from_bytes(data, byteorder, bits, signed)
+    return type(name, (nint,), {
+        "__init__": __init__,
+        "from_bytes": from_bytes
+    })
+
+# Shorthands
+int8   = nint_type('int8',   bits=8,  signed=True)
+int16  = nint_type('int16',  bits=16, signed=True)
+int32  = nint_type('int32',  bits=32, signed=True)
+int64  = nint_type('int64',  bits=64, signed=True)
+uint8  = nint_type('uint8',  bits=8,  signed=False)
+uint16 = nint_type('uint16', bits=16, signed=False)
+uint32 = nint_type('uint32', bits=32, signed=False)
+uint64 = nint_type('uint64', bits=64, signed=False)
```

## Comparing `nativetypes-1.0.4.dist-info/LICENSE` & `nativetypes-1.0.5.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2017 Alexandro Sanchez Bach
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2017 Alexandro Sanchez Bach
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `nativetypes-1.0.4.dist-info/METADATA` & `nativetypes-1.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: nativetypes
-Version: 1.0.4
+Version: 1.0.5
 Summary: Native integer and floating-point type emulation
 Home-page: https://github.com/AlexAltea/ntypes
 Author: Alexandro Sanchez Bach
 Author-email: alexandro@phi.nz
 License: MIT
-Download-URL: https://github.com/AlexAltea/ntypes/tarball/1.0.4
+Download-URL: https://github.com/AlexAltea/ntypes/tarball/1.0.5
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English
+License-File: LICENSE
 
 Native Types
 ============
 
 .. image:: https://api.travis-ci.org/AlexAltea/ntypes.svg?branch=master
     :target: https://travis-ci.org/AlexAltea/ntypes/
-
+    
 .. image:: https://coveralls.io/repos/github/AlexAltea/ntypes/badge.svg?branch=master
     :target: https://coveralls.io/github/AlexAltea/ntypes?branch=master
-
+    
 .. image:: https://img.shields.io/pypi/v/nativetypes.svg
     :target: https://pypi.python.org/pypi/nativetypes
 
 Emulate native integer and floating-point types in Python 2.x and 3.x.
 
 More information at: https://github.com/AlexAltea/ntypes
```

