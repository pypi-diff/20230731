# Comparing `tmp/classiq-0.9.1-py3-none-any.whl.zip` & `tmp/classiq-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 149019 bytes, number of entries: 161
+Zip file size: 149030 bytes, number of entries: 161
 -rw-r--r--  2.0 unx      856 b- defN 80-Jan-01 00:00 classiq/__init__.py
 -rw-r--r--  2.0 unx     7168 b- defN 80-Jan-01 00:00 classiq/_internals/api_wrapper.py
 -rw-r--r--  2.0 unx      966 b- defN 80-Jan-01 00:00 classiq/_internals/async_utils.py
 -rw-r--r--  2.0 unx     2766 b- defN 80-Jan-01 00:00 classiq/_internals/authentication/auth0.py
 -rw-r--r--  2.0 unx      298 b- defN 80-Jan-01 00:00 classiq/_internals/authentication/authentication.py
 -rw-r--r--  2.0 unx     3428 b- defN 80-Jan-01 00:00 classiq/_internals/authentication/device.py
 -rw-r--r--  2.0 unx     2443 b- defN 80-Jan-01 00:00 classiq/_internals/authentication/password_manager.py
@@ -86,15 +86,15 @@
 -rw-r--r--  2.0 unx     2499 b- defN 80-Jan-01 00:00 classiq/interface/finance/function_input.py
 -rw-r--r--  2.0 unx     1261 b- defN 80-Jan-01 00:00 classiq/interface/finance/gaussian_model_input.py
 -rw-r--r--  2.0 unx      912 b- defN 80-Jan-01 00:00 classiq/interface/finance/log_normal_model_input.py
 -rw-r--r--  2.0 unx      474 b- defN 80-Jan-01 00:00 classiq/interface/finance/model_input.py
 -rw-r--r--  2.0 unx      453 b- defN 80-Jan-01 00:00 classiq/interface/generator/adjacency.py
 -rw-r--r--  2.0 unx     1562 b- defN 80-Jan-01 00:00 classiq/interface/generator/amplitude_estimation.py
 -rw-r--r--  2.0 unx     1342 b- defN 80-Jan-01 00:00 classiq/interface/generator/ansatz_library.py
--rw-r--r--  2.0 unx     4475 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/arithmetic.py
+-rw-r--r--  2.0 unx     4525 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/arithmetic.py
 -rw-r--r--  2.0 unx     6485 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/binary_ops.py
 -rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/endianness.py
 -rw-r--r--  2.0 unx     6827 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/fix_point_number.py
 -rw-r--r--  2.0 unx     2543 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/logical_ops.py
 -rw-r--r--  2.0 unx      652 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/register_user_input.py
 -rw-r--r--  2.0 unx      986 b- defN 80-Jan-01 00:00 classiq/interface/generator/arith/unary_ops.py
 -rw-r--r--  2.0 unx      213 b- defN 80-Jan-01 00:00 classiq/interface/generator/circuit_outline.py
@@ -153,11 +153,11 @@
 -rw-r--r--  2.0 unx      750 b- defN 80-Jan-01 00:00 classiq/interface/pyomo_extension/__init__.py
 -rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 classiq/interface/pyomo_extension/equality_expression.py
 -rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 classiq/interface/pyomo_extension/inequality_expression.py
 -rw-r--r--  2.0 unx      307 b- defN 80-Jan-01 00:00 classiq/interface/pyomo_extension/set_pprint.py
 -rw-r--r--  2.0 unx      131 b- defN 80-Jan-01 00:00 classiq/interface/server/authentication.py
 -rw-r--r--  2.0 unx     1625 b- defN 80-Jan-01 00:00 classiq/interface/server/routes.py
 -rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 classiq/interface/status.py
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 classiq-0.9.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2920 b- defN 16-Jan-01 00:00 classiq-0.9.1.dist-info/METADATA
-?rw-r--r--  2.0 unx    16720 b- defN 16-Jan-01 00:00 classiq-0.9.1.dist-info/RECORD
-161 files, 382549 bytes uncompressed, 121425 bytes compressed:  68.3%
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 classiq-0.9.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2920 b- defN 16-Jan-01 00:00 classiq-0.9.3.dist-info/METADATA
+?rw-r--r--  2.0 unx    16720 b- defN 16-Jan-01 00:00 classiq-0.9.3.dist-info/RECORD
+161 files, 382599 bytes uncompressed, 121436 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -468,17 +468,17 @@
 
 Filename: classiq/interface/server/routes.py
 Comment: 
 
 Filename: classiq/interface/status.py
 Comment: 
 
