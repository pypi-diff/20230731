# Comparing `tmp/redcat-0.0.6.tar.gz` & `tmp/redcat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.6.tar", max compression
+gzip compressed data, was "redcat-0.0.7.tar", max compression
```

## Comparing `redcat-0.0.6.tar` & `redcat-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0     1501 2023-06-24 23:40:47.361479 redcat-0.0.6/LICENSE
--rw-r--r--   0        0        0     2156 2023-06-24 23:40:47.361479 redcat-0.0.6/README.md
--rw-r--r--   0        0        0     4330 2023-06-24 23:40:47.361479 redcat-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      354 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/__init__.py
--rw-r--r--   0        0        0    18034 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/base.py
--rw-r--r--   0        0        0    17391 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/batchdict.py
--rw-r--r--   0        0        0     6733 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/batchlist.py
--rw-r--r--   0        0        0     2769 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/comparators.py
--rw-r--r--   0        0        0        0 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/__init__.py
--rw-r--r--   0        0        0      315 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/__init__.py
--rw-r--r--   0        0        0     4109 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/batching.py
--rw-r--r--   0        0        0     3764 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/joining.py
--rw-r--r--   0        0        0     2158 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/shuffling.py
--rw-r--r--   0        0        0   140507 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/tensor.py
--rw-r--r--   0        0        0    52673 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/tensorseq.py
--rw-r--r--   0        0        0        0 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/__init__.py
--rw-r--r--   0        0        0     1128 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/format.py
--rw-r--r--   0        0        0     1446 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/imports.py
--rw-r--r--   0        0        0    10148 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/tensor.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 redcat-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-31 14:56:36.999959 redcat-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2156 2023-07-31 14:56:36.999959 redcat-0.0.7/README.md
+-rw-r--r--   0        0        0     4363 2023-07-31 14:56:37.003959 redcat-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/__init__.py
+-rw-r--r--   0        0        0    18314 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/base.py
+-rw-r--r--   0        0        0    19152 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/batchdict.py
+-rw-r--r--   0        0        0     6954 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/batchlist.py
+-rw-r--r--   0        0        0     2879 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/comparators.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/datapipes/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     4118 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     3773 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/datapipes/iter/joining.py
+-rw-r--r--   0        0        0     2167 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0   146047 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/tensor.py
+-rw-r--r--   0        0        0    54549 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/utils/__init__.py
+-rw-r--r--   0        0        0    11060 2023-07-31 14:56:37.003959 redcat-0.0.7/src/redcat/utils/tensor.py
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 redcat-0.0.7/PKG-INFO
```

### Comparing `redcat-0.0.6/LICENSE` & `redcat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.6/README.md` & `redcat-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.6/pyproject.toml` & `redcat-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.6"
+version = "0.0.7"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
@@ -26,29 +26,31 @@
 
 packages = [
     { include = "redcat", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
-coola = ">=0.0.12,<1.0"
-numpy = ">=1.24,<2.0"
+coola = ">=0.0.15,<1.0"
+numpy = ">=1.20,<2.0"
 python = "^3.9"
-torch = ">=2.0.1,<3.0.0"
+torch = ">=2.0,<3.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3"
+black = "^23.7"
 coverage = { extras = ["toml"], version = "^7.2" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.3"
+pygments = "^2.15"
 pylint = "^2.17"
 pytest = "^7.3"
 pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = ">=0.0.275,<1.0"
+ruff = ">=0.0.280,<1.0"
+xdoctest = "^1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `redcat-0.0.6/src/redcat/base.py` & `redcat-0.0.7/src/redcat/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ###############################
 
     @abstractmethod
     def clone(self) -> TBatch:
         r"""Creates a copy of the current batch.
 
         Returns:
+        -------
             ``BaseBatch``: A copy of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -59,23 +60,25 @@
     @abstractmethod
     def allclose(
         self, other: Any, rtol: float = 1e-5, atol: float = 1e-8, equal_nan: bool = False
     ) -> bool:
         r"""Indicates if two batches are equal within a tolerance or not.
 
         Args:
+        ----
             other: Specifies the value to compare.
             rtol (float, optional): Specifies the relative tolerance
                 parameter. Default: ``1e-5``
             atol (float, optional): Specifies the absolute tolerance
                 parameter. Default: ``1e-8``
             equal_nan (bool, optional): If ``True``, then two ``NaN``s
                 will be considered equal. Default: ``False``
 
         Returns:
+        -------
             bool: ``True`` if the batches are equal within a tolerance,
                 ``False`` otherwise.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -88,17 +91,19 @@
         """
 
     @abstractmethod
     def equal(self, other: Any) -> bool:
         r"""Indicates if two batches are equal or not.
 
         Args:
+        ----
             other: Specifies the value to compare.
 
         Returns:
+        -------
             bool: ``True`` if the batches have the same size,
                 elements and same batch dimension, ``False`` otherwise.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -113,20 +118,22 @@
     ###########################################################
 
     @abstractmethod
     def permute_along_batch(self, permutation: Sequence[int] | Tensor) -> TBatch:
         r"""Permutes the data/batch along the batch dimension.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Returns:
+        -------
             ``BaseBatch``: A new batch with permuted data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -141,14 +148,15 @@
         """
 
     @abstractmethod
     def permute_along_batch_(self, permutation: Sequence[int] | Tensor) -> None:
         r"""Permutes the data/batch along the batch dimension.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Example usage:
 
@@ -166,59 +174,54 @@
                     [8, 9]], batch_dim=0)
         """
 
     def shuffle_along_batch(self, generator: torch.Generator | None = None) -> TBatch:
         r"""Shuffles the data/batch along the batch dimension.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Returns:
+        -------
             ``BaseBatch``:  A new batch with shuffled data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
-            >>> batch.shuffle_along_batch()
-            tensor([[4, 5],
-                    [2, 3],
-                    [6, 7],
-                    [0, 1],
-                    [8, 9]], batch_dim=0)
+            >>> batch.shuffle_along_batch()  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0)
         """
         return self.permute_along_batch(torch.randperm(self.batch_size, generator=generator))
 
     def shuffle_along_batch_(self, generator: torch.Generator | None = None) -> None:
         r"""Shuffles the data/batch along the batch dimension.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.shuffle_along_batch_()
-            >>> batch
-            tensor([[4, 5],
-                    [2, 3],
-                    [6, 7],
-                    [0, 1],
-                    [8, 9]], batch_dim=0)
+            >>> batch  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0)
         """
         self.permute_along_batch_(torch.randperm(self.batch_size, generator=generator))
 
     ################################################
     #     Mathematical | point-wise operations     #
     ################################################
 
@@ -232,14 +235,15 @@
 
     @abstractmethod
     def append(self, other: BaseBatch) -> None:
         r"""Appends a new batch to the current batch along the batch
         dimension.
 
         Args:
+        ----
             other (``TensorSeqBatch``): Specifies the batch to append
                 at the end of current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -256,21 +260,24 @@
         """
 
     @abstractmethod
     def chunk_along_batch(self, chunks: int) -> tuple[TBatch, ...]:
         r"""Splits the batch into chunks along the batch dimension.
 
         Args:
+        ----
             chunks (int): Specifies the number of chunks.
 
         Returns:
+        -------
             tuple: The batch split into chunks along the batch
                 dimension.
 
         Raises:
+        ------
             RuntimeError if the number of chunks is incorrect
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -291,45 +298,49 @@
         data as ``torch.Tensor`` by another batch representing data
         as ``torch.Tensor``, but it is usually not possible to extend
         a batch representing data ``torch.Tensor`` by a batch
         representing data with a dictionary. Please check each
         implementation to know the supported batch implementations.
 
         Args:
+        ----
             other (iterable): Specifies the batches to append to the
                 current batch.
 
         Raises:
+        ------
             TypeError: if there is no available implementation for the
                 input batch type.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.extend([BatchedTensor(torch.zeros(1, 3)), BatchedTensor(torch.full((1, 3), 2.0))])
-            >>> batch.data
+            >>> batch
             tensor([[1., 1., 1.],
                     [1., 1., 1.],
                     [0., 0., 0.],
                     [2., 2., 2.]], batch_dim=0)
         """
 
     @abstractmethod
     def index_select_along_batch(self, index: Tensor | Sequence[int]) -> BaseBatch:
         r"""Selects data at the given indices along the batch dimension.
 
         Args:
+        ----
             index (``torch.Tensor`` or list or tuple): Specifies the
                 indices to select.
 
         Returns:
+        -------
             ``BaseBatch``: A new batch which indexes ``self``
                 along the batch dimension using the entries in
                 ``index``.
 
         Example usage:
 
         .. code-block:: pycon
@@ -349,17 +360,19 @@
         """
 
     def select_along_batch(self, index: int) -> T:
         r"""Selects the batch along the batch dimension at the given
         index.
 
         Args:
+        ----
             index (int): Specifies the index to select.
 
         Returns:
+        -------
             ``BaseBatch``: The batch sliced along the batch
                 dimension at the given index.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -370,23 +383,25 @@
         """
 
     @abstractmethod
     def slice_along_batch(self, start: int = 0, stop: int | None = None, step: int = 1) -> TBatch:
         r"""Slices the batch in the batch dimension.
 
         Args:
+        ----
             start (int, optional): Specifies the index where the
                 slicing of object starts. Default: ``0``
             stop (int, optional): Specifies the index where the
                 slicing of object stops. ``None`` means last.
                 Default: ``None``
             step (int, optional): Specifies the increment between
                 each index for slicing. Default: ``1``
 
         Returns:
+        -------
             ``BaseBatch``: A slice of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -406,18 +421,20 @@
         """
 
     @abstractmethod
     def split_along_batch(self, split_size_or_sections: int | Sequence[int]) -> tuple[TBatch, ...]:
         r"""Splits the batch into chunks along the batch dimension.
 
         Args:
+        ----
             split_size_or_sections (int or sequence): Specifies the
                 size of a single chunk or list of sizes for each chunk.
 
         Returns:
+        -------
             tuple: The batch split into chunks along the batch
                 dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -433,21 +450,23 @@
     #     mini-batches     #
     ########################
 
     def get_num_minibatches(self, batch_size: int, drop_last: bool = False) -> int:
         r"""Gets the number of mini-batches for a given batch size.
 
         Args:
+        ----
             batch_size (int): Specifies the target batch size of the
                 mini-batches.
             drop_last (bool, optional): If ``True``, the last batch is
                 dropped if it is not full, otherwise it is returned.
                 Default: ``False``
 
         Returns:
+        -------
             int: The number of mini-batches.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -467,27 +486,29 @@
         batch_size: int,
         drop_last: bool = False,
         deepcopy: bool = False,
     ) -> Iterable[TBatch]:
         r"""Gets the mini-batches of the current batch.
 
         Args:
+        ----
             batch_size (int): Specifies the target batch size of the
                 mini-batches.
             drop_last (bool, optional): If ``True``, the last batch is
                 dropped if it is not full, otherwise it is returned.
                 Default: ``False``
             deepcopy (bool, optional): If ``True``, a deepcopy of the
                 batch is performed before to return the mini-batches.
                 If ``False``, each chunk is a view of the original
                 batch/tensor. Using deepcopy allows a deterministic
                 behavior when in-place operations are performed on the
                 data. Default: ``False``
 
         Returns:
+        -------
             iterable: The mini-batches.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -528,18 +549,20 @@
     #################
 
     @abstractmethod
     def summary(self) -> str:
         r"""Returns a summary of the current batch.
 
         Returns:
+        -------
             str: The summary of the current batch
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(20).view(10, 2)).summary()
-            'BatchedTensor(dtype=torch.int64, shape=torch.Size([2, 5]), device=cpu, batch_dim=0)'
+            >>> batch = BatchedTensor(torch.arange(20).view(10, 2))
+            >>> print(batch.summary())
+            BatchedTensor(dtype=torch.int64, shape=torch.Size([10, 2]), device=cpu, batch_dim=0)
         """
```

### Comparing `redcat-0.0.6/src/redcat/batchdict.py` & `redcat-0.0.7/src/redcat/batchdict.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,43 @@
     Sequence,
     ValuesView,
 )
 from typing import Any, TypeVar
 
 import torch
 from coola import objects_are_allclose, objects_are_equal
-from coola.utils.format import str_indent
+from coola.utils.format import str_indent, str_mapping
 from torch import Tensor
 
 from redcat.base import BaseBatch
-from redcat.utils.format import str_mapping
 
 # Workaround because Self is not available for python 3.9 and 3.10
 # https://peps.python.org/pep-0673/
 TBatchDict = TypeVar("TBatchDict", bound="BatchDict")
 
 
 class BatchDict(BaseBatch[dict[Hashable, BaseBatch]]):
     r"""Implements a batch object to represent a dictionary of batches.
 
     Args:
+    ----
         data (dict): Specifies the dictionary of batches.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
+        >>> batch = BatchDict(
+        ...     {
+        ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
+        ...         "key2": BatchList(["a", "b"]),
+        ...     }
+        ... )
     """
 
     def __init__(self, data: dict[Hashable, BaseBatch]) -> None:
         if not isinstance(data, dict):
             raise TypeError(f"Incorrect type. Expect a dict but received {type(data)}")
         check_same_batch_size(data)
         self._data = data
@@ -132,20 +145,22 @@
         method should be called only if all the sequences have the
         same length.
 
         This method only permutes the values that implement
         ``permute_along_seq``.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Returns:
+        -------
             ``BatchDict``: A new batch with permuted data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -154,17 +169,17 @@
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
             >>> batch.permute_along_seq([2, 1, 3, 0, 4])
             BatchDict(
-              (key1) tensor([[2, 1, 3, 0, 4],
+              (key1): tensor([[2, 1, 3, 0, 4],
                              [7, 6, 8, 5, 9]], batch_dim=0, seq_dim=1)
-              (key2) BatchList(data=['a', 'b'])
+              (key2): BatchList(data=['a', 'b'])
             )
         """
         out = {}
         for key, val in self._data.items():
             if hasattr(val, "permute_along_seq"):
                 val = val.permute_along_seq(permutation)
             out[key] = val
@@ -177,14 +192,15 @@
         method should be called only if all the sequences have the
         same length.
 
         This method only permutes the values that implement
         ``permute_along_seq``.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Example usage:
 
@@ -197,35 +213,37 @@
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
             >>> batch.permute_along_seq_([2, 1, 3, 0, 4])
             >>> batch
             BatchDict(
-              (key1) tensor([[2, 1, 3, 0, 4],
+              (key1): tensor([[2, 1, 3, 0, 4],
                              [7, 6, 8, 5, 9]], batch_dim=0, seq_dim=1)
-              (key2) BatchList(data=['a', 'b'])
+              (key2): BatchList(data=['a', 'b'])
             )
         """
         for val in self._data.values():
             if hasattr(val, "permute_along_seq_"):
                 val.permute_along_seq_(permutation)
 
     def shuffle_along_seq(self, generator: torch.Generator | None = None) -> TBatchDict:
         r"""Shuffles the data along the sequence dimension.
 
         This method should be called only if all the sequences have
         the same length.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Returns:
+        -------
             ``BatchDict``:  A new batch with shuffled data.
 
         Raises:
             RuntimeError if the batch has multiple sequence lengths.
 
         Example usage:
 
@@ -235,19 +253,18 @@
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> batch = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
-            >>> batch.shuffle_along_seq()
+            >>> batch.shuffle_along_seq()  # doctest:+ELLIPSIS
             BatchDict(
-              (key1) tensor([[2, 1, 3, 0, 4],
-                             [7, 6, 8, 5, 9]], batch_dim=0, seq_dim=1)
-              (key2) BatchList(data=['a', 'b'])
+              (key1): tensor([[...]], batch_dim=0, seq_dim=1)
+              (key2): BatchList(data=['a', 'b'])
             )
         """
         seq_lens = get_seq_lens(self._data)
         if not seq_lens:
             return self
         if len(seq_lens) > 1:
             raise RuntimeError(
@@ -258,19 +275,21 @@
     def shuffle_along_seq_(self, generator: torch.Generator | None = None) -> None:
         r"""Shuffles the data along the sequence dimension.
 
         This method should be called only if all the sequences have
         the same length.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Raises:
+        ------
             RuntimeError if the batch has multiple sequence lengths.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -278,19 +297,18 @@
             >>> batch = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
             >>> batch.shuffle_along_seq()
-            >>> batch
+            >>> batch  # doctest:+ELLIPSIS
             BatchDict(
-              (key1) tensor([[2, 1, 3, 0, 4],
-                             [7, 6, 8, 5, 9]], batch_dim=0, seq_dim=1)
-              (key2) BatchList(data=['a', 'b'])
+              (key1): tensor([[...]], batch_dim=0, seq_dim=1)
+              (key2): BatchList(data=['a', 'b'])
             )
         """
         seq_lens = get_seq_lens(self._data)
         if not seq_lens:
             return
         if len(seq_lens) > 1:
             raise RuntimeError(
@@ -318,18 +336,20 @@
     def cat_along_seq(self, batches: BatchDict | Sequence[BatchDict]) -> TBatchDict:
         r"""Concatenates the data of the batch(es) to the current batch
         along the sequence dimension and creates a new batch.
 
         Note that only the sequences are concatenated.
 
         Args:
+        ----
             batches (``BatchDict`` or  ``Sequence``): Specifies the
                 batch(es) to concatenate along the sequence dimension.
 
         Returns:
+        -------
             ``BatchDict``: A batch with the concatenated data
                 along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -341,17 +361,17 @@
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
             >>> b.cat_along_seq(
             ...     BatchDict({"key1": BatchedTensorSeq(torch.tensor([[10, 11, 12], [20, 21, 22]]))})
             ... )
             BatchDict(
-              (key1) tensor([[ 0,  1,  2,  3,  4, 10, 11, 12],
-                             [ 5,  6,  7,  8,  9, 20, 21, 22]], batch_dim=0, seq_dim=1)
-              (key2) BatchList(data=['a', 'b'])
+              (key1): tensor([[ 0,  1,  2,  3,  4, 10, 11, 12],
+                        [ 5,  6,  7,  8,  9, 20, 21, 22]], batch_dim=0, seq_dim=1)
+              (key2): BatchList(data=['a', 'b'])
             )
         """
         if isinstance(batches, BatchDict):
             batches = [batches]
         out = {}
         for key, val in self._data.items():
             if hasattr(val, "cat_along_seq"):
@@ -362,14 +382,15 @@
     def cat_along_seq_(self, batches: BatchDict | Sequence[BatchDict]) -> None:
         r"""Concatenates the data of the batch(es) to the current batch
         along the sequence dimension and creates a new batch.
 
         Note that only the sequences are concatenated.
 
         Args:
+        ----
             batches (``BatchDict`` or  ``Sequence``): Specifies the
                 batch(es) to concatenate along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -382,17 +403,17 @@
             ...     }
             ... )
             >>> b.cat_along_seq_(
             ...     BatchDict({"key1": BatchedTensorSeq(torch.tensor([[10, 11, 12], [20, 21, 22]]))})
             ... )
             >>> b
             BatchDict(
-              (key1) tensor([[ 0,  1,  2,  3,  4, 10, 11, 12],
-                             [ 5,  6,  7,  8,  9, 20, 21, 22]], batch_dim=0, seq_dim=1)
-              (key2) BatchList(data=['a', 'b'])
+              (key1): tensor([[ 0,  1,  2,  3,  4, 10, 11, 12],
+                        [ 5,  6,  7,  8,  9, 20, 21, 22]], batch_dim=0, seq_dim=1)
+              (key2): BatchList(data=['a', 'b'])
             )
         """
         if isinstance(batches, BatchDict):
             batches = [batches]
         for key, val in self._data.items():
             if hasattr(val, "cat_along_seq_"):
                 val.cat_along_seq_([batch[key] for batch in batches])
@@ -448,19 +469,34 @@
 
 
 def check_same_batch_size(data: dict[Hashable, BaseBatch]) -> None:
     r"""Checks if the all the batches in a group have the same batch
     size.
 
     Args:
+    ----
         group (``BaseBatch`` or dict or sequence): Specifies the group
             of batches to check.
 
     Raises:
+    ------
         RuntimeError if there are several batch sizes.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat import BatchedTensor, BatchedTensorSeq
+        >>> from redcat.batchdict import check_same_batch_size
+        >>> check_same_batch_size(
+        ...     {
+        ...         "key1": BatchedTensorSeq(torch.ones(2, 3)),
+        ...         "key2": BatchedTensor(torch.ones(2, 6)),
+        ...     }
+        ... )
     """
     if not data:
         raise RuntimeError("The dictionary cannot be empty")
     batch_sizes = {val.batch_size for val in data.values()}
     if len(batch_sizes) != 1:
         raise RuntimeError(
             "Incorrect batch size. A single batch size is expected but received several values: "
@@ -468,29 +504,64 @@
         )
 
 
 def check_same_keys(data1: dict, data2: dict) -> None:
     r"""Checks if the dictionaries have the same keys.
 
     Args:
+    ----
         data1 (dict): Specifies the first dictionary.
         data2 (dict): Specifies the second dictionary.
 
     Raises:
+    ------
         RuntimeError if the keys are different.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat import BatchedTensor, BatchedTensorSeq
+        >>> from redcat.batchdict import check_same_keys
+        >>> check_same_keys(
+        ...     {
+        ...         "key1": BatchedTensorSeq(torch.ones(2, 3)),
+        ...         "key2": BatchedTensor(torch.ones(2, 6)),
+        ...     },
+        ...     {
+        ...         "key1": BatchedTensorSeq(torch.zeros(2, 4)),
+        ...         "key2": BatchedTensor(torch.zeros(2, 4)),
+        ...     },
+        ... )
     """
     keys1 = set(data1.keys())
     keys2 = set(data2.keys())
     if keys1 != keys2:
         raise RuntimeError(f"Keys do not match: ({keys1} vs {keys2})")
 
 
 def get_seq_lens(data: dict[Hashable, BaseBatch]) -> set[int]:
     r"""Gets the sequence lengths from the inputs.
 
     Args:
+    ----
         data (dict): Specifies the data with the sequences.
 
     Returns:
+    -------
         set: The sequence lengths.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat import BatchedTensor, BatchedTensorSeq
+        >>> from redcat.batchdict import get_seq_lens
+        >>> get_seq_lens(
+        ...     {
+        ...         "key1": BatchedTensorSeq(torch.ones(2, 3)),
+        ...         "key2": BatchedTensor(torch.ones(2, 6)),
+        ...     }
+        ... )
+        {3}
     """
     return {val.seq_len for val in data.values() if hasattr(val, "seq_len")}
```

### Comparing `redcat-0.0.6/src/redcat/batchlist.py` & `redcat-0.0.7/src/redcat/batchlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,27 @@
 
 
 class BatchList(BaseBatch[list[T]]):
     r"""Implements a batch object to easily manipulate a list of
     examples.
 
     Args:
+    ----
         data (list): Specifies the list of examples.
+
+    Raises:
+    ------
+        TypeError if the input is not a list.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat import BatchList
+        >>> batch = BatchList([1, 2, 3])
     """
 
     def __init__(self, data: list[T]) -> None:
         if not isinstance(data, list):
             raise TypeError(f"Incorrect type. Expect a list but received {type(data)}")
         self._data = data
 
@@ -146,50 +158,54 @@
     #################
 
     def apply(self, fn: Callable[[T], T]) -> TBatchList:
         r"""Apply a function to transform the element in the list of the
         current batch.
 
         Args:
+        ----
             fn (``Callable``): Specifies the function to be applied to
                 the element in the list. It is the responsibility of
                 the user to verify the function applies a valid
                 transformation of the data.
 
         Returns:
-            ``BatchedTensor``: The transformed batch.
+        -------
+            ``BatchList``: The transformed batch.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> import torch
+
             >>> from redcat import BatchList
-            >>> BatchList([1, 2, 3]).apply(lambda val: val + 2)
+            >>> batch = BatchList([1, 2, 3])
+            >>> batch.apply(lambda val: val + 2)
             BatchList(data=[3, 4, 5])
         """
         return self._create_new_batch([fn(val) for val in self._data])
 
     def apply_(self, fn: Callable[[T], T]) -> None:
         r"""Apply a function to transform the element in the list of the
         current batch.
 
         In-place version of ``apply``.
 
         Args:
+        ----
             fn (``Callable``): Specifies the function to be applied to
                 the element in the list. It is the responsibility of
                 the user to verify the function applies a valid
                 transformation of the data.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> import torch
+
             >>> from redcat import BatchList
             >>> batch = BatchList([1, 2, 3])
             >>> batch.apply_(lambda val: val + 2)
             >>> batch
             BatchList(data=[3, 4, 5])
         """
         self._data = [fn(val) for val in self._data]
```

### Comparing `redcat-0.0.6/src/redcat/comparators.py` & `redcat-0.0.7/src/redcat/comparators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-r"""This module implements some comparators to use ``BaseBatch`` objects with
-``coola.objects_are_equal`` and ``coola.objects_are_allclose``."""
+r"""This module implements some comparators to use ``BaseBatch`` objects
+with ``coola.objects_are_equal`` and ``coola.objects_are_allclose``."""
 from __future__ import annotations
 
 __all__ = ["BatchEqualityOperator", "BatchAllCloseOperator"]
 
 import logging
 from typing import Any
 
@@ -33,14 +33,16 @@
         object1: BaseBatch,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not isinstance(object2, BaseBatch):
             if show_difference:
                 logger.info(f"object2 is not a `BaseBatch` object: {type(object2)}")
             return False
         object_equal = object1.allclose(object2, rtol=rtol, atol=atol, equal_nan=equal_nan)
         if show_difference and not object_equal:
             logger.info(
@@ -64,14 +66,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: BaseBatch,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not isinstance(object2, BaseBatch):
             if show_difference:
                 logger.info(f"object2 is not a `BaseBatch` object: {type(object2)}")
             return False
         object_equal = object1.equal(object2)
         if show_difference and not object_equal:
             logger.info(
```

### Comparing `redcat-0.0.6/src/redcat/datapipes/iter/batching.py` & `redcat-0.0.7/src/redcat/datapipes/iter/batching.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 class MiniBatcherIterDataPipe(IterDataPipe[BaseBatch[T]]):
     r"""Implements a DataPipe to generate mini-batches from a batch
     (``BaseBatch`` object).
 
     Args:
+    ----
         datapipe_or_batch (``IterDataPipe`` or ``BaseBatch``):
             Specifies the datapipe of batches to split.
             The generated mini-batches have the same structure
             as the input batches.
         batch_size (int): Specifies the batch size.
         shuffle (bool, optional): If ``True``, the batches are
             shuffled before to create the mini-batches. The
@@ -104,10 +105,10 @@
     @property
     def batch_size(self) -> int:
         r"""``int``: The batch size."""
         return self._batch_size
 
     @property
     def random_seed(self) -> int:
-        r"""``int``: The random seed used to initialize the pseudo random
-        generator."""
+        r"""``int``: The random seed used to initialize the pseudo
+        random generator."""
         return self._generator.initial_seed()
```

### Comparing `redcat-0.0.6/src/redcat/datapipes/iter/joining.py` & `redcat-0.0.7/src/redcat/datapipes/iter/joining.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class BatchExtenderIterDataPipe(IterDataPipe[BaseBatch[T]]):
-    r"""Implements a DataPipe to combine several ``BaseBatch`` object into a
-    single ``BaseBatch`` object.
+    r"""Implements a DataPipe to combine several ``BaseBatch`` object
+    into a single ``BaseBatch`` object.
 
     Args:
+    ----
         datapipe (``IterDataPipe``): Specifies the source
             DataPipe. The DataPipe has to return compatible
             ``BaseBatch`` objects.
         buffer_size (int, optional): Specifies the buffer size i.e.
             the number of batches that are combined into a bigger
             batch. Default: ``10``
         drop_last (bool, optional): If ``True``, the last samples are
```

### Comparing `redcat-0.0.6/src/redcat/datapipes/iter/shuffling.py` & `redcat-0.0.7/src/redcat/datapipes/iter/shuffling.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 T = TypeVar("T")
 
 
 class BatchShufflerIterDataPipe(IterDataPipe[BaseBatch[T]]):
     r"""Implements a DataPipe to shuffle data in ``BaseBatch`` objects.
 
     Args:
+    ----
         datapipe (``IterDataPipe``): Specifies the source DataPipe.
             The DataPipe has to return ``BaseBatch`` objects.
         random_seed (int, optional): Specifies the random seed used
             to shuffle the data. Default: ``3770589329299158004``
 
     Example usage:
 
@@ -61,10 +62,10 @@
             f"{self.__class__.__qualname__}(\n"
             f"  random_seed={self.random_seed},\n"
             f"  datapipe={str_indent(self._datapipe)},\n)"
         )
 
     @property
     def random_seed(self) -> int:
-        r"""``int``: The random seed used to initialize the pseudo random
-        generator."""
+        r"""``int``: The random seed used to initialize the pseudo
+        random generator."""
         return self._generator.initial_seed()
```

### Comparing `redcat-0.0.6/src/redcat/tensor.py` & `redcat-0.0.7/src/redcat/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,30 @@
 
 
 class BatchedTensor(BaseBatch[Tensor]):
     r"""Implements a batched tensor to easily manipulate a batch of
     examples.
 
     Args:
+    ----
         data (array_like): Specifies the data for the tensor. It can
             be a torch.Tensor, list, tuple, NumPy ndarray, scalar,
             and other types.
         batch_dim (int, optional): Specifies the batch dimension
             in the ``torch.Tensor`` object. Default: ``0``
         kwargs: Keyword arguments that are passed to
             ``torch.as_tensor``.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat import BatchedTensor
+        >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
     """
 
     def __init__(self, data: Any, *, batch_dim: int = 0, **kwargs) -> None:
         super().__init__()
         self._data = torch.as_tensor(data, **kwargs)
         check_data_and_dim(self._data, batch_dim)
         self._batch_dim = int(batch_dim)
@@ -75,88 +84,97 @@
     @property
     def data(self) -> Tensor:
         r"""``torch.Tensor``: The data in the batch."""
         return self._data
 
     @property
     def device(self) -> torch.device:
-        r"""``torch.device``: The device where the batch data/tensor is."""
+        r"""``torch.device``: The device where the batch data/tensor
+        is."""
         return self._data.device
 
     @property
     def shape(self) -> torch.Size:
         r"""``torch.Size``: The shape of the tensor."""
         return self._data.shape
 
     def dim(self) -> int:
         r"""Gets the number of dimensions.
 
         Returns:
+        -------
             int: The number of dimensions
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.ones(2, 3)).dim()
+            >>> batch = BatchedTensor(torch.ones(2, 3))
+            >>> batch.dim()
             2
         """
         return self._data.dim()
 
     def ndimension(self) -> int:
         r"""Gets the number of dimensions.
 
         Returns:
