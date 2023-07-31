# Comparing `tmp/fatld-0.1.7.tar.gz` & `tmp/fatld-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fatld-0.1.7.tar", max compression
+gzip compressed data, was "fatld-0.1.8.tar", max compression
```

## Comparing `fatld-0.1.7.tar` & `fatld-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     3238 2023-07-03 09:25:25.776302 fatld-0.1.7/README.md
--rwxr-xr-x   0        0        0      147 2023-04-18 13:22:51.567061 fatld-0.1.7/fatld/__init__.py
--rwxr-xr-x   0        0        0    37463 2023-07-05 14:24:40.991279 fatld-0.1.7/fatld/design.py
--rwxr-xr-x   0        0        0     6794 2023-03-10 14:53:29.404853 fatld-0.1.7/fatld/main.py
--rwxr-xr-x   0        0        0     8448 2023-03-10 14:53:29.419886 fatld-0.1.7/fatld/relation.py
--rwxr-xr-x   0        0        0     1040 2023-07-05 13:00:57.622808 fatld-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 fatld-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0     3238 2023-07-03 09:25:25.776302 fatld-0.1.8/README.md
+-rwxr-xr-x   0        0        0      147 2023-04-18 13:22:51.567061 fatld-0.1.8/fatld/__init__.py
+-rwxr-xr-x   0        0        0    42796 2023-07-31 19:57:57.077647 fatld-0.1.8/fatld/design.py
+-rwxr-xr-x   0        0        0     6967 2023-07-31 19:57:57.091646 fatld-0.1.8/fatld/main.py
+-rwxr-xr-x   0        0        0     8611 2023-07-31 19:57:57.093684 fatld-0.1.8/fatld/relation.py
+-rwxr-xr-x   0        0        0     1040 2023-07-31 19:57:57.105173 fatld-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 fatld-0.1.8/PKG-INFO
```

### Comparing `fatld-0.1.7/README.md` & `fatld-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fatld-0.1.7/fatld/design.py` & `fatld-0.1.8/fatld/design.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,28 +43,28 @@
         Number of two-level factors in the design
     k : int
         Number of basic factors. Equals to the log2 of the runsize.
     p : int
         Number of added factors
 
     bf : List[int]
-        List of the column numbers of the basic factors not used in the pseudo-factors
-        `pf`.
+        List of the column numbers of the basic factors not used in the
+        pseudo-factors `pf`.
     pf : List[List[int]]
-        List of the pseudo-factors triplets (as lists of integers), used to define the
-        four-level factors.
+        List of the pseudo-factors triplets (as lists of integers), used to
+        define the four-level factors.
     af : List[int]
         List of the column numbers of the added factors
     cols : List[int]
         List of the column numbers of all the two-level factors of the design.
 
     array : np.ndarray
-        Design matrix of the design with the four-level factors first and then the
-        two-level factors. The two-level factors are ordered by column number and not
-        kept in the original order.
+        Design matrix of the design with the four-level factors first and then
+        the two-level factors. The two-level factors are ordered by column
+        number and not kept in the original order.
     """
 
     # TODO: refactor the docstring of the Design class
     def __init__(self, runsize: int, m: int, cols: list[int]):
         # TODO: think about a `strict` keyword
         # it would bypass columns check and uses only the columns suplied
         # Run size value check
@@ -87,19 +87,24 @@
                 """`m` must be lower of equal to `k/2`
                 Four-level factors are made of basic factors."""
             )
         self.m = m
 
         # Define the pseudo-factors based on the value of m
         self.pf = [
-            [2 ** (2 * m), 2 ** ((2 * m) + 1), 2 ** (2 * m) + 2 ** ((2 * m) + 1)]
+            [
+                2 ** (2 * m),
+                2 ** ((2 * m) + 1),
+                2 ** (2 * m) + 2 ** ((2 * m) + 1),
+            ]
             for m in range(self.m)
         ]
 
-        # Available basic factors are the ones not used in the four-level factors
+        # Available basic factors are the ones not used in the four-level
+        # factors
         all_basic_factors = [2**i for i in range(self.k)]
         self.bf = [i for i in all_basic_factors if i not in chain(*self.pf)]
 
         # Cols value check
         if not isinstance(cols, list):
             raise TypeError("`cols` must be a list of integer")
         if not all([isinstance(i, int) for i in cols]):
@@ -114,15 +119,16 @@
                 f"""Some column numbers are used to define pseudo-factors
                 for the four-level factor: {self.pf}"""
             )
         # User should know if columns are basic factors
         if any([i in self.bf for i in cols]):
             cols = [i for i in cols if i not in self.bf]
             warnings.warn(
-                f"Some column numbers are basic factors: {self.bf}", UserWarning
+                f"Some column numbers are basic factors: {self.bf}",
+                UserWarning,
             )
         # Number of added factors
         self.p = len(cols)
         # List of added factors
         self.af = cols
         self.af.sort()
         # List of all two-level columns in the design
@@ -134,15 +140,18 @@
         # Generate the design matrix
         # 4-level part
         coeff_matrix_4lvl = np.zeros((2 * self.m, self.m), dtype=int)
         bf_matrix = basic_factor_matrix(self.k)
         for i in range(self.m):
             idx = [2 * i, ((2 * i) + 1)]
             coeff_matrix_4lvl[idx, i] = [2, 1]
-        four_lvl_part = bf_matrix[:, 0 : (2 * self.m)] @ coeff_matrix_4lvl
+        end_four_lvl_part = 2 * self.m
+        four_lvl_part = (
+            bf_matrix[:, 0:end_four_lvl_part] @ coeff_matrix_4lvl
+        )  # noqa: E203
         # 2-level part
         two_lvl_part = custom_design(self.runsize, self.cols)
         # Assemble into one matrix
         self.array = np.concatenate([four_lvl_part, two_lvl_part], axis=1)
 
     def __str__(self):
         return f"4^{self.m} 2^{self.n}-{self.p} design in {self.runsize} runs"
@@ -151,140 +160,202 @@
         return f"Design(runsize={self.runsize}, m={self.m}, cols={self.af})"
 
     def twlp(
         self, type_0: bool = True, max_length: int | None = None
     ) -> list[list[int]]:
         """Type-specific word length pattern
 
-        Compute the type-specific word length pattern of a design, starting with words
-        of length 3.
+        Compute the type-specific word length pattern of a design, starting
+        with words of length 3.
 
         Parameters
         ----------
         type_0 : bool, optional
             Return the word length pattern of type 0, by default True.
             If False, return the word length pattern of type `m`.
         max_length : int, optional
-            Max word length to display in the word length pattern, by default None,
-            all the word lengths are displayed.
-            If this number is more than the maximum word length of the design, ignores
-            it.
+            Max word length to display in the word length pattern, by default
+            None, all the word lengths are displayed.
+            If this number is more than the maximum word length of the design,
+            ignores it.
 
         Returns
         -------
         List[List[int]]
             Type-specific word length pattern, starting with words of length 3.
-            Each sublist give the number of words of that length, sorted by type.
+            Each sublist give the number of words of that length, sorted by
+            type.
         """
         ar = oa.array_link(self.array)
         return twlp(ar, type_0, max_length)
 
     def wlp(self, max_length: int | None = None) -> list[int]:
         """Generalized word length pattern
 
-        Compute the word length pattern, i.e., the number of words in the defining
-        relation of the design, and arrange them by length.
+        Compute the word length pattern, i.e., the number of words in the
+        defining relation of the design, and arrange them by length.
 
         Parameters
         ----------
         max_length : int, optional