-Filename: classiq-0.9.1.dist-info/WHEEL
+Filename: classiq-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: classiq-0.9.1.dist-info/METADATA
+Filename: classiq-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: classiq-0.9.1.dist-info/RECORD
+Filename: classiq-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## classiq/model_designer/function_handler.pyi

 * *Ordering differences only*

```diff
@@ -24,88 +24,88 @@
 
 class FunctionHandler(abc.ABC, metaclass=abc.ABCMeta):
     def __init__(self) -> None: ...
     def apply(self, function_name: str, in_wires: Optional[Union[Dict[str, QregOrWire], QuantumRegister]] = ..., out_wires: Optional[Union[Dict[str, QregOrWire], QuantumRegister]] = ..., call_name: Optional[str] = ...) -> Dict[str, Wire]: ...
     def __getattr__(self, item): ...
     def __dir__(self): ...
     def include_library(self, library: FunctionLibrary) -> None: ...
+    def RZZGate(self, params: RZZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Mcx(self, params: Mcx, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def GridEntangler(self, params: GridEntangler, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def HartreeFock(self, params: HartreeFock, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CRXGate(self, params: CRXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def ZGate(self, params: ZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def BitwiseAnd(self, params: BitwiseAnd, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LogicalAnd(self, params: LogicalAnd, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def TGate(self, params: TGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CYGate(self, params: CYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def QFT(self, params: QFT, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CyclicShift(self, params: CyclicShift, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CPhaseGate(self, params: CPhaseGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CDFComparator(self, params: CDFComparator, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def PhaseGate(self, params: PhaseGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def SparseAmpLoad(self, params: SparseAmpLoad, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def UCC(self, params: UCC, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CSXGate(self, params: CSXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def YGate(self, params: YGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def TdgGate(self, params: TdgGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Adder(self, params: Adder, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def TwoDimensionalEntangler(self, params: TwoDimensionalEntangler, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Arithmetic(self, params: Arithmetic, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def SXdgGate(self, params: SXdgGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def GreaterThan(self, params: GreaterThan, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CZGate(self, params: CZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def CXGate(self, params: CXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CustomFunction(self, params: CustomFunction, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Finance(self, params: Finance, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Mcx(self, params: Mcx, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def BitwiseXor(self, params: BitwiseXor, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RZZGate(self, params: RZZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def HypercubeEntangler(self, params: HypercubeEntangler, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def SXGate(self, params: SXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def YGate(self, params: YGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LinearPauliRotations(self, params: LinearPauliRotations, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def BitwiseInvert(self, params: BitwiseInvert, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CSXGate(self, params: CSXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def StatePreparation(self, params: StatePreparation, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RYYGate(self, params: RYYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RGate(self, params: RGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Max(self, params: Max, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RShift(self, params: RShift, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def BitwiseOr(self, params: BitwiseOr, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def StatePropagator(self, params: StatePropagator, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RXGate(self, params: RXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def SdgGate(self, params: SdgGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def FinancePayoff(self, params: FinancePayoff, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LessThan(self, params: LessThan, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def iSwapGate(self, params: iSwapGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CHGate(self, params: CHGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def C3XGate(self, params: C3XGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def FinanceModels(self, params: FinanceModels, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def BitwiseOr(self, params: BitwiseOr, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def SXGate(self, params: SXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CCXGate(self, params: CCXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RZGate(self, params: RZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RYYGate(self, params: RYYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LShift(self, params: LShift, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def Exponentiation(self, params: Exponentiation, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def TwoDimensionalEntangler(self, params: TwoDimensionalEntangler, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Arithmetic(self, params: Arithmetic, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def ArithmeticOracle(self, params: ArithmeticOracle, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def HardwareEfficientAnsatz(self, params: HardwareEfficientAnsatz, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CHGate(self, params: CHGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def SGate(self, params: SGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def GroverOperator(self, params: GroverOperator, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LessEqual(self, params: LessEqual, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Equal(self, params: Equal, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def MCPhaseGate(self, params: MCPhaseGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def SdgGate(self, params: SdgGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def XGate(self, params: XGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RZGate(self, params: RZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def HypercubeEntangler(self, params: HypercubeEntangler, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LinearGCI(self, params: LinearGCI, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def HadamardAmpLoad(self, params: HadamardAmpLoad, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def FinancePayoff(self, params: FinancePayoff, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RXGate(self, params: RXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CPhaseGate(self, params: CPhaseGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def SGate(self, params: SGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def WeightedAdder(self, params: WeightedAdder, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CyclicShift(self, params: CyclicShift, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def ArithmeticOracle(self, params: ArithmeticOracle, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Finance(self, params: Finance, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RYGate(self, params: RYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RXXGate(self, params: RXXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def GreaterThan(self, params: GreaterThan, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LogicalOr(self, params: LogicalOr, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def Subtractor(self, params: Subtractor, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CRZGate(self, params: CRZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CustomFunction(self, params: CustomFunction, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def UnitaryGate(self, params: UnitaryGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def IGate(self, params: IGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def SparseAmpLoad(self, params: SparseAmpLoad, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CRYGate(self, params: CRYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def NotEqual(self, params: NotEqual, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def WeightedAdder(self, params: WeightedAdder, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def MCPhaseGate(self, params: MCPhaseGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def UCC(self, params: UCC, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def C4XGate(self, params: C4XGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LogicalOr(self, params: LogicalOr, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def GridEntangler(self, params: GridEntangler, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def iSwapGate(self, params: iSwapGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Max(self, params: Max, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CCXGate(self, params: CCXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def GreaterEqual(self, params: GreaterEqual, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def AmplitudeEstimation(self, params: AmplitudeEstimation, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RShift(self, params: RShift, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def HadamardAmpLoad(self, params: HadamardAmpLoad, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CRXGate(self, params: CRXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def SwapGate(self, params: SwapGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CRZGate(self, params: CRZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def C3XGate(self, params: C3XGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RYGate(self, params: RYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def RXXGate(self, params: RXXGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def HGate(self, params: HGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LogicalAnd(self, params: LogicalAnd, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def Multiplier(self, params: Multiplier, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LShift(self, params: LShift, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Subtractor(self, params: Subtractor, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Equal(self, params: Equal, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CYGate(self, params: CYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LinearPauliRotations(self, params: LinearPauliRotations, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def BitwiseAnd(self, params: BitwiseAnd, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def HGate(self, params: HGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def PhaseGate(self, params: PhaseGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def Negation(self, params: Negation, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def CRYGate(self, params: CRYGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def Adder(self, params: Adder, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
-    def LinearGCI(self, params: LinearGCI, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def GroverOperator(self, params: GroverOperator, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def AmplitudeEstimation(self, params: AmplitudeEstimation, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def StatePreparation(self, params: StatePreparation, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CZGate(self, params: CZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def ZGate(self, params: ZGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def QFT(self, params: QFT, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LessEqual(self, params: LessEqual, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
     def Min(self, params: Min, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def GreaterEqual(self, params: GreaterEqual, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def BitwiseInvert(self, params: BitwiseInvert, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def LessThan(self, params: LessThan, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def CDFComparator(self, params: CDFComparator, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def BitwiseXor(self, params: BitwiseXor, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def TGate(self, params: TGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def C4XGate(self, params: C4XGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
+    def RGate(self, params: RGate, in_wires: Optional[Dict[str, Wire]] = None) -> Dict[str, Wire]: ...
```

