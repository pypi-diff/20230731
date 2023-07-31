# Comparing `tmp/didppy-0.4.0.tar.gz` & `tmp/didppy-0.4.1.tar.gz`

## Comparing `didppy-0.4.0.tar` & `didppy-0.4.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 didppy-0.4.0/local_dependencies/dypdl/Cargo.toml
--rw-r--r--   0      501       20     5194 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/README.md
--rw-r--r--   0      501       20     9080 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/base_case.rs
--rw-r--r--   0      501       20     1344 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/effect.rs
--rw-r--r--   0      501       20    16931 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/argument_expression.rs
--rw-r--r--   0      501       20    59188 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/condition.rs
--rw-r--r--   0      501       20   290240 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_expression.rs
--rw-r--r--   0      501       20    36620 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs
--rw-r--r--   0      501       20    88634 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/element_expression.rs
--rw-r--r--   0      501       20   134795 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_expression.rs
--rw-r--r--   0      501       20    25379 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_vector_expression.rs
--rw-r--r--   0      501       20    18114 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_operator.rs
--rw-r--r--   0      501       20    62551 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_table_expression.rs
--rw-r--r--   0      501       20     4969 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/reference_expression.rs
--rw-r--r--   0      501       20    48744 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/set_condition.rs
--rw-r--r--   0      501       20   114732 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/set_expression.rs
--rw-r--r--   0      501       20   135581 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/set_reduce_expression.rs
--rw-r--r--   0      501       20    15550 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/table_expression.rs
--rw-r--r--   0      501       20    56292 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/table_vector_expression.rs
--rw-r--r--   0      501       20     1787 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/util.rs
--rw-r--r--   0      501       20    19963 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/vector_expression.rs
--rw-r--r--   0      501       20     1500 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression.rs
--rw-r--r--   0      501       20    26414 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/grounded_condition.rs
--rw-r--r--   0      501       20   671792 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/lib.rs
--rw-r--r--   0      501       20   131319 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/state.rs
--rw-r--r--   0      501       20    18956 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/table.rs
--rw-r--r--   0      501       20    46003 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/table_data.rs
--rw-r--r--   0      501       20    84395 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/table_registry.rs
--rw-r--r--   0      501       20    57672 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/transition.rs
--rw-r--r--   0      501       20      438 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/util.rs
--rw-r--r--   0      501       20     3476 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/variable_type.rs
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/Cargo.toml
--rw-r--r--   0      501       20     1631 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/README.md
--rw-r--r--   0      501       20     4995 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/caasdy.rs
--rw-r--r--   0      501       20     5025 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs
--rw-r--r--   0      501       20     4970 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs
--rw-r--r--   0      501       20     4699 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_breadth_first_search.rs
--rw-r--r--   0      501       20     5107 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs
--rw-r--r--   0      501       20     4706 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs
--rw-r--r--   0      501       20     4778 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs
--rw-r--r--   0      501       20     4472 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs
--rw-r--r--   0      501       20     4807 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs
--rw-r--r--   0      501       20     7488 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs
--rw-r--r--   0      501       20     1717 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs
--rw-r--r--   0      501       20     1230 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/lib.rs
--rw-r--r--   0      501       20    13643 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs
--rw-r--r--   0      501       20    13189 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs
--rw-r--r--   0      501       20    10454 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs
--rw-r--r--   0      501       20     9953 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs
--rw-r--r--   0      501       20    11475 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs
--rw-r--r--   0      501       20    10748 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs
--rw-r--r--   0      501       20    10449 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs
--rw-r--r--   0      501       20    15763 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs
--rw-r--r--   0      501       20    47180 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs
--rw-r--r--   0      501       20      835 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/bfs_node.rs
--rw-r--r--   0      501       20    28848 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/cost_node.rs
--rw-r--r--   0      501       20    34204 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/custom_f_node.rs
--rw-r--r--   0      501       20    48547 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/f_node.rs
--rw-r--r--   0      501       20    52543 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/weighted_f_node.rs
--rw-r--r--   0      501       20      237 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node.rs
--rw-r--r--   0      501       20    63006 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/state_registry.rs
--rw-r--r--   0      501       20    20278 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs
--rw-r--r--   0      501       20    12373 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_custom_cost.rs
--rw-r--r--   0      501       20    10595 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_id.rs
--rw-r--r--   0      501       20      167 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition.rs
--rw-r--r--   0      501       20     3808 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs
--rw-r--r--   0      501       20     1971 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs
--rw-r--r--   0      501       20      713 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs
--rw-r--r--   0      501       20    11942 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs
--rw-r--r--   0      501       20     9330 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs
--rw-r--r--   0      501       20     7031 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs
--rw-r--r--   0      501       20    27771 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs
--rw-r--r--   0      501       20     4791 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs
--rw-r--r--   0      501       20    11386 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/util.rs
--rw-r--r--   0      501       20      988 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm.rs
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 didppy-0.4.0/Cargo.toml
--rw-r--r--   0      501       20      705 2023-05-25 22:02:32.000000 didppy-0.4.0/.gitignore
--rw-r--r--   0      501       20     1872 2023-05-25 22:02:32.000000 didppy-0.4.0/README.md
--rw-r--r--   0      501       20       71 2023-05-25 22:02:32.000000 didppy-0.4.0/build.rs
--rw-r--r--   0      501       20      634 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/Makefile
--rw-r--r--   0      501       20    29958 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/_static/images/TSPTW.png
--rw-r--r--   0      501       20      645 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0      501       20     8470 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/advanced-tutorials/forced-transitions.rst
--rw-r--r--   0      501       20     6060 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/advanced-tutorials/general-cost.rst
--rw-r--r--   0      501       20      250 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/advanced-tutorials.rst
--rw-r--r--   0      501       20     1912 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/api-reference.rst
--rw-r--r--   0      501       20     2246 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/conf.py
--rw-r--r--   0      501       20     4189 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging/common-mistakes.rst
--rw-r--r--   0      501       20     5939 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging/state.rst
--rw-r--r--   0      501       20     2881 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging/validate.rst
--rw-r--r--   0      501       20      255 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging.rst
--rw-r--r--   0      501       20     2237 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/examples.rst
--rw-r--r--   0      501       20     1086 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/index.rst
--rw-r--r--   0      501       20      800 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/make.bat
--rw-r--r--   0      501       20     1494 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/papers.rst
--rw-r--r--   0      501       20     4205 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/quickstart.rst
--rw-r--r--   0      501       20     7668 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/ref.bib
--rw-r--r--   0      501       20       67 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/references.rst
--rw-r--r--   0      501       20       45 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/requirements.txt
--rw-r--r--   0      501       20     4797 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/solver-selection.rst
--rw-r--r--   0      501       20    28927 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/tutorial.rst
--rw-r--r--   0      501       20     2617 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/README.md
--rw-r--r--   0      501       20    10351 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/bin-packing.ipynb
--rw-r--r--   0      501       20     9197 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/cvrp.ipynb
--rw-r--r--   0      501       20     5970 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/graph-clear.ipynb
--rw-r--r--   0      501       20     4927 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/knapsack.ipynb
--rw-r--r--   0      501       20     9316 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/m-pdtsp.ipynb
--rw-r--r--   0      501       20     6931 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/mosp.ipynb
--rw-r--r--   0      501       20     9948 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/salbp-1.ipynb
--rw-r--r--   0      501       20     5314 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/single-machine.ipynb
--rw-r--r--   0      501       20     7687 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/talent-scheduling.ipynb
--rw-r--r--   0      501       20     8114 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/tsptw.ipynb
--rw-r--r--   0      501       20      582 2023-05-25 22:02:32.000000 didppy-0.4.0/pyproject.toml
--rw-r--r--   0      501       20     9328 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/acps.rs
--rw-r--r--   0      501       20     9251 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/apps.rs
--rw-r--r--   0      501       20     8726 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/breadth_first_search.rs
--rw-r--r--   0      501       20     8606 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/caasdy.rs
--rw-r--r--   0      501       20     9260 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/cabs.rs
--rw-r--r--   0      501       20     8297 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/cbfs.rs
--rw-r--r--   0      501       20     8792 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/dbdfs.rs
--rw-r--r--   0      501       20     8235 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/dfbb.rs
--rw-r--r--   0      501       20    13995 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/expression_beam_search.rs
--rw-r--r--   0      501       20     1755 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/f_operator.rs
--rw-r--r--   0      501       20     3804 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/forward_recursion.rs
--rw-r--r--   0      501       20     8314 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/weighted_astar.rs
--rw-r--r--   0      501       20     6297 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/wrapped_solver.rs
--rw-r--r--   0      501       20      684 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver.rs
--rw-r--r--   0      501       20     2914 2023-05-25 22:02:32.000000 didppy-0.4.0/src/lib.rs
--rw-r--r--   0      501       20   377271 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/expression.rs
--rw-r--r--   0      501       20     4897 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/state.rs
--rw-r--r--   0      501       20   172084 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/table.rs
--rw-r--r--   0      501       20    44011 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/transition.rs
--rw-r--r--   0      501       20   546337 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model.rs
--rw-r--r--   0      501       20     2741 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_acps.py
--rw-r--r--   0      501       20     2741 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_apps.py
--rw-r--r--   0      501       20     2687 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_bradth_first_search.py
--rw-r--r--   0      501       20     2627 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_caasdy.py
--rw-r--r--   0      501       20     2561 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_cabs.py
--rw-r--r--   0      501       20     2617 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_cbfs.py
--rw-r--r--   0      501       20     2658 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_dbdfs.py
--rw-r--r--   0      501       20     2617 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_dfbb.py
--rw-r--r--   0      501       20     1613 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_expression_beam_search.py
--rw-r--r--   0      501       20     1589 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_forward_recursion.py
--rw-r--r--   0      501       20     2727 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_weighted_astar.py
--rw-r--r--   0      501       20    85219 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_expression.py
--rw-r--r--   0      501       20     6576 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_state.py
--rw-r--r--   0      501       20    66254 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_table.py
--rw-r--r--   0      501       20    16456 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_transition.py
--rw-r--r--   0      501       20    56856 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/test_model.py
--rw-r--r--   0      501       20    12339 2023-05-25 22:02:32.000000 didppy-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 didppy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 didppy-0.4.1/local_dependencies/dypdl/Cargo.toml
+-rw-r--r--   0      501       20     5194 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/README.md
+-rw-r--r--   0      501       20     9080 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/base_case.rs
+-rw-r--r--   0      501       20     1344 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/effect.rs
+-rw-r--r--   0      501       20    16931 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/argument_expression.rs
+-rw-r--r--   0      501       20    59188 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/condition.rs
+-rw-r--r--   0      501       20   290240 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/continuous_expression.rs
+-rw-r--r--   0      501       20    36620 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs
+-rw-r--r--   0      501       20    88634 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/element_expression.rs
+-rw-r--r--   0      501       20   134795 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/integer_expression.rs
+-rw-r--r--   0      501       20    25379 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/integer_vector_expression.rs
+-rw-r--r--   0      501       20    18114 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/numeric_operator.rs
+-rw-r--r--   0      501       20    62551 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/numeric_table_expression.rs
+-rw-r--r--   0      501       20     4969 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/reference_expression.rs
+-rw-r--r--   0      501       20    48744 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/set_condition.rs
+-rw-r--r--   0      501       20   114732 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/set_expression.rs
+-rw-r--r--   0      501       20   135581 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/set_reduce_expression.rs
+-rw-r--r--   0      501       20    15550 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/table_expression.rs
+-rw-r--r--   0      501       20    56292 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/table_vector_expression.rs
+-rw-r--r--   0      501       20     1787 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/util.rs
+-rw-r--r--   0      501       20    19963 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression/vector_expression.rs
+-rw-r--r--   0      501       20     1500 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/expression.rs
+-rw-r--r--   0      501       20    26414 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/grounded_condition.rs
+-rw-r--r--   0      501       20   710959 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/lib.rs
+-rw-r--r--   0      501       20   131319 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/state.rs
+-rw-r--r--   0      501       20    18956 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/table.rs
+-rw-r--r--   0      501       20    46003 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/table_data.rs
+-rw-r--r--   0      501       20    84395 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/table_registry.rs
+-rw-r--r--   0      501       20    57672 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/transition.rs
+-rw-r--r--   0      501       20      438 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/util.rs
+-rw-r--r--   0      501       20     3476 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl/src/variable_type.rs
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/Cargo.toml
+-rw-r--r--   0      501       20     1631 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/README.md
+-rw-r--r--   0      501       20     4995 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/caasdy.rs
+-rw-r--r--   0      501       20     5025 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs
+-rw-r--r--   0      501       20     4970 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs
+-rw-r--r--   0      501       20     4699 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_breadth_first_search.rs
+-rw-r--r--   0      501       20     5107 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs
+-rw-r--r--   0      501       20     4706 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs
+-rw-r--r--   0      501       20     4778 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs
+-rw-r--r--   0      501       20     4472 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs
+-rw-r--r--   0      501       20     4807 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs
+-rw-r--r--   0      501       20     7488 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs
+-rw-r--r--   0      501       20     1717 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs
+-rw-r--r--   0      501       20     1230 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/lib.rs
+-rw-r--r--   0      501       20    13643 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs
+-rw-r--r--   0      501       20    13189 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs
+-rw-r--r--   0      501       20    10454 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs
+-rw-r--r--   0      501       20     9953 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs
+-rw-r--r--   0      501       20    11475 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs
+-rw-r--r--   0      501       20    10748 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs
+-rw-r--r--   0      501       20    10449 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs
+-rw-r--r--   0      501       20    15763 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs
+-rw-r--r--   0      501       20    47180 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs
+-rw-r--r--   0      501       20      835 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/bfs_node.rs
+-rw-r--r--   0      501       20    28848 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/cost_node.rs
+-rw-r--r--   0      501       20    34204 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/custom_f_node.rs
+-rw-r--r--   0      501       20    48547 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/f_node.rs
+-rw-r--r--   0      501       20    52543 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/weighted_f_node.rs
+-rw-r--r--   0      501       20      237 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node.rs
+-rw-r--r--   0      501       20    63006 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/state_registry.rs
+-rw-r--r--   0      501       20    20278 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs
+-rw-r--r--   0      501       20    12373 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_custom_cost.rs
+-rw-r--r--   0      501       20    10595 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_id.rs
+-rw-r--r--   0      501       20      167 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition.rs
+-rw-r--r--   0      501       20     3808 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs
+-rw-r--r--   0      501       20     1971 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs
+-rw-r--r--   0      501       20      713 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs
+-rw-r--r--   0      501       20    11942 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs
+-rw-r--r--   0      501       20     9330 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs
+-rw-r--r--   0      501       20     7031 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs
+-rw-r--r--   0      501       20    27771 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs
+-rw-r--r--   0      501       20     4791 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs
+-rw-r--r--   0      501       20    11386 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/util.rs
+-rw-r--r--   0      501       20      988 2023-07-31 20:32:24.000000 didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm.rs
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 didppy-0.4.1/Cargo.toml
+-rw-r--r--   0      501       20      705 2023-07-31 20:32:23.000000 didppy-0.4.1/.gitignore
+-rw-r--r--   0      501       20     1872 2023-07-31 20:32:23.000000 didppy-0.4.1/README.md
+-rw-r--r--   0      501       20       71 2023-07-31 20:32:23.000000 didppy-0.4.1/build.rs
+-rw-r--r--   0      501       20      634 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/Makefile
+-rw-r--r--   0      501       20    29958 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/_static/images/TSPTW.png
+-rw-r--r--   0      501       20      645 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0      501       20     8470 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/advanced-tutorials/forced-transitions.rst
+-rw-r--r--   0      501       20     6060 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/advanced-tutorials/general-cost.rst
+-rw-r--r--   0      501       20      250 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/advanced-tutorials.rst
+-rw-r--r--   0      501       20     1912 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/api-reference.rst
+-rw-r--r--   0      501       20     2246 2023-07-31 20:32:23.000000 didppy-0.4.1/docs/conf.py
+-rw-r--r--   0      501       20     4189 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/debugging/common-mistakes.rst
+-rw-r--r--   0      501       20     5939 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/debugging/state.rst
+-rw-r--r--   0      501       20     2881 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/debugging/validate.rst
+-rw-r--r--   0      501       20      255 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/debugging.rst
+-rw-r--r--   0      501       20     2237 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/examples.rst
+-rw-r--r--   0      501       20     1086 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/make.bat
+-rw-r--r--   0      501       20     1494 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/papers.rst
+-rw-r--r--   0      501       20     4205 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/quickstart.rst
+-rw-r--r--   0      501       20     7668 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/ref.bib
+-rw-r--r--   0      501       20       67 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/references.rst
+-rw-r--r--   0      501       20       45 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/requirements.txt
+-rw-r--r--   0      501       20     4797 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/solver-selection.rst
+-rw-r--r--   0      501       20    28927 2023-07-31 20:32:24.000000 didppy-0.4.1/docs/tutorial.rst
+-rw-r--r--   0      501       20     2617 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/README.md
+-rw-r--r--   0      501       20    10351 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/bin-packing.ipynb
+-rw-r--r--   0      501       20     9197 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/cvrp.ipynb
+-rw-r--r--   0      501       20     5970 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/graph-clear.ipynb
+-rw-r--r--   0      501       20     4927 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/knapsack.ipynb
+-rw-r--r--   0      501       20     9316 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/m-pdtsp.ipynb
+-rw-r--r--   0      501       20     6931 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/mosp.ipynb
+-rw-r--r--   0      501       20     9948 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/salbp-1.ipynb
+-rw-r--r--   0      501       20     5314 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/single-machine.ipynb
+-rw-r--r--   0      501       20     7687 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/talent-scheduling.ipynb
+-rw-r--r--   0      501       20     8114 2023-07-31 20:32:24.000000 didppy-0.4.1/examples/tsptw.ipynb
+-rw-r--r--   0      501       20      582 2023-07-31 20:32:24.000000 didppy-0.4.1/pyproject.toml
+-rw-r--r--   0      501       20     9328 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/acps.rs
+-rw-r--r--   0      501       20     9251 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/apps.rs
+-rw-r--r--   0      501       20     8726 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/breadth_first_search.rs
+-rw-r--r--   0      501       20     8606 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/caasdy.rs
+-rw-r--r--   0      501       20     9260 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/cabs.rs
+-rw-r--r--   0      501       20     8297 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/cbfs.rs
+-rw-r--r--   0      501       20     8792 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/dbdfs.rs
+-rw-r--r--   0      501       20     8235 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/dfbb.rs
+-rw-r--r--   0      501       20    13995 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/expression_beam_search.rs
+-rw-r--r--   0      501       20     1755 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/f_operator.rs
+-rw-r--r--   0      501       20     3804 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/forward_recursion.rs
+-rw-r--r--   0      501       20     8314 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/weighted_astar.rs
+-rw-r--r--   0      501       20     6297 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver/wrapped_solver.rs
+-rw-r--r--   0      501       20      684 2023-07-31 20:32:24.000000 didppy-0.4.1/src/heuristic_search_solver.rs
+-rw-r--r--   0      501       20     2914 2023-07-31 20:32:24.000000 didppy-0.4.1/src/lib.rs
+-rw-r--r--   0      501       20   377271 2023-07-31 20:32:24.000000 didppy-0.4.1/src/model/expression.rs
+-rw-r--r--   0      501       20     4897 2023-07-31 20:32:24.000000 didppy-0.4.1/src/model/state.rs
+-rw-r--r--   0      501       20   172084 2023-07-31 20:32:24.000000 didppy-0.4.1/src/model/table.rs
+-rw-r--r--   0      501       20    44011 2023-07-31 20:32:24.000000 didppy-0.4.1/src/model/transition.rs
+-rw-r--r--   0      501       20   546337 2023-07-31 20:32:24.000000 didppy-0.4.1/src/model.rs
+-rw-r--r--   0      501       20     2741 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_acps.py
+-rw-r--r--   0      501       20     2741 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_apps.py
+-rw-r--r--   0      501       20     2687 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_bradth_first_search.py
+-rw-r--r--   0      501       20     2627 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_caasdy.py
+-rw-r--r--   0      501       20     2561 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_cabs.py
+-rw-r--r--   0      501       20     2617 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_cbfs.py
+-rw-r--r--   0      501       20     2658 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_dbdfs.py
+-rw-r--r--   0      501       20     2617 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_dfbb.py
+-rw-r--r--   0      501       20     1613 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_expression_beam_search.py
+-rw-r--r--   0      501       20     1589 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_forward_recursion.py
+-rw-r--r--   0      501       20     2727 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/heuristic_search_solver/test_weighted_astar.py
+-rw-r--r--   0      501       20    85219 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/model/test_expression.py
+-rw-r--r--   0      501       20     6576 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/model/test_state.py
+-rw-r--r--   0      501       20    66254 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/model/test_table.py
+-rw-r--r--   0      501       20    16456 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/model/test_transition.py
+-rw-r--r--   0      501       20    56856 2023-07-31 20:32:24.000000 didppy-0.4.1/tests/test_model.py
+-rw-r--r--   0      501       20    12339 2023-07-31 20:32:23.000000 didppy-0.4.1/Cargo.lock
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 didppy-0.4.1/PKG-INFO
```

### Comparing `didppy-0.4.0/local_dependencies/dypdl/Cargo.toml` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [package]
-name = "dypdl"
-version = "0.4.0"
+name = "dypdl-heuristic-search"
+version = "0.4.1"
 edition = "2021"
 rust-version = "1.64"
-description = "Libarary for Dynamic Programming Description Language (DyPDL)."
+description = "Heuristic search solvers for Dynamic Programming Description Language (DyPDL)."
 license = "MIT OR Apache-2.0"
 authors = ["Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>"]
 homepage = "https://didp.ai"
 repository = "https://github.com/domain-independent-dp/didp-rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 ordered-float = "3.0"
-fixedbitset = "0.4"
-approx = "0.5"
-num-traits = "0.2"
-rustc-hash = "1.1"
+dypdl = { path = "../dypdl", version = "0.4.0" }
+rustc-hash = "1.1"
```