-            Max word length to display in the word length pattern, by default None,
-            all the word lengths are displayed.
-            If this number is more than the maximum word length of the design, ignores
-            it.
+            Max word length to display in the word length pattern, by default
+            None, all the word lengths are displayed.
+            If this number is more than the maximum word length of the design,
+            ignores it.
 
         Returns
         -------
         List[int]
             Word length pattern, starting with words of length 3.
         """
         ar = oa.array_link(self.array)
         wlp_list = list(map(int, ar.GWLP()[3:]))
-        if max_length is not None and (max_length <= 3 or max_length > len(wlp_list)):
+        if max_length is not None and (
+            max_length <= 3 or max_length > len(wlp_list)
+        ):
             warnings.warn("Wrong max_length value, ignoring")
             return wlp_list
         elif max_length is None:
             return wlp_list
         else:
-            return wlp_list[0 : (max_length - 2)]
+            return wlp_list[0 : (max_length - 2)]  # noqa: E203
 
-    def beta_wlp(self, max_length: int | None = None) -> tuple[list[float], list[int]]:
-        """
-        Find the permutation of the levels of the m four-level factors that minimize
-        the qWLP for the design.
+    def beta_star_wlp(
+        self, max_length: int | None = None
+    ) -> "tuple[list[tuple[float]], list[list[int]]]":
+        """Compute the 𝛽* vector for a design.
+        It contains tuples with the 𝛽*_i value, and the A_i^0 value for values
+        of i starting with 3.
 
         Parameters
         ----------
-        max_length : int, optional
-            Max word length to consider in the qWLP, by default None,
-            all the word lengths are computed (careful as it is computationally
-            intensive for large values of n).
+        design : fatld.Design
+            A design object
+        max_length : int | None
+            Maximum value of i for which the 𝛽* is computed. Default is None,
+            so all length are considered.
 
         Returns
         -------
-        best_wlp, permutations : tuple[list[float], list[int]]
-            Returns the minimal qWLP and the corresponding permutations of the
-            factor levels. The qWLP starts with words of length 3.
+        beta_star_vector : list[tuple[float | int]]
+            The 𝛽* vector with tuples of 𝛽* and A_i^0 values
+        perm : list[list[int]]
+            Permutation of the four-level factors associated with the 𝛽* vector
         """
-        # Declare global variables
-        global scaled_contrast_matrix
-
         # Compute the 12 basic permutations of the four levels
         perms = []
         for p in permutations(range(3)):
             for i in range(4):
                 ordering = list(p)
                 ordering.insert(i, 3)
                 perms.append(ordering)
         perms = perms[:12]
 
         # Compute all possible permutations for m factors
         all_perms = []
         for _, p in enumerate(product(range(12), repeat=self.m)):
             all_perms.append([perms[i] for i in p])
 
+        # Isolate four-level and two-level part of the design
+        m = self.m
+        fl_matrix = self.array[:, :m]
+        tl_matrix = self.array[:, m:]  # noqa: E201
+
+        # Build all interactions between all two-level factors
+        n = self.n
+        if max_length is None:
+            max_n_value = n
+        else:
+            max_n_value = max_length - 1
+        tfi_model_matrix = build_tfi_model_matrix(n=n, max_length=max_n_value)
+        tl_interaction_matrix = np.matmul(tl_matrix, tfi_model_matrix) % 2
+        tl_interaction_matrix = (2 * tl_interaction_matrix) - 1
+        tl_interaction_length = np.sum(tfi_model_matrix, axis=0).tolist()
+
         # Compute beta wlp for all permutations
-        a_vector_list = qwlp(
-            design=self, permutation_list=all_perms, max_length=max_length
-        )
+        beta_vector_list = []
+        for perms in all_perms:
+            beta_vector = compute_correlations(
+                tl_interaction_matrix=tl_interaction_matrix,
+                tl_interaction_length=tl_interaction_length,
+                fl_matrix=fl_matrix,
+                permutations_list=perms,
+                max_length=max_length,
+            )
+            beta_vector_list.append(beta_vector)
 
         # Find the best Beta vector and the corresponding permutation
-        best_vector = a_vector_list[0]
+        best_vector = beta_vector_list[0]
         best_perm = all_perms[0]
 
-        for i, v in enumerate(a_vector_list[1:]):
+        for i, v in enumerate(beta_vector_list[1:]):
             if best_vector > v:
                 best_vector = v
                 best_perm = all_perms[i]
 
-        return best_vector, best_perm
+        # Return a combination of the A_i^0 values and the beta values
+        beta_star_vector = []
+        twlp = self.twlp(type_0=True)
+        for i, x in enumerate(best_vector):
+            if i >= len(twlp):
+                beta_star_vector.append([x, 0])
+            else:
+                beta_star_vector.append([x, twlp[i][0]])
+
+        return beta_star_vector, best_perm
+
+    def beta_wlp(
+        self, max_length: int | None = None
+    ) -> tuple[list[float], list[int]]:
+        """
+        Find the permutation of the levels of the m four-level factors that
+        minimize the qWLP for the design.
+
+        Parameters
+        ----------
+        max_length : int, optional
+            Max word length to consider in the qWLP, by default None,
+            all the word lengths are computed (careful as it is computationally
+            intensive for large values of n).
+
+        Returns
+        -------
+        best_wlp, permutations : tuple[list[float], list[int]]
+            Returns the minimal qWLP and the corresponding permutations of the
+            factor levels. The qWLP starts with words of length 3.
+        """
+        beta_vector, perm = self.beta_star_wlp(max_length=max_length)
+        return [x[0] for x in beta_vector], perm
 
-    def w2_wlp(self) -> tuple[list[float], str]:
+    def w2_wlp(self) -> tuple[list[int], str]:
         """
         Compute the W_2 word length pattern of the design.
         The structure of the W_2 vector is:
         A3.0, A2.1, A4.0, A5.0, A3.1, A6.0, A7.0, ...
 
         Returns
         -------
-        W2_vector: list[float]
-            The vector containing the A_x.i values of the W_2 word length pattern
+        W2_vector: list[int]
+            The vector containing the A_x.i values of the W_2 word length
+            pattern
         factor: str
             A string indicating which factor must be used to obtain W_2 optimal
             blocking. Can either be 'A', 'B', or 'C'.
-            
+
         """
         design_oa = oa.array_link(self.array)
         design_wlp = list(map(int, design_oa.GWLP()))
 
         best_factor = "A"
         best_w2_vector = []
         for factor_index in range(self.m):
             # Remove the blocking factor and evaluate the WLP of the design
-            trmt_wlp = list(map(int, design_oa.deleteColumn(factor_index).GWLP()))
+            trmt_wlp = list(
+                map(int, design_oa.deleteColumn(factor_index).GWLP())
+            )
             block_wlp = [design_wlp[i] - x for i, x in enumerate(trmt_wlp)]
             w2_vector = build_w2_vector(block_wlp, trmt_wlp)
             # Set as default if it is the first factor we evaluate
             if factor_index == 0:
                 best_w2_vector = w2_vector
             else:
                 if w2_vector < best_w2_vector:
@@ -321,15 +392,17 @@
         omega_values = dict()
         for name, weight_vector in omega_weights.items():
             if len(name) == 2:
                 value = [w * a for w, a in zip(weight_vector, a3_vector)]
             else:
                 value = [w * a for w, a in zip(weight_vector, a4_vector)]
             omega_values[name] = sum(value)
