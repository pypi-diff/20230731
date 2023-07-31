# Comparing `tmp/atopy-0.5.1.tar.gz` & `tmp/atopy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atopy-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "atopy-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `atopy-0.5.1.tar` & `atopy-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1799 2023-07-25 09:53:45.838764 atopy-0.5.1/.gitignore
--rw-r--r--   0        0        0     1060 2023-07-25 09:53:45.838764 atopy-0.5.1/LICENSE
--rw-r--r--   0        0        0      228 2023-07-25 09:53:45.838764 atopy-0.5.1/README.md
--rw-r--r--   0        0        0       51 2023-07-25 10:34:50.097798 atopy-0.5.1/atopy/__init__.py
--rw-r--r--   0        0        0     1654 2023-07-25 09:53:45.838764 atopy-0.5.1/atopy/datetime.py
--rw-r--r--   0        0        0     2278 2023-07-25 10:34:50.097798 atopy-0.5.1/atopy/decimal.py
--rw-r--r--   0        0        0      521 2023-07-25 09:53:45.838764 atopy-0.5.1/atopy/io.py
--rw-r--r--   0        0        0       84 2023-07-25 09:53:45.838764 atopy-0.5.1/atopy/main.py
--rw-r--r--   0        0        0        0 2023-07-25 09:53:45.838764 atopy-0.5.1/atopy/py.typed
--rw-r--r--   0        0        0      228 2023-07-25 09:53:45.838764 atopy-0.5.1/atopy/pydantic.py
--rw-r--r--   0        0        0       85 2023-07-25 09:53:45.838764 atopy-0.5.1/atopy/typer.py
--rwxr-xr-x   0        0        0      138 2023-07-25 09:53:45.838764 atopy-0.5.1/lint.sh
--rw-r--r--   0        0        0     1545 2023-07-25 09:53:45.838764 atopy-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 atopy-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-25 09:53:45.838764 atopy-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1060 2023-07-25 09:53:45.838764 atopy-0.5.2/LICENSE
+-rw-r--r--   0        0        0      228 2023-07-25 09:53:45.838764 atopy-0.5.2/README.md
+-rw-r--r--   0        0        0       51 2023-07-31 12:13:51.293480 atopy-0.5.2/atopy/__init__.py
+-rw-r--r--   0        0        0     1654 2023-07-25 09:53:45.838764 atopy-0.5.2/atopy/datetime.py
+-rw-r--r--   0        0        0     2057 2023-07-31 12:13:51.293480 atopy-0.5.2/atopy/decimal.py
+-rw-r--r--   0        0        0      521 2023-07-25 09:53:45.838764 atopy-0.5.2/atopy/io.py
+-rw-r--r--   0        0        0       84 2023-07-25 09:53:45.838764 atopy-0.5.2/atopy/main.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:53:45.838764 atopy-0.5.2/atopy/py.typed
+-rw-r--r--   0        0        0      228 2023-07-25 09:53:45.838764 atopy-0.5.2/atopy/pydantic.py
+-rw-r--r--   0        0        0       85 2023-07-25 09:53:45.838764 atopy-0.5.2/atopy/typer.py
+-rwxr-xr-x   0        0        0      138 2023-07-25 09:53:45.838764 atopy-0.5.2/lint.sh
+-rw-r--r--   0        0        0     1545 2023-07-25 09:53:45.838764 atopy-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 atopy-0.5.2/PKG-INFO
```

### Comparing `atopy-0.5.1/.gitignore` & `atopy-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `atopy-0.5.1/LICENSE` & `atopy-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atopy-0.5.1/atopy/datetime.py` & `atopy-0.5.2/atopy/datetime.py`

 * *Files identical despite different names*

### Comparing `atopy-0.5.1/atopy/decimal.py` & `atopy-0.5.2/atopy/decimal.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,49 +43,41 @@
     return di_down(div(dividend, divisor))
 
 
 def div_di_up(dividend: Decimal, divisor: Decimal) -> Decimal:
     return di_up(div(dividend, divisor))
 
 
-def bid_ticksize(price: Decimal, ticksize: Decimal) -> Decimal:
-    return ticksize * div_di_floor(price, ticksize)
+def cal_qty(qty: Decimal, qty_unit: Decimal) -> Decimal:
+    return qty_unit * div_di_down(qty, qty_unit)
 
 
-def ask_ticksize(price: Decimal, ticksize: Decimal) -> Decimal:
-    return ticksize * div_di_ceil(price, ticksize)
-
-
-def qty_unit(qty: Decimal, qtyunit: Decimal) -> Decimal:
-    return qtyunit * div_di_down(qty, qtyunit)
-
-
-def cash_qty(
+def cal_cash_qty(
     cash: Decimal,
     price: Decimal,
     contract_unit: Decimal,
-    qtyunit: Decimal,
+    qty_unit: Decimal,
 ) -> Decimal:
-    assert price > 0 and contract_unit > 0 and qtyunit > 0
+    assert price > 0 and contract_unit > 0 and qty_unit > 0
     if cash <= 0:
         return Decimal()
-    return qty_unit(div(cash, price * contract_unit), qtyunit)
+    return cal_qty(div(cash, price * contract_unit), qty_unit)
 
 
-def cash_risk_qty(
+def cal_cash_risk_qty(
     cash: Decimal,
     bet_fraction: Decimal,
     risk_point: Decimal,
     contract_unit: Decimal,
-    qtyunit: Decimal,
+    qty_unit: Decimal,
 ) -> Decimal:
     assert (
         bet_fraction >= 0
         and risk_point > 0
         and contract_unit > 0
-        and qtyunit > 0
+        and qty_unit > 0
     )
     if cash <= 0:
         return Decimal()
-    return qty_unit(
-        div(cash * bet_fraction, risk_point * contract_unit), qtyunit
+    return cal_qty(
+        div(cash * bet_fraction, risk_point * contract_unit), qty_unit
     )
```

### Comparing `atopy-0.5.1/atopy/io.py` & `atopy-0.5.2/atopy/io.py`

 * *Files identical despite different names*

### Comparing `atopy-0.5.1/pyproject.toml` & `atopy-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atopy-0.5.1/PKG-INFO` & `atopy-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atopy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python Common Library
 Author-email: Tom <nanticj@users.noreply.github.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: loguru >=0.7,<0.8
 Requires-Dist: pydantic >=1.10,<1.11
```

