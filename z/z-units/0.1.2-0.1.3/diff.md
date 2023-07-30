# Comparing `tmp/z_units-0.1.2.tar.gz` & `tmp/z_units-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z_units-0.1.2.tar", last modified: Tue Jul 18 14:22:12 2023, max compression
+gzip compressed data, was "z_units-0.1.3.tar", last modified: Sun Jul 30 15:01:30 2023, max compression
```

## Comparing `z_units-0.1.2.tar` & `z_units-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.2/LICENSE
--rw-r--r--   0        0        0     1524 2023-07-18 14:19:21.237992 z_units-0.1.2/README.md
--rw-r--r--   0        0        0      482 2023-07-18 14:22:12.751657 z_units-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.2/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.2/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.2/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-07-02 15:02:03.569818 z_units-0.1.2/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1339 2023-07-03 15:10:37.598530 z_units-0.1.2/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-07-03 15:10:37.598530 z_units-0.1.2/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0    19021 2023-07-02 15:02:03.269821 z_units-0.1.2/tests/test_quantity.py
--rw-r--r--   0        0        0      476 2023-06-27 16:02:52.925927 z_units-0.1.2/tests/test_unit.py
--rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.2/z_units/__init__.py
--rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.2/z_units/config.py
--rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.2/z_units/constant.py
--rw-r--r--   0        0        0     5132 2023-07-10 15:01:56.710109 z_units-0.1.2/z_units/quantity.py
--rw-r--r--   0        0        0    23140 2023-07-03 15:10:37.389231 z_units-0.1.2/z_units/unit.py
--rw-r--r--   0        0        0     9232 2023-06-02 15:07:02.749962 z_units-0.1.2/z_units/unit_registry.py
--rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.2/z_units/util.py
--rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 z_units-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2175 2023-07-29 16:04:59.100145 z_units-0.1.3/README.md
+-rw-r--r--   0        0        0      480 2023-07-30 15:01:30.134987 z_units-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.3/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.3/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.3/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-07-18 14:59:00.022077 z_units-0.1.3/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1339 2023-07-30 14:56:27.281388 z_units-0.1.3/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-07-30 14:56:27.281388 z_units-0.1.3/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    19166 2023-07-18 15:04:09.433848 z_units-0.1.3/tests/test_quantity.py
+-rw-r--r--   0        0        0      476 2023-06-27 16:02:52.925927 z_units-0.1.3/tests/test_unit.py
+-rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.3/z_units/__init__.py
+-rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.3/z_units/config.py
+-rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.3/z_units/constant.py
+-rw-r--r--   0        0        0     5409 2023-07-26 14:34:40.166856 z_units-0.1.3/z_units/quantity.py
+-rw-r--r--   0        0        0    23176 2023-07-26 14:34:40.157886 z_units-0.1.3/z_units/unit.py
+-rw-r--r--   0        0        0     9258 2023-07-26 14:34:40.161873 z_units-0.1.3/z_units/unit_registry.py
+-rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.3/z_units/util.py
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 z_units-0.1.3/PKG-INFO
```

### Comparing `z_units-0.1.2/LICENSE` & `z_units-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `z_units-0.1.2/tests/.pytest_cache/v/cache/nodeids` & `z_units-0.1.3/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `z_units-0.1.2/tests/test_quantity.py` & `z_units-0.1.3/tests/test_quantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 from z_units.config import set_local_atmospheric_pressure, set_standard_temperature
 
 
 def test_length():
     x = q.Length(1)
     assert x.unit.symbol == 'm'
     assert x.unit == x.base_unit
-    assert f'{x:U}' == '1 m'
-    assert f'{x:Uq}' == '1 m'
-    assert f'{x:Up}' == '1 m'
+    assert f'{x:u}' == '1 m'
+    assert f'{x:uq}' == '1 m'
+    assert f'{x:up}' == '1 m'
+    print(f"Length(1) * 5 = {x * 5:u}")
+    print(f"5 * Length(1) = {5 * x:u}")
+    print(f"5 * Length(1, 'ft') = {5 * q.Length(1, 'ft'):u}")
     assert isclose(x.to('km').value, 1e-3, rel_tol=1e-4)
     assert isclose(x.to('dm').value, 1e1, rel_tol=1e-4)
     assert isclose(x.to('cm').value, 1e2, rel_tol=1e-4)
     assert isclose(x.to('mm').value, 1e3, rel_tol=1e-4)
     assert isclose(x.to('um').value, 1e6, rel_tol=1e-4)
     assert isclose(x.to('ft').value, 3.28084, rel_tol=1e-4)
     assert isclose(x.to('in').value, 39.37008, rel_tol=1e-4)
 
 
 def test_area():
     x = q.Area(1)
     assert x.unit.symbol == 'm2'