-        alpha_wlp = [omega_values[i] for i in ["w4", "w2", "w42", "w22", "w44"]]
+        alpha_wlp = [
+            omega_values[i] for i in ["w4", "w2", "w42", "w22", "w44"]
+        ]
         if rounding:
             alpha_wlp = [round(i, 3) for i in alpha_wlp]
         return alpha_wlp
 
     def resolution(self) -> int | None:
         """
         Compute the resolution of the design.
@@ -358,69 +431,73 @@
         for i in range(self.m):
             flat_4lvl_part[:, 3 * i] = self.array[:, i] > 1
             flat_4lvl_part[:, (3 * i + 1)] = self.array[:, i] % 2 == 0
             # Using !XOR so that -/- and +/+ both give +
             flat_4lvl_part[:, (3 * i + 2)] = np.logical_not(
                 np.logical_xor(self.array[:, i] > 1, self.array[:, i] % 2 == 0)
             )
-        mat = np.concatenate((flat_4lvl_part, self.array[:, self.m :]), axis=1)
+        mat = np.concatenate(
+            (flat_4lvl_part, self.array[:, self.m :]), axis=1  # noqa: E203
+        )
         if zero_coding is False:
             return mat * 2 - 1
         else:
             return mat
 
     def tfi_clearance(self) -> dict[str, dict[str, object]]:
         """
         Compute clarity of all two-factor interactions in the design.
 
         There are three types of two-factor interactions in a design:
 
         - 4-4: interaction between two pseudo-factors of four-level factors
         - 4-2: interaction between a pseudo-factor of a four-level factor and
-          a two-level factor.
+               a two-level factor.
         - 2-2: interaction between two two-level factors.
 
-        An interaction is called clear when it is not aliased with any other interaction
-        of a specific type. Thus, an interaction is '4-4 clear' when it is not aliased
-        with any 4-4 interactions, '4-2 clear' when it is not aliased with any 4-2
-        interactions, and '2-2 clear' when it is not aliased with any 2-2 interactions.
-        When an interaction is 4-4 clear, 4-2 clear, and 2-2 clear, we call it a
-        "totally clear (TC)" interaction.
+        An interaction is called clear when it is not aliased with any other
+        interaction of a specific type. Thus, an interaction is '4-4 clear'
+        when it is not aliased with any 4-4 interactions, '4-2 clear' when it
+        is not aliased with any 4-2 interactions, and '2-2 clear' when it is
+        not aliased with any 2-2 interactions.
+        When an interaction is 4-4 clear, 4-2 clear, and 2-2 clear, we call it
+        a totally clear (TC)" interaction.
         Defining how clear is an interaction, is called the *clarity* of an
         interaction.
 
         Returns
         -------
 
-        A dictionary where each entry corresponds to an interaction of the design,
-        where the key is the name of the interaction, and the value is another
-        dictionary containing four entries:
+        A dictionary where each entry corresponds to an interaction of the
+        design, where the key is the name of the interaction, and the value is
+        another dictionary containing four entries:
 
             - 'clear': the interaction is clear from main effects
             - '4-4': the interaction is '4-4' clear (True or False)
             - '4-2': the interaction is '4-2' clear (True or False)
             - '2-2': the interaction is '2-2' clear (True or False)
-            - 'Type': the type of the interaction, either '4-4', '4-2', or '2-2'
+            - 'Type': the type of the interaction, either '4-4', '4-2',
+            or '2-2'
 
         """
         # LABELS
         # MAIN EFFECTS
 
         # 4lvl PF are labeled as uppercase + index i = 1,2,3
         label_list_4lvl_pf = [
             [f"{chr(65 + i)}{j}" for j in [1, 2, 3]] for i in range(self.m)
         ]
         # 2lvl factors labeled as lowercase
         label_list_2lvl = [chr(97 + i) for i in range(self.n)]
 
         # TWO-FACTOR-INTERACTIONS
 
-        # Combinations of PF from the same four-level factors cannot be considered as
-        # for any PF, p1 x p2 = p3 so combine BETWEEN the pseudo-factors triplets and
-        # not within
+        # Combinations of PF from the same four-level factors cannot be
+        # considered as for any PF, p1 x p2 = p3 so combine BETWEEN the
+        # pseudo-factors triplets and not within
         if self.m > 1:
             label_list_44_tfi = list(
                 chain(
                     *[
                         [f"{i}.{j}" for i in x for j in y]
                         for x, y in combinations(label_list_4lvl_pf, 2)
                     ]
@@ -431,18 +508,22 @@
             label_list_44_tfi = []
         # A 4-2 interaction is any combination of a PF and a two-level factor
         label_list_42_tfi = [
             f"{i}.{j}"
             for i in list(chain(*label_list_4lvl_pf))
             for j in label_list_2lvl
         ]
-        label_list_22_tfi = [f"{i}.{j}" for i, j in combinations(label_list_2lvl, 2)]
+        label_list_22_tfi = [
+            f"{i}.{j}" for i, j in combinations(label_list_2lvl, 2)
+        ]
 
         # All combinations of labels are all the TFI
-        label_list_tfi = label_list_44_tfi + label_list_42_tfi + label_list_22_tfi
+        label_list_tfi = (
+            label_list_44_tfi + label_list_42_tfi + label_list_22_tfi
+        )
 
         # MATRIX
 
         # Zero coding (0/1) is needed to perform multiplication of factors
         flat_array_coded = self.flatten(zero_coding=False)
 
         # MAIN EFFECTS
@@ -476,15 +557,21 @@
                     for i in range(3 * x, (3 * x) + 3)
                     for j in range(3 * y, (3 * y) + 3)
                 ]
                 for x, y in combinations(range(self.m), 2)
             ]
             matrix_44_tfi = np.hstack(list(chain(*list_44_tfi)))
             effect_mat = np.concatenate(
-                (matrix_44_tfi, matrix_42_tfi, matrix_22_tfi, matrix_2_me, matrix_4_me),
+                (
+                    matrix_44_tfi,
+                    matrix_42_tfi,
+                    matrix_22_tfi,
+                    matrix_2_me,
+                    matrix_4_me,
+                ),
                 axis=1,
             )
             # We don't need to define clarity for the ME
             tfi_mat = np.concatenate(
                 (matrix_44_tfi, matrix_42_tfi, matrix_22_tfi),
                 axis=1,
             )
@@ -503,15 +590,17 @@
 
         # tfi can be one of three types: 4-4, 4-2, or 2-2
         type_list_tfi = (
             ["4-4"] * len(label_list_44_tfi)
             + ["4-2"] * len(label_list_42_tfi)  # noqa : W503
             + ["2-2"] * len(label_list_22_tfi)  # noqa : W503
             + ["clear"]  # noqa : W503
-            * (len(label_list_2lvl) + 3 * len(label_list_4lvl_pf))  # noqa : W503
+            * (
+                len(label_list_2lvl) + 3 * len(label_list_4lvl_pf)
+            )  # noqa : W503
         )
 
         # All alias-related variables are NA and will be filled later on
         tfi = dict()
         for tfi_idx, label in enumerate(label_list_tfi):
             tfi_type = type_list_tfi[tfi_idx]
             tfi[label] = {
@@ -538,16 +627,16 @@
         """
         Generate the clarity matrix of the design.
 
         The clarity matrix is a table where:
 
         - the rows represent the type of the interactions (4-4, 4-2, 2-2,
             or any type)
-        - the columns represent the type of clarity that the interactions can have (
-            4-4 clear, 4-2 clear, 2-2 clear, or totally clear)
+        - the columns represent the type of clarity that the interactions can
+            have (4-4 clear, 4-2 clear, 2-2 clear, or totally clear)
 
         Returns
         -------
         clarity_matrix
             A pandas dataframe holding the clarity matrix where the rows are
             ["4-4", "4-2", "2-2", "Any type"] and the columns are ["4-4 clear",
             "4-2 clear", "2-2 clear", "Totally clear"]