### Comparing `didppy-0.4.0/local_dependencies/dypdl/README.md` & `didppy-0.4.1/local_dependencies/dypdl/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/base_case.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/base_case.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/effect.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/effect.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/argument_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/argument_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/condition.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/condition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/continuous_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/element_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/element_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/integer_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_vector_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/integer_vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_operator.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/numeric_operator.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_table_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/numeric_table_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/reference_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/reference_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/set_condition.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/set_condition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/set_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/set_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/set_reduce_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/set_reduce_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/table_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/table_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/table_vector_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/table_vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/util.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/util.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression/vector_expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression/vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/expression.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/grounded_condition.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/grounded_condition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/lib.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2387,15 +2387,15 @@
                     }
                     expression::NumericTableExpression::Table2D(id, x, y) => {
                         self.table_registry.$x.check_table_2d(*id)?;
                         self.check_expression(x, allow_cost)?;
                         self.check_expression(y, allow_cost)
                     }
                     expression::NumericTableExpression::Table3D(id, x, y, z) => {
-                        self.table_registry.$x.check_table_2d(*id)?;
+                        self.table_registry.$x.check_table_3d(*id)?;
                         self.check_expression(x, allow_cost)?;
                         self.check_expression(y, allow_cost)?;
                         self.check_expression(z, allow_cost)
                     }
                     expression::NumericTableExpression::Table1DReduce(_, id, x) => {
                         self.table_registry.$x.check_table_1d(*id)?;
                         self.check_expression(x, allow_cost)
@@ -2441,15 +2441,15 @@
                     }
                     expression::NumericTableExpression::Table2DVectorReduceY(_, id, x, y) => {
                         self.table_registry.$x.check_table_2d(*id)?;
                         self.check_expression(x, allow_cost)?;
                         self.check_expression(y, allow_cost)
                     }
                     expression::NumericTableExpression::Table3DReduce(_, id, x, y, z) => {
-                        self.table_registry.$x.check_table_2d(*id)?;
+                        self.table_registry.$x.check_table_3d(*id)?;
                         self.check_expression(x, allow_cost)?;
                         self.check_expression(y, allow_cost)?;
                         self.check_expression(z, allow_cost)
                     }
                 }
             }
         }