+        -------
             int: The number of dimensions
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.ones(2, 3)).ndimension()
+            >>> batch = BatchedTensor(torch.ones(2, 3))
+            >>> batch.ndimension()
             2
         """
         return self.dim()
 
     def numel(self) -> int:
         r"""Gets the total number of elements in the tensor.
 
         Returns:
+        -------
             int: The total number of elements
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.ones(2, 3)).numel()
+            >>> batch = BatchedTensor(torch.ones(2, 3))
+            >>> batch.numel()
             6
         """
         return self._data.numel()
 
     #################################
     #     Conversion operations     #
     #################################
 
     def contiguous(
         self, memory_format: torch.memory_format = torch.contiguous_format
     ) -> TBatchedTensor:
         r"""Creates a batch with a contiguous representation of the data.
 
         Args:
+        ----
             memory_format (``torch.memory_format``, optional):
                 Specifies the desired memory format.
                 Default: ``torch.contiguous_format``
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with a contiguous
                 representation of the data.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -169,71 +187,76 @@
         return self._create_new_batch(self._data.contiguous(memory_format=memory_format))
 
     def is_contiguous(self, memory_format: torch.memory_format = torch.contiguous_format) -> bool:
         r"""Indicates if a batch as a contiguous representation of the
         data.
 
         Args:
+        ----
             memory_format (``torch.memory_format``, optional):
                 Specifies the desired memory format.
                 Default: ``torch.contiguous_format``
 
         Returns:
+        -------
             bool: ``True`` if the data are stored with a contiguous
                 tensor, otherwise ``False``.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.ones(2, 3)).is_contiguous()
+            >>> batch = BatchedTensor(torch.ones(2, 3))
+            >>> batch.is_contiguous()
             True
         """
         return self._data.is_contiguous(memory_format=memory_format)
 
     def to(self, *args, **kwargs) -> TBatchedTensor:
         r"""Moves and/or casts the data.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.to``
             **kwargs: See the documentation of ``torch.Tensor.to``
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with the data after
                 dtype and/or device conversion.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
-            >>> batch_cuda = batch.to(device=torch.device("cuda:0"))
-            >>> batch_bool = batch.to(dtype=torch.bool)
-            >>> batch_bool
+            >>> batch.to(dtype=torch.bool)
             tensor([[True, True, True],
                     [True, True, True]], batch_dim=0)
         """
         return self._create_new_batch(self._data.to(*args, **kwargs))
 
     ###############################
     #     Creation operations     #
     ###############################
 
     def clone(self, *args, **kwargs) -> TBatchedTensor:
         r"""Creates a copy of the current batch.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.clone``
             **kwargs: See the documentation of ``torch.Tensor.clone``
 
         Returns:
+        -------
             ``BatchedTensor``: A copy of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -247,45 +270,48 @@
         return self._create_new_batch(self._data.clone(*args, **kwargs))
 
     def empty_like(self, *args, **kwargs) -> TBatchedTensor:
         r"""Creates an uninitialized batch, with the same shape as the
         current batch.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.empty_like``
             **kwargs: See the documentation of
                 ``torch.Tensor.empty_like``
 
         Returns:
+        -------
             ``BatchedTensor``: A uninitialized batch with the same
                 shape as the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
-            >>> batch.empty_like(42)
-            tensor([[0., 0., 0.],
-                    [0., 0., 0.]], batch_dim=0)
+            >>> batch.empty_like()  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0)
         """
         return self._create_new_batch(torch.empty_like(self._data, *args, **kwargs))
 
     def full_like(self, *args, **kwargs) -> TBatchedTensor:
         r"""Creates a batch filled with a given scalar value, with the
         same shape as the current batch.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.full_like``
             **kwargs: See the documentation of
                 ``torch.Tensor.full_like``
 
         Returns:
+        -------
             ``BatchedTensor``: A batch filled with the scalar
                 value, with the same shape as the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -307,23 +333,25 @@
         r"""Creates a batch filled with a scalar value.
 
         By default, the tensor in the returned batch has the same
         shape, ``torch.dtype`` and ``torch.device`` as the tensor in
         the current batch.
 
         Args:
+        ----
             fill_value (float or int or bool): Specifies the number
                 to fill the batch with.
             batch_size (int or ``None``): Specifies the batch size.
                 If ``None``, the batch size of the current batch is
                 used. Default: ``None``.
             **kwargs: See the documentation of
                 ``torch.Tensor.new_full``.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch filled with the scalar value.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -354,21 +382,23 @@
         r"""Creates a batch filled with the scalar value ``1``.
 
         By default, the tensor in the returned batch has the same
         shape, ``torch.dtype`` and ``torch.device`` as the tensor in
         the current batch.
 
         Args:
+        ----
             batch_size (int or ``None``): Specifies the batch size.
                 If ``None``, the batch size of the current batch is
                 used. Default: ``None``.
             **kwargs: See the documentation of
                 ``torch.Tensor.new_ones``.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch filled with the scalar
                 value ``1``.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -400,21 +430,23 @@
         r"""Creates a batch filled with the scalar value ``0``.
 
         By default, the tensor in the returned batch has the same
         shape, ``torch.dtype`` and ``torch.device`` as the tensor
         in the current batch.
 
         Args:
+        ----
             batch_size (int or ``None``): Specifies the batch size.
                 If ``None``, the batch size of the current batch is
                 used. Default: ``None``.
             **kwargs: See the documentation of
                 ``torch.Tensor.new_zeros``.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch filled with the scalar
                 value ``0``.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -435,23 +467,25 @@
         if batch_size is not None:
             shape[self._batch_dim] = batch_size
         kwargs["dtype"] = kwargs.get("dtype", self.dtype)
         kwargs["device"] = kwargs.get("device", self.device)
         return self._create_new_batch(torch.zeros(*shape, **kwargs))
 
     def ones_like(self, *args, **kwargs) -> TBatchedTensor:
-        r"""Creates a batch filled with the scalar value ``1``, with the same
-        shape as the current batch.
+        r"""Creates a batch filled with the scalar value ``1``, with the
+        same shape as the current batch.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.ones_like``
             **kwargs: See the documentation of
                 ``torch.Tensor.ones_like``
 
         Returns:
+        -------
             ``BatchedTensor``: A batch filled with the scalar
                 value ``1``, with the same shape as the current
                 batch.
 
         Example usage:
 
         .. code-block:: pycon
@@ -462,23 +496,25 @@
             >>> batch.ones_like()
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=0)
         """
         return self._create_new_batch(torch.ones_like(self._data, *args, **kwargs))
 
     def zeros_like(self, *args, **kwargs) -> TBatchedTensor:
-        r"""Creates a batch filled with the scalar value ``0``, with the same
-        shape as the current batch.
+        r"""Creates a batch filled with the scalar value ``0``, with the
+        same shape as the current batch.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.zeros_like``
             **kwargs: See the documentation of
                 ``torch.Tensor.zeros_like``
 
         Returns:
+        -------
             ``BatchedTensor``: A batch filled with the scalar
                 value ``0``, with the same shape as the current
                 batch.
 
         Example usage:
 
         .. code-block:: pycon
@@ -522,17 +558,19 @@
             return False
         return self._data.allclose(other.data, rtol=rtol, atol=atol, equal_nan=equal_nan)
 
     def eq(self, other: BatchedTensor | Tensor | bool | int | float) -> TBatchedTensor:
         r"""Computes element-wise equality.
 
         Args:
+        ----
             other: Specifies the batch to compare.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 equality.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -559,18 +597,20 @@
             return False
         return self._data.equal(other.data)
 
     def ge(self, other: BatchedTensor | Tensor | bool | int | float) -> TBatchedTensor:
         r"""Computes ``self >= other`` element-wise.
 
         Args:
+        ----
             other: Specifies the value to compare
                 with.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -590,17 +630,19 @@
         """
         return torch.ge(self, other)
 
     def gt(self, other: BatchedTensor | Tensor | bool | int | float) -> TBatchedTensor:
         r"""Computes ``self > other`` element-wise.
 
         Args:
+        ----
             other: Specifies the batch to compare.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -621,14 +663,15 @@
         return torch.gt(self, other)
 
     def isinf(self) -> TBatchedTensor:
         r"""Indicates if each element of the batch is infinite (positive
         or negative infinity) or not.
 
         Returns:
+        -------
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is infinite
                 and ``False`` elsewhere.
 
         Example usage:
 
         .. code-block:: pycon
@@ -645,14 +688,15 @@
         return torch.isinf(self)
 
     def isneginf(self) -> TBatchedTensor:
         r"""Indicates if each element of the batch is negative infinity
         or not.
 
         Returns:
+        -------
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is negative
                 infinity and ``False`` elsewhere.
 
         Example usage:
 
         .. code-block:: pycon
@@ -669,14 +713,15 @@
         return torch.isneginf(self)
 
     def isposinf(self) -> TBatchedTensor:
         r"""Indicates if each element of the batch is positive infinity
         or not.
 
         Returns:
+        -------
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is positive
                 infinity and ``False`` elsewhere.
 
         Example usage:
 
         .. code-block:: pycon
@@ -692,14 +737,15 @@
         """
         return torch.isposinf(self)
 
     def isnan(self) -> TBatchedTensor:
         r"""Indicates if each element in the batch is NaN or not.
 
         Returns:
+        -------
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is infinite
                 and ``False`` elsewhere.
 
         Example usage:
 
         .. code-block:: pycon
@@ -715,17 +761,19 @@
         """
         return torch.isnan(self)
 
     def le(self, other: BatchedTensor | Tensor | bool | int | float) -> TBatchedTensor:
         r"""Computes ``self <= other`` element-wise.
 
         Args:
+        ----
             other: Specifies the batch to compare.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -745,17 +793,19 @@
         """
         return torch.le(self, other)
 
     def lt(self, other: BatchedTensor | Tensor | bool | int | float) -> TBatchedTensor:
         r"""Computes ``self < other`` element-wise.
 
         Args:
+        ----
             other: Specifies the batch to compare.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -784,14 +834,15 @@
         r"""``torch.dtype``: The data type."""
         return self._data.dtype
 
     def bool(self) -> TBatchedTensor:
         r"""Converts the current batch to bool data type.
 
         Returns:
+        -------
             ``BatchedTensor``: The current batch to bool data type.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -802,14 +853,15 @@
         """
         return self._create_new_batch(self._data.bool())
 
     def double(self) -> TBatchedTensor:
         r"""Converts the current batch to double data type.
 
         Returns:
+        -------
             ``BatchedTensor``: The current batch to double data type.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -820,14 +872,15 @@
         """
         return self._create_new_batch(self._data.double())
 
     def float(self) -> TBatchedTensor:
         r"""Converts the current batch to float data type.
 
         Returns:
+        -------
             ``BatchedTensor``: The current batch to float data type.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -838,14 +891,15 @@
         """
         return self._create_new_batch(self._data.float())
 
     def int(self) -> TBatchedTensor:
         r"""Converts the current batch to int data type.
 
         Returns:
+        -------
             ``BatchedTensor``: The current batch to int data type.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -856,14 +910,15 @@
         """
         return self._create_new_batch(self._data.int())
 
     def long(self) -> TBatchedTensor:
         r"""Converts the current batch to long data type.
 
         Returns:
+        -------
             ``BatchedTensor``: The current batch to long data type.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -910,27 +965,29 @@
         return self
 
     def add(
         self,
         other: BatchedTensor | Tensor | int | float,
         alpha: int | float = 1.0,
     ) -> TBatchedTensor:
-        r"""Adds the input ``other``, scaled by ``alpha``, to the ``self``
-        batch.
+        r"""Adds the input ``other``, scaled by ``alpha``, to the
+        ``self`` batch.
 
         Similar to ``out = self + alpha * other``
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the other value to add to the
                 current batch.
             alpha (int or float, optional): Specifies the scale of the
                 batch to add. Default: ``1.0``
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch containing the addition of
                 the two batches.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -948,20 +1005,21 @@
         return torch.add(self, other, alpha=alpha)
 
     def add_(
         self,
         other: BatchedTensor | Tensor | int | float,
         alpha: int | float = 1.0,
     ) -> None:
-        r"""Adds the input ``other``, scaled by ``alpha``, to the ``self``
-        batch.
+        r"""Adds the input ``other``, scaled by ``alpha``, to the
+        ``self`` batch.
 
         Similar to ``self += alpha * other`` (in-place)
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the other value to add to the
                 current batch.
             alpha (int or float, optional): Specifies the scale of the
                 batch to add. Default: ``1.0``
 
         Example usage:
@@ -985,25 +1043,27 @@
         rounding_mode: str | None = None,
     ) -> TBatchedTensor:
         r"""Divides the ``self`` batch by the input ``other`.
 
         Similar to ``out = self / other``
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the dividend.
             rounding_mode (str or ``None``, optional): Specifies the
                 type of rounding applied to the result.
                 - ``None``: true division.
                 - ``"trunc"``: rounds the results of the division
                     towards zero.
                 - ``"floor"``: floor division.
                 Default: ``None``
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch containing the division
                 of the two batches.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1026,14 +1086,15 @@
         rounding_mode: str | None = None,
     ) -> None:
         r"""Divides the ``self`` batch by the input ``other`.
 
         Similar to ``self /= other`` (in-place)
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the dividend.
             rounding_mode (str or ``None``, optional): Specifies the
                 type of rounding applied to the result.
                 - ``None``: true division.
                 - ``"trunc"``: rounds the results of the division
                     towards zero.
@@ -1060,18 +1121,20 @@
         divisor: BatchedTensor | Tensor | int | float,
     ) -> TBatchedTensor:
         r"""Computes the element-wise remainder of division.
 
         The current batch is the dividend.
 
         Args:
+        ----
             divisor (``BatchedTensor`` or ``torch.Tensor`` or int
                 or float): Specifies the divisor.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch containing the
                 element-wise remainder of division.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1090,14 +1153,15 @@
 
     def fmod_(self, divisor: BatchedTensor | Tensor | int | float) -> None:
         r"""Computes the element-wise remainder of division.
 
         The current batch is the dividend.
 
         Args:
+        ----
             divisor (``BatchedTensor`` or ``torch.Tensor`` or int
                 or float): Specifies the divisor.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1114,18 +1178,20 @@
 
     def mul(self, other: BatchedTensor | Tensor | int | float) -> TBatchedTensor:
         r"""Multiplies the ``self`` batch by the input ``other`.
 
         Similar to ``out = self * other``
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the value to multiply.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch containing the
                 multiplication of the two batches.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1144,18 +1210,20 @@
 
     def mul_(self, other: BatchedTensor | Tensor | int | float) -> None:
         r"""Multiplies the ``self`` batch by the input ``other`.
 
         Similar to ``self *= other`` (in-place)
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the value to multiply.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch containing the
                 multiplication of the two batches.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1170,14 +1238,15 @@
         check_batch_dims(get_batch_dims((self, other)))
         self._data.mul_(other)
 
     def neg(self) -> TBatchedTensor:
         r"""Returns a new batch with the negative of the elements.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with the negative of
                 the elements.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1195,26 +1264,28 @@
         return torch.neg(self)
 
     def sub(
         self,
         other: BatchedTensor | Tensor | int | float,
         alpha: int | float = 1,
     ) -> TBatchedTensor:
-        r"""Subtracts the input ``other``, scaled by ``alpha``, to the ``self``
-        batch.
+        r"""Subtracts the input ``other``, scaled by ``alpha``, to the
+        ``self`` batch.
 
         Similar to ``out = self - alpha * other``
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the value to subtract.
             alpha (int or float, optional): Specifies the scale of the
                 batch to substract. Default: ``1``
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch containing the diffence of
                 the two batches.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1232,20 +1303,21 @@
         return torch.sub(self, other, alpha=alpha)
 
     def sub_(
         self,
         other: BatchedTensor | Tensor | int | float,
         alpha: int | float = 1,
     ) -> None:
-        r"""Subtracts the input ``other``, scaled by ``alpha``, to the ``self``
-        batch.
+        r"""Subtracts the input ``other``, scaled by ``alpha``, to the
+        ``self`` batch.
 
         Similar to ``self -= alpha * other`` (in-place)
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the value to subtract.
             alpha (int or float, optional): Specifies the scale of the
                 batch to substract. Default: ``1``
 
         Example usage:
 
@@ -1267,73 +1339,80 @@
     ###########################################################
 
     def cumsum(self, dim: int, **kwargs) -> TBatchedTensor:
         r"""Computes the cumulative sum of elements of the current batch
         in a given dimension.
 
         Args:
+        ----
             dim (int): Specifies the dimension of the cumulative sum.
             **kwargs: see ``torch.cumsum`` documentation
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with the cumulative sum of
                 elements of the current batch in a given dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).cumsum(dim=1)
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.cumsum(dim=0)
             tensor([[ 0,  1,  2,  3,  4],
                     [ 5,  7,  9, 11, 13]], batch_dim=0)
         """
         return torch.cumsum(self, dim=dim, **kwargs)
 
     def cumsum_(self, dim: int, **kwargs) -> None:
         r"""Computes the cumulative sum of elements of the current batch
         in a given dimension.
 
         Args:
+        ----
             dim (int): Specifies the dimension of the cumulative sum.
             **kwargs: see ``torch.cumsum_`` documentation
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
-            >>> batch.cumsum_(dim=1)
+            >>> batch.cumsum_(dim=0)
             >>> batch
             tensor([[ 0,  1,  2,  3,  4],
                     [ 5,  7,  9, 11, 13]], batch_dim=0)
         """
         self._data.cumsum_(dim=dim, **kwargs)
 
     def cumsum_along_batch(self, **kwargs) -> TBatchedTensor:
         r"""Computes the cumulative sum of elements of the current batch
         in the batch dimension.
 
         Args:
+        ----
             **kwargs: see ``torch.cumsum`` documentation
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with the cumulative sum of
                 elements of the current batch in the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).cumsum_along_batch()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.cumsum_along_batch()
             tensor([[ 0,  1,  2,  3,  4],
                     [ 5,  7,  9, 11, 13]], batch_dim=0)
         """
         return self.cumsum(self._batch_dim, **kwargs)
 
     def cumsum_along_batch_(self) -> None:
         r"""Computes the cumulative sum of elements of the current batch
@@ -1355,39 +1434,43 @@
 
     def logcumsumexp(self, dim: int) -> TBatchedTensor:
         r"""Computes the logarithm of the cumulative summation of the
         exponentiation of elements of the current batch in a given
         dimension.
 
         Args:
+        ----
             dim (int): Specifies the dimension of the cumulative sum.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with the cumulative
                 summation of the exponentiation of elements of the
                 current batch in a given dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).logcumsumexp(dim=1)
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5).float())
+            >>> batch.logcumsumexp(dim=1)
             tensor([[0.0000, 1.3133, 2.4076, 3.4402, 4.4519],
                     [5.0000, 6.3133, 7.4076, 8.4402, 9.4519]], batch_dim=0)
         """
         return torch.logcumsumexp(self, dim=dim)
 
     def logcumsumexp_(self, dim: int) -> None:
         r"""Computes the logarithm of the cumulative summation of the
         exponentiation of elements of the current batch in a given
         dimension.
 
         Args:
+        ----
             dim (int): Specifies the dimension of the cumulative sum.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -1402,25 +1485,27 @@
 
     def logcumsumexp_along_batch(self) -> TBatchedTensor:
         r"""Computes the logarithm of the cumulative summation of the
         exponentiation of elements of the current batch in the batch
         dimension.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with the cumulative
                 summation of the exponentiation of elements of the
                 current batch in the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).logcumsumexp_along_batch()
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2).float())
+            >>> batch.logcumsumexp_along_batch()
             tensor([[0.0000, 1.0000],
                     [2.1269, 3.1269],
                     [4.1429, 5.1429],
                     [6.1451, 7.1451],
                     [8.1454, 9.1454]], batch_dim=0)
         """
         return self.logcumsumexp(self._batch_dim)