-    assert f'{x:U}' == '1 m2'
-    assert f'{x:Up}' == '1 m**2'
+    assert f'{x:u}' == '1 m2'
+    assert f'{x:up}' == '1 m**2'
     assert x.unit == x.base_unit
     assert isclose(x.to('km2').value, 1e-6, rel_tol=1e-4)
     assert isclose(x.to('dm2').value, 1e2, rel_tol=1e-4)
     assert isclose(x.to('cm2').value, 1e4, rel_tol=1e-4)
     assert isclose(x.to('mm2').value, 1e6, rel_tol=1e-4)
     assert isclose(x.to('um2').value, 1e12, rel_tol=1e-4)
     assert isclose(x.to('ft2').value, 10.7639, rel_tol=1e-4)
```

### Comparing `z_units-0.1.2/z_units/config.py` & `z_units-0.1.3/z_units/config.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.2/z_units/quantity.py` & `z_units-0.1.3/z_units/quantity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from typing import List
+from __future__ import annotations
+from typing import List, Union
 
 from .unit import Unit
 from .unit_registry import UnitRegistry
 from . import unit_registry as reg
 
 
 class Quantity:
     """
     Class used to represent a Quantity
 
     A quantity has a value and a unit
     """
 
-    def __init__(self, value, unit_symbol: str = None):
+    def __init__(self, value, unit: Union[str, Unit] = None):
         self.value = value
-        if unit_symbol is None:
+        if unit is None:
             self._unit = self.unit_registry.base_unit
         else:
-            self._unit = self.unit_registry.get_unit(unit_symbol)
+            self._unit = self.unit_registry.get_unit(str(unit))
 
-    def to(self, unit_symbol: str):
+    def to(self, unit: Union[str, Unit]):
         if self.value is None:
             return None
         ref_value = self._unit.to_base_unit(self.value)
-        value = self.unit_registry.get_unit(unit_symbol).from_base_unit(ref_value)
-        return self.__class__(value, unit_symbol)
+        value = self.unit_registry.get_unit(str(unit)).from_base_unit(ref_value)
+        return self.__class__(value, unit)
 
     @property
     def unit_registry(self) -> UnitRegistry:
         return self.get_unit_registry()
 
     def get_unit_registry(self):
         return UnitRegistry(reg.dimensionless)
@@ -57,14 +58,23 @@
             unit = format(self.unit, format_spec[pos + 1:])
             format_spec = format_spec[0:pos]
             if unit:
                 return ' '.join([format(self.value, format_spec), unit])
 
         return format(self.value, format_spec)
 
+    def __mul__(self, other):
+        if isinstance(other, (int, float)):
+            return self.__class__(self.value * other, self.unit)
+
+        return NotImplemented
+
+    def __rmul__(self, other):
+        return self * other
+
     @property
     def unit(self) -> Unit:
         return self._unit
 
 
 class Length(Quantity):
     def get_unit_registry(self):
```

### Comparing `z_units-0.1.2/z_units/unit.py` & `z_units-0.1.3/z_units/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Union, Callable
 
 from .config import get_local_atmospheric_pressure, get_standard_temperature
 from .util import multi_replace
 from . import constant
```

### Comparing `z_units-0.1.2/z_units/unit_registry.py` & `z_units-0.1.3/z_units/unit_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Iterable
 
 from . import unit as u
 from .unit import Unit, BaseUnit
 
 
 class UnitRegistry:
@@ -25,15 +26,15 @@
     @property
     def base_unit(self):
         return self._base_unit
 
     def get_unit(self, symbol: str):
         if unit := self._symbol_to_unit.get(symbol):
             return unit