@@ -7200,14 +7200,131 @@
                     ..Default::default()
                 }
             ]
         );
     }
 
     #[test]
+    fn add_forward_transition_with_table1d_ok() {
+        // Test success when the model that has only one Int table 1D,
+        // and using the constants inside in a forward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.forward_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(0)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_forward_transition_with_table2d_ok() {
+        // Test success when the model that has only one Int table 2D,
+        // and using the constants inside in a forward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index [0,1] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.forward_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_forward_transition_with_table3d_ok() {
+        // Test success when the model that has only one Int table 3D,
+        // and using the constants inside in a forward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index [0,0,1] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.forward_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
     fn add_forward_transition_err() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let transition = Transition {
             cost: CostExpression::Continuous(ContinuousExpression::Cost),
@@ -7716,14 +7833,155 @@
             },
             ..Default::default()
         };
         assert!(model.add_forward_transition(transition).is_err());
     }
 
     #[test]
+    fn add_forward_transition_with_table1d_err() {
+        // Test failure when the model that has only one Int table 1D, but try to use the constants
+        // inside a Int table 2D or 3D in a forward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_forward_transition_with_table2d_err() {
+        // Test failure when the model that has only one Int table 2D, but try to use the constants
+        // inside a Int table 1D or 3D in a forward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_forward_transition_with_table3d_err() {
+        // Test failure when the model that has only one Int table 3D, but try to use the constants
+        // inside a Int table 1D or 2D in a forward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
     fn add_forward_forced_transition_ok() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let ob = model.add_object_type("something", 10);
         assert!(ob.is_ok());
@@ -8265,14 +8523,131 @@
                     ..Default::default()
                 }
             ]
         );
     }
 
     #[test]