## classiq/interface/generator/arith/arithmetic.py

```diff
@@ -14,14 +14,15 @@
 from classiq.interface.generator.function_params import FunctionParams
 from classiq.interface.helpers.custom_pydantic_types import pydanticExpressionStr
 
 DEFAULT_OUT_NAME = "out"
 DEFAULT_ARG_NAME = "in_arg"
 
 SUPPORTED_FUNC_NAMES = ("CLShift", "CRShift", "min", "max")
+SUPPORTED_VAR_NAMES_REG = "[A-Za-z][A-Za-z0-9]*"
 
 white_list = {"or", "and"}.union(SUPPORTED_FUNC_NAMES)
 black_list = set(keyword.kwlist) - white_list
 
 
 class MappingMethods(str, enum.Enum):
     topological = "naive"
@@ -50,15 +51,15 @@
             raise ValueError(f"Failed to parse expression '{expression}'")
         return expression
 
     @pydantic.root_validator()
     def check_all_variable_are_defined(cls, values):
         expression, definitions = values.get("expression"), values.get("definitions")
 
-        literals = set(re.findall("[A-Za-z][A-Za-z0-9]*", expression))
+        literals = set(re.findall(SUPPORTED_VAR_NAMES_REG, expression))
 
         not_allowed = literals.intersection(black_list)
         undefined_literals = literals.difference(definitions, white_list)
         if not_allowed:
             raise ValueError(f"The following names: {not_allowed} are not allowed")
 
         if undefined_literals:
```