-        raise ValueError(f"Unit with symbol {symbol} not found")
+        raise ValueError(f"Unit '{symbol}' not found")
 
     @property
     def units(self):
         return self._units
 
 
 length = UnitRegistry(units=[
```

### Comparing `z_units-0.1.2/z_units/util.py` & `z_units-0.1.3/z_units/util.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.2/PKG-INFO` & `z_units-0.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,107 @@
-Metadata-Version: 2.1
-Name: z-units
-Version: 0.1.2
-Summary: A simple unit converter for chemical engineering
-Author-Email: zenius <zenius@outlook.com>
-License: MIT
-Project-URL: Homepage, https://github.com/zxzenius/z-units
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# z-units
-
-A simple unit-converter for chemical engineers
-
-## Feature
-
-* Gauge pressure (MPag, kPag, psig, ...) can be used
-* Friendly to HYSYS user
-
-## Install
-
-```shell
-pip install z-units
-```
-
-## Usage
-
-```python
-from z_units import quantity as q
-# pick a quantity
-f = q.MolarFlow(3)
-# to base unit
-f.to_base()
-# convert
-f.to('kmol/s')
-# list available units
-print(f.units)
-# get value
-value, unit = f.value, f.unit
-# gauge pressure
-p = q.Pressure(5, 'bar').to('MPag')
-# change local atmospheric pressure (default: 101325 Pa)
-from z_units import config
-config.set_local_atmospheric_pressure(50e3)
-q.Pressure(100, 'kPa').to('kPag')
-# change standard temperature (default: 20 degC)
-# affect standard cubic meter "Sm**3"
-config.set_standard_temperature(15)
-q.Substance(100, 'Nm3').to('Sm3')
-# formatting
-# with unit in styles, format spec starts with "u"
-format(q.MolarEntropy(100), 'u')
-# '100 kJ/kmol-C' (quick-style)
-format(q.MolarEntropy(100), 'up')
-# '100 kJ/(kmol*C)' (expression-style)
-```
-
-## Predefined Quantities
-
-* Length
-* Area
-* Volume
-* Time
-* Mass
-* Force
-* Substance
-* Energy
-* Velocity
-* Temperature
-* DeltaTemperature
-* Pressure
-* VolumeFlow
-* MassDensity
-* HeatFlow
-* MolarFlow
-* MassFlow
-* MolarDensity
-* MolarHeatCapacity
-* MolarEntropy
-* MolarHeat
-* ThermalConductivity
-* Viscosity
-* SurfaceTension
-* MassHeatCapacity
-* MassEntropy
-* MassHeat
-* StandardGasFlow
-* KinematicViscosity
-* MolarVolume
-* Fraction
-* Dimensionless
+# z-units
+
+A simple unit-converter for chemical engineers
+
+## Feature
+
+* Gauge pressure units (MPag, kPag, psig, ...) are ready for use
+* Friendly to HYSYS user
+
+## Install
+
+```shell
+pip install z-units
+```
+
+## Quickstart
+
+```python
+>>> from z_units import quantity as q
+>>> f = q.MolarFlow(3)
+>>> f
+<MolarFlow(3, 'kmol/s')>
+f.value, f.unit
+(3, <Unit('kmol/s')>)
+>>> f.to('kmol/h')
+<MolarFlow(10800.0, 'kmol/h')>
+>>> q.Pressure(15, 'psi').to('MPag')
+<Pressure(0.0020963594, 'MPag')>
+```
+Related to gauge pressure, local atmospheric pressure (default: 101325 Pa) can be altered:
+
+```python
+>>> from z_units import config
+# Before
+>>> q.Pressure(100, 'kPa').to('kPag')
+<Pressure(-1.325, 'kPag')>
+# Set to 50e3 Pa (50 kPa)
+>>> config.set_local_atmospheric_pressure(50e3)
+# After
+>>> q.Pressure(100, 'kPa').to('kPag')
+<Pressure(50.0, 'kPag')>
+```
+
+Standard temperature (default: 20 degC) can be redefined, affecting standard cubic meter "Sm**3":
+
+```python
+# Before
+>>> q.Substance(100, 'Nm3').to('Sm3')
+<Substance(107.321984, 'Sm3')>
+# Set to 15 degC
+>>> config.set_standard_temperature(15)
+# After
+>>> q.Substance(100, 'Nm3').to('Sm3')
+<Substance(105.491488, 'Sm3')>
+```
+
+Format quantity to string with styles:  
+```python
+# Only value
+>>> format(q.MolarEntropy(100))
+'100'
+# With unit, quick style
+>>> format(q.MolarEntropy(100), 'u')
+'100 kJ/kmol-C'
+# With unit, definition style
+>>> format(q.MolarEntropy(100), 'up')
+'100 kJ/(kmol*C)'
+```
+
+## Predefined Quantities
+
+* Length
+* Area
+* Volume
+* Time
+* Mass
+* Force
+* Substance
+* Energy
+* Velocity
+* Temperature
+* DeltaTemperature
+* Pressure
+* VolumeFlow
+* MassDensity
+* HeatFlow
+* MolarFlow
+* MassFlow
+* MolarDensity
+* MolarHeatCapacity
+* MolarEntropy
+* MolarHeat
+* ThermalConductivity
+* Viscosity
+* SurfaceTension
+* MassHeatCapacity
+* MassEntropy
+* MassHeat
+* StandardGasFlow
+* KinematicViscosity
+* MolarVolume
+* Fraction
+* Dimensionless
+
+## About it
+
+As a chemical engineer, the Gauge-Pressure units are very useful to me. Unfortunately those units are not supported in some popular modules, so I reinvent the wheel.
```