@@ -1453,31 +1538,34 @@
     def permute_along_batch_(self, permutation: Sequence[int] | Tensor) -> None:
         self.permute_along_dim_(permutation, dim=self._batch_dim)
 
     def permute_along_dim(self, permutation: Sequence[int] | Tensor, dim: int) -> TBatchedTensor:
         r"""Permutes the data/batch along a given dimension.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
             dim (int): Specifies the dimension where the permutation
                 is computed.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with permuted data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).permute_along_dim([2, 1, 3, 0, 4], dim=0)
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.permute_along_dim([2, 1, 3, 0, 4], dim=0)
             tensor([[4, 5],
                     [2, 3],
                     [6, 7],
                     [0, 1],
                     [8, 9]], batch_dim=0)
         """
         if not torch.is_tensor(permutation):
@@ -1486,14 +1574,15 @@
             permute_along_dim(tensor=self._data, permutation=permutation, dim=dim)
         )
 
     def permute_along_dim_(self, permutation: Sequence[int] | Tensor, dim: int) -> None:
         r"""Permutes the data/batch along a given dimension.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
             dim (int): Specifies the dimension where the permutation
                 is computed.
 
@@ -1518,155 +1607,159 @@
 
     def shuffle_along_dim(
         self, dim: int, generator: torch.Generator | None = None
     ) -> TBatchedTensor:
         r"""Shuffles the data/batch along a given dimension.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Returns:
+        -------
             ``BatchedTensor``:  A new batch with shuffled data
                 along a given dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).shuffle_along_dim(dim=0)
-            tensor([[4, 5],
-                    [2, 3],
-                    [6, 7],
-                    [0, 1],
-                    [8, 9]], batch_dim=0)
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.shuffle_along_dim(dim=0)  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0)
         """
         return self.permute_along_dim(
             torch.randperm(self._data.shape[dim], generator=generator), dim=dim
         )
 
     def shuffle_along_dim_(self, dim: int, generator: torch.Generator | None = None) -> None:
         r"""Shuffles the data/batch along a given dimension.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Returns:
+        -------
             ``BatchedTensor``:  A new batch with shuffled data
                 along a given dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.shuffle_along_dim_(dim=0)
-            >>> batch
-            tensor([[4, 5],
-                    [2, 3],
-                    [6, 7],
-                    [0, 1],
-                    [8, 9]], batch_dim=0)
+            >>> batch  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0)
         """
         self.permute_along_dim_(torch.randperm(self._data.shape[dim], generator=generator), dim=dim)
 
     def sort(
         self,
         dim: int = -1,
         descending: bool = False,
         stable: bool = False,
     ) -> torch.return_types.sort:
         r"""Sorts the elements of the batch along a given dimension in
         monotonic order by value.
 
         Args:
+        ----
             descending (bool, optional): Controls the sorting order.
                 If ``True``, the elements are sorted in descending
                 order by value. Default: ``False``
             stable (bool, optional): Makes the sorting routine stable,
                 which guarantees that the order of equivalent elements
                 is preserved. Default: ``False``
 
         Returns:
+        -------
             (``BatchedTensor``, ``BatchedTensor``): A tuple
                 two values:
                     - The first batch contains the batch values sorted
                         along the given dimension.
                     - The second batch contains the indices that sort
                         the batch along the given dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.rand(2, 5)).sort()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.sort(descending=True)
             torch.return_types.sort(
-            values=tensor([[0.0239, 0.1395, 0.1742, 0.2742, 0.3203],
-                    [0.1096, 0.1745, 0.5360, 0.8954, 0.9036]], batch_dim=0),
-            indices=tensor([[0, 1, 2, 3, 4],
-                    [2, 0, 3, 4, 1]], batch_dim=0))
+            values=tensor([[4, 3, 2, 1, 0],
+                    [9, 8, 7, 6, 5]], batch_dim=0),
+            indices=tensor([[4, 3, 2, 1, 0],
+                    [4, 3, 2, 1, 0]], batch_dim=0))
         """
         return torch.sort(self, dim=dim, descending=descending, stable=stable)
 
     def sort_along_batch(
         self,
         descending: bool = False,
         stable: bool = False,
     ) -> torch.return_types.sort:
         r"""Sorts the elements of the batch along the batch dimension in
         monotonic order by value.
 
         Args:
+        ----
             descending (bool, optional): Controls the sorting order.
                 If ``True``, the elements are sorted in descending
                 order by value. Default: ``False``
             stable (bool, optional): Makes the sorting routine stable,
                 which guarantees that the order of equivalent elements
                 is preserved. Default: ``False``
 
         Returns:
+        -------
             (``BatchedTensor``, ``BatchedTensor``): A tuple
                 two values:
                     - The first batch contains the batch values sorted
                         along the given dimension.
                     - The second batch contains the indices that sort
                         the batch along the given dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.rand(2, 5)).sort_along_batch()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.sort_along_batch(descending=True)
             torch.return_types.sort(
-            values=tensor([[0.0091, 0.5615, 0.5453, 0.1468, 0.5192],
-                    [0.4122, 0.8932, 0.8783, 0.6494, 0.7763]], batch_dim=0),
-            indices=tensor([[0, 0, 1, 1, 0],
-                    [1, 1, 0, 0, 1]], batch_dim=0))
+            values=tensor([[5, 6, 7, 8, 9],
+                    [0, 1, 2, 3, 4]], batch_dim=0),
+            indices=tensor([[1, 1, 1, 1, 1],
+                    [0, 0, 0, 0, 0]], batch_dim=0))
         """
         return self.sort(dim=self._batch_dim, descending=descending, stable=stable)
 
     ################################################
     #     Mathematical | point-wise operations     #
     ################################################
 
     def abs(self) -> TBatchedTensor:
         r"""Computes the absolute value of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the absolute value of
                 each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1699,42 +1792,45 @@
         self._data.abs_()
 
     def clamp(
         self,
         min: int | float | None = None,  # noqa: A002
         max: int | float | None = None,  # noqa: A002
     ) -> TBatchedTensor:
-        r"""Clamps all elements in ``self`` into the range ``[min, max]``.
+        r"""Clamps all elements in ``self`` into the range ``[min,
+        max]``.
 
         Note: ``min`` and ``max`` cannot be both ``None``.
 
         Args:
+        ----
             min (int, float or ``None``, optional): Specifies
                 the lower bound. If ``min`` is ``None``,
                 there is no lower bound. Default: ``None``
             max (int, float or ``None``, optional): Specifies
                 the upper bound. If ``max`` is ``None``,
                 there is no upper bound. Default: ``None``
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with clamped values.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.clamp(min=2, max=5)
             tensor([[2, 2, 2, 3, 4],
                     [5, 5, 5, 5, 5]], batch_dim=0)
             >>> batch.clamp(min=2)
             tensor([[2, 2, 2, 3, 4],
-                    [5, 6, 7, 8, 9]])
+                    [5, 6, 7, 8, 9]], batch_dim=0)
             >>> batch.clamp(max=7)
             tensor([[0, 1, 2, 3, 4],
                     [5, 6, 7, 7, 7]], batch_dim=0)
         """
         return torch.clamp(self, min=min, max=max)
 
     def clamp_(
@@ -1746,14 +1842,15 @@
         max]``.
 
         Inplace version of ``clamp``.
 
         Note: ``min`` and ``max`` cannot be both ``None``.
 
         Args:
+        ----
             min (int, float or ``None``, optional): Specifies
                 the lower bound.  If ``min`` is ``None``,
                 there is no lower bound. Default: ``None``
             max (int, float or ``None``, optional): Specifies
                 the upper bound. If ``max`` is ``None``,
                 there is no upper bound. Default: ``None``
 
@@ -1780,28 +1877,29 @@
                     [5, 6, 7, 7, 7]], batch_dim=0)
         """
         self._data.clamp_(min=min, max=max)
 
     def exp(self) -> TBatchedTensor:
         r"""Computes the exponential of the elements.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the exponential of the
                 elements of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
             >>> batch.exp()
-            tensor([[  2.7183,   7.3891,  20.0855],
-                    [ 54.5981, 148.4132, 403.4288]], batch_dim=0)
+            tensor([[  1.0000,   2.7183,   7.3891],
+                    [ 20.0855,  54.5981, 148.4132]], batch_dim=0)
         """
         return torch.exp(self)
 
     def exp_(self) -> None:
         r"""Computes the exponential of the elements.
 
         In-place version of ``exp()``.
@@ -1811,23 +1909,24 @@
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
             >>> batch.exp_()
             >>> batch
-            tensor([[  2.7183,   7.3891,  20.0855],
-                    [ 54.5981, 148.4132, 403.4288]], batch_dim=0)
+            tensor([[  1.0000,   2.7183,   7.3891],
+                    [ 20.0855,  54.5981, 148.4132]], batch_dim=0)
         """
         self._data.exp_()
 
     def log(self) -> BatchedTensor:
         r"""Computes the natural logarithm of the elements.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the natural
                 logarithm of the elements of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1859,18 +1958,63 @@
             >>> batch.log_()
             >>> batch
             tensor([[  -inf, 0.0000, 0.6931, 1.0986, 1.3863],
                     [1.6094, 1.7918, 1.9459, 2.0794, 2.1972]], batch_dim=0)
         """
         self._data.log_()
 
+    def log10(self) -> BatchedTensor:
+        r"""Computes the logarithm to the base 10 of the elements.
+
+        Returns:
+        -------
+            ``BatchedTensor``: A batch with the logarithm to the
+                base 10 of the elements of the current batch.
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> batch = BatchedTensor(
+            ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
+            ... )
+            >>> batch.log10()
+            tensor([[  -inf, 0.0000, 0.3010, 0.4771, 0.6021],
+                    [0.6990, 0.7782, 0.8451, 0.9031, 0.9542]], batch_dim=0)
+        """
+        return torch.log10(self)
+
+    def log10_(self) -> None:
+        r"""Computes the logarithm to the base 10 of the elements.
+
+        In-place version of ``log10()``.
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> batch = BatchedTensor(
+            ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
+            ... )
+            >>> batch.log10_()
+            >>> batch
+            tensor([[  -inf, 0.0000, 0.3010, 0.4771, 0.6021],
+                    [0.6990, 0.7782, 0.8451, 0.9031, 0.9542]], batch_dim=0)
+        """
+        self._data.log10_()
+
     def log1p(self) -> BatchedTensor:
         r"""Computes the natural logarithm of ``self + 1``.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the natural
                 logarithm of ``self + 1``.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1902,22 +2046,68 @@
             >>> batch.log1p_()
             >>> batch
             tensor([[0.0000, 0.6931, 1.0986, 1.3863, 1.6094],
                     [1.7918, 1.9459, 2.0794, 2.1972, 2.3026]], batch_dim=0)
         """
         self._data.log1p_()
 
+    def log2(self) -> BatchedTensor:
+        r"""Computes the logarithm to the base 2 of the elements.
+
+        Returns:
+        -------
+            ``BatchedTensor``: A batch with the logarithm to the
+                base 2 of the elements of the current batch.
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> batch = BatchedTensor(
+            ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
+            ... )
+            >>> batch.log2()
+            tensor([[  -inf, 0.0000, 1.0000, 1.5850, 2.0000],
+                    [2.3219, 2.5850, 2.8074, 3.0000, 3.1699]], batch_dim=0)
+        """
+        return torch.log2(self)
+
+    def log2_(self) -> None:
+        r"""Computes the logarithm to the base 2 of the elements.
+
+        In-place version of ``log2()``.
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> batch = BatchedTensor(
+            ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
+            ... )
+            >>> batch.log2_()
+            >>> batch
+            tensor([[  -inf, 0.0000, 1.0000, 1.5850, 2.0000],
+                    [2.3219, 2.5850, 2.8074, 3.0000, 3.1699]], batch_dim=0)
+        """
+        self._data.log2_()
+
     def maximum(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise maximum of ``self`` and ``other``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``): Specifies
                 a batch.
 
         Returns:
+        -------
             ``BatchedTensor``: The batch with the element-wise
                 maximum of ``self`` and ``other``
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1930,18 +2120,20 @@
         """
         return torch.maximum(self, other)
 
     def minimum(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise minimum of ``self`` and ``other``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``): Specifies
                 a batch.
 
         Returns:
+        -------
             ``BatchedTensor``: The batch with the element-wise
                 minimum of ``self`` and ``other``
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1954,20 +2146,22 @@
         """
         return torch.minimum(self, other)
 
     def pow(self, exponent: int | float | BatchedTensor) -> TBatchedTensor:
         r"""Computes the power of each element with the given exponent.
 
         Args:
+        ----
             exponent (int or float or ``BatchedTensor``): Specifies
                 the exponent value. ``exponent`` can be either a single
                 numeric number or a ``BatchedTensor`` with the same
                 number of elements.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the power of each
                 element with the given exponent.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1982,14 +2176,15 @@
 
     def pow_(self, exponent: int | float | BatchedTensor) -> None:
         r"""Computes the power of each element with the given exponent.
 
         In-place version of ``pow(exponent)``.
 
         Args:
+        ----
             exponent (int or float or ``BatchedTensor``): Specifies
                 the exponent value. ``exponent`` can be either a
                 single numeric number or a ``BatchedTensor``
                 with the same number of elements.
 
         Example usage:
 
@@ -2005,25 +2200,27 @@
         """
         check_batch_dims(get_batch_dims((self, exponent)))
         self._data.pow_(exponent)
 
     def rsqrt(self) -> TBatchedTensor:
         r"""Computes the reciprocal of the square-root of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the square-root of
                 each element.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[1.0, 4.0], [16.0, 25.0]])).rsqrt()
+            >>> batch = BatchedTensor(torch.tensor([[1.0, 4.0], [16.0, 25.0]]))
+            >>> batch.rsqrt()
             tensor([[1.0000, 0.5000],
                     [0.2500, 0.2000]], batch_dim=0)
         """
         return torch.rsqrt(self)
 
     def rsqrt_(self) -> None:
         r"""Computes the reciprocal of the square-root of each element.
@@ -2043,15 +2240,16 @@
                     [0.2500, 0.2000]], batch_dim=0)
         """
         self._data.rsqrt_()
 
     def sqrt(self) -> TBatchedTensor:
         r"""Computes the square-root of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the square-root of
                 each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2087,530 +2285,563 @@
     #     Reduction operations     #
     ################################
 
     def max(self, *args, **kwargs) -> Tensor | torch.return_types.max:
         r"""Computes the maximum of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.max``
             **kwargs: See the documentation of ``torch.Tensor.max``
 
         Returns:
+        -------
             ``torch.Tensor`` or ``torch.return_types.max``:
                 The maximum of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).max()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.max()
             tensor(9)
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).max(dim=1)
+            >>> batch.max(dim=1)
             torch.return_types.max(
             values=tensor([4, 9]),
             indices=tensor([4, 4]))
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).max(dim=1, keepdim=True)
+            >>> batch.max(dim=1, keepdim=True)
             torch.return_types.max(
             values=tensor([[4], [9]]),
             indices=tensor([[4], [4]]))
         """
         return torch.max(self, *args, **kwargs)
 
     def max_along_batch(self, keepdim: bool = False) -> torch.return_types.max:
         r"""Computes the maximum values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the batch dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.max``: A batch with
                 the maximum values along the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).max_along_batch()
+            >>> batch = BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]]))
+            >>> batch.max_along_batch()
             torch.return_types.max(
             values=tensor([4, 9]),
             indices=tensor([4, 4]))
-            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).max_along_batch(
-            ...     keepdim=True
-            ... )
+            >>> batch.max_along_batch(keepdim=True)
             torch.return_types.max(
-            values=tensor([[4], [9]]),
-            indices=tensor([[4], [4]]))
+            values=tensor([[4, 9]]),
+            indices=tensor([[4, 4]]))
         """
         return self.max(dim=self._batch_dim, keepdim=keepdim)
 
     def mean(self, *args, **kwargs) -> Tensor:
         r"""Computes the mean of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.mean``
             **kwargs: See the documentation of ``torch.Tensor.mean``
 
         Returns:
+        -------
             ``torch.Tensor``: The mean of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean()
-            tensor(4.5)
-            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean(dim=1)
-            tensor([2.0, 7.0])
-            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean(dim=1, keepdim=True)
-            tensor([[2.0], [7.0]])
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5).float())
+            >>> batch.mean()
+            tensor(4.5000)
+            >>> batch.mean(dim=1)
+            tensor([2., 7.])
+            >>> batch.mean(dim=1, keepdim=True)
+            tensor([[2.], [7.]])
         """
         return torch.mean(self, *args, **kwargs)
 
     def mean_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the mean values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the batch dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A batch with
                 the mean values along the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_batch()
-            tensor([4.0, 5.0])
-            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_batch(keepdim=True)
-            tensor([[4.0], [5.0]])
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2).float())
+            >>> batch.mean_along_batch()
+            tensor([4., 5.])
+            >>> batch.mean_along_batch(keepdim=True)
+            tensor([[4., 5.]])
         """
         return self.mean(dim=self._batch_dim, keepdim=keepdim)
 
     def median(self, *args, **kwargs) -> Tensor | torch.return_types.median:
         r"""Computes the median of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.median``
             **kwargs: See the documentation of ``torch.Tensor.median``
 
         Returns:
+        -------
             ``torch.Tensor`` or ``torch.return_types.median``:
                 The median of all elements or per dimension.
                 The first tensor will be populated with the median
                 values and the second tensor, which must have dtype
                 long, with their indices in the dimension dim of input.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).median()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.median()
             tensor(4)
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).median(dim=1)
+            >>> batch.median(dim=1)
             torch.return_types.median(
             values=tensor([2, 7]),
             indices=tensor([2, 2]))
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).median(dim=1, keepdim=True)
+            >>> batch.median(dim=1, keepdim=True)
             torch.return_types.median(
             values=tensor([[2], [7]]),
             indices=tensor([[2], [2]]))
         """
         return torch.median(self, *args, **kwargs)
 
     def median_along_batch(self, keepdim: bool = False) -> torch.return_types.median:
         r"""Computes the median values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.median``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the batch dimension of input.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
-            ... ).median_along_batch()
+            >>> batch = BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]]))
+            >>> batch.median_along_batch()
             torch.return_types.median(
             values=tensor([2, 7]),
             indices=tensor([2, 2]))
         """
         return self.median(dim=self._batch_dim, keepdim=keepdim)
 
     def min(self, *args, **kwargs) -> Tensor | torch.return_types.min:
         r"""Computes the minimum of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.min``
             **kwargs: See the documentation of ``torch.Tensor.min``
 
         Returns:
+        -------
             ``torch.Tensor`` or ``torch.return_types.min``:
                 The minimum of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).min()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.min()
             tensor(0)
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).min(dim=1)
+            >>> batch.min(dim=1)
             torch.return_types.min(
             values=tensor([0, 5]),
             indices=tensor([0, 0]))
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).min(dim=1, keepdim=True)
+            >>> batch.min(dim=1, keepdim=True)
             torch.return_types.min(
             values=tensor([[0], [5]]),
             indices=tensor([[0], [0]]))
         """
         return torch.min(self, *args, **kwargs)
 
     def min_along_batch(self, keepdim: bool = False) -> torch.return_types.min:
         r"""Computes the minimum values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the batch dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.min``: A batch with
                 the minimum values along the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).min_along_batch()
+            >>> batch = BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]]))
+            >>> batch.min_along_batch()
             torch.return_types.min(
             values=tensor([0, 5]),
             indices=tensor([0, 0]))
-            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).min_along_batch(
-            ...     keepdim=True
-            ... )
+            >>> batch.min_along_batch(keepdim=True)
             torch.return_types.min(
-            values=tensor([[0], [5]]),
-            indices=tensor([[0], [0]]))
+            values=tensor([[0, 5]]),
+            indices=tensor([[0, 0]]))
         """
         return self.min(dim=self._batch_dim, keepdim=keepdim)
 
     def nanmean(self, *args, **kwargs) -> Tensor:
         r"""Computes the mean of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.nanmean``
             **kwargs: See the documentation of ``torch.Tensor.nanmean``
 
         Returns:
+        -------
             ``torch.Tensor``: The mean of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmean()
-            tensor(4.0)
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmean(
-            ...     dim=1
-            ... )
-            tensor([2.0, 6.5])
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmean(
-            ...     dim=1, keepdim=True
-            ... )
-            tensor([[2.0], [6.5]])
+            >>> batch = BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]]))
+            >>> batch.nanmean()
+            tensor(4.)
+            >>> batch.nanmean(dim=1)
+            tensor([2.0000, 6.5000])
+            >>> batch.nanmean(dim=1, keepdim=True)
+            tensor([[2.0000], [6.5000]])
         """
         return torch.nanmean(self, *args, **kwargs)
 
     def nanmean_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the mean values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the batch dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A batch with
                 the mean values along the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
-            ... ).nanmean_along_batch()
-            tensor([2.0, 6.5])
-            >>> BatchedTensor(
+            >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
-            ... ).nanmean_along_batch(keepdim=True)
-            tensor([[2.0, 6.5]])
+            ... )
+            >>> batch.nanmean_along_batch()
+            tensor([2.0000, 6.5000])
+            >>> batch.nanmean_along_batch(keepdim=True)
+            tensor([[2.0000, 6.5000]])
         """
         return self.nanmean(dim=self._batch_dim, keepdim=keepdim)
 
     def nanmedian(self, *args, **kwargs) -> Tensor | torch.return_types.nanmedian:
         r"""Computes the median of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.nanmedian``
             **kwargs: See the documentation of ``torch.Tensor.nanmedian``
 
         Returns:
+        -------
             ``torch.Tensor`` or ``torch.return_types.nanmedian``:
                 The median of all elements or per dimension.
                 The first tensor will be populated with the median
                 values and the second tensor, which must have dtype
                 long, with their indices in the dimension dim of input.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmedian()
-            tensor(4.0)
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmedian(
-            ...     dim=1
-            ... )
+            >>> batch = BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]]))
+            >>> batch.nanmedian()
+            tensor(4.)
+            >>> batch.nanmedian(dim=1)
             torch.return_types.nanmedian(
             values=tensor([2., 6.]),
             indices=tensor([2, 1]))
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmedian(
-            ...     dim=1, keepdim=True
-            ... )
+            >>> batch.nanmedian(dim=1, keepdim=True)
             torch.return_types.nanmedian(
             values=tensor([[2.], [6.]]),
             indices=tensor([[2], [1]]))
         """
         return torch.nanmedian(self, *args, **kwargs)
 
     def nanmedian_along_batch(self, keepdim: bool = False) -> torch.return_types.nanmedian:
         r"""Computes the median values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.nanmedian``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the batch dimension of input.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
+            >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
-            ... ).nanmedian_along_batch()
+            ... )
+            >>> batch.nanmedian_along_batch()
             torch.return_types.nanmedian(
             values=tensor([2., 6.]),
             indices=tensor([2, 1]))
         """
         return self.nanmedian(dim=self._batch_dim, keepdim=keepdim)
 
     def nansum(self, *args, **kwargs) -> Tensor:
         r"""Computes the sum of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.nansum``
             **kwargs: See the documentation of ``torch.Tensor.nansum``
 
         Returns:
+        -------
             ``torch.Tensor``: The sum of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nansum()
+            >>> batch = BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]]))
+            >>> batch.nansum()
             tensor(36.)
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nansum(dim=1)
+            >>> batch.nansum(dim=1)
             tensor([10., 26.])
-            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nansum(
-            ...     dim=1, keepdim=True
-            ... )
+            >>> batch.nansum(dim=1, keepdim=True)
             tensor([[10.], [26.]])
         """
         return torch.nansum(self, *args, **kwargs)
 
     def nansum_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A tensor with the sum values along the
                 batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
+            >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
-            ... ).nansum_along_batch()
-            tensor([20., 26.])
+            ... )
+            >>> batch.nansum_along_batch()
+            tensor([10., 26.])
         """
         return self.nansum(dim=self._batch_dim, keepdim=keepdim)
 
     def prod(self, *args, **kwargs) -> Tensor:
         r"""Computes the product of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.nansum``
             **kwargs: See the documentation of ``torch.Tensor.nansum``
 
         Returns:
+        -------
             ``torch.Tensor``: The product of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod()
+            >>> batch = BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]]))
+            >>> batch.prod()
             tensor(362880)
-            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod(dim=1)
+            >>> batch.prod(dim=1)
             tensor([ 120, 3024])
-            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod(
-            ...     dim=1, keepdim=True
-            ... )
+            >>> batch.prod(dim=1, keepdim=True)
             tensor([[ 120], [3024]])
         """
         return torch.prod(self, *args, **kwargs)
 
     def prod_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the product values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the batch dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A batch with
                 the product values along the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])).prod_along_batch()
+            >>> batch = BatchedTensor(torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]]))
+            >>> batch.prod_along_batch()
             tensor([ 120, 3024])
-            >>> BatchedTensor(torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])).prod_along_batch(
-            ...     keepdim=True
-            ... )
+            >>> batch.prod_along_batch(keepdim=True)
             tensor([[ 120, 3024]])
         """
         return self.prod(dim=self._batch_dim, keepdim=keepdim)
 
     def sum(self, *args, **kwargs) -> Tensor:
         r"""Computes the sum of all elements.
 
         Args:
+        ----
             *args: See the documentation of ``torch.Tensor.sum``
             **kwargs: See the documentation of ``torch.Tensor.sum``
 
         Returns:
+        -------
             ``torch.Tensor``: The sum of all elements.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).sum()
+            >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
+            >>> batch.sum()
             tensor(45)
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).sum(dim=1)
+            >>> batch.sum(dim=1)
             tensor([10, 35])
-            >>> BatchedTensor(torch.arange(10).view(2, 5)).sum(dim=1, keepdim=True)
+            >>> batch.sum(dim=1, keepdim=True)
             tensor([[10], [35]])
         """
         return torch.sum(self, *args, **kwargs)
 
     def sum_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the batch dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A tensor with the sum values along the
                 batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).sum_along_batch()
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.sum_along_batch()
             tensor([20, 25])
         """
         return self.sum(dim=self._batch_dim, keepdim=keepdim)
 
     ###########################################
     #     Mathematical | trigo operations     #
     ###########################################
 
     def acos(self) -> TBatchedTensor:
         r"""Computes the inverse cosine (arccos) of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse cosine
                 (arccos) of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2633,24 +2864,25 @@
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.acos_()
             >>> batch
-            tensor([[-1.5708,  0.0000,  1.5708],
-                    [-0.5236,  0.0000,  0.5236]], batch_dim=0)
+            tensor([[3.1416, 1.5708, 0.0000],
+                    [2.0944, 1.5708, 1.0472]], batch_dim=0)
         """
         self._data.acos_()
 
     def acosh(self) -> TBatchedTensor:
         r"""Computes the inverse hyperbolic cosine (arccosh) of each
         element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 cosine (arccosh) of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2663,15 +2895,16 @@
         """
         return torch.acosh(self)
 
     def acosh_(self) -> None:
         r"""Computes the inverse hyperbolic cosine (arccosh) of each
         element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 cosine (arccosh) of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2684,15 +2917,16 @@
                     [2.0634, 2.2924, 2.4779]], batch_dim=0)
         """
         self._data.acosh_()
 
     def asin(self) -> TBatchedTensor:
         r"""Computes the inverse cosine (arcsin) of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse sine
                 (arcsin) of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2715,24 +2949,25 @@
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.asin_()
             >>> batch
-            tensor([[3.1416, 1.5708, 0.0000],
-                    [2.0944, 1.5708, 1.0472]], batch_dim=0)
+            tensor([[-1.5708,  0.0000,  1.5708],
+                    [-0.5236,  0.0000,  0.5236]], batch_dim=0)
         """
         self._data.asin_()
 
     def asinh(self) -> TBatchedTensor:
         r"""Computes the inverse hyperbolic sine (arcsinh) of each
         element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 sine (arcsinh) of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2764,15 +2999,16 @@
                     [-0.4812,  0.0000,  0.4812]], batch_dim=0)
         """
         self._data.asinh_()
 
     def atan(self) -> TBatchedTensor:
         r"""Computes the inverse tangent of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse tangent
                 of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2803,15 +3039,16 @@
                     [-1.1071, -0.7854,  0.0000]], batch_dim=0)
         """
         self._data.atan_()
 
     def atanh(self) -> TBatchedTensor:
         r"""Computes the inverse hyperbolic tangent of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 tangent of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2842,15 +3079,16 @@
                     [-0.1003,  0.0000,  0.1003]], batch_dim=0)
         """
         self._data.atanh_()
 
     def cos(self) -> TBatchedTensor:
         r"""Computes the cosine of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the cosine of each
                 element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2877,64 +3115,66 @@
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 0.5 * math.pi, math.pi], [2 * math.pi, 1.5 * math.pi, 0.0]])
             ... )
-            >>> batch.cos()
+            >>> batch.cos_()
             >>> batch
             tensor([[ 1.0000e+00, -4.3711e-08, -1.0000e+00],
                     [ 1.0000e+00,  1.1925e-08,  1.0000e+00]], batch_dim=0)
         """
         self._data.cos_()
 
     def cosh(self) -> TBatchedTensor:
         r"""Computes the hyperbolic cosine (cosh) of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the hyperbolic
                 cosine (arccosh) of each element.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
+            >>> batch = BatchedTensor(torch.tensor([[1.0, 2.1, 3.2], [4.0, 5.1, 6.2]]))
             >>> batch.cosh()
-            tensor([[0.0000, 1.3170, 1.7627],
-                    [2.0634, 2.2924, 2.4779]], batch_dim=0)
+            tensor([[  1.5431,   4.1443,  12.2866],
+                    [ 27.3082,  82.0140, 246.3755]], batch_dim=0)
         """
         return torch.cosh(self)
 
     def cosh_(self) -> None:
         r"""Computes the hyperbolic cosine (arccosh) of each element.
 
         In-place version of ``cosh()``.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
+            >>> batch = BatchedTensor(torch.tensor([[1.0, 2.1, 3.2], [4.0, 5.1, 6.2]]))
             >>> batch.cosh_()
             >>> batch
-            tensor([[0.0000, 1.3170, 1.7627],
-                    [2.0634, 2.2924, 2.4779]], batch_dim=0)
+            tensor([[  1.5431,   4.1443,  12.2866],
+                    [ 27.3082,  82.0140, 246.3755]], batch_dim=0)
         """
         self._data.cosh_()
 
     def sin(self) -> TBatchedTensor:
         r"""Computes the sine of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the sine of each
                 element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -2971,15 +3211,16 @@
                     [ 1.7485e-07, -1.0000e+00,  0.0000e+00]], batch_dim=0)
         """
         self._data.sin_()
 
     def sinh(self) -> TBatchedTensor:
         r"""Computes the hyperbolic sine of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the hyperbolic sine of
                 each element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3010,15 +3251,16 @@
                     [-0.5211,  0.0000,  0.5211]], batch_dim=0)
         """
         self._data.sinh_()
 
     def tan(self) -> TBatchedTensor:
         r"""Computes the tangent of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the tangent of each
                 element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3059,15 +3301,16 @@
                     [ 1.7485e-07, -1.0000e+00, -1.0000e+00]], batch_dim=0)
         """
         self._data.tan_()
 
     def tanh(self) -> TBatchedTensor:
         r"""Computes the tangent of each element.
 
-        Return:
+        Returns:
+        -------
             ``BatchedTensor``: A batch with the tangent of each
                 element.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3106,19 +3349,21 @@
     def logical_and(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise logical AND.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch or tensor to compute
                 logical AND with.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 logical AND.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3139,14 +3384,15 @@
     def logical_and_(self, other: BatchedTensor | Tensor) -> None:
         r"""Computes the element-wise logical AND.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch or tensor to compute
                 logical AND with.
 
         Example usage:
 
         .. code-block:: pycon
@@ -3170,14 +3416,15 @@
     def logical_not(self) -> TBatchedTensor:
         r"""Computes the element-wise logical NOT of the current batch.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 logical NOT of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3217,18 +3464,20 @@
     def logical_or(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise logical OR.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch to compute logical OR with.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 logical OR.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3249,14 +3498,15 @@
     def logical_or_(self, other: BatchedTensor | Tensor) -> None:
         r"""Computes the element-wise logical OR.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch to compute logical OR with.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3279,18 +3529,20 @@
     def logical_xor(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise logical XOR.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch to compute logical XOR with.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch containing the element-wise
                 logical XOR.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3311,14 +3563,15 @@
     def logical_xor_(self, other: BatchedTensor | Tensor) -> None:
         r"""Computes the element-wise logical XOR.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Args:
+        ----
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch to compute logical XOR with.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3364,30 +3617,31 @@
         tensors: BatchedTensor | Tensor | Iterable[BatchedTensor | Tensor],
         dim: int = 0,
     ) -> TBatchedTensor:
         r"""Concatenates the data of the batch(es) to the current batch
         along a given dimension and creates a new batch.
 
         Args:
+        ----
             tensors (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with the concatenated data
                 in the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]])).cat(
-            ...     BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]]))
-            ... )
+            >>> batch = BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]]))
+            >>> batch.cat(BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]])))
             tensor([[ 0,  1,  2],
                     [ 4,  5,  6],
                     [10, 11, 12],
                     [13, 14, 15]], batch_dim=0)
         """
         if isinstance(tensors, (BatchedTensor, Tensor)):
             tensors = [tensors]
@@ -3398,14 +3652,15 @@
         tensors: BatchedTensor | Tensor | Iterable[BatchedTensor | Tensor],
         dim: int = 0,
     ) -> None:
         r"""Concatenates the data of the batch(es) to the current batch
         along a given dimension and creates a new batch.
 
         Args:
+        ----
             tensor (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3424,35 +3679,37 @@
     def cat_along_batch(
         self, tensors: BatchedTensor | Tensor | Iterable[BatchedTensor | Tensor]
     ) -> TBatchedTensor:
         r"""Concatenates the data of the batch(es) to the current batch
         along the batch dimension and creates a new batch.
 
         Args:
+        ----
             tensors (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Returns:
+        -------
             ``BatchedTensor``: A batch with the concatenated data
                 in the batch dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]])).cat_along_batch(
-            ...     BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]]))
-            ... )
+            >>> batch = BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]]))
+            >>> batch.cat_along_batch(BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]])))
             tensor([[ 0,  1,  2],
                     [ 4,  5,  6],
                     [10, 11, 12],
                     [13, 14, 15]], batch_dim=0)
-            >>> BatchedTensor(torch.tensor([[0, 4], [1, 5], [2, 6]])).cat_along_batch(
+            >>> batch = BatchedTensor(torch.tensor([[0, 4], [1, 5], [2, 6]]))
+            >>> batch.cat_along_batch(
             ...     [
             ...         BatchedTensor(torch.tensor([[10, 12], [11, 13]])),
             ...         BatchedTensor(torch.tensor([[20, 22], [21, 23]])),
             ...     ]
             ... )
             tensor([[ 0,  4],
                     [ 1,  5],
@@ -3467,14 +3724,15 @@
     def cat_along_batch_(
         self, tensors: BatchedTensor | Tensor | Iterable[BatchedTensor | Tensor]
     ) -> None:
         r"""Concatenates the data of the batch(es) to the current batch
         along the batch dimension and creates a new batch.
 
         Args:
+        ----
             tensors (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3483,15 +3741,15 @@
             >>> batch = BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]]))
             >>> batch.cat_along_batch_(BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]])))
             >>> batch
             tensor([[ 0,  1,  2],
                     [ 4,  5,  6],
                     [10, 11, 12],
                     [13, 14, 15]], batch_dim=0)
-            >>> BatchedTensor(torch.tensor([[0, 4], [1, 5], [2, 6]]))
+            >>> batch = BatchedTensor(torch.tensor([[0, 4], [1, 5], [2, 6]]))
             >>> batch.cat_along_batch_(
             ...     [
             ...         BatchedTensor(torch.tensor([[10, 12], [11, 13]])),
             ...         BatchedTensor(torch.tensor([[20, 22], [21, 23]])),
             ...     ]
             ... )
             >>> batch
@@ -3505,29 +3763,32 @@
         """
         self.cat_(tensors, dim=self._batch_dim)
 
     def chunk(self, chunks: int, dim: int = 0) -> tuple[TBatchedTensor, ...]:
         r"""Splits the batch into chunks along a given dimension.
 
         Args:
+        ----
             chunks (int): Specifies the number of chunks.
             dim (int, optional): Specifies the dimension along which
                 to split the tensor. Default: ``0``
 
         Returns:
+        -------
             tuple: The batch split into chunks along the given
                 dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).chunk(chunks=3)
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.chunk(chunks=3)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
         """
         return torch.chunk(self, chunks, dim=dim)
 
     def chunk_along_batch(self, chunks: int) -> tuple[TBatchedTensor, ...]:
@@ -3536,19 +3797,21 @@
     def extend(self, other: Iterable[BatchedTensor]) -> None:
         self.cat_along_batch_(other)
 
     def index_select(self, dim: int, index: Tensor | Sequence[int]) -> TBatchedTensor:
         r"""Selects data at the given indices along a given dimension.
 
         Args:
+        ----
             dim (int): Specifies the index dimension.
             index (``torch.Tensor`` or list or tuple): Specifies the
                 indices to select.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch which indexes ``self``
                 along the batch dimension using the entries in
                 ``index``.
 
         Example usage:
 
         .. code-block:: pycon
@@ -3572,23 +3835,25 @@
 
     def index_select_along_batch(self, index: Tensor | Sequence[int]) -> TBatchedTensor:
         return self.index_select(self._batch_dim, index)
 
     def masked_fill(
         self, mask: BatchedTensor | Tensor, value: bool | int | float
     ) -> TBatchedTensor:
-        r"""Fills elements of ``self`` batch with ``value`` where ``mask`` is
-        ``True``.
+        r"""Fills elements of ``self`` batch with ``value`` where
+        ``mask`` is ``True``.
 
         Args:
+        ----
             mask (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch of boolean masks.
             value (number): Specifies the value to fill in with.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with the updated values.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -3618,28 +3883,31 @@
         return self._create_new_batch(self._data.masked_fill(mask.data, value))
 
     def select(self, dim: int, index: int) -> Tensor:
         r"""Selects the batch along the batch dimension at the given
         index.
 
         Args:
+        ----
             dim (int): Specifies the index dimension.
             index (int): Specifies the index to select.
 
         Returns:
+        -------
             ``Tensor``: The batch sliced along the batch
                 dimension at the given index.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).select(dim=0, index=2)
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.select(dim=0, index=2)
             tensor([4, 5])
         """
         return torch.select(self._data, dim=dim, index=index)
 
     def select_along_batch(self, index: int) -> Tensor:
         return self._data.select(self._batch_dim, index)
 
@@ -3654,42 +3922,45 @@
         start: int = 0,
         stop: int | None = None,
         step: int = 1,
     ) -> TBatchedTensor:
         r"""Slices the batch in a given dimension.
 
         Args:
+        ----
             dim (int, optional): Specifies the dimension along which
                 to slice the tensor. Default: ``0``
             start (int, optional): Specifies the index where the
                 slicing of object starts. Default: ``0``
             stop (int, optional): Specifies the index where the
                 slicing of object stops. ``None`` means last.
                 Default: ``None``
             step (int, optional): Specifies the increment between
                 each index for slicing. Default: ``1``
 
         Returns:
+        -------
             ``BatchedTensor``: A slice of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).slice_along_dim(start=2)
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.slice_along_dim(start=2)
             tensor([[4, 5],
                     [6, 7],
                     [8, 9]], batch_dim=0)
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).slice_along_dim(stop=3)
+            >>> batch.slice_along_dim(stop=3)
             tensor([[0, 1],
                     [2, 3],
                     [4, 5]], batch_dim=0)
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).slice_along_dim(step=2)
+            >>> batch.slice_along_dim(step=2)
             tensor([[0, 1],
                     [4, 5],
                     [8, 9]], batch_dim=0)
         """
         if dim == 0:
             data = self._data[start:stop:step]
         elif dim == 1:
@@ -3700,30 +3971,33 @@
 
     def split(
         self, split_size_or_sections: int | Sequence[int], dim: int = 0
     ) -> tuple[TBatchedTensor, ...]:
         r"""Splits the batch into chunks along a given dimension.
 
         Args:
+        ----
             split_size_or_sections (int or sequence): Specifies the
                 size of a single chunk or list of sizes for each chunk.
             dim (int, optional): Specifies the dimension along which
                 to split the tensor. Default: ``0``
 
         Returns:
+        -------
             tuple: The batch split into chunks along the given
                 dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).split(2, dim=0)
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.split(2, dim=0)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
         """
         return torch.split(self, split_size_or_sections, dim=dim)
 
     def split_along_batch(
@@ -3733,60 +4007,62 @@
 
     def take_along_batch(
         self, indices: BaseBatch[Tensor | Sequence] | Tensor | Sequence
     ) -> TBatchedTensor:
         r"""Takes values along the batch dimension.
 
         Args:
+        ----
             indices (``BaseBatch`` or ``Tensor`` or sequence):
                 Specifies the indices to take along the batch
                 dimension.
 
         Returns:
-            ``BaseBatch``: The batch with the selected data.
+        -------
+            ``BatchedTensor``: The batch with the selected data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).take_along_batch(
-            ...     BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]]))
-            ... )
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.take_along_batch(BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]])))
             tensor([[6, 5],
                     [0, 7],
                     [2, 9]], batch_dim=0)
         """
         return self.take_along_dim(indices, dim=self._batch_dim)
 
     def take_along_dim(
         self,
         indices: BaseBatch[Tensor | Sequence] | Tensor | Sequence,
         dim: int | None = None,
     ) -> TBatchedTensor:
         r"""Takes values along the batch dimension.
 
         Args:
+        ----
             indices (``BaseBatch`` or ``Tensor`` or sequence):
                 Specifies the indices to take along the batch
                 dimension.
 
         Returns:
-            ``BaseBatch``: The batch with the selected data.
+        -------
+            ``BatchedTensor``: The batch with the selected data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).take_along_dim(
-            ...     BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]])), dim=0
-            ... )
+            >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
+            >>> batch.take_along_dim(BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]])), dim=0)
             tensor([[6, 5],
                     [0, 7],
                     [2, 9]], batch_dim=0)
         """
         if isinstance(indices, Sequence):
             indices = torch.as_tensor(indices)
         return torch.take_along_dim(self, indices, dim=dim)
@@ -3795,34 +4071,37 @@
         r"""Returns a new batch with a dimension of size one inserted at
         the specified position.
 
         The returned tensor shares the same underlying data with this
         batch.
 
         Args:
+        ----
             dim (int): Specifies the dimension at which to insert the
                 singleton dimension.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with an added singleton
                 dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.ones(2, 3)).unsqueeze(dim=0)
+            >>> batch = BatchedTensor(torch.ones(2, 3))
+            >>> batch.unsqueeze(dim=0)
             tensor([[[1., 1., 1.],
                     [1., 1., 1.]]], batch_dim=1)
-            >>> BatchedTensor(torch.ones(2, 3)).unsqueeze(dim=1)
+            >>> batch.unsqueeze(dim=1)
             tensor([[[1., 1., 1.]],
                     [[1., 1., 1.]]], batch_dim=0)
-            >>> BatchedTensor(torch.ones(2, 3)).unsqueeze(dim=-1)
+            >>> batch.unsqueeze(dim=-1)
             tensor([[[1.],
                      [1.],
                      [1.]],
                     [[1.],
                      [1.],
                      [1.]]], batch_dim=0)
         """
@@ -3830,52 +4109,57 @@
             self._data.unsqueeze(dim=dim),
             batch_dim=self._batch_dim + 1
             if self._batch_dim >= dim and dim >= 0
             else self._batch_dim,
         )
 
     def view(self, *shape: tuple[int, ...]) -> Tensor:
-        r"""Creates a new tensor with the same data as the ``self`` batch but
-        with a new shape.
+        r"""Creates a new tensor with the same data as the ``self`` batch
+        but with a new shape.
 
         Args:
+        ----
             shape (tuple): Specifies the desired shape.
 
-        Retunrs:
+        Returns:
+        -------
             ``torch.Tensor``: A new view of the tensor in the batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.ones(2, 6)).view(2, 3, 2)
+            >>> batch = BatchedTensor(torch.ones(2, 6))
+            >>> batch.view(2, 3, 2)
             tensor([[[1., 1.],
                      [1., 1.],
                      [1., 1.]],
                     [[1., 1.],
                      [1., 1.],
                      [1., 1.]]])
         """
         return self._data.view(*shape)
 
     def view_as(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
-        r"""Creates a new batch with the same data as the ``self`` batch but the
-        shape of ``other``.
+        r"""Creates a new batch with the same data as the ``self`` batch
+        but the shape of ``other``.
 
         The returned batch shares the same data and must have the
         same number of elements, but the data may have a different
         size.
 
         Args:
+        ----
             other (``BatchedTensor``): Specifies the batch with
                 the target shape.
 
         Returns:
+        -------
             ``BatchedTensor``: A new batch with the shape of
                 ``other``.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -3907,20 +4191,22 @@
     #################
 
     def apply(self, fn: Callable[[Tensor], Tensor]) -> TBatchedTensor:
         r"""Apply a function to transform the tensor of the current
         batch.
 
         Args:
+        ----
             fn (``Callable``): Specifies the function to be applied to
                 the tensor. It is the responsibility of the user to
                 verify the function applies a valid transformation of
                 the data.
 
         Returns:
+        -------
             ``BatchedTensor``: The transformed batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -3935,14 +4221,15 @@
     def apply_(self, fn: Callable[[Tensor], Tensor]) -> None:
         r"""Apply a function to transform the tensor of the current
         batch.
 
         In-place version of ``apply``.
 
         Args:
+        ----
             fn (``Callable``): Specifies the function to be applied to
                 the tensor. It is the responsibility of the user to
                 verify the function applies a valid transformation of
                 the data.
 
         Example usage:
 
@@ -3972,51 +4259,84 @@
         return {"batch_dim": self._batch_dim}
 
 
 def check_data_and_dim(data: Tensor, batch_dim: int) -> None:
     r"""Checks if the tensor ``data`` and ``batch_dim`` are correct.
 
     Args:
+    ----
         data (``torch.Tensor``): Specifies the tensor in the batch.
         batch_dim (int): Specifies the batch dimension in the
             ``torch.Tensor`` object.
 
     Raises:
+    ------
         RuntimeError: if one of the input is incorrect.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat.tensor import check_data_and_dim
+        >>> check_data_and_dim(torch.ones(2, 3), batch_dim=0)
     """
     if data.dim() < 1:
         raise RuntimeError(f"data needs at least 1 dimensions (received: {data.dim()})")
     if batch_dim < 0 or batch_dim >= data.dim():
         raise RuntimeError(
             f"Incorrect batch_dim ({batch_dim}) but the value should be in [0, {data.dim() - 1}]"
         )
 
 
 def check_batch_dims(dims: set[int]) -> None:
     r"""Gets the batch dimensions from the inputs.
 
     Args:
+    ----
         dims (set): Specifies the batch dims to check.
 
     Raises:
+    ------
         RuntimeError if there are more than one batch dimension.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat.tensor import check_batch_dims
+        >>> check_batch_dims({0})
     """
     if len(dims) != 1:
         raise RuntimeError(f"The batch dimensions do not match. Received multiple values: {dims}")
 
 
 def get_batch_dims(args: Iterable[Any], kwargs: Mapping[str, Any] | None = None) -> set[int]:
     r"""Gets the batch dimensions from the inputs.
 
     Args:
+    ----
         args: Variable length argument list.
         kwargs: Arbitrary keyword arguments.
 
     Returns:
+    -------
         set: The batch dimensions.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat import BatchedTensor
+        >>> from redcat.tensor import get_batch_dims
+        >>> get_batch_dims(
+        ...     args=(BatchedTensor(torch.ones(2, 3)), BatchedTensor(torch.ones(2, 6))),
+        ...     kwargs={"batch": BatchedTensor(torch.ones(2, 4))},
+        ... )
+        {0}
     """
     kwargs = kwargs or {}
     dims = {val._batch_dim for val in args if hasattr(val, "_batch_dim")}
     dims.update({val._batch_dim for val in kwargs.values() if hasattr(val, "_batch_dim")})
     return dims
```

### Comparing `redcat-0.0.6/src/redcat/tensorseq.py` & `redcat-0.0.7/src/redcat/tensorseq.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,23 +38,32 @@
 
 
 class BatchedTensorSeq(BatchedTensor):
     r"""Implements a batched tensor to easily manipulate a batch of
     sequences.
 
     Args:
+    ----
         data (array_like): Specifies the data for the tensor. It can
             be a torch.Tensor, list, tuple, NumPy ndarray, scalar,
             and other types.
         batch_dim (int, optional): Specifies the batch dimension
             in the ``torch.Tensor`` object. Default: ``0``
         seq_dim (int, optional): Specifies the sequence dimension in
             the ``torch.Tensor`` object. Default: ``1``
         kwargs: Keyword arguments that are passed to
             ``torch.as_tensor``.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat import BatchedTensorSeq
+        >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
     """
 
     def __init__(self, data: Any, *, batch_dim: int = 0, seq_dim: int = 1, **kwargs) -> None:
         super().__init__(data, batch_dim=batch_dim, **kwargs)
         check_data_and_dims(self._data, batch_dim, seq_dim)
         self._seq_dim = int(seq_dim)
 
@@ -104,26 +113,28 @@
         r"""Creates a batch filled with a scalar value.
 
         By default, the tensor in the returned batch has the same
         shape, ``torch.dtype`` and ``torch.device`` as the tensor in
         the current batch.
 
         Args:
+        ----
             fill_value (float or int or bool): Specifies the number
                 to fill the batch with.
             batch_size (int or ``None``): Specifies the batch size.
                 If ``None``, the batch size of the current batch is
                 used. Default: ``None``.
             seq_len (int or ``None``): Specifies the sequence length.
                 If ``None``, the sequence length of the current batch
                 is used. Default: ``None``.
             **kwargs: See the documentation of
                 ``torch.Tensor.new_full``.
 
         Returns:
+        -------
             ``BaseBatchedTensor``: A batch filled with the scalar value.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -160,24 +171,26 @@
         r"""Creates a batch filled with the scalar value ``1``.
 
         By default, the tensor in the returned batch has the same
         shape, ``torch.dtype`` and ``torch.device`` as the tensor in
         the current batch.
 
         Args:
+        ----
             batch_size (int or ``None``): Specifies the batch size.
                 If ``None``, the batch size of the current batch is
                 used. Default: ``None``.
             seq_len (int or ``None``): Specifies the sequence length.
                 If ``None``, the sequence length of the current batch
                 is used. Default: ``None``.
             **kwargs: See the documentation of
                 ``torch.Tensor.new_ones``.
 
         Returns:
+        -------
             ``BaseBatchedTensor``: A batch filled with the scalar
                 value ``1``.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -215,24 +228,26 @@
         r"""Creates a batch filled with the scalar value ``0``.
 
         By default, the tensor in the returned batch has the same
         shape, ``torch.dtype`` and ``torch.device`` as the tensor
         in the current batch.
 
         Args:
+        ----
             batch_size (int or ``None``): Specifies the batch size.
                 If ``None``, the batch size of the current batch is
                 used. Default: ``None``.
             seq_len (int or ``None``): Specifies the sequence length.
                 If ``None``, the sequence length of the current batch
                 is used. Default: ``None``.
             **kwargs: See the documentation of
                 ``torch.Tensor.new_zeros``.
 
         Returns:
+        -------
             ``BaseBatchedTensor``: A batch filled with the scalar
                 value ``0``.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -263,27 +278,29 @@
 
     @classmethod
     def from_seq_batch(cls, data: Any, **kwargs) -> BatchedTensorSeq:
         r"""Creates a batch where the first dimension is the sequence
         dimension and the second dimension is the batch dimension.
 
         Args:
+        ----
             data (array_like): Specifies the data for the tensor. It can
                 be a torch.Tensor, list, tuple, NumPy ndarray, scalar,
                 and other types.
             kwargs: Keyword arguments that are passed to
                 ``torch.as_tensor``.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq.from_seq_batch(torch.ones(2, 3))
+            >>> batch = BatchedTensorSeq.from_seq_batch(torch.ones(2, 3))
+            >>> batch
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=1, seq_dim=0)
         """
         return cls(data, batch_dim=1, seq_dim=0, **kwargs)
 
     #################################
     #     Comparison operations     #
@@ -348,17 +365,19 @@
     ###########################################################
 
     def cumsum_along_seq(self, **kwargs) -> BatchedTensorSeq:
         r"""Computes the cumulative sum of elements of the current batch
         in the sequence dimension.
 
         Args:
+        ----
             **kwargs: see ``torch.cumsum`` documentation
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A batch with the cumulative sum of
                 elements of the current batch in the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -391,14 +410,15 @@
 
     def logcumsumexp_along_seq(self) -> BatchedTensorSeq:
         r"""Computes the logarithm of the cumulative summation of the
         exponentiation of elements of the current batch in the sequence
         dimension.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A batch with the cumulative
                 summation of the exponentiation of elements of the
                 current batch in the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
@@ -430,20 +450,22 @@
         """
         self.logcumsumexp_(self._seq_dim)
 
     def permute_along_seq(self, permutation: Sequence[int] | Tensor) -> BatchedTensorSeq:
         r"""Permutes the data along the sequence dimension.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A new batch with permuted data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -455,14 +477,15 @@
         """
         return self.permute_along_dim(permutation, dim=self._seq_dim)
 
     def permute_along_seq_(self, permutation: Sequence[int] | Tensor) -> None:
         r"""Permutes the data along the sequence dimension.
 
         Args:
+        ----
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Example usage:
 
@@ -478,89 +501,94 @@
         """
         self.permute_along_dim_(permutation, dim=self._seq_dim)
 
     def shuffle_along_seq(self, generator: torch.Generator | None = None) -> BatchedTensorSeq:
         r"""Shuffles the data along the sequence dimension.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Returns:
+        -------
             ``BatchedTensorSeq``:  A new batch with shuffled data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).shuffle_along_seq()
-            tensor([[2, 1, 4, 0, 3],
-                    [7, 6, 9, 5, 8]], batch_dim=0, seq_dim=1)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.shuffle_along_seq()  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0, seq_dim=1)
         """
         return self.permute_along_seq(torch.randperm(self.seq_len, generator=generator))
 
     def shuffle_along_seq_(self, generator: torch.Generator | None = None) -> None:
         r"""Shuffles the data along the sequence dimension.
 
         Args:
+        ----
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
             >>> batch.shuffle_along_seq_()
-            >>> batch
-            tensor([[2, 1, 4, 0, 3],
-                    [7, 6, 9, 5, 8]], batch_dim=0, seq_dim=1)
+            >>> batch  # doctest:+ELLIPSIS
+            tensor([[...]], batch_dim=0, seq_dim=1)
         """
         self.permute_along_seq_(torch.randperm(self.seq_len, generator=generator))
 
     def sort_along_seq(
         self, descending: bool = False, stable: bool = False
     ) -> torch.return_types.sort:
         r"""Sorts the elements of the batch along the sequence dimension
         in monotonic order by value.
 
         Args:
+        ----
             descending (bool, optional): Controls the sorting order.
                 If ``True``, the elements are sorted in descending
                 order by value. Default: ``False``
             stable (bool, optional): Makes the sorting routine stable,
                 which guarantees that the order of equivalent elements
                 is preserved. Default: ``False``
 
         Returns:
+        -------
             (``BatchedTensorSeq``, ``BatchedTensorSeq``): A tuple with
                 two values:
                     - The first batch contains the batch values sorted
                         along the sequence dimension.
                     - The second batch contains the indices that sort
                         the batch along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.rand(2, 5)).sort_along_seq()
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.sort_along_seq(descending=True)
             torch.return_types.sort(
-            values=tensor([[0.2884, 0.4014, 0.5857, 0.6949, 0.8264],
-                    [0.3811, 0.4431, 0.4857, 0.6009, 0.7207]], batch_dim=0, seq_dim=1),
-            indices=tensor([[2, 4, 3, 0, 1],
-                    [1, 0, 4, 2, 3]], batch_dim=0, seq_dim=1))
+            values=tensor([[4, 3, 2, 1, 0],
+                    [9, 8, 7, 6, 5]], batch_dim=0, seq_dim=1),
+            indices=tensor([[4, 3, 2, 1, 0],
+                    [4, 3, 2, 1, 0]], batch_dim=0, seq_dim=1))
         """
         return self.sort(dim=self._seq_dim, descending=descending, stable=stable)
 
     ################################################
     #     Mathematical | point-wise operations     #
     ################################################
 
@@ -588,251 +616,271 @@
     #     Reduction operations     #
     ################################
 
     def max_along_seq(self, keepdim: bool = False) -> torch.return_types.max:
         r"""Computes the maximum values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.max``: A batch with
                 the maximum values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).max_along_seq()
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.max_along_seq()
             torch.return_types.max(
             values=tensor([4, 9]),
             indices=tensor([4, 4]))
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).max_along_seq(keepdim=True)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.max_along_seq(keepdim=True)
             torch.return_types.max(
             values=tensor([[4], [9]]),
             indices=tensor([[4], [4]]))
         """
         return self.max(dim=self._seq_dim, keepdim=keepdim)
 
     def mean_along_seq(self, keepdim: bool = False) -> BatchedTensor | BatchedTensorSeq:
         r"""Computes the mean values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not. If ``False``
                 the returned type is ``BatchedTensor``, otherwise it
                 is ``BatchedTensorSeq``. Default: ``False``
 
         Returns:
+        -------
             ``BatchedTensor`` or ``BatchedTensorSeq``: A batch with
                 the mean values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).mean_along_seq()
-            tensor([2.0, 7.0])
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).mean_along_seq(keepdim=True)
-            tensor([[2.0], [7.0]])
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5).float())
+            >>> batch.mean_along_seq()
+            tensor([2., 7.])
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5).float())
+            >>> batch.mean_along_seq(keepdim=True)
+            tensor([[2.], [7.]])
         """
         return self.mean(dim=self._seq_dim, keepdim=keepdim)
 
     def median_along_seq(self, keepdim: bool = False) -> torch.return_types.median:
         r"""Computes the median values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.median``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the sequence dimension of input.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).median_along_seq()
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.median_along_seq()
             torch.return_types.median(
             values=tensor([2, 7]),
             indices=tensor([2, 2]))
         """
         return self.median(dim=self._seq_dim, keepdim=keepdim)
 
     def min_along_seq(self, keepdim: bool = False) -> torch.return_types.min:
         r"""Computes the minimum values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.min``: A batch with
                 the minimum values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).min_along_seq()
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.min_along_seq()
             torch.return_types.min(
             values=tensor([0, 5]),
             indices=tensor([0, 0]))
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).min_along_seq(keepdim=True)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.min_along_seq(keepdim=True)
             torch.return_types.min(
             values=tensor([[0], [5]]),
             indices=tensor([[0], [0]]))
         """
         return self.min(dim=self._seq_dim, keepdim=keepdim)
 
     def nanmean_along_seq(self, keepdim: bool = False) -> Tensor:
         r"""Computes the mean values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the batch dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A batch with
                 the mean values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmean_along_seq()
-            tensor([2.0, 6.5])
-            >>> BatchedTensorSeq(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmean_along_seq(keepdim=True)
-            tensor([[2.0], [6.5]])
+            >>> batch = BatchedTensorSeq(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]]))
+            >>> batch.nanmean_along_seq()
+            tensor([2.0000, 6.5000])
+            >>> batch.nanmean_along_seq(keepdim=True)
+            tensor([[2.0000], [6.5000]])
         """
         return self.nanmean(dim=self._seq_dim, keepdim=keepdim)
 
     def nanmedian_along_seq(self, keepdim: bool = False) -> torch.return_types.nanmedian:
         r"""Computes the median values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.return_types.nanmedian``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the sequence dimension of input.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmedian_along_seq()
+            >>> batch = BatchedTensorSeq(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]]))
+            >>> batch.nanmedian_along_seq()
             torch.return_types.nanmedian(
             values=tensor([2., 6.]),
             indices=tensor([2, 1]))
         """
         return self.nanmedian(dim=self._seq_dim, keepdim=keepdim)
 
     def nansum_along_seq(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A tensor with the sum values along the
                 sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nansum_along_seq()
-            tensor([20., 26.])
+            >>> batch = BatchedTensorSeq(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]]))
+            >>> batch.nansum_along_seq()
+            tensor([10., 26.])
         """
         return self.nansum(dim=self._seq_dim, keepdim=keepdim)
 
     def prod_along_seq(self, keepdim: bool = False) -> Tensor:
         r"""Computes the product values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
                 Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A batch with
                 the product values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq()
+            >>> batch = BatchedTensorSeq(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]]))
+            >>> batch.prod_along_seq()
             tensor([ 120, 3024])