@@ -561,39 +650,42 @@
         tfi = self.tfi_clearance()
         for interaction in tfi.values():
             int_type = interaction["Type"]
             all_clear = 0
             for clear_type in ["4-4", "4-2", "2-2"]:
                 if interaction[clear_type]:
                     column_label = f"{clear_type} clear"
-                    clarity_df.loc[int_type, column_label] += 1  # type: ignore
-                    clarity_df.loc["Any type", column_label] += 1  # type: ignore
+                    clarity_df.loc[int_type, column_label] += 1
+                    clarity_df.loc["Any type", column_label] += 1
                     all_clear += 1
                 if all_clear == 3:
-                    clarity_df.loc[int_type, "Totally clear"] += 1  # type: ignore
-                    clarity_df.loc["Any type", "Totally clear"] += 1  # type: ignore
+                    clarity_df.loc[int_type, "Totally clear"] += 1
+                    clarity_df.loc["Any type", "Totally clear"] += 1
         return clarity_df
 
     def clear(self, interaction_type: str, clear_from: str = "all") -> int:
         """
-        Compute the number of interactions of type `interaction_type` that are clear
-        from interactions of the `clear_from` type.
+        Compute the number of interactions of type `interaction_type` that are
+        clear from interactions of the `clear_from` type.
 
         Parameters
         ----------
         interaction_type : str
-            Type of the interaction studied. Can either be "4-4", "4-2", "2-2", or "all"
-            to count for all types of interaction.
+            Type of the interaction studied. Can either be "4-4", "4-2", "2-2",
+            or "all" to count for all types of interaction.
         clear_from : str
-            Type of clarity to count. Can either be "4-4", "4-2", "2-2", or "all" to
-            count the number of totally clear interaction.
+            Type of clarity to count. Can either be "4-4", "4-2", "2-2", or
+            "all" to count the number of totally clear interaction.
 
         """
         possible_types = ["4-4", "4-2", "2-2", "all"]
-        if interaction_type not in possible_types or clear_from not in possible_types:
+        if (
+            interaction_type not in possible_types
+            or clear_from not in possible_types
+        ):
             raise ValueError(
                 """
                 Wrong type of interaction provided.
                 Must be one of '4-4', '4-2', '2-2' or 'all'.
                 """
             )
         tfi = self.tfi_clearance()
@@ -609,74 +701,81 @@
         return count
 
     def defining_relation(self, raw: bool = False):
         """
         Generate the defining relation of the design.
 
         For each added factor, generate the word representing the added factor.
-        Each word contains the generator + the letter representing the added factor.
-        The pseudo-factors used to generate the four-level factors are replaced by
-        four-level factors labels in the final words.
-        For example, if factor `A` is created using pseudo-factors `a`, `b` and `ab`,
-        then the replacement scheme is: `a -> A1`, `b -> A2`, and `ab -> A3`.
+        Each word contains the generator + the letter representing the added
+        factor.
+        The pseudo-factors used to generate the four-level factors are replaced
+        by four-level factors labels in the final words.
+        For example, if factor `A` is created using pseudo-factors `a`, `b`
+        and `ab`, then the replacement scheme is: `a -> A1`, `b -> A2`,
+        and `ab -> A3`.
 
         Parameters
         ----------
         raw : bool, optional
-            Return the relation without replacing the pseudo-factors by their four-level
-            factor label, by default False
+            Return the relation without replacing the pseudo-factors by their
+            four-level factor label, by default False
 
         Returns
         -------
         Relation
             Defining relation as a ``Relation`` object.
         """
         relation = [
-            f"{num2gen(x)}{chr(97 + self.k + i)}" for i, x in enumerate(self.af)
+            f"{num2gen(x)}{chr(97 + self.k + i)}"
+            for i, x in enumerate(self.af)
         ]
         return Relation(words=relation, m=self.m)
 
     def add_factor(self, number: int):
         """
         Add a two-level factor to the design.
 
-        Generate a design with an added two-level factor defined by the number supplied.
+        Generate a design with an added two-level factor defined by the number
+        supplied.
 
         Parameters
         ----------
         number : int
-            Column number of the factor to add. Cannot correspond to a column number
-            already in use (as two-level factor or pseudo-factor) in the design.
+            Column number of the factor to add. Cannot correspond to a column
+            number already in use (as two-level factor or pseudo-factor) in the
+            design.
 
         Returns
         -------
         Design
             A `Design` object containing the added two-level factor
 
         """
         # Factor cannot be used in the columns, the pf or be out of range
         if number < 0 or number >= self.runsize:
             raise ValueError(
                 """Supplied column number must be greater than zero and less
                    than the runsize."""
             )
         if number in self.cols or number in list(chain(*self.pf)):
-            raise ValueError(f"Column number {number} already used in the design")
+            raise ValueError(
+                f"Column number {number} already used in the design"
+            )
         new_cols = self.af + [number]
         return Design(self.runsize, self.m, new_cols)
 
     def remove_factor(self, number: int):
         """
         Remove a two-level factor from the design.
 
         Parameters
         ----------
         number : int
-            Column number of the factor to remove. Must correspond to one of the factor
-            used in the design.
+            Column number of the factor to remove. Must correspond to one of
+            the factor used in the design.
 
         Returns
         -------
         Design
             A `Design` object containing the added two-level factor
 
         """
@@ -695,15 +794,16 @@
     Create a Design object from a matrix.
 
     Parameters
     ----------
     mat : np.ndarray
         Design matrix
     zero_coded : bool, optional
-        The two-level factors in the design matrix are coded in 0/1, by default True.
+        The two-level factors in the design matrix are coded in 0/1, by
+        default True.
 
     Returns
     -------
     Design
         A Design object with the factors detected in the matrix.
     """
     # Define runsize
@@ -732,173 +832,250 @@
     cols_id, _ = np.nonzero(cols_mat)
     cols_gen = [labels_list[i] for i in cols_id]
     cols_num = [gen2num(i) for i in cols_gen]
     added_cols = [i for i in cols_num if np.log2(i) % 1 != 0]
     return Design(run_size, n_flvl, added_cols)
 
 
-def qwlp(
-    design: Design,
-    permutation_list: list[list[list[int]]],
-    max_length: None | int = None,
-) -> list[list[float]]:
-    """
-    Compute the beta WLP of the design.
+def fl_to_contrast(
+    fl_matrix: np.ndarray,
+    scaled_contrast_matrix: np.ndarray,
+    permutations_list: "list[list[int]]",
+) -> np.ndarray:
+    """Decompose each four-level factor of `fl_matrix` into its three
+    polynomial components: linear (L), quadratic (Q), and cubic (C) and apply a
+    specific permutation to each factor.
 
     Parameters
     ----------
-    design : fatld.Design
-        Four-and-two-level design
-    permutation_list : list[list[list[int]]]
-        List of permutations for the m four-level factors.
-        Each permutation is a list of m sublists, where each sublist corresponds to the
-        ordering of the levels of a four-level factor (of the form [0,1,2,3]).
-    max_length : None | int, optional
-        Maximum length of words considered in the beta WLP, by default None so that all
-        the word lengths are considered.
+    fl_matrix : np.ndarray
+        2D array of size N by m containing the m four-level factors with levels
+        0, 1, 2, and 3.
+    scaled_contrast_matrix : np.ndarray
+        2D array of size 4 by 3 containing the scaled polynomial contrasts.
+        The four rows correspond to the four levels of a four-level factor,
+        while the three columns correspond to the 3 polynomial contrasts:
+        linear (L), quadratic (Q), and cubic (C).
+    permutations_list : list[list[int]]
+        List of length m containing the permutations for the levels of each
+        four-level factor.
+        Each permutation must be a list of length four containing the levels 0,
+        1, 2, and 3 in a specific order.
 
     Returns
     -------
-    beta_wlp : list[list[float]]
-        List of vectors of the Aq values starting with words of length 3.
-        Each vector in the list corresponds to the beta wlp for the corresponding
-        permutation in `permutation_list`.
-    """
-    # Declare global variables
-    global scaled_contrast_matrix
+    np.ndarray
+        2D array of size N by 3*m containing the LQC-decomposed four-level
+        factors with the permutations applied.
 