## Comparing `classiq-0.9.1.dist-info/METADATA` & `classiq-0.9.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classiq
-Version: 0.9.1
+Version: 0.9.3
 Summary: Classiq's Python SDK for quantum computing
 Home-page: https://classiq.io
 License: Proprietary
 Keywords: quantum computing,quantum circuits,quantum algorithms,QAD,QDL
 Author: Classiq Technologies
 Author-email: support@classiq.io
 Requires-Python: >=3.7,<4.0
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: classiq Version: 0.9.1 Summary: Classiq's Python
+Metadata-Version: 2.1 Name: classiq Version: 0.9.3 Summary: Classiq's Python
 SDK for quantum computing Home-page: https://classiq.io License: Proprietary
 Keywords: quantum computing,quantum circuits,quantum algorithms,QAD,QDL Author:
 Classiq Technologies Author-email: support@classiq.io Requires-Python:
 >=3.7,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Operating System ::
```

## Comparing `classiq-0.9.1.dist-info/RECORD` & `classiq-0.9.3.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 classiq/builtin_functions/standard_gates.py,sha256=6eiEQIjknd-sTjOXAx7QQoELlmlcfiWLfDAGrM8FWLQ,103
 classiq/examples/Circuit_Generation.ipynb,sha256=7Y6j2NHTCABThtZF7cXMlEmkE6N1q3cy2rx-epu8W0c,5899
 classiq/exceptions.py,sha256=BAHqPkEoTszQZy9YuvlD2tUQAay86-vVuQYsL3ay4ts,887
 classiq/executor.py,sha256=lIlpnKeXJxHS0Bb5HUpzIJ7uEnmLJNMcKCOZExK6xJM,5250
 classiq/model_designer/__init__.py,sha256=gICM4PXRYQN95SUkoh4hRtapM7qq6yQYI7SVwfd_ZJM,192
 classiq/model_designer/composite_function_generator.py,sha256=LQd_xVHmlZ15hrMYV3F3LNL_Wgxe062PxxPs6CDo_ps,2369
 classiq/model_designer/function_handler.py,sha256=mrNbQLyIwUkUmpzoerF-qd08kXAknmKgR7SRblBzp4I,10267
-classiq/model_designer/function_handler.pyi,sha256=cGoEXbD1CpYaldRtZJd2mll99VIq-9INsnwwmF5zkE8,10741
+classiq/model_designer/function_handler.pyi,sha256=9N53hxcxxuyHZnowMFgfZj0ehqEhFEd3AG1Ln4KfHDs,10741
 classiq/model_designer/model_designer.py,sha256=ErNMdZtZ105tdzTOS8tzznG40HCElRSLO_6w2P2aofE,5661
 classiq/model_designer/wire.py,sha256=aa4RuVg82lydej1kcanHqaQKJWFttHt59odNmGpp3Mg,2617
 classiq/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 classiq/quantum_functions/__init__.py,sha256=-9N0rQHizuga39WJCspt5FxDxvmchGCVe3vNnIdYZkY,199
 classiq/quantum_functions/annotation_parser.py,sha256=JhSHJXX9wo4erxOwi3h88IxkNaespD5kdTDuDGNTBrM,8039
 classiq/quantum_functions/decorators.py,sha256=eFLDllTUhGGFEQ_hM_gC8-7LTWP4N2zpyOKKBr_hT8A,232
 classiq/quantum_functions/function_library.py,sha256=w0mpypJcB6Id7z7jUqPW0gQQZ0TPfZrMm9LgRfIFeFE,3979