+    fn add_forward_forced_transition_with_table1d_ok() {
+        // Test success when the model that has only one Int table 1D,
+        // and using the constants inside in a forward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.forward_forced_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(0)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_forward_forced_transition_with_table2d_ok() {
+        // Test success when the model that has only one Int table 2D,
+        // and using the constants inside in a forward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index [0,1] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.forward_forced_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_forward_forced_transition_with_table3d_ok() {
+        // Test success when the model that has only one Int table 3D,
+        // and using the constants inside in a forward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index [0,0,1] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.forward_forced_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
     fn add_forward_forced_transition_err() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let transition = Transition {
             cost: CostExpression::Continuous(ContinuousExpression::Cost),
@@ -8781,14 +9156,155 @@
             },
             ..Default::default()
         };
         assert!(model.add_forward_forced_transition(transition).is_err());
     }
 
     #[test]
+    fn add_forward_forced_transition_with_table1d_err() {
+        // Test failure when the model that has only one Int table 1D, but try to use the constants
+        // inside a Int table 2D or 3D in a forward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_forward_forced_transition_with_table2d_err() {
+        // Test failure when the model that has only one Int table 2D, but try to use the constants
+        // inside a Int table 1D or 3D in a forward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_forward_forced_transition_with_table3d_err() {
+        // Test failure when the model that has only one Int table 3D, but try to use the constants
+        // inside a Int table 1D or 2D in a forward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_forward_forced_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
     fn add_backward_transition_ok() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let ob = model.add_object_type("something", 10);
         assert!(ob.is_ok());
@@ -9330,14 +9846,131 @@
                     ..Default::default()
                 }
             ]
         );
     }
 
     #[test]