-    design_matrix = design.array
-    m = design.m
-    n = design.n
-    N = design.runsize
-
-    # Each permutation must contain m sublists
-    if any([len(i) != m for i in permutation_list]):
-        raise ValueError("Each permutation must contain m sublists")
-    # Each sublist in a permutation has to contain only 0,1,2,3
-    for p in permutation_list:
-        if any([len(i) != 4 for i in p]):
-            raise ValueError("Each sublist in a permutation must contain four elements")
-
-        if any([i not in [0, 1, 2, 3] for x in p for i in x]):
-            raise ValueError("Sublists in permutations can only contain 0, 1, 2, or 3")
-
-    # Isolate four-level and two-level part of the design
-    fl_matrix = design_matrix[:, :m]
-    tl_matrix = design_matrix[:, m:]
+    Raises
+    ------
+    ValueError
+        permutations_list must have the same length as the number of columns in
+        the fl_matrix.
+    :meta private:
+    """
+    # There must be one permutation for each 4LF
+    N, m = fl_matrix.shape
+    if len(permutations_list) != m:
+        raise ValueError("permutations_list must have length %i" % m)
+
+    # Matrix holding all contrasts for m 4LFs
+    fl_contrast_matrix = np.zeros((N, 3 * m), dtype=float)
+
+    # Apply each permutation to the contrast matrix sequentially
+    for fl_index, permutation in enumerate(permutations_list):
+        perm_contrast_matrix = scaled_contrast_matrix[permutation, :]
+        # Iterate over the permutated contrast matrix
+        for index, contrast_value in np.ndenumerate(perm_contrast_matrix):
+            i, j = index  # Unfold index for easier array indexing
+            # Fnd rows in 4lf equal to i
+            row_indices = fl_matrix[:, fl_index] == i
+            # Set these rows equal to the contrast value
+            fl_contrast_matrix[row_indices, 3 * fl_index + j] = contrast_value
+
+    return fl_contrast_matrix
+
+
+def contrast_interactions(
+    fl_contrast_matrix: np.ndarray, m: int
+) -> "tuple[np.ndarray, list[int]]":
+    """Compute all interactions of order 1 up to `m` for `m` four-level factors
+    decomposed into their LQC contrasts.
 
-    # Build all interactions between all two-level factors
-    if max_length is None:
-        max_n_value = n
-    else:
-        max_n_value = max_length - 1
-    tfi_model_matrix = build_tfi_model_matrix(n=n, max_length=max_n_value)
-    tl_interaction_matrix = np.matmul(tl_matrix, tfi_model_matrix) % 2
-    tl_interaction_matrix = (2 * tl_interaction_matrix) - 1
-    tl_interaction_length = np.sum(tfi_model_matrix, axis=0).tolist()
-
-    # Empty list to hold the Beta vectors for all the permutations
-    a_vectors_list = []
-    for single_permutation in permutation_list:
-        # Unfold the four-level factors into L, Q, C matrices
-        fl_contrast_list = []
-        for x in range(m):
-            permutation = single_permutation[x]
-            mix_contrast_matrix = scaled_contrast_matrix[permutation, :]
-            single_fl_contrast_matrix = np.zeros((N, 3))
-            for i in range(4):
-                single_fl_contrast_matrix[
-                    fl_matrix[:, x] == i, :
-                ] = mix_contrast_matrix[  # noqa: E201
-                    i, :
-                ]
-            fl_contrast_list.append(single_fl_contrast_matrix)
-        fl_contrast_matrix = np.hstack(fl_contrast_list)
+    Parameters
+    ----------
+    fl_contrast_matrix : np.ndarray
+        2D array of size N by 3*m containing the LQC-decomposition of the m
+        four-level factors.
+    m : int
+        Number of four-level factors.
 