-            >>> BatchedTensorSeq(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq(
-            ...     keepdim=True
-            ... )
+            >>> batch.prod_along_seq(keepdim=True)
             tensor([[ 120], [3024]])
         """
         return self.prod(dim=self._seq_dim, keepdim=keepdim)
 
     def sum_along_seq(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the sequence dimension.
 
         Args:
+        ----
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not. If ``False``
                 the returned type is ``BatchedTensor``, otherwise it
                 is ``BatchedTensorSeq``. Default: ``False``
 
         Returns:
+        -------
             ``torch.Tensor``: A tensor with the sum values along the
                 sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).sum_along_seq()
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.sum_along_seq()
             tensor([10, 35])
         """
         return self.sum(dim=self._seq_dim, keepdim=keepdim)
 
     ##########################################################
     #    Indexing, slicing, joining, mutating operations     #
     ##########################################################
@@ -840,41 +888,43 @@
     def align_as(self, other: BatchedTensorSeq) -> BatchedTensorSeq:
         r"""Aligns the current batch with the batch ``other``.
 
         This method makes sure the batch and sequence dimensions
         are aligned.
 
         Args:
+        ----
             other (``BatchedTensorSeq``): Specifies the batch to use to
                 align the current batch.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: The aligned batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            # batch-sequence -> sequence-batch
+            >>> # batch-sequence -> sequence-batch
             >>> seq_batch = BatchedTensorSeq(torch.ones(2, 3), batch_dim=1, seq_dim=0)
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).align_as(seq_batch)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.align_as(seq_batch)
             tensor([[0, 5],
                     [1, 6],
                     [2, 7],
                     [3, 8],
-                    [4, 9]], batch_dim=0, seq_dim=1)
-            # sequence-batch -> batch-sequence
+                    [4, 9]], batch_dim=1, seq_dim=0)
+            >>> # sequence-batch -> batch-sequence
             >>> batch_seq = BatchedTensorSeq(torch.ones(2, 3))
-            >>> BatchedTensorSeq.from_seq_batch(
-            ...     torch.arange(10).view(5, 2), batch_dim=1, seq_dim=0
-            ... ).align_as(batch_seq)
+            >>> batch = BatchedTensorSeq.from_seq_batch(torch.arange(10).view(5, 2))
+            >>> batch.align_as(batch_seq)
             tensor([[0, 2, 4, 6, 8],
-                    [1, 3, 5, 7, 9]], batch_dim=1, seq_dim=0)
+                    [1, 3, 5, 7, 9]], batch_dim=0, seq_dim=1)
         """
         if not isinstance(other, self.__class__):
             raise TypeError(
                 f"Incorrect type {type(other)}. No implementation available to `align_as` "
                 f"{type(self)} with {type(other)}"
             )
         return self.__class__(
@@ -891,14 +941,15 @@
             seq_dim=other.seq_dim,
         )
 
     def align_to_batch_seq(self) -> BatchedTensorSeq:
         r"""Aligns the current batch to the batch-sequence format.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: The batch in the batch-sequence
                 format.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -915,14 +966,15 @@
             seq_dim=1,
         )
 
     def align_to_seq_batch(self) -> BatchedTensorSeq:
         r"""Aligns the current batch to the sequence-batch format.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: The batch in the sequence-batch format.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -944,37 +996,35 @@
     def cat_along_seq(
         self, tensors: BatchedTensor | Tensor | Iterable[BatchedTensor | Tensor]
     ) -> BatchedTensorSeq:
         r"""Concatenates the data of the batch(es) to the current batch
         along the sequence dimension and creates a new batch.
 
         Args:
+        ----
             tensors (``BatchedTensorSeq`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A batch with the concatenated data
                 along the sequence dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.tensor([[0, 1, 2], [4, 5, 6]])).cat_along_seq(
-            ...     BatchedTensorSeq(torch.tensor([[10, 11], [12, 13]]))
-            ... )
+            >>> batch = BatchedTensorSeq(torch.tensor([[0, 1, 2], [4, 5, 6]]))
+            >>> batch.cat_along_seq(BatchedTensorSeq(torch.tensor([[10, 11], [12, 13]])))
             tensor([[ 0,  1,  2, 10, 11],
                     [ 4,  5,  6, 12, 13]], batch_dim=0, seq_dim=1)
-            >>> BatchedTensorSeq(
-            ...     torch.tensor([[0, 4], [1, 5], [2, 6]]),
-            ...     batch_dim=1,
-            ...     seq_dim=0,
-            ... ).cat_along_seq(
+            >>> batch = BatchedTensorSeq(torch.tensor([[0, 4], [1, 5], [2, 6]]), batch_dim=1, seq_dim=0)
+            >>> batch.cat_along_seq(
             ...     [
             ...         BatchedTensorSeq(torch.tensor([[10, 12], [11, 13]]), batch_dim=1, seq_dim=0),
             ...         BatchedTensorSeq(torch.tensor([[20, 22], [21, 23]]), batch_dim=1, seq_dim=0),
             ...     ]
             ... )
             tensor([[ 0,  4],
                     [ 1,  5],
@@ -991,14 +1041,15 @@
     ) -> None:
         r"""Concatenates the data of the batch(es) to the current batch
         along the sequence dimension.
 
         In-place version of ``cat_along_seq()``.
 
         Args:
+        ----
             tensors (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1010,15 +1061,15 @@
             tensor([[ 0,  1,  2, 10, 11],
                     [ 4,  5,  6, 12, 13]], batch_dim=0, seq_dim=1)
             >>> batch = BatchedTensorSeq(
             ...     torch.tensor([[0, 4], [1, 5], [2, 6]]),
             ...     batch_dim=1,
             ...     seq_dim=0,
             ... )
-            >>> batch.cat_along_seq(
+            >>> batch.cat_along_seq_(
             ...     [
             ...         BatchedTensorSeq(torch.tensor([[10, 12], [11, 13]]), batch_dim=1, seq_dim=0),
             ...         BatchedTensorSeq(torch.tensor([[20, 22], [21, 23]]), batch_dim=1, seq_dim=0),
             ...     ]
             ... )
             >>> batch
             tensor([[ 0,  4],
@@ -1031,42 +1082,47 @@
         """
         self.cat_(tensors, dim=self._seq_dim)
 
     def chunk_along_seq(self, chunks: int) -> tuple[BatchedTensorSeq, ...]:
         r"""Splits the batch into chunks along the sequence dimension.
 
         Args:
+        ----
             chunks (int): Specifies the number of chunks.
 
         Returns:
+        -------
             tuple: The batch split into chunks along the sequence
                 dimension.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).chunk_along_seq(chunks=3)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.chunk_along_seq(chunks=3)
             (tensor([[0, 1], [5, 6]], batch_dim=0, seq_dim=1),
              tensor([[2, 3], [7, 8]], batch_dim=0, seq_dim=1),
              tensor([[4], [9]], batch_dim=0, seq_dim=1))
         """
         return self.chunk(chunks, self._seq_dim)
 
     def index_select_along_seq(self, index: Tensor | Sequence[int]) -> BatchedTensorSeq:
         r"""Slices the batch along the sequence dimension at the given
         indices.
 
         Args:
+        ----
             index (``torch.Tensor`` or list or tuple): Specifies the
                 indices to select.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A new batch sliced along the sequence
                 dimension at the given indices.
 
         Example usage:
 
         .. code-block:: pycon
 
@@ -1091,74 +1147,82 @@
             mask = mask.data
         return self._create_new_batch(self._data.masked_fill(mask.data, value))
 
     def repeat_along_seq(self, repeats: int) -> BatchedTensorSeq:
         r"""Repeats the batch along the sequence dimension.
 
         Args:
+        ----
             repeats (int): Specifies the number of times to repeat
                 the batch along the sequence dimension.
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A repeated version of the input batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).repeat_along_seq(2)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.repeat_along_seq(2)
             tensor([[0, 1, 2, 3, 4, 0, 1, 2, 3, 4],
                     [5, 6, 7, 8, 9, 5, 6, 7, 8, 9]], batch_dim=0, seq_dim=1)
         """
         sizes = [1] * self._data.dim()
         sizes[self._seq_dim] = repeats
         return self._create_new_batch(self._data.repeat(*sizes))
 
     def select_along_seq(self, index: int) -> BatchedTensor:
         r"""Slices the batch along the sequence dimension at the given
         index.
 
         Args:
+        ----
             index (int): Specifies the index to select.
 
         Returns:
-            ``BatchedTensorSeq``: The batch sliced along the sequence
+        -------
+            ``BatchedTensor``: The batch sliced along the sequence
                 dimension at the given index.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).select_along_seq(2)
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.select_along_seq(2)
             tensor([2, 7], batch_dim=0)
         """
         return BatchedTensor(
             data=self._data.select(self._seq_dim, index),
             batch_dim=self._batch_dim if self._seq_dim > self._batch_dim else self._batch_dim - 1,
         )
 
     def slice_along_seq(
         self, start: int = 0, stop: int | None = None, step: int = 1
     ) -> BatchedTensorSeq:
         r"""Slices the batch in the sequence dimension.
 
         Args:
+        ----
             start (int, optional): Specifies the index where the
                 slicing of object starts. Default: ``0``
             stop (int, optional): Specifies the index where the
                 slicing of object stops. ``None`` means last.
                 Default: ``None``
             step (int, optional): Specifies the increment between
                 each index for slicing. Default: ``1``
 
         Returns:
+        -------
             ``BatchedTensorSeq``: A slice of the current batch.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
@@ -1181,30 +1245,31 @@
     ) -> tuple[BatchedTensorSeq, ...]:
         return self.split(split_size_or_sections, dim=self._seq_dim)
 
     def take_along_seq(self, indices: BaseBatch | Tensor | Sequence) -> BatchedTensorSeq:
         r"""Takes values along the sequence dimension.
 
         Args:
+        ----
             indices (``BaseBatch`` or ``Tensor`` or sequence):
                 Specifies the indices to take along the sequence
                 dimension.
 
         Returns:
-            ``BaseBatch``: The sequence with the selected data.
+        -------
+            ``BatchedTensorSeq``: The sequence with the selected data.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).take_along_seq(
-            ...     BatchedTensorSeq(torch.tensor([[3, 0, 1], [2, 3, 4]]))
-            ... )
+            >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
+            >>> batch.take_along_seq(BatchedTensorSeq(torch.tensor([[3, 0, 1], [2, 3, 4]])))
             tensor([[3, 0, 1],
                     [7, 8, 9]], batch_dim=0, seq_dim=1)
         """
         return self.take_along_dim(indices, dim=self._seq_dim)
 
     def unsqueeze(self, dim: int) -> BatchedTensorSeq:
         return self.__class__(
@@ -1225,22 +1290,32 @@
 
 
 def check_data_and_dims(data: Tensor, batch_dim: int, seq_dim: int) -> None:
     r"""Checks if the tensor ``data``, ``batch_dim`` and ``seq_dim`` are
     correct.
 
     Args:
+    ----
         data (``torch.Tensor``): Specifies the tensor in the batch.
         batch_dim (int): Specifies the batch dimension in the
             ``torch.Tensor`` object.
         seq_dim (int, optional): Specifies the sequence dimension in
             the ``torch.Tensor`` object.
 
     Raises:
+    ------
         RuntimeError: if one of the input is incorrect.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat.tensorseq import check_data_and_dims
+        >>> check_data_and_dims(torch.ones(2, 3), batch_dim=0, seq_dim=1)
     """
     if data.dim() < 2:
         raise RuntimeError(f"data needs at least 2 dimensions (received: {data.dim()})")
     if batch_dim < 0 or batch_dim >= data.dim():
         raise RuntimeError(
             f"Incorrect batch_dim ({batch_dim}) but the value should be in [0, {data.dim() - 1}]"
         )
@@ -1252,34 +1327,57 @@
         raise RuntimeError(f"batch_dim ({batch_dim}) and seq_dim ({seq_dim}) have to be different")
 
 
 def check_seq_dims(dims: set[int]) -> None:
     r"""Gets the sequence dimensions from the inputs.
 
     Args:
+    ----
         dims (set): Specifies the sequence dims to check.
 
     Raises:
+    ------
         RuntimeError if there are more than one sequence dimension.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat.tensorseq import get_seq_dims
+        >>> get_seq_dims({1})
     """
     if len(dims) != 1:
         raise RuntimeError(
             f"The sequence dimensions do not match. Received multiple values: {dims}"
         )
 
 
 def get_seq_dims(args: Iterable[Any, ...], kwargs: Mapping[str, Any] | None = None) -> set[int]:
     r"""Gets the sequence dimensions from the inputs.
 
     Args:
+    ----
         args: Variable length argument list.
         kwargs: Arbitrary keyword arguments.
 
     Returns:
+    -------
         set: The sequence dimensions.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> from redcat import BatchedTensorSeq
+        >>> from redcat.tensorseq import get_seq_dims
+        >>> get_seq_dims(
+        ...     args=(BatchedTensorSeq(torch.ones(2, 3)), BatchedTensorSeq(torch.ones(2, 6))),
+        ...     kwargs={"batch": BatchedTensorSeq(torch.ones(2, 4))},
+        ... )
+        {1}
     """
     kwargs = kwargs or {}
     dims = {val._seq_dim for val in args if hasattr(val, "_seq_dim")}
     dims.update({val._seq_dim for val in kwargs.values() if hasattr(val, "_seq_dim")})
     return dims
 
 
@@ -1420,23 +1518,25 @@
 
 def from_sequences(
     sequences: Iterable[torch.Tensor], padding_value: bool | int | float = 0
 ) -> BatchedTensorSeq:
     r"""Converts variable length sequences to a single padded tensor.
 
     Args:
+    ----
         sequences (iterable): Specifies an iterable over the variable
             length sequences. Each sequence is a ``torch.Tensor`` of
             shape ``(sequence_length, *)``. This function assumes
             trailing dimensions and type of all the tensors in
             sequences are same.
         padding_value (bool or int or float, optional): Specifies the
         padding value. Default: ``0``
 
     Returns:
+    -------
         ``BatchedTensorSeq``: A padded tensor. The underlying data is
             a ``torch.Tensor`` of shape
             ``(batch_size, sequence_length, *)``.
 
     Example usage:
 
     .. code-block:: pycon
```

### Comparing `redcat-0.0.6/src/redcat/utils/tensor.py` & `redcat-0.0.7/src/redcat/utils/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 import torch
 from torch import Tensor
 
 DeviceType = Union[torch.device, str, int]
 
 
 def align_to_batch_first(tensor: Tensor, batch_dim: int) -> Tensor:
-    r"""Aligns the input tensor format to ``(batch_size, *)`` where `*` means
-    any number of dimensions.
+    r"""Aligns the input tensor format to ``(batch_size, *)`` where `*`
+    means any number of dimensions.
 
     Args:
+    ----
         tensor (``torch.Tensor``): Specifies the tensor to change
             format.
         batch_dim (int): Specifies the batch dimension in the input
             tensor.
 
     Returns:
+    -------
         ``torch.Tensor``: A tensor of shape ``(batch_size, *)`` where
             `*` means any number of dimensions.
 
     Example usage:
 
     .. code-block:: pycon
 
@@ -56,25 +58,40 @@
 
 
 def align_to_batch_seq(tensor: Tensor, batch_dim: int, seq_dim: int) -> Tensor:
     r"""Aligns the input tensor format to ``(batch_size, sequence_length,
     *)`` where `*` means any number of dimensions.
 
     Args:
+    ----
         tensor (``torch.Tensor``): Specifies the tensor to change
             format.
         batch_dim (int): Specifies the batch dimension in the input
             tensor.
         seq_dim (int): Specifies the sequence dimension in the input
             tensor.
 
     Returns:
+    -------
         ``torch.Tensor``: A tensor of shape
             ``(batch_size, sequence_length, *)`` where `*` means any
             number of dimensions.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat.utils.tensor import align_to_batch_seq
+        >>> align_to_batch_seq(torch.arange(20).view(4, 5), batch_dim=1, seq_dim=0)
+        tensor([[ 0,  5, 10, 15],
+                [ 1,  6, 11, 16],
+                [ 2,  7, 12, 17],
+                [ 3,  8, 13, 18],
+                [ 4,  9, 14, 19]])
     """
     return tensor.permute(
         *compute_batch_seq_permutation(
             num_dims=tensor.dim(),
             old_batch_dim=batch_dim,
             old_seq_dim=seq_dim,
             new_batch_dim=0,
@@ -84,25 +101,40 @@
 
 
 def align_to_seq_batch(tensor: Tensor, batch_dim: int, seq_dim: int) -> Tensor:
     r"""Aligns the input tensor format to ``(sequence_length, batch_size,
     *)`` where `*` means any number of dimensions.
 
     Args:
+    ----
         tensor (``torch.Tensor``): Specifies the tensor to change
             format.
         batch_dim (int): Specifies the batch dimension in the input
             tensor.
         seq_dim (int): Specifies the sequence dimension in the input
             tensor.
 
     Returns:
+    -------
         ``torch.Tensor``: A tensor of shape
             ``(sequence_length, batch_size, *)`` where `*` means any
             number of dimensions.
+
+    Example usage:
+
+    .. code-block:: pycon
+
+        >>> import torch
+        >>> from redcat.utils.tensor import align_to_seq_batch
+        >>> align_to_seq_batch(torch.arange(20).view(4, 5), batch_dim=0, seq_dim=1)
+        tensor([[ 0,  5, 10, 15],
+                [ 1,  6, 11, 16],
+                [ 2,  7, 12, 17],
+                [ 3,  8, 13, 18],
+                [ 4,  9, 14, 19]])
     """
     return tensor.permute(
         *compute_batch_seq_permutation(
             num_dims=tensor.dim(),
             old_batch_dim=batch_dim,
             old_seq_dim=seq_dim,
             new_batch_dim=1,
@@ -118,21 +150,23 @@
     new_batch_dim: int,
     new_seq_dim: int,
 ) -> list[int]:
     r"""Computes the permutation to update the batch and sequence
     dimensions.
 
     Args:
+    ----
         num_dims (int): Specifies the number of dimensions.
         old_batch_dim (int): Specifies the old batch dimension.
         old_seq_dim (int): Specifies the old sequence dimension.
         new_batch_dim (int): Specifies the new batch dimension.
         new_seq_dim (int): Specifies the new sequence dimension.
 
     Returns:
+    -------
         list: The permutation to update the batch and sequence
             dimensions.
 
     Example usage:
 
     .. code-block:: pycon
 
@@ -175,22 +209,23 @@
         tuple: The available devices.
 
     Example usage:
 
     .. code-block:: pycon
 
         >>> from redcat.utils.tensor import get_available_devices
-        >>> get_available_devices()
-        ('cpu', 'cuda:0')
+        >>> get_available_devices()  # doctest:+ELLIPSIS
+        ('cpu'...)
     """
+    devices = ["cpu"]
     if torch.cuda.is_available():
-        return ("cpu", "cuda:0")
+        devices.append("cuda:0")
     if torch.backends.mps.is_available():
-        return ("cpu", "mps:0")
-    return ("cpu",)
+        devices.append("mps:0")
+    return tuple(devices)
 
 
 def get_torch_generator(
     random_seed: int = 1, device: torch.device | str | None = "cpu"
 ) -> torch.Generator:
     r"""Creates a ``torch.Generator`` initialized with a given seed.
 
@@ -209,21 +244,19 @@
     Example usage:
 
     .. code-block:: pycon
 
         >>> import torch
         >>> from redcat.utils.tensor import get_torch_generator
         >>> generator = get_torch_generator(42)
-        >>> torch.rand(2, 4, generator=generator)
-        tensor([[0.8823, 0.9150, 0.3829, 0.9593],
-                [0.3904, 0.6009, 0.2566, 0.7936]])
+        >>> torch.rand(2, 4, generator=generator)  # doctest:+ELLIPSIS
+        tensor([[...]])
         >>> generator = get_torch_generator(42)
-        >>> torch.rand(2, 4, generator=generator)
-        tensor([[0.8823, 0.9150, 0.3829, 0.9593],
-                [0.3904, 0.6009, 0.2566, 0.7936]])
+        >>> torch.rand(2, 4, generator=generator)  # doctest:+ELLIPSIS
+        tensor([[...]])
     """
     generator = torch.Generator(device)
     generator.manual_seed(random_seed)
     return generator
 
 
 def permute_along_dim(tensor: Tensor, permutation: Tensor, dim: int = 0) -> Tensor:
@@ -250,15 +283,18 @@
         >>> from redcat.utils.tensor import permute_along_dim
         >>> permute_along_dim(tensor=torch.arange(4), permutation=torch.tensor([0, 2, 1, 3]))
         tensor([0, 2, 1, 3])
         >>> permute_along_dim(
         ...     tensor=torch.arange(20).view(4, 5),
         ...     permutation=torch.tensor([0, 2, 1, 3]),
         ... )
-        tensor([[0, 1, 2, 3, 4], [10, 11, 12, 13, 14], [5, 6, 7, 8, 9], [15, 16, 17, 18, 19]])
+        tensor([[ 0,  1,  2,  3,  4],
+                [10, 11, 12, 13, 14],
+                [ 5,  6,  7,  8,  9],
+                [15, 16, 17, 18, 19]])
         >>> permute_along_dim(
         ...     tensor=torch.arange(20).view(4, 5),
         ...     permutation=torch.tensor([0, 4, 2, 1, 3]),
         ...     dim=1,
         ... )
         tensor([[ 0,  4,  2,  1,  3],
                 [ 5,  9,  7,  6,  8],
@@ -293,21 +329,25 @@
 
 
 def swap2(
     sequence: Tensor | np.ndarray | MutableSequence, index0: int, index1: int
 ) -> Tensor | np.ndarray | MutableSequence:
     r"""Swaps two values in a mutable sequence.
 
+    The swap is performed in-place.
+
     Args:
+    ----
         sequence (``torch.Tensor`` or ``numpy.ndarray`` or
             ``MutableSequence``): Specifies the sequence to update.
         index0 (int): Specifies the index of the first value to swap.
         index1 (int): Specifies the index of the second value to swap.
 
     Returns:
+    -------
         ``torch.Tensor`` or ``numpy.ndarray`` or ``MutableSequence``:
             The updated sequence.
 
     Example usage:
 
     .. code-block:: pycon
```

### Comparing `redcat-0.0.6/PKG-INFO` & `redcat-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause
 Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: coola (>=0.0.12,<1.0)
-Requires-Dist: numpy (>=1.24,<2.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: coola (>=0.0.15,<1.0)
+Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: torch (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/redcat
 Description-Content-Type: text/markdown
 
 # redcat
 
 <p align="center">
     <a href="https://github.com/durandtibo/redcat/actions">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.6 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.7 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries Requires-Dist: coola (>=0.0.12,<1.0) Requires-Dist:
-numpy (>=1.24,<2.0) Requires-Dist: torch (>=2.0.1,<3.0.0) Project-URL:
-Repository, https://github.com/durandtibo/redcat Description-Content-Type:
-text/markdown # redcat
+Development :: Libraries Requires-Dist: coola (>=0.0.15,<1.0) Requires-Dist:
+numpy (>=1.20,<2.0) Requires-Dist: torch (>=2.0,<3.0) Project-URL: Repository,
+https://github.com/durandtibo/redcat Description-Content-Type: text/markdown #
+redcat
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  0987ab26fe4d52025085/maintainability] [https://api.codeclimate.com/v1/badges/
                      0987ab26fe4d52025085/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
                                     [logo]
 --- *The logo was generated with Stable Diffusion 2.1*
```