@@ -85,15 +85,15 @@
 classiq/interface/finance/function_input.py,sha256=6gwywV12pxIWhQiho3oRad_MJjbLY9R1tyzyyxtdQeE,2499
 classiq/interface/finance/gaussian_model_input.py,sha256=VOGb6FjT6bbjbJrOEuEaj4NLLTnv0oQtWQ5ADxRRZSQ,1261
 classiq/interface/finance/log_normal_model_input.py,sha256=FdvkT8Bx1XsnbVbEJHKIPr88Ok7T-C9_hwc_UByR8_k,912
 classiq/interface/finance/model_input.py,sha256=IkzishpQsCLvsC08YdP92BsB1Vz0fw5XEv4yGlHaiB8,474
 classiq/interface/generator/adjacency.py,sha256=Pi3zjPWCC33gUU_B3fRiNmpqK8wMze4AP6WVCVY8eY0,453
 classiq/interface/generator/amplitude_estimation.py,sha256=PbmCVS1dbi6wsLG5luKu2RZevkcX8ModZ29yy7fVH2Q,1562
 classiq/interface/generator/ansatz_library.py,sha256=f5Na1a8YBMZoapXBYPzZ2jU9A5a7jppJuBEUK0c7aoI,1342
-classiq/interface/generator/arith/arithmetic.py,sha256=wf-ZMQkmU4rGMjib4Tk7YA0dn4_IzfTc8JxRc7iHae8,4475
+classiq/interface/generator/arith/arithmetic.py,sha256=zRRg_5BFbhthpddCuVvezbP54TkcJpjkVQ0xue3OpOk,4525
 classiq/interface/generator/arith/binary_ops.py,sha256=qeyX97n9jQC7AK9T9NvDzCMik6Sz2PMMr-r14yFkRsY,6485
 classiq/interface/generator/arith/endianness.py,sha256=pVozR_jaNsrFOBn7cFbw5RjYToEZ2ozVvMTv0ruyUnQ,86
 classiq/interface/generator/arith/fix_point_number.py,sha256=jZ0OVXra6Ptd9OCCOPVspXox1hX445hCCDZQDzWcsaY,6827
 classiq/interface/generator/arith/logical_ops.py,sha256=pXN3EZENqiyK2DVcJFC0hoSW1LyLXp8sl1JEkFbpHi4,2543
 classiq/interface/generator/arith/register_user_input.py,sha256=_FCgb9YoMSdlcqOZklu_7dD6alNJBP1puv24IjPp6Y0,652
 classiq/interface/generator/arith/unary_ops.py,sha256=uUan1XMfosd_qbcIheRtrOPhO9IFOC0-w3ZtWBGbExw,986
 classiq/interface/generator/circuit_outline.py,sha256=w67uw-cQw5DlZBmzh2XC_Vi5yAvFWB2qxVLVrR2JHII,213
@@ -152,10 +152,10 @@
 classiq/interface/pyomo_extension/__init__.py,sha256=6AOCbixrKpzzZtHKpRfZx92PFb0Wkkc0JY_r5vbMy4Q,750
 classiq/interface/pyomo_extension/equality_expression.py,sha256=Kuj1uaCdEuDmiZ3Xl0_mYmBlTGzjIxEghwugrk6XTfc,56
 classiq/interface/pyomo_extension/inequality_expression.py,sha256=L_1Q3lHfAOROPh9hjpxyFrZZPRItPnpvXsjFmVrPjUE,58
 classiq/interface/pyomo_extension/set_pprint.py,sha256=UeUEHEgxZipDOspVaaLAbYmxnIdrhAasioo49xoTKS0,307
 classiq/interface/server/authentication.py,sha256=HS1AQuaNsAy5Vpb1hMejU2CutOB6UxO91GG5cO5vTF4,131
 classiq/interface/server/routes.py,sha256=tBRlpFrDC_ZaIX3AOE-uuCz48OZFWKmvBTWIagFS8Bk,1625
 classiq/interface/status.py,sha256=Kbpy9nv1pV-XlRbFf2Pjkvq_SkJTnGUKv8M0VGW3XpA,88
-classiq-0.9.1.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-classiq-0.9.1.dist-info/METADATA,sha256=iMWiKwRiy4jCaMVZSwK3p-wQWl6efaphkgJpxY6zaOE,2920
-classiq-0.9.1.dist-info/RECORD,,
+classiq-0.9.3.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+classiq-0.9.3.dist-info/METADATA,sha256=PE9yd4dgEDwtK7dN0WIYjco6K_DNGjPOwcIP0yBumjM,2920
+classiq-0.9.3.dist-info/RECORD,,
```