-        # Initialize the length and type vectors
-        fl_contrast_length = [i + 1 for _ in range(m) for i in range(3)]
+    Returns
+    -------
+    fl_full_contrast_matrix : np.ndarray
+        2D array containing all interactions between the LQC contrasts of m
+        four-level factors.
+    fl_contrast_length :  list[int]
+        List containing the order (L is 1, Q is 2, and C is 3) of all the
+        interactions generated
+
+    Raises
+    ------
+    ValueError
+        The number of four-level factors `m` must be either 1, 2, or 3.
+    """
+    # Number of 4LF is either 1, 2, or 3
+    if m not in [1, 2, 3]:
+        raise ValueError("`m` must be 1, 2, or 3.")
+
+    # Contrast length is 1, 2, 3 for L, Q, C
+    fl_contrast_length = [i + 1 for _ in range(m) for i in range(3)]
+
+    # Number of runs to define empty matrices
+    N = fl_contrast_matrix.shape[0]
+
+    # No interaction can be created with one four-level factor
+    if m == 1:
+        fl_full_contrast_matrix = fl_contrast_matrix
+
+    # Main effects for the two four-level factors and the 3^2 interactions
+    # between the 6 terms.
+    elif m == 2:
+        fl_contrast_interaction_matrix = np.zeros((N, 9), dtype=float)
+        for fac_idx, pair in enumerate(product([0, 1, 2], [3, 4, 5])):
+            fl_contrast_interaction_matrix[:, fac_idx] = np.prod(
+                fl_contrast_matrix[:, pair], axis=1
+            )
+            normalized_indices = [i % 3 for i in pair]
+            fl_contrast_length.append(sum(normalized_indices) + 2)
+        fl_full_contrast_matrix: np.ndarray = np.hstack(
+            (fl_contrast_matrix, fl_contrast_interaction_matrix)
+        )
 
-        # No interaction can be created
-        if m == 1:
-            fl_full_contrast_matrix = fl_contrast_matrix
-        # Main effects for the two four-level factors and the 3^2 interactions between
-        # the 6 terms.
-        elif m == 2:
-            fl_contrast_interaction_list = []
-            for p in product(range(3), repeat=2):
-                new_p = [x + (3 * i) for i, x in enumerate(p)]
-                single_fl_contrast_interaction_vector = np.prod(
-                    fl_contrast_matrix[:, new_p], axis=1
+    # Three different terms:
+    # - Main effects for the 3 four-level factors (3*3=9 terms)
+    # - Interactions between 2 of the 3 four-level factors (3 ways of
+    # creating 9)
+    # - Interactions between the 3 four-level factors (27 terms)
+    elif m == 3:
+        # Interactions between 2 of the 3 four-level factors
+        fl_contrast_2f_interaction_matrix = np.zeros((N, 27), dtype=float)
+        for comb_idx, combi in enumerate([(0, 1), (0, 2), (1, 2)]):
+            range1 = [3 * combi[0], 3 * combi[0] + 1, 3 * combi[0] + 2]
+            range2 = [3 * comb[1], 3 * comb[1] + 1, 3 * comb[1] + 2]
+            for pair_idx, pair in enumerate(product(range1, range2)):
+                index = 9 * comb_idx + pair_idx
+                fl_contrast_2f_interaction_matrix[:, index] = np.prod(
+                    fl_contrast_matrix[:, pair], axis=1
                 )[:, None]
-                fl_contrast_interaction_list.append(
-                    single_fl_contrast_interaction_vector
-                )
-                fl_contrast_length.append(sum(p) + 2)
-            fl_contrast_interaction_matrix = np.hstack(fl_contrast_interaction_list)
-            fl_full_contrast_matrix = np.concatenate(
-                (fl_contrast_matrix, fl_contrast_interaction_matrix), axis=1
-            )
-        # Three different terms:
-        # - Main effects for the 3 four-level factors (3*3=9 terms)
-        # - Interactions between 2 of the 3 four-level factors (3 ways of creating 9)
-        # - Interactions between the 3 four-level factors (27 terms)
-        elif m == 3:
-            # Interactions between 2 of the 3 four-level factors
-            fl_contrast_interaction_list = []
-            for c in combinations(range(3), 2):
-                for p in product(range(3), repeat=2):
-                    new_p = [3 * c[i] + x for i, x in enumerate(p)]
-                    single_fl_contrast_interaction_vector = np.prod(
-                        fl_contrast_matrix[:, new_p], axis=1
-                    )[:, None]
-                    fl_contrast_interaction_list.append(
-                        single_fl_contrast_interaction_vector
-                    )
-                    fl_contrast_length.append(sum(p) + 2)
-
-            # Interactions between 3 four-level factors
-            for p in product(range(3), repeat=3):
-                # p is a tuple with two numbers corresponding with the polynomial
-                # contrasts chosen for the product
-                new_p = [3 * i + x for i, x in enumerate(p)]
-                single_fl_contrast_interaction_vector = np.prod(
-                    fl_contrast_matrix[:, new_p], axis=1
-                )[:, None]
-                fl_contrast_interaction_list.append(
-                    single_fl_contrast_interaction_vector
-                )
-                fl_contrast_length.append(sum(p) + 3)
-            fl_contrast_interaction_matrix = np.hstack(fl_contrast_interaction_list)
-            fl_full_contrast_matrix = np.concatenate(
-                (fl_contrast_matrix, fl_contrast_interaction_matrix), axis=1
-            )
-        else:
-            raise ValueError("Unknown m value: %i" % m)
+                normalized_indices = [i % 3 for i in pair]
+                fl_contrast_length.append(sum(normalized_indices) + 2)
 
-        # Build word length vector
-        word_length = (
-            np.array(fl_contrast_length)[:, None].T
-            + np.array(tl_interaction_length)[:, None]  # noqa: W503
+        # Interactions between 3 four-level factors
+        fl_contrast_3f_interaction_matrix = np.zeros((N, 27), dtype=float)
+        for triplet_idx, triplet in enumerate(
+            product([0, 1, 2], [3, 4, 5], [6, 7, 8])
+        ):
+            fl_contrast_3f_interaction_matrix[:, triplet_idx] = np.prod(
+                fl_contrast_matrix[:, triplet], axis=1
+            )[:, None]
+            normalized_indices = [i % 3 for i in triplet]
+            fl_contrast_length.append(sum(normalized_indices) + 3)
+
+        # Join ME, 2FI, and 3FI into a single matrix
+        fl_full_contrast_matrix: np.ndarray = np.hstack(
+            (
+                fl_contrast_matrix,
+                fl_contrast_2f_interaction_matrix,
+                fl_contrast_3f_interaction_matrix,
+            )
         )
+    return fl_full_contrast_matrix, fl_contrast_length  # type: ignore
 
-        # Compute squared correlations
-        correlation = (tl_interaction_matrix.T @ fl_full_contrast_matrix) / N
-        correlation_sq = np.round(correlation**2, 2)
 
-        # Compute Beta values
-        if max_length is None:
-            max_Aq_length = int(np.amax(word_length)) + 1
-        else:
-            max_Aq_length = max_length + 1
-        a_vector = []
-        for length in range(3, max_Aq_length):
-            a_value = np.round(np.sum(correlation_sq[word_length == length]), 2)
-            a_vector.append(a_value)
-        a_vectors_list.append(a_vector)
-    return a_vectors_list
+def compute_correlations(
+    tl_interaction_matrix: np.ndarray,
+    tl_interaction_length: "list[int]",
+    fl_matrix: np.ndarray,
+    permutations_list: "list[list[int]]",
+    max_length: int | None = None,
+) -> "list[float]":
+    """Compute the squared correlations between the two-level
+    factors, and the LQC decomposition of the four-level factors.
+    Summarise the correlations by summing them by interaction order.
+
+    For example, an interaction between a xyz interaction (order 3) and a Q
+    component (order 2), has order 5.
+
+    Parameters
+    ----------
+    tl_interaction_matrix : np.ndarray
+        2D array containing all interactions between two-level factors.
+    tl_interaction_length : list[int]
+        A list containing the order of all interactions between two-level
+        factors. It must have the same size as the number of columns in
+        `tl_interaction_matrix`.
+    fl_matrix : np.ndarray
+        2D array of size N by m containing the four-level factors.
+    permutations_list : list[list[int]]
+        List of length m containing the permutations for the levels of each
+        four-level factor.
+        Each permutation must be a list of length four containing the levels 0,
+        1, 2, and 3 in a specific order.
+    max_length : int | None, optional
+        Maximum order to consider when summing the correlations. Default is
+        None so all orders are considered.
+
+    Returns
+    -------
+    beta_vector : list[float]
+        A list of the summed squared correlations, starting with order 3 and
+        going up to order `max_length`.
+    """
+    # Declare global variables
+    global scaled_contrast_matrix
+
+    # Compute runsize and number of four-level factors
+    N, m = fl_matrix.shape
+
+    # Unfold and permute levels of 4LFs
+    fl_contrast_matrix = fl_to_contrast(
+        fl_matrix=fl_matrix,
+        scaled_contrast_matrix=scaled_contrast_matrix,
+        permutations_list=permutations_list,
+    )
+
+    # Length of the contrasts unfolded from the 4LF
+    fl_full_contrast_matrix, fl_contrast_length = contrast_interactions(
+        fl_contrast_matrix=fl_contrast_matrix, m=m
+    )
+
+    # Build word length vector
+    word_length = (
+        np.array(fl_contrast_length)[:, None].T
+        + np.array(tl_interaction_length)[:, None]
+    )
+
+    # Compute squared correlations
+    correlation = (tl_interaction_matrix.T @ fl_full_contrast_matrix) / N
+    correlation_sq = np.round(correlation**2, 2)
+
+    # Compute Beta values
+    max_possible_length = max(fl_contrast_length) + max(tl_interaction_length)
+    if max_length is None:
+        max_Aq_length = max_possible_length
+    else:
+        max_Aq_length = max_length + 1
+    beta_vector = []
+    for length in range(3, max_Aq_length):
+        beta_value = np.round(np.sum(correlation_sq[word_length == length]), 2)
+        beta_vector.append(beta_value)
+
+    return beta_vector
 
 
 def nbr_interactions(n: int, max_length: int) -> int:
     """
     Compute the total number of interactions between i factors among n, where i
     ranges between 1 and max_length.
     """
@@ -906,49 +1083,55 @@
     for i in range(max_length):
         val += comb(n, (i + 1))
     return val
 
 
 def build_tfi_model_matrix(n: int, max_length: int) -> np.ndarray:
     """