+    fn add_backward_transition_with_table1d_ok() {
+        // Test success when the model that has only one Int table 1D,
+        // and using the constants inside in a backward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.backward_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(0)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_backward_transition_with_table2d_ok() {
+        // Test success when the model that has only one Int table 2D,
+        // and using the constants inside in a backward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index [0,1] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.backward_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_backward_transition_with_table3d_ok() {
+        // Test success when the model that has only one Int table 3D,
+        // and using the constants inside in a backward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index [0,0,1] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.backward_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
     fn add_backward_transition_err() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let transition = Transition {
             cost: CostExpression::Continuous(ContinuousExpression::Cost),
@@ -9846,14 +10479,155 @@
             },
             ..Default::default()
         };
         assert!(model.add_backward_transition(transition).is_err());
     }
 
     #[test]
+    fn add_backward_transition_with_table1d_err() {
+        // Test failure when the model that has only one Int table 1D, but try to use the constants
+        // inside a Int table 2D or 3D in a backward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_backward_transition_with_table2d_err() {
+        // Test failure when the model that has only one Int table 2D, but try to use the constants
+        // inside a Int table 1D or 3D in a backward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_backward_transition_with_table3d_err() {
+        // Test failure when the model that has only one Int table 3D, but try to use the constants
+        // inside a Int table 1D or 2D in a backward transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_err());
+
+        //Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
     fn add_backward_forced_transition_ok() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let ob = model.add_object_type("something", 10);
         assert!(ob.is_ok());
@@ -10395,14 +11169,131 @@
                     ..Default::default()
                 }
             ]
         );
     }
 
     #[test]
+    fn add_backward_forced_transition_with_table1d_ok() {
+        // Test success when the model that has only one Int table 1D,
+        // and using the constants inside in a backward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.backward_forced_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(0)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_backward_forced_transition_with_table2d_ok() {
+        // Test success when the model that has only one Int table 2D,
+        // and using the constants inside in a backward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index [0,1] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.backward_forced_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
+    fn add_backward_forced_transition_with_table3d_ok() {
+        // Test success when the model that has only one Int table 3D,
+        // and using the constants inside in a backward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index [0,0,1] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(1),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.backward_forced_transitions,
+            vec![Transition {
+                cost: CostExpression::Integer(
+                    IntegerExpression::Cost + IntegerExpression::Constant(1)
+                ),
+                ..Default::default()
+            }]
+        );
+    }
+
+    #[test]
     fn add_backward_forced_transition_err() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         let transition = Transition {
             cost: CostExpression::Continuous(ContinuousExpression::Cost),
@@ -10911,14 +11802,155 @@
             },
             ..Default::default()
         };
         assert!(model.add_backward_forced_transition(transition).is_err());
     }
 
     #[test]
+    fn add_backward_forced_transition_with_table1d_err() {
+        // Test failure when the model that has only one Int table 1D, but try to use the constants
+        // inside a Int table 2D or 3D in a backward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table1d = model.add_table_1d("t1", vec![0, 1]);
+        assert!(table1d.is_ok());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_backward_forced_transition_with_table2d_err() {
+        // Test failure when the model that has only one Int table 2D, but try to use the constants
+        // inside a Int table 1D or 3D in a backward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table2d = model.add_table_2d("t1", vec![vec![0, 1]]);
+        assert!(table2d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0,0] in the first 3D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table3D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_backward_forced_transition_with_table3d_err() {
+        // Test failure when the model that has only one Int table 3D, but try to use the constants
+        // inside a Int table 1D or 2D in a backward forced transition.
+        let mut model = Model {
+            cost_type: CostType::Integer,
+            ..Default::default()
+        };
+
+        let table3d = model.add_table_3d("t1", vec![vec![vec![0, 1]]]);
+        assert!(table3d.is_ok());
+
+        // Try to access the element at index 0 in the first 1D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table1D(
+                            0,
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_err());
+
+        // Try to access the element at index [0,0] in the first 2D Integer Table
+        let transition = Transition {
+            cost: CostExpression::Integer(
+                IntegerExpression::Cost
+                    + IntegerExpression::Table(Box::new(
+                        NumericTableExpression::<Integer>::Table2D(
+                            0,
+                            ElementExpression::Constant(0),
+                            ElementExpression::Constant(0),
+                        ),
+                    )),
+            ),
+            ..Default::default()
+        };
+        let result = model.add_backward_forced_transition(transition);
+        assert!(result.is_err());
+    }
+
+    #[test]
     fn add_dual_bound_ok() {
         let mut model = Model {
             cost_type: CostType::Integer,
             ..Default::default()
         };
         assert!(model
             .add_dual_bound(IntegerExpression::UnaryOperation(
```

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/state.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/state.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/table.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/table.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/table_data.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/table_data.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/table_registry.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/table_registry.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/transition.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/transition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl/src/variable_type.rs` & `didppy-0.4.1/local_dependencies/dypdl/src/variable_type.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/Cargo.toml` & `didppy-0.4.1/local_dependencies/dypdl/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [package]
-name = "dypdl-heuristic-search"
-version = "0.4.0"
+name = "dypdl"
+version = "0.4.1"
 edition = "2021"
 rust-version = "1.64"
-description = "Heuristic search solvers for Dynamic Programming Description Language (DyPDL)."
+description = "Libarary for Dynamic Programming Description Language (DyPDL)."
 license = "MIT OR Apache-2.0"
 authors = ["Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>"]
 homepage = "https://didp.ai"
 repository = "https://github.com/domain-independent-dp/didp-rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 ordered-float = "3.0"
-dypdl = { path = "../dypdl", version = "0.4.0" }
-rustc-hash = "1.1"
+fixedbitset = "0.4"
+approx = "0.5"
+num-traits = "0.2"
+rustc-hash = "1.1"
```

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/README.md` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/caasdy.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/caasdy.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_breadth_first_search.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_breadth_first_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/lib.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/lib.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/bfs_node.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/bfs_node.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/cost_node.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/cost_node.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/custom_f_node.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/custom_f_node.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/f_node.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/f_node.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/weighted_f_node.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/weighted_f_node.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/state_registry.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/state_registry.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_custom_cost.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_custom_cost.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_id.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_id.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/util.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm/util.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm.rs` & `didppy-0.4.1/local_dependencies/dypdl-heuristic-search/src/search_algorithm.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/Cargo.toml` & `didppy-0.4.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "didppy"
-version = "0.4.0"
+version = "0.4.1"
 edition = "2021"
 rust-version = "1.64"
 description = "Python interface for Dynamic Programming Description Language (DyPDL) and DyPDL solvers."
 license = "MIT OR Apache-2.0"
 authors = ["Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>"]
 homepage = "https://didp.ai"
 repository = "https://github.com/domain-independent-dp/didp-rs"
```

### Comparing `didppy-0.4.0/.gitignore` & `didppy-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/README.md` & `didppy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/Makefile` & `didppy-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/_static/images/TSPTW.png` & `didppy-0.4.1/docs/_static/images/TSPTW.png`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/_templates/autosummary/class.rst` & `didppy-0.4.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/advanced-tutorials/forced-transitions.rst` & `didppy-0.4.1/docs/advanced-tutorials/forced-transitions.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/advanced-tutorials/general-cost.rst` & `didppy-0.4.1/docs/advanced-tutorials/general-cost.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/api-reference.rst` & `didppy-0.4.1/docs/api-reference.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/conf.py` & `didppy-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/debugging/common-mistakes.rst` & `didppy-0.4.1/docs/debugging/common-mistakes.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/debugging/state.rst` & `didppy-0.4.1/docs/debugging/state.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/debugging/validate.rst` & `didppy-0.4.1/docs/debugging/validate.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/examples.rst` & `didppy-0.4.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/index.rst` & `didppy-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/make.bat` & `didppy-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/papers.rst` & `didppy-0.4.1/docs/papers.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/quickstart.rst` & `didppy-0.4.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/ref.bib` & `didppy-0.4.1/docs/ref.bib`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/solver-selection.rst` & `didppy-0.4.1/docs/solver-selection.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/docs/tutorial.rst` & `didppy-0.4.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/README.md` & `didppy-0.4.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/bin-packing.ipynb` & `didppy-0.4.1/examples/bin-packing.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/cvrp.ipynb` & `didppy-0.4.1/examples/cvrp.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/graph-clear.ipynb` & `didppy-0.4.1/examples/graph-clear.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/knapsack.ipynb` & `didppy-0.4.1/examples/knapsack.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/m-pdtsp.ipynb` & `didppy-0.4.1/examples/m-pdtsp.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/mosp.ipynb` & `didppy-0.4.1/examples/mosp.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/salbp-1.ipynb` & `didppy-0.4.1/examples/salbp-1.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/single-machine.ipynb` & `didppy-0.4.1/examples/single-machine.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/talent-scheduling.ipynb` & `didppy-0.4.1/examples/talent-scheduling.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/examples/tsptw.ipynb` & `didppy-0.4.1/examples/tsptw.ipynb`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/pyproject.toml` & `didppy-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/acps.rs` & `didppy-0.4.1/src/heuristic_search_solver/acps.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/apps.rs` & `didppy-0.4.1/src/heuristic_search_solver/apps.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/breadth_first_search.rs` & `didppy-0.4.1/src/heuristic_search_solver/breadth_first_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/caasdy.rs` & `didppy-0.4.1/src/heuristic_search_solver/caasdy.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/cabs.rs` & `didppy-0.4.1/src/heuristic_search_solver/cabs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/cbfs.rs` & `didppy-0.4.1/src/heuristic_search_solver/cbfs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/dbdfs.rs` & `didppy-0.4.1/src/heuristic_search_solver/dbdfs.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/dfbb.rs` & `didppy-0.4.1/src/heuristic_search_solver/dfbb.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/expression_beam_search.rs` & `didppy-0.4.1/src/heuristic_search_solver/expression_beam_search.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/f_operator.rs` & `didppy-0.4.1/src/heuristic_search_solver/f_operator.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/forward_recursion.rs` & `didppy-0.4.1/src/heuristic_search_solver/forward_recursion.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/weighted_astar.rs` & `didppy-0.4.1/src/heuristic_search_solver/weighted_astar.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver/wrapped_solver.rs` & `didppy-0.4.1/src/heuristic_search_solver/wrapped_solver.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/heuristic_search_solver.rs` & `didppy-0.4.1/src/heuristic_search_solver.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/lib.rs` & `didppy-0.4.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/model/expression.rs` & `didppy-0.4.1/src/model/expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/model/state.rs` & `didppy-0.4.1/src/model/state.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/model/table.rs` & `didppy-0.4.1/src/model/table.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/model/transition.rs` & `didppy-0.4.1/src/model/transition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/src/model.rs` & `didppy-0.4.1/src/model.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_acps.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_acps.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_apps.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_apps.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_bradth_first_search.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_bradth_first_search.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_caasdy.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_caasdy.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_cabs.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_cabs.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_cbfs.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_cbfs.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_dbdfs.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_dbdfs.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_dfbb.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_dfbb.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_expression_beam_search.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_expression_beam_search.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_forward_recursion.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_forward_recursion.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/heuristic_search_solver/test_weighted_astar.py` & `didppy-0.4.1/tests/heuristic_search_solver/test_weighted_astar.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/model/test_expression.py` & `didppy-0.4.1/tests/model/test_expression.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/model/test_state.py` & `didppy-0.4.1/tests/model/test_state.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/model/test_table.py` & `didppy-0.4.1/tests/model/test_table.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/model/test_transition.py` & `didppy-0.4.1/tests/model/test_transition.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/tests/test_model.py` & `didppy-0.4.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `didppy-0.4.0/Cargo.lock` & `didppy-0.4.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "didp-yaml"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "approx",
  "dypdl",
  "dypdl-heuristic-search",
  "lazy_static",
  "linked-hash-map",
  "num-traits",
@@ -50,37 +50,37 @@
  "serde_yaml",
  "tikv-jemallocator",
  "yaml-rust",
 ]
 
 [[package]]
 name = "didppy"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "dypdl",
  "dypdl-heuristic-search",
  "pyo3",
  "pyo3-build-config",
  "rustc-hash",
 ]
 
 [[package]]
 name = "dypdl"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "approx",
  "fixedbitset",
  "num-traits",
  "ordered-float",
  "rustc-hash",
 ]
 
 [[package]]
 name = "dypdl-heuristic-search"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "dypdl",
  "ordered-float",
  "rustc-hash",
 ]
 
 [[package]]
```

### Comparing `didppy-0.4.0/PKG-INFO` & `didppy-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didppy
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python interface for Dynamic Programming Description Language (DyPDL) and DyPDL solvers.
 Home-Page: https://didp.ai
 Author: Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>
 Author-email: Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>
```