-    Build the model matrix to compute all interactions between i factors among n
-    with i ranging from 1 to n.
-    In this model matrix, a 1 represents an active factor in the interaction, while
-    a 0 zero represents an inactive factor.
+    Build the model matrix to compute all interactions between i factors among
+    n with i ranging from 1 to n.
+    In this model matrix, a 1 represents an active factor in the interaction,
+    while a 0 zero represents an inactive factor.
 
     Parameters
     ----------
     n : int
         Number of two-level factors
     max_length : int
         Maximum number of factors to consider in the interactions.
-        For example, for a two-factor interaction, max_length should be equal to 2.
+        For example, for a two-factor interaction, max_length should be equal
+        to 2.
 
     Returns
     -------
     np.ndarray
-        Model matrix of size n-by-s, where s is the total number of interactions.
+        Model matrix of size n-by-s, where s is the total number of
+        interactions.
     """
     # Initialize matrix
-    tfi_model_matrix = np.zeros((n, nbr_interactions(n, max_length)), dtype=int)
+    tfi_model_matrix = np.zeros(
+        (n, nbr_interactions(n, max_length)), dtype=int
+    )
     # Ones represent an active factor in the interaction
     index = 0
     for i in range(max_length):
         for c in combinations(range(n), i + 1):
             tfi_model_matrix[c, index] = 1
             index += 1
     return tfi_model_matrix
 
 
-def build_w2_vector(blocking_wlp: list[int], treatment_wlp: list[int]) -> list[int]:
+def build_w2_vector(
+    blocking_wlp: list[int], treatment_wlp: list[int]
+) -> list[int]:
     """
-    Compute the W_2 word length pattern (WLP) of a design, given its treatment WLP and
-    blocking WLP.
-    Both WLP must start with words of length 0 (so that list indices matches word
-    lengths).
+    Compute the W_2 word length pattern (WLP) of a design, given its treatment
+    WLP and blocking WLP.
+    Both WLP must start with words of length 0 (so that list indices matches
+    word lengths).
     """
     if len(blocking_wlp) != len(treatment_wlp):
         raise ValueError("Both WLP must have the same length")
     w2_vector = [treatment_wlp[3], blocking_wlp[3]]
     n_words = len(blocking_wlp) - 1
     max_i = 1 + (n_words - 1) // 2
     for i in range(2, max_i):
```

### Comparing `fatld-0.1.7/fatld/main.py` & `fatld-0.1.8/fatld/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,28 +35,29 @@
     Decompose a number into powers of 2 and returns the corresponding indices.
 
     Parameters
     ----------
     n : int
         Number to decompose
     length : int, optional
-        Wanted length for the list of indices, by default None, returns the list when
-        the last power of two `x` for which `x` < `n` is reached
+        Wanted length for the list of indices, by default None, returns the
+        list when the last power of two `x` for which `x` < `n` is reached
 
     Returns
     -------
     List[int]
         List of the indices of the powers of two obtained in the decomposition
 
     Example
     -------
     >>> # 7 can be decomposed into 1*2 + 1*2 + 1*4
     >>> power2_decomposition(7)
     [1, 1, 1]
-    >>> # 11 can be decomposed into 1*1 + 1*2 + 0*4 + 1*8, we want a list of length 7
+    >>> # 11 can be decomposed into 1*1 + 1*2 + 0*4 + 1*8, we want a list of
+    >>> # length 7
     >>> power2_decomposition(11, length=7)
     [1, 1, 0, 1, 0, 0, 0]
     """
     powers = []
     i = 1
     while i <= n:
         if i & n:
@@ -69,16 +70,16 @@
     elif length is not None and len(powers) > length:
         warnings.warn("Power list larger than supplied length", UserWarning)
     return powers
 
 
 def custom_design(runsize: int, column_list: List[int]) -> np.ndarray:
     """
-    Create a custom design with a specific run size, based on the column numbers
-    provided.
+    Create a custom design with a specific run size, based on the column
+    numbers provided.
 
     Parameters
     ----------
     runsize : int
         Number of runs
     column_list : List[int]
         Column numbers to be used for the design
@@ -97,28 +98,29 @@
     return custom_mat
 
 
 def twlp(
     ar: oa.array_link, type_0: bool = True, max_length: Optional[int] = None
 ) -> List[List[int]]:
     """
-    Compute the type-specific word length pattern of a design, starting with words
-    of length 3.
+    Compute the type-specific word length pattern of a design, starting with
+    words of length 3.
 
     Parameters
     ----------
     ar : oa.array_link
         Design matrix
     type_0 : bool, optional
         Return the word length pattern of type 0, by default True.
         If False, return the word length pattern of type `m`.
     max_length : int, optional
         Max word length to display in the word length pattern, by default None,
         all the word lengths are displayed.
-        If this number is more than the maximum word length of the design, ignores it.
+        If this number is more than the maximum word length of the design,
+        ignores it.
 
     Returns
     -------
     List[List[int]]
         Type-specific word length pattern, starting with words of length 3.
         Each sublist give the number of words of that length, sorted by type.
     """
@@ -143,40 +145,51 @@
     max_word_length = r + c - 1
     wlp_matrix = np.zeros((max_type, max_word_length), dtype=int)
     # Sum the transformed matrix over diagonal rows
     for idx in range(max_word_length):
         if idx < r and idx < c:
             comb = [(i, idx - i) for i in range(idx + 1)]
         else:
-            comb = [(i, idx - i) for i in range(idx + 1) if ((i < r) and (idx - i) < c)]
+            comb = [
+                (i, idx - i)
+                for i in range(idx + 1)
+                if ((i < r) and (idx - i) < c)
+            ]
         for coord in comb:
-            wlp_matrix[coord[0], idx] = dst_dist_transformed_mat[coord[0], coord[1]]
+            wlp_matrix[coord[0], idx] = dst_dist_transformed_mat[
+                coord[0], coord[1]
+            ]
     # Trim the matrix to max_length if needed
-    if max_length is not None and (max_length < 3 or max_length > max_word_length):
+    if max_length is not None and (
+        max_length < 3 or max_length > max_word_length
+    ):
         max_length = None
-        warnings.warn("Incorrect max_length. Full type-specific WLP is outputted")
+        warnings.warn(
+            "Incorrect max_length. Full type-specific WLP is outputted"
+        )
     if max_length is None:
         wlp_matrix_trimmed = wlp_matrix[:, 3:]
     else:
-        wlp_matrix_trimmed = wlp_matrix[:, 3 : (max_length + 1)]
+        end = max_length + 1
+        wlp_matrix_trimmed = wlp_matrix[:, 3:end]
     # Create a list of lists
     wlp_type_list = wlp_matrix_trimmed.T.tolist()
-    # Reverse the sublists if it's not type 0 because they are ordered in type 0
-    # by default
+    # Reverse the sublists if it's not type 0 because they are ordered in type
+    # 0 by default
     if type_0 is False:
         return [x[::-1] for x in wlp_type_list]
     else:
         return wlp_type_list
 
 
 def read_OA(filename: str) -> np.ndarray:
     """
-    Read a `.oa` file, generated by the `OApackage` package and return all the matrices
-    it contains as a 3-D numpy array, where the third dimension is the index of the
-    designs.
+    Read a `.oa` file, generated by the `OApackage` package and return all the
+    matrices it contains as a 3-D numpy array, where the third dimension is the
+    index of the designs.
     """
     with open(filename, "r") as f:
         info = f.readline()
         n_fac, run_size, n_des = [int(i) for i in info.strip().split(" ")]
         designs = np.zeros((run_size, n_fac, n_des), dtype=int)
         row_index = 0
         design_index = 0
```

### Comparing `fatld-0.1.7/fatld/relation.py` & `fatld-0.1.8/fatld/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 from .main import power2_decomposition
 
 
 def num2gen(n: int, m: Optional[int] = None) -> str:
     """
     Return the generator corresponding to a given column number
 
-    If a value is provided for the number of four-level factors, the pseudo-factors
-    used to generate the four-level factors will be replaced by their corresponding
-    labels in the generator.
+    If a value is provided for the number of four-level factors, the
+    pseudo-factors used to generate the four-level factors will be replaced by
+    their corresponding labels in the generator.
     The labels are:
 
     - `A1=a`, `A2=b`, `A3=ab` for the first factor
     - `B1=c`, `B2=d`, `B3=cd` for the second factor
     - `C1=e`, `C2=f`, `C3=ef` for the third factor
 
     Parameters
     ----------
     n : int
         Column number
 
     m : Optional[int]
-        Number of four-level factors. If no value is provided, the generator will be
-        considered to come from a two-level design. By default, no value is provided.
+        Number of four-level factors. If no value is provided, the generator
+        will be considered to come from a two-level design. By default, no
+        value is provided.
 
 
     Examples
     ------
     >>> num2gen(7)
     'abc'
     >>> num2gen(7, m=1)
@@ -92,25 +93,26 @@
     return sum([2 ** (i - 97) for i in ascii_code])
 
 
 def relabel_word(word: str, m: int) -> str:
     """
     Relabel basic factors in a word to their corresponding pseudo-factors.
 
-    Relabel a word containing only two-level factors by replacing the basic factors
-    used as pseudo-factors by their corresponding pseudo-factor labels.
-    The pseudo-factor labels are A_i, B_i and C_i with i = 1,2,3, for the first,
-    second, and third four-level factor, respectively.
+    Relabel a word containing only two-level factors by replacing the basic
+    factors used as pseudo-factors by their corresponding pseudo-factor labels.
+    The pseudo-factor labels are A_i, B_i and C_i with i = 1,2,3, for the
+    first, second, and third four-level factor, respectively.
 
     Parameters
     ----------
     word : str
         Word to relabel
     m : int
-        Number of four-level factors. Define up to which factor the relabeling occurs.
+        Number of four-level factors. Define up to which factor the relabeling
+        occurs.
 
     Examples
     --------
     >>> # The value of `m` define how many factors are relabeled
     >>> relabel_word(word='abcde', m=1)
     'A3cde'
     >>> relabel_word(word='abcde', m=3)
@@ -120,15 +122,16 @@
     for i in range(m):
         pf_factors = [
             chr(97 + 2 * i),
             chr(97 + 2 * i + 1),
             f"{chr(97 + 2 * i)}{chr(97 + 2 * i + 1)}",
         ]
         pf_labels = [f"{chr(65 + i)}{x}" for x in [1, 2, 3]]
-        # We start with p1p2 to avoid replacing p1/p2 first and not the interaction
+        # We start with p1p2 to avoid replacing p1/p2 first and not the
+        # interaction
         s = (
             word.replace(pf_factors[2], pf_labels[2])
             .replace(pf_factors[1], pf_labels[1])
             .replace(pf_factors[0], pf_labels[0])
         )
         word = s
     return word
@@ -161,29 +164,33 @@
     """
     return len(set(re.findall("[A-C]", word)))
 
 
 class Relation:
     # TODO: document the relation class
     def __init__(self, words: List[str], m: int = 0):
-        # `m` can only be 0, 1,2 or 3 since there can't be more four-level factors
-        # 0 means there are no four-level factors
+        # `m` can only be 0, 1,2 or 3 since there can't be more four-level
+        # factors, 0 means there are no four-level factors
         if m not in [0, 1, 2, 3]:
             raise ValueError("m can only take value of 0, 1, 2, and 3")
         # Words must be strings and only contain basic factors
-        if not isinstance(words, List) or any([not isinstance(w, str) for w in words]):
+        if not isinstance(words, List) or any(
+            [not isinstance(w, str) for w in words]
+        ):
             raise TypeError("Words must be given as a list of strings")
         if any([(ord(i) > 122 or ord(i) < 97) for w in words for i in w]):
             raise ValueError(
                 "Words can only contain lowercase letters (representing "
                 "basic factors)"
             )
         self.m = m
         self.words = words
-        self.relabel_words = [relabel_word(word=w, m=self.m) for w in self.words]
+        self.relabel_words = [
+            relabel_word(word=w, m=self.m) for w in self.words
+        ]
 
     def __repr__(self):
         return f"{self.relabel_words}"
 
     def expand(self, relabel: bool = False) -> List[str]:
         """
         Expand a defining subgroup into the complete defining relation.
@@ -208,21 +215,25 @@
         """
         full_relation = [w for w in self.words]
         for i in range(1, len(self.words)):
             word_combination = combinations(self.words, i + 1)
             for comb in word_combination:
                 word_freq = Counter("".join(comb))
                 remaining_factors = [
-                    factor for factor, freq in word_freq.items() if freq % 2 == 1
+                    factor
+                    for factor, freq in word_freq.items()
+                    if freq % 2 == 1
                 ]
                 remaining_factors.sort()
                 new_word = "".join(remaining_factors)
                 full_relation.append(new_word)
         if relabel:
-            return [relabel_word(word=word, m=self.m) for word in full_relation]
+            return [
+                relabel_word(word=word, m=self.m) for word in full_relation
+            ]
         else:
             return full_relation
 
     def word_length_pattern(self) -> List[List[int]]:
         """
         Compute the type-specific word length pattern of the defining relation.
 
@@ -240,15 +251,16 @@
         >>> # If m=0, then output a normal word length pattern
         >>> Relation(words=['abcdf', 'aceg']).word_length_pattern()
         [0, 1, 2]
         """
         full_relation = self.expand(relabel=True)
         lengths = [word_length(w) for w in full_relation]
         types = [word_type(w) for w in full_relation]
-        # Each sublist must be initiated as an individual object (can't do shallow copy)
+        # Each sublist must be initiated as an individual object (can't do
+        # shallow copy)
         wlp = [[0 for _ in range(self.m + 1)] for _ in range(max(lengths) + 1)]
         for i, x in enumerate(lengths):
             t = types[i]
             wlp[x][t] += 1
         if self.m == 0:
             return list(chain(*wlp[3:]))  # type: ignore
         return wlp[3:]
```

### Comparing `fatld-0.1.7/pyproject.toml` & `fatld-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fatld"
-version = "0.1.7"
+version = "0.1.8"
 description = "Generate and characterize designs with four-and-two-level (FATL) factors"
 authors = ["Alexandre Bohyn <alexandre.bohyn@kuleuven.be>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://abohyndoe.github.io/fatld/"
 repository = "https://github.com/ABohynDOE/fatld"
 keywords = ["design", "doe"]
```

### Comparing `fatld-0.1.7/PKG-INFO` & `fatld-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fatld
-Version: 0.1.7
+Version: 0.1.8
 Summary: Generate and characterize designs with four-and-two-level (FATL) factors
 Home-page: https://abohyndoe.github.io/fatld/
 License: MIT
 Keywords: design,doe
 Author: Alexandre Bohyn
 Author-email: alexandre.bohyn@kuleuven.be
 Requires-Python: >=3.8,<4.0
```

