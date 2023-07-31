# Comparing `tmp/pymc-5.6.1.tar.gz` & `tmp/pymc-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.6.1.tar", last modified: Fri Jul 14 07:23:02 2023, max compression
+gzip compressed data, was "dist/pymc-5.7.0.tar", last modified: Mon Jul 31 08:57:00 2023, max compression
```

## Comparing `pymc-5.6.1.tar` & `pymc-5.7.0.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-14 07:22:52.000000 pymc-5.6.1/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-14 07:22:52.000000 pymc-5.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-14 07:22:52.000000 pymc-5.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-07-14 07:22:52.000000 pymc-5.6.1/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-14 07:22:52.000000 pymc-5.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 07:22:52.000000 pymc-5.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-14 07:23:02.000000 pymc-5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-14 07:22:52.000000 pymc-5.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-07-14 07:22:52.000000 pymc-5.6.1/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89229 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    85727 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39443 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 07:22:52.000000 pymc-5.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 07:22:52.000000 pymc-5.6.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-14 07:22:52.000000 pymc-5.6.1/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-07-14 07:22:52.000000 pymc-5.6.1/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 07:23:02.000000 pymc-5.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-07-14 07:22:52.000000 pymc-5.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-07-14 07:22:52.000000 pymc-5.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-31 08:56:45.000000 pymc-5.7.0/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 08:56:45.000000 pymc-5.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 08:56:45.000000 pymc-5.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-07-31 08:56:45.000000 pymc-5.7.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-31 08:56:45.000000 pymc-5.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 08:56:45.000000 pymc-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-07-31 08:57:00.000000 pymc-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-31 08:56:45.000000 pymc-5.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-07-31 08:56:45.000000 pymc-5.7.0/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90174 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85727 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39422 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36584 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57955 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 08:56:45.000000 pymc-5.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 08:56:45.000000 pymc-5.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-31 08:56:45.000000 pymc-5.7.0/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-07-31 08:56:45.000000 pymc-5.7.0/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 08:57:00.000000 pymc-5.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2653 2023-07-31 08:56:45.000000 pymc-5.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-07-31 08:56:45.000000 pymc-5.7.0/versioneer.py
```

### Comparing `pymc-5.6.1/ARCHITECTURE.md` & `pymc-5.7.0/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/CODE_OF_CONDUCT.md` & `pymc-5.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/CONTRIBUTING.md` & `pymc-5.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/GOVERNANCE.md` & `pymc-5.7.0/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/LICENSE` & `pymc-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/PKG-INFO` & `pymc-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.6.1
+Version: 5.7.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
@@ -182,18 +182,17 @@
         .. |ODSC| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/odsc/sponsor_odsc.png?raw=true
            :target: https://odsc.com/california/?utm_source=pymc&utm_medium=referral
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `pymc-5.6.1/README.rst` & `pymc-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/RELEASE-NOTES.md` & `pymc-5.7.0/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/__init__.py` & `pymc-5.7.0/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/backends/__init__.py` & `pymc-5.7.0/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/backends/arviz.py` & `pymc-5.7.0/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/backends/base.py` & `pymc-5.7.0/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/backends/mcbackend.py` & `pymc-5.7.0/pymc/backends/mcbackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from pymc.backends.base import IBaseTrace
 from pymc.model import Model
 from pymc.pytensorf import PointFunc
 from pymc.step_methods.compound import (
     BlockedStep,
     CompoundStep,
     StatsBijection,
+    check_step_emits_tune,
     flat_statname,
     flatten_steps,
 )
 
 _log = logging.getLogger(__name__)
 
 
@@ -203,31 +204,34 @@
     *,
     initial_point: Mapping[str, np.ndarray],
     step: Union[CompoundStep, BlockedStep],
     model: Model,
 ) -> Tuple[mcb.RunMeta, PointFunc]:
     variables, point_fn = get_variables_and_point_fn(model, initial_point)
 
-    sample_stats = [
-        mcb.Variable("tune", "bool"),
-    ]
+    check_step_emits_tune(step)
 
     # In PyMC the sampler stats are grouped by the sampler.
+    sample_stats = []
     steps = flatten_steps(step)
     for s, sm in enumerate(steps):
         for statname, (dtype, shape) in sm.stats_dtypes_shapes.items():
             sname = flat_statname(s, statname)
             sshape = [
                 # PyMC uses None to indicate dynamic dims, MCB uses -1
                 (-1 if s is None else s)
                 for s in (shape or [])
             ]
+            dt = np.dtype(dtype).name
+            # Object types will be pickled by the ChainRecordAdapter!
+            if dt == "object":
+                dt = "str"
             svar = mcb.Variable(
                 name=sname,
-                dtype=np.dtype(dtype).name,
+                dtype=dt,
                 shape=sshape,
                 undefined_ndim=shape is None,
             )
             sample_stats.append(svar)
 
     coordinates = [
         mcb.Coordinate(dname, mcb.npproto.utils.ndarray_from_numpy(np.array(cvals)))
```

### Comparing `pymc-5.6.1/pymc/backends/ndarray.py` & `pymc-5.7.0/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/backends/report.py` & `pymc-5.7.0/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/blocking.py` & `pymc-5.7.0/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/data.py` & `pymc-5.7.0/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/__init__.py` & `pymc-5.7.0/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/bound.py` & `pymc-5.7.0/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/censored.py` & `pymc-5.7.0/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/continuous.py` & `pymc-5.7.0/pymc/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/discrete.py` & `pymc-5.7.0/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/dist_math.py` & `pymc-5.7.0/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/distribution.py` & `pymc-5.7.0/pymc/distributions/distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from pytensor.graph.replace import clone_replace
 from pytensor.graph.rewriting.basic import in2out
 from pytensor.graph.utils import MetaType
 from pytensor.tensor.basic import as_tensor_variable
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
 from pytensor.tensor.random.utils import normalize_size_param
+from pytensor.tensor.rewriting.shape import ShapeFeature
 from pytensor.tensor.var import TensorVariable
 from typing_extensions import TypeAlias
 
 from pymc.distributions.shape_utils import (
     Dims,
     Shape,
     _change_dist_size,
@@ -50,15 +51,20 @@
 )
 from pymc.exceptions import BlockModelAccessError
 from pymc.logprob.abstract import MeasurableVariable, _icdf, _logcdf, _logprob
 from pymc.logprob.basic import logp
 from pymc.logprob.rewriting import logprob_rewrites_db
 from pymc.model import new_or_existing_block_model_access
 from pymc.printing import str_for_dist
-from pymc.pytensorf import collect_default_updates, convert_observed_data, floatX
+from pymc.pytensorf import (
+    collect_default_updates,
+    constant_fold,
+    convert_observed_data,
+    floatX,
+)
 from pymc.util import UNSET, _add_future_warning_tag
 from pymc.vartypes import continuous_types, string_types
 
 __all__ = [
     "CustomDist",
     "DensityDist",
     "DiracDelta",
@@ -478,14 +484,19 @@
         moment: Optional[Callable] = None,
         ndim_supp: int = 0,
         ndims_params: Optional[Sequence[int]] = None,
         dtype: str = "floatX",
         class_name: str = "CustomDist",
         **kwargs,
     ):
+        if ndim_supp > 0:
+            raise NotImplementedError(
+                "CustomDist with ndim_supp > 0 and without a `dist` function are not supported."
+            )
+
         dist_params = [as_tensor_variable(param) for param in dist_params]
 
         # Assume scalar ndims_params
         if ndims_params is None:
             ndims_params = [0] * len(dist_params)
 
         if logp is None:
@@ -1225,23 +1236,20 @@
                 )
                 if np.array_equal(constant_mask, expanded_mask):
                     mask = trimmed_mask
                     antimask = ~trimmed_mask
                     can_rewrite = True
 
     if can_rewrite:
-        # Rewrite doesn't work with boolean masks. Should be fixed after https://github.com/pymc-devs/pytensor/pull/329
-        mask, antimask = mask.nonzero(), antimask.nonzero()
-
         masked_rv = rv[mask]
-        fgraph = FunctionGraph(outputs=[masked_rv], clone=False)
+        fgraph = FunctionGraph(outputs=[masked_rv], clone=False, features=[ShapeFeature()])
         [unobserved_rv] = local_subtensor_rv_lift.transform(fgraph, fgraph.outputs[0].owner)
 
         antimasked_rv = rv[antimask]
-        fgraph = FunctionGraph(outputs=[antimasked_rv], clone=False)
+        fgraph = FunctionGraph(outputs=[antimasked_rv], clone=False, features=[ShapeFeature()])
         [observed_rv] = local_subtensor_rv_lift.transform(fgraph, fgraph.outputs[0].owner)
 
         # Make a clone of the observedRV, with a distinct rng so that observed and
         # unobserved are never treated as equivalent (and mergeable) nodes by pytensor.
         _, size, _, *inps = observed_rv.owner.inputs
         observed_rv = observed_rv.owner.op(*inps, size=size)
 
@@ -1266,15 +1274,15 @@
 
 
 @_logprob.register(PartialObservedRV)
 def partial_observed_rv_logprob(op, values, dist, mask, **kwargs):
     # For the logp, simply join the values
     [obs_value, unobs_value] = values
     antimask = ~mask
-    joined_value = pt.empty_like(dist)
+    joined_value = pt.empty(constant_fold([dist.shape])[0])
     joined_value = pt.set_subtensor(joined_value[mask], unobs_value)
     joined_value = pt.set_subtensor(joined_value[antimask], obs_value)
     joined_logp = logp(dist, joined_value)
 
     # If we have a univariate RV we can split apart the logp terms
     if op.ndim_supp == 0:
         return joined_logp[antimask], joined_logp[mask]
```

### Comparing `pymc-5.6.1/pymc/distributions/mixture.py` & `pymc-5.7.0/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/multivariate.py` & `pymc-5.7.0/pymc/distributions/multivariate.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,5507 +71,5566 @@
 00000460: 6e73 6f72 2e72 616e 646f 6d2e 6261 7369  nsor.random.basi
 00000470: 6320 696d 706f 7274 2064 6972 6963 686c  c import dirichl
 00000480: 6574 2c20 6d75 6c74 696e 6f6d 6961 6c2c  et, multinomial,
 00000490: 206d 756c 7469 7661 7269 6174 655f 6e6f   multivariate_no
 000004a0: 726d 616c 0a66 726f 6d20 7079 7465 6e73  rmal.from pytens
 000004b0: 6f72 2e74 656e 736f 722e 7261 6e64 6f6d  or.tensor.random
 000004c0: 2e6f 7020 696d 706f 7274 2052 616e 646f  .op import Rando
-000004d0: 6d56 6172 6961 626c 652c 2064 6566 6175  mVariable, defau
-000004e0: 6c74 5f73 7570 705f 7368 6170 655f 6672  lt_supp_shape_fr
-000004f0: 6f6d 5f70 6172 616d 730a 6672 6f6d 2070  om_params.from p
-00000500: 7974 656e 736f 722e 7465 6e73 6f72 2e72  ytensor.tensor.r
-00000510: 616e 646f 6d2e 7574 696c 7320 696d 706f  andom.utils impo
-00000520: 7274 2062 726f 6164 6361 7374 5f70 6172  rt broadcast_par
-00000530: 616d 730a 6672 6f6d 2070 7974 656e 736f  ams.from pytenso
-00000540: 722e 7465 6e73 6f72 2e73 6c69 6e61 6c67  r.tensor.slinalg
-00000550: 2069 6d70 6f72 7420 4368 6f6c 6573 6b79   import Cholesky
-00000560: 2c20 536f 6c76 6554 7269 616e 6775 6c61  , SolveTriangula
-00000570: 720a 6672 6f6d 2070 7974 656e 736f 722e  r.from pytensor.
-00000580: 7465 6e73 6f72 2e74 7970 6520 696d 706f  tensor.type impo
-00000590: 7274 2054 656e 736f 7254 7970 650a 6672  rt TensorType.fr
-000005a0: 6f6d 2073 6369 7079 2069 6d70 6f72 7420  om scipy import 
-000005b0: 6c69 6e61 6c67 2c20 7374 6174 730a 0a69  linalg, stats..i
-000005c0: 6d70 6f72 7420 7079 6d63 2061 7320 706d  mport pymc as pm
-000005d0: 0a0a 6672 6f6d 2070 796d 632e 6469 7374  ..from pymc.dist
-000005e0: 7269 6275 7469 6f6e 7320 696d 706f 7274  ributions import
-000005f0: 2074 7261 6e73 666f 726d 730a 6672 6f6d   transforms.from
-00000600: 2070 796d 632e 6469 7374 7269 6275 7469   pymc.distributi
-00000610: 6f6e 732e 636f 6e74 696e 756f 7573 2069  ons.continuous i
-00000620: 6d70 6f72 7420 426f 756e 6465 6443 6f6e  mport BoundedCon
-00000630: 7469 6e75 6f75 732c 2043 6869 5371 7561  tinuous, ChiSqua
-00000640: 7265 642c 204e 6f72 6d61 6c0a 6672 6f6d  red, Normal.from
-00000650: 2070 796d 632e 6469 7374 7269 6275 7469   pymc.distributi
-00000660: 6f6e 732e 6469 7374 5f6d 6174 6820 696d  ons.dist_math im
-00000670: 706f 7274 2028 0a20 2020 2062 6574 616c  port (.    betal
-00000680: 6e2c 0a20 2020 2063 6865 636b 5f70 6172  n,.    check_par
-00000690: 616d 6574 6572 732c 0a20 2020 2066 6163  ameters,.    fac
-000006a0: 746c 6e2c 0a20 2020 206c 6f67 706f 772c  tln,.    logpow,
-000006b0: 0a20 2020 206d 756c 7469 6761 6d6d 616c  .    multigammal
-000006c0: 6e2c 0a29 0a66 726f 6d20 7079 6d63 2e64  n,.).from pymc.d
-000006d0: 6973 7472 6962 7574 696f 6e73 2e64 6973  istributions.dis
-000006e0: 7472 6962 7574 696f 6e20 696d 706f 7274  tribution import
-000006f0: 2028 0a20 2020 2043 6f6e 7469 6e75 6f75   (.    Continuou
-00000700: 732c 0a20 2020 2044 6973 6372 6574 652c  s,.    Discrete,
-00000710: 0a20 2020 2044 6973 7472 6962 7574 696f  .    Distributio
-00000720: 6e2c 0a20 2020 2053 796d 626f 6c69 6352  n,.    SymbolicR
-00000730: 616e 646f 6d56 6172 6961 626c 652c 0a20  andomVariable,. 
-00000740: 2020 205f 6d6f 6d65 6e74 2c0a 2020 2020     _moment,.    
-00000750: 6d6f 6d65 6e74 2c0a 290a 6672 6f6d 2070  moment,.).from p
-00000760: 796d 632e 6469 7374 7269 6275 7469 6f6e  ymc.distribution
-00000770: 732e 7368 6170 655f 7574 696c 7320 696d  s.shape_utils im
-00000780: 706f 7274 2028 0a20 2020 205f 6368 616e  port (.    _chan
-00000790: 6765 5f64 6973 745f 7369 7a65 2c0a 2020  ge_dist_size,.  
-000007a0: 2020 6272 6f61 6463 6173 745f 6469 7374    broadcast_dist
-000007b0: 5f73 616d 706c 6573 5f73 6861 7065 2c0a  _samples_shape,.
-000007c0: 2020 2020 6368 616e 6765 5f64 6973 745f      change_dist_
-000007d0: 7369 7a65 2c0a 2020 2020 6765 745f 7375  size,.    get_su
-000007e0: 7070 6f72 745f 7368 6170 652c 0a20 2020  pport_shape,.   
-000007f0: 2072 765f 7369 7a65 5f69 735f 6e6f 6e65   rv_size_is_none
-00000800: 2c0a 2020 2020 746f 5f74 7570 6c65 2c0a  ,.    to_tuple,.
-00000810: 290a 6672 6f6d 2070 796d 632e 6469 7374  ).from pymc.dist
-00000820: 7269 6275 7469 6f6e 732e 7472 616e 7366  ributions.transf
-00000830: 6f72 6d73 2069 6d70 6f72 7420 496e 7465  orms import Inte
-00000840: 7276 616c 2c20 5a65 726f 5375 6d54 7261  rval, ZeroSumTra
-00000850: 6e73 666f 726d 2c20 5f64 6566 6175 6c74  nsform, _default
-00000860: 5f74 7261 6e73 666f 726d 0a66 726f 6d20  _transform.from 
-00000870: 7079 6d63 2e6c 6f67 7072 6f62 2e61 6273  pymc.logprob.abs
-00000880: 7472 6163 7420 696d 706f 7274 205f 6c6f  tract import _lo
-00000890: 6770 726f 620a 6672 6f6d 2070 796d 632e  gprob.from pymc.
-000008a0: 6d61 7468 2069 6d70 6f72 7420 6b72 6f6e  math import kron
-000008b0: 5f64 6961 672c 206b 726f 6e5f 646f 740a  _diag, kron_dot.
-000008c0: 6672 6f6d 2070 796d 632e 7079 7465 6e73  from pymc.pytens
-000008d0: 6f72 6620 696d 706f 7274 2066 6c6f 6174  orf import float
-000008e0: 582c 2069 6e74 580a 6672 6f6d 2070 796d  X, intX.from pym
-000008f0: 632e 7574 696c 2069 6d70 6f72 7420 6368  c.util import ch
-00000900: 6563 6b5f 6469 7374 5f6e 6f74 5f72 6567  eck_dist_not_reg
-00000910: 6973 7465 7265 640a 0a5f 5f61 6c6c 5f5f  istered..__all__
-00000920: 203d 205b 0a20 2020 2022 4d76 4e6f 726d   = [.    "MvNorm
-00000930: 616c 222c 0a20 2020 2022 5a65 726f 5375  al",.    "ZeroSu
-00000940: 6d4e 6f72 6d61 6c22 2c0a 2020 2020 224d  mNormal",.    "M
-00000950: 7653 7475 6465 6e74 5422 2c0a 2020 2020  vStudentT",.    
-00000960: 2244 6972 6963 686c 6574 222c 0a20 2020  "Dirichlet",.   
-00000970: 2022 4d75 6c74 696e 6f6d 6961 6c22 2c0a   "Multinomial",.
-00000980: 2020 2020 2244 6972 6963 686c 6574 4d75      "DirichletMu
-00000990: 6c74 696e 6f6d 6961 6c22 2c0a 2020 2020  ltinomial",.    
-000009a0: 224f 7264 6572 6564 4d75 6c74 696e 6f6d  "OrderedMultinom
-000009b0: 6961 6c22 2c0a 2020 2020 2257 6973 6861  ial",.    "Wisha
-000009c0: 7274 222c 0a20 2020 2022 5769 7368 6172  rt",.    "Wishar
-000009d0: 7442 6172 746c 6574 7422 2c0a 2020 2020  tBartlett",.    
-000009e0: 224c 4b4a 436f 7272 222c 0a20 2020 2022  "LKJCorr",.    "
-000009f0: 4c4b 4a43 686f 6c65 736b 7943 6f76 222c  LKJCholeskyCov",
-00000a00: 0a20 2020 2022 4d61 7472 6978 4e6f 726d  .    "MatrixNorm
-00000a10: 616c 222c 0a20 2020 2022 4b72 6f6e 6563  al",.    "Kronec
-00000a20: 6b65 724e 6f72 6d61 6c22 2c0a 2020 2020  kerNormal",.    
-00000a30: 2243 4152 222c 0a20 2020 2022 5374 6963  "CAR",.    "Stic
-00000a40: 6b42 7265 616b 696e 6757 6569 6768 7473  kBreakingWeights
-00000a50: 222c 0a5d 0a0a 736f 6c76 655f 6c6f 7765  ",.]..solve_lowe
-00000a60: 7220 3d20 536f 6c76 6554 7269 616e 6775  r = SolveTriangu
-00000a70: 6c61 7228 6c6f 7765 723d 5472 7565 290a  lar(lower=True).
-00000a80: 736f 6c76 655f 7570 7065 7220 3d20 536f  solve_upper = So
-00000a90: 6c76 6554 7269 616e 6775 6c61 7228 6c6f  lveTriangular(lo
-00000aa0: 7765 723d 4661 6c73 6529 0a0a 0a63 6c61  wer=False)...cla
-00000ab0: 7373 2053 696d 706c 6578 436f 6e74 696e  ss SimplexContin
-00000ac0: 756f 7573 2843 6f6e 7469 6e75 6f75 7329  uous(Continuous)
-00000ad0: 3a0a 2020 2020 2222 2242 6173 6520 636c  :.    """Base cl
-00000ae0: 6173 7320 666f 7220 7369 6d70 6c65 7820  ass for simplex 
-00000af0: 636f 6e74 696e 756f 7573 2064 6973 7472  continuous distr
-00000b00: 6962 7574 696f 6e73 2222 220a 0a0a 405f  ibutions"""...@_
-00000b10: 6465 6661 756c 745f 7472 616e 7366 6f72  default_transfor
-00000b20: 6d2e 7265 6769 7374 6572 2853 696d 706c  m.register(Simpl
-00000b30: 6578 436f 6e74 696e 756f 7573 290a 6465  exContinuous).de
-00000b40: 6620 7369 6d70 6c65 785f 636f 6e74 5f74  f simplex_cont_t
-00000b50: 7261 6e73 666f 726d 286f 702c 2072 7629  ransform(op, rv)
-00000b60: 3a0a 2020 2020 7265 7475 726e 2074 7261  :.    return tra
-00000b70: 6e73 666f 726d 732e 7369 6d70 6c65 780a  nsforms.simplex.
-00000b80: 0a0a 2320 5374 6570 206d 6574 686f 6473  ..# Step methods
-00000b90: 2061 6e64 2061 6476 6920 646f 206e 6f74   and advi do not
-00000ba0: 2063 6174 6368 204c 696e 416c 6745 7272   catch LinAlgErr
-00000bb0: 6f72 7320 6174 2074 6865 0a23 206d 6f6d  ors at the.# mom
-00000bc0: 656e 742e 2057 6520 776f 726b 2061 726f  ent. We work aro
-00000bd0: 756e 6420 7468 6174 2062 7920 7573 696e  und that by usin
-00000be0: 6720 6120 6368 6f6c 6573 6b79 206f 700a  g a cholesky op.
-00000bf0: 2320 7468 6174 2072 6574 7572 6e73 2061  # that returns a
-00000c00: 206e 616e 2061 7320 6669 7273 7420 656e   nan as first en
-00000c10: 7472 7920 696e 7374 6561 6420 6f66 2072  try instead of r
-00000c20: 6169 7369 6e67 0a23 2061 6e20 6572 726f  aising.# an erro
-00000c30: 722e 0a63 686f 6c65 736b 7920 3d20 4368  r..cholesky = Ch
-00000c40: 6f6c 6573 6b79 286c 6f77 6572 3d54 7275  olesky(lower=Tru
-00000c50: 652c 206f 6e5f 6572 726f 723d 226e 616e  e, on_error="nan
-00000c60: 2229 0a0a 0a64 6566 2071 7561 6464 6973  ")...def quaddis
-00000c70: 745f 6d61 7472 6978 2863 6f76 3d4e 6f6e  t_matrix(cov=Non
-00000c80: 652c 2063 686f 6c3d 4e6f 6e65 2c20 7461  e, chol=None, ta
-00000c90: 753d 4e6f 6e65 2c20 6c6f 7765 723d 5472  u=None, lower=Tr
-00000ca0: 7565 2c20 2a61 7267 732c 202a 2a6b 7761  ue, *args, **kwa
-00000cb0: 7267 7329 3a0a 2020 2020 6966 2063 686f  rgs):.    if cho
-00000cc0: 6c20 6973 206e 6f74 204e 6f6e 6520 616e  l is not None an
-00000cd0: 6420 6e6f 7420 6c6f 7765 723a 0a20 2020  d not lower:.   
-00000ce0: 2020 2020 2063 686f 6c20 3d20 6368 6f6c       chol = chol
-00000cf0: 2e54 0a0a 2020 2020 6966 206c 656e 285b  .T..    if len([
-00000d00: 6920 666f 7220 6920 696e 205b 7461 752c  i for i in [tau,
-00000d10: 2063 6f76 2c20 6368 6f6c 5d20 6966 2069   cov, chol] if i
-00000d20: 2069 7320 6e6f 7420 4e6f 6e65 5d29 2021   is not None]) !
-00000d30: 3d20 313a 0a20 2020 2020 2020 2072 6169  = 1:.        rai
-00000d40: 7365 2056 616c 7565 4572 726f 7228 2249  se ValueError("I
-00000d50: 6e63 6f6d 7061 7469 626c 6520 7061 7261  ncompatible para
-00000d60: 6d65 7465 7269 7a61 7469 6f6e 2e20 5370  meterization. Sp
-00000d70: 6563 6966 7920 6578 6163 746c 7920 6f6e  ecify exactly on
-00000d80: 6520 6f66 2074 6175 2c20 636f 762c 206f  e of tau, cov, o
-00000d90: 7220 6368 6f6c 2e22 290a 0a20 2020 2069  r chol.")..    i
-00000da0: 6620 636f 7620 6973 206e 6f74 204e 6f6e  f cov is not Non
-00000db0: 653a 0a20 2020 2020 2020 2063 6f76 203d  e:.        cov =
-00000dc0: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00000dd0: 7269 6162 6c65 2863 6f76 290a 2020 2020  riable(cov).    
-00000de0: 2020 2020 6966 2063 6f76 2e6e 6469 6d20      if cov.ndim 
-00000df0: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
-00000e00: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00000e10: 6f72 2822 636f 7620 6d75 7374 2062 6520  or("cov must be 
-00000e20: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
-00000e30: 2229 0a20 2020 2065 6c69 6620 7461 7520  ").    elif tau 
-00000e40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00000e50: 2020 2020 2074 6175 203d 2070 742e 6173       tau = pt.as
-00000e60: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-00000e70: 2874 6175 290a 2020 2020 2020 2020 6966  (tau).        if
-00000e80: 2074 6175 2e6e 6469 6d20 213d 2032 3a0a   tau.ndim != 2:.
-00000e90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00000ea0: 6520 5661 6c75 6545 7272 6f72 2822 7461  e ValueError("ta
-00000eb0: 7520 6d75 7374 2062 6520 7477 6f20 6469  u must be two di
-00000ec0: 6d65 6e73 696f 6e61 6c2e 2229 0a20 2020  mensional.").   
-00000ed0: 2020 2020 2023 2054 4f44 4f3a 2057 6861       # TODO: Wha
-00000ee0: 7427 7320 7468 6520 636f 7272 6563 7420  t's the correct 
-00000ef0: 6f72 6465 722f 6170 7072 6f61 6368 2028  order/approach (
-00000f00: 696e 2074 6865 206e 6f6e 2d73 7175 6172  in the non-squar
-00000f10: 6520 6361 7365 293f 0a20 2020 2020 2020  e case)?.       
-00000f20: 2023 2060 7079 7465 6e73 6f72 2e74 656e   # `pytensor.ten
-00000f30: 736f 722e 6e6c 696e 616c 672e 7465 6e73  sor.nlinalg.tens
-00000f40: 6f72 696e 7660 3f0a 2020 2020 2020 2020  orinv`?.        
-00000f50: 636f 7620 3d20 6d61 7472 6978 5f69 6e76  cov = matrix_inv
-00000f60: 6572 7365 2874 6175 290a 2020 2020 656c  erse(tau).    el
-00000f70: 7365 3a0a 2020 2020 2020 2020 2320 544f  se:.        # TO
-00000f80: 444f 3a20 5768 6174 2773 2074 6865 2063  DO: What's the c
-00000f90: 6f72 7265 6374 206f 7264 6572 2f61 7070  orrect order/app
-00000fa0: 726f 6163 6820 2869 6e20 7468 6520 6e6f  roach (in the no
-00000fb0: 6e2d 7371 7561 7265 2063 6173 6529 3f0a  n-square case)?.
-00000fc0: 2020 2020 2020 2020 6368 6f6c 203d 2070          chol = p
-00000fd0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00000fe0: 6162 6c65 2863 686f 6c29 0a20 2020 2020  able(chol).     
-00000ff0: 2020 2069 6620 6368 6f6c 2e6e 6469 6d20     if chol.ndim 
-00001000: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
-00001010: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00001020: 6f72 2822 6368 6f6c 206d 7573 7420 6265  or("chol must be
-00001030: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
-00001040: 2e22 290a 0a20 2020 2020 2020 2023 2074  .")..        # t
-00001050: 6167 2061 7320 6c6f 7765 7220 7472 6961  ag as lower tria
-00001060: 6e67 756c 6172 2074 6f20 656e 6162 6c65  ngular to enable
-00001070: 2070 7974 656e 736f 7220 7265 7772 6974   pytensor rewrit
-00001080: 6573 206f 6620 6368 6f6c 286c 2e6c 2729  es of chol(l.l')
-00001090: 202d 3e20 6c0a 2020 2020 2020 2020 6368   -> l.        ch
-000010a0: 6f6c 2e74 6167 2e6c 6f77 6572 5f74 7269  ol.tag.lower_tri
-000010b0: 616e 6775 6c61 7220 3d20 5472 7565 0a20  angular = True. 
-000010c0: 2020 2020 2020 2063 6f76 203d 2063 686f         cov = cho
-000010d0: 6c2e 646f 7428 6368 6f6c 2e54 290a 0a20  l.dot(chol.T).. 
-000010e0: 2020 2072 6574 7572 6e20 636f 760a 0a0a     return cov...
-000010f0: 6465 6620 7175 6164 6469 7374 5f70 6172  def quaddist_par
-00001100: 7365 2876 616c 7565 2c20 6d75 2c20 636f  se(value, mu, co
-00001110: 762c 206d 6174 5f74 7970 653d 2263 6f76  v, mat_type="cov
-00001120: 2229 3a0a 2020 2020 2222 2243 6f6d 7075  "):.    """Compu
-00001130: 7465 2028 7820 2d20 6d75 292e 5420 4020  te (x - mu).T @ 
-00001140: 5369 676d 615e 2d31 2040 2028 7820 2d20  Sigma^-1 @ (x - 
-00001150: 6d75 2920 616e 6420 7468 6520 6c6f 6764  mu) and the logd
-00001160: 6574 206f 6620 5369 676d 612e 2222 220a  et of Sigma.""".
-00001170: 2020 2020 6966 2076 616c 7565 2e6e 6469      if value.ndi
-00001180: 6d20 3e20 3220 6f72 2076 616c 7565 2e6e  m > 2 or value.n
-00001190: 6469 6d20 3d3d 2030 3a0a 2020 2020 2020  dim == 0:.      
-000011a0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000011b0: 6f72 2822 496e 7661 6c69 6420 6469 6d65  or("Invalid dime
-000011c0: 6e73 696f 6e20 666f 7220 7661 6c75 653a  nsion for value:
-000011d0: 2025 7322 2025 2076 616c 7565 2e6e 6469   %s" % value.ndi
-000011e0: 6d29 0a20 2020 2069 6620 7661 6c75 652e  m).    if value.
-000011f0: 6e64 696d 203d 3d20 313a 0a20 2020 2020  ndim == 1:.     
-00001200: 2020 206f 6e65 6469 6d20 3d20 5472 7565     onedim = True
-00001210: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
-00001220: 2076 616c 7565 5b4e 6f6e 652c 203a 5d0a   value[None, :].
-00001230: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001240: 2020 6f6e 6564 696d 203d 2046 616c 7365    onedim = False
-00001250: 0a0a 2020 2020 6465 6c74 6120 3d20 7661  ..    delta = va
-00001260: 6c75 6520 2d20 6d75 0a20 2020 2023 2055  lue - mu.    # U
-00001270: 7365 2074 6869 7320 7768 656e 2054 6865  se this when The
-00001280: 616e 6f23 3539 3038 2069 7320 7265 6c65  ano#5908 is rele
-00001290: 6173 6564 2e0a 2020 2020 2320 7265 7475  ased..    # retu
-000012a0: 726e 204d 764e 6f72 6d61 6c4c 6f67 7028  rn MvNormalLogp(
-000012b0: 2928 7365 6c66 2e63 6f76 2c20 6465 6c74  )(self.cov, delt
-000012c0: 6129 0a20 2020 2063 686f 6c5f 636f 7620  a).    chol_cov 
-000012d0: 3d20 6368 6f6c 6573 6b79 2863 6f76 290a  = cholesky(cov).
-000012e0: 2020 2020 6966 206d 6174 5f74 7970 6520      if mat_type 
-000012f0: 213d 2022 7461 7522 3a0a 2020 2020 2020  != "tau":.      
-00001300: 2020 6469 7374 2c20 6c6f 6764 6574 2c20    dist, logdet, 
-00001310: 6f6b 203d 2071 7561 6464 6973 745f 6368  ok = quaddist_ch
-00001320: 6f6c 2864 656c 7461 2c20 6368 6f6c 5f63  ol(delta, chol_c
-00001330: 6f76 290a 2020 2020 656c 7365 3a0a 2020  ov).    else:.  
-00001340: 2020 2020 2020 6469 7374 2c20 6c6f 6764        dist, logd
-00001350: 6574 2c20 6f6b 203d 2071 7561 6464 6973  et, ok = quaddis
-00001360: 745f 7461 7528 6465 6c74 612c 2063 686f  t_tau(delta, cho
-00001370: 6c5f 636f 7629 0a20 2020 2069 6620 6f6e  l_cov).    if on
-00001380: 6564 696d 3a0a 2020 2020 2020 2020 7265  edim:.        re
-00001390: 7475 726e 2064 6973 745b 305d 2c20 6c6f  turn dist[0], lo
-000013a0: 6764 6574 2c20 6f6b 0a0a 2020 2020 7265  gdet, ok..    re
-000013b0: 7475 726e 2064 6973 742c 206c 6f67 6465  turn dist, logde
-000013c0: 742c 206f 6b0a 0a0a 6465 6620 7175 6164  t, ok...def quad
-000013d0: 6469 7374 5f63 686f 6c28 6465 6c74 612c  dist_chol(delta,
-000013e0: 2063 686f 6c5f 6d61 7429 3a0a 2020 2020   chol_mat):.    
-000013f0: 6469 6167 203d 2070 742e 6469 6167 2863  diag = pt.diag(c
-00001400: 686f 6c5f 6d61 7429 0a20 2020 2023 2043  hol_mat).    # C
-00001410: 6865 636b 2069 6620 7468 6520 636f 7661  heck if the cova
-00001420: 7269 616e 6365 206d 6174 7269 7820 6973  riance matrix is
-00001430: 2070 6f73 6974 6976 6520 6465 6669 6e69   positive defini
-00001440: 7465 2e0a 2020 2020 6f6b 203d 2070 742e  te..    ok = pt.
-00001450: 616c 6c28 6469 6167 203e 2030 290a 2020  all(diag > 0).  
-00001460: 2020 2320 4966 206e 6f74 2c20 7265 706c    # If not, repl
-00001470: 6163 6520 7468 6520 6469 6167 6f6e 616c  ace the diagonal
-00001480: 2e20 5765 2072 6574 7572 6e20 2d69 6e66  . We return -inf
-00001490: 206c 6174 6572 2c20 6275 740a 2020 2020   later, but.    
-000014a0: 2320 6e65 6564 2074 6f20 7072 6576 656e  # need to preven
-000014b0: 7420 736f 6c76 655f 6c6f 7765 7220 6672  t solve_lower fr
-000014c0: 6f6d 2074 6872 6f77 696e 6720 616e 2065  om throwing an e
-000014d0: 7863 6570 7469 6f6e 2e0a 2020 2020 6368  xception..    ch
-000014e0: 6f6c 5f63 6f76 203d 2070 742e 7377 6974  ol_cov = pt.swit
-000014f0: 6368 286f 6b2c 2063 686f 6c5f 6d61 742c  ch(ok, chol_mat,
-00001500: 2031 290a 0a20 2020 2064 656c 7461 5f74   1)..    delta_t
-00001510: 7261 6e73 203d 2073 6f6c 7665 5f6c 6f77  rans = solve_low
-00001520: 6572 2863 686f 6c5f 636f 762c 2064 656c  er(chol_cov, del
-00001530: 7461 2e54 292e 540a 2020 2020 7175 6164  ta.T).T.    quad
-00001540: 6469 7374 203d 2028 6465 6c74 615f 7472  dist = (delta_tr
-00001550: 616e 732a 2a32 292e 7375 6d28 6178 6973  ans**2).sum(axis
-00001560: 3d2d 3129 0a20 2020 206c 6f67 6465 7420  =-1).    logdet 
-00001570: 3d20 7074 2e73 756d 2870 742e 6c6f 6728  = pt.sum(pt.log(
-00001580: 6469 6167 2929 0a20 2020 2072 6574 7572  diag)).    retur
-00001590: 6e20 7175 6164 6469 7374 2c20 6c6f 6764  n quaddist, logd
-000015a0: 6574 2c20 6f6b 0a0a 0a64 6566 2071 7561  et, ok...def qua
-000015b0: 6464 6973 745f 7461 7528 6465 6c74 612c  ddist_tau(delta,
-000015c0: 2063 686f 6c5f 6d61 7429 3a0a 2020 2020   chol_mat):.    
-000015d0: 6469 6167 203d 2070 742e 6e6c 696e 616c  diag = pt.nlinal
-000015e0: 672e 6469 6167 2863 686f 6c5f 6d61 7429  g.diag(chol_mat)
-000015f0: 0a20 2020 2023 2043 6865 636b 2069 6620  .    # Check if 
-00001600: 7468 6520 7072 6563 6973 696f 6e20 6d61  the precision ma
-00001610: 7472 6978 2069 7320 706f 7369 7469 7665  trix is positive
-00001620: 2064 6566 696e 6974 652e 0a20 2020 206f   definite..    o
-00001630: 6b20 3d20 7074 2e61 6c6c 2864 6961 6720  k = pt.all(diag 
-00001640: 3e20 3029 0a20 2020 2023 2049 6620 6e6f  > 0).    # If no
-00001650: 742c 2072 6570 6c61 6365 2074 6865 2064  t, replace the d
-00001660: 6961 676f 6e61 6c2e 2057 6520 7265 7475  iagonal. We retu
-00001670: 726e 202d 696e 6620 6c61 7465 722c 2062  rn -inf later, b
-00001680: 7574 0a20 2020 2023 206e 6565 6420 746f  ut.    # need to
-00001690: 2070 7265 7665 6e74 2073 6f6c 7665 5f6c   prevent solve_l
-000016a0: 6f77 6572 2066 726f 6d20 7468 726f 7769  ower from throwi
-000016b0: 6e67 2061 6e20 6578 6365 7074 696f 6e2e  ng an exception.
-000016c0: 0a20 2020 2063 686f 6c5f 7461 7520 3d20  .    chol_tau = 
-000016d0: 7074 2e73 7769 7463 6828 6f6b 2c20 6368  pt.switch(ok, ch
-000016e0: 6f6c 5f6d 6174 2c20 3129 0a0a 2020 2020  ol_mat, 1)..    
-000016f0: 6465 6c74 615f 7472 616e 7320 3d20 7074  delta_trans = pt
-00001700: 2e64 6f74 2864 656c 7461 2c20 6368 6f6c  .dot(delta, chol
-00001710: 5f74 6175 290a 2020 2020 7175 6164 6469  _tau).    quaddi
-00001720: 7374 203d 2028 6465 6c74 615f 7472 616e  st = (delta_tran
-00001730: 732a 2a32 292e 7375 6d28 6178 6973 3d2d  s**2).sum(axis=-
-00001740: 3129 0a20 2020 206c 6f67 6465 7420 3d20  1).    logdet = 
-00001750: 2d70 742e 7375 6d28 7074 2e6c 6f67 2864  -pt.sum(pt.log(d
-00001760: 6961 6729 290a 2020 2020 7265 7475 726e  iag)).    return
-00001770: 2071 7561 6464 6973 742c 206c 6f67 6465   quaddist, logde
-00001780: 742c 206f 6b0a 0a0a 636c 6173 7320 4d76  t, ok...class Mv
-00001790: 4e6f 726d 616c 2843 6f6e 7469 6e75 6f75  Normal(Continuou
-000017a0: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
-000017b0: 204d 756c 7469 7661 7269 6174 6520 6e6f   Multivariate no
-000017c0: 726d 616c 206c 6f67 2d6c 696b 656c 6968  rmal log-likelih
-000017d0: 6f6f 642e 0a0a 2020 2020 2e2e 206d 6174  ood...    .. mat
-000017e0: 683a 3a0a 0a20 2020 2020 2020 6628 7820  h::..       f(x 
-000017f0: 5c6d 6964 205c 7069 2c20 5429 203d 0a20  \mid \pi, T) =. 
-00001800: 2020 2020 2020 2020 2020 5c66 7261 637b            \frac{
-00001810: 7c54 7c5e 7b31 2f32 7d7d 7b28 325c 7069  |T|^{1/2}}{(2\pi
-00001820: 295e 7b6b 2f32 7d7d 0a20 2020 2020 2020  )^{k/2}}.       
-00001830: 2020 2020 5c65 7870 5c6c 6566 745c 7b20      \exp\left\{ 
-00001840: 2d5c 6672 6163 7b31 7d7b 327d 2028 782d  -\frac{1}{2} (x-
-00001850: 5c6d 7529 5e7b 5c70 7269 6d65 7d20 5420  \mu)^{\prime} T 
-00001860: 2878 2d5c 6d75 2920 5c72 6967 6874 5c7d  (x-\mu) \right\}
-00001870: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  ..    ========  
-00001880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001890: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
-000018a0: 7570 706f 7274 2020 203a 6d61 7468 3a60  upport   :math:`
-000018b0: 7820 5c69 6e20 5c6d 6174 6862 627b 527d  x \in \mathbb{R}
-000018c0: 5e6b 600a 2020 2020 4d65 616e 2020 2020  ^k`.    Mean    
-000018d0: 2020 3a6d 6174 683a 605c 6d75 600a 2020    :math:`\mu`.  
-000018e0: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
-000018f0: 683a 6054 5e7b 2d31 7d60 0a20 2020 203d  h:`T^{-1}`.    =
-00001900: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
-00001910: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001920: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
-00001930: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00001940: 2d2d 0a20 2020 206d 7520 3a20 7465 6e73  --.    mu : tens
-00001950: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-00001960: 0a20 2020 2020 2020 2056 6563 746f 7220  .        Vector 
-00001970: 6f66 206d 6561 6e73 2e0a 2020 2020 636f  of means..    co
-00001980: 7620 3a20 7465 6e73 6f72 5f6c 696b 6520  v : tensor_like 
-00001990: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
-000019a0: 616c 0a20 2020 2020 2020 2043 6f76 6172  al.        Covar
-000019b0: 6961 6e63 6520 6d61 7472 6978 2e20 4578  iance matrix. Ex
-000019c0: 6163 746c 7920 6f6e 6520 6f66 2063 6f76  actly one of cov
-000019d0: 2c20 7461 752c 206f 7220 6368 6f6c 2069  , tau, or chol i
-000019e0: 7320 6e65 6564 6564 2e0a 2020 2020 7461  s needed..    ta
-000019f0: 7520 3a20 7465 6e73 6f72 5f6c 696b 6520  u : tensor_like 
-00001a00: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
-00001a10: 616c 0a20 2020 2020 2020 2050 7265 6369  al.        Preci
-00001a20: 7369 6f6e 206d 6174 7269 782e 2045 7861  sion matrix. Exa
-00001a30: 6374 6c79 206f 6e65 206f 6620 636f 762c  ctly one of cov,
-00001a40: 2074 6175 2c20 6f72 2063 686f 6c20 6973   tau, or chol is
-00001a50: 206e 6565 6465 642e 0a20 2020 2063 686f   needed..    cho
-00001a60: 6c20 3a20 7465 6e73 6f72 5f6c 696b 6520  l : tensor_like 
-00001a70: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
-00001a80: 616c 0a20 2020 2020 2020 2043 686f 6c65  al.        Chole
-00001a90: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
-00001aa0: 6e20 6f66 2063 6f76 6172 6961 6e63 6520  n of covariance 
-00001ab0: 6d61 7472 6978 2e20 4578 6163 746c 7920  matrix. Exactly 
-00001ac0: 6f6e 6520 6f66 2063 6f76 2c0a 2020 2020  one of cov,.    
-00001ad0: 2020 2020 7461 752c 206f 7220 6368 6f6c      tau, or chol
-00001ae0: 2069 7320 6e65 6564 6564 2e0a 2020 2020   is needed..    
-00001af0: 6c6f 7765 723a 2062 6f6f 6c2c 2064 6566  lower: bool, def
-00001b00: 6175 6c74 3d54 7275 650a 2020 2020 2020  ault=True.      
-00001b10: 2020 5768 6574 6865 7220 6368 6f6c 2069    Whether chol i
-00001b20: 7320 7468 6520 6c6f 7765 7220 7472 6964  s the lower trid
-00001b30: 6961 676f 6e61 6c20 6368 6f6c 6573 6b79  iagonal cholesky
-00001b40: 2066 6163 746f 722e 0a0a 2020 2020 4578   factor...    Ex
-00001b50: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-00001b60: 2d2d 2d0a 2020 2020 4465 6669 6e65 2061  ---.    Define a
-00001b70: 206d 756c 7469 7661 7269 6174 6520 6e6f   multivariate no
-00001b80: 726d 616c 2076 6172 6961 626c 6520 666f  rmal variable fo
-00001b90: 7220 6120 6769 7665 6e20 636f 7661 7269  r a given covari
-00001ba0: 616e 6365 0a20 2020 206d 6174 7269 783a  ance.    matrix:
-00001bb0: 3a0a 0a20 2020 2020 2020 2063 6f76 203d  :..        cov =
-00001bc0: 206e 702e 6172 7261 7928 5b5b 312e 2c20   np.array([[1., 
-00001bd0: 302e 355d 2c20 5b30 2e35 2c20 325d 5d29  0.5], [0.5, 2]])
-00001be0: 0a20 2020 2020 2020 206d 7520 3d20 6e70  .        mu = np
-00001bf0: 2e7a 6572 6f73 2832 290a 2020 2020 2020  .zeros(2).      
-00001c00: 2020 7661 6c73 203d 2070 6d2e 4d76 4e6f    vals = pm.MvNo
-00001c10: 726d 616c 2827 7661 6c73 272c 206d 753d  rmal('vals', mu=
-00001c20: 6d75 2c20 636f 763d 636f 762c 2073 6861  mu, cov=cov, sha
-00001c30: 7065 3d28 352c 2032 2929 0a0a 2020 2020  pe=(5, 2))..    
-00001c40: 4d6f 7374 206f 6620 7468 6520 7469 6d65  Most of the time
-00001c50: 2069 7420 6973 2070 7265 6665 7261 626c   it is preferabl
-00001c60: 6520 746f 2073 7065 6369 6679 2074 6865  e to specify the
-00001c70: 2063 686f 6c65 736b 790a 2020 2020 6661   cholesky.    fa
-00001c80: 6374 6f72 206f 6620 7468 6520 636f 7661  ctor of the cova
-00001c90: 7269 616e 6365 2069 6e73 7465 6164 2e20  riance instead. 
-00001ca0: 466f 7220 6578 616d 706c 652c 2077 6520  For example, we 
-00001cb0: 636f 756c 640a 2020 2020 6669 7420 6120  could.    fit a 
-00001cc0: 6d75 6c74 6976 6172 6961 7465 206f 7574  multivariate out
-00001cd0: 636f 6d65 206c 696b 6520 7468 6973 2028  come like this (
-00001ce0: 7365 6520 7468 6520 646f 6373 7472 696e  see the docstrin
-00001cf0: 670a 2020 2020 6f66 2060 4c4b 4a43 686f  g.    of `LKJCho
-00001d00: 6c65 736b 7943 6f76 6020 666f 7220 6d6f  leskyCov` for mo
-00001d10: 7265 2069 6e66 6f72 6d61 7469 6f6e 2061  re information a
-00001d20: 626f 7574 2074 6869 7329 3a3a 0a0a 2020  bout this)::..  
-00001d30: 2020 2020 2020 6d75 203d 206e 702e 7a65        mu = np.ze
-00001d40: 726f 7328 3329 0a20 2020 2020 2020 2074  ros(3).        t
-00001d50: 7275 655f 636f 7620 3d20 6e70 2e61 7272  rue_cov = np.arr
-00001d60: 6179 285b 5b31 2e30 2c20 302e 352c 2030  ay([[1.0, 0.5, 0
-00001d70: 2e31 5d2c 0a20 2020 2020 2020 2020 2020  .1],.           
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2020 5b30 2e35 2c20 322e 302c 2030 2e32    [0.5, 2.0, 0.2
-00001da0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 5b30 2e31 2c20 302e 322c 2031 2e30 5d5d  [0.1, 0.2, 1.0]]
-00001dd0: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
-00001de0: 206e 702e 7261 6e64 6f6d 2e6d 756c 7469   np.random.multi
-00001df0: 7661 7269 6174 655f 6e6f 726d 616c 286d  variate_normal(m
-00001e00: 752c 2074 7275 655f 636f 762c 2031 3029  u, true_cov, 10)
-00001e10: 0a0a 2020 2020 2020 2020 7364 5f64 6973  ..        sd_dis
-00001e20: 7420 3d20 706d 2e45 7870 6f6e 656e 7469  t = pm.Exponenti
-00001e30: 616c 2e64 6973 7428 312e 302c 2073 6861  al.dist(1.0, sha
-00001e40: 7065 3d33 290a 2020 2020 2020 2020 6368  pe=3).        ch
-00001e50: 6f6c 2c20 636f 7272 2c20 7374 6473 203d  ol, corr, stds =
-00001e60: 2070 6d2e 4c4b 4a43 686f 6c65 736b 7943   pm.LKJCholeskyC
-00001e70: 6f76 2827 6368 6f6c 5f63 6f76 272c 206e  ov('chol_cov', n
-00001e80: 3d33 2c20 6574 613d 322c 0a20 2020 2020  =3, eta=2,.     
-00001e90: 2020 2020 2020 2073 645f 6469 7374 3d73         sd_dist=s
-00001ea0: 645f 6469 7374 2c20 636f 6d70 7574 655f  d_dist, compute_
-00001eb0: 636f 7272 3d54 7275 6529 0a20 2020 2020  corr=True).     
-00001ec0: 2020 2076 616c 7320 3d20 706d 2e4d 764e     vals = pm.MvN
-00001ed0: 6f72 6d61 6c28 2776 616c 7327 2c20 6d75  ormal('vals', mu
-00001ee0: 3d6d 752c 2063 686f 6c3d 6368 6f6c 2c20  =mu, chol=chol, 
-00001ef0: 6f62 7365 7276 6564 3d64 6174 6129 0a0a  observed=data)..
-00001f00: 2020 2020 466f 7220 756e 6f62 7365 7276      For unobserv
-00001f10: 6564 2076 616c 7565 7320 6974 2063 616e  ed values it can
-00001f20: 2062 6520 6265 7474 6572 2074 6f20 7573   be better to us
-00001f30: 6520 6120 6e6f 6e2d 6365 6e74 6572 6564  e a non-centered
-00001f40: 0a20 2020 2070 6172 616d 6574 7269 7a61  .    parametriza
-00001f50: 7469 6f6e 3a3a 0a0a 2020 2020 2020 2020  tion::..        
-00001f60: 7364 5f64 6973 7420 3d20 706d 2e45 7870  sd_dist = pm.Exp
-00001f70: 6f6e 656e 7469 616c 2e64 6973 7428 312e  onential.dist(1.
-00001f80: 302c 2073 6861 7065 3d33 290a 2020 2020  0, shape=3).    
-00001f90: 2020 2020 6368 6f6c 2c20 5f2c 205f 203d      chol, _, _ =
-00001fa0: 2070 6d2e 4c4b 4a43 686f 6c65 736b 7943   pm.LKJCholeskyC
-00001fb0: 6f76 2827 6368 6f6c 5f63 6f76 272c 206e  ov('chol_cov', n
-00001fc0: 3d33 2c20 6574 613d 322c 0a20 2020 2020  =3, eta=2,.     
-00001fd0: 2020 2020 2020 2073 645f 6469 7374 3d73         sd_dist=s
-00001fe0: 645f 6469 7374 2c20 636f 6d70 7574 655f  d_dist, compute_
-00001ff0: 636f 7272 3d54 7275 6529 0a20 2020 2020  corr=True).     
-00002000: 2020 2076 616c 735f 7261 7720 3d20 706d     vals_raw = pm
-00002010: 2e4e 6f72 6d61 6c28 2776 616c 735f 7261  .Normal('vals_ra
-00002020: 7727 2c20 6d75 3d30 2c20 7369 676d 613d  w', mu=0, sigma=
-00002030: 312c 2073 6861 7065 3d28 352c 2033 2929  1, shape=(5, 3))
-00002040: 0a20 2020 2020 2020 2076 616c 7320 3d20  .        vals = 
-00002050: 706d 2e44 6574 6572 6d69 6e69 7374 6963  pm.Deterministic
-00002060: 2827 7661 6c73 272c 2070 742e 646f 7428  ('vals', pt.dot(
-00002070: 6368 6f6c 2c20 7661 6c73 5f72 6177 2e54  chol, vals_raw.T
-00002080: 292e 5429 0a20 2020 2022 2222 0a20 2020  ).T).    """.   
-00002090: 2072 765f 6f70 203d 206d 756c 7469 7661   rv_op = multiva
-000020a0: 7269 6174 655f 6e6f 726d 616c 0a0a 2020  riate_normal..  
-000020b0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-000020c0: 2020 2064 6566 2064 6973 7428 636c 732c     def dist(cls,
-000020d0: 206d 752c 2063 6f76 3d4e 6f6e 652c 2074   mu, cov=None, t
-000020e0: 6175 3d4e 6f6e 652c 2063 686f 6c3d 4e6f  au=None, chol=No
-000020f0: 6e65 2c20 6c6f 7765 723d 5472 7565 2c20  ne, lower=True, 
-00002100: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00002110: 2020 206d 7520 3d20 7074 2e61 735f 7465     mu = pt.as_te
-00002120: 6e73 6f72 5f76 6172 6961 626c 6528 6d75  nsor_variable(mu
-00002130: 290a 2020 2020 2020 2020 636f 7620 3d20  ).        cov = 
-00002140: 7175 6164 6469 7374 5f6d 6174 7269 7828  quaddist_matrix(
-00002150: 636f 762c 2063 686f 6c2c 2074 6175 2c20  cov, chol, tau, 
-00002160: 6c6f 7765 7229 0a20 2020 2020 2020 2023  lower).        #
-00002170: 2050 7954 656e 736f 7220 6973 2073 7472   PyTensor is str
-00002180: 6963 7465 7220 6162 6f75 7420 7468 6520  icter about the 
-00002190: 7368 6170 6520 6f66 206d 752c 2074 6861  shape of mu, tha
-000021a0: 6e20 5079 4d43 2075 7365 6420 746f 2062  n PyMC used to b
-000021b0: 650a 2020 2020 2020 2020 6d75 203d 2070  e.        mu = p
-000021c0: 742e 6272 6f61 6463 6173 745f 6172 7261  t.broadcast_arra
-000021d0: 7973 286d 752c 2063 6f76 5b2e 2e2e 2c20  ys(mu, cov[..., 
-000021e0: 2d31 5d29 5b30 5d0a 2020 2020 2020 2020  -1])[0].        
-000021f0: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
-00002200: 6973 7428 5b6d 752c 2063 6f76 5d2c 202a  ist([mu, cov], *
-00002210: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-00002220: 6620 6d6f 6d65 6e74 2872 762c 2073 697a  f moment(rv, siz
-00002230: 652c 206d 752c 2063 6f76 293a 0a20 2020  e, mu, cov):.   
-00002240: 2020 2020 206d 6f6d 656e 7420 3d20 6d75       moment = mu
-00002250: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00002260: 7276 5f73 697a 655f 6973 5f6e 6f6e 6528  rv_size_is_none(
-00002270: 7369 7a65 293a 0a20 2020 2020 2020 2020  size):.         
-00002280: 2020 206d 6f6d 656e 745f 7369 7a65 203d     moment_size =
-00002290: 2070 742e 636f 6e63 6174 656e 6174 6528   pt.concatenate(
-000022a0: 5b73 697a 652c 205b 6d75 2e73 6861 7065  [size, [mu.shape
-000022b0: 5b2d 315d 5d5d 290a 2020 2020 2020 2020  [-1]]]).        
-000022c0: 2020 2020 6d6f 6d65 6e74 203d 2070 742e      moment = pt.
-000022d0: 6675 6c6c 286d 6f6d 656e 745f 7369 7a65  full(moment_size
-000022e0: 2c20 6d75 290a 2020 2020 2020 2020 7265  , mu).        re
-000022f0: 7475 726e 206d 6f6d 656e 740a 0a20 2020  turn moment..   
-00002300: 2064 6566 206c 6f67 7028 7661 6c75 652c   def logp(value,
-00002310: 206d 752c 2063 6f76 293a 0a20 2020 2020   mu, cov):.     
-00002320: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00002330: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
-00002340: 6261 6269 6c69 7479 206f 6620 4d75 6c74  bability of Mult
-00002350: 6976 6172 6961 7465 204e 6f72 6d61 6c20  ivariate Normal 
-00002360: 6469 7374 7269 6275 7469 6f6e 0a20 2020  distribution.   
-00002370: 2020 2020 2061 7420 7370 6563 6966 6965       at specifie
-00002380: 6420 7661 6c75 652e 0a0a 2020 2020 2020  d value...      
-00002390: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000023a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000023b0: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
-000023c0: 756d 6572 6963 0a20 2020 2020 2020 2020  umeric.         
-000023d0: 2020 2056 616c 7565 2066 6f72 2077 6869     Value for whi
-000023e0: 6368 206c 6f67 2d70 726f 6261 6269 6c69  ch log-probabili
-000023f0: 7479 2069 7320 6361 6c63 756c 6174 6564  ty is calculated
-00002400: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00002410: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00002420: 2d2d 0a20 2020 2020 2020 2054 656e 736f  --.        Tenso
-00002430: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
-00002440: 2020 2222 220a 2020 2020 2020 2020 7175    """.        qu
-00002450: 6164 6469 7374 2c20 6c6f 6764 6574 2c20  addist, logdet, 
-00002460: 6f6b 203d 2071 7561 6464 6973 745f 7061  ok = quaddist_pa
-00002470: 7273 6528 7661 6c75 652c 206d 752c 2063  rse(value, mu, c
-00002480: 6f76 290a 2020 2020 2020 2020 6b20 3d20  ov).        k = 
-00002490: 666c 6f61 7458 2876 616c 7565 2e73 6861  floatX(value.sha
-000024a0: 7065 5b2d 315d 290a 2020 2020 2020 2020  pe[-1]).        
-000024b0: 6e6f 726d 203d 202d 302e 3520 2a20 6b20  norm = -0.5 * k 
-000024c0: 2a20 706d 2e66 6c6f 6174 5828 6e70 2e6c  * pm.floatX(np.l
-000024d0: 6f67 2832 202a 206e 702e 7069 2929 0a20  og(2 * np.pi)). 
-000024e0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
-000024f0: 6563 6b5f 7061 7261 6d65 7465 7273 280a  eck_parameters(.
-00002500: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-00002510: 202d 2030 2e35 202a 2071 7561 6464 6973   - 0.5 * quaddis
-00002520: 7420 2d20 6c6f 6764 6574 2c0a 2020 2020  t - logdet,.    
-00002530: 2020 2020 2020 2020 6f6b 2c0a 2020 2020          ok,.    
-00002540: 2020 2020 2020 2020 6d73 673d 2270 6f73          msg="pos
-00002550: 6465 6622 2c0a 2020 2020 2020 2020 290a  def",.        ).
-00002560: 0a0a 636c 6173 7320 4d76 5374 7564 656e  ..class MvStuden
-00002570: 7454 5256 2852 616e 646f 6d56 6172 6961  tTRV(RandomVaria
-00002580: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
-00002590: 2022 6d75 6c74 6976 6172 6961 7465 5f73   "multivariate_s
-000025a0: 7475 6465 6e74 7422 0a20 2020 206e 6469  tudentt".    ndi
-000025b0: 6d5f 7375 7070 203d 2031 0a20 2020 206e  m_supp = 1.    n
-000025c0: 6469 6d73 5f70 6172 616d 7320 3d20 5b30  dims_params = [0
-000025d0: 2c20 312c 2032 5d0a 2020 2020 6474 7970  , 1, 2].    dtyp
-000025e0: 6520 3d20 2266 6c6f 6174 5822 0a20 2020  e = "floatX".   
-000025f0: 205f 7072 696e 745f 6e61 6d65 203d 2028   _print_name = (
-00002600: 224d 7653 7475 6465 6e74 5422 2c20 225c  "MvStudentT", "\
-00002610: 5c6f 7065 7261 746f 726e 616d 657b 4d76  \operatorname{Mv
-00002620: 5374 7564 656e 7454 7d22 290a 0a20 2020  StudentT}")..   
-00002630: 2064 6566 206d 616b 655f 6e6f 6465 2873   def make_node(s
-00002640: 656c 662c 2072 6e67 2c20 7369 7a65 2c20  elf, rng, size, 
-00002650: 6474 7970 652c 206e 752c 206d 752c 2063  dtype, nu, mu, c
-00002660: 6f76 293a 0a20 2020 2020 2020 206e 7520  ov):.        nu 
-00002670: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00002680: 6172 6961 626c 6528 6e75 290a 2020 2020  ariable(nu).    
-00002690: 2020 2020 6966 206e 6f74 206e 752e 6e64      if not nu.nd
-000026a0: 696d 203d 3d20 303a 0a20 2020 2020 2020  im == 0:.       
-000026b0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000026c0: 4572 726f 7228 226e 7520 6d75 7374 2062  Error("nu must b
-000026d0: 6520 6120 7363 616c 6172 2028 6e64 696d  e a scalar (ndim
-000026e0: 3d30 292e 2229 0a0a 2020 2020 2020 2020  =0).")..        
-000026f0: 7265 7475 726e 2073 7570 6572 2829 2e6d  return super().m
-00002700: 616b 655f 6e6f 6465 2872 6e67 2c20 7369  ake_node(rng, si
-00002710: 7a65 2c20 6474 7970 652c 206e 752c 206d  ze, dtype, nu, m
-00002720: 752c 2063 6f76 290a 0a20 2020 2064 6566  u, cov)..    def
-00002730: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-00002740: 6e75 2c20 6d75 3d4e 6f6e 652c 2063 6f76  nu, mu=None, cov
-00002750: 3d4e 6f6e 652c 2073 697a 653d 4e6f 6e65  =None, size=None
-00002760: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00002770: 2020 2020 2064 7479 7065 203d 2070 7974       dtype = pyt
-00002780: 656e 736f 722e 636f 6e66 6967 2e66 6c6f  ensor.config.flo
-00002790: 6174 5820 6966 2073 656c 662e 6474 7970  atX if self.dtyp
-000027a0: 6520 3d3d 2022 666c 6f61 7458 2220 656c  e == "floatX" el
-000027b0: 7365 2073 656c 662e 6474 7970 650a 0a20  se self.dtype.. 
-000027c0: 2020 2020 2020 2069 6620 6d75 2069 7320         if mu is 
-000027d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000027e0: 2020 6d75 203d 206e 702e 6172 7261 7928    mu = np.array(
-000027f0: 5b30 2e30 5d2c 2064 7479 7065 3d64 7479  [0.0], dtype=dty
-00002800: 7065 290a 2020 2020 2020 2020 6966 2063  pe).        if c
-00002810: 6f76 2069 7320 4e6f 6e65 3a0a 2020 2020  ov is None:.    
-00002820: 2020 2020 2020 2020 636f 7620 3d20 6e70          cov = np
-00002830: 2e61 7272 6179 285b 5b31 2e30 5d5d 2c20  .array([[1.0]], 
-00002840: 6474 7970 653d 6474 7970 6529 0a20 2020  dtype=dtype).   
-00002850: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00002860: 7228 292e 5f5f 6361 6c6c 5f5f 286e 752c  r().__call__(nu,
-00002870: 206d 752c 2063 6f76 2c20 7369 7a65 3d73   mu, cov, size=s
-00002880: 697a 652c 202a 2a6b 7761 7267 7329 0a0a  ize, **kwargs)..
-00002890: 2020 2020 6465 6620 5f73 7570 705f 7368      def _supp_sh
-000028a0: 6170 655f 6672 6f6d 5f70 6172 616d 7328  ape_from_params(
-000028b0: 7365 6c66 2c20 6469 7374 5f70 6172 616d  self, dist_param
-000028c0: 732c 2072 6570 5f70 6172 616d 5f69 6478  s, rep_param_idx
-000028d0: 3d31 2c20 7061 7261 6d5f 7368 6170 6573  =1, param_shapes
-000028e0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-000028f0: 7265 7475 726e 2064 6566 6175 6c74 5f73  return default_s
-00002900: 7570 705f 7368 6170 655f 6672 6f6d 5f70  upp_shape_from_p
-00002910: 6172 616d 7328 0a20 2020 2020 2020 2020  arams(.         
-00002920: 2020 2073 656c 662e 6e64 696d 5f73 7570     self.ndim_sup
-00002930: 702c 2064 6973 745f 7061 7261 6d73 2c20  p, dist_params, 
-00002940: 7265 705f 7061 7261 6d5f 6964 782c 2070  rep_param_idx, p
-00002950: 6172 616d 5f73 6861 7065 730a 2020 2020  aram_shapes.    
-00002960: 2020 2020 290a 0a20 2020 2040 636c 6173      )..    @clas
-00002970: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00002980: 726e 675f 666e 2863 6c73 2c20 726e 672c  rng_fn(cls, rng,
-00002990: 206e 752c 206d 752c 2063 6f76 2c20 7369   nu, mu, cov, si
-000029a0: 7a65 293a 0a20 2020 2020 2020 206d 765f  ze):.        mv_
-000029b0: 7361 6d70 6c65 7320 3d20 6d75 6c74 6976  samples = multiv
-000029c0: 6172 6961 7465 5f6e 6f72 6d61 6c2e 726e  ariate_normal.rn
-000029d0: 675f 666e 2872 6e67 3d72 6e67 2c20 6d65  g_fn(rng=rng, me
-000029e0: 616e 3d6e 702e 7a65 726f 735f 6c69 6b65  an=np.zeros_like
-000029f0: 286d 7529 2c20 636f 763d 636f 762c 2073  (mu), cov=cov, s
-00002a00: 697a 653d 7369 7a65 290a 0a20 2020 2020  ize=size)..     
-00002a10: 2020 2023 2054 616b 6520 6368 6932 2064     # Take chi2 d
-00002a20: 7261 7773 2061 6e64 2061 6464 2061 6e20  raws and add an 
-00002a30: 6178 6973 206f 6620 6c65 6e67 7468 2031  axis of length 1
-00002a40: 2074 6f20 7468 6520 7269 6768 7420 666f   to the right fo
-00002a50: 7220 636f 7272 6563 7420 6272 6f61 6463  r correct broadc
-00002a60: 6173 7469 6e67 2062 656c 6f77 0a20 2020  asting below.   
-00002a70: 2020 2020 2063 6869 325f 7361 6d70 6c65       chi2_sample
-00002a80: 7320 3d20 6e70 2e73 7172 7428 726e 672e  s = np.sqrt(rng.
-00002a90: 6368 6973 7175 6172 6528 6e75 2c20 7369  chisquare(nu, si
-00002aa0: 7a65 3d73 697a 6529 202f 206e 7529 5b2e  ze=size) / nu)[.
-00002ab0: 2e2e 2c20 4e6f 6e65 5d0a 0a20 2020 2020  .., None]..     
-00002ac0: 2020 2069 6620 7369 7a65 3a0a 2020 2020     if size:.    
-00002ad0: 2020 2020 2020 2020 6d75 203d 206e 702e          mu = np.
-00002ae0: 6272 6f61 6463 6173 745f 746f 286d 752c  broadcast_to(mu,
-00002af0: 2073 697a 6520 2b20 286d 752e 7368 6170   size + (mu.shap
-00002b00: 655b 2d31 5d2c 2929 0a0a 2020 2020 2020  e[-1],))..      
-00002b10: 2020 7265 7475 726e 2028 6d76 5f73 616d    return (mv_sam
-00002b20: 706c 6573 202f 2063 6869 325f 7361 6d70  ples / chi2_samp
-00002b30: 6c65 7329 202b 206d 750a 0a0a 6d76 5f73  les) + mu...mv_s
-00002b40: 7475 6465 6e74 7420 3d20 4d76 5374 7564  tudentt = MvStud
-00002b50: 656e 7454 5256 2829 0a0a 0a63 6c61 7373  entTRV()...class
-00002b60: 204d 7653 7475 6465 6e74 5428 436f 6e74   MvStudentT(Cont
-00002b70: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
-00002b80: 220a 2020 2020 4d75 6c74 6976 6172 6961  ".    Multivaria
-00002b90: 7465 2053 7475 6465 6e74 2d54 206c 6f67  te Student-T log
-00002ba0: 2d6c 696b 656c 6968 6f6f 642e 0a0a 2020  -likelihood...  
-00002bb0: 2020 2e2e 206d 6174 683a 3a0a 2020 2020    .. math::.    
-00002bc0: 2020 2020 6628 5c6d 6174 6862 667b 787d      f(\mathbf{x}
-00002bd0: 7c20 5c6e 752c 5c6d 752c 5c53 6967 6d61  | \nu,\mu,\Sigma
-00002be0: 2920 3d0a 2020 2020 2020 2020 5c66 7261  ) =.        \fra
-00002bf0: 630a 2020 2020 2020 2020 2020 2020 7b5c  c.            {\
-00002c00: 4761 6d6d 615c 6c65 6674 5b28 5c6e 752b  Gamma\left[(\nu+
-00002c10: 7029 2f32 5c72 6967 6874 5d7d 0a20 2020  p)/2\right]}.   
-00002c20: 2020 2020 2020 2020 207b 5c47 616d 6d61           {\Gamma
-00002c30: 285c 6e75 2f32 295c 6e75 5e7b 702f 327d  (\nu/2)\nu^{p/2}
-00002c40: 5c70 695e 7b70 2f32 7d0a 2020 2020 2020  \pi^{p/2}.      
-00002c50: 2020 2020 2020 205c 6c65 6674 7c7b 5c53         \left|{\S
-00002c60: 6967 6d61 7d5c 7269 6768 747c 5e7b 312f  igma}\right|^{1/
-00002c70: 327d 0a20 2020 2020 2020 2020 2020 2020  2}.             
-00002c80: 5c6c 6566 745b 0a20 2020 2020 2020 2020  \left[.         
-00002c90: 2020 2020 2020 312b 5c66 7261 637b 317d        1+\frac{1}
-00002ca0: 7b5c 6e75 7d0a 2020 2020 2020 2020 2020  {\nu}.          
-00002cb0: 2020 2020 2028 7b5c 6d61 7468 6266 2078       ({\mathbf x
-00002cc0: 7d2d 7b5c 6d75 7d29 5e54 0a20 2020 2020  }-{\mu})^T.     
-00002cd0: 2020 2020 2020 2020 2020 7b5c 5369 676d            {\Sigm
-00002ce0: 617d 5e7b 2d31 7d28 7b5c 6d61 7468 6266  a}^{-1}({\mathbf
-00002cf0: 2078 7d2d 7b5c 6d75 7d29 0a20 2020 2020   x}-{\mu}).     
-00002d00: 2020 2020 2020 2020 5c72 6967 6874 5d5e          \right]^
-00002d10: 7b2d 285c 6e75 2b70 292f 327d 7d0a 0a20  {-(\nu+p)/2}}.. 
-00002d20: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
-00002d30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002d40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002d50: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
-00002d60: 7570 706f 7274 2020 203a 6d61 7468 3a60  upport   :math:`
-00002d70: 7820 5c69 6e20 5c6d 6174 6862 627b 527d  x \in \mathbb{R}
-00002d80: 5e70 600a 2020 2020 4d65 616e 2020 2020  ^p`.    Mean    
-00002d90: 2020 3a6d 6174 683a 605c 6d75 6020 6966    :math:`\mu` if
-00002da0: 203a 6d61 7468 3a60 5c6e 7520 3e20 3160   :math:`\nu > 1`
-00002db0: 2065 6c73 6520 756e 6465 6669 6e65 640a   else undefined.
-00002dc0: 2020 2020 5661 7269 616e 6365 2020 3a6d      Variance  :m
-00002dd0: 6174 683a 605c 6672 6163 7b5c 6e75 7d7b  ath:`\frac{\nu}{
-00002de0: 5c6d 752d 327d 5c53 6967 6d61 600a 2020  \mu-2}\Sigma`.  
-00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e00: 6966 203a 6d61 7468 3a60 5c6e 753e 3260  if :math:`\nu>2`
-00002e10: 2065 6c73 6520 756e 6465 6669 6e65 640a   else undefined.
-00002e20: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
-00002e30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020  ===========..   
-00002e60: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00002e70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
-00002e80: 7520 3a20 7465 6e73 6f72 5f6c 696b 6520  u : tensor_like 
-00002e90: 6f66 2066 6c6f 6174 0a20 2020 2020 2020  of float.       
-00002ea0: 2044 6567 7265 6573 206f 6620 6672 6565   Degrees of free
-00002eb0: 646f 6d2c 2073 686f 756c 6420 6265 2061  dom, should be a
-00002ec0: 2070 6f73 6974 6976 6520 7363 616c 6172   positive scalar
-00002ed0: 2e0a 2020 2020 5369 676d 6120 3a20 7465  ..    Sigma : te
-00002ee0: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
-00002ef0: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
-00002f00: 2020 2020 2053 6361 6c65 206d 6174 7269       Scale matri
-00002f10: 782e 2055 7365 2060 7363 616c 6560 2069  x. Use `scale` i
-00002f20: 6e20 6e65 7720 636f 6465 2e0a 2020 2020  n new code..    
-00002f30: 6d75 203a 2074 656e 736f 725f 6c69 6b65  mu : tensor_like
-00002f40: 206f 6620 666c 6f61 742c 206f 7074 696f   of float, optio
-00002f50: 6e61 6c0a 2020 2020 2020 2020 5665 6374  nal.        Vect
-00002f60: 6f72 206f 6620 6d65 616e 732e 0a20 2020  or of means..   
-00002f70: 2073 6361 6c65 203a 2074 656e 736f 725f   scale : tensor_
-00002f80: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
-00002f90: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00002fa0: 5468 6520 7363 616c 6520 6d61 7472 6978  The scale matrix
-00002fb0: 2e0a 2020 2020 7461 7520 3a20 7465 6e73  ..    tau : tens
-00002fc0: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-00002fd0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00002fe0: 2020 2054 6865 2070 7265 6369 7369 6f6e     The precision
-00002ff0: 206d 6174 7269 782e 0a20 2020 2063 686f   matrix..    cho
-00003000: 6c20 3a20 7465 6e73 6f72 5f6c 696b 6520  l : tensor_like 
+000004d0: 6d56 6172 6961 626c 650a 6672 6f6d 2070  mVariable.from p
+000004e0: 7974 656e 736f 722e 7465 6e73 6f72 2e72  ytensor.tensor.r
+000004f0: 616e 646f 6d2e 7574 696c 7320 696d 706f  andom.utils impo
+00000500: 7274 2028 0a20 2020 2062 726f 6164 6361  rt (.    broadca
+00000510: 7374 5f70 6172 616d 732c 0a20 2020 2073  st_params,.    s
+00000520: 7570 705f 7368 6170 655f 6672 6f6d 5f72  upp_shape_from_r
+00000530: 6566 5f70 6172 616d 5f73 6861 7065 2c0a  ef_param_shape,.
+00000540: 290a 6672 6f6d 2070 7974 656e 736f 722e  ).from pytensor.
+00000550: 7465 6e73 6f72 2e73 6c69 6e61 6c67 2069  tensor.slinalg i
+00000560: 6d70 6f72 7420 4368 6f6c 6573 6b79 2c20  mport Cholesky, 
+00000570: 536f 6c76 6554 7269 616e 6775 6c61 720a  SolveTriangular.
+00000580: 6672 6f6d 2070 7974 656e 736f 722e 7465  from pytensor.te
+00000590: 6e73 6f72 2e74 7970 6520 696d 706f 7274  nsor.type import
+000005a0: 2054 656e 736f 7254 7970 650a 6672 6f6d   TensorType.from
+000005b0: 2073 6369 7079 2069 6d70 6f72 7420 6c69   scipy import li
+000005c0: 6e61 6c67 2c20 7374 6174 730a 0a69 6d70  nalg, stats..imp
+000005d0: 6f72 7420 7079 6d63 2061 7320 706d 0a0a  ort pymc as pm..
+000005e0: 6672 6f6d 2070 796d 632e 6469 7374 7269  from pymc.distri
+000005f0: 6275 7469 6f6e 7320 696d 706f 7274 2074  butions import t
+00000600: 7261 6e73 666f 726d 730a 6672 6f6d 2070  ransforms.from p
+00000610: 796d 632e 6469 7374 7269 6275 7469 6f6e  ymc.distribution
+00000620: 732e 636f 6e74 696e 756f 7573 2069 6d70  s.continuous imp
+00000630: 6f72 7420 426f 756e 6465 6443 6f6e 7469  ort BoundedConti
+00000640: 6e75 6f75 732c 2043 6869 5371 7561 7265  nuous, ChiSquare
+00000650: 642c 204e 6f72 6d61 6c0a 6672 6f6d 2070  d, Normal.from p
+00000660: 796d 632e 6469 7374 7269 6275 7469 6f6e  ymc.distribution
+00000670: 732e 6469 7374 5f6d 6174 6820 696d 706f  s.dist_math impo
+00000680: 7274 2028 0a20 2020 2062 6574 616c 6e2c  rt (.    betaln,
+00000690: 0a20 2020 2063 6865 636b 5f70 6172 616d  .    check_param
+000006a0: 6574 6572 732c 0a20 2020 2066 6163 746c  eters,.    factl
+000006b0: 6e2c 0a20 2020 206c 6f67 706f 772c 0a20  n,.    logpow,. 
+000006c0: 2020 206d 756c 7469 6761 6d6d 616c 6e2c     multigammaln,
+000006d0: 0a29 0a66 726f 6d20 7079 6d63 2e64 6973  .).from pymc.dis
+000006e0: 7472 6962 7574 696f 6e73 2e64 6973 7472  tributions.distr
+000006f0: 6962 7574 696f 6e20 696d 706f 7274 2028  ibution import (
+00000700: 0a20 2020 2043 6f6e 7469 6e75 6f75 732c  .    Continuous,
+00000710: 0a20 2020 2044 6973 6372 6574 652c 0a20  .    Discrete,. 
+00000720: 2020 2044 6973 7472 6962 7574 696f 6e2c     Distribution,
+00000730: 0a20 2020 2053 796d 626f 6c69 6352 616e  .    SymbolicRan
+00000740: 646f 6d56 6172 6961 626c 652c 0a20 2020  domVariable,.   
+00000750: 205f 6d6f 6d65 6e74 2c0a 2020 2020 6d6f   _moment,.    mo
+00000760: 6d65 6e74 2c0a 290a 6672 6f6d 2070 796d  ment,.).from pym
+00000770: 632e 6469 7374 7269 6275 7469 6f6e 732e  c.distributions.
+00000780: 7368 6170 655f 7574 696c 7320 696d 706f  shape_utils impo
+00000790: 7274 2028 0a20 2020 205f 6368 616e 6765  rt (.    _change
+000007a0: 5f64 6973 745f 7369 7a65 2c0a 2020 2020  _dist_size,.    
+000007b0: 6272 6f61 6463 6173 745f 6469 7374 5f73  broadcast_dist_s
+000007c0: 616d 706c 6573 5f73 6861 7065 2c0a 2020  amples_shape,.  
+000007d0: 2020 6368 616e 6765 5f64 6973 745f 7369    change_dist_si
+000007e0: 7a65 2c0a 2020 2020 6765 745f 7375 7070  ze,.    get_supp
+000007f0: 6f72 745f 7368 6170 652c 0a20 2020 2072  ort_shape,.    r
+00000800: 765f 7369 7a65 5f69 735f 6e6f 6e65 2c0a  v_size_is_none,.
+00000810: 2020 2020 746f 5f74 7570 6c65 2c0a 290a      to_tuple,.).
+00000820: 6672 6f6d 2070 796d 632e 6469 7374 7269  from pymc.distri
+00000830: 6275 7469 6f6e 732e 7472 616e 7366 6f72  butions.transfor
+00000840: 6d73 2069 6d70 6f72 7420 496e 7465 7276  ms import Interv
+00000850: 616c 2c20 5a65 726f 5375 6d54 7261 6e73  al, ZeroSumTrans
+00000860: 666f 726d 2c20 5f64 6566 6175 6c74 5f74  form, _default_t
+00000870: 7261 6e73 666f 726d 0a66 726f 6d20 7079  ransform.from py
+00000880: 6d63 2e6c 6f67 7072 6f62 2e61 6273 7472  mc.logprob.abstr
+00000890: 6163 7420 696d 706f 7274 205f 6c6f 6770  act import _logp
+000008a0: 726f 620a 6672 6f6d 2070 796d 632e 6d61  rob.from pymc.ma
+000008b0: 7468 2069 6d70 6f72 7420 6b72 6f6e 5f64  th import kron_d
+000008c0: 6961 672c 206b 726f 6e5f 646f 740a 6672  iag, kron_dot.fr
+000008d0: 6f6d 2070 796d 632e 7079 7465 6e73 6f72  om pymc.pytensor
+000008e0: 6620 696d 706f 7274 2066 6c6f 6174 582c  f import floatX,
+000008f0: 2069 6e74 580a 6672 6f6d 2070 796d 632e   intX.from pymc.
+00000900: 7574 696c 2069 6d70 6f72 7420 6368 6563  util import chec
+00000910: 6b5f 6469 7374 5f6e 6f74 5f72 6567 6973  k_dist_not_regis
+00000920: 7465 7265 640a 0a5f 5f61 6c6c 5f5f 203d  tered..__all__ =
+00000930: 205b 0a20 2020 2022 4d76 4e6f 726d 616c   [.    "MvNormal
+00000940: 222c 0a20 2020 2022 5a65 726f 5375 6d4e  ",.    "ZeroSumN
+00000950: 6f72 6d61 6c22 2c0a 2020 2020 224d 7653  ormal",.    "MvS
+00000960: 7475 6465 6e74 5422 2c0a 2020 2020 2244  tudentT",.    "D
+00000970: 6972 6963 686c 6574 222c 0a20 2020 2022  irichlet",.    "
+00000980: 4d75 6c74 696e 6f6d 6961 6c22 2c0a 2020  Multinomial",.  
+00000990: 2020 2244 6972 6963 686c 6574 4d75 6c74    "DirichletMult
+000009a0: 696e 6f6d 6961 6c22 2c0a 2020 2020 224f  inomial",.    "O
+000009b0: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
+000009c0: 6c22 2c0a 2020 2020 2257 6973 6861 7274  l",.    "Wishart
+000009d0: 222c 0a20 2020 2022 5769 7368 6172 7442  ",.    "WishartB
+000009e0: 6172 746c 6574 7422 2c0a 2020 2020 224c  artlett",.    "L
+000009f0: 4b4a 436f 7272 222c 0a20 2020 2022 4c4b  KJCorr",.    "LK
+00000a00: 4a43 686f 6c65 736b 7943 6f76 222c 0a20  JCholeskyCov",. 
+00000a10: 2020 2022 4d61 7472 6978 4e6f 726d 616c     "MatrixNormal
+00000a20: 222c 0a20 2020 2022 4b72 6f6e 6563 6b65  ",.    "Kronecke
+00000a30: 724e 6f72 6d61 6c22 2c0a 2020 2020 2243  rNormal",.    "C
+00000a40: 4152 222c 0a20 2020 2022 5374 6963 6b42  AR",.    "StickB
+00000a50: 7265 616b 696e 6757 6569 6768 7473 222c  reakingWeights",
+00000a60: 0a5d 0a0a 736f 6c76 655f 6c6f 7765 7220  .]..solve_lower 
+00000a70: 3d20 536f 6c76 6554 7269 616e 6775 6c61  = SolveTriangula
+00000a80: 7228 6c6f 7765 723d 5472 7565 290a 736f  r(lower=True).so
+00000a90: 6c76 655f 7570 7065 7220 3d20 536f 6c76  lve_upper = Solv
+00000aa0: 6554 7269 616e 6775 6c61 7228 6c6f 7765  eTriangular(lowe
+00000ab0: 723d 4661 6c73 6529 0a0a 0a63 6c61 7373  r=False)...class
+00000ac0: 2053 696d 706c 6578 436f 6e74 696e 756f   SimplexContinuo
+00000ad0: 7573 2843 6f6e 7469 6e75 6f75 7329 3a0a  us(Continuous):.
+00000ae0: 2020 2020 2222 2242 6173 6520 636c 6173      """Base clas
+00000af0: 7320 666f 7220 7369 6d70 6c65 7820 636f  s for simplex co
+00000b00: 6e74 696e 756f 7573 2064 6973 7472 6962  ntinuous distrib
+00000b10: 7574 696f 6e73 2222 220a 0a0a 405f 6465  utions"""...@_de
+00000b20: 6661 756c 745f 7472 616e 7366 6f72 6d2e  fault_transform.
+00000b30: 7265 6769 7374 6572 2853 696d 706c 6578  register(Simplex
+00000b40: 436f 6e74 696e 756f 7573 290a 6465 6620  Continuous).def 
+00000b50: 7369 6d70 6c65 785f 636f 6e74 5f74 7261  simplex_cont_tra
+00000b60: 6e73 666f 726d 286f 702c 2072 7629 3a0a  nsform(op, rv):.
+00000b70: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
+00000b80: 666f 726d 732e 7369 6d70 6c65 780a 0a0a  forms.simplex...
+00000b90: 2320 5374 6570 206d 6574 686f 6473 2061  # Step methods a
+00000ba0: 6e64 2061 6476 6920 646f 206e 6f74 2063  nd advi do not c
+00000bb0: 6174 6368 204c 696e 416c 6745 7272 6f72  atch LinAlgError
+00000bc0: 7320 6174 2074 6865 0a23 206d 6f6d 656e  s at the.# momen
+00000bd0: 742e 2057 6520 776f 726b 2061 726f 756e  t. We work aroun
+00000be0: 6420 7468 6174 2062 7920 7573 696e 6720  d that by using 
+00000bf0: 6120 6368 6f6c 6573 6b79 206f 700a 2320  a cholesky op.# 
+00000c00: 7468 6174 2072 6574 7572 6e73 2061 206e  that returns a n
+00000c10: 616e 2061 7320 6669 7273 7420 656e 7472  an as first entr
+00000c20: 7920 696e 7374 6561 6420 6f66 2072 6169  y instead of rai
+00000c30: 7369 6e67 0a23 2061 6e20 6572 726f 722e  sing.# an error.
+00000c40: 0a63 686f 6c65 736b 7920 3d20 4368 6f6c  .cholesky = Chol
+00000c50: 6573 6b79 286c 6f77 6572 3d54 7275 652c  esky(lower=True,
+00000c60: 206f 6e5f 6572 726f 723d 226e 616e 2229   on_error="nan")
+00000c70: 0a0a 0a64 6566 2071 7561 6464 6973 745f  ...def quaddist_
+00000c80: 6d61 7472 6978 2863 6f76 3d4e 6f6e 652c  matrix(cov=None,
+00000c90: 2063 686f 6c3d 4e6f 6e65 2c20 7461 753d   chol=None, tau=
+00000ca0: 4e6f 6e65 2c20 6c6f 7765 723d 5472 7565  None, lower=True
+00000cb0: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00000cc0: 7329 3a0a 2020 2020 6966 2063 686f 6c20  s):.    if chol 
+00000cd0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00000ce0: 6e6f 7420 6c6f 7765 723a 0a20 2020 2020  not lower:.     
+00000cf0: 2020 2063 686f 6c20 3d20 6368 6f6c 2e54     chol = chol.T
+00000d00: 0a0a 2020 2020 6966 206c 656e 285b 6920  ..    if len([i 
+00000d10: 666f 7220 6920 696e 205b 7461 752c 2063  for i in [tau, c
+00000d20: 6f76 2c20 6368 6f6c 5d20 6966 2069 2069  ov, chol] if i i
+00000d30: 7320 6e6f 7420 4e6f 6e65 5d29 2021 3d20  s not None]) != 
+00000d40: 313a 0a20 2020 2020 2020 2072 6169 7365  1:.        raise
+00000d50: 2056 616c 7565 4572 726f 7228 2249 6e63   ValueError("Inc
+00000d60: 6f6d 7061 7469 626c 6520 7061 7261 6d65  ompatible parame
+00000d70: 7465 7269 7a61 7469 6f6e 2e20 5370 6563  terization. Spec
+00000d80: 6966 7920 6578 6163 746c 7920 6f6e 6520  ify exactly one 
+00000d90: 6f66 2074 6175 2c20 636f 762c 206f 7220  of tau, cov, or 
+00000da0: 6368 6f6c 2e22 290a 0a20 2020 2069 6620  chol.")..    if 
+00000db0: 636f 7620 6973 206e 6f74 204e 6f6e 653a  cov is not None:
+00000dc0: 0a20 2020 2020 2020 2063 6f76 203d 2070  .        cov = p
+00000dd0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00000de0: 6162 6c65 2863 6f76 290a 2020 2020 2020  able(cov).      
+00000df0: 2020 6966 2063 6f76 2e6e 6469 6d20 213d    if cov.ndim !=
+00000e00: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00000e10: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00000e20: 2822 636f 7620 6d75 7374 2062 6520 7477  ("cov must be tw
+00000e30: 6f20 6469 6d65 6e73 696f 6e61 6c2e 2229  o dimensional.")
+00000e40: 0a20 2020 2065 6c69 6620 7461 7520 6973  .    elif tau is
+00000e50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00000e60: 2020 2074 6175 203d 2070 742e 6173 5f74     tau = pt.as_t
+00000e70: 656e 736f 725f 7661 7269 6162 6c65 2874  ensor_variable(t
+00000e80: 6175 290a 2020 2020 2020 2020 6966 2074  au).        if t
+00000e90: 6175 2e6e 6469 6d20 213d 2032 3a0a 2020  au.ndim != 2:.  
+00000ea0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00000eb0: 5661 6c75 6545 7272 6f72 2822 7461 7520  ValueError("tau 
+00000ec0: 6d75 7374 2062 6520 7477 6f20 6469 6d65  must be two dime
+00000ed0: 6e73 696f 6e61 6c2e 2229 0a20 2020 2020  nsional.").     
+00000ee0: 2020 2023 2054 4f44 4f3a 2057 6861 7427     # TODO: What'
+00000ef0: 7320 7468 6520 636f 7272 6563 7420 6f72  s the correct or
+00000f00: 6465 722f 6170 7072 6f61 6368 2028 696e  der/approach (in
+00000f10: 2074 6865 206e 6f6e 2d73 7175 6172 6520   the non-square 
+00000f20: 6361 7365 293f 0a20 2020 2020 2020 2023  case)?.        #
+00000f30: 2060 7079 7465 6e73 6f72 2e74 656e 736f   `pytensor.tenso
+00000f40: 722e 6e6c 696e 616c 672e 7465 6e73 6f72  r.nlinalg.tensor
+00000f50: 696e 7660 3f0a 2020 2020 2020 2020 636f  inv`?.        co
+00000f60: 7620 3d20 6d61 7472 6978 5f69 6e76 6572  v = matrix_inver
+00000f70: 7365 2874 6175 290a 2020 2020 656c 7365  se(tau).    else
+00000f80: 3a0a 2020 2020 2020 2020 2320 544f 444f  :.        # TODO
+00000f90: 3a20 5768 6174 2773 2074 6865 2063 6f72  : What's the cor
+00000fa0: 7265 6374 206f 7264 6572 2f61 7070 726f  rect order/appro
+00000fb0: 6163 6820 2869 6e20 7468 6520 6e6f 6e2d  ach (in the non-
+00000fc0: 7371 7561 7265 2063 6173 6529 3f0a 2020  square case)?.  
+00000fd0: 2020 2020 2020 6368 6f6c 203d 2070 742e        chol = pt.
+00000fe0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+00000ff0: 6c65 2863 686f 6c29 0a20 2020 2020 2020  le(chol).       
+00001000: 2069 6620 6368 6f6c 2e6e 6469 6d20 213d   if chol.ndim !=
+00001010: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00001020: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00001030: 2822 6368 6f6c 206d 7573 7420 6265 2074  ("chol must be t
+00001040: 776f 2064 696d 656e 7369 6f6e 616c 2e22  wo dimensional."
+00001050: 290a 0a20 2020 2020 2020 2023 2074 6167  )..        # tag
+00001060: 2061 7320 6c6f 7765 7220 7472 6961 6e67   as lower triang
+00001070: 756c 6172 2074 6f20 656e 6162 6c65 2070  ular to enable p
+00001080: 7974 656e 736f 7220 7265 7772 6974 6573  ytensor rewrites
+00001090: 206f 6620 6368 6f6c 286c 2e6c 2729 202d   of chol(l.l') -
+000010a0: 3e20 6c0a 2020 2020 2020 2020 6368 6f6c  > l.        chol
+000010b0: 2e74 6167 2e6c 6f77 6572 5f74 7269 616e  .tag.lower_trian
+000010c0: 6775 6c61 7220 3d20 5472 7565 0a20 2020  gular = True.   
+000010d0: 2020 2020 2063 6f76 203d 2063 686f 6c2e       cov = chol.
+000010e0: 646f 7428 6368 6f6c 2e54 290a 0a20 2020  dot(chol.T)..   
+000010f0: 2072 6574 7572 6e20 636f 760a 0a0a 6465   return cov...de
+00001100: 6620 7175 6164 6469 7374 5f70 6172 7365  f quaddist_parse
+00001110: 2876 616c 7565 2c20 6d75 2c20 636f 762c  (value, mu, cov,
+00001120: 206d 6174 5f74 7970 653d 2263 6f76 2229   mat_type="cov")
+00001130: 3a0a 2020 2020 2222 2243 6f6d 7075 7465  :.    """Compute
+00001140: 2028 7820 2d20 6d75 292e 5420 4020 5369   (x - mu).T @ Si
+00001150: 676d 615e 2d31 2040 2028 7820 2d20 6d75  gma^-1 @ (x - mu
+00001160: 2920 616e 6420 7468 6520 6c6f 6764 6574  ) and the logdet
+00001170: 206f 6620 5369 676d 612e 2222 220a 2020   of Sigma.""".  
+00001180: 2020 6966 2076 616c 7565 2e6e 6469 6d20    if value.ndim 
+00001190: 3e20 3220 6f72 2076 616c 7565 2e6e 6469  > 2 or value.ndi
+000011a0: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
+000011b0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000011c0: 2822 496e 7661 6c69 6420 6469 6d65 6e73  ("Invalid dimens
+000011d0: 696f 6e20 666f 7220 7661 6c75 653a 2025  ion for value: %
+000011e0: 7322 2025 2076 616c 7565 2e6e 6469 6d29  s" % value.ndim)
+000011f0: 0a20 2020 2069 6620 7661 6c75 652e 6e64  .    if value.nd
+00001200: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+00001210: 206f 6e65 6469 6d20 3d20 5472 7565 0a20   onedim = True. 
+00001220: 2020 2020 2020 2076 616c 7565 203d 2076         value = v
+00001230: 616c 7565 5b4e 6f6e 652c 203a 5d0a 2020  alue[None, :].  
+00001240: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001250: 6f6e 6564 696d 203d 2046 616c 7365 0a0a  onedim = False..
+00001260: 2020 2020 6465 6c74 6120 3d20 7661 6c75      delta = valu
+00001270: 6520 2d20 6d75 0a20 2020 2023 2055 7365  e - mu.    # Use
+00001280: 2074 6869 7320 7768 656e 2054 6865 616e   this when Thean
+00001290: 6f23 3539 3038 2069 7320 7265 6c65 6173  o#5908 is releas
+000012a0: 6564 2e0a 2020 2020 2320 7265 7475 726e  ed..    # return
+000012b0: 204d 764e 6f72 6d61 6c4c 6f67 7028 2928   MvNormalLogp()(
+000012c0: 7365 6c66 2e63 6f76 2c20 6465 6c74 6129  self.cov, delta)
+000012d0: 0a20 2020 2063 686f 6c5f 636f 7620 3d20  .    chol_cov = 
+000012e0: 6368 6f6c 6573 6b79 2863 6f76 290a 2020  cholesky(cov).  
+000012f0: 2020 6966 206d 6174 5f74 7970 6520 213d    if mat_type !=
+00001300: 2022 7461 7522 3a0a 2020 2020 2020 2020   "tau":.        
+00001310: 6469 7374 2c20 6c6f 6764 6574 2c20 6f6b  dist, logdet, ok
+00001320: 203d 2071 7561 6464 6973 745f 6368 6f6c   = quaddist_chol
+00001330: 2864 656c 7461 2c20 6368 6f6c 5f63 6f76  (delta, chol_cov
+00001340: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00001350: 2020 2020 6469 7374 2c20 6c6f 6764 6574      dist, logdet
+00001360: 2c20 6f6b 203d 2071 7561 6464 6973 745f  , ok = quaddist_
+00001370: 7461 7528 6465 6c74 612c 2063 686f 6c5f  tau(delta, chol_
+00001380: 636f 7629 0a20 2020 2069 6620 6f6e 6564  cov).    if oned
+00001390: 696d 3a0a 2020 2020 2020 2020 7265 7475  im:.        retu
+000013a0: 726e 2064 6973 745b 305d 2c20 6c6f 6764  rn dist[0], logd
+000013b0: 6574 2c20 6f6b 0a0a 2020 2020 7265 7475  et, ok..    retu
+000013c0: 726e 2064 6973 742c 206c 6f67 6465 742c  rn dist, logdet,
+000013d0: 206f 6b0a 0a0a 6465 6620 7175 6164 6469   ok...def quaddi
+000013e0: 7374 5f63 686f 6c28 6465 6c74 612c 2063  st_chol(delta, c
+000013f0: 686f 6c5f 6d61 7429 3a0a 2020 2020 6469  hol_mat):.    di
+00001400: 6167 203d 2070 742e 6469 6167 2863 686f  ag = pt.diag(cho
+00001410: 6c5f 6d61 7429 0a20 2020 2023 2043 6865  l_mat).    # Che
+00001420: 636b 2069 6620 7468 6520 636f 7661 7269  ck if the covari
+00001430: 616e 6365 206d 6174 7269 7820 6973 2070  ance matrix is p
+00001440: 6f73 6974 6976 6520 6465 6669 6e69 7465  ositive definite
+00001450: 2e0a 2020 2020 6f6b 203d 2070 742e 616c  ..    ok = pt.al
+00001460: 6c28 6469 6167 203e 2030 290a 2020 2020  l(diag > 0).    
+00001470: 2320 4966 206e 6f74 2c20 7265 706c 6163  # If not, replac
+00001480: 6520 7468 6520 6469 6167 6f6e 616c 2e20  e the diagonal. 
+00001490: 5765 2072 6574 7572 6e20 2d69 6e66 206c  We return -inf l
+000014a0: 6174 6572 2c20 6275 740a 2020 2020 2320  ater, but.    # 
+000014b0: 6e65 6564 2074 6f20 7072 6576 656e 7420  need to prevent 
+000014c0: 736f 6c76 655f 6c6f 7765 7220 6672 6f6d  solve_lower from
+000014d0: 2074 6872 6f77 696e 6720 616e 2065 7863   throwing an exc
+000014e0: 6570 7469 6f6e 2e0a 2020 2020 6368 6f6c  eption..    chol
+000014f0: 5f63 6f76 203d 2070 742e 7377 6974 6368  _cov = pt.switch
+00001500: 286f 6b2c 2063 686f 6c5f 6d61 742c 2031  (ok, chol_mat, 1
+00001510: 290a 0a20 2020 2064 656c 7461 5f74 7261  )..    delta_tra
+00001520: 6e73 203d 2073 6f6c 7665 5f6c 6f77 6572  ns = solve_lower
+00001530: 2863 686f 6c5f 636f 762c 2064 656c 7461  (chol_cov, delta
+00001540: 2e54 292e 540a 2020 2020 7175 6164 6469  .T).T.    quaddi
+00001550: 7374 203d 2028 6465 6c74 615f 7472 616e  st = (delta_tran
+00001560: 732a 2a32 292e 7375 6d28 6178 6973 3d2d  s**2).sum(axis=-
+00001570: 3129 0a20 2020 206c 6f67 6465 7420 3d20  1).    logdet = 
+00001580: 7074 2e73 756d 2870 742e 6c6f 6728 6469  pt.sum(pt.log(di
+00001590: 6167 2929 0a20 2020 2072 6574 7572 6e20  ag)).    return 
+000015a0: 7175 6164 6469 7374 2c20 6c6f 6764 6574  quaddist, logdet
+000015b0: 2c20 6f6b 0a0a 0a64 6566 2071 7561 6464  , ok...def quadd
+000015c0: 6973 745f 7461 7528 6465 6c74 612c 2063  ist_tau(delta, c
+000015d0: 686f 6c5f 6d61 7429 3a0a 2020 2020 6469  hol_mat):.    di
+000015e0: 6167 203d 2070 742e 6e6c 696e 616c 672e  ag = pt.nlinalg.
+000015f0: 6469 6167 2863 686f 6c5f 6d61 7429 0a20  diag(chol_mat). 
+00001600: 2020 2023 2043 6865 636b 2069 6620 7468     # Check if th
+00001610: 6520 7072 6563 6973 696f 6e20 6d61 7472  e precision matr
+00001620: 6978 2069 7320 706f 7369 7469 7665 2064  ix is positive d
+00001630: 6566 696e 6974 652e 0a20 2020 206f 6b20  efinite..    ok 
+00001640: 3d20 7074 2e61 6c6c 2864 6961 6720 3e20  = pt.all(diag > 
+00001650: 3029 0a20 2020 2023 2049 6620 6e6f 742c  0).    # If not,
+00001660: 2072 6570 6c61 6365 2074 6865 2064 6961   replace the dia
+00001670: 676f 6e61 6c2e 2057 6520 7265 7475 726e  gonal. We return
+00001680: 202d 696e 6620 6c61 7465 722c 2062 7574   -inf later, but
+00001690: 0a20 2020 2023 206e 6565 6420 746f 2070  .    # need to p
+000016a0: 7265 7665 6e74 2073 6f6c 7665 5f6c 6f77  revent solve_low
+000016b0: 6572 2066 726f 6d20 7468 726f 7769 6e67  er from throwing
+000016c0: 2061 6e20 6578 6365 7074 696f 6e2e 0a20   an exception.. 
+000016d0: 2020 2063 686f 6c5f 7461 7520 3d20 7074     chol_tau = pt
+000016e0: 2e73 7769 7463 6828 6f6b 2c20 6368 6f6c  .switch(ok, chol
+000016f0: 5f6d 6174 2c20 3129 0a0a 2020 2020 6465  _mat, 1)..    de
+00001700: 6c74 615f 7472 616e 7320 3d20 7074 2e64  lta_trans = pt.d
+00001710: 6f74 2864 656c 7461 2c20 6368 6f6c 5f74  ot(delta, chol_t
+00001720: 6175 290a 2020 2020 7175 6164 6469 7374  au).    quaddist
+00001730: 203d 2028 6465 6c74 615f 7472 616e 732a   = (delta_trans*
+00001740: 2a32 292e 7375 6d28 6178 6973 3d2d 3129  *2).sum(axis=-1)
+00001750: 0a20 2020 206c 6f67 6465 7420 3d20 2d70  .    logdet = -p
+00001760: 742e 7375 6d28 7074 2e6c 6f67 2864 6961  t.sum(pt.log(dia
+00001770: 6729 290a 2020 2020 7265 7475 726e 2071  g)).    return q
+00001780: 7561 6464 6973 742c 206c 6f67 6465 742c  uaddist, logdet,
+00001790: 206f 6b0a 0a0a 636c 6173 7320 4d76 4e6f   ok...class MvNo
+000017a0: 726d 616c 2843 6f6e 7469 6e75 6f75 7329  rmal(Continuous)
+000017b0: 3a0a 2020 2020 7222 2222 0a20 2020 204d  :.    r""".    M
+000017c0: 756c 7469 7661 7269 6174 6520 6e6f 726d  ultivariate norm
+000017d0: 616c 206c 6f67 2d6c 696b 656c 6968 6f6f  al log-likelihoo
+000017e0: 642e 0a0a 2020 2020 2e2e 206d 6174 683a  d...    .. math:
+000017f0: 3a0a 0a20 2020 2020 2020 6628 7820 5c6d  :..       f(x \m
+00001800: 6964 205c 7069 2c20 5429 203d 0a20 2020  id \pi, T) =.   
+00001810: 2020 2020 2020 2020 5c66 7261 637b 7c54          \frac{|T
+00001820: 7c5e 7b31 2f32 7d7d 7b28 325c 7069 295e  |^{1/2}}{(2\pi)^
+00001830: 7b6b 2f32 7d7d 0a20 2020 2020 2020 2020  {k/2}}.         
+00001840: 2020 5c65 7870 5c6c 6566 745c 7b20 2d5c    \exp\left\{ -\
+00001850: 6672 6163 7b31 7d7b 327d 2028 782d 5c6d  frac{1}{2} (x-\m
+00001860: 7529 5e7b 5c70 7269 6d65 7d20 5420 2878  u)^{\prime} T (x
+00001870: 2d5c 6d75 2920 5c72 6967 6874 5c7d 0a0a  -\mu) \right\}..
+00001880: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
+00001890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000018a0: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053 7570  ========.    Sup
+000018b0: 706f 7274 2020 203a 6d61 7468 3a60 7820  port   :math:`x 
+000018c0: 5c69 6e20 5c6d 6174 6862 627b 527d 5e6b  \in \mathbb{R}^k
+000018d0: 600a 2020 2020 4d65 616e 2020 2020 2020  `.    Mean      
+000018e0: 3a6d 6174 683a 605c 6d75 600a 2020 2020  :math:`\mu`.    
+000018f0: 5661 7269 616e 6365 2020 3a6d 6174 683a  Variance  :math:
+00001900: 6054 5e7b 2d31 7d60 0a20 2020 203d 3d3d  `T^{-1}`.    ===
+00001910: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
+00001920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001930: 3d0a 0a20 2020 2050 6172 616d 6574 6572  =..    Parameter
+00001940: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00001950: 0a20 2020 206d 7520 3a20 7465 6e73 6f72  .    mu : tensor
+00001960: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
+00001970: 2020 2020 2020 2056 6563 746f 7220 6f66         Vector of
+00001980: 206d 6561 6e73 2e0a 2020 2020 636f 7620   means..    cov 
+00001990: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+000019a0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+000019b0: 0a20 2020 2020 2020 2043 6f76 6172 6961  .        Covaria
+000019c0: 6e63 6520 6d61 7472 6978 2e20 4578 6163  nce matrix. Exac
+000019d0: 746c 7920 6f6e 6520 6f66 2063 6f76 2c20  tly one of cov, 
+000019e0: 7461 752c 206f 7220 6368 6f6c 2069 7320  tau, or chol is 
+000019f0: 6e65 6564 6564 2e0a 2020 2020 7461 7520  needed..    tau 
+00001a00: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+00001a10: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+00001a20: 0a20 2020 2020 2020 2050 7265 6369 7369  .        Precisi
+00001a30: 6f6e 206d 6174 7269 782e 2045 7861 6374  on matrix. Exact
+00001a40: 6c79 206f 6e65 206f 6620 636f 762c 2074  ly one of cov, t
+00001a50: 6175 2c20 6f72 2063 686f 6c20 6973 206e  au, or chol is n
+00001a60: 6565 6465 642e 0a20 2020 2063 686f 6c20  eeded..    chol 
+00001a70: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+00001a80: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+00001a90: 0a20 2020 2020 2020 2043 686f 6c65 736b  .        Cholesk
+00001aa0: 7920 6465 636f 6d70 6f73 6974 696f 6e20  y decomposition 
+00001ab0: 6f66 2063 6f76 6172 6961 6e63 6520 6d61  of covariance ma
+00001ac0: 7472 6978 2e20 4578 6163 746c 7920 6f6e  trix. Exactly on
+00001ad0: 6520 6f66 2063 6f76 2c0a 2020 2020 2020  e of cov,.      
+00001ae0: 2020 7461 752c 206f 7220 6368 6f6c 2069    tau, or chol i
+00001af0: 7320 6e65 6564 6564 2e0a 2020 2020 6c6f  s needed..    lo
+00001b00: 7765 723a 2062 6f6f 6c2c 2064 6566 6175  wer: bool, defau
+00001b10: 6c74 3d54 7275 650a 2020 2020 2020 2020  lt=True.        
+00001b20: 5768 6574 6865 7220 6368 6f6c 2069 7320  Whether chol is 
+00001b30: 7468 6520 6c6f 7765 7220 7472 6964 6961  the lower tridia
+00001b40: 676f 6e61 6c20 6368 6f6c 6573 6b79 2066  gonal cholesky f
+00001b50: 6163 746f 722e 0a0a 2020 2020 4578 616d  actor...    Exam
+00001b60: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+00001b70: 2d0a 2020 2020 4465 6669 6e65 2061 206d  -.    Define a m
+00001b80: 756c 7469 7661 7269 6174 6520 6e6f 726d  ultivariate norm
+00001b90: 616c 2076 6172 6961 626c 6520 666f 7220  al variable for 
+00001ba0: 6120 6769 7665 6e20 636f 7661 7269 616e  a given covarian
+00001bb0: 6365 0a20 2020 206d 6174 7269 783a 3a0a  ce.    matrix::.
+00001bc0: 0a20 2020 2020 2020 2063 6f76 203d 206e  .        cov = n
+00001bd0: 702e 6172 7261 7928 5b5b 312e 2c20 302e  p.array([[1., 0.
+00001be0: 355d 2c20 5b30 2e35 2c20 325d 5d29 0a20  5], [0.5, 2]]). 
+00001bf0: 2020 2020 2020 206d 7520 3d20 6e70 2e7a         mu = np.z
+00001c00: 6572 6f73 2832 290a 2020 2020 2020 2020  eros(2).        
+00001c10: 7661 6c73 203d 2070 6d2e 4d76 4e6f 726d  vals = pm.MvNorm
+00001c20: 616c 2827 7661 6c73 272c 206d 753d 6d75  al('vals', mu=mu
+00001c30: 2c20 636f 763d 636f 762c 2073 6861 7065  , cov=cov, shape
+00001c40: 3d28 352c 2032 2929 0a0a 2020 2020 4d6f  =(5, 2))..    Mo
+00001c50: 7374 206f 6620 7468 6520 7469 6d65 2069  st of the time i
+00001c60: 7420 6973 2070 7265 6665 7261 626c 6520  t is preferable 
+00001c70: 746f 2073 7065 6369 6679 2074 6865 2063  to specify the c
+00001c80: 686f 6c65 736b 790a 2020 2020 6661 6374  holesky.    fact
+00001c90: 6f72 206f 6620 7468 6520 636f 7661 7269  or of the covari
+00001ca0: 616e 6365 2069 6e73 7465 6164 2e20 466f  ance instead. Fo
+00001cb0: 7220 6578 616d 706c 652c 2077 6520 636f  r example, we co
+00001cc0: 756c 640a 2020 2020 6669 7420 6120 6d75  uld.    fit a mu
+00001cd0: 6c74 6976 6172 6961 7465 206f 7574 636f  ltivariate outco
+00001ce0: 6d65 206c 696b 6520 7468 6973 2028 7365  me like this (se
+00001cf0: 6520 7468 6520 646f 6373 7472 696e 670a  e the docstring.
+00001d00: 2020 2020 6f66 2060 4c4b 4a43 686f 6c65      of `LKJChole
+00001d10: 736b 7943 6f76 6020 666f 7220 6d6f 7265  skyCov` for more
+00001d20: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00001d30: 7574 2074 6869 7329 3a3a 0a0a 2020 2020  ut this)::..    
+00001d40: 2020 2020 6d75 203d 206e 702e 7a65 726f      mu = np.zero
+00001d50: 7328 3329 0a20 2020 2020 2020 2074 7275  s(3).        tru
+00001d60: 655f 636f 7620 3d20 6e70 2e61 7272 6179  e_cov = np.array
+00001d70: 285b 5b31 2e30 2c20 302e 352c 2030 2e31  ([[1.0, 0.5, 0.1
+00001d80: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 5b30 2e35 2c20 322e 302c 2030 2e32 5d2c  [0.5, 2.0, 0.2],
+00001db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
+00001dd0: 2e31 2c20 302e 322c 2031 2e30 5d5d 290a  .1, 0.2, 1.0]]).
+00001de0: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
+00001df0: 702e 7261 6e64 6f6d 2e6d 756c 7469 7661  p.random.multiva
+00001e00: 7269 6174 655f 6e6f 726d 616c 286d 752c  riate_normal(mu,
+00001e10: 2074 7275 655f 636f 762c 2031 3029 0a0a   true_cov, 10)..
+00001e20: 2020 2020 2020 2020 7364 5f64 6973 7420          sd_dist 
+00001e30: 3d20 706d 2e45 7870 6f6e 656e 7469 616c  = pm.Exponential
+00001e40: 2e64 6973 7428 312e 302c 2073 6861 7065  .dist(1.0, shape
+00001e50: 3d33 290a 2020 2020 2020 2020 6368 6f6c  =3).        chol
+00001e60: 2c20 636f 7272 2c20 7374 6473 203d 2070  , corr, stds = p
+00001e70: 6d2e 4c4b 4a43 686f 6c65 736b 7943 6f76  m.LKJCholeskyCov
+00001e80: 2827 6368 6f6c 5f63 6f76 272c 206e 3d33  ('chol_cov', n=3
+00001e90: 2c20 6574 613d 322c 0a20 2020 2020 2020  , eta=2,.       
+00001ea0: 2020 2020 2073 645f 6469 7374 3d73 645f       sd_dist=sd_
+00001eb0: 6469 7374 2c20 636f 6d70 7574 655f 636f  dist, compute_co
+00001ec0: 7272 3d54 7275 6529 0a20 2020 2020 2020  rr=True).       
+00001ed0: 2076 616c 7320 3d20 706d 2e4d 764e 6f72   vals = pm.MvNor
+00001ee0: 6d61 6c28 2776 616c 7327 2c20 6d75 3d6d  mal('vals', mu=m
+00001ef0: 752c 2063 686f 6c3d 6368 6f6c 2c20 6f62  u, chol=chol, ob
+00001f00: 7365 7276 6564 3d64 6174 6129 0a0a 2020  served=data)..  
+00001f10: 2020 466f 7220 756e 6f62 7365 7276 6564    For unobserved
+00001f20: 2076 616c 7565 7320 6974 2063 616e 2062   values it can b
+00001f30: 6520 6265 7474 6572 2074 6f20 7573 6520  e better to use 
+00001f40: 6120 6e6f 6e2d 6365 6e74 6572 6564 0a20  a non-centered. 
+00001f50: 2020 2070 6172 616d 6574 7269 7a61 7469     parametrizati
+00001f60: 6f6e 3a3a 0a0a 2020 2020 2020 2020 7364  on::..        sd
+00001f70: 5f64 6973 7420 3d20 706d 2e45 7870 6f6e  _dist = pm.Expon
+00001f80: 656e 7469 616c 2e64 6973 7428 312e 302c  ential.dist(1.0,
+00001f90: 2073 6861 7065 3d33 290a 2020 2020 2020   shape=3).      
+00001fa0: 2020 6368 6f6c 2c20 5f2c 205f 203d 2070    chol, _, _ = p
+00001fb0: 6d2e 4c4b 4a43 686f 6c65 736b 7943 6f76  m.LKJCholeskyCov
+00001fc0: 2827 6368 6f6c 5f63 6f76 272c 206e 3d33  ('chol_cov', n=3
+00001fd0: 2c20 6574 613d 322c 0a20 2020 2020 2020  , eta=2,.       
+00001fe0: 2020 2020 2073 645f 6469 7374 3d73 645f       sd_dist=sd_
+00001ff0: 6469 7374 2c20 636f 6d70 7574 655f 636f  dist, compute_co
+00002000: 7272 3d54 7275 6529 0a20 2020 2020 2020  rr=True).       
+00002010: 2076 616c 735f 7261 7720 3d20 706d 2e4e   vals_raw = pm.N
+00002020: 6f72 6d61 6c28 2776 616c 735f 7261 7727  ormal('vals_raw'
+00002030: 2c20 6d75 3d30 2c20 7369 676d 613d 312c  , mu=0, sigma=1,
+00002040: 2073 6861 7065 3d28 352c 2033 2929 0a20   shape=(5, 3)). 
+00002050: 2020 2020 2020 2076 616c 7320 3d20 706d         vals = pm
+00002060: 2e44 6574 6572 6d69 6e69 7374 6963 2827  .Deterministic('
+00002070: 7661 6c73 272c 2070 742e 646f 7428 6368  vals', pt.dot(ch
+00002080: 6f6c 2c20 7661 6c73 5f72 6177 2e54 292e  ol, vals_raw.T).
+00002090: 5429 0a20 2020 2022 2222 0a20 2020 2072  T).    """.    r
+000020a0: 765f 6f70 203d 206d 756c 7469 7661 7269  v_op = multivari
+000020b0: 6174 655f 6e6f 726d 616c 0a0a 2020 2020  ate_normal..    
+000020c0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+000020d0: 2064 6566 2064 6973 7428 636c 732c 206d   def dist(cls, m
+000020e0: 752c 2063 6f76 3d4e 6f6e 652c 2074 6175  u, cov=None, tau
+000020f0: 3d4e 6f6e 652c 2063 686f 6c3d 4e6f 6e65  =None, chol=None
+00002100: 2c20 6c6f 7765 723d 5472 7565 2c20 2a2a  , lower=True, **
+00002110: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00002120: 206d 7520 3d20 7074 2e61 735f 7465 6e73   mu = pt.as_tens
+00002130: 6f72 5f76 6172 6961 626c 6528 6d75 290a  or_variable(mu).
+00002140: 2020 2020 2020 2020 636f 7620 3d20 7175          cov = qu
+00002150: 6164 6469 7374 5f6d 6174 7269 7828 636f  addist_matrix(co
+00002160: 762c 2063 686f 6c2c 2074 6175 2c20 6c6f  v, chol, tau, lo
+00002170: 7765 7229 0a20 2020 2020 2020 2023 2050  wer).        # P
+00002180: 7954 656e 736f 7220 6973 2073 7472 6963  yTensor is stric
+00002190: 7465 7220 6162 6f75 7420 7468 6520 7368  ter about the sh
+000021a0: 6170 6520 6f66 206d 752c 2074 6861 6e20  ape of mu, than 
+000021b0: 5079 4d43 2075 7365 6420 746f 2062 650a  PyMC used to be.
+000021c0: 2020 2020 2020 2020 6d75 203d 2070 742e          mu = pt.
+000021d0: 6272 6f61 6463 6173 745f 6172 7261 7973  broadcast_arrays
+000021e0: 286d 752c 2063 6f76 5b2e 2e2e 2c20 2d31  (mu, cov[..., -1
+000021f0: 5d29 5b30 5d0a 2020 2020 2020 2020 7265  ])[0].        re
+00002200: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
+00002210: 7428 5b6d 752c 2063 6f76 5d2c 202a 2a6b  t([mu, cov], **k
+00002220: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+00002230: 6d6f 6d65 6e74 2872 762c 2073 697a 652c  moment(rv, size,
+00002240: 206d 752c 2063 6f76 293a 0a20 2020 2020   mu, cov):.     
+00002250: 2020 206d 6f6d 656e 7420 3d20 6d75 0a20     moment = mu. 
+00002260: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
+00002270: 5f73 697a 655f 6973 5f6e 6f6e 6528 7369  _size_is_none(si
+00002280: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
+00002290: 206d 6f6d 656e 745f 7369 7a65 203d 2070   moment_size = p
+000022a0: 742e 636f 6e63 6174 656e 6174 6528 5b73  t.concatenate([s
+000022b0: 697a 652c 205b 6d75 2e73 6861 7065 5b2d  ize, [mu.shape[-
+000022c0: 315d 5d5d 290a 2020 2020 2020 2020 2020  1]]]).          
+000022d0: 2020 6d6f 6d65 6e74 203d 2070 742e 6675    moment = pt.fu
+000022e0: 6c6c 286d 6f6d 656e 745f 7369 7a65 2c20  ll(moment_size, 
+000022f0: 6d75 290a 2020 2020 2020 2020 7265 7475  mu).        retu
+00002300: 726e 206d 6f6d 656e 740a 0a20 2020 2064  rn moment..    d
+00002310: 6566 206c 6f67 7028 7661 6c75 652c 206d  ef logp(value, m
+00002320: 752c 2063 6f76 293a 0a20 2020 2020 2020  u, cov):.       
+00002330: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+00002340: 6375 6c61 7465 206c 6f67 2d70 726f 6261  culate log-proba
+00002350: 6269 6c69 7479 206f 6620 4d75 6c74 6976  bility of Multiv
+00002360: 6172 6961 7465 204e 6f72 6d61 6c20 6469  ariate Normal di
+00002370: 7374 7269 6275 7469 6f6e 0a20 2020 2020  stribution.     
+00002380: 2020 2061 7420 7370 6563 6966 6965 6420     at specified 
+00002390: 7661 6c75 652e 0a0a 2020 2020 2020 2020  value...        
+000023a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000023b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000023c0: 2020 2020 2020 7661 6c75 653a 206e 756d        value: num
+000023d0: 6572 6963 0a20 2020 2020 2020 2020 2020  eric.           
+000023e0: 2056 616c 7565 2066 6f72 2077 6869 6368   Value for which
+000023f0: 206c 6f67 2d70 726f 6261 6269 6c69 7479   log-probability
+00002400: 2069 7320 6361 6c63 756c 6174 6564 2e0a   is calculated..
+00002410: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00002420: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002430: 0a20 2020 2020 2020 2054 656e 736f 7256  .        TensorV
+00002440: 6172 6961 626c 650a 2020 2020 2020 2020  ariable.        
+00002450: 2222 220a 2020 2020 2020 2020 7175 6164  """.        quad
+00002460: 6469 7374 2c20 6c6f 6764 6574 2c20 6f6b  dist, logdet, ok
+00002470: 203d 2071 7561 6464 6973 745f 7061 7273   = quaddist_pars
+00002480: 6528 7661 6c75 652c 206d 752c 2063 6f76  e(value, mu, cov
+00002490: 290a 2020 2020 2020 2020 6b20 3d20 666c  ).        k = fl
+000024a0: 6f61 7458 2876 616c 7565 2e73 6861 7065  oatX(value.shape
+000024b0: 5b2d 315d 290a 2020 2020 2020 2020 6e6f  [-1]).        no
+000024c0: 726d 203d 202d 302e 3520 2a20 6b20 2a20  rm = -0.5 * k * 
+000024d0: 706d 2e66 6c6f 6174 5828 6e70 2e6c 6f67  pm.floatX(np.log
+000024e0: 2832 202a 206e 702e 7069 2929 0a20 2020  (2 * np.pi)).   
+000024f0: 2020 2020 2072 6574 7572 6e20 6368 6563       return chec
+00002500: 6b5f 7061 7261 6d65 7465 7273 280a 2020  k_parameters(.  
+00002510: 2020 2020 2020 2020 2020 6e6f 726d 202d            norm -
+00002520: 2030 2e35 202a 2071 7561 6464 6973 7420   0.5 * quaddist 
+00002530: 2d20 6c6f 6764 6574 2c0a 2020 2020 2020  - logdet,.      
+00002540: 2020 2020 2020 6f6b 2c0a 2020 2020 2020        ok,.      
+00002550: 2020 2020 2020 6d73 673d 2270 6f73 6465        msg="posde
+00002560: 6622 2c0a 2020 2020 2020 2020 290a 0a0a  f",.        )...
+00002570: 636c 6173 7320 4d76 5374 7564 656e 7454  class MvStudentT
+00002580: 5256 2852 616e 646f 6d56 6172 6961 626c  RV(RandomVariabl
+00002590: 6529 3a0a 2020 2020 6e61 6d65 203d 2022  e):.    name = "
+000025a0: 6d75 6c74 6976 6172 6961 7465 5f73 7475  multivariate_stu
+000025b0: 6465 6e74 7422 0a20 2020 206e 6469 6d5f  dentt".    ndim_
+000025c0: 7375 7070 203d 2031 0a20 2020 206e 6469  supp = 1.    ndi
+000025d0: 6d73 5f70 6172 616d 7320 3d20 5b30 2c20  ms_params = [0, 
+000025e0: 312c 2032 5d0a 2020 2020 6474 7970 6520  1, 2].    dtype 
+000025f0: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
+00002600: 7072 696e 745f 6e61 6d65 203d 2028 224d  print_name = ("M
+00002610: 7653 7475 6465 6e74 5422 2c20 225c 5c6f  vStudentT", "\\o
+00002620: 7065 7261 746f 726e 616d 657b 4d76 5374  peratorname{MvSt
+00002630: 7564 656e 7454 7d22 290a 0a20 2020 2064  udentT}")..    d
+00002640: 6566 206d 616b 655f 6e6f 6465 2873 656c  ef make_node(sel
+00002650: 662c 2072 6e67 2c20 7369 7a65 2c20 6474  f, rng, size, dt
+00002660: 7970 652c 206e 752c 206d 752c 2063 6f76  ype, nu, mu, cov
+00002670: 293a 0a20 2020 2020 2020 206e 7520 3d20  ):.        nu = 
+00002680: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+00002690: 6961 626c 6528 6e75 290a 2020 2020 2020  iable(nu).      
+000026a0: 2020 6966 206e 6f74 206e 752e 6e64 696d    if not nu.ndim
+000026b0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+000026c0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000026d0: 726f 7228 226e 7520 6d75 7374 2062 6520  ror("nu must be 
+000026e0: 6120 7363 616c 6172 2028 6e64 696d 3d30  a scalar (ndim=0
+000026f0: 292e 2229 0a0a 2020 2020 2020 2020 7265  ).")..        re
+00002700: 7475 726e 2073 7570 6572 2829 2e6d 616b  turn super().mak
+00002710: 655f 6e6f 6465 2872 6e67 2c20 7369 7a65  e_node(rng, size
+00002720: 2c20 6474 7970 652c 206e 752c 206d 752c  , dtype, nu, mu,
+00002730: 2063 6f76 290a 0a20 2020 2064 6566 205f   cov)..    def _
+00002740: 5f63 616c 6c5f 5f28 7365 6c66 2c20 6e75  _call__(self, nu
+00002750: 2c20 6d75 3d4e 6f6e 652c 2063 6f76 3d4e  , mu=None, cov=N
+00002760: 6f6e 652c 2073 697a 653d 4e6f 6e65 2c20  one, size=None, 
+00002770: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00002780: 2020 2064 7479 7065 203d 2070 7974 656e     dtype = pyten
+00002790: 736f 722e 636f 6e66 6967 2e66 6c6f 6174  sor.config.float
+000027a0: 5820 6966 2073 656c 662e 6474 7970 6520  X if self.dtype 
+000027b0: 3d3d 2022 666c 6f61 7458 2220 656c 7365  == "floatX" else
+000027c0: 2073 656c 662e 6474 7970 650a 0a20 2020   self.dtype..   
+000027d0: 2020 2020 2069 6620 6d75 2069 7320 4e6f       if mu is No
+000027e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000027f0: 6d75 203d 206e 702e 6172 7261 7928 5b30  mu = np.array([0
+00002800: 2e30 5d2c 2064 7479 7065 3d64 7479 7065  .0], dtype=dtype
+00002810: 290a 2020 2020 2020 2020 6966 2063 6f76  ).        if cov
+00002820: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00002830: 2020 2020 2020 636f 7620 3d20 6e70 2e61        cov = np.a
+00002840: 7272 6179 285b 5b31 2e30 5d5d 2c20 6474  rray([[1.0]], dt
+00002850: 7970 653d 6474 7970 6529 0a20 2020 2020  ype=dtype).     
+00002860: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00002870: 292e 5f5f 6361 6c6c 5f5f 286e 752c 206d  ).__call__(nu, m
+00002880: 752c 2063 6f76 2c20 7369 7a65 3d73 697a  u, cov, size=siz
+00002890: 652c 202a 2a6b 7761 7267 7329 0a0a 2020  e, **kwargs)..  
+000028a0: 2020 6465 6620 5f73 7570 705f 7368 6170    def _supp_shap
+000028b0: 655f 6672 6f6d 5f70 6172 616d 7328 7365  e_from_params(se
+000028c0: 6c66 2c20 6469 7374 5f70 6172 616d 732c  lf, dist_params,
+000028d0: 2070 6172 616d 5f73 6861 7065 733d 4e6f   param_shapes=No
+000028e0: 6e65 293a 0a20 2020 2020 2020 2072 6574  ne):.        ret
+000028f0: 7572 6e20 7375 7070 5f73 6861 7065 5f66  urn supp_shape_f
+00002900: 726f 6d5f 7265 665f 7061 7261 6d5f 7368  rom_ref_param_sh
+00002910: 6170 6528 0a20 2020 2020 2020 2020 2020  ape(.           
+00002920: 206e 6469 6d5f 7375 7070 3d73 656c 662e   ndim_supp=self.
+00002930: 6e64 696d 5f73 7570 702c 0a20 2020 2020  ndim_supp,.     
+00002940: 2020 2020 2020 2064 6973 745f 7061 7261         dist_para
+00002950: 6d73 3d64 6973 745f 7061 7261 6d73 2c0a  ms=dist_params,.
+00002960: 2020 2020 2020 2020 2020 2020 7061 7261              para
+00002970: 6d5f 7368 6170 6573 3d70 6172 616d 5f73  m_shapes=param_s
+00002980: 6861 7065 732c 0a20 2020 2020 2020 2020  hapes,.         
+00002990: 2020 2072 6566 5f70 6172 616d 5f69 6478     ref_param_idx
+000029a0: 3d31 2c0a 2020 2020 2020 2020 290a 0a20  =1,.        ).. 
+000029b0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000029c0: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
+000029d0: 6c73 2c20 726e 672c 206e 752c 206d 752c  ls, rng, nu, mu,
+000029e0: 2063 6f76 2c20 7369 7a65 293a 0a20 2020   cov, size):.   
+000029f0: 2020 2020 206d 765f 7361 6d70 6c65 7320       mv_samples 
+00002a00: 3d20 6d75 6c74 6976 6172 6961 7465 5f6e  = multivariate_n
+00002a10: 6f72 6d61 6c2e 726e 675f 666e 2872 6e67  ormal.rng_fn(rng
+00002a20: 3d72 6e67 2c20 6d65 616e 3d6e 702e 7a65  =rng, mean=np.ze
+00002a30: 726f 735f 6c69 6b65 286d 7529 2c20 636f  ros_like(mu), co
+00002a40: 763d 636f 762c 2073 697a 653d 7369 7a65  v=cov, size=size
+00002a50: 290a 0a20 2020 2020 2020 2023 2054 616b  )..        # Tak
+00002a60: 6520 6368 6932 2064 7261 7773 2061 6e64  e chi2 draws and
+00002a70: 2061 6464 2061 6e20 6178 6973 206f 6620   add an axis of 
+00002a80: 6c65 6e67 7468 2031 2074 6f20 7468 6520  length 1 to the 
+00002a90: 7269 6768 7420 666f 7220 636f 7272 6563  right for correc
+00002aa0: 7420 6272 6f61 6463 6173 7469 6e67 2062  t broadcasting b
+00002ab0: 656c 6f77 0a20 2020 2020 2020 2063 6869  elow.        chi
+00002ac0: 325f 7361 6d70 6c65 7320 3d20 6e70 2e73  2_samples = np.s
+00002ad0: 7172 7428 726e 672e 6368 6973 7175 6172  qrt(rng.chisquar
+00002ae0: 6528 6e75 2c20 7369 7a65 3d73 697a 6529  e(nu, size=size)
+00002af0: 202f 206e 7529 5b2e 2e2e 2c20 4e6f 6e65   / nu)[..., None
+00002b00: 5d0a 0a20 2020 2020 2020 2069 6620 7369  ]..        if si
+00002b10: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+00002b20: 6d75 203d 206e 702e 6272 6f61 6463 6173  mu = np.broadcas
+00002b30: 745f 746f 286d 752c 2073 697a 6520 2b20  t_to(mu, size + 
+00002b40: 286d 752e 7368 6170 655b 2d31 5d2c 2929  (mu.shape[-1],))
+00002b50: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002b60: 2028 6d76 5f73 616d 706c 6573 202f 2063   (mv_samples / c
+00002b70: 6869 325f 7361 6d70 6c65 7329 202b 206d  hi2_samples) + m
+00002b80: 750a 0a0a 6d76 5f73 7475 6465 6e74 7420  u...mv_studentt 
+00002b90: 3d20 4d76 5374 7564 656e 7454 5256 2829  = MvStudentTRV()
+00002ba0: 0a0a 0a63 6c61 7373 204d 7653 7475 6465  ...class MvStude
+00002bb0: 6e74 5428 436f 6e74 696e 756f 7573 293a  ntT(Continuous):
+00002bc0: 0a20 2020 2072 2222 220a 2020 2020 4d75  .    r""".    Mu
+00002bd0: 6c74 6976 6172 6961 7465 2053 7475 6465  ltivariate Stude
+00002be0: 6e74 2d54 206c 6f67 2d6c 696b 656c 6968  nt-T log-likelih
+00002bf0: 6f6f 642e 0a0a 2020 2020 2e2e 206d 6174  ood...    .. mat
+00002c00: 683a 3a0a 2020 2020 2020 2020 6628 5c6d  h::.        f(\m
+00002c10: 6174 6862 667b 787d 7c20 5c6e 752c 5c6d  athbf{x}| \nu,\m
+00002c20: 752c 5c53 6967 6d61 2920 3d0a 2020 2020  u,\Sigma) =.    
+00002c30: 2020 2020 5c66 7261 630a 2020 2020 2020      \frac.      
+00002c40: 2020 2020 2020 7b5c 4761 6d6d 615c 6c65        {\Gamma\le
+00002c50: 6674 5b28 5c6e 752b 7029 2f32 5c72 6967  ft[(\nu+p)/2\rig
+00002c60: 6874 5d7d 0a20 2020 2020 2020 2020 2020  ht]}.           
+00002c70: 207b 5c47 616d 6d61 285c 6e75 2f32 295c   {\Gamma(\nu/2)\
+00002c80: 6e75 5e7b 702f 327d 5c70 695e 7b70 2f32  nu^{p/2}\pi^{p/2
+00002c90: 7d0a 2020 2020 2020 2020 2020 2020 205c  }.             \
+00002ca0: 6c65 6674 7c7b 5c53 6967 6d61 7d5c 7269  left|{\Sigma}\ri
+00002cb0: 6768 747c 5e7b 312f 327d 0a20 2020 2020  ght|^{1/2}.     
+00002cc0: 2020 2020 2020 2020 5c6c 6566 745b 0a20          \left[. 
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 312b                1+
+00002ce0: 5c66 7261 637b 317d 7b5c 6e75 7d0a 2020  \frac{1}{\nu}.  
+00002cf0: 2020 2020 2020 2020 2020 2020 2028 7b5c               ({\
+00002d00: 6d61 7468 6266 2078 7d2d 7b5c 6d75 7d29  mathbf x}-{\mu})
+00002d10: 5e54 0a20 2020 2020 2020 2020 2020 2020  ^T.             
+00002d20: 2020 7b5c 5369 676d 617d 5e7b 2d31 7d28    {\Sigma}^{-1}(
+00002d30: 7b5c 6d61 7468 6266 2078 7d2d 7b5c 6d75  {\mathbf x}-{\mu
+00002d40: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
+00002d50: 5c72 6967 6874 5d5e 7b2d 285c 6e75 2b70  \right]^{-(\nu+p
+00002d60: 292f 327d 7d0a 0a20 2020 203d 3d3d 3d3d  )/2}}..    =====
+00002d70: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+00002d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002da0: 3d3d 0a20 2020 2053 7570 706f 7274 2020  ==.    Support  
+00002db0: 203a 6d61 7468 3a60 7820 5c69 6e20 5c6d   :math:`x \in \m
+00002dc0: 6174 6862 627b 527d 5e70 600a 2020 2020  athbb{R}^p`.    
+00002dd0: 4d65 616e 2020 2020 2020 3a6d 6174 683a  Mean      :math:
+00002de0: 605c 6d75 6020 6966 203a 6d61 7468 3a60  `\mu` if :math:`
+00002df0: 5c6e 7520 3e20 3160 2065 6c73 6520 756e  \nu > 1` else un
+00002e00: 6465 6669 6e65 640a 2020 2020 5661 7269  defined.    Vari
+00002e10: 616e 6365 2020 3a6d 6174 683a 605c 6672  ance  :math:`\fr
+00002e20: 6163 7b5c 6e75 7d7b 5c6d 752d 327d 5c53  ac{\nu}{\mu-2}\S
+00002e30: 6967 6d61 600a 2020 2020 2020 2020 2020  igma`.          
+00002e40: 2020 2020 2020 2020 6966 203a 6d61 7468          if :math
+00002e50: 3a60 5c6e 753e 3260 2065 6c73 6520 756e  :`\nu>2` else un
+00002e60: 6465 6669 6e65 640a 2020 2020 3d3d 3d3d  defined.    ====
+00002e70: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+00002e80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002e90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002ea0: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
+00002eb0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00002ec0: 2d2d 0a20 2020 206e 7520 3a20 7465 6e73  --.    nu : tens
+00002ed0: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+00002ee0: 0a20 2020 2020 2020 2044 6567 7265 6573  .        Degrees
+00002ef0: 206f 6620 6672 6565 646f 6d2c 2073 686f   of freedom, sho
+00002f00: 756c 6420 6265 2061 2070 6f73 6974 6976  uld be a positiv
+00002f10: 6520 7363 616c 6172 2e0a 2020 2020 5369  e scalar..    Si
+00002f20: 676d 6120 3a20 7465 6e73 6f72 5f6c 696b  gma : tensor_lik
+00002f30: 6520 6f66 2066 6c6f 6174 2c20 6f70 7469  e of float, opti
+00002f40: 6f6e 616c 0a20 2020 2020 2020 2053 6361  onal.        Sca
+00002f50: 6c65 206d 6174 7269 782e 2055 7365 2060  le matrix. Use `
+00002f60: 7363 616c 6560 2069 6e20 6e65 7720 636f  scale` in new co
+00002f70: 6465 2e0a 2020 2020 6d75 203a 2074 656e  de..    mu : ten
+00002f80: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
+00002f90: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+00002fa0: 2020 2020 5665 6374 6f72 206f 6620 6d65      Vector of me
+00002fb0: 616e 732e 0a20 2020 2073 6361 6c65 203a  ans..    scale :
+00002fc0: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
+00002fd0: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+00002fe0: 2020 2020 2020 2020 5468 6520 7363 616c          The scal
+00002ff0: 6520 6d61 7472 6978 2e0a 2020 2020 7461  e matrix..    ta
+00003000: 7520 3a20 7465 6e73 6f72 5f6c 696b 6520  u : tensor_like 
 00003010: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
-00003020: 616c 0a20 2020 2020 2020 2054 6865 2063  al.        The c
-00003030: 686f 6c65 736b 7920 6661 6374 6f72 206f  holesky factor o
-00003040: 6620 7468 6520 7363 616c 6520 6d61 7472  f the scale matr
-00003050: 6978 2e0a 2020 2020 6c6f 7765 7220 3a20  ix..    lower : 
-00003060: 626f 6f6c 2c20 6465 6661 756c 743d 5472  bool, default=Tr
-00003070: 7565 0a20 2020 2020 2020 2057 6865 7468  ue.        Wheth
-00003080: 6572 2074 6865 2063 686f 6c65 736b 7920  er the cholesky 
-00003090: 6661 7463 6f72 2069 7320 6769 7665 6e20  fatcor is given 
-000030a0: 6173 2061 206c 6f77 6572 2074 7269 616e  as a lower trian
-000030b0: 6775 6c61 7220 6d61 7472 6978 2e0a 2020  gular matrix..  
-000030c0: 2020 2222 220a 2020 2020 7276 5f6f 7020    """.    rv_op 
-000030d0: 3d20 6d76 5f73 7475 6465 6e74 740a 0a20  = mv_studentt.. 
-000030e0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-000030f0: 2020 2020 6465 6620 6469 7374 2863 6c73      def dist(cls
-00003100: 2c20 6e75 2c20 5369 676d 613d 4e6f 6e65  , nu, Sigma=None
-00003110: 2c20 6d75 3d4e 6f6e 652c 2073 6361 6c65  , mu=None, scale
-00003120: 3d4e 6f6e 652c 2074 6175 3d4e 6f6e 652c  =None, tau=None,
-00003130: 2063 686f 6c3d 4e6f 6e65 2c20 6c6f 7765   chol=None, lowe
-00003140: 723d 5472 7565 2c20 2a2a 6b77 6172 6773  r=True, **kwargs
-00003150: 293a 0a20 2020 2020 2020 2063 6f76 203d  ):.        cov =
-00003160: 206b 7761 7267 732e 706f 7028 2263 6f76   kwargs.pop("cov
-00003170: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-00003180: 2069 6620 636f 7620 6973 206e 6f74 204e   if cov is not N
-00003190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000031a0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031c0: 2255 7365 2074 6865 2073 6361 6c65 2061  "Use the scale a
-000031d0: 7267 756d 656e 7420 746f 2073 7065 6369  rgument to speci
-000031e0: 6679 2074 6865 2073 6361 6c65 206d 6174  fy the scale mat
-000031f0: 7269 782e 2022 0a20 2020 2020 2020 2020  rix. ".         
-00003200: 2020 2020 2020 2022 636f 7620 7769 6c6c         "cov will
-00003210: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
-00003220: 7574 7572 6520 7665 7273 696f 6e73 2e22  uture versions."
-00003230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003240: 2020 4675 7475 7265 5761 726e 696e 672c    FutureWarning,
-00003250: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00003260: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00003270: 203d 2063 6f76 0a20 2020 2020 2020 2069   = cov.        i
-00003280: 6620 5369 676d 6120 6973 206e 6f74 204e  f Sigma is not N
-00003290: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000032a0: 2069 6620 7363 616c 6520 6973 206e 6f74   if scale is not
-000032b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000032c0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000032d0: 7565 4572 726f 7228 2253 7065 6369 6679  ueError("Specify
-000032e0: 206f 6e6c 7920 6f6e 6520 6f66 2073 6361   only one of sca
-000032f0: 6c65 2061 6e64 2053 6967 6d61 2229 0a20  le and Sigma"). 
-00003300: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00003310: 203d 2053 6967 6d61 0a20 2020 2020 2020   = Sigma.       
-00003320: 206e 7520 3d20 7074 2e61 735f 7465 6e73   nu = pt.as_tens
-00003330: 6f72 5f76 6172 6961 626c 6528 666c 6f61  or_variable(floa
-00003340: 7458 286e 7529 290a 2020 2020 2020 2020  tX(nu)).        
-00003350: 6d75 203d 2070 742e 6173 5f74 656e 736f  mu = pt.as_tenso
-00003360: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
-00003370: 5828 6d75 2929 0a20 2020 2020 2020 2073  X(mu)).        s
-00003380: 6361 6c65 203d 2071 7561 6464 6973 745f  cale = quaddist_
-00003390: 6d61 7472 6978 2873 6361 6c65 2c20 6368  matrix(scale, ch
-000033a0: 6f6c 2c20 7461 752c 206c 6f77 6572 290a  ol, tau, lower).
-000033b0: 2020 2020 2020 2020 2320 5079 5465 6e73          # PyTens
-000033c0: 6f72 2069 7320 7374 7269 6374 6572 2061  or is stricter a
-000033d0: 626f 7574 2074 6865 2073 6861 7065 206f  bout the shape o
-000033e0: 6620 6d75 2c20 7468 616e 2050 794d 4320  f mu, than PyMC 
-000033f0: 7573 6564 2074 6f20 6265 0a20 2020 2020  used to be.     
-00003400: 2020 206d 7520 3d20 7074 2e62 726f 6164     mu = pt.broad
-00003410: 6361 7374 5f61 7272 6179 7328 6d75 2c20  cast_arrays(mu, 
-00003420: 7363 616c 655b 2e2e 2e2c 202d 315d 295b  scale[..., -1])[
-00003430: 305d 0a0a 2020 2020 2020 2020 7265 7475  0]..        retu
-00003440: 726e 2073 7570 6572 2829 2e64 6973 7428  rn super().dist(
-00003450: 5b6e 752c 206d 752c 2073 6361 6c65 5d2c  [nu, mu, scale],
-00003460: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-00003470: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
-00003480: 697a 652c 206e 752c 206d 752c 2073 6361  ize, nu, mu, sca
-00003490: 6c65 293a 0a20 2020 2020 2020 206d 6f6d  le):.        mom
-000034a0: 656e 7420 3d20 6d75 0a20 2020 2020 2020  ent = mu.       
-000034b0: 2069 6620 6e6f 7420 7276 5f73 697a 655f   if not rv_size_
-000034c0: 6973 5f6e 6f6e 6528 7369 7a65 293a 0a20  is_none(size):. 
-000034d0: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
-000034e0: 745f 7369 7a65 203d 2070 742e 636f 6e63  t_size = pt.conc
-000034f0: 6174 656e 6174 6528 5b73 697a 652c 205b  atenate([size, [
-00003500: 6d75 2e73 6861 7065 5b2d 315d 5d5d 290a  mu.shape[-1]]]).
-00003510: 2020 2020 2020 2020 2020 2020 6d6f 6d65              mome
-00003520: 6e74 203d 2070 742e 6675 6c6c 286d 6f6d  nt = pt.full(mom
-00003530: 656e 745f 7369 7a65 2c20 6d6f 6d65 6e74  ent_size, moment
-00003540: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00003550: 206d 6f6d 656e 740a 0a20 2020 2064 6566   moment..    def
-00003560: 206c 6f67 7028 7661 6c75 652c 206e 752c   logp(value, nu,
-00003570: 206d 752c 2073 6361 6c65 293a 0a20 2020   mu, scale):.   
-00003580: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003590: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
-000035a0: 726f 6261 6269 6c69 7479 206f 6620 4d75  robability of Mu
-000035b0: 6c74 6976 6172 6961 7465 2053 7475 6465  ltivariate Stude
-000035c0: 6e74 2773 2054 2064 6973 7472 6962 7574  nt's T distribut
-000035d0: 696f 6e0a 2020 2020 2020 2020 6174 2073  ion.        at s
-000035e0: 7065 6369 6669 6564 2076 616c 7565 2e0a  pecified value..
-000035f0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00003600: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00003610: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2076  ------.        v
-00003620: 616c 7565 3a20 6e75 6d65 7269 630a 2020  alue: numeric.  
-00003630: 2020 2020 2020 2020 2020 5661 6c75 6520            Value 
-00003640: 666f 7220 7768 6963 6820 6c6f 672d 7072  for which log-pr
-00003650: 6f62 6162 696c 6974 7920 6973 2063 616c  obability is cal
-00003660: 6375 6c61 7465 642e 0a0a 2020 2020 2020  culated...      
-00003670: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00003680: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00003690: 2020 5465 6e73 6f72 5661 7269 6162 6c65    TensorVariable
-000036a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000036b0: 2020 2020 2071 7561 6464 6973 742c 206c       quaddist, l
-000036c0: 6f67 6465 742c 206f 6b20 3d20 7175 6164  ogdet, ok = quad
-000036d0: 6469 7374 5f70 6172 7365 2876 616c 7565  dist_parse(value
-000036e0: 2c20 6d75 2c20 7363 616c 6529 0a20 2020  , mu, scale).   
-000036f0: 2020 2020 206b 203d 2066 6c6f 6174 5828       k = floatX(
-00003700: 7661 6c75 652e 7368 6170 655b 2d31 5d29  value.shape[-1])
-00003710: 0a0a 2020 2020 2020 2020 6e6f 726d 203d  ..        norm =
-00003720: 2067 616d 6d61 6c6e 2828 6e75 202b 206b   gammaln((nu + k
-00003730: 2920 2f20 322e 3029 202d 2067 616d 6d61  ) / 2.0) - gamma
-00003740: 6c6e 286e 7520 2f20 322e 3029 202d 2030  ln(nu / 2.0) - 0
-00003750: 2e35 202a 206b 202a 2070 742e 6c6f 6728  .5 * k * pt.log(
-00003760: 6e75 202a 206e 702e 7069 290a 2020 2020  nu * np.pi).    
-00003770: 2020 2020 696e 6e65 7220 3d20 2d28 6e75      inner = -(nu
-00003780: 202b 206b 2920 2f20 322e 3020 2a20 7074   + k) / 2.0 * pt
-00003790: 2e6c 6f67 3170 2871 7561 6464 6973 7420  .log1p(quaddist 
-000037a0: 2f20 6e75 290a 2020 2020 2020 2020 7265  / nu).        re
-000037b0: 7320 3d20 6e6f 726d 202b 2069 6e6e 6572  s = norm + inner
-000037c0: 202d 206c 6f67 6465 740a 0a20 2020 2020   - logdet..     
-000037d0: 2020 2072 6574 7572 6e20 6368 6563 6b5f     return check_
-000037e0: 7061 7261 6d65 7465 7273 2872 6573 2c20  parameters(res, 
-000037f0: 6f6b 2c20 6e75 203e 2030 2c20 6d73 673d  ok, nu > 0, msg=
-00003800: 2270 6f73 6465 662c 206e 7520 3e20 3022  "posdef, nu > 0"
-00003810: 290a 0a0a 636c 6173 7320 4469 7269 6368  )...class Dirich
-00003820: 6c65 7428 5369 6d70 6c65 7843 6f6e 7469  let(SimplexConti
-00003830: 6e75 6f75 7329 3a0a 2020 2020 7222 2222  nuous):.    r"""
-00003840: 0a20 2020 2044 6972 6963 686c 6574 206c  .    Dirichlet l
-00003850: 6f67 2d6c 696b 656c 6968 6f6f 642e 0a0a  og-likelihood...
-00003860: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
-00003870: 2020 2020 2020 6628 5c6d 6174 6862 667b        f(\mathbf{
-00003880: 787d 7c5c 6d61 7468 6266 7b61 7d29 203d  x}|\mathbf{a}) =
-00003890: 0a20 2020 2020 2020 2020 2020 5c66 7261  .           \fra
-000038a0: 637b 5c47 616d 6d61 285c 7375 6d5f 7b69  c{\Gamma(\sum_{i
-000038b0: 3d31 7d5e 6b20 615f 6929 7d7b 5c70 726f  =1}^k a_i)}{\pro
-000038c0: 645f 7b69 3d31 7d5e 6b20 5c47 616d 6d61  d_{i=1}^k \Gamma
-000038d0: 2861 5f69 297d 0a20 2020 2020 2020 2020  (a_i)}.         
-000038e0: 2020 5c70 726f 645f 7b69 3d31 7d5e 6b20    \prod_{i=1}^k 
-000038f0: 785f 695e 7b61 5f69 202d 2031 7d0a 0a20  x_i^{a_i - 1}.. 
-00003900: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
-00003910: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
-00003940: 2053 7570 706f 7274 2020 203a 6d61 7468   Support   :math
-00003950: 3a60 785f 6920 5c69 6e20 2830 2c20 3129  :`x_i \in (0, 1)
-00003960: 6020 666f 7220 3a6d 6174 683a 6069 205c  ` for :math:`i \
-00003970: 696e 205c 7b31 2c20 5c6c 646f 7473 2c20  in \{1, \ldots, 
-00003980: 4b5c 7d60 0a20 2020 2020 2020 2020 2020  K\}`.           
-00003990: 2020 2073 7563 6820 7468 6174 203a 6d61     such that :ma
-000039a0: 7468 3a60 5c73 756d 2078 5f69 203d 2031  th:`\sum x_i = 1
-000039b0: 600a 2020 2020 4d65 616e 2020 2020 2020  `.    Mean      
-000039c0: 3a6d 6174 683a 605c 6466 7261 637b 615f  :math:`\dfrac{a_
-000039d0: 697d 7b5c 7375 6d20 615f 697d 600a 2020  i}{\sum a_i}`.  
-000039e0: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
-000039f0: 683a 605c 6466 7261 637b 615f 6920 2d20  h:`\dfrac{a_i - 
-00003a00: 5c73 756d 2061 5f30 7d7b 615f 305e 3220  \sum a_0}{a_0^2 
-00003a10: 2861 5f30 202b 2031 297d 600a 2020 2020  (a_0 + 1)}`.    
-00003a20: 2020 2020 2020 2020 2020 7768 6572 6520            where 
-00003a30: 3a6d 6174 683a 6061 5f30 203d 205c 7375  :math:`a_0 = \su
-00003a40: 6d20 615f 6960 0a20 2020 203d 3d3d 3d3d  m a_i`.    =====
-00003a50: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
-00003a60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003a70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003a80: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
-00003a90: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00003aa0: 2d2d 2d0a 2020 2020 6120 3a20 7465 6e73  ---.    a : tens
-00003ab0: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-00003ac0: 0a20 2020 2020 2020 2043 6f6e 6365 6e74  .        Concent
-00003ad0: 7261 7469 6f6e 2070 6172 616d 6574 6572  ration parameter
-00003ae0: 7320 2861 203e 2030 292e 2054 6865 206e  s (a > 0). The n
-00003af0: 756d 6265 7220 6f66 2063 6174 6567 6f72  umber of categor
-00003b00: 6965 7320 6973 2067 6976 656e 2062 7920  ies is given by 
-00003b10: 7468 650a 2020 2020 2020 2020 6c65 6e67  the.        leng
-00003b20: 7468 206f 6620 7468 6520 6c61 7374 2061  th of the last a
-00003b30: 7869 732e 0a20 2020 2022 2222 0a20 2020  xis..    """.   
-00003b40: 2072 765f 6f70 203d 2064 6972 6963 686c   rv_op = dirichl
-00003b50: 6574 0a0a 2020 2020 4063 6c61 7373 6d65  et..    @classme
-00003b60: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
-00003b70: 7428 636c 732c 2061 2c20 2a2a 6b77 6172  t(cls, a, **kwar
-00003b80: 6773 293a 0a20 2020 2020 2020 2061 203d  gs):.        a =
-00003b90: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00003ba0: 7269 6162 6c65 2861 290a 2020 2020 2020  riable(a).      
-00003bb0: 2020 2320 6d65 616e 203d 2061 202f 2070    # mean = a / p
-00003bc0: 742e 7375 6d28 6129 0a20 2020 2020 2020  t.sum(a).       
-00003bd0: 2023 206d 6f64 6520 3d20 7074 2e73 7769   # mode = pt.swi
-00003be0: 7463 6828 7074 2e61 6c6c 2861 203e 2031  tch(pt.all(a > 1
-00003bf0: 292c 2028 6120 2d20 3129 202f 2070 742e  ), (a - 1) / pt.
-00003c00: 7375 6d28 6120 2d20 3129 2c20 6e70 2e6e  sum(a - 1), np.n
-00003c10: 616e 290a 0a20 2020 2020 2020 2072 6574  an)..        ret
-00003c20: 7572 6e20 7375 7065 7228 292e 6469 7374  urn super().dist
-00003c30: 285b 615d 2c20 2a2a 6b77 6172 6773 290a  ([a], **kwargs).
-00003c40: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
-00003c50: 7276 2c20 7369 7a65 2c20 6129 3a0a 2020  rv, size, a):.  
-00003c60: 2020 2020 2020 6e6f 726d 5f63 6f6e 7374        norm_const
-00003c70: 616e 7420 3d20 7074 2e73 756d 2861 2c20  ant = pt.sum(a, 
-00003c80: 6178 6973 3d2d 3129 5b2e 2e2e 2c20 4e6f  axis=-1)[..., No
-00003c90: 6e65 5d0a 2020 2020 2020 2020 6d6f 6d65  ne].        mome
-00003ca0: 6e74 203d 2061 202f 206e 6f72 6d5f 636f  nt = a / norm_co
-00003cb0: 6e73 7461 6e74 0a20 2020 2020 2020 2069  nstant.        i
-00003cc0: 6620 6e6f 7420 7276 5f73 697a 655f 6973  f not rv_size_is
-00003cd0: 5f6e 6f6e 6528 7369 7a65 293a 0a20 2020  _none(size):.   
-00003ce0: 2020 2020 2020 2020 206d 6f6d 656e 7420           moment 
-00003cf0: 3d20 7074 2e66 756c 6c28 7074 2e63 6f6e  = pt.full(pt.con
-00003d00: 6361 7465 6e61 7465 285b 7369 7a65 2c20  catenate([size, 
-00003d10: 5b61 2e73 6861 7065 5b2d 315d 5d5d 292c  [a.shape[-1]]]),
-00003d20: 206d 6f6d 656e 7429 0a20 2020 2020 2020   moment).       
-00003d30: 2072 6574 7572 6e20 6d6f 6d65 6e74 0a0a   return moment..
-00003d40: 2020 2020 6465 6620 6c6f 6770 2876 616c      def logp(val
-00003d50: 7565 2c20 6129 3a0a 2020 2020 2020 2020  ue, a):.        
-00003d60: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
-00003d70: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
-00003d80: 696c 6974 7920 6f66 2044 6972 6963 686c  ility of Dirichl
-00003d90: 6574 2064 6973 7472 6962 7574 696f 6e0a  et distribution.
-00003da0: 2020 2020 2020 2020 6174 2073 7065 6369          at speci
-00003db0: 6669 6564 2076 616c 7565 2e0a 0a20 2020  fied value...   
-00003dc0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00003dd0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00003de0: 2d2d 0a20 2020 2020 2020 2076 616c 7565  --.        value
-00003df0: 3a20 6e75 6d65 7269 630a 2020 2020 2020  : numeric.      
-00003e00: 2020 2020 2020 5661 6c75 6520 666f 7220        Value for 
-00003e10: 7768 6963 6820 6c6f 672d 7072 6f62 6162  which log-probab
-00003e20: 696c 6974 7920 6973 2063 616c 6375 6c61  ility is calcula
-00003e30: 7465 642e 0a0a 2020 2020 2020 2020 5265  ted...        Re
-00003e40: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00003e50: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5465  -----.        Te
-00003e60: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
-00003e70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003e80: 2023 206f 6e6c 7920 6465 6669 6e65 6420   # only defined 
-00003e90: 666f 7220 7375 6d28 7661 6c75 6529 203d  for sum(value) =
-00003ea0: 3d20 310a 2020 2020 2020 2020 7265 7320  = 1.        res 
-00003eb0: 3d20 7074 2e73 756d 286c 6f67 706f 7728  = pt.sum(logpow(
-00003ec0: 7661 6c75 652c 2061 202d 2031 2920 2d20  value, a - 1) - 
-00003ed0: 6761 6d6d 616c 6e28 6129 2c20 6178 6973  gammaln(a), axis
-00003ee0: 3d2d 3129 202b 2067 616d 6d61 6c6e 2870  =-1) + gammaln(p
-00003ef0: 742e 7375 6d28 612c 2061 7869 733d 2d31  t.sum(a, axis=-1
-00003f00: 2929 0a20 2020 2020 2020 2072 6573 203d  )).        res =
-00003f10: 2070 742e 7377 6974 6368 280a 2020 2020   pt.switch(.    
-00003f20: 2020 2020 2020 2020 7074 2e6f 725f 280a          pt.or_(.
-00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f40: 7074 2e61 6e79 2870 742e 6c74 2876 616c  pt.any(pt.lt(val
-00003f50: 7565 2c20 3029 2c20 6178 6973 3d2d 3129  ue, 0), axis=-1)
-00003f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003f70: 2020 7074 2e61 6e79 2870 742e 6774 2876    pt.any(pt.gt(v
-00003f80: 616c 7565 2c20 3129 2c20 6178 6973 3d2d  alue, 1), axis=-
-00003f90: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
-00003fa0: 292c 0a20 2020 2020 2020 2020 2020 202d  ),.            -
-00003fb0: 6e70 2e69 6e66 2c0a 2020 2020 2020 2020  np.inf,.        
-00003fc0: 2020 2020 7265 732c 0a20 2020 2020 2020      res,.       
-00003fd0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00003fe0: 6e20 6368 6563 6b5f 7061 7261 6d65 7465  n check_paramete
-00003ff0: 7273 280a 2020 2020 2020 2020 2020 2020  rs(.            
-00004000: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
-00004010: 2061 203e 2030 2c0a 2020 2020 2020 2020   a > 0,.        
-00004020: 2020 2020 6d73 673d 2261 203e 2030 222c      msg="a > 0",
-00004030: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
-00004040: 7373 204d 756c 7469 6e6f 6d69 616c 2844  ss Multinomial(D
-00004050: 6973 6372 6574 6529 3a0a 2020 2020 7222  iscrete):.    r"
-00004060: 2222 0a20 2020 204d 756c 7469 6e6f 6d69  "".    Multinomi
-00004070: 616c 206c 6f67 2d6c 696b 656c 6968 6f6f  al log-likelihoo
-00004080: 642e 0a0a 2020 2020 4765 6e65 7261 6c69  d...    Generali
-00004090: 7a65 7320 6269 6e6f 6d69 616c 2064 6973  zes binomial dis
-000040a0: 7472 6962 7574 696f 6e2c 2062 7574 2069  tribution, but i
-000040b0: 6e73 7465 6164 206f 6620 6561 6368 2074  nstead of each t
-000040c0: 7269 616c 2072 6573 756c 7469 6e67 0a20  rial resulting. 
-000040d0: 2020 2069 6e20 2273 7563 6365 7373 2220     in "success" 
-000040e0: 6f72 2022 6661 696c 7572 6522 2c20 6561  or "failure", ea
-000040f0: 6368 206f 6e65 2072 6573 756c 7473 2069  ch one results i
-00004100: 6e20 6578 6163 746c 7920 6f6e 6520 6f66  n exactly one of
-00004110: 2073 6f6d 650a 2020 2020 6669 7865 6420   some.    fixed 
-00004120: 6669 6e69 7465 206e 756d 6265 7220 6b20  finite number k 
-00004130: 6f66 2070 6f73 7369 626c 6520 6f75 7463  of possible outc
-00004140: 6f6d 6573 206f 7665 7220 6e20 696e 6465  omes over n inde
-00004150: 7065 6e64 656e 7420 7472 6961 6c73 2e0a  pendent trials..
-00004160: 2020 2020 2778 5b69 5d27 2069 6e64 6963      'x[i]' indic
-00004170: 6174 6573 2074 6865 206e 756d 6265 7220  ates the number 
-00004180: 6f66 2074 696d 6573 206f 7574 636f 6d65  of times outcome
-00004190: 206e 756d 6265 7220 6920 7761 7320 6f62   number i was ob
-000041a0: 7365 7276 6564 0a20 2020 206f 7665 7220  served.    over 
-000041b0: 7468 6520 6e20 7472 6961 6c73 2e0a 0a20  the n trials... 
-000041c0: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
-000041d0: 2020 2020 2066 2878 205c 6d69 6420 6e2c       f(x \mid n,
-000041e0: 2070 2920 3d20 5c66 7261 637b 6e21 7d7b   p) = \frac{n!}{
-000041f0: 5c70 726f 645f 7b69 3d31 7d5e 6b20 785f  \prod_{i=1}^k x_
-00004200: 6921 7d20 5c70 726f 645f 7b69 3d31 7d5e  i!} \prod_{i=1}^
-00004210: 6b20 705f 695e 7b78 5f69 7d0a 0a20 2020  k p_i^{x_i}..   
-00004220: 203d 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d   ==========  ===
-00004230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004250: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053 7570  ========.    Sup
-00004260: 706f 7274 2020 2020 203a 6d61 7468 3a60  port     :math:`
-00004270: 7820 5c69 6e20 5c7b 302c 2031 2c20 5c6c  x \in \{0, 1, \l
-00004280: 646f 7473 2c20 6e5c 7d60 2073 7563 6820  dots, n\}` such 
-00004290: 7468 6174 0a20 2020 2020 2020 2020 2020  that.           
-000042a0: 2020 2020 203a 6d61 7468 3a60 5c73 756d       :math:`\sum
-000042b0: 2078 5f69 203d 206e 600a 2020 2020 4d65   x_i = n`.    Me
-000042c0: 616e 2020 2020 2020 2020 3a6d 6174 683a  an        :math:
-000042d0: 606e 2070 5f69 600a 2020 2020 5661 7269  `n p_i`.    Vari
-000042e0: 616e 6365 2020 2020 3a6d 6174 683a 606e  ance    :math:`n
-000042f0: 2070 5f69 2028 3120 2d20 705f 6929 600a   p_i (1 - p_i)`.
-00004300: 2020 2020 436f 7661 7269 616e 6365 2020      Covariance  
-00004310: 3a6d 6174 683a 602d 6e20 705f 6920 705f  :math:`-n p_i p_
-00004320: 6a60 2066 6f72 203a 6d61 7468 3a60 6920  j` for :math:`i 
-00004330: 5c6e 6520 6a60 0a20 2020 203d 3d3d 3d3d  \ne j`.    =====
-00004340: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
-00004350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004370: 3d3d 0a0a 2020 2020 5061 7261 6d65 7465  ==..    Paramete
-00004380: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00004390: 2d0a 2020 2020 6e20 3a20 7465 6e73 6f72  -.    n : tensor
-000043a0: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
-000043b0: 2020 2020 2054 6f74 616c 2063 6f75 6e74       Total count
-000043c0: 7320 696e 2065 6163 6820 7265 706c 6963  s in each replic
-000043d0: 6174 6520 286e 203e 2030 292e 0a20 2020  ate (n > 0)..   
-000043e0: 2070 203a 2074 656e 736f 725f 6c69 6b65   p : tensor_like
-000043f0: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
-00004400: 2020 5072 6f62 6162 696c 6974 7920 6f66    Probability of
-00004410: 2065 6163 6820 6f6e 6520 6f66 2074 6865   each one of the
-00004420: 2064 6966 6665 7265 6e74 206f 7574 636f   different outco
-00004430: 6d65 7320 2830 203c 3d20 7020 3c3d 2031  mes (0 <= p <= 1
-00004440: 292e 2054 6865 206e 756d 6265 7220 6f66  ). The number of
-00004450: 0a20 2020 2020 2020 2063 6174 6567 6f72  .        categor
-00004460: 6965 7320 6973 2067 6976 656e 2062 7920  ies is given by 
-00004470: 7468 6520 6c65 6e67 7468 206f 6620 7468  the length of th
-00004480: 6520 6c61 7374 2061 7869 732e 2045 6c65  e last axis. Ele
-00004490: 6d65 6e74 7320 6172 6520 6578 7065 6374  ments are expect
-000044a0: 6564 2074 6f20 7375 6d0a 2020 2020 2020  ed to sum.      
-000044b0: 2020 746f 2031 2061 6c6f 6e67 2074 6865    to 1 along the
-000044c0: 206c 6173 7420 6178 6973 2e0a 2020 2020   last axis..    
-000044d0: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
-000044e0: 6d75 6c74 696e 6f6d 6961 6c0a 0a20 2020  multinomial..   
-000044f0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00004500: 2020 6465 6620 6469 7374 2863 6c73 2c20    def dist(cls, 
-00004510: 6e2c 2070 2c20 2a61 7267 732c 202a 2a6b  n, p, *args, **k
-00004520: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00004530: 7020 3d20 7074 2e61 735f 7465 6e73 6f72  p = pt.as_tensor
-00004540: 5f76 6172 6961 626c 6528 7029 0a20 2020  _variable(p).   
-00004550: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00004560: 6365 2870 2c20 5465 6e73 6f72 436f 6e73  ce(p, TensorCons
-00004570: 7461 6e74 293a 0a20 2020 2020 2020 2020  tant):.         
-00004580: 2020 2070 5f20 3d20 6e70 2e61 7361 7272     p_ = np.asarr
-00004590: 6179 2870 2e64 6174 6129 0a20 2020 2020  ay(p.data).     
-000045a0: 2020 2020 2020 2069 6620 6e70 2e61 6e79         if np.any
-000045b0: 2870 5f20 3c20 3029 3a0a 2020 2020 2020  (p_ < 0):.      
-000045c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000045d0: 5661 6c75 6545 7272 6f72 2866 224e 6567  ValueError(f"Neg
-000045e0: 6174 6976 6520 6070 6020 7061 7261 6d65  ative `p` parame
-000045f0: 7465 7273 2061 7265 206e 6f74 2076 616c  ters are not val
-00004600: 6964 2c20 676f 743a 207b 705f 7d22 290a  id, got: {p_}").
-00004610: 2020 2020 2020 2020 2020 2020 705f 7375              p_su
-00004620: 6d5f 203d 206e 702e 7375 6d28 5b70 5f5d  m_ = np.sum([p_]
-00004630: 2c20 6178 6973 3d2d 3129 0a20 2020 2020  , axis=-1).     
-00004640: 2020 2020 2020 2069 6620 6e6f 7420 6e70         if not np
-00004650: 2e61 6c6c 286e 702e 6973 636c 6f73 6528  .all(np.isclose(
-00004660: 705f 7375 6d5f 2c20 312e 3029 293a 0a20  p_sum_, 1.0)):. 
-00004670: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004680: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
-00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046a0: 2020 6622 6070 6020 7061 7261 6d65 7465    f"`p` paramete
-000046b0: 7273 2073 756d 2074 6f20 7b70 5f73 756d  rs sum to {p_sum
-000046c0: 5f7d 2c20 696e 7374 6561 6420 6f66 2031  _}, instead of 1
-000046d0: 2e30 2e20 220a 2020 2020 2020 2020 2020  .0. ".          
-000046e0: 2020 2020 2020 2020 2020 2254 6865 7920            "They 
-000046f0: 7769 6c6c 2062 6520 6175 746f 6d61 7469  will be automati
-00004700: 6361 6c6c 7920 7265 7363 616c 6564 2e20  cally rescaled. 
-00004710: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004720: 2020 2020 2020 2259 6f75 2063 616e 2072        "You can r
-00004730: 6573 6361 6c65 2074 6865 6d20 6469 7265  escale them dire
-00004740: 6374 6c79 2074 6f20 6765 7420 7269 6420  ctly to get rid 
-00004750: 6f66 2074 6869 7320 7761 726e 696e 672e  of this warning.
-00004760: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004770: 2020 2020 2020 2055 7365 7257 6172 6e69         UserWarni
-00004780: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-00004790: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000047a0: 2020 2020 2020 705f 203d 2070 5f20 2f20        p_ = p_ / 
-000047b0: 7074 2e73 756d 2870 5f2c 2061 7869 733d  pt.sum(p_, axis=
-000047c0: 2d31 2c20 6b65 6570 6469 6d73 3d54 7275  -1, keepdims=Tru
-000047d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-000047e0: 2020 2070 203d 2070 742e 6173 5f74 656e     p = pt.as_ten
-000047f0: 736f 725f 7661 7269 6162 6c65 2870 5f29  sor_variable(p_)
-00004800: 0a20 2020 2020 2020 206e 203d 2070 742e  .        n = pt.
-00004810: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-00004820: 6c65 286e 290a 2020 2020 2020 2020 7020  le(n).        p 
-00004830: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00004840: 6172 6961 626c 6528 7029 0a20 2020 2020  ariable(p).     
-00004850: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-00004860: 292e 6469 7374 285b 6e2c 2070 5d2c 202a  ).dist([n, p], *
-00004870: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-00004880: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
-00004890: 7276 2c20 7369 7a65 2c20 6e2c 2070 293a  rv, size, n, p):
-000048a0: 0a20 2020 2020 2020 206e 203d 2070 742e  .        n = pt.
-000048b0: 7368 6170 655f 7061 6472 6967 6874 286e  shape_padright(n
-000048c0: 290a 2020 2020 2020 2020 6d6f 6465 203d  ).        mode =
-000048d0: 2070 742e 726f 756e 6428 6e20 2a20 7029   pt.round(n * p)
-000048e0: 0a20 2020 2020 2020 2064 6966 6620 3d20  .        diff = 
-000048f0: 6e20 2d20 7074 2e73 756d 286d 6f64 652c  n - pt.sum(mode,
-00004900: 2061 7869 733d 2d31 2c20 6b65 6570 6469   axis=-1, keepdi
-00004910: 6d73 3d54 7275 6529 0a20 2020 2020 2020  ms=True).       
-00004920: 2069 6e63 5f62 6f6f 6c5f 6172 7220 3d20   inc_bool_arr = 
-00004930: 7074 2e61 6273 2864 6966 6629 203e 2030  pt.abs(diff) > 0
-00004940: 0a20 2020 2020 2020 206d 6f64 6520 3d20  .        mode = 
-00004950: 7074 2e69 6e63 5f73 7562 7465 6e73 6f72  pt.inc_subtensor
-00004960: 286d 6f64 655b 696e 635f 626f 6f6c 5f61  (mode[inc_bool_a
-00004970: 7272 2e6e 6f6e 7a65 726f 2829 5d2c 2064  rr.nonzero()], d
-00004980: 6966 665b 696e 635f 626f 6f6c 5f61 7272  iff[inc_bool_arr
-00004990: 2e6e 6f6e 7a65 726f 2829 5d29 0a20 2020  .nonzero()]).   
-000049a0: 2020 2020 2069 6620 6e6f 7420 7276 5f73       if not rv_s
-000049b0: 697a 655f 6973 5f6e 6f6e 6528 7369 7a65  ize_is_none(size
-000049c0: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
-000049d0: 7574 7075 745f 7369 7a65 203d 2070 742e  utput_size = pt.
-000049e0: 636f 6e63 6174 656e 6174 6528 5b73 697a  concatenate([siz
-000049f0: 652c 205b 702e 7368 6170 655b 2d31 5d5d  e, [p.shape[-1]]
-00004a00: 5d29 0a20 2020 2020 2020 2020 2020 206d  ]).            m
-00004a10: 6f64 6520 3d20 7074 2e66 756c 6c28 6f75  ode = pt.full(ou
-00004a20: 7470 7574 5f73 697a 652c 206d 6f64 6529  tput_size, mode)
-00004a30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004a40: 6d6f 6465 0a0a 2020 2020 6465 6620 6c6f  mode..    def lo
-00004a50: 6770 2876 616c 7565 2c20 6e2c 2070 293a  gp(value, n, p):
-00004a60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004a70: 2020 2020 2043 616c 6375 6c61 7465 206c       Calculate l
-00004a80: 6f67 2d70 726f 6261 6269 6c69 7479 206f  og-probability o
-00004a90: 6620 4d75 6c74 696e 6f6d 6961 6c20 6469  f Multinomial di
-00004aa0: 7374 7269 6275 7469 6f6e 0a20 2020 2020  stribution.     
-00004ab0: 2020 2061 7420 7370 6563 6966 6965 6420     at specified 
-00004ac0: 7661 6c75 652e 0a0a 2020 2020 2020 2020  value...        
-00004ad0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00004ae0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00004af0: 2020 2020 2020 7661 6c75 653a 206e 756d        value: num
-00004b00: 6572 6963 0a20 2020 2020 2020 2020 2020  eric.           
-00004b10: 2056 616c 7565 2066 6f72 2077 6869 6368   Value for which
-00004b20: 206c 6f67 2d70 726f 6261 6269 6c69 7479   log-probability
-00004b30: 2069 7320 6361 6c63 756c 6174 6564 2e0a   is calculated..
-00004b40: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004b50: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00004b60: 0a20 2020 2020 2020 2054 656e 736f 7256  .        TensorV
-00004b70: 6172 6961 626c 650a 2020 2020 2020 2020  ariable.        
-00004b80: 2222 220a 0a20 2020 2020 2020 2072 6573  """..        res
-00004b90: 203d 2066 6163 746c 6e28 6e29 202b 2070   = factln(n) + p
-00004ba0: 742e 7375 6d28 2d66 6163 746c 6e28 7661  t.sum(-factln(va
-00004bb0: 6c75 6529 202b 206c 6f67 706f 7728 702c  lue) + logpow(p,
-00004bc0: 2076 616c 7565 292c 2061 7869 733d 2d31   value), axis=-1
-00004bd0: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
-00004be0: 7074 2e73 7769 7463 6828 0a20 2020 2020  pt.switch(.     
-00004bf0: 2020 2020 2020 2070 742e 6f72 5f28 7074         pt.or_(pt
-00004c00: 2e61 6e79 2870 742e 6c74 2876 616c 7565  .any(pt.lt(value
-00004c10: 2c20 3029 2c20 6178 6973 3d2d 3129 2c20  , 0), axis=-1), 
-00004c20: 7074 2e6e 6571 2870 742e 7375 6d28 7661  pt.neq(pt.sum(va
-00004c30: 6c75 652c 2061 7869 733d 2d31 292c 206e  lue, axis=-1), n
-00004c40: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00004c50: 2d6e 702e 696e 662c 0a20 2020 2020 2020  -np.inf,.       
-00004c60: 2020 2020 2072 6573 2c0a 2020 2020 2020       res,.      
-00004c70: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
-00004c80: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
-00004c90: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
-00004ca0: 2072 6573 2c0a 2020 2020 2020 2020 2020   res,.          
-00004cb0: 2020 3020 3c3d 2070 2c0a 2020 2020 2020    0 <= p,.      
-00004cc0: 2020 2020 2020 7020 3c3d 2031 2c0a 2020        p <= 1,.  
-00004cd0: 2020 2020 2020 2020 2020 7074 2e69 7363            pt.isc
-00004ce0: 6c6f 7365 2870 742e 7375 6d28 702c 2061  lose(pt.sum(p, a
-00004cf0: 7869 733d 2d31 292c 2031 292c 0a20 2020  xis=-1), 1),.   
-00004d00: 2020 2020 2020 2020 2070 742e 6765 286e           pt.ge(n
-00004d10: 2c20 3029 2c0a 2020 2020 2020 2020 2020  , 0),.          
-00004d20: 2020 6d73 673d 2230 203c 3d20 7020 3c3d    msg="0 <= p <=
-00004d30: 2031 2c20 7375 6d28 7029 203d 2031 2c20   1, sum(p) = 1, 
-00004d40: 6e20 3e3d 2030 222c 0a20 2020 2020 2020  n >= 0",.       
-00004d50: 2029 0a0a 0a63 6c61 7373 2044 6972 6963   )...class Diric
-00004d60: 686c 6574 4d75 6c74 696e 6f6d 6961 6c52  hletMultinomialR
-00004d70: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
-00004d80: 293a 0a20 2020 206e 616d 6520 3d20 2264  ):.    name = "d
-00004d90: 6972 6963 686c 6574 5f6d 756c 7469 6e6f  irichlet_multino
-00004da0: 6d69 616c 220a 2020 2020 6e64 696d 5f73  mial".    ndim_s
-00004db0: 7570 7020 3d20 310a 2020 2020 6e64 696d  upp = 1.    ndim
-00004dc0: 735f 7061 7261 6d73 203d 205b 302c 2031  s_params = [0, 1
-00004dd0: 5d0a 2020 2020 6474 7970 6520 3d20 2269  ].    dtype = "i
-00004de0: 6e74 3634 220a 2020 2020 5f70 7269 6e74  nt64".    _print
-00004df0: 5f6e 616d 6520 3d20 2822 4469 7269 6368  _name = ("Dirich
-00004e00: 6c65 744d 4e22 2c20 225c 5c6f 7065 7261  letMN", "\\opera
-00004e10: 746f 726e 616d 657b 4469 7269 6368 6c65  torname{Dirichle
-00004e20: 744d 4e7d 2229 0a0a 2020 2020 6465 6620  tMN}")..    def 
-00004e30: 5f73 7570 705f 7368 6170 655f 6672 6f6d  _supp_shape_from
-00004e40: 5f70 6172 616d 7328 7365 6c66 2c20 6469  _params(self, di
-00004e50: 7374 5f70 6172 616d 732c 2072 6570 5f70  st_params, rep_p
-00004e60: 6172 616d 5f69 6478 3d31 2c20 7061 7261  aram_idx=1, para
-00004e70: 6d5f 7368 6170 6573 3d4e 6f6e 6529 3a0a  m_shapes=None):.
-00004e80: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00004e90: 6566 6175 6c74 5f73 7570 705f 7368 6170  efault_supp_shap
-00004ea0: 655f 6672 6f6d 5f70 6172 616d 7328 0a20  e_from_params(. 
-00004eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004ec0: 6e64 696d 5f73 7570 702c 2064 6973 745f  ndim_supp, dist_
-00004ed0: 7061 7261 6d73 2c20 7265 705f 7061 7261  params, rep_para
-00004ee0: 6d5f 6964 782c 2070 6172 616d 5f73 6861  m_idx, param_sha
-00004ef0: 7065 730a 2020 2020 2020 2020 290a 0a20  pes.        ).. 
-00004f00: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00004f10: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
-00004f20: 6c73 2c20 726e 672c 206e 2c20 612c 2073  ls, rng, n, a, s
-00004f30: 697a 6529 3a0a 2020 2020 2020 2020 6966  ize):.        if
-00004f40: 206e 2e6e 6469 6d20 3e20 3020 6f72 2061   n.ndim > 0 or a
-00004f50: 2e6e 6469 6d20 3e20 313a 0a20 2020 2020  .ndim > 1:.     
-00004f60: 2020 2020 2020 206e 2c20 6120 3d20 6272         n, a = br
-00004f70: 6f61 6463 6173 745f 7061 7261 6d73 285b  oadcast_params([
-00004f80: 6e2c 2061 5d2c 2063 6c73 2e6e 6469 6d73  n, a], cls.ndims
-00004f90: 5f70 6172 616d 7329 0a20 2020 2020 2020  _params).       
-00004fa0: 2020 2020 2073 697a 6520 3d20 7475 706c       size = tupl
-00004fb0: 6528 7369 7a65 206f 7220 2829 290a 0a20  e(size or ()).. 
-00004fc0: 2020 2020 2020 2020 2020 2069 6620 7369             if si
-00004fd0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
-00004fe0: 2020 2020 6e20 3d20 6e70 2e62 726f 6164      n = np.broad
-00004ff0: 6361 7374 5f74 6f28 6e2c 2073 697a 6529  cast_to(n, size)
-00005000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005010: 2061 203d 206e 702e 6272 6f61 6463 6173   a = np.broadcas
-00005020: 745f 746f 2861 2c20 7369 7a65 202b 2028  t_to(a, size + (
-00005030: 612e 7368 6170 655b 2d31 5d2c 2929 0a0a  a.shape[-1],))..
-00005040: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00005050: 3d20 6e70 2e65 6d70 7479 2861 2e73 6861  = np.empty(a.sha
-00005060: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
-00005070: 666f 7220 6964 7820 696e 206e 702e 6e64  for idx in np.nd
-00005080: 696e 6465 7828 612e 7368 6170 655b 3a2d  index(a.shape[:-
-00005090: 315d 293a 0a20 2020 2020 2020 2020 2020  1]):.           
-000050a0: 2020 2020 2070 203d 2072 6e67 2e64 6972       p = rng.dir
-000050b0: 6963 686c 6574 2861 5b69 6478 5d29 0a20  ichlet(a[idx]). 
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000050d0: 6573 5b69 6478 5d20 3d20 726e 672e 6d75  es[idx] = rng.mu
-000050e0: 6c74 696e 6f6d 6961 6c28 6e5b 6964 785d  ltinomial(n[idx]
-000050f0: 2c20 7029 0a20 2020 2020 2020 2020 2020  , p).           
-00005100: 2072 6574 7572 6e20 7265 730a 2020 2020   return res.    
-00005110: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005120: 2020 2020 2020 2320 6e20 6973 2061 2073        # n is a s
-00005130: 6361 6c61 722c 2061 2069 7320 6120 3164  calar, a is a 1d
-00005140: 2061 7272 6179 0a20 2020 2020 2020 2020   array.         
-00005150: 2020 2070 203d 2072 6e67 2e64 6972 6963     p = rng.diric
-00005160: 686c 6574 2861 2c20 7369 7a65 3d73 697a  hlet(a, size=siz
-00005170: 6529 2020 2320 2873 697a 652c 2061 2e73  e)  # (size, a.s
-00005180: 6861 7065 290a 0a20 2020 2020 2020 2020  hape)..         
-00005190: 2020 2072 6573 203d 206e 702e 656d 7074     res = np.empt
-000051a0: 7928 702e 7368 6170 6529 0a20 2020 2020  y(p.shape).     
-000051b0: 2020 2020 2020 2066 6f72 2069 6478 2069         for idx i
-000051c0: 6e20 6e70 2e6e 6469 6e64 6578 2870 2e73  n np.ndindex(p.s
-000051d0: 6861 7065 5b3a 2d31 5d29 3a0a 2020 2020  hape[:-1]):.    
-000051e0: 2020 2020 2020 2020 2020 2020 7265 735b              res[
-000051f0: 6964 785d 203d 2072 6e67 2e6d 756c 7469  idx] = rng.multi
-00005200: 6e6f 6d69 616c 286e 2c20 705b 6964 785d  nomial(n, p[idx]
-00005210: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00005220: 6574 7572 6e20 7265 730a 0a0a 6469 7269  eturn res...diri
-00005230: 6368 6c65 745f 6d75 6c74 696e 6f6d 6961  chlet_multinomia
-00005240: 6c20 3d20 4469 7269 6368 6c65 744d 756c  l = DirichletMul
-00005250: 7469 6e6f 6d69 616c 5256 2829 0a0a 0a63  tinomialRV()...c
-00005260: 6c61 7373 2044 6972 6963 686c 6574 4d75  lass DirichletMu
-00005270: 6c74 696e 6f6d 6961 6c28 4469 7363 7265  ltinomial(Discre
-00005280: 7465 293a 0a20 2020 2072 2222 2244 6972  te):.    r"""Dir
-00005290: 6963 686c 6574 204d 756c 7469 6e6f 6d69  ichlet Multinomi
-000052a0: 616c 206c 6f67 2d6c 696b 656c 6968 6f6f  al log-likelihoo
-000052b0: 642e 0a0a 2020 2020 4469 7269 6368 6c65  d...    Dirichle
-000052c0: 7420 6d69 7874 7572 6520 6f66 204d 756c  t mixture of Mul
-000052d0: 7469 6e6f 6d69 616c 7320 6469 7374 7269  tinomials distri
-000052e0: 6275 7469 6f6e 2c20 7769 7468 2061 206d  bution, with a m
-000052f0: 6172 6769 6e61 6c69 7a65 6420 504d 462e  arginalized PMF.
-00005300: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
-00005310: 0a20 2020 2020 2020 2066 2878 205c 6d69  .        f(x \mi
-00005320: 6420 6e2c 2061 2920 3d20 5c66 7261 637b  d n, a) = \frac{
-00005330: 5c47 616d 6d61 286e 202b 2031 295c 4761  \Gamma(n + 1)\Ga
-00005340: 6d6d 6128 5c73 756d 2061 5f6b 297d 0a20  mma(\sum a_k)}. 
-00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005360: 2020 2020 2020 2020 2020 2020 207b 5c47               {\G
-00005370: 616d 6d61 286e 202b 205c 7375 6d20 615f  amma(n + \sum a_
-00005380: 6b29 7d0a 2020 2020 2020 2020 2020 2020  k)}.            
-00005390: 2020 2020 2020 2020 2020 2020 205c 7072               \pr
-000053a0: 6f64 5f7b 6b3d 317d 5e4b 0a20 2020 2020  od_{k=1}^K.     
-000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053c0: 2020 2020 5c66 7261 637b 5c47 616d 6d61      \frac{\Gamma
-000053d0: 2878 5f6b 202b 2020 615f 6b29 7d0a 2020  (x_k +  a_k)}.  
-000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053f0: 2020 2020 2020 2020 2020 2020 7b5c 4761              {\Ga
-00005400: 6d6d 6128 785f 6b20 2b20 3129 5c47 616d  mma(x_k + 1)\Gam
-00005410: 6d61 2861 5f6b 297d 0a0a 2020 2020 3d3d  ma(a_k)}..    ==
-00005420: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-00005430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005450: 3d3d 3d3d 3d0a 2020 2020 5375 7070 6f72  =====.    Suppor
-00005460: 7420 2020 2020 3a6d 6174 683a 6078 205c  t     :math:`x \
-00005470: 696e 205c 7b30 2c20 312c 205c 6c64 6f74  in \{0, 1, \ldot
-00005480: 732c 206e 5c7d 6020 7375 6368 2074 6861  s, n\}` such tha
-00005490: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000054a0: 2020 3a6d 6174 683a 605c 7375 6d20 785f    :math:`\sum x_
-000054b0: 6920 3d20 6e60 0a20 2020 204d 6561 6e20  i = n`.    Mean 
-000054c0: 2020 2020 2020 203a 6d61 7468 3a60 6e20         :math:`n 
-000054d0: 5c66 7261 637b 615f 697d 7b5c 7375 6d7b  \frac{a_i}{\sum{
-000054e0: 615f 6b7d 7d60 0a20 2020 203d 3d3d 3d3d  a_k}}`.    =====
-000054f0: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
-00005500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005520: 3d3d 0a0a 2020 2020 5061 7261 6d65 7465  ==..    Paramete
-00005530: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00005540: 2d0a 2020 2020 6e20 3a20 7465 6e73 6f72  -.    n : tensor
-00005550: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
-00005560: 2020 2020 2054 6f74 616c 2063 6f75 6e74       Total count
-00005570: 7320 696e 2065 6163 6820 7265 706c 6963  s in each replic
-00005580: 6174 6520 286e 203e 2030 292e 0a0a 2020  ate (n > 0)...  
-00005590: 2020 6120 3a20 7465 6e73 6f72 5f6c 696b    a : tensor_lik
-000055a0: 6520 6f66 2066 6c6f 6174 0a20 2020 2020  e of float.     
-000055b0: 2020 2044 6972 6963 686c 6574 2063 6f6e     Dirichlet con
-000055c0: 6365 6e74 7261 7469 6f6e 2070 6172 616d  centration param
-000055d0: 6574 6572 7320 2861 203e 2030 292e 2054  eters (a > 0). T
-000055e0: 6865 206e 756d 6265 7220 6f66 2063 6174  he number of cat
-000055f0: 6567 6f72 6965 7320 6973 2067 6976 656e  egories is given
-00005600: 2062 790a 2020 2020 2020 2020 7468 6520   by.        the 
-00005610: 6c65 6e67 7468 206f 6620 7468 6520 6c61  length of the la
-00005620: 7374 2061 7869 732e 0a20 2020 2022 2222  st axis..    """
-00005630: 0a20 2020 2072 765f 6f70 203d 2064 6972  .    rv_op = dir
-00005640: 6963 686c 6574 5f6d 756c 7469 6e6f 6d69  ichlet_multinomi
-00005650: 616c 0a0a 2020 2020 4063 6c61 7373 6d65  al..    @classme
-00005660: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
-00005670: 7428 636c 732c 206e 2c20 612c 202a 6172  t(cls, n, a, *ar
-00005680: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-00005690: 2020 2020 2020 206e 203d 2069 6e74 5828         n = intX(
-000056a0: 6e29 0a20 2020 2020 2020 2061 203d 2066  n).        a = f
-000056b0: 6c6f 6174 5828 6129 0a0a 2020 2020 2020  loatX(a)..      
-000056c0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-000056d0: 2e64 6973 7428 5b6e 2c20 615d 2c20 2a2a  .dist([n, a], **
-000056e0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-000056f0: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
-00005700: 2c20 6e2c 2061 293a 0a20 2020 2020 2020  , n, a):.       
-00005710: 2070 203d 2061 202f 2070 742e 7375 6d28   p = a / pt.sum(
-00005720: 612c 2061 7869 733d 2d31 2c20 6b65 6570  a, axis=-1, keep
-00005730: 6469 6d73 3d54 7275 6529 0a20 2020 2020  dims=True).     
-00005740: 2020 2072 6574 7572 6e20 6d6f 6d65 6e74     return moment
-00005750: 284d 756c 7469 6e6f 6d69 616c 2e64 6973  (Multinomial.dis
-00005760: 7428 6e3d 6e2c 2070 3d70 2c20 7369 7a65  t(n=n, p=p, size
-00005770: 3d73 697a 6529 290a 0a20 2020 2064 6566  =size))..    def
-00005780: 206c 6f67 7028 7661 6c75 652c 206e 2c20   logp(value, n, 
-00005790: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
-000057a0: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-000057b0: 6520 6c6f 672d 7072 6f62 6162 696c 6974  e log-probabilit
-000057c0: 7920 6f66 2044 6972 6963 686c 6574 4d75  y of DirichletMu
-000057d0: 6c74 696e 6f6d 6961 6c20 6469 7374 7269  ltinomial distri
-000057e0: 6275 7469 6f6e 0a20 2020 2020 2020 2061  bution.        a
-000057f0: 7420 7370 6563 6966 6965 6420 7661 6c75  t specified valu
-00005800: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-00005810: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00005820: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00005830: 2020 7661 6c75 653a 2069 6e74 6567 6572    value: integer
-00005840: 2061 7272 6179 0a20 2020 2020 2020 2020   array.         
-00005850: 2020 2056 616c 7565 2066 6f72 2077 6869     Value for whi
-00005860: 6368 206c 6f67 2d70 726f 6261 6269 6c69  ch log-probabili
-00005870: 7479 2069 7320 6361 6c63 756c 6174 6564  ty is calculated
-00005880: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00005890: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-000058a0: 2d2d 0a20 2020 2020 2020 2054 656e 736f  --.        Tenso
-000058b0: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
-000058c0: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
-000058d0: 6d5f 6120 3d20 612e 7375 6d28 6178 6973  m_a = a.sum(axis
-000058e0: 3d2d 3129 0a20 2020 2020 2020 2063 6f6e  =-1).        con
-000058f0: 7374 203d 2028 6761 6d6d 616c 6e28 6e20  st = (gammaln(n 
-00005900: 2b20 3129 202b 2067 616d 6d61 6c6e 2873  + 1) + gammaln(s
-00005910: 756d 5f61 2929 202d 2067 616d 6d61 6c6e  um_a)) - gammaln
-00005920: 286e 202b 2073 756d 5f61 290a 2020 2020  (n + sum_a).    
-00005930: 2020 2020 7365 7269 6573 203d 2067 616d      series = gam
-00005940: 6d61 6c6e 2876 616c 7565 202b 2061 2920  maln(value + a) 
-00005950: 2d20 2867 616d 6d61 6c6e 2876 616c 7565  - (gammaln(value
-00005960: 202b 2031 2920 2b20 6761 6d6d 616c 6e28   + 1) + gammaln(
-00005970: 6129 290a 2020 2020 2020 2020 7265 7320  a)).        res 
-00005980: 3d20 636f 6e73 7420 2b20 7365 7269 6573  = const + series
-00005990: 2e73 756d 2861 7869 733d 2d31 290a 0a20  .sum(axis=-1).. 
-000059a0: 2020 2020 2020 2072 6573 203d 2070 742e         res = pt.
-000059b0: 7377 6974 6368 280a 2020 2020 2020 2020  switch(.        
-000059c0: 2020 2020 7074 2e6f 725f 280a 2020 2020      pt.or_(.    
-000059d0: 2020 2020 2020 2020 2020 2020 7074 2e61              pt.a
-000059e0: 6e79 2870 742e 6c74 2876 616c 7565 2c20  ny(pt.lt(value, 
-000059f0: 3029 2c20 6178 6973 3d2d 3129 2c0a 2020  0), axis=-1),.  
-00005a00: 2020 2020 2020 2020 2020 2020 2020 7074                pt
-00005a10: 2e6e 6571 2870 742e 7375 6d28 7661 6c75  .neq(pt.sum(valu
-00005a20: 652c 2061 7869 733d 2d31 292c 206e 292c  e, axis=-1), n),
-00005a30: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00005a40: 2020 2020 2020 2020 2020 2020 2d6e 702e              -np.
-00005a50: 696e 662c 0a20 2020 2020 2020 2020 2020  inf,.           
-00005a60: 2072 6573 2c0a 2020 2020 2020 2020 290a   res,.        ).
-00005a70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005a80: 6368 6563 6b5f 7061 7261 6d65 7465 7273  check_parameters
-00005a90: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-00005aa0: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
-00005ab0: 203e 2030 2c0a 2020 2020 2020 2020 2020   > 0,.          
-00005ac0: 2020 6e20 3e3d 2030 2c0a 2020 2020 2020    n >= 0,.      
-00005ad0: 2020 2020 2020 6d73 673d 2261 203e 2030        msg="a > 0
-00005ae0: 2c20 6e20 3e3d 2030 222c 0a20 2020 2020  , n >= 0",.     
-00005af0: 2020 2029 0a0a 0a63 6c61 7373 205f 4f72     )...class _Or
-00005b00: 6465 7265 644d 756c 7469 6e6f 6d69 616c  deredMultinomial
-00005b10: 284d 756c 7469 6e6f 6d69 616c 293a 0a20  (Multinomial):. 
-00005b20: 2020 2072 2222 220a 2020 2020 556e 6465     r""".    Unde
-00005b30: 726c 7969 6e67 2063 6c61 7373 2066 6f72  rlying class for
-00005b40: 206f 7264 6572 6564 206d 756c 7469 6e6f   ordered multino
-00005b50: 6d69 616c 2064 6973 7472 6962 7574 696f  mial distributio
-00005b60: 6e73 2e0a 2020 2020 5365 6520 646f 6373  ns..    See docs
-00005b70: 2066 6f72 2074 6865 204f 7264 6572 6564   for the Ordered
-00005b80: 4d75 6c74 696e 6f6d 6961 6c20 7772 6170  Multinomial wrap
-00005b90: 7065 7220 636c 6173 7320 666f 7220 6d6f  per class for mo
-00005ba0: 7265 2064 6574 6169 6c73 206f 6e20 686f  re details on ho
-00005bb0: 7720 746f 2075 7365 2069 7420 696e 206d  w to use it in m
-00005bc0: 6f64 656c 732e 0a20 2020 2022 2222 0a20  odels..    """. 
-00005bd0: 2020 2072 765f 6f70 203d 206d 756c 7469     rv_op = multi
-00005be0: 6e6f 6d69 616c 0a0a 2020 2020 4063 6c61  nomial..    @cla
-00005bf0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00005c00: 2064 6973 7428 636c 732c 2065 7461 2c20   dist(cls, eta, 
-00005c10: 6375 7470 6f69 6e74 732c 206e 2c20 2a61  cutpoints, n, *a
-00005c20: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
-00005c30: 2020 2020 2020 2020 6574 6120 3d20 7074          eta = pt
-00005c40: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
-00005c50: 626c 6528 666c 6f61 7458 2865 7461 2929  ble(floatX(eta))
-00005c60: 0a20 2020 2020 2020 2063 7574 706f 696e  .        cutpoin
-00005c70: 7473 203d 2070 742e 6173 5f74 656e 736f  ts = pt.as_tenso
-00005c80: 725f 7661 7269 6162 6c65 2863 7574 706f  r_variable(cutpo
-00005c90: 696e 7473 290a 2020 2020 2020 2020 6e20  ints).        n 
-00005ca0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00005cb0: 6172 6961 626c 6528 696e 7458 286e 2929  ariable(intX(n))
-00005cc0: 0a0a 2020 2020 2020 2020 7061 203d 2073  ..        pa = s
-00005cd0: 6967 6d6f 6964 2863 7574 706f 696e 7473  igmoid(cutpoints
-00005ce0: 202d 2070 742e 7368 6170 655f 7061 6472   - pt.shape_padr
-00005cf0: 6967 6874 2865 7461 2929 0a20 2020 2020  ight(eta)).     
-00005d00: 2020 2070 5f63 756d 203d 2070 742e 636f     p_cum = pt.co
-00005d10: 6e63 6174 656e 6174 6528 0a20 2020 2020  ncatenate(.     
-00005d20: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00005d30: 2020 2020 2020 2020 2070 742e 7a65 726f           pt.zero
-00005d40: 735f 6c69 6b65 2870 742e 7368 6170 655f  s_like(pt.shape_
-00005d50: 7061 6472 6967 6874 2870 615b 2e2e 2e2c  padright(pa[...,
-00005d60: 2030 5d29 292c 0a20 2020 2020 2020 2020   0])),.         
-00005d70: 2020 2020 2020 2070 612c 0a20 2020 2020         pa,.     
-00005d80: 2020 2020 2020 2020 2020 2070 742e 6f6e             pt.on
-00005d90: 6573 5f6c 696b 6528 7074 2e73 6861 7065  es_like(pt.shape
-00005da0: 5f70 6164 7269 6768 7428 7061 5b2e 2e2e  _padright(pa[...
-00005db0: 2c20 305d 2929 2c0a 2020 2020 2020 2020  , 0])),.        
-00005dc0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00005dd0: 2020 2061 7869 733d 2d31 2c0a 2020 2020     axis=-1,.    
-00005de0: 2020 2020 290a 2020 2020 2020 2020 7020      ).        p 
-00005df0: 3d20 705f 6375 6d5b 2e2e 2e2c 2031 3a5d  = p_cum[..., 1:]
-00005e00: 202d 2070 5f63 756d 5b2e 2e2e 2c20 3a2d   - p_cum[..., :-
-00005e10: 315d 0a0a 2020 2020 2020 2020 7265 7475  1]..        retu
-00005e20: 726e 2073 7570 6572 2829 2e64 6973 7428  rn super().dist(
-00005e30: 6e2c 2070 2c20 2a61 7267 732c 202a 2a6b  n, p, *args, **k
-00005e40: 7761 7267 7329 0a0a 0a63 6c61 7373 204f  wargs)...class O
-00005e50: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
-00005e60: 6c3a 0a20 2020 2072 2222 220a 2020 2020  l:.    r""".    
-00005e70: 5772 6170 7065 7220 636c 6173 7320 666f  Wrapper class fo
-00005e80: 7220 4f72 6465 7265 6420 4d75 6c74 696e  r Ordered Multin
-00005e90: 6f6d 6961 6c20 6469 7374 7269 6275 7469  omial distributi
-00005ea0: 6f6e 732e 0a0a 2020 2020 5573 6566 756c  ons...    Useful
-00005eb0: 2066 6f72 2072 6567 7265 7373 696f 6e20   for regression 
-00005ec0: 6f6e 206f 7264 696e 616c 2064 6174 6120  on ordinal data 
-00005ed0: 7768 6f73 6520 7661 6c75 6573 2072 616e  whose values ran
-00005ee0: 6765 0a20 2020 2066 726f 6d20 3120 746f  ge.    from 1 to
-00005ef0: 204b 2061 7320 6120 6675 6e63 7469 6f6e   K as a function
-00005f00: 206f 6620 736f 6d65 2070 7265 6469 6374   of some predict
-00005f10: 6f72 2c20 3a6d 6174 683a 605c 6574 6160  or, :math:`\eta`
-00005f20: 2c20 6275 740a 2020 2020 7768 6963 6820  , but.    which 
-00005f30: 6172 6520 5f61 6767 7265 6761 7465 645f  are _aggregated_
-00005f40: 2062 7920 7472 6961 6c2c 206c 696b 6520   by trial, like 
-00005f50: 6d75 6c74 696e 6f6d 6961 6c20 6f62 7365  multinomial obse
-00005f60: 7276 6174 696f 6e73 2028 696e 0a20 2020  rvations (in.   
-00005f70: 2063 6f6e 7472 6173 7420 746f 2060 706d   contrast to `pm
-00005f80: 2e4f 7264 6572 6564 4c6f 6769 7374 6963  .OrderedLogistic
-00005f90: 602c 2077 6869 6368 206f 6e6c 7920 6163  `, which only ac
-00005fa0: 6365 7074 7320 6f72 6469 6e61 6c20 6461  cepts ordinal da
-00005fb0: 7461 0a20 2020 2069 6e20 6120 5f64 6973  ta.    in a _dis
-00005fc0: 6167 6772 6567 6174 6564 5f20 666f 726d  aggregated_ form
-00005fd0: 6174 2c20 6c69 6b65 2063 6174 6567 6f72  at, like categor
-00005fe0: 6963 616c 206f 6273 6572 7661 7469 6f6e  ical observation
-00005ff0: 7329 2e0a 2020 2020 5468 6520 6375 7470  s)..    The cutp
-00006000: 6f69 6e74 732c 203a 6d61 7468 3a60 6360  oints, :math:`c`
-00006010: 2c20 7365 7061 7261 7465 2077 6869 6368  , separate which
-00006020: 2072 616e 6765 7320 6f66 203a 6d61 7468   ranges of :math
-00006030: 3a60 5c65 7461 6020 6172 650a 2020 2020  :`\eta` are.    
-00006040: 6d61 7070 6564 2074 6f20 7768 6963 6820  mapped to which 
-00006050: 6f66 2074 6865 204b 206f 6273 6572 7665  of the K observe
-00006060: 6420 6465 7065 6e64 656e 7420 7661 7269  d dependent vari
-00006070: 6162 6c65 732e 2054 6865 206e 756d 6265  ables. The numbe
-00006080: 720a 2020 2020 6f66 2063 7574 706f 696e  r.    of cutpoin
-00006090: 7473 2069 7320 4b20 2d20 312e 2049 7420  ts is K - 1. It 
-000060a0: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
-000060b0: 6861 7420 7468 6520 6375 7470 6f69 6e74  hat the cutpoint
-000060c0: 7320 6172 650a 2020 2020 636f 6e73 7472  s are.    constr
-000060d0: 6169 6e65 6420 746f 2062 6520 6f72 6465  ained to be orde
-000060e0: 7265 642e 0a0a 2020 2020 2e2e 206d 6174  red...    .. mat
-000060f0: 683a 3a0a 0a20 2020 2020 2020 6628 6b20  h::..       f(k 
-00006100: 5c6d 6964 205c 6574 612c 2063 2920 3d20  \mid \eta, c) = 
-00006110: 5c6c 6566 745c 7b0a 2020 2020 2020 2020  \left\{.        
-00006120: 205c 6265 6769 6e7b 6172 7261 797d 7b6c   \begin{array}{l
-00006130: 7d0a 2020 2020 2020 2020 2020 2031 202d  }.           1 -
-00006140: 205c 7465 7874 7b6c 6f67 6974 7d5e 7b2d   \text{logit}^{-
-00006150: 317d 285c 6574 6120 2d20 635f 3129 0a20  1}(\eta - c_1). 
-00006160: 2020 2020 2020 2020 2020 2020 5c2c 2c20              \,, 
-00006170: 5c74 6578 747b 6966 207d 206b 203d 2030  \text{if } k = 0
-00006180: 205c 5c0a 2020 2020 2020 2020 2020 205c   \\.           \
-00006190: 7465 7874 7b6c 6f67 6974 7d5e 7b2d 317d  text{logit}^{-1}
-000061a0: 285c 6574 6120 2d20 635f 7b6b 202d 2031  (\eta - c_{k - 1
-000061b0: 7d29 202d 0a20 2020 2020 2020 2020 2020  }) -.           
-000061c0: 5c74 6578 747b 6c6f 6769 747d 5e7b 2d31  \text{logit}^{-1
-000061d0: 7d28 5c65 7461 202d 2063 5f7b 6b7d 290a  }(\eta - c_{k}).
-000061e0: 2020 2020 2020 2020 2020 2020 205c 2c2c               \,,
-000061f0: 205c 7465 7874 7b69 6620 7d20 3020 3c20   \text{if } 0 < 
-00006200: 6b20 3c20 4b20 5c5c 0a20 2020 2020 2020  k < K \\.       
-00006210: 2020 2020 5c74 6578 747b 6c6f 6769 747d      \text{logit}
-00006220: 5e7b 2d31 7d28 5c65 7461 202d 2063 5f7b  ^{-1}(\eta - c_{
-00006230: 4b20 2d20 317d 290a 2020 2020 2020 2020  K - 1}).        
-00006240: 2020 2020 205c 2c2c 205c 7465 7874 7b69       \,, \text{i
-00006250: 6620 7d20 6b20 3d20 4b20 5c5c 0a20 2020  f } k = K \\.   
-00006260: 2020 2020 2020 5c65 6e64 7b61 7272 6179        \end{array
-00006270: 7d0a 2020 2020 2020 205c 7269 6768 742e  }.       \right.
-00006280: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00006290: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-000062a0: 2020 2020 6574 6120 3a20 7465 6e73 6f72      eta : tensor
-000062b0: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-000062c0: 2020 2020 2020 2054 6865 2070 7265 6469         The predi
-000062d0: 6374 6f72 2e0a 2020 2020 6375 7470 6f69  ctor..    cutpoi
-000062e0: 6e74 7320 3a20 7465 6e73 6f72 5f6c 696b  nts : tensor_lik
-000062f0: 6520 6f66 2066 6c6f 6174 0a20 2020 2020  e of float.     
-00006300: 2020 2054 6865 206c 656e 6774 6820 4b20     The length K 
-00006310: 2d20 3120 6172 7261 7920 6f66 2063 7574  - 1 array of cut
-00006320: 706f 696e 7473 2077 6869 6368 2062 7265  points which bre
-00006330: 616b 203a 6d61 7468 3a60 5c65 7461 6020  ak :math:`\eta` 
-00006340: 696e 746f 0a20 2020 2020 2020 2072 616e  into.        ran
-00006350: 6765 732e 2044 6f20 6e6f 7420 6578 706c  ges. Do not expl
-00006360: 6963 6974 6c79 2073 6574 2074 6865 2066  icitly set the f
-00006370: 6972 7374 2061 6e64 206c 6173 7420 656c  irst and last el
-00006380: 656d 656e 7473 206f 660a 2020 2020 2020  ements of.      
-00006390: 2020 3a6d 6174 683a 6063 6020 746f 206e    :math:`c` to n
-000063a0: 6567 6174 6976 6520 616e 6420 706f 7369  egative and posi
-000063b0: 7469 7665 2069 6e66 696e 6974 792e 0a20  tive infinity.. 
-000063c0: 2020 206e 203a 2074 656e 736f 725f 6c69     n : tensor_li
-000063d0: 6b65 206f 6620 696e 740a 2020 2020 2020  ke of int.      
-000063e0: 2020 5468 6520 746f 7461 6c20 6e75 6d62    The total numb
-000063f0: 6572 206f 6620 6d75 6c74 696e 6f6d 6961  er of multinomia
-00006400: 6c20 7472 6961 6c73 2e0a 2020 2020 636f  l trials..    co
-00006410: 6d70 7574 655f 7020 3a20 626f 6f6c 6561  mpute_p : boolea
-00006420: 6e2c 2064 6566 6175 6c74 3d54 7275 650a  n, default=True.
-00006430: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00006440: 746f 2063 6f6d 7075 7465 2061 6e64 2073  to compute and s
-00006450: 746f 7265 2069 6e20 7468 6520 7472 6163  tore in the trac
-00006460: 6520 7468 6520 696e 6665 7272 6564 2070  e the inferred p
-00006470: 726f 6261 6269 6c69 7469 6573 206f 6620  robabilities of 
-00006480: 6561 6368 0a20 2020 2020 2020 2063 6174  each.        cat
-00006490: 6567 6f72 6965 732c 0a20 2020 2020 2020  egories,.       
-000064a0: 2062 6173 6564 206f 6e20 7468 6520 6375   based on the cu
-000064b0: 7470 6f69 6e74 7327 2076 616c 7565 732e  tpoints' values.
-000064c0: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-000064d0: 652e 0a20 2020 2020 2020 204d 6967 6874  e..        Might
-000064e0: 2062 6520 7573 6566 756c 2074 6f20 6469   be useful to di
-000064f0: 7361 626c 6520 6974 2069 6620 6d65 6d6f  sable it if memo
-00006500: 7279 2075 7361 6765 2069 7320 6f66 2069  ry usage is of i
-00006510: 6e74 6572 6573 742e 0a0a 2020 2020 4578  nterest...    Ex
-00006520: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-00006530: 2d2d 2d0a 2020 2020 2e2e 2063 6f64 652d  ---.    .. code-
-00006540: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
-00006550: 2020 2020 2020 2020 2320 4765 6e65 7261          # Genera
-00006560: 7465 2064 6174 6120 666f 7220 6120 7369  te data for a si
-00006570: 6d70 6c65 2031 2064 696d 656e 7369 6f6e  mple 1 dimension
-00006580: 616c 2065 7861 6d70 6c65 2070 726f 626c  al example probl
-00006590: 656d 0a20 2020 2020 2020 2074 7275 655f  em.        true_
-000065a0: 6375 6d5f 7020 3d20 6e70 2e61 7272 6179  cum_p = np.array
-000065b0: 285b 302e 312c 2030 2e31 352c 2030 2e32  ([0.1, 0.15, 0.2
-000065c0: 352c 2030 2e35 302c 2030 2e36 352c 2030  5, 0.50, 0.65, 0
-000065d0: 2e39 302c 2031 2e30 5d29 0a20 2020 2020  .90, 1.0]).     
-000065e0: 2020 2074 7275 655f 7020 3d20 6e70 2e68     true_p = np.h
-000065f0: 7374 6163 6b28 5b74 7275 655f 6375 6d5f  stack([true_cum_
-00006600: 705b 305d 2c20 7472 7565 5f63 756d 5f70  p[0], true_cum_p
-00006610: 5b31 3a5d 202d 2074 7275 655f 6375 6d5f  [1:] - true_cum_
-00006620: 705b 3a2d 315d 5d29 0a20 2020 2020 2020  p[:-1]]).       
-00006630: 2066 616b 655f 656c 6563 7469 6f6e 7320   fake_elections 
-00006640: 3d20 6e70 2e72 616e 646f 6d2e 6d75 6c74  = np.random.mult
-00006650: 696e 6f6d 6961 6c28 6e3d 315f 3030 302c  inomial(n=1_000,
-00006660: 2070 7661 6c73 3d74 7275 655f 702c 2073   pvals=true_p, s
-00006670: 697a 653d 3630 290a 0a20 2020 2020 2020  ize=60)..       
-00006680: 2023 204f 7264 6572 6564 206d 756c 7469   # Ordered multi
-00006690: 6e6f 6d69 616c 2072 6567 7265 7373 696f  nomial regressio
-000066a0: 6e0a 2020 2020 2020 2020 7769 7468 2070  n.        with p
-000066b0: 6d2e 4d6f 6465 6c28 2920 6173 206d 6f64  m.Model() as mod
-000066c0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
-000066d0: 6375 7470 6f69 6e74 7320 3d20 706d 2e4e  cutpoints = pm.N
-000066e0: 6f72 6d61 6c28 0a20 2020 2020 2020 2020  ormal(.         
-000066f0: 2020 2020 2020 2022 6375 7470 6f69 6e74         "cutpoint
-00006700: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00006710: 2020 2020 6d75 3d6e 702e 6172 616e 6765      mu=np.arange
-00006720: 2836 2920 2d20 322e 352c 0a20 2020 2020  (6) - 2.5,.     
-00006730: 2020 2020 2020 2020 2020 2073 6967 6d61             sigma
-00006740: 3d31 2e35 2c0a 2020 2020 2020 2020 2020  =1.5,.          
-00006750: 2020 2020 2020 696e 6974 7661 6c3d 6e70        initval=np
-00006760: 2e61 7261 6e67 6528 3629 202d 2032 2e35  .arange(6) - 2.5
-00006770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006780: 2020 7472 616e 7366 6f72 6d3d 706d 2e64    transform=pm.d
-00006790: 6973 7472 6962 7574 696f 6e73 2e74 7261  istributions.tra
-000067a0: 6e73 666f 726d 732e 6f72 6465 7265 642c  nsforms.ordered,
-000067b0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000067c0: 2020 2020 2020 2020 2020 2020 706d 2e4f              pm.O
-000067d0: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
-000067e0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-000067f0: 2020 2022 7265 7375 6c74 7322 2c0a 2020     "results",.  
-00006800: 2020 2020 2020 2020 2020 2020 2020 6574                et
-00006810: 613d 302e 302c 0a20 2020 2020 2020 2020  a=0.0,.         
-00006820: 2020 2020 2020 2063 7574 706f 696e 7473         cutpoints
-00006830: 3d63 7574 706f 696e 7473 2c0a 2020 2020  =cutpoints,.    
-00006840: 2020 2020 2020 2020 2020 2020 6e3d 6661              n=fa
-00006850: 6b65 5f65 6c65 6374 696f 6e73 2e73 756d  ke_elections.sum
-00006860: 2831 292c 0a20 2020 2020 2020 2020 2020  (1),.           
-00006870: 2020 2020 206f 6273 6572 7665 643d 6661       observed=fa
-00006880: 6b65 5f65 6c65 6374 696f 6e73 2c0a 2020  ke_elections,.  
-00006890: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000068a0: 2020 2020 2020 2020 2074 7261 6365 203d           trace =
-000068b0: 2070 6d2e 7361 6d70 6c65 2829 0a0a 2020   pm.sample()..  
-000068c0: 2020 2020 2020 2320 506c 6f74 2074 6865        # Plot the
-000068d0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
-000068e0: 2061 7276 697a 2e70 6c6f 745f 706f 7374   arviz.plot_post
-000068f0: 6572 696f 7228 7472 6163 655f 3132 5f34  erior(trace_12_4
-00006900: 2c20 7661 725f 6e61 6d65 733d 5b22 636f  , var_names=["co
-00006910: 6d70 6c65 7465 5f70 225d 2c20 7265 665f  mplete_p"], ref_
-00006920: 7661 6c3d 6c69 7374 2874 7275 655f 7029  val=list(true_p)
-00006930: 293b 0a20 2020 2022 2222 0a0a 2020 2020  );.    """..    
-00006940: 6465 6620 5f5f 6e65 775f 5f28 636c 732c  def __new__(cls,
-00006950: 206e 616d 652c 202a 6172 6773 2c20 636f   name, *args, co
-00006960: 6d70 7574 655f 703d 5472 7565 2c20 2a2a  mpute_p=True, **
-00006970: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00006980: 206f 7574 5f72 7620 3d20 5f4f 7264 6572   out_rv = _Order
-00006990: 6564 4d75 6c74 696e 6f6d 6961 6c28 6e61  edMultinomial(na
-000069a0: 6d65 2c20 2a61 7267 732c 202a 2a6b 7761  me, *args, **kwa
-000069b0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
-000069c0: 636f 6d70 7574 655f 703a 0a20 2020 2020  compute_p:.     
-000069d0: 2020 2020 2020 2070 6d2e 4465 7465 726d         pm.Determ
-000069e0: 696e 6973 7469 6328 6622 7b6e 616d 657d  inistic(f"{name}
-000069f0: 5f70 726f 6273 222c 206f 7574 5f72 762e  _probs", out_rv.
-00006a00: 6f77 6e65 722e 696e 7075 7473 5b34 5d2c  owner.inputs[4],
-00006a10: 2064 696d 733d 6b77 6172 6773 2e67 6574   dims=kwargs.get
-00006a20: 2822 6469 6d73 2229 290a 2020 2020 2020  ("dims")).      
-00006a30: 2020 7265 7475 726e 206f 7574 5f72 760a    return out_rv.
-00006a40: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00006a50: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
-00006a60: 6c73 2c20 2a61 7267 732c 202a 2a6b 7761  ls, *args, **kwa
-00006a70: 7267 7329 3a0a 2020 2020 2020 2020 7265  rgs):.        re
-00006a80: 7475 726e 205f 4f72 6465 7265 644d 756c  turn _OrderedMul
-00006a90: 7469 6e6f 6d69 616c 2e64 6973 7428 2a61  tinomial.dist(*a
-00006aa0: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
-00006ab0: 0a64 6566 2070 6f73 6465 6628 4141 293a  .def posdef(AA):
-00006ac0: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-00006ad0: 2020 6c69 6e61 6c67 2e63 686f 6c65 736b    linalg.cholesk
-00006ae0: 7928 4141 290a 2020 2020 2020 2020 7265  y(AA).        re
-00006af0: 7475 726e 2031 0a20 2020 2065 7863 6570  turn 1.    excep
-00006b00: 7420 6c69 6e61 6c67 2e4c 696e 416c 6745  t linalg.LinAlgE
-00006b10: 7272 6f72 3a0a 2020 2020 2020 2020 7265  rror:.        re
-00006b20: 7475 726e 2030 0a0a 0a63 6c61 7373 2050  turn 0...class P
-00006b30: 6f73 4465 664d 6174 7269 7828 4f70 293a  osDefMatrix(Op):
-00006b40: 0a20 2020 2022 2222 0a20 2020 2043 6865  .    """.    Che
-00006b50: 636b 2069 6620 696e 7075 7420 6973 2070  ck if input is p
-00006b60: 6f73 6974 6976 6520 6465 6669 6e69 7465  ositive definite
-00006b70: 2e20 496e 7075 7420 7368 6f75 6c64 2062  . Input should b
-00006b80: 6520 6120 7371 7561 7265 206d 6174 7269  e a square matri
-00006b90: 782e 0a0a 2020 2020 2222 220a 0a20 2020  x...    """..   
-00006ba0: 2023 2050 726f 7065 7274 6965 7320 6174   # Properties at
-00006bb0: 7472 6962 7574 650a 2020 2020 5f5f 7072  tribute.    __pr
-00006bc0: 6f70 735f 5f20 3d20 2829 0a0a 2020 2020  ops__ = ()..    
-00006bd0: 2320 436f 6d70 756c 736f 7279 2069 6620  # Compulsory if 
-00006be0: 6974 7970 6573 2061 6e64 206f 7479 7065  itypes and otype
-00006bf0: 7320 6172 6520 6e6f 7420 6465 6669 6e65  s are not define
-00006c00: 640a 0a20 2020 2064 6566 206d 616b 655f  d..    def make_
-00006c10: 6e6f 6465 2873 656c 662c 2078 293a 0a20  node(self, x):. 
-00006c20: 2020 2020 2020 2078 203d 2070 742e 6173         x = pt.as
-00006c30: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-00006c40: 2878 290a 2020 2020 2020 2020 6173 7365  (x).        asse
-00006c50: 7274 2078 2e6e 6469 6d20 3d3d 2032 0a20  rt x.ndim == 2. 
-00006c60: 2020 2020 2020 206f 203d 2054 656e 736f         o = Tenso
-00006c70: 7254 7970 6528 6474 7970 653d 2269 6e74  rType(dtype="int
-00006c80: 3822 2c20 7368 6170 653d 5b5d 2928 290a  8", shape=[])().
-00006c90: 2020 2020 2020 2020 7265 7475 726e 2041          return A
-00006ca0: 7070 6c79 2873 656c 662c 205b 785d 2c20  pply(self, [x], 
-00006cb0: 5b6f 5d29 0a0a 2020 2020 2320 5079 7468  [o])..    # Pyth
-00006cc0: 6f6e 2069 6d70 6c65 6d65 6e74 6174 696f  on implementatio
-00006cd0: 6e3a 0a20 2020 2064 6566 2070 6572 666f  n:.    def perfo
-00006ce0: 726d 2873 656c 662c 206e 6f64 652c 2069  rm(self, node, i
-00006cf0: 6e70 7574 732c 206f 7574 7075 7473 293a  nputs, outputs):
-00006d00: 0a20 2020 2020 2020 2028 782c 2920 3d20  .        (x,) = 
-00006d10: 696e 7075 7473 0a20 2020 2020 2020 2028  inputs.        (
-00006d20: 7a2c 2920 3d20 6f75 7470 7574 730a 2020  z,) = outputs.  
-00006d30: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00006d40: 2020 2020 2020 207a 5b30 5d20 3d20 6e70         z[0] = np
-00006d50: 2e61 7272 6179 2870 6f73 6465 6628 7829  .array(posdef(x)
-00006d60: 2c20 6474 7970 653d 2269 6e74 3822 290a  , dtype="int8").
-00006d70: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00006d80: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00006d90: 2020 2020 2020 706d 2e5f 6c6f 672e 6578        pm._log.ex
-00006da0: 6365 7074 696f 6e28 2246 6169 6c65 6420  ception("Failed 
-00006db0: 746f 2063 6865 636b 2069 6620 2573 2070  to check if %s p
-00006dc0: 6f73 6974 6976 6520 6465 6669 6e69 7465  ositive definite
-00006dd0: 222c 2078 290a 2020 2020 2020 2020 2020  ", x).          
-00006de0: 2020 7261 6973 650a 0a20 2020 2064 6566    raise..    def
-00006df0: 2069 6e66 6572 5f73 6861 7065 2873 656c   infer_shape(sel
-00006e00: 662c 2066 6772 6170 682c 206e 6f64 652c  f, fgraph, node,
-00006e10: 2073 6861 7065 7329 3a0a 2020 2020 2020   shapes):.      
-00006e20: 2020 7265 7475 726e 205b 5b5d 5d0a 0a20    return [[]].. 
-00006e30: 2020 2064 6566 2067 7261 6428 7365 6c66     def grad(self
-00006e40: 2c20 696e 702c 2067 7261 6473 293a 0a20  , inp, grads):. 
-00006e50: 2020 2020 2020 2028 782c 2920 3d20 696e         (x,) = in
-00006e60: 700a 2020 2020 2020 2020 7265 7475 726e  p.        return
-00006e70: 205b 782e 7a65 726f 735f 6c69 6b65 2870   [x.zeros_like(p
-00006e80: 7974 656e 736f 722e 636f 6e66 6967 2e66  ytensor.config.f
-00006e90: 6c6f 6174 5829 5d0a 0a20 2020 2064 6566  loatX)]..    def
-00006ea0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
-00006eb0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00006ec0: 4d61 7472 6978 4973 506f 7369 7469 7665  MatrixIsPositive
-00006ed0: 4465 6669 6e69 7465 220a 0a0a 6d61 7472  Definite"...matr
-00006ee0: 6978 5f70 6f73 5f64 6566 203d 2050 6f73  ix_pos_def = Pos
-00006ef0: 4465 664d 6174 7269 7828 290a 0a0a 636c  DefMatrix()...cl
-00006f00: 6173 7320 5769 7368 6172 7452 5628 5261  ass WishartRV(Ra
-00006f10: 6e64 6f6d 5661 7269 6162 6c65 293a 0a20  ndomVariable):. 
-00006f20: 2020 206e 616d 6520 3d20 2277 6973 6861     name = "wisha
-00006f30: 7274 220a 2020 2020 6e64 696d 5f73 7570  rt".    ndim_sup
-00006f40: 7020 3d20 320a 2020 2020 6e64 696d 735f  p = 2.    ndims_
-00006f50: 7061 7261 6d73 203d 205b 302c 2032 5d0a  params = [0, 2].
-00006f60: 2020 2020 6474 7970 6520 3d20 2266 6c6f      dtype = "flo
-00006f70: 6174 5822 0a20 2020 205f 7072 696e 745f  atX".    _print_
-00006f80: 6e61 6d65 203d 2028 2257 6973 6861 7274  name = ("Wishart
-00006f90: 222c 2022 5c5c 6f70 6572 6174 6f72 6e61  ", "\\operatorna
-00006fa0: 6d65 7b57 6973 6861 7274 7d22 290a 0a20  me{Wishart}").. 
-00006fb0: 2020 2064 6566 205f 7375 7070 5f73 6861     def _supp_sha
-00006fc0: 7065 5f66 726f 6d5f 7061 7261 6d73 2873  pe_from_params(s
-00006fd0: 656c 662c 2064 6973 745f 7061 7261 6d73  elf, dist_params
-00006fe0: 2c20 7265 705f 7061 7261 6d5f 6964 783d  , rep_param_idx=
-00006ff0: 312c 2070 6172 616d 5f73 6861 7065 733d  1, param_shapes=
-00007000: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
-00007010: 2054 6865 2073 6861 7065 206f 6620 7365   The shape of se
-00007020: 636f 6e64 2070 6172 616d 6574 6572 2060  cond parameter `
-00007030: 5660 2064 6566 696e 6573 2074 6865 2073  V` defines the s
-00007040: 6861 7065 206f 6620 7468 6520 6f75 7470  hape of the outp
-00007050: 7574 2e0a 2020 2020 2020 2020 7265 7475  ut..        retu
-00007060: 726e 2064 6973 745f 7061 7261 6d73 5b31  rn dist_params[1
-00007070: 5d2e 7368 6170 655b 2d32 3a5d 0a0a 2020  ].shape[-2:]..  
-00007080: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-00007090: 2020 2064 6566 2072 6e67 5f66 6e28 636c     def rng_fn(cl
-000070a0: 732c 2072 6e67 2c20 6e75 2c20 562c 2073  s, rng, nu, V, s
-000070b0: 697a 6529 3a0a 2020 2020 2020 2020 7363  ize):.        sc
-000070c0: 6970 795f 7369 7a65 203d 2073 697a 6520  ipy_size = size 
-000070d0: 6966 2073 697a 6520 656c 7365 2031 2020  if size else 1  
-000070e0: 2320 4465 6661 756c 7420 7369 7a65 2066  # Default size f
-000070f0: 6f72 2053 6369 7079 2773 2077 6973 6861  or Scipy's wisha
-00007100: 7274 2e72 7673 2069 7320 310a 2020 2020  rt.rvs is 1.    
-00007110: 2020 2020 7265 7375 6c74 203d 2073 7461      result = sta
-00007120: 7473 2e77 6973 6861 7274 2e72 7673 2869  ts.wishart.rvs(i
-00007130: 6e74 286e 7529 2c20 562c 2073 697a 653d  nt(nu), V, size=
-00007140: 7363 6970 795f 7369 7a65 2c20 7261 6e64  scipy_size, rand
-00007150: 6f6d 5f73 7461 7465 3d72 6e67 290a 2020  om_state=rng).  
-00007160: 2020 2020 2020 6966 2073 697a 6520 3d3d        if size ==
-00007170: 2028 312c 293a 0a20 2020 2020 2020 2020   (1,):.         
-00007180: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00007190: 5b6e 702e 6e65 7761 7869 732c 202e 2e2e  [np.newaxis, ...
-000071a0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-000071b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000071c0: 726e 2072 6573 756c 740a 0a0a 7769 7368  rn result...wish
-000071d0: 6172 7420 3d20 5769 7368 6172 7452 5628  art = WishartRV(
-000071e0: 290a 0a0a 636c 6173 7320 5769 7368 6172  )...class Wishar
-000071f0: 7428 436f 6e74 696e 756f 7573 293a 0a20  t(Continuous):. 
-00007200: 2020 2072 2222 220a 2020 2020 5769 7368     r""".    Wish
-00007210: 6172 7420 6c6f 672d 6c69 6b65 6c69 686f  art log-likeliho
-00007220: 6f64 2e0a 0a20 2020 2054 6865 2057 6973  od...    The Wis
-00007230: 6861 7274 2064 6973 7472 6962 7574 696f  hart distributio
-00007240: 6e20 6973 2074 6865 2070 726f 6261 6269  n is the probabi
-00007250: 6c69 7479 2064 6973 7472 6962 7574 696f  lity distributio
-00007260: 6e20 6f66 2074 6865 0a20 2020 206d 6178  n of the.    max
-00007270: 696d 756d 2d6c 696b 656c 6968 6f6f 6420  imum-likelihood 
-00007280: 6573 7469 6d61 746f 7220 284d 4c45 2920  estimator (MLE) 
-00007290: 6f66 2074 6865 2070 7265 6369 7369 6f6e  of the precision
-000072a0: 206d 6174 7269 7820 6f66 2061 0a20 2020   matrix of a.   
-000072b0: 206d 756c 7469 7661 7269 6174 6520 6e6f   multivariate no
-000072c0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
-000072d0: 6e2e 2020 4966 2056 3d31 2c20 7468 6520  n.  If V=1, the 
-000072e0: 6469 7374 7269 6275 7469 6f6e 2069 730a  distribution is.
-000072f0: 2020 2020 6964 656e 7469 6361 6c20 746f      identical to
-00007300: 2074 6865 2063 6869 2d73 7175 6172 6520   the chi-square 
-00007310: 6469 7374 7269 6275 7469 6f6e 2077 6974  distribution wit
-00007320: 6820 6e75 2064 6567 7265 6573 206f 660a  h nu degrees of.
-00007330: 2020 2020 6672 6565 646f 6d2e 0a0a 2020      freedom...  
-00007340: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
-00007350: 2020 2020 6628 5820 5c6d 6964 206e 752c      f(X \mid nu,
-00007360: 2054 2920 3d0a 2020 2020 2020 2020 2020   T) =.          
-00007370: 205c 6672 6163 7b7b 5c6d 6964 2054 205c   \frac{{\mid T \
-00007380: 6d69 647d 5e7b 6e75 2f32 7d7b 5c6d 6964  mid}^{nu/2}{\mid
-00007390: 2058 205c 6d69 647d 5e7b 286e 752d 6b2d   X \mid}^{(nu-k-
-000073a0: 3129 2f32 7d7d 7b32 5e7b 6e75 206b 2f32  1)/2}}{2^{nu k/2
-000073b0: 7d0a 2020 2020 2020 2020 2020 205c 4761  }.           \Ga
-000073c0: 6d6d 615f 7028 6e75 2f32 297d 205c 6578  mma_p(nu/2)} \ex
-000073d0: 705c 6c65 6674 5c7b 202d 5c66 7261 637b  p\left\{ -\frac{
-000073e0: 317d 7b32 7d20 5472 2854 5829 205c 7269  1}{2} Tr(TX) \ri
-000073f0: 6768 745c 7d0a 0a20 2020 2077 6865 7265  ght\}..    where
-00007400: 203a 6d61 7468 3a60 6b60 2069 7320 7468   :math:`k` is th
-00007410: 6520 7261 6e6b 206f 6620 3a6d 6174 683a  e rank of :math:
-00007420: 6058 602e 0a0a 2020 2020 3d3d 3d3d 3d3d  `X`...    ======
-00007430: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
-00007440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
-00007460: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
-00007470: 683a 6058 2870 2078 2070 2960 2070 6f73  h:`X(p x p)` pos
-00007480: 6974 6976 6520 6465 6669 6e69 7465 206d  itive definite m
-00007490: 6174 7269 780a 2020 2020 4d65 616e 2020  atrix.    Mean  
-000074a0: 2020 2020 3a6d 6174 683a 606e 7520 5660      :math:`nu V`
-000074b0: 0a20 2020 2056 6172 6961 6e63 6520 203a  .    Variance  :
-000074c0: 6d61 7468 3a60 6e75 2028 765f 7b69 6a7d  math:`nu (v_{ij}
-000074d0: 5e32 202b 2076 5f7b 6969 7d20 765f 7b6a  ^2 + v_{ii} v_{j
-000074e0: 6a7d 2960 0a20 2020 203d 3d3d 3d3d 3d3d  j})`.    =======
-000074f0: 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =  =============
-00007500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020  ============..  
-00007520: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00007530: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00007540: 6e75 203a 2074 656e 736f 725f 6c69 6b65  nu : tensor_like
-00007550: 206f 6620 696e 740a 2020 2020 2020 2020   of int.        
-00007560: 4465 6772 6565 7320 6f66 2066 7265 6564  Degrees of freed
-00007570: 6f6d 2c20 3e20 302e 0a20 2020 2056 203a  om, > 0..    V :
-00007580: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-00007590: 666c 6f61 740a 2020 2020 2020 2020 7020  float.        p 
-000075a0: 7820 7020 706f 7369 7469 7665 2064 6566  x p positive def
-000075b0: 696e 6974 6520 6d61 7472 6978 2e0a 0a20  inite matrix... 
-000075c0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-000075d0: 2d2d 0a20 2020 2054 6869 7320 6469 7374  --.    This dist
-000075e0: 7269 6275 7469 6f6e 2069 7320 756e 7573  ribution is unus
-000075f0: 6162 6c65 2069 6e20 6120 5079 4d43 206d  able in a PyMC m
-00007600: 6f64 656c 2e20 596f 7520 7368 6f75 6c64  odel. You should
-00007610: 2069 6e73 7465 6164 0a20 2020 2075 7365   instead.    use
-00007620: 204c 4b4a 4368 6f6c 6573 6b79 436f 7620   LKJCholeskyCov 
-00007630: 6f72 204c 4b4a 436f 7272 2e0a 2020 2020  or LKJCorr..    
-00007640: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
-00007650: 7769 7368 6172 740a 0a20 2020 2040 636c  wishart..    @cl
-00007660: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00007670: 6620 6469 7374 2863 6c73 2c20 6e75 2c20  f dist(cls, nu, 
-00007680: 562c 202a 6172 6773 2c20 2a2a 6b77 6172  V, *args, **kwar
-00007690: 6773 293a 0a20 2020 2020 2020 206e 7520  gs):.        nu 
-000076a0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-000076b0: 6172 6961 626c 6528 696e 7458 286e 7529  ariable(intX(nu)
-000076c0: 290a 2020 2020 2020 2020 5620 3d20 7074  ).        V = pt
-000076d0: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
-000076e0: 626c 6528 666c 6f61 7458 2856 2929 0a0a  ble(floatX(V))..
-000076f0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00007700: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-00007710: 2020 2022 5468 6520 5769 7368 6172 7420     "The Wishart 
-00007720: 6469 7374 7269 6275 7469 6f6e 2063 616e  distribution can
-00007730: 2063 7572 7265 6e74 6c79 206e 6f74 2062   currently not b
-00007740: 6520 7573 6564 2022 0a20 2020 2020 2020  e used ".       
-00007750: 2020 2020 2022 666f 7220 4d43 4d43 2073       "for MCMC s
-00007760: 616d 706c 696e 672e 2054 6865 2070 726f  ampling. The pro
-00007770: 6261 6269 6c69 7479 206f 6620 7361 6d70  bability of samp
-00007780: 6c69 6e67 2061 2022 0a20 2020 2020 2020  ling a ".       
-00007790: 2020 2020 2022 7379 6d6d 6574 7269 6320       "symmetric 
-000077a0: 6d61 7472 6978 2069 7320 6261 7369 6361  matrix is basica
-000077b0: 6c6c 7920 7a65 726f 2e20 496e 7374 6561  lly zero. Instea
-000077c0: 642c 2070 6c65 6173 6520 220a 2020 2020  d, please ".    
-000077d0: 2020 2020 2020 2020 2275 7365 204c 4b4a          "use LKJ
-000077e0: 4368 6f6c 6573 6b79 436f 7620 6f72 204c  CholeskyCov or L
-000077f0: 4b4a 436f 7272 2e20 466f 7220 6d6f 7265  KJCorr. For more
-00007800: 2069 6e66 6f72 6d61 7469 6f6e 2022 0a20   information ". 
-00007810: 2020 2020 2020 2020 2020 2022 6f6e 2074             "on t
-00007820: 6865 2069 7373 7565 7320 7375 7272 6f75  he issues surrou
-00007830: 6e64 696e 6720 7468 6520 5769 7368 6172  nding the Wishar
-00007840: 7420 7365 6520 6865 7265 3a20 220a 2020  t see here: ".  
-00007850: 2020 2020 2020 2020 2020 2268 7474 7073            "https
-00007860: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00007870: 6d63 2d64 6576 732f 7079 6d63 2f69 7373  mc-devs/pymc/iss
-00007880: 7565 732f 3533 382e 222c 0a20 2020 2020  ues/538.",.     
-00007890: 2020 2020 2020 2055 7365 7257 6172 6e69         UserWarni
-000078a0: 6e67 2c0a 2020 2020 2020 2020 290a 0a20  ng,.        ).. 
-000078b0: 2020 2020 2020 2023 206d 6561 6e20 3d20         # mean = 
-000078c0: 6e75 202a 2056 0a20 2020 2020 2020 2023  nu * V.        #
-000078d0: 2070 203d 2056 2e73 6861 7065 5b30 5d0a   p = V.shape[0].
-000078e0: 2020 2020 2020 2020 2320 6d6f 6465 203d          # mode =
-000078f0: 2070 742e 7377 6974 6368 2870 742e 6765   pt.switch(pt.ge
-00007900: 286e 752c 2070 202b 2031 292c 2028 6e75  (nu, p + 1), (nu
-00007910: 202d 2070 202d 2031 2920 2a20 562c 206e   - p - 1) * V, n
-00007920: 702e 6e61 6e29 0a20 2020 2020 2020 2072  p.nan).        r
-00007930: 6574 7572 6e20 7375 7065 7228 292e 6469  eturn super().di
-00007940: 7374 285b 6e75 2c20 565d 2c20 2a61 7267  st([nu, V], *arg
-00007950: 732c 202a 2a6b 7761 7267 7329 0a0a 2020  s, **kwargs)..  
-00007960: 2020 6465 6620 6c6f 6770 2858 2c20 6e75    def logp(X, nu
-00007970: 2c20 5629 3a0a 2020 2020 2020 2020 2222  , V):.        ""
-00007980: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
-00007990: 6174 6520 6c6f 672d 7072 6f62 6162 696c  ate log-probabil
-000079a0: 6974 7920 6f66 2057 6973 6861 7274 2064  ity of Wishart d
-000079b0: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
-000079c0: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
-000079d0: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
-000079e0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000079f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00007a00: 2020 2020 2020 2058 3a20 6e75 6d65 7269         X: numeri
-00007a10: 630a 2020 2020 2020 2020 2020 2020 5661  c.            Va
-00007a20: 6c75 6520 666f 7220 7768 6963 6820 6c6f  lue for which lo
-00007a30: 672d 7072 6f62 6162 696c 6974 7920 6973  g-probability is
-00007a40: 2063 616c 6375 6c61 7465 642e 0a0a 2020   calculated...  
-00007a50: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00007a60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00007a70: 2020 2020 2020 5465 6e73 6f72 5661 7269        TensorVari
-00007a80: 6162 6c65 0a20 2020 2020 2020 2022 2222  able.        """
-00007a90: 0a0a 2020 2020 2020 2020 7020 3d20 562e  ..        p = V.
-00007aa0: 7368 6170 655b 305d 0a0a 2020 2020 2020  shape[0]..      
-00007ab0: 2020 4956 4920 3d20 6465 7428 5629 0a20    IVI = det(V). 
-00007ac0: 2020 2020 2020 2049 5849 203d 2064 6574         IXI = det
-00007ad0: 2858 290a 0a20 2020 2020 2020 2072 6574  (X)..        ret
-00007ae0: 7572 6e20 6368 6563 6b5f 7061 7261 6d65  urn check_parame
-00007af0: 7465 7273 280a 2020 2020 2020 2020 2020  ters(.          
-00007b00: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00007b10: 2020 2020 286e 7520 2d20 7020 2d20 3129      (nu - p - 1)
-00007b20: 202a 2070 742e 6c6f 6728 4958 4929 0a20   * pt.log(IXI). 
-00007b30: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00007b40: 2074 7261 6365 286d 6174 7269 785f 696e   trace(matrix_in
-00007b50: 7665 7273 6528 5629 2e64 6f74 2858 2929  verse(V).dot(X))
-00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b70: 202d 206e 7520 2a20 7020 2a20 7074 2e6c   - nu * p * pt.l
-00007b80: 6f67 2832 290a 2020 2020 2020 2020 2020  og(2).          
-00007b90: 2020 2020 2020 2d20 6e75 202a 2070 742e        - nu * pt.
-00007ba0: 6c6f 6728 4956 4929 0a20 2020 2020 2020  log(IVI).       
-00007bb0: 2020 2020 2020 2020 202d 2032 202a 206d           - 2 * m
-00007bc0: 756c 7469 6761 6d6d 616c 6e28 6e75 202f  ultigammaln(nu /
-00007bd0: 2032 2e30 2c20 7029 0a20 2020 2020 2020   2.0, p).       
-00007be0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00007bf0: 2020 202f 2032 2c0a 2020 2020 2020 2020     / 2,.        
-00007c00: 2020 2020 6d61 7472 6978 5f70 6f73 5f64      matrix_pos_d
-00007c10: 6566 2858 292c 0a20 2020 2020 2020 2020  ef(X),.         
-00007c20: 2020 2070 742e 6571 2858 2c20 582e 5429     pt.eq(X, X.T)
-00007c30: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-00007c40: 203e 2028 7020 2d20 3129 2c0a 2020 2020   > (p - 1),.    
-00007c50: 2020 2020 290a 0a0a 6465 6620 5769 7368      )...def Wish
-00007c60: 6172 7442 6172 746c 6574 7428 6e61 6d65  artBartlett(name
-00007c70: 2c20 532c 206e 752c 2069 735f 6368 6f6c  , S, nu, is_chol
-00007c80: 6573 6b79 3d46 616c 7365 2c20 7265 7475  esky=False, retu
-00007c90: 726e 5f63 686f 6c65 736b 793d 4661 6c73  rn_cholesky=Fals
-00007ca0: 652c 2069 6e69 7476 616c 3d4e 6f6e 6529  e, initval=None)
-00007cb0: 3a0a 2020 2020 7222 2222 0a20 2020 2042  :.    r""".    B
-00007cc0: 6172 746c 6574 7420 6465 636f 6d70 6f73  artlett decompos
-00007cd0: 6974 696f 6e20 6f66 2074 6865 2057 6973  ition of the Wis
-00007ce0: 6861 7274 2064 6973 7472 6962 7574 696f  hart distributio
-00007cf0: 6e2e 2041 7320 7468 6520 5769 7368 6172  n. As the Wishar
-00007d00: 740a 2020 2020 6469 7374 7269 6275 7469  t.    distributi
-00007d10: 6f6e 2072 6571 7569 7265 7320 7468 6520  on requires the 
-00007d20: 6d61 7472 6978 2074 6f20 6265 2073 796d  matrix to be sym
-00007d30: 6d65 7472 6963 2070 6f73 6974 6976 6520  metric positive 
-00007d40: 7365 6d69 2d64 6566 696e 6974 650a 2020  semi-definite.  
-00007d50: 2020 6974 2069 7320 696d 706f 7373 6962    it is impossib
-00007d60: 6c65 2066 6f72 204d 434d 4320 746f 2065  le for MCMC to e
-00007d70: 7665 7220 7072 6f70 6f73 6520 6163 6365  ver propose acce
-00007d80: 7074 6162 6c65 206d 6174 7269 6365 732e  ptable matrices.
-00007d90: 0a0a 2020 2020 496e 7374 6561 642c 2077  ..    Instead, w
-00007da0: 6520 6361 6e20 7573 6520 7468 6520 4261  e can use the Ba
-00007db0: 726c 6574 7420 6465 636f 6d70 6f73 6974  rlett decomposit
-00007dc0: 696f 6e20 7768 6963 6820 7361 6d70 6c65  ion which sample
-00007dd0: 7320 6120 6c6f 7765 720a 2020 2020 6469  s a lower.    di
-00007de0: 6167 6f6e 616c 206d 6174 7269 782e 2053  agonal matrix. S
-00007df0: 7065 6369 6669 6361 6c6c 793a 0a0a 2020  pecifically:..  
-00007e00: 2020 2e2e 206d 6174 683a 3a0a 2020 2020    .. math::.    
-00007e10: 2020 2020 5c74 6578 747b 4966 7d20 4c20      \text{If} L 
-00007e20: 5c73 696d 205c 6265 6769 6e7b 706d 6174  \sim \begin{pmat
-00007e30: 7269 787d 0a20 2020 2020 2020 205c 7371  rix}.        \sq
-00007e40: 7274 7b63 5f31 7d20 2620 3020 2620 3020  rt{c_1} & 0 & 0 
-00007e50: 5c5c 0a20 2020 2020 2020 207a 5f7b 3231  \\.        z_{21
-00007e60: 7d20 2620 5c73 7172 747b 635f 327d 2026  } & \sqrt{c_2} &
-00007e70: 2030 205c 5c0a 2020 2020 2020 2020 7a5f   0 \\.        z_
-00007e80: 7b33 317d 2026 207a 5f7b 3332 7d20 2620  {31} & z_{32} & 
-00007e90: 5c73 7172 747b 635f 337d 0a20 2020 2020  \sqrt{c_3}.     
-00007ea0: 2020 205c 656e 647b 706d 6174 7269 787d     \end{pmatrix}
-00007eb0: 0a0a 2020 2020 2020 2020 5c74 6578 747b  ..        \text{
-00007ec0: 7769 7468 7d20 635f 6920 5c73 696d 205c  with} c_i \sim \
-00007ed0: 6368 695e 3228 6e2d 692b 3129 205c 7465  chi^2(n-i+1) \te
-00007ee0: 7874 7b20 616e 6420 7d20 6e5f 7b69 6a7d  xt{ and } n_{ij}
-00007ef0: 205c 7369 6d20 5c6d 6174 6863 616c 7b4e   \sim \mathcal{N
-00007f00: 7d28 302c 2031 292c 205c 7465 7874 7b74  }(0, 1), \text{t
-00007f10: 6865 6e7d 205c 5c0a 2020 2020 2020 2020  hen} \\.        
-00007f20: 4c20 5c74 696d 6573 2041 205c 7469 6d65  L \times A \time
-00007f30: 7320 412e 5420 5c74 696d 6573 204c 2e54  s A.T \times L.T
-00007f40: 205c 7369 6d20 5c74 6578 747b 5769 7368   \sim \text{Wish
-00007f50: 6172 747d 284c 205c 7469 6d65 7320 4c2e  art}(L \times L.
-00007f60: 542c 205c 6e75 290a 0a20 2020 2053 6565  T, \nu)..    See
-00007f70: 2068 7474 703a 2f2f 656e 2e77 696b 6970   http://en.wikip
-00007f80: 6564 6961 2e6f 7267 2f77 696b 692f 5769  edia.org/wiki/Wi
-00007f90: 7368 6172 745f 6469 7374 7269 6275 7469  shart_distributi
-00007fa0: 6f6e 2342 6172 746c 6574 745f 6465 636f  on#Bartlett_deco
-00007fb0: 6d70 6f73 6974 696f 6e0a 2020 2020 666f  mposition.    fo
-00007fc0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00007fd0: 6f6e 2e0a 0a20 2020 2050 6172 616d 6574  on...    Paramet
-00007fe0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00007ff0: 2d2d 0a20 2020 2053 203a 206e 6461 7272  --.    S : ndarr
-00008000: 6179 0a20 2020 2020 2020 2070 2078 2070  ay.        p x p
-00008010: 2070 6f73 6974 6976 6520 6465 6669 6e69   positive defini
-00008020: 7465 206d 6174 7269 780a 2020 2020 2020  te matrix.      
-00008030: 2020 4f72 3a0a 2020 2020 2020 2020 7020    Or:.        p 
-00008040: 7820 7020 6c6f 7765 722d 7472 6961 6e67  x p lower-triang
-00008050: 756c 6172 206d 6174 7269 7820 7468 6174  ular matrix that
-00008060: 2069 7320 7468 6520 4368 6f6c 6573 6b79   is the Cholesky
-00008070: 2066 6163 746f 720a 2020 2020 2020 2020   factor.        
-00008080: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
-00008090: 6520 6d61 7472 6978 2e0a 2020 2020 6e75  e matrix..    nu
-000080a0: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-000080b0: 6620 696e 740a 2020 2020 2020 2020 4465  f int.        De
-000080c0: 6772 6565 7320 6f66 2066 7265 6564 6f6d  grees of freedom
-000080d0: 2c20 3e20 6469 6d28 5329 2e0a 2020 2020  , > dim(S)..    
-000080e0: 6973 5f63 686f 6c65 736b 7920 3a20 626f  is_cholesky : bo
-000080f0: 6f6c 2c20 6465 6661 756c 743d 4661 6c73  ol, default=Fals
-00008100: 650a 2020 2020 2020 2020 496e 7075 7420  e.        Input 
-00008110: 6d61 7472 6978 2053 2069 7320 616c 7265  matrix S is alre
-00008120: 6164 7920 4368 6f6c 6573 6b79 2064 6563  ady Cholesky dec
-00008130: 6f6d 706f 7365 6420 6173 2053 2e54 202a  omposed as S.T *
-00008140: 2053 0a20 2020 2072 6574 7572 6e5f 6368   S.    return_ch
-00008150: 6f6c 6573 6b79 203a 2062 6f6f 6c2c 2064  olesky : bool, d
-00008160: 6566 6175 6c74 3d46 616c 7365 0a20 2020  efault=False.   
-00008170: 2020 2020 204f 6e6c 7920 7265 7475 726e       Only return
-00008180: 2074 6865 2043 686f 6c65 736b 7920 6465   the Cholesky de
-00008190: 636f 6d70 6f73 6564 206d 6174 7269 782e  composed matrix.
-000081a0: 0a20 2020 2069 6e69 7476 616c 203a 206e  .    initval : n
-000081b0: 6461 7272 6179 0a20 2020 2020 2020 2070  darray.        p
-000081c0: 2078 2070 2070 6f73 6974 6976 6520 6465   x p positive de
-000081d0: 6669 6e69 7465 206d 6174 7269 7820 7573  finite matrix us
-000081e0: 6564 2074 6f20 696e 6974 6961 6c69 7a65  ed to initialize
-000081f0: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
-00008200: 2d2d 2d2d 2d0a 2020 2020 5468 6973 2069  -----.    This i
-00008210: 7320 6e6f 7420 6120 7374 616e 6461 7264  s not a standard
-00008220: 2044 6973 7472 6962 7574 696f 6e20 636c   Distribution cl
-00008230: 6173 7320 6275 7420 666f 6c6c 6f77 7320  ass but follows 
-00008240: 6120 7369 6d69 6c61 720a 2020 2020 696e  a similar.    in
-00008250: 7465 7266 6163 652e 2042 6573 6964 6573  terface. Besides
-00008260: 2074 6865 2057 6973 6861 7274 2064 6973   the Wishart dis
-00008270: 7472 6962 7574 696f 6e2c 2069 7420 7769  tribution, it wi
-00008280: 6c6c 2061 6464 2052 5673 0a20 2020 206e  ll add RVs.    n
-00008290: 616d 655f 6320 616e 6420 6e61 6d65 5f7a  ame_c and name_z
-000082a0: 2074 6f20 796f 7572 206d 6f64 656c 2077   to your model w
-000082b0: 6869 6368 206d 616b 6520 7570 2074 6865  hich make up the
-000082c0: 206d 6174 7269 782e 0a0a 2020 2020 5468   matrix...    Th
-000082d0: 6973 2064 6973 7472 6962 7574 696f 6e20  is distribution 
-000082e0: 6973 2075 7375 616c 6c79 2061 2062 6164  is usually a bad
-000082f0: 2069 6465 6120 746f 2075 7365 2061 7320   idea to use as 
-00008300: 6120 7072 696f 7220 666f 7220 6d75 6c74  a prior for mult
-00008310: 6976 6172 6961 7465 0a20 2020 206e 6f72  ivariate.    nor
-00008320: 6d61 6c2e 2059 6f75 2073 686f 756c 6420  mal. You should 
-00008330: 696e 7374 6561 6420 7573 6520 4c4b 4a43  instead use LKJC
-00008340: 686f 6c65 736b 7943 6f76 206f 7220 4c4b  holeskyCov or LK
-00008350: 4a43 6f72 722e 0a20 2020 2022 2222 0a0a  JCorr..    """..
-00008360: 2020 2020 4c20 3d20 5320 6966 2069 735f      L = S if is_
-00008370: 6368 6f6c 6573 6b79 2065 6c73 6520 7363  cholesky else sc
-00008380: 6970 792e 6c69 6e61 6c67 2e63 686f 6c65  ipy.linalg.chole
-00008390: 736b 7928 5329 0a20 2020 2064 6961 675f  sky(S).    diag_
-000083a0: 6964 7820 3d20 6e70 2e64 6961 675f 696e  idx = np.diag_in
-000083b0: 6469 6365 735f 6672 6f6d 2853 290a 2020  dices_from(S).  
-000083c0: 2020 7472 696c 5f69 6478 203d 206e 702e    tril_idx = np.
-000083d0: 7472 696c 5f69 6e64 6963 6573 5f66 726f  tril_indices_fro
-000083e0: 6d28 532c 206b 3d2d 3129 0a20 2020 206e  m(S, k=-1).    n
-000083f0: 5f64 6961 6720 3d20 6c65 6e28 6469 6167  _diag = len(diag
-00008400: 5f69 6478 5b30 5d29 0a20 2020 206e 5f74  _idx[0]).    n_t
-00008410: 7269 6c20 3d20 6c65 6e28 7472 696c 5f69  ril = len(tril_i
-00008420: 6478 5b30 5d29 0a0a 2020 2020 6966 2069  dx[0])..    if i
-00008430: 6e69 7476 616c 2069 7320 6e6f 7420 4e6f  nitval is not No
-00008440: 6e65 3a0a 2020 2020 2020 2020 2320 496e  ne:.        # In
-00008450: 7665 7273 6520 7472 616e 7366 6f72 6d0a  verse transform.
-00008460: 2020 2020 2020 2020 696e 6974 7661 6c20          initval 
-00008470: 3d20 6e70 2e64 6f74 286e 702e 646f 7428  = np.dot(np.dot(
-00008480: 6e70 2e6c 696e 616c 672e 696e 7628 4c29  np.linalg.inv(L)
-00008490: 2c20 696e 6974 7661 6c29 2c20 6e70 2e6c  , initval), np.l
-000084a0: 696e 616c 672e 696e 7628 4c2e 5429 290a  inalg.inv(L.T)).
-000084b0: 2020 2020 2020 2020 696e 6974 7661 6c20          initval 
-000084c0: 3d20 6c69 6e61 6c67 2e63 686f 6c65 736b  = linalg.cholesk
-000084d0: 7928 696e 6974 7661 6c2c 206c 6f77 6572  y(initval, lower
-000084e0: 3d54 7275 6529 0a20 2020 2020 2020 2064  =True).        d
-000084f0: 6961 675f 7465 7374 7661 6c20 3d20 696e  iag_testval = in
-00008500: 6974 7661 6c5b 6469 6167 5f69 6478 5d20  itval[diag_idx] 
-00008510: 2a2a 2032 0a20 2020 2020 2020 2074 7269  ** 2.        tri
-00008520: 6c5f 7465 7374 7661 6c20 3d20 696e 6974  l_testval = init
-00008530: 7661 6c5b 7472 696c 5f69 6478 5d0a 2020  val[tril_idx].  
-00008540: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008550: 6469 6167 5f74 6573 7476 616c 203d 204e  diag_testval = N
-00008560: 6f6e 650a 2020 2020 2020 2020 7472 696c  one.        tril
-00008570: 5f74 6573 7476 616c 203d 204e 6f6e 650a  _testval = None.
-00008580: 0a20 2020 2063 203d 2070 742e 7371 7274  .    c = pt.sqrt
-00008590: 280a 2020 2020 2020 2020 4368 6953 7175  (.        ChiSqu
-000085a0: 6172 6564 2822 2573 5f63 2220 2520 6e61  ared("%s_c" % na
-000085b0: 6d65 2c20 6e75 202d 206e 702e 6172 616e  me, nu - np.aran
-000085c0: 6765 2832 2c20 3220 2b20 6e5f 6469 6167  ge(2, 2 + n_diag
-000085d0: 292c 2073 6861 7065 3d6e 5f64 6961 672c  ), shape=n_diag,
-000085e0: 2069 6e69 7476 616c 3d64 6961 675f 7465   initval=diag_te
-000085f0: 7374 7661 6c29 0a20 2020 2029 0a20 2020  stval).    ).   
-00008600: 2070 6d2e 5f6c 6f67 2e69 6e66 6f28 2241   pm._log.info("A
-00008610: 6464 6564 206e 6577 2076 6172 6961 626c  dded new variabl
-00008620: 6520 2573 5f63 2074 6f20 6d6f 6465 6c20  e %s_c to model 
-00008630: 6469 6167 6f6e 616c 206f 6620 5769 7368  diagonal of Wish
-00008640: 6172 742e 2220 2520 6e61 6d65 290a 2020  art." % name).  
-00008650: 2020 7a20 3d20 4e6f 726d 616c 2822 2573    z = Normal("%s
-00008660: 5f7a 2220 2520 6e61 6d65 2c20 302e 302c  _z" % name, 0.0,
-00008670: 2031 2e30 2c20 7368 6170 653d 6e5f 7472   1.0, shape=n_tr
-00008680: 696c 2c20 696e 6974 7661 6c3d 7472 696c  il, initval=tril
-00008690: 5f74 6573 7476 616c 290a 2020 2020 706d  _testval).    pm
-000086a0: 2e5f 6c6f 672e 696e 666f 2822 4164 6465  ._log.info("Adde
-000086b0: 6420 6e65 7720 7661 7269 6162 6c65 2025  d new variable %
-000086c0: 735f 7a20 746f 206d 6f64 656c 206f 6666  s_z to model off
-000086d0: 2d64 6961 676f 6e61 6c73 206f 6620 5769  -diagonals of Wi
-000086e0: 7368 6172 742e 2220 2520 6e61 6d65 290a  shart." % name).
-000086f0: 2020 2020 2320 436f 6e73 7472 7563 7420      # Construct 
-00008700: 4120 6d61 7472 6978 0a20 2020 2041 203d  A matrix.    A =
-00008710: 2070 742e 7a65 726f 7328 532e 7368 6170   pt.zeros(S.shap
-00008720: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
-00008730: 7433 3229 0a20 2020 2041 203d 2070 742e  t32).    A = pt.
-00008740: 7365 745f 7375 6274 656e 736f 7228 415b  set_subtensor(A[
-00008750: 6469 6167 5f69 6478 5d2c 2063 290a 2020  diag_idx], c).  
-00008760: 2020 4120 3d20 7074 2e73 6574 5f73 7562    A = pt.set_sub
-00008770: 7465 6e73 6f72 2841 5b74 7269 6c5f 6964  tensor(A[tril_id
-00008780: 785d 2c20 7a29 0a0a 2020 2020 2320 4c20  x], z)..    # L 
-00008790: 2a20 4120 2a20 412e 5420 2a20 4c2e 5420  * A * A.T * L.T 
-000087a0: 7e20 5769 7368 6172 7428 4c2a 4c2e 542c  ~ Wishart(L*L.T,
-000087b0: 206e 7529 0a20 2020 2069 6620 7265 7475   nu).    if retu
-000087c0: 726e 5f63 686f 6c65 736b 793a 0a20 2020  rn_cholesky:.   
-000087d0: 2020 2020 2072 6574 7572 6e20 706d 2e44       return pm.D
-000087e0: 6574 6572 6d69 6e69 7374 6963 286e 616d  eterministic(nam
-000087f0: 652c 2070 742e 646f 7428 4c2c 2041 2929  e, pt.dot(L, A))
-00008800: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00008810: 2020 2072 6574 7572 6e20 706d 2e44 6574     return pm.Det
-00008820: 6572 6d69 6e69 7374 6963 286e 616d 652c  erministic(name,
-00008830: 2070 742e 646f 7428 7074 2e64 6f74 2870   pt.dot(pt.dot(p
-00008840: 742e 646f 7428 4c2c 2041 292c 2041 2e54  t.dot(L, A), A.T
-00008850: 292c 204c 2e54 2929 0a0a 0a64 6566 205f  ), L.T))...def _
-00008860: 6c6b 6a5f 6e6f 726d 616c 697a 696e 675f  lkj_normalizing_
-00008870: 636f 6e73 7461 6e74 2865 7461 2c20 6e29  constant(eta, n)
-00008880: 3a0a 2020 2020 2320 544f 444f 3a20 5468  :.    # TODO: Th
-00008890: 6973 2069 7320 6d69 7869 6e67 2070 7974  is is mixing pyt
-000088a0: 686f 6e20 6272 616e 6368 696e 6720 7769  hon branching wi
-000088b0: 7468 2074 6865 2070 6f74 656e 7469 616c  th the potential
-000088c0: 6c79 2073 796d 626f 6c69 6320 6e20 616e  ly symbolic n an
-000088d0: 6420 6574 6120 7661 7269 6162 6c65 730a  d eta variables.
-000088e0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-000088f0: 7461 6e63 6528 6574 612c 2028 696e 742c  tance(eta, (int,
-00008900: 2066 6c6f 6174 2929 3a0a 2020 2020 2020   float)):.      
-00008910: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-00008920: 6d65 6e74 6564 4572 726f 7228 2265 7461  mentedError("eta
-00008930: 206d 7573 7420 6265 2061 6e20 696e 7420   must be an int 
-00008940: 6f72 2066 6c6f 6174 2229 0a20 2020 2069  or float").    i
-00008950: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00008960: 286e 2c20 696e 7429 3a0a 2020 2020 2020  (n, int):.      
-00008970: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-00008980: 6d65 6e74 6564 4572 726f 7228 226e 206d  mentedError("n m
-00008990: 7573 7420 6265 2061 6e20 696e 7465 6765  ust be an intege
-000089a0: 7222 290a 2020 2020 6966 2065 7461 203d  r").    if eta =
-000089b0: 3d20 313a 0a20 2020 2020 2020 2072 6573  = 1:.        res
-000089c0: 756c 7420 3d20 6761 6d6d 616c 6e28 322e  ult = gammaln(2.
-000089d0: 3020 2a20 7074 2e61 7261 6e67 6528 312c  0 * pt.arange(1,
-000089e0: 2069 6e74 2828 6e20 2d20 3129 202f 2032   int((n - 1) / 2
-000089f0: 2920 2b20 3129 292e 7375 6d28 290a 2020  ) + 1)).sum().  
-00008a00: 2020 2020 2020 6966 206e 2025 2032 203d        if n % 2 =
-00008a10: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00008a20: 2072 6573 756c 7420 2b3d 2028 0a20 2020   result += (.   
-00008a30: 2020 2020 2020 2020 2020 2020 2030 2e32               0.2
-00008a40: 3520 2a20 286e 2a2a 3220 2d20 3129 202a  5 * (n**2 - 1) *
-00008a50: 2070 742e 6c6f 6728 6e70 2e70 6929 0a20   pt.log(np.pi). 
-00008a60: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00008a70: 2030 2e32 3520 2a20 286e 202d 2031 2920   0.25 * (n - 1) 
-00008a80: 2a2a 2032 202a 2070 742e 6c6f 6728 322e  ** 2 * pt.log(2.
-00008a90: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-00008aa0: 2020 202d 2028 6e20 2d20 3129 202a 2067     - (n - 1) * g
-00008ab0: 616d 6d61 6c6e 2869 6e74 2828 6e20 2b20  ammaln(int((n + 
-00008ac0: 3129 202f 2032 2929 0a20 2020 2020 2020  1) / 2)).       
-00008ad0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00008ae0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008af0: 2072 6573 756c 7420 2b3d 2028 0a20 2020   result += (.   
-00008b00: 2020 2020 2020 2020 2020 2020 2030 2e32               0.2
-00008b10: 3520 2a20 6e20 2a20 286e 202d 2032 2920  5 * n * (n - 2) 
-00008b20: 2a20 7074 2e6c 6f67 286e 702e 7069 290a  * pt.log(np.pi).
-00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b40: 2b20 302e 3235 202a 2028 3320 2a20 6e2a  + 0.25 * (3 * n*
-00008b50: 2a32 202d 2034 202a 206e 2920 2a20 7074  *2 - 4 * n) * pt
-00008b60: 2e6c 6f67 2832 2e30 290a 2020 2020 2020  .log(2.0).      
-00008b70: 2020 2020 2020 2020 2020 2b20 6e20 2a20            + n * 
-00008b80: 6761 6d6d 616c 6e28 6e20 2f20 3229 0a20  gammaln(n / 2). 
-00008b90: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00008ba0: 2028 6e20 2d20 3129 202a 2067 616d 6d61   (n - 1) * gamma
-00008bb0: 6c6e 286e 290a 2020 2020 2020 2020 2020  ln(n).          
-00008bc0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
-00008bd0: 2020 2020 2020 7265 7375 6c74 203d 202d        result = -
-00008be0: 286e 202d 2031 2920 2a20 6761 6d6d 616c  (n - 1) * gammal
-00008bf0: 6e28 6574 6120 2b20 302e 3520 2a20 286e  n(eta + 0.5 * (n
-00008c00: 202d 2031 2929 0a20 2020 2020 2020 206b   - 1)).        k
-00008c10: 203d 2070 742e 6172 616e 6765 2831 2c20   = pt.arange(1, 
-00008c20: 6e29 0a20 2020 2020 2020 2072 6573 756c  n).        resul
-00008c30: 7420 2b3d 2028 302e 3520 2a20 6b20 2a20  t += (0.5 * k * 
-00008c40: 7074 2e6c 6f67 286e 702e 7069 2920 2b20  pt.log(np.pi) + 
-00008c50: 6761 6d6d 616c 6e28 6574 6120 2b20 302e  gammaln(eta + 0.
-00008c60: 3520 2a20 286e 202d 2031 202d 206b 2929  5 * (n - 1 - k))
-00008c70: 292e 7375 6d28 290a 2020 2020 7265 7475  ).sum().    retu
-00008c80: 726e 2072 6573 756c 740a 0a0a 636c 6173  rn result...clas
-00008c90: 7320 5f4c 4b4a 4368 6f6c 6573 6b79 436f  s _LKJCholeskyCo
-00008ca0: 7642 6173 6552 5628 5261 6e64 6f6d 5661  vBaseRV(RandomVa
-00008cb0: 7269 6162 6c65 293a 0a20 2020 206e 616d  riable):.    nam
-00008cc0: 6520 3d20 225f 6c6b 6a63 686f 6c65 736b  e = "_lkjcholesk
-00008cd0: 7963 6f76 6261 7365 220a 2020 2020 6e64  ycovbase".    nd
-00008ce0: 696d 5f73 7570 7020 3d20 310a 2020 2020  im_supp = 1.    
-00008cf0: 6e64 696d 735f 7061 7261 6d73 203d 205b  ndims_params = [
-00008d00: 302c 2030 2c20 315d 0a20 2020 2064 7479  0, 0, 1].    dty
-00008d10: 7065 203d 2022 666c 6f61 7458 220a 2020  pe = "floatX".  
-00008d20: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
-00008d30: 2822 5f6c 6b6a 6368 6f6c 6573 6b79 636f  ("_lkjcholeskyco
-00008d40: 7662 6173 6522 2c20 225c 5c6f 7065 7261  vbase", "\\opera
-00008d50: 746f 726e 616d 657b 5f6c 6b6a 6368 6f6c  torname{_lkjchol
-00008d60: 6573 6b79 636f 7662 6173 657d 2229 0a0a  eskycovbase}")..
-00008d70: 2020 2020 6465 6620 6d61 6b65 5f6e 6f64      def make_nod
-00008d80: 6528 7365 6c66 2c20 726e 672c 2073 697a  e(self, rng, siz
-00008d90: 652c 2064 7479 7065 2c20 6e2c 2065 7461  e, dtype, n, eta
-00008da0: 2c20 4429 3a0a 2020 2020 2020 2020 6e20  , D):.        n 
-00008db0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00008dc0: 6172 6961 626c 6528 6e29 0a20 2020 2020  ariable(n).     
-00008dd0: 2020 2069 6620 6e6f 7420 6e2e 6e64 696d     if not n.ndim
-00008de0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00008df0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00008e00: 726f 7228 226e 206d 7573 7420 6265 2061  ror("n must be a
-00008e10: 2073 6361 6c61 7220 286e 6469 6d3d 3029   scalar (ndim=0)
-00008e20: 2e22 290a 0a20 2020 2020 2020 2065 7461  .")..        eta
-00008e30: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-00008e40: 7661 7269 6162 6c65 2865 7461 290a 2020  variable(eta).  
-00008e50: 2020 2020 2020 6966 206e 6f74 2065 7461        if not eta
-00008e60: 2e6e 6469 6d20 3d3d 2030 3a0a 2020 2020  .ndim == 0:.    
-00008e70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00008e80: 6c75 6545 7272 6f72 2822 6574 6120 6d75  lueError("eta mu
-00008e90: 7374 2062 6520 6120 7363 616c 6172 2028  st be a scalar (
-00008ea0: 6e64 696d 3d30 292e 2229 0a0a 2020 2020  ndim=0).")..    
-00008eb0: 2020 2020 4420 3d20 7074 2e61 735f 7465      D = pt.as_te
-00008ec0: 6e73 6f72 5f76 6172 6961 626c 6528 4429  nsor_variable(D)
-00008ed0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008ee0: 2073 7570 6572 2829 2e6d 616b 655f 6e6f   super().make_no
-00008ef0: 6465 2872 6e67 2c20 7369 7a65 2c20 6474  de(rng, size, dt
-00008f00: 7970 652c 206e 2c20 6574 612c 2044 290a  ype, n, eta, D).
-00008f10: 0a20 2020 2064 6566 205f 7375 7070 5f73  .    def _supp_s
-00008f20: 6861 7065 5f66 726f 6d5f 7061 7261 6d73  hape_from_params
-00008f30: 2873 656c 662c 2064 6973 745f 7061 7261  (self, dist_para
-00008f40: 6d73 2c20 7061 7261 6d5f 7368 6170 6573  ms, param_shapes
-00008f50: 293a 0a20 2020 2020 2020 206e 203d 2064  ):.        n = d
-00008f60: 6973 745f 7061 7261 6d73 5b30 5d0a 2020  ist_params[0].  
-00008f70: 2020 2020 2020 7265 7475 726e 2028 286e        return ((n
-00008f80: 202a 2028 6e20 2b20 3129 2920 2f2f 2032   * (n + 1)) // 2
-00008f90: 2c29 0a0a 2020 2020 6465 6620 726e 675f  ,)..    def rng_
-00008fa0: 666e 2873 656c 662c 2072 6e67 2c20 6e2c  fn(self, rng, n,
-00008fb0: 2065 7461 2c20 442c 2073 697a 6529 3a0a   eta, D, size):.
-00008fc0: 2020 2020 2020 2020 2320 5765 2066 6c61          # We fla
-00008fd0: 7474 656e 2074 6865 2073 697a 6520 746f  tten the size to
-00008fe0: 206d 616b 6520 6f70 6572 6174 696f 6e73   make operations
-00008ff0: 2065 6173 6965 722c 2061 6e64 2074 6865   easier, and the
-00009000: 6e20 7265 6275 696c 6420 6974 0a20 2020  n rebuild it.   
-00009010: 2020 2020 2069 6620 7369 7a65 2069 7320       if size is 
-00009020: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00009030: 2020 7369 7a65 203d 2044 2e73 6861 7065    size = D.shape
-00009040: 5b3a 2d31 5d0a 2020 2020 2020 2020 666c  [:-1].        fl
-00009050: 6174 5f73 697a 6520 3d20 6e70 2e70 726f  at_size = np.pro
-00009060: 6428 7369 7a65 292e 6173 7479 7065 2869  d(size).astype(i
-00009070: 6e74 290a 0a20 2020 2020 2020 2043 203d  nt)..        C =
-00009080: 204c 4b4a 436f 7272 5256 2e5f 7261 6e64   LKJCorrRV._rand
-00009090: 6f6d 5f63 6f72 725f 6d61 7472 6978 2872  om_corr_matrix(r
-000090a0: 6e67 3d72 6e67 2c20 6e3d 6e2c 2065 7461  ng=rng, n=n, eta
-000090b0: 3d65 7461 2c20 666c 6174 5f73 697a 653d  =eta, flat_size=
-000090c0: 666c 6174 5f73 697a 6529 0a20 2020 2020  flat_size).     
-000090d0: 2020 2044 203d 2044 2e72 6573 6861 7065     D = D.reshape
-000090e0: 2866 6c61 745f 7369 7a65 2c20 6e29 0a20  (flat_size, n). 
-000090f0: 2020 2020 2020 2043 202a 3d20 445b 2e2e         C *= D[..
-00009100: 2e2c 203a 2c20 6e70 2e6e 6577 6178 6973  ., :, np.newaxis
-00009110: 5d20 2a20 445b 2e2e 2e2c 206e 702e 6e65  ] * D[..., np.ne
-00009120: 7761 7869 732c 203a 5d0a 0a20 2020 2020  waxis, :]..     
-00009130: 2020 2074 7269 6c5f 6964 7820 3d20 6e70     tril_idx = np
-00009140: 2e74 7269 6c5f 696e 6469 6365 7328 6e2c  .tril_indices(n,
-00009150: 206b 3d30 290a 2020 2020 2020 2020 7361   k=0).        sa
-00009160: 6d70 6c65 7320 3d20 6e70 2e6c 696e 616c  mples = np.linal
-00009170: 672e 6368 6f6c 6573 6b79 2843 295b 2e2e  g.cholesky(C)[..
-00009180: 2e2c 2074 7269 6c5f 6964 785b 305d 2c20  ., tril_idx[0], 
-00009190: 7472 696c 5f69 6478 5b31 5d5d 0a0a 2020  tril_idx[1]]..  
-000091a0: 2020 2020 2020 6966 2073 697a 6520 6973        if size is
-000091b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000091c0: 2020 2073 616d 706c 6573 203d 2073 616d     samples = sam
-000091d0: 706c 6573 5b30 5d0a 2020 2020 2020 2020  ples[0].        
-000091e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000091f0: 2020 6469 7374 5f73 6861 7065 203d 2028    dist_shape = (
-00009200: 6e20 2a20 286e 202b 2031 2929 202f 2f20  n * (n + 1)) // 
-00009210: 320a 2020 2020 2020 2020 2020 2020 7361  2.            sa
-00009220: 6d70 6c65 7320 3d20 6e70 2e72 6573 6861  mples = np.resha
-00009230: 7065 2873 616d 706c 6573 2c20 282a 7369  pe(samples, (*si
-00009240: 7a65 2c20 6469 7374 5f73 6861 7065 2929  ze, dist_shape))
-00009250: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00009260: 2073 616d 706c 6573 0a0a 0a5f 6c6a 6b5f   samples..._ljk_
-00009270: 6368 6f6c 6573 6b79 5f63 6f76 5f62 6173  cholesky_cov_bas
-00009280: 6520 3d20 5f4c 4b4a 4368 6f6c 6573 6b79  e = _LKJCholesky
-00009290: 436f 7642 6173 6552 5628 290a 0a0a 2320  CovBaseRV()...# 
-000092a0: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7642  _LKJCholeskyCovB
-000092b0: 6173 6552 5620 7265 7175 6972 6573 2061  aseRV requires a
-000092c0: 2070 726f 7065 726c 7920 7368 6170 6564   properly shaped
-000092d0: 2060 4460 2c20 7768 6963 6820 6d65 616e   `D`, which mean
-000092e0: 7320 7468 6520 7661 7269 6162 6c65 2063  s the variable c
-000092f0: 616e 2774 0a23 2062 6520 7361 6665 6c79  an't.# be safely
-00009300: 2072 6573 697a 6564 2e20 4265 6361 7573   resized. Becaus
-00009310: 6520 6f66 2074 6869 732c 2077 6520 6164  e of this, we ad
-00009320: 6420 7468 6520 7468 696e 2053 796d 626f  d the thin Symbo
-00009330: 6c69 6352 616e 646f 6d56 6172 6961 626c  licRandomVariabl
-00009340: 6520 7772 6170 7065 720a 636c 6173 7320  e wrapper.class 
-00009350: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7652  _LKJCholeskyCovR
-00009360: 5628 5379 6d62 6f6c 6963 5261 6e64 6f6d  V(SymbolicRandom
-00009370: 5661 7269 6162 6c65 293a 0a20 2020 2064  Variable):.    d
-00009380: 6566 6175 6c74 5f6f 7574 7075 7420 3d20  efault_output = 
-00009390: 310a 2020 2020 5f70 7269 6e74 5f6e 616d  1.    _print_nam
-000093a0: 6520 3d20 2822 5f6c 6b6a 6368 6f6c 6573  e = ("_lkjcholes
-000093b0: 6b79 636f 7622 2c20 225c 5c6f 7065 7261  kycov", "\\opera
-000093c0: 746f 726e 616d 657b 5f6c 6b6a 6368 6f6c  torname{_lkjchol
-000093d0: 6573 6b79 636f 767d 2229 0a0a 2020 2020  eskycov}")..    
-000093e0: 6465 6620 7570 6461 7465 2873 656c 662c  def update(self,
-000093f0: 206e 6f64 6529 3a0a 2020 2020 2020 2020   node):.        
-00009400: 7265 7475 726e 207b 6e6f 6465 2e69 6e70  return {node.inp
-00009410: 7574 735b 305d 3a20 6e6f 6465 2e6f 7574  uts[0]: node.out
-00009420: 7075 7473 5b30 5d7d 0a0a 0a63 6c61 7373  puts[0]}...class
-00009430: 205f 4c4b 4a43 686f 6c65 736b 7943 6f76   _LKJCholeskyCov
-00009440: 2844 6973 7472 6962 7574 696f 6e29 3a0a  (Distribution):.
-00009450: 2020 2020 7222 2222 556e 6465 726c 7969      r"""Underlyi
-00009460: 6e67 2063 6c61 7373 2066 6f72 2063 6f76  ng class for cov
-00009470: 6172 6961 6e63 6520 6d61 7472 6978 2077  ariance matrix w
-00009480: 6974 6820 4c4b 4a20 6469 7374 7269 6275  ith LKJ distribu
-00009490: 7465 6420 636f 7272 656c 6174 696f 6e73  ted correlations
-000094a0: 2e0a 2020 2020 5365 6520 646f 6373 2066  ..    See docs f
-000094b0: 6f72 204c 4b4a 4368 6f6c 6573 6b79 436f  or LKJCholeskyCo
-000094c0: 7620 6675 6e63 7469 6f6e 2066 6f72 206d  v function for m
-000094d0: 6f72 6520 6465 7461 696c 7320 6f6e 2068  ore details on h
-000094e0: 6f77 2074 6f20 7573 6520 6974 2069 6e20  ow to use it in 
-000094f0: 6d6f 6465 6c73 2e0a 2020 2020 2222 220a  models..    """.
-00009500: 0a20 2020 2072 765f 7479 7065 203d 205f  .    rv_type = _
-00009510: 4c4b 4a43 686f 6c65 736b 7943 6f76 5256  LKJCholeskyCovRV
-00009520: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00009530: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
-00009540: 636c 732c 206e 2c20 6574 612c 2073 645f  cls, n, eta, sd_
-00009550: 6469 7374 2c20 2a2a 6b77 6172 6773 293a  dist, **kwargs):
-00009560: 0a20 2020 2020 2020 206e 203d 2070 742e  .        n = pt.
-00009570: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-00009580: 6c65 2869 6e74 5828 6e29 290a 2020 2020  le(intX(n)).    
-00009590: 2020 2020 6574 6120 3d20 7074 2e61 735f      eta = pt.as_
-000095a0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-000095b0: 666c 6f61 7458 2865 7461 2929 0a0a 2020  floatX(eta))..  
-000095c0: 2020 2020 2020 6966 206e 6f74 2028 0a20        if not (. 
-000095d0: 2020 2020 2020 2020 2020 2069 7369 6e73             isins
-000095e0: 7461 6e63 6528 7364 5f64 6973 742c 2056  tance(sd_dist, V
-000095f0: 6172 6961 626c 6529 0a20 2020 2020 2020  ariable).       
-00009600: 2020 2020 2061 6e64 2073 645f 6469 7374       and sd_dist
-00009610: 2e6f 776e 6572 2069 7320 6e6f 7420 4e6f  .owner is not No
-00009620: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
-00009630: 6e64 2069 7369 6e73 7461 6e63 6528 7364  nd isinstance(sd
-00009640: 5f64 6973 742e 6f77 6e65 722e 6f70 2c20  _dist.owner.op, 
-00009650: 2852 616e 646f 6d56 6172 6961 626c 652c  (RandomVariable,
-00009660: 2053 796d 626f 6c69 6352 616e 646f 6d56   SymbolicRandomV
-00009670: 6172 6961 626c 6529 290a 2020 2020 2020  ariable)).      
-00009680: 2020 2020 2020 616e 6420 7364 5f64 6973        and sd_dis
-00009690: 742e 6f77 6e65 722e 6f70 2e6e 6469 6d5f  t.owner.op.ndim_
-000096a0: 7375 7070 203c 2032 0a20 2020 2020 2020  supp < 2.       
-000096b0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-000096c0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-000096d0: 2273 645f 6469 7374 206d 7573 7420 6265  "sd_dist must be
-000096e0: 2061 2073 6361 6c61 7220 6f72 2076 6563   a scalar or vec
-000096f0: 746f 7220 6469 7374 7269 6275 7469 6f6e  tor distribution
-00009700: 2076 6172 6961 626c 6522 290a 0a20 2020   variable")..   
-00009710: 2020 2020 2063 6865 636b 5f64 6973 745f       check_dist_
-00009720: 6e6f 745f 7265 6769 7374 6572 6564 2873  not_registered(s
-00009730: 645f 6469 7374 290a 2020 2020 2020 2020  d_dist).        
-00009740: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
-00009750: 6973 7428 5b6e 2c20 6574 612c 2073 645f  ist([n, eta, sd_
-00009760: 6469 7374 5d2c 202a 2a6b 7761 7267 7329  dist], **kwargs)
-00009770: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00009780: 6f64 0a20 2020 2064 6566 2072 765f 6f70  od.    def rv_op
-00009790: 2863 6c73 2c20 6e2c 2065 7461 2c20 7364  (cls, n, eta, sd
-000097a0: 5f64 6973 742c 2073 697a 653d 4e6f 6e65  _dist, size=None
-000097b0: 293a 0a20 2020 2020 2020 2023 2057 6520  ):.        # We 
-000097c0: 7265 7369 7a65 2074 6865 2073 645f 6469  resize the sd_di
-000097d0: 7374 2061 7574 6f6d 6174 6963 616c 6c79  st automatically
-000097e0: 2073 6f20 7468 6174 2069 7420 6861 7320   so that it has 
-000097f0: 2873 697a 6520 7820 6e29 2069 6e64 6570  (size x n) indep
-00009800: 656e 6465 6e74 0a20 2020 2020 2020 2023  endent.        #
-00009810: 2064 7261 7773 2077 6869 6368 2069 7320   draws which is 
-00009820: 7768 6174 2074 6865 2060 5f4c 4b4a 4368  what the `_LKJCh
-00009830: 6f6c 6573 6b79 436f 7642 6173 6552 562e  oleskyCovBaseRV.
-00009840: 726e 675f 666e 6020 6578 7065 6374 732e  rng_fn` expects.
-00009850: 2054 6869 7320 6d61 6b65 7320 7468 650a   This makes the.
-00009860: 2020 2020 2020 2020 2320 7261 6e64 6f6d          # random
-00009870: 2061 6e64 206c 6f67 7020 6d65 7468 6f64   and logp method
-00009880: 7320 6571 7569 7661 6c65 6e74 2c20 6173  s equivalent, as
-00009890: 2074 6865 206c 6174 7465 7220 616c 736f   the latter also
-000098a0: 2061 7373 756d 6573 2061 2075 6e69 7175   assumes a uniqu
-000098b0: 6520 7661 6c75 650a 2020 2020 2020 2020  e value.        
-000098c0: 2320 666f 7220 6561 6368 2064 6961 676f  # for each diago
-000098d0: 6e61 6c20 656c 656d 656e 742e 0a20 2020  nal element..   
-000098e0: 2020 2020 2023 2053 696e 6365 2060 6574       # Since `et
-000098f0: 6160 2061 6e64 2060 6e60 2061 7265 2066  a` and `n` are f
-00009900: 6f72 6365 6420 746f 2062 6520 7363 616c  orced to be scal
-00009910: 6172 7320 7765 2064 6f6e 2774 206e 6565  ars we don't nee
-00009920: 6420 746f 2077 6f72 7279 2061 626f 7574  d to worry about
-00009930: 0a20 2020 2020 2020 2023 2069 6d70 6c69  .        # impli
-00009940: 6564 2062 6174 6368 6564 2064 696d 656e  ed batched dimen
-00009950: 7369 6f6e 7320 6672 6f6d 2074 686f 7365  sions from those
-00009960: 2066 6f72 2074 6865 2074 696d 6520 6265   for the time be
-00009970: 696e 672e 0a20 2020 2020 2020 2069 6620  ing..        if 
-00009980: 7369 7a65 2069 7320 4e6f 6e65 3a0a 2020  size is None:.  
-00009990: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
-000099a0: 2073 645f 6469 7374 2e73 6861 7065 5b3a   sd_dist.shape[:
-000099b0: 2d31 5d0a 2020 2020 2020 2020 7368 6170  -1].        shap
-000099c0: 6520 3d20 7475 706c 6528 7369 7a65 2920  e = tuple(size) 
-000099d0: 2b20 286e 2c29 0a20 2020 2020 2020 2069  + (n,).        i
-000099e0: 6620 7364 5f64 6973 742e 6f77 6e65 722e  f sd_dist.owner.
-000099f0: 6f70 2e6e 6469 6d5f 7375 7070 203d 3d20  op.ndim_supp == 
-00009a00: 303a 0a20 2020 2020 2020 2020 2020 2073  0:.            s
-00009a10: 645f 6469 7374 203d 2063 6861 6e67 655f  d_dist = change_
-00009a20: 6469 7374 5f73 697a 6528 7364 5f64 6973  dist_size(sd_dis
-00009a30: 742c 2073 6861 7065 290a 2020 2020 2020  t, shape).      
-00009a40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009a50: 2020 2020 2320 5468 6520 7375 7070 6f72      # The suppor
-00009a60: 7420 7368 6170 6520 6d75 7374 2062 6520  t shape must be 
-00009a70: 606e 6020 6275 7420 7765 2068 6176 6520  `n` but we have 
-00009a80: 6e6f 2077 6179 206f 6620 636f 6e74 726f  no way of contro
-00009a90: 6c6c 696e 6720 6974 0a20 2020 2020 2020  lling it.       
-00009aa0: 2020 2020 2073 645f 6469 7374 203d 2063       sd_dist = c
-00009ab0: 6861 6e67 655f 6469 7374 5f73 697a 6528  hange_dist_size(
-00009ac0: 7364 5f64 6973 742c 2073 6861 7065 5b3a  sd_dist, shape[:
-00009ad0: 2d31 5d29 0a0a 2020 2020 2020 2020 2320  -1])..        # 
-00009ae0: 4372 6561 7465 206e 6577 2072 6e67 2066  Create new rng f
-00009af0: 6f72 2074 6865 205f 6c6b 6a63 686f 6c65  or the _lkjchole
-00009b00: 736b 7963 6f76 2069 6e74 6572 6e61 6c20  skycov internal 
-00009b10: 5256 0a20 2020 2020 2020 2072 6e67 203d  RV.        rng =
-00009b20: 2070 7974 656e 736f 722e 7368 6172 6564   pytensor.shared
-00009b30: 286e 702e 7261 6e64 6f6d 2e64 6566 6175  (np.random.defau
-00009b40: 6c74 5f72 6e67 2829 290a 0a20 2020 2020  lt_rng())..     
-00009b50: 2020 2072 6e67 5f2c 206e 5f2c 2065 7461     rng_, n_, eta
-00009b60: 5f2c 2073 645f 6469 7374 5f20 3d20 726e  _, sd_dist_ = rn
-00009b70: 672e 7479 7065 2829 2c20 6e2e 7479 7065  g.type(), n.type
-00009b80: 2829 2c20 6574 612e 7479 7065 2829 2c20  (), eta.type(), 
-00009b90: 7364 5f64 6973 742e 7479 7065 2829 0a20  sd_dist.type(). 
-00009ba0: 2020 2020 2020 206e 6578 745f 726e 675f         next_rng_
-00009bb0: 2c20 6c6b 6a63 6f76 5f20 3d20 5f6c 6a6b  , lkjcov_ = _ljk
-00009bc0: 5f63 686f 6c65 736b 795f 636f 765f 6261  _cholesky_cov_ba
-00009bd0: 7365 286e 5f2c 2065 7461 5f2c 2073 645f  se(n_, eta_, sd_
-00009be0: 6469 7374 5f2c 2072 6e67 3d72 6e67 5f29  dist_, rng=rng_)
-00009bf0: 2e6f 776e 6572 2e6f 7574 7075 7473 0a0a  .owner.outputs..
-00009c00: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00009c10: 4c4b 4a43 686f 6c65 736b 7943 6f76 5256  LKJCholeskyCovRV
-00009c20: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-00009c30: 7075 7473 3d5b 726e 675f 2c20 6e5f 2c20  puts=[rng_, n_, 
-00009c40: 6574 615f 2c20 7364 5f64 6973 745f 5d2c  eta_, sd_dist_],
-00009c50: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00009c60: 7075 7473 3d5b 6e65 7874 5f72 6e67 5f2c  puts=[next_rng_,
-00009c70: 206c 6b6a 636f 765f 5d2c 0a20 2020 2020   lkjcov_],.     
-00009c80: 2020 2020 2020 206e 6469 6d5f 7375 7070         ndim_supp
-00009c90: 3d31 2c0a 2020 2020 2020 2020 2928 726e  =1,.        )(rn
-00009ca0: 672c 206e 2c20 6574 612c 2073 645f 6469  g, n, eta, sd_di
-00009cb0: 7374 290a 0a0a 405f 6368 616e 6765 5f64  st)...@_change_d
-00009cc0: 6973 745f 7369 7a65 2e72 6567 6973 7465  ist_size.registe
-00009cd0: 7228 5f4c 4b4a 4368 6f6c 6573 6b79 436f  r(_LKJCholeskyCo
-00009ce0: 7652 5629 0a64 6566 2063 6861 6e67 655f  vRV).def change_
-00009cf0: 4c4b 4a43 686f 6c65 6b73 7943 6f76 5256  LKJCholeksyCovRV
-00009d00: 5f73 697a 6528 6f70 2c20 6469 7374 2c20  _size(op, dist, 
-00009d10: 6e65 775f 7369 7a65 2c20 6578 7061 6e64  new_size, expand
-00009d20: 3d46 616c 7365 293a 0a20 2020 206e 2c20  =False):.    n, 
-00009d30: 6574 612c 2073 645f 6469 7374 203d 2064  eta, sd_dist = d
-00009d40: 6973 742e 6f77 6e65 722e 696e 7075 7473  ist.owner.inputs
-00009d50: 5b31 3a5d 0a0a 2020 2020 6966 2065 7870  [1:]..    if exp
-00009d60: 616e 643a 0a20 2020 2020 2020 206f 6c64  and:.        old
-00009d70: 5f73 697a 6520 3d20 7364 5f64 6973 742e  _size = sd_dist.
-00009d80: 7368 6170 655b 3a2d 315d 0a20 2020 2020  shape[:-1].     
-00009d90: 2020 206e 6577 5f73 697a 6520 3d20 7475     new_size = tu
-00009da0: 706c 6528 6e65 775f 7369 7a65 2920 2b20  ple(new_size) + 
-00009db0: 7475 706c 6528 6f6c 645f 7369 7a65 290a  tuple(old_size).
-00009dc0: 0a20 2020 2072 6574 7572 6e20 5f4c 4b4a  .    return _LKJ
-00009dd0: 4368 6f6c 6573 6b79 436f 762e 7276 5f6f  CholeskyCov.rv_o
-00009de0: 7028 6e2c 2065 7461 2c20 7364 5f64 6973  p(n, eta, sd_dis
-00009df0: 742c 2073 697a 653d 6e65 775f 7369 7a65  t, size=new_size
-00009e00: 290a 0a0a 405f 6d6f 6d65 6e74 2e72 6567  )...@_moment.reg
-00009e10: 6973 7465 7228 5f4c 4b4a 4368 6f6c 6573  ister(_LKJCholes
-00009e20: 6b79 436f 7652 5629 0a64 6566 205f 4c4b  kyCovRV).def _LK
-00009e30: 4a43 686f 6c65 6b73 7943 6f76 5256 5f6d  JCholeksyCovRV_m
-00009e40: 6f6d 656e 7428 6f70 2c20 7276 2c20 726e  oment(op, rv, rn
-00009e50: 672c 206e 2c20 6574 612c 2073 645f 6469  g, n, eta, sd_di
-00009e60: 7374 293a 0a20 2020 2064 6961 675f 6964  st):.    diag_id
-00009e70: 7873 203d 2028 7074 2e63 756d 7375 6d28  xs = (pt.cumsum(
-00009e80: 7074 2e61 7261 6e67 6528 312c 206e 202b  pt.arange(1, n +
-00009e90: 2031 2929 202d 2031 292e 6173 7479 7065   1)) - 1).astype
-00009ea0: 2822 696e 7433 3222 290a 2020 2020 6d6f  ("int32").    mo
-00009eb0: 6d65 6e74 203d 2070 742e 7a65 726f 735f  ment = pt.zeros_
-00009ec0: 6c69 6b65 2872 7629 0a20 2020 206d 6f6d  like(rv).    mom
-00009ed0: 656e 7420 3d20 7074 2e73 6574 5f73 7562  ent = pt.set_sub
-00009ee0: 7465 6e73 6f72 286d 6f6d 656e 745b 2e2e  tensor(moment[..
-00009ef0: 2e2c 2064 6961 675f 6964 7873 5d2c 2031  ., diag_idxs], 1
-00009f00: 290a 2020 2020 7265 7475 726e 206d 6f6d  ).    return mom
-00009f10: 656e 740a 0a0a 405f 6465 6661 756c 745f  ent...@_default_
-00009f20: 7472 616e 7366 6f72 6d2e 7265 6769 7374  transform.regist
-00009f30: 6572 285f 4c4b 4a43 686f 6c65 736b 7943  er(_LKJCholeskyC
-00009f40: 6f76 5256 290a 6465 6620 5f4c 4b4a 4368  ovRV).def _LKJCh
-00009f50: 6f6c 656b 7379 436f 7652 565f 6465 6661  oleksyCovRV_defa
-00009f60: 756c 745f 7472 616e 7366 6f72 6d28 6f70  ult_transform(op
-00009f70: 2c20 7276 293a 0a20 2020 205f 2c20 6e2c  , rv):.    _, n,
-00009f80: 205f 2c20 5f20 3d20 7276 2e6f 776e 6572   _, _ = rv.owner
-00009f90: 2e69 6e70 7574 730a 2020 2020 7265 7475  .inputs.    retu
-00009fa0: 726e 2074 7261 6e73 666f 726d 732e 4368  rn transforms.Ch
-00009fb0: 6f6c 6573 6b79 436f 7650 6163 6b65 6428  oleskyCovPacked(
-00009fc0: 6e29 0a0a 0a40 5f6c 6f67 7072 6f62 2e72  n)...@_logprob.r
-00009fd0: 6567 6973 7465 7228 5f4c 4b4a 4368 6f6c  egister(_LKJChol
-00009fe0: 6573 6b79 436f 7652 5629 0a64 6566 205f  eskyCovRV).def _
-00009ff0: 4c4b 4a43 686f 6c65 6b73 7943 6f76 5256  LKJCholeksyCovRV
-0000a000: 5f6c 6f67 7028 6f70 2c20 7661 6c75 6573  _logp(op, values
-0000a010: 2c20 726e 672c 206e 2c20 6574 612c 2073  , rng, n, eta, s
-0000a020: 645f 6469 7374 2c20 2a2a 6b77 6172 6773  d_dist, **kwargs
-0000a030: 293a 0a20 2020 2028 7661 6c75 652c 2920  ):.    (value,) 
-0000a040: 3d20 7661 6c75 6573 0a0a 2020 2020 6966  = values..    if
-0000a050: 2076 616c 7565 2e6e 6469 6d20 3e20 313a   value.ndim > 1:
-0000a060: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-0000a070: 616c 7565 4572 726f 7228 225f 4c4b 4a43  alueError("_LKJC
-0000a080: 686f 6c65 736b 7943 6f76 206c 6f67 7020  holeskyCov logp 
-0000a090: 6973 206f 6e6c 7920 696d 706c 656d 656e  is only implemen
-0000a0a0: 7465 6420 666f 7220 7665 6374 6f72 2076  ted for vector v
-0000a0b0: 616c 7565 7320 286e 6469 6d3d 3129 2229  alues (ndim=1)")
-0000a0c0: 0a0a 2020 2020 6469 6167 5f69 6478 7320  ..    diag_idxs 
-0000a0d0: 3d20 7074 2e63 756d 7375 6d28 7074 2e61  = pt.cumsum(pt.a
-0000a0e0: 7261 6e67 6528 312c 206e 202b 2031 2929  range(1, n + 1))
-0000a0f0: 202d 2031 0a20 2020 2063 756d 7375 6d20   - 1.    cumsum 
-0000a100: 3d20 7074 2e63 756d 7375 6d28 7661 6c75  = pt.cumsum(valu
-0000a110: 652a 2a32 290a 2020 2020 7661 7269 616e  e**2).    varian
-0000a120: 6365 203d 2070 742e 7a65 726f 7328 7074  ce = pt.zeros(pt
-0000a130: 2e61 746c 6561 7374 5f31 6428 6e29 290a  .atleast_1d(n)).
-0000a140: 2020 2020 7661 7269 616e 6365 203d 2070      variance = p
-0000a150: 742e 696e 635f 7375 6274 656e 736f 7228  t.inc_subtensor(
-0000a160: 7661 7269 616e 6365 5b30 5d2c 2076 616c  variance[0], val
-0000a170: 7565 5b30 5d20 2a2a 2032 290a 2020 2020  ue[0] ** 2).    
-0000a180: 7661 7269 616e 6365 203d 2070 742e 696e  variance = pt.in
-0000a190: 635f 7375 6274 656e 736f 7228 7661 7269  c_subtensor(vari
-0000a1a0: 616e 6365 5b31 3a5d 2c20 6375 6d73 756d  ance[1:], cumsum
-0000a1b0: 5b64 6961 675f 6964 7873 5b31 3a5d 5d20  [diag_idxs[1:]] 
-0000a1c0: 2d20 6375 6d73 756d 5b64 6961 675f 6964  - cumsum[diag_id
-0000a1d0: 7873 5b3a 2d31 5d5d 290a 2020 2020 7364  xs[:-1]]).    sd
-0000a1e0: 5f76 616c 7320 3d20 7074 2e73 7172 7428  _vals = pt.sqrt(
-0000a1f0: 7661 7269 616e 6365 290a 0a20 2020 206c  variance)..    l
-0000a200: 6f67 705f 7364 203d 2070 6d2e 6c6f 6770  ogp_sd = pm.logp
-0000a210: 2873 645f 6469 7374 2c20 7364 5f76 616c  (sd_dist, sd_val
-0000a220: 7329 2e73 756d 2829 0a20 2020 2063 6f72  s).sum().    cor
-0000a230: 725f 6469 6167 203d 2076 616c 7565 5b64  r_diag = value[d
-0000a240: 6961 675f 6964 7873 5d20 2f20 7364 5f76  iag_idxs] / sd_v
-0000a250: 616c 730a 0a20 2020 206c 6f67 705f 6c6b  als..    logp_lk
-0000a260: 6a20 3d20 2832 202a 2065 7461 202d 2033  j = (2 * eta - 3
-0000a270: 202b 206e 202d 2070 742e 6172 616e 6765   + n - pt.arange
-0000a280: 286e 2929 202a 2070 742e 6c6f 6728 636f  (n)) * pt.log(co
-0000a290: 7272 5f64 6961 6729 0a20 2020 206c 6f67  rr_diag).    log
-0000a2a0: 705f 6c6b 6a20 3d20 7074 2e73 756d 286c  p_lkj = pt.sum(l
-0000a2b0: 6f67 705f 6c6b 6a29 0a0a 2020 2020 2320  ogp_lkj)..    # 
-0000a2c0: 436f 6d70 7574 6520 7468 6520 6c6f 6720  Compute the log 
-0000a2d0: 6465 7420 6a61 636f 6269 616e 206f 6620  det jacobian of 
-0000a2e0: 7468 6520 7365 636f 6e64 2074 7261 6e73  the second trans
-0000a2f0: 666f 726d 6174 696f 6e0a 2020 2020 2320  formation.    # 
-0000a300: 6465 7363 7269 6265 6420 696e 2074 6865  described in the
-0000a310: 2064 6f63 7374 7269 6e67 2e0a 2020 2020   docstring..    
-0000a320: 6964 7820 3d20 7074 2e61 7261 6e67 6528  idx = pt.arange(
-0000a330: 6e29 0a20 2020 2064 6574 5f69 6e76 6a61  n).    det_invja
-0000a340: 6320 3d20 7074 2e6c 6f67 2863 6f72 725f  c = pt.log(corr_
-0000a350: 6469 6167 2920 2d20 6964 7820 2a20 7074  diag) - idx * pt
-0000a360: 2e6c 6f67 2873 645f 7661 6c73 290a 2020  .log(sd_vals).  
-0000a370: 2020 6465 745f 696e 766a 6163 203d 2064    det_invjac = d
-0000a380: 6574 5f69 6e76 6a61 632e 7375 6d28 290a  et_invjac.sum().
-0000a390: 0a20 2020 2023 2054 4f44 4f3a 205f 6c6b  .    # TODO: _lk
-0000a3a0: 6a5f 6e6f 726d 616c 697a 696e 675f 636f  j_normalizing_co
-0000a3b0: 6e73 7461 6e74 2063 7572 7265 6e74 6c79  nstant currently
-0000a3c0: 2072 6571 7569 7265 7320 6065 7461 6020   requires `eta` 
-0000a3d0: 616e 6420 606e 6020 746f 2062 6520 636f  and `n` to be co
-0000a3e0: 6e73 7461 6e74 730a 2020 2020 6966 206e  nstants.    if n
-0000a3f0: 6f74 2069 7369 6e73 7461 6e63 6528 6e2c  ot isinstance(n,
-0000a400: 2043 6f6e 7374 616e 7429 3a0a 2020 2020   Constant):.    
-0000a410: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000a420: 6c65 6d65 6e74 6564 4572 726f 7228 226c  lementedError("l
-0000a430: 6f67 7020 6f6e 6c79 2069 6d70 6c65 6d65  ogp only impleme
-0000a440: 6e74 6564 2066 6f72 2063 6f6e 7374 616e  nted for constan
-0000a450: 7420 606e 6022 290a 2020 2020 6e20 3d20  t `n`").    n = 
-0000a460: 696e 7428 6e2e 6461 7461 290a 0a20 2020  int(n.data)..   
-0000a470: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-0000a480: 6365 2865 7461 2c20 436f 6e73 7461 6e74  ce(eta, Constant
-0000a490: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-0000a4a0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-0000a4b0: 7272 6f72 2822 6c6f 6770 206f 6e6c 7920  rror("logp only 
-0000a4c0: 696d 706c 656d 656e 7465 6420 666f 7220  implemented for 
-0000a4d0: 636f 6e73 7461 6e74 2060 6574 6160 2229  constant `eta`")
-0000a4e0: 0a20 2020 2065 7461 203d 2066 6c6f 6174  .    eta = float
-0000a4f0: 2865 7461 2e64 6174 6129 0a0a 2020 2020  (eta.data)..    
-0000a500: 6e6f 726d 203d 205f 6c6b 6a5f 6e6f 726d  norm = _lkj_norm
-0000a510: 616c 697a 696e 675f 636f 6e73 7461 6e74  alizing_constant
-0000a520: 2865 7461 2c20 6e29 0a0a 2020 2020 7265  (eta, n)..    re
-0000a530: 7475 726e 206e 6f72 6d20 2b20 6c6f 6770  turn norm + logp
-0000a540: 5f6c 6b6a 202b 206c 6f67 705f 7364 202b  _lkj + logp_sd +
-0000a550: 2064 6574 5f69 6e76 6a61 630a 0a0a 636c   det_invjac...cl
-0000a560: 6173 7320 4c4b 4a43 686f 6c65 736b 7943  ass LKJCholeskyC
-0000a570: 6f76 3a0a 2020 2020 7222 2222 5772 6170  ov:.    r"""Wrap
-0000a580: 7065 7220 636c 6173 7320 666f 7220 636f  per class for co
-0000a590: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
-0000a5a0: 7769 7468 204c 4b4a 2064 6973 7472 6962  with LKJ distrib
-0000a5b0: 7574 6564 2063 6f72 7265 6c61 7469 6f6e  uted correlation
-0000a5c0: 732e 0a0a 2020 2020 5468 6973 2064 6566  s...    This def
-0000a5d0: 696e 6573 2061 2064 6973 7472 6962 7574  ines a distribut
-0000a5e0: 696f 6e20 6f76 6572 2043 686f 6c65 736b  ion over Cholesk
-0000a5f0: 7920 6465 636f 6d70 6f73 6564 2063 6f76  y decomposed cov
-0000a600: 6172 6961 6e63 650a 2020 2020 6d61 7472  ariance.    matr
-0000a610: 6963 6573 2c20 7375 6368 2074 6861 7420  ices, such that 
-0000a620: 7468 6520 756e 6465 726c 7969 6e67 2063  the underlying c
-0000a630: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
-0000a640: 6365 7320 666f 6c6c 6f77 2061 6e0a 2020  ces follow an.  
-0000a650: 2020 4c4b 4a20 6469 7374 7269 6275 7469    LKJ distributi
-0000a660: 6f6e 205b 315d 2061 6e64 2074 6865 2073  on [1] and the s
-0000a670: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
-0000a680: 6e73 2066 6f6c 6c6f 7720 616e 2061 7262  ns follow an arb
-0000a690: 6974 7261 7279 0a20 2020 2064 6973 7472  itrary.    distr
-0000a6a0: 6962 7574 696f 6e20 7370 6563 6966 6965  ibution specifie
-0000a6b0: 6420 6279 2074 6865 2075 7365 722e 0a0a  d by the user...
-0000a6c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000a6d0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000a6e0: 2020 6e61 6d65 203a 2073 7472 0a20 2020    name : str.   
-0000a6f0: 2020 2020 2054 6865 206e 616d 6520 6769       The name gi
-0000a700: 7665 6e20 746f 2074 6865 2076 6172 6961  ven to the varia
-0000a710: 626c 6520 696e 2074 6865 206d 6f64 656c  ble in the model
-0000a720: 2e0a 2020 2020 6574 6120 3a20 7465 6e73  ..    eta : tens
-0000a730: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-0000a740: 0a20 2020 2020 2020 2054 6865 2073 6861  .        The sha
-0000a750: 7065 2070 6172 616d 6574 6572 2028 6574  pe parameter (et
-0000a760: 6120 3e20 3029 206f 6620 7468 6520 4c4b  a > 0) of the LK
-0000a770: 4a20 6469 7374 7269 6275 7469 6f6e 2e20  J distribution. 
-0000a780: 6574 6120 3d20 310a 2020 2020 2020 2020  eta = 1.        
-0000a790: 696d 706c 6965 7320 6120 756e 6966 6f72  implies a unifor
-0000a7a0: 6d20 6469 7374 7269 6275 7469 6f6e 206f  m distribution o
-0000a7b0: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
-0000a7c0: 6e20 6d61 7472 6963 6573 3b0a 2020 2020  n matrices;.    
-0000a7d0: 2020 2020 6c61 7267 6572 2076 616c 7565      larger value
-0000a7e0: 7320 7075 7420 6d6f 7265 2077 6569 6768  s put more weigh
-0000a7f0: 7420 6f6e 206d 6174 7269 6365 7320 7769  t on matrices wi
-0000a800: 7468 2066 6577 2063 6f72 7265 6c61 7469  th few correlati
-0000a810: 6f6e 732e 0a20 2020 206e 203a 2074 656e  ons..    n : ten
-0000a820: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
-0000a830: 2020 2020 2020 2020 4469 6d65 6e73 696f          Dimensio
-0000a840: 6e20 6f66 2074 6865 2063 6f76 6172 6961  n of the covaria
-0000a850: 6e63 6520 6d61 7472 6978 2028 6e20 3e20  nce matrix (n > 
-0000a860: 3129 2e0a 2020 2020 7364 5f64 6973 7420  1)..    sd_dist 
-0000a870: 3a20 4469 7374 7269 6275 7469 6f6e 0a20  : Distribution. 
-0000a880: 2020 2020 2020 2041 2070 6f73 6974 6976         A positiv
-0000a890: 6520 7363 616c 6172 206f 7220 7665 6374  e scalar or vect
-0000a8a0: 6f72 2064 6973 7472 6962 7574 696f 6e20  or distribution 
-0000a8b0: 666f 7220 7468 6520 7374 616e 6461 7264  for the standard
-0000a8c0: 2064 6576 6961 7469 6f6e 732c 2063 7265   deviations, cre
-0000a8d0: 6174 6564 0a20 2020 2020 2020 2077 6974  ated.        wit
-0000a8e0: 6820 7468 6520 602e 6469 7374 2829 6020  h the `.dist()` 
-0000a8f0: 4150 492e 2053 686f 756c 6420 6861 7665  API. Should have
-0000a900: 2060 7368 6170 655b 2d31 5d3d 6e60 2e20   `shape[-1]=n`. 
-0000a910: 5363 616c 6172 2064 6973 7472 6962 7574  Scalar distribut
-0000a920: 696f 6e73 2077 696c 6c20 6265 0a20 2020  ions will be.   
-0000a930: 2020 2020 2061 7574 6f6d 6174 6963 616c       automatical
-0000a940: 6c79 2072 6573 697a 6564 2074 6f20 656e  ly resized to en
-0000a950: 7375 7265 2074 6869 732e 0a0a 2020 2020  sure this...    
-0000a960: 2020 2020 2e2e 2077 6172 6e69 6e67 3a3a      .. warning::
-0000a970: 2073 645f 6469 7374 2077 696c 6c20 6265   sd_dist will be
-0000a980: 2063 6c6f 6e65 642c 2072 656e 6465 7269   cloned, renderi
-0000a990: 6e67 2069 7420 696e 6465 7065 6e64 656e  ng it independen
-0000a9a0: 7420 6f66 2074 6865 206f 6e65 2070 6173  t of the one pas
-0000a9b0: 7365 6420 6173 2069 6e70 7574 2e0a 0a20  sed as input... 
-0000a9c0: 2020 2063 6f6d 7075 7465 5f63 6f72 7220     compute_corr 
-0000a9d0: 3a20 626f 6f6c 2c20 6465 6661 756c 743d  : bool, default=
-0000a9e0: 5472 7565 0a20 2020 2020 2020 2049 6620  True.        If 
-0000a9f0: 6054 7275 6560 2c20 7265 7475 726e 7320  `True`, returns 
-0000aa00: 7468 7265 6520 7661 6c75 6573 3a20 7468  three values: th
-0000aa10: 6520 4368 6f6c 6573 6b79 2064 6563 6f6d  e Cholesky decom
-0000aa20: 706f 7369 7469 6f6e 2c20 7468 6520 636f  position, the co
-0000aa30: 7272 656c 6174 696f 6e73 0a20 2020 2020  rrelations.     
-0000aa40: 2020 2061 6e64 2074 6865 2073 7461 6e64     and the stand
-0000aa50: 6172 6420 6465 7669 6174 696f 6e73 206f  ard deviations o
-0000aa60: 6620 7468 6520 636f 7661 7269 616e 6365  f the covariance
-0000aa70: 206d 6174 7269 782e 204f 7468 6572 7769   matrix. Otherwi
-0000aa80: 7365 2c20 6f6e 6c79 2072 6574 7572 6e73  se, only returns
-0000aa90: 0a20 2020 2020 2020 2074 6865 2070 6163  .        the pac
-0000aaa0: 6b65 6420 4368 6f6c 6573 6b79 2064 6563  ked Cholesky dec
-0000aab0: 6f6d 706f 7369 7469 6f6e 2e20 4465 6661  omposition. Defa
-0000aac0: 756c 7473 2074 6f20 6054 7275 6560 2e0a  ults to `True`..
-0000aad0: 2020 2020 2020 2020 636f 6d70 6174 6962          compatib
-0000aae0: 696c 6974 792e 0a20 2020 2073 746f 7265  ility..    store
-0000aaf0: 5f69 6e5f 7472 6163 6520 3a20 626f 6f6c  _in_trace : bool
-0000ab00: 2c20 6465 6661 756c 743d 5472 7565 0a20  , default=True. 
-0000ab10: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-0000ab20: 6f20 7374 6f72 6520 7468 6520 636f 7272  o store the corr
-0000ab30: 656c 6174 696f 6e73 2061 6e64 2073 7461  elations and sta
-0000ab40: 6e64 6172 6420 6465 7669 6174 696f 6e73  ndard deviations
-0000ab50: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
-0000ab60: 6365 0a20 2020 2020 2020 206d 6174 7269  ce.        matri
-0000ab70: 7820 696e 2074 6865 2070 6f73 7465 7269  x in the posteri
-0000ab80: 6f72 2074 7261 6365 2e20 4966 2060 5472  or trace. If `Tr
-0000ab90: 7565 602c 2074 6865 7920 7769 6c6c 2061  ue`, they will a
-0000aba0: 7574 6f6d 6174 6963 616c 6c79 2062 6520  utomatically be 
-0000abb0: 6e61 6d65 6420 6173 0a20 2020 2020 2020  named as.       
-0000abc0: 2060 7b6e 616d 657d 5f63 6f72 7260 2061   `{name}_corr` a
-0000abd0: 6e64 2060 7b6e 616d 657d 5f73 7464 7360  nd `{name}_stds`
-0000abe0: 2072 6573 7065 6374 6976 656c 792e 2045   respectively. E
-0000abf0: 6666 6563 7469 7665 206f 6e6c 7920 7768  ffective only wh
-0000ac00: 656e 0a20 2020 2020 2020 2060 636f 6d70  en.        `comp
-0000ac10: 7574 655f 636f 7272 3d54 7275 6560 2e0a  ute_corr=True`..
-0000ac20: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0000ac30: 202d 2d2d 2d2d 2d2d 0a20 2020 2063 686f   -------.    cho
-0000ac40: 6c20 3a20 2054 656e 736f 7256 6172 6961  l :  TensorVaria
-0000ac50: 626c 650a 2020 2020 2020 2020 4966 2060  ble.        If `
-0000ac60: 636f 6d70 7574 655f 636f 7272 3d54 7275  compute_corr=Tru
-0000ac70: 6560 2e20 5468 6520 756e 7061 636b 6564  e`. The unpacked
-0000ac80: 2043 686f 6c65 736b 7920 636f 7661 7269   Cholesky covari
-0000ac90: 616e 6365 2064 6563 6f6d 706f 7369 7469  ance decompositi
-0000aca0: 6f6e 2e0a 2020 2020 636f 7272 203a 2054  on..    corr : T
-0000acb0: 656e 736f 7256 6172 6961 626c 650a 2020  ensorVariable.  
-0000acc0: 2020 2020 2020 4966 2060 636f 6d70 7574        If `comput
-0000acd0: 655f 636f 7272 3d54 7275 6560 2e20 5468  e_corr=True`. Th
-0000ace0: 6520 636f 7272 656c 6174 696f 6e73 206f  e correlations o
-0000acf0: 6620 7468 6520 636f 7661 7269 616e 6365  f the covariance
-0000ad00: 206d 6174 7269 782e 0a20 2020 2073 7464   matrix..    std
-0000ad10: 7320 3a20 5465 6e73 6f72 5661 7269 6162  s : TensorVariab
-0000ad20: 6c65 0a20 2020 2020 2020 2049 6620 6063  le.        If `c
-0000ad30: 6f6d 7075 7465 5f63 6f72 723d 5472 7565  ompute_corr=True
-0000ad40: 602e 2054 6865 2073 7461 6e64 6172 6420  `. The standard 
-0000ad50: 6465 7669 6174 696f 6e73 206f 6620 7468  deviations of th
-0000ad60: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
-0000ad70: 7269 782e 0a20 2020 2070 6163 6b65 645f  rix..    packed_
-0000ad80: 6368 6f6c 203a 2054 656e 736f 7256 6172  chol : TensorVar
-0000ad90: 6961 626c 650a 2020 2020 2020 2020 4966  iable.        If
-0000ada0: 2060 636f 6d70 7574 655f 636f 7272 3d46   `compute_corr=F
-0000adb0: 616c 7365 6020 5468 6520 7061 636b 6564  alse` The packed
-0000adc0: 2043 686f 6c65 736b 7920 636f 7661 7269   Cholesky covari
-0000add0: 616e 6365 2064 6563 6f6d 706f 7369 7469  ance decompositi
-0000ade0: 6f6e 2e0a 0a20 2020 204e 6f74 6573 0a20  on...    Notes. 
-0000adf0: 2020 202d 2d2d 2d2d 0a20 2020 2053 696e     -----.    Sin
-0000ae00: 6365 2074 6865 2043 686f 6c65 736b 7920  ce the Cholesky 
-0000ae10: 6661 6374 6f72 2069 7320 6120 6c6f 7765  factor is a lowe
-0000ae20: 7220 7472 6961 6e67 756c 6172 206d 6174  r triangular mat
-0000ae30: 7269 782c 2077 6520 7573 6520 7061 636b  rix, we use pack
-0000ae40: 6564 2073 746f 7261 6765 2066 6f72 0a20  ed storage for. 
-0000ae50: 2020 2074 6865 206d 6174 7269 783a 2057     the matrix: W
-0000ae60: 6520 7374 6f72 6520 7468 6520 7661 6c75  e store the valu
-0000ae70: 6573 206f 6620 7468 6520 6c6f 7765 7220  es of the lower 
-0000ae80: 7472 6961 6e67 756c 6172 206d 6174 7269  triangular matri
-0000ae90: 7820 696e 2061 206f 6e65 2d64 696d 656e  x in a one-dimen
-0000aea0: 7369 6f6e 616c 0a20 2020 2061 7272 6179  sional.    array
-0000aeb0: 2c20 6e75 6d62 6572 6564 2062 7920 726f  , numbered by ro
-0000aec0: 773a 3a0a 0a20 2020 2020 2020 205b 5b30  w::..        [[0
-0000aed0: 202d 202d 202d 5d0a 2020 2020 2020 2020   - - -].        
-0000aee0: 205b 3120 3220 2d20 2d5d 0a20 2020 2020   [1 2 - -].     
-0000aef0: 2020 2020 5b33 2034 2035 202d 5d0a 2020      [3 4 5 -].  
-0000af00: 2020 2020 2020 205b 3620 3720 3820 395d         [6 7 8 9]
-0000af10: 5d0a 0a20 2020 2054 6865 2075 6e70 6163  ]..    The unpac
-0000af20: 6b65 6420 4368 6f6c 6573 6b79 2063 6f76  ked Cholesky cov
-0000af30: 6172 6961 6e63 6520 6d61 7472 6978 2069  ariance matrix i
-0000af40: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
-0000af50: 636f 6d70 7574 6564 2061 6e64 2072 6574  computed and ret
-0000af60: 7572 6e65 6420 7768 656e 0a20 2020 2079  urned when.    y
-0000af70: 6f75 2073 7065 6369 6679 2060 636f 6d70  ou specify `comp
-0000af80: 7574 655f 636f 7272 3d54 7275 6560 2069  ute_corr=True` i
-0000af90: 6e20 6070 6d2e 4c4b 4a43 686f 6c65 736b  n `pm.LKJCholesk
-0000afa0: 7943 6f76 6020 2873 6565 2065 7861 6d70  yCov` (see examp
-0000afb0: 6c65 2062 656c 6f77 292e 0a20 2020 204f  le below)..    O
-0000afc0: 7468 6572 7769 7365 2c20 796f 7520 6361  therwise, you ca
-0000afd0: 6e20 7573 6520 6070 6d2e 6578 7061 6e64  n use `pm.expand
-0000afe0: 5f70 6163 6b65 645f 7472 6961 6e67 756c  _packed_triangul
-0000aff0: 6172 2870 6163 6b65 645f 636f 762c 206c  ar(packed_cov, l
-0000b000: 6f77 6572 3d54 7275 6529 600a 2020 2020  ower=True)`.    
-0000b010: 746f 2063 6f6e 7665 7274 2074 6865 2070  to convert the p
-0000b020: 6163 6b65 6420 4368 6f6c 6573 6b79 206d  acked Cholesky m
-0000b030: 6174 7269 7820 746f 2061 2072 6567 756c  atrix to a regul
-0000b040: 6172 2074 776f 2d64 696d 656e 7369 6f6e  ar two-dimension
-0000b050: 616c 2061 7272 6179 2e0a 0a20 2020 2045  al array...    E
-0000b060: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-0000b070: 2d2d 2d2d 0a20 2020 202e 2e20 636f 6465  ----.    .. code
-0000b080: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-0000b090: 2020 2077 6974 6820 706d 2e4d 6f64 656c     with pm.Model
-0000b0a0: 2829 2061 7320 6d6f 6465 6c3a 0a20 2020  () as model:.   
-0000b0b0: 2020 2020 2020 2020 2023 204e 6f74 6520           # Note 
-0000b0c0: 7468 6174 2077 6520 6163 6365 7373 2074  that we access t
-0000b0d0: 6865 2064 6973 7472 6962 7574 696f 6e20  he distribution 
-0000b0e0: 666f 7220 7468 6520 7374 616e 6461 7264  for the standard
-0000b0f0: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
-0000b100: 6576 6961 7469 6f6e 732c 2061 6e64 2064  eviations, and d
-0000b110: 6f20 6e6f 7420 6372 6561 7465 2061 206e  o not create a n
-0000b120: 6577 2072 616e 646f 6d20 7661 7269 6162  ew random variab
-0000b130: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
-0000b140: 7364 5f64 6973 7420 3d20 706d 2e45 7870  sd_dist = pm.Exp
-0000b150: 6f6e 656e 7469 616c 2e64 6973 7428 312e  onential.dist(1.
-0000b160: 302c 2073 697a 653d 3130 290a 2020 2020  0, size=10).    
-0000b170: 2020 2020 2020 2020 6368 6f6c 2c20 636f          chol, co
-0000b180: 7272 2c20 7369 676d 6173 203d 2070 6d2e  rr, sigmas = pm.
-0000b190: 4c4b 4a43 686f 6c65 736b 7943 6f76 280a  LKJCholeskyCov(.
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 2763 686f 6c5f 636f 7627 2c20 6574 613d  'chol_cov', eta=
-0000b1c0: 342c 206e 3d31 302c 2073 645f 6469 7374  4, n=10, sd_dist
-0000b1d0: 3d73 645f 6469 7374 0a20 2020 2020 2020  =sd_dist.       
-0000b1e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b1f0: 2020 2020 2320 6966 2079 6f75 206f 6e6c      # if you onl
-0000b200: 7920 7761 6e74 2074 6865 2070 6163 6b65  y want the packe
-0000b210: 6420 4368 6f6c 6573 6b79 3a0a 2020 2020  d Cholesky:.    
-0000b220: 2020 2020 2020 2020 2320 7061 636b 6564          # packed
-0000b230: 5f63 686f 6c20 3d20 706d 2e4c 4b4a 4368  _chol = pm.LKJCh
-0000b240: 6f6c 6573 6b79 436f 7628 0a20 2020 2020  oleskyCov(.     
-0000b250: 2020 2020 2020 2020 2020 2027 6368 6f6c             'chol
-0000b260: 5f63 6f76 272c 2065 7461 3d34 2c20 6e3d  _cov', eta=4, n=
-0000b270: 3130 2c20 7364 5f64 6973 743d 7364 5f64  10, sd_dist=sd_d
-0000b280: 6973 742c 2063 6f6d 7075 7465 5f63 6f72  ist, compute_cor
-0000b290: 723d 4661 6c73 650a 2020 2020 2020 2020  r=False.        
-0000b2a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000b2b0: 2020 2320 6368 6f6c 203d 2070 6d2e 6578    # chol = pm.ex
-0000b2c0: 7061 6e64 5f70 6163 6b65 645f 7472 6961  pand_packed_tria
-0000b2d0: 6e67 756c 6172 2831 302c 2070 6163 6b65  ngular(10, packe
-0000b2e0: 645f 6368 6f6c 2c20 6c6f 7765 723d 5472  d_chol, lower=Tr
-0000b2f0: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
-0000b300: 2023 2044 6566 696e 6520 6120 6e65 7720   # Define a new 
-0000b310: 4d76 4e6f 726d 616c 2077 6974 6820 7468  MvNormal with th
-0000b320: 6520 6769 7665 6e20 636f 7661 7269 616e  e given covarian
-0000b330: 6365 0a20 2020 2020 2020 2020 2020 2076  ce.            v
-0000b340: 616c 7320 3d20 706d 2e4d 764e 6f72 6d61  als = pm.MvNorma
-0000b350: 6c28 2776 616c 7327 2c20 6d75 3d6e 702e  l('vals', mu=np.
-0000b360: 7a65 726f 7328 3130 292c 2063 686f 6c3d  zeros(10), chol=
-0000b370: 6368 6f6c 2c20 7368 6170 653d 3130 290a  chol, shape=10).
-0000b380: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
-0000b390: 7220 7472 616e 7366 6f72 6d20 616e 2075  r transform an u
-0000b3a0: 6e63 6f72 7265 6c61 7465 6420 6e6f 726d  ncorrelated norm
-0000b3b0: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
-0000b3c0: 7661 6c73 5f72 6177 203d 2070 6d2e 4e6f  vals_raw = pm.No
-0000b3d0: 726d 616c 2827 7661 6c73 5f72 6177 272c  rmal('vals_raw',
-0000b3e0: 206d 753d 302c 2073 6967 6d61 3d31 2c20   mu=0, sigma=1, 
-0000b3f0: 7368 6170 653d 3130 290a 2020 2020 2020  shape=10).      
-0000b400: 2020 2020 2020 7661 6c73 203d 2070 742e        vals = pt.
-0000b410: 646f 7428 6368 6f6c 2c20 7661 6c73 5f72  dot(chol, vals_r
-0000b420: 6177 290a 0a20 2020 2020 2020 2020 2020  aw)..           
-0000b430: 2023 204f 7220 636f 6d70 7574 6520 7468   # Or compute th
-0000b440: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
-0000b450: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
-0000b460: 636f 7620 3d20 7074 2e64 6f74 2863 686f  cov = pt.dot(cho
-0000b470: 6c2c 2063 686f 6c2e 5429 0a0a 2020 2020  l, chol.T)..    
-0000b480: 2a2a 496d 706c 656d 656e 7461 7469 6f6e  **Implementation
-0000b490: 2a2a 2049 6e20 7468 6520 756e 636f 6e73  ** In the uncons
-0000b4a0: 7472 6169 6e65 6420 7370 6163 6520 616c  trained space al
-0000b4b0: 6c20 7661 6c75 6573 206f 6620 7468 6520  l values of the 
-0000b4c0: 6368 6f6c 6573 6b79 2066 6163 746f 720a  cholesky factor.
-0000b4d0: 2020 2020 6172 6520 7374 6f72 6564 2075      are stored u
-0000b4e0: 6e74 7261 6e73 666f 726d 6564 2c20 6578  ntransformed, ex
-0000b4f0: 6365 7074 2066 6f72 2074 6865 2064 6961  cept for the dia
-0000b500: 676f 6e61 6c20 656e 7472 6965 732c 2077  gonal entries, w
-0000b510: 6865 7265 0a20 2020 2077 6520 7573 6520  here.    we use 
-0000b520: 6120 6c6f 672d 7472 616e 7366 6f72 6d20  a log-transform 
-0000b530: 746f 2072 6573 7472 6963 7420 7468 656d  to restrict them
-0000b540: 2074 6f20 706f 7369 7469 7665 2076 616c   to positive val
-0000b550: 7565 732e 0a0a 2020 2020 546f 2063 6f72  ues...    To cor
-0000b560: 7265 6374 6c79 2063 6f6d 7075 7465 206c  rectly compute l
-0000b570: 6f67 2d6c 696b 656c 6968 6f6f 6473 2066  og-likelihoods f
-0000b580: 6f72 2074 6865 2073 7461 6e64 6172 6420  or the standard 
-0000b590: 6465 7669 6174 696f 6e73 0a20 2020 2061  deviations.    a
-0000b5a0: 6e64 2074 6865 2063 6f72 7265 6c61 7469  nd the correlati
-0000b5b0: 6f6e 206d 6174 7269 7820 7365 7061 7261  on matrix separa
-0000b5c0: 7465 6c79 2c20 7765 206e 6565 6420 746f  tely, we need to
-0000b5d0: 2063 6f6e 7369 6465 7220 610a 2020 2020   consider a.    
-0000b5e0: 7365 636f 6e64 2074 7261 6e73 666f 726d  second transform
-0000b5f0: 6174 696f 6e3a 2047 6976 656e 2061 2063  ation: Given a c
-0000b600: 686f 6c65 736b 7920 6661 6374 6f72 697a  holesky factoriz
-0000b610: 6174 696f 6e0a 2020 2020 3a6d 6174 683a  ation.    :math:
-0000b620: 604c 4c5e 5420 3d20 5c53 6967 6d61 6020  `LL^T = \Sigma` 
-0000b630: 6f66 2061 2063 6f76 6172 6961 6e63 6520  of a covariance 
-0000b640: 6d61 7472 6978 2077 6520 6361 6e20 7265  matrix we can re
-0000b650: 636f 7665 7220 7468 650a 2020 2020 7374  cover the.    st
-0000b660: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-0000b670: 7320 3a6d 6174 683a 605c 7369 676d 6160  s :math:`\sigma`
-0000b680: 2061 7320 7468 6520 6575 636c 6964 6561   as the euclidea
-0000b690: 6e20 6c65 6e67 7468 7320 6f66 0a20 2020  n lengths of.   
-0000b6a0: 2074 6865 2072 6f77 7320 6f66 203a 6d61   the rows of :ma
-0000b6b0: 7468 3a60 4c60 2c20 616e 6420 7468 6520  th:`L`, and the 
-0000b6c0: 6368 6f6c 6573 6b79 2066 6163 746f 7220  cholesky factor 
-0000b6d0: 6f66 2074 6865 0a20 2020 2063 6f72 7265  of the.    corre
-0000b6e0: 6c61 7469 6f6e 206d 6174 7269 7820 6173  lation matrix as
-0000b6f0: 203a 6d61 7468 3a60 5520 3d20 5c74 6578   :math:`U = \tex
-0000b700: 747b 6469 6167 7d28 5c73 6967 6d61 295e  t{diag}(\sigma)^
-0000b710: 7b2d 317d 4c60 2e0a 2020 2020 5369 6e63  {-1}L`..    Sinc
-0000b720: 6520 6561 6368 2072 6f77 206f 6620 3a6d  e each row of :m
-0000b730: 6174 683a 6055 6020 6861 7320 6c65 6e67  ath:`U` has leng
-0000b740: 7468 2031 2c20 7765 2064 6f20 6e6f 7420  th 1, we do not 
-0000b750: 6e65 6564 2074 6f0a 2020 2020 7374 6f72  need to.    stor
-0000b760: 6520 7468 6520 6469 6167 6f6e 616c 2e20  e the diagonal. 
-0000b770: 5765 2064 6566 696e 6520 6120 7472 616e  We define a tran
-0000b780: 7366 6f72 6d61 7469 6f6e 203a 6d61 7468  sformation :math
-0000b790: 3a60 5c70 6869 600a 2020 2020 7375 6368  :`\phi`.    such
-0000b7a0: 2074 6861 7420 3a6d 6174 683a 605c 7068   that :math:`\ph
-0000b7b0: 6928 4c29 6020 6973 2074 6865 206c 6f77  i(L)` is the low
-0000b7c0: 6572 2074 7269 616e 6775 6c61 7220 6d61  er triangular ma
-0000b7d0: 7472 6978 2063 6f6e 7461 696e 696e 670a  trix containing.
-0000b7e0: 2020 2020 7468 6520 7374 616e 6461 7264      the standard
-0000b7f0: 2064 6576 6961 7469 6f6e 7320 3a6d 6174   deviations :mat
-0000b800: 683a 605c 7369 676d 6160 206f 6e20 7468  h:`\sigma` on th
-0000b810: 6520 6469 6167 6f6e 616c 2061 6e64 2074  e diagonal and t
-0000b820: 6865 0a20 2020 2063 6f72 7265 6c61 7469  he.    correlati
-0000b830: 6f6e 206d 6174 7269 7820 3a6d 6174 683a  on matrix :math:
-0000b840: 6055 6020 6265 6c6f 772e 2049 6e20 7468  `U` below. In th
-0000b850: 6973 2066 6f72 6d20 7765 2063 616e 2065  is form we can e
-0000b860: 6173 696c 790a 2020 2020 636f 6d70 7574  asily.    comput
-0000b870: 6520 7468 6520 6469 6666 6572 656e 7420  e the different 
-0000b880: 6c69 6b65 6c69 686f 6f64 7320 7365 7061  likelihoods sepa
-0000b890: 7261 7465 6c79 2c20 6173 2074 6865 206c  rately, as the l
-0000b8a0: 696b 656c 6968 6f6f 640a 2020 2020 6f66  ikelihood.    of
-0000b8b0: 2074 6865 2063 6f72 7265 6c61 7469 6f6e   the correlation
-0000b8c0: 206d 6174 7269 7820 6f6e 6c79 2064 6570   matrix only dep
-0000b8d0: 656e 6473 206f 6e20 7468 6520 7661 6c75  ends on the valu
-0000b8e0: 6573 2062 656c 6f77 2074 6865 0a20 2020  es below the.   
-0000b8f0: 2064 6961 676f 6e61 6c2c 2061 6e64 2074   diagonal, and t
-0000b900: 6865 206c 696b 656c 6968 6f6f 6420 6f66  he likelihood of
-0000b910: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
-0000b920: 7669 6174 696f 6e20 6465 7065 6e64 730a  viation depends.
-0000b930: 2020 2020 6f6e 6c79 206f 6e20 7468 6520      only on the 
-0000b940: 6469 6167 6f6e 616c 2076 616c 7565 732e  diagonal values.
-0000b950: 0a0a 2020 2020 5765 2073 7469 6c6c 206e  ..    We still n
-0000b960: 6565 6420 7468 6520 6465 7465 726d 696e  eed the determin
-0000b970: 616e 7420 6f66 2074 6865 206a 6163 6f62  ant of the jacob
-0000b980: 6961 6e20 6f66 203a 6d61 7468 3a60 5c70  ian of :math:`\p
-0000b990: 6869 5e7b 2d31 7d60 2e0a 2020 2020 4966  hi^{-1}`..    If
-0000b9a0: 2077 6520 7468 696e 6b20 6f66 203a 6d61   we think of :ma
-0000b9b0: 7468 3a60 5c70 6869 6020 6173 2061 6e20  th:`\phi` as an 
-0000b9c0: 6175 746f 6d6f 7270 6869 736d 206f 6e0a  automorphism on.
-0000b9d0: 2020 2020 3a6d 6174 683a 605c 6d61 7468      :math:`\math
-0000b9e0: 6262 7b52 7d5e 7b5c 7466 7261 637b 6e28  bb{R}^{\tfrac{n(
-0000b9f0: 6e2b 3129 7d7b 327d 7d60 2c20 7768 6572  n+1)}{2}}`, wher
-0000ba00: 6520 7765 206f 7264 6572 0a20 2020 2074  e we order.    t
-0000ba10: 6865 2064 696d 656e 7369 6f6e 7320 6173  he dimensions as
-0000ba20: 2064 6573 6372 6962 6564 2069 6e20 7468   described in th
-0000ba30: 6520 6e6f 7465 7320 6162 6f76 652c 2074  e notes above, t
-0000ba40: 6865 206a 6163 6f62 6961 6e0a 2020 2020  he jacobian.    
-0000ba50: 6973 2061 2062 6c6f 636b 2d64 6961 676f  is a block-diago
-0000ba60: 6e61 6c20 6d61 7472 6978 2c20 7768 6572  nal matrix, wher
-0000ba70: 6520 6561 6368 2062 6c6f 636b 2063 6f72  e each block cor
-0000ba80: 7265 7370 6f6e 6473 2074 6f0a 2020 2020  responds to.    
-0000ba90: 6f6e 6520 726f 7720 6f66 203a 6d61 7468  one row of :math
-0000baa0: 3a60 5560 2e20 4561 6368 2062 6c6f 636b  :`U`. Each block
-0000bab0: 2068 6173 2061 7272 6f77 6865 6164 2073   has arrowhead s
-0000bac0: 6861 7065 2c20 616e 6420 7765 0a20 2020  hape, and we.   
-0000bad0: 2063 616e 2063 6f6d 7075 7465 2074 6865   can compute the
-0000bae0: 2064 6574 6572 6d69 6e61 6e74 206f 6620   determinant of 
-0000baf0: 7468 6174 2061 7320 6465 7363 7269 6265  that as describe
-0000bb00: 6420 696e 205b 325d 2e20 5369 6e63 650a  d in [2]. Since.
-0000bb10: 2020 2020 7468 6520 6465 7465 726d 696e      the determin
-0000bb20: 616e 7420 6f66 2061 2062 6c6f 636b 2d64  ant of a block-d
-0000bb30: 6961 676f 6e61 6c20 6d61 7472 6978 2069  iagonal matrix i
-0000bb40: 7320 7468 6520 7072 6f64 7563 740a 2020  s the product.  
-0000bb50: 2020 6f66 2074 6865 2064 6574 6572 6d69    of the determi
-0000bb60: 6e61 6e74 7320 6f66 2074 6865 2062 6c6f  nants of the blo
-0000bb70: 636b 732c 2077 6520 6765 740a 0a20 2020  cks, we get..   
-0000bb80: 202e 2e20 6d61 7468 3a3a 0a0a 2020 2020   .. math::..    
-0000bb90: 2020 205c 7465 7874 7b64 6574 7d28 4a5f     \text{det}(J_
-0000bba0: 7b5c 7068 695e 7b2d 317d 7d28 5529 2920  {\phi^{-1}}(U)) 
-0000bbb0: 3d0a 2020 2020 2020 205c 6c65 6674 5b0a  =.       \left[.
-0000bbc0: 2020 2020 2020 2020 205c 7072 6f64 5f7b           \prod_{
-0000bbd0: 693d 327d 5e4e 2075 5f7b 6969 7d5e 7b69  i=2}^N u_{ii}^{i
-0000bbe0: 202d 2031 7d20 4c5f 7b69 697d 0a20 2020   - 1} L_{ii}.   
-0000bbf0: 2020 2020 5c72 6967 6874 5d5e 7b2d 317d      \right]^{-1}
-0000bc00: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
-0000bc10: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0000bc20: 2020 2020 2e2e 205b 315d 204c 6577 616e      .. [1] Lewan
-0000bc30: 646f 7773 6b69 2c20 442e 2c20 4b75 726f  dowski, D., Kuro
-0000bc40: 7769 636b 612c 2044 2e20 616e 6420 4a6f  wicka, D. and Jo
-0000bc50: 652c 2048 2e20 2832 3030 3929 2e0a 2020  e, H. (2009)..  
-0000bc60: 2020 2020 2022 4765 6e65 7261 7469 6e67       "Generating
-0000bc70: 2072 616e 646f 6d20 636f 7272 656c 6174   random correlat
-0000bc80: 696f 6e20 6d61 7472 6963 6573 2062 6173  ion matrices bas
-0000bc90: 6564 206f 6e20 7669 6e65 7320 616e 640a  ed on vines and.
-0000bca0: 2020 2020 2020 2065 7874 656e 6465 6420         extended 
-0000bcb0: 6f6e 696f 6e20 6d65 7468 6f64 2e22 204a  onion method." J
-0000bcc0: 6f75 726e 616c 206f 6620 6d75 6c74 6976  ournal of multiv
-0000bcd0: 6172 6961 7465 2061 6e61 6c79 7369 732c  ariate analysis,
-0000bce0: 0a20 2020 2020 2020 3130 3028 3929 2c20  .       100(9), 
-0000bcf0: 7070 2e31 3938 392d 3230 3031 2e0a 0a20  pp.1989-2001... 
-0000bd00: 2020 202e 2e20 5b32 5d20 4a2e 204d 2e20     .. [2] J. M. 
-0000bd10: 6973 6e27 7420 6120 6d61 7468 656d 6174  isn't a mathemat
-0000bd20: 6963 6961 6e20 2868 7474 703a 2f2f 6d61  ician (http://ma
-0000bd30: 7468 2e73 7461 636b 6578 6368 616e 6765  th.stackexchange
-0000bd40: 2e63 6f6d 2f75 7365 7273 2f34 3938 2f0a  .com/users/498/.
-0000bd50: 2020 2020 2020 206a 2d6d 2d69 736e 742d         j-m-isnt-
-0000bd60: 612d 6d61 7468 656d 6174 6963 6961 6e29  a-mathematician)
-0000bd70: 2c20 4469 6666 6572 656e 7420 6170 7072  , Different appr
-0000bd80: 6f61 6368 6573 2074 6f20 6576 616c 7561  oaches to evalua
-0000bd90: 7465 2074 6869 730a 2020 2020 2020 2064  te this.       d
-0000bda0: 6574 6572 6d69 6e61 6e74 2c20 5552 4c20  eterminant, URL 
-0000bdb0: 2876 6572 7369 6f6e 3a20 3230 3132 2d30  (version: 2012-0
-0000bdc0: 342d 3134 293a 0a20 2020 2020 2020 6874  4-14):.       ht
-0000bdd0: 7470 3a2f 2f6d 6174 682e 7374 6163 6b65  tp://math.stacke
-0000bde0: 7863 6861 6e67 652e 636f 6d2f 712f 3133  xchange.com/q/13
-0000bdf0: 3030 3236 0a20 2020 2022 2222 0a0a 2020  0026.    """..  
-0000be00: 2020 6465 6620 5f5f 6e65 775f 5f28 636c    def __new__(cl
-0000be10: 732c 206e 616d 652c 2065 7461 2c20 6e2c  s, name, eta, n,
-0000be20: 2073 645f 6469 7374 2c20 2a2c 2063 6f6d   sd_dist, *, com
-0000be30: 7075 7465 5f63 6f72 723d 5472 7565 2c20  pute_corr=True, 
-0000be40: 7374 6f72 655f 696e 5f74 7261 6365 3d54  store_in_trace=T
-0000be50: 7275 652c 202a 2a6b 7761 7267 7329 3a0a  rue, **kwargs):.
-0000be60: 2020 2020 2020 2020 7061 636b 6564 5f63          packed_c
-0000be70: 686f 6c20 3d20 5f4c 4b4a 4368 6f6c 6573  hol = _LKJCholes
-0000be80: 6b79 436f 7628 6e61 6d65 2c20 6574 613d  kyCov(name, eta=
-0000be90: 6574 612c 206e 3d6e 2c20 7364 5f64 6973  eta, n=n, sd_dis
-0000bea0: 743d 7364 5f64 6973 742c 202a 2a6b 7761  t=sd_dist, **kwa
-0000beb0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
-0000bec0: 6e6f 7420 636f 6d70 7574 655f 636f 7272  not compute_corr
-0000bed0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000bee0: 7475 726e 2070 6163 6b65 645f 6368 6f6c  turn packed_chol
-0000bef0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000bf00: 2020 2020 2020 2020 2020 2063 686f 6c2c             chol,
-0000bf10: 2063 6f72 722c 2073 7464 7320 3d20 636c   corr, stds = cl
-0000bf20: 732e 6865 6c70 6572 5f64 6574 6572 6d69  s.helper_determi
-0000bf30: 6e69 7374 6963 7328 6e2c 2070 6163 6b65  nistics(n, packe
-0000bf40: 645f 6368 6f6c 290a 2020 2020 2020 2020  d_chol).        
-0000bf50: 2020 2020 6966 2073 746f 7265 5f69 6e5f      if store_in_
-0000bf60: 7472 6163 653a 0a20 2020 2020 2020 2020  trace:.         
-0000bf70: 2020 2020 2020 2063 6f72 7220 3d20 706d         corr = pm
-0000bf80: 2e44 6574 6572 6d69 6e69 7374 6963 2866  .Deterministic(f
-0000bf90: 227b 6e61 6d65 7d5f 636f 7272 222c 2063  "{name}_corr", c
-0000bfa0: 6f72 7229 0a20 2020 2020 2020 2020 2020  orr).           
-0000bfb0: 2020 2020 2073 7464 7320 3d20 706d 2e44       stds = pm.D
-0000bfc0: 6574 6572 6d69 6e69 7374 6963 2866 227b  eterministic(f"{
-0000bfd0: 6e61 6d65 7d5f 7374 6473 222c 2073 7464  name}_stds", std
-0000bfe0: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
-0000bff0: 6574 7572 6e20 6368 6f6c 2c20 636f 7272  eturn chol, corr
-0000c000: 2c20 7374 6473 0a0a 2020 2020 4063 6c61  , stds..    @cla
-0000c010: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-0000c020: 2064 6973 7428 636c 732c 2065 7461 2c20   dist(cls, eta, 
-0000c030: 6e2c 2073 645f 6469 7374 2c20 2a2c 2063  n, sd_dist, *, c
-0000c040: 6f6d 7075 7465 5f63 6f72 723d 5472 7565  ompute_corr=True
-0000c050: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-0000c060: 2020 2020 2023 2063 6f6d 7075 7465 2043       # compute C
-0000c070: 686f 6c65 736b 7920 6465 636f 6d70 6f73  holesky decompos
-0000c080: 6974 696f 6e0a 2020 2020 2020 2020 7061  ition.        pa
-0000c090: 636b 6564 5f63 686f 6c20 3d20 5f4c 4b4a  cked_chol = _LKJ
-0000c0a0: 4368 6f6c 6573 6b79 436f 762e 6469 7374  CholeskyCov.dist
-0000c0b0: 2865 7461 3d65 7461 2c20 6e3d 6e2c 2073  (eta=eta, n=n, s
-0000c0c0: 645f 6469 7374 3d73 645f 6469 7374 2c20  d_dist=sd_dist, 
-0000c0d0: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-0000c0e0: 2020 6966 206e 6f74 2063 6f6d 7075 7465    if not compute
-0000c0f0: 5f63 6f72 723a 0a20 2020 2020 2020 2020  _corr:.         
-0000c100: 2020 2072 6574 7572 6e20 7061 636b 6564     return packed
-0000c110: 5f63 686f 6c0a 2020 2020 2020 2020 656c  _chol.        el
-0000c120: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000c130: 7265 7475 726e 2063 6c73 2e68 656c 7065  return cls.helpe
-0000c140: 725f 6465 7465 726d 696e 6973 7469 6373  r_deterministics
-0000c150: 286e 2c20 7061 636b 6564 5f63 686f 6c29  (n, packed_chol)
-0000c160: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-0000c170: 6f64 0a20 2020 2064 6566 2068 656c 7065  od.    def helpe
-0000c180: 725f 6465 7465 726d 696e 6973 7469 6373  r_deterministics
-0000c190: 2863 6c73 2c20 6e2c 2070 6163 6b65 645f  (cls, n, packed_
-0000c1a0: 6368 6f6c 293a 0a20 2020 2020 2020 2063  chol):.        c
-0000c1b0: 686f 6c20 3d20 706d 2e65 7870 616e 645f  hol = pm.expand_
-0000c1c0: 7061 636b 6564 5f74 7269 616e 6775 6c61  packed_triangula
-0000c1d0: 7228 6e2c 2070 6163 6b65 645f 6368 6f6c  r(n, packed_chol
-0000c1e0: 2c20 6c6f 7765 723d 5472 7565 290a 2020  , lower=True).  
-0000c1f0: 2020 2020 2020 2320 636f 6d70 7574 6520        # compute 
-0000c200: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-0000c210: 780a 2020 2020 2020 2020 636f 7620 3d20  x.        cov = 
-0000c220: 7074 2e64 6f74 2863 686f 6c2c 2063 686f  pt.dot(chol, cho
-0000c230: 6c2e 5429 0a20 2020 2020 2020 2023 2065  l.T).        # e
-0000c240: 7874 7261 6374 2073 7461 6e64 6172 6420  xtract standard 
-0000c250: 6465 7669 6174 696f 6e73 2061 6e64 2072  deviations and r
-0000c260: 686f 0a20 2020 2020 2020 2073 7464 7320  ho.        stds 
-0000c270: 3d20 7074 2e73 7172 7428 7074 2e64 6961  = pt.sqrt(pt.dia
-0000c280: 6728 636f 7629 290a 2020 2020 2020 2020  g(cov)).        
-0000c290: 696e 765f 7374 6473 203d 2031 202f 2073  inv_stds = 1 / s
-0000c2a0: 7464 730a 2020 2020 2020 2020 636f 7272  tds.        corr
-0000c2b0: 203d 2069 6e76 5f73 7464 735b 4e6f 6e65   = inv_stds[None
-0000c2c0: 2c20 3a5d 202a 2063 6f76 202a 2069 6e76  , :] * cov * inv
-0000c2d0: 5f73 7464 735b 3a2c 204e 6f6e 655d 0a20  _stds[:, None]. 
-0000c2e0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
-0000c2f0: 6f6c 2c20 636f 7272 2c20 7374 6473 0a0a  ol, corr, stds..
-0000c300: 0a63 6c61 7373 204c 4b4a 436f 7272 5256  .class LKJCorrRV
-0000c310: 2852 616e 646f 6d56 6172 6961 626c 6529  (RandomVariable)
-0000c320: 3a0a 2020 2020 6e61 6d65 203d 2022 6c6b  :.    name = "lk
-0000c330: 6a63 6f72 7222 0a20 2020 206e 6469 6d5f  jcorr".    ndim_
-0000c340: 7375 7070 203d 2031 0a20 2020 206e 6469  supp = 1.    ndi
-0000c350: 6d73 5f70 6172 616d 7320 3d20 5b30 2c20  ms_params = [0, 
-0000c360: 305d 0a20 2020 2064 7479 7065 203d 2022  0].    dtype = "
-0000c370: 666c 6f61 7458 220a 2020 2020 5f70 7269  floatX".    _pri
-0000c380: 6e74 5f6e 616d 6520 3d20 2822 4c4b 4a43  nt_name = ("LKJC
-0000c390: 6f72 7252 5622 2c20 225c 5c6f 7065 7261  orrRV", "\\opera
-0000c3a0: 746f 726e 616d 657b 4c4b 4a43 6f72 7252  torname{LKJCorrR
-0000c3b0: 567d 2229 0a0a 2020 2020 6465 6620 6d61  V}")..    def ma
-0000c3c0: 6b65 5f6e 6f64 6528 7365 6c66 2c20 726e  ke_node(self, rn
-0000c3d0: 672c 2073 697a 652c 2064 7479 7065 2c20  g, size, dtype, 
-0000c3e0: 6e2c 2065 7461 293a 0a20 2020 2020 2020  n, eta):.       
-0000c3f0: 206e 203d 2070 742e 6173 5f74 656e 736f   n = pt.as_tenso
-0000c400: 725f 7661 7269 6162 6c65 286e 290a 2020  r_variable(n).  
-0000c410: 2020 2020 2020 6966 206e 6f74 206e 2e6e        if not n.n
-0000c420: 6469 6d20 3d3d 2030 3a0a 2020 2020 2020  dim == 0:.      
-0000c430: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000c440: 6545 7272 6f72 2822 6e20 6d75 7374 2062  eError("n must b
-0000c450: 6520 6120 7363 616c 6172 2028 6e64 696d  e a scalar (ndim
-0000c460: 3d30 292e 2229 0a0a 2020 2020 2020 2020  =0).")..        
-0000c470: 6574 6120 3d20 7074 2e61 735f 7465 6e73  eta = pt.as_tens
-0000c480: 6f72 5f76 6172 6961 626c 6528 6574 6129  or_variable(eta)
-0000c490: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000c4a0: 6574 612e 6e64 696d 203d 3d20 303a 0a20  eta.ndim == 0:. 
-0000c4b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000c4c0: 2056 616c 7565 4572 726f 7228 2265 7461   ValueError("eta
-0000c4d0: 206d 7573 7420 6265 2061 2073 6361 6c61   must be a scala
-0000c4e0: 7220 286e 6469 6d3d 3029 2e22 290a 0a20  r (ndim=0).").. 
-0000c4f0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-0000c500: 7065 7228 292e 6d61 6b65 5f6e 6f64 6528  per().make_node(
-0000c510: 726e 672c 2073 697a 652c 2064 7479 7065  rng, size, dtype
-0000c520: 2c20 6e2c 2065 7461 290a 0a20 2020 2064  , n, eta)..    d
-0000c530: 6566 205f 7375 7070 5f73 6861 7065 5f66  ef _supp_shape_f
-0000c540: 726f 6d5f 7061 7261 6d73 2873 656c 662c  rom_params(self,
-0000c550: 2064 6973 745f 7061 7261 6d73 2c20 2a2a   dist_params, **
-0000c560: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-0000c570: 206e 203d 2064 6973 745f 7061 7261 6d73   n = dist_params
-0000c580: 5b30 5d0a 2020 2020 2020 2020 6469 7374  [0].        dist
-0000c590: 5f73 6861 7065 203d 2028 286e 202a 2028  _shape = ((n * (
-0000c5a0: 6e20 2d20 3129 2920 2f2f 2032 2c29 0a20  n - 1)) // 2,). 
-0000c5b0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-0000c5c0: 7374 5f73 6861 7065 0a0a 2020 2020 4063  st_shape..    @c
-0000c5d0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-0000c5e0: 6566 2072 6e67 5f66 6e28 636c 732c 2072  ef rng_fn(cls, r
-0000c5f0: 6e67 2c20 6e2c 2065 7461 2c20 7369 7a65  ng, n, eta, size
-0000c600: 293a 0a20 2020 2020 2020 2023 2057 6520  ):.        # We 
-0000c610: 666c 6174 7465 6e20 7468 6520 7369 7a65  flatten the size
-0000c620: 2074 6f20 6d61 6b65 206f 7065 7261 7469   to make operati
-0000c630: 6f6e 7320 6561 7369 6572 2c20 616e 6420  ons easier, and 
-0000c640: 7468 656e 2072 6562 7569 6c64 2069 740a  then rebuild it.
-0000c650: 2020 2020 2020 2020 6966 2073 697a 6520          if size 
-0000c660: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000c670: 2020 2020 2066 6c61 745f 7369 7a65 203d       flat_size =
-0000c680: 2031 0a20 2020 2020 2020 2065 6c73 653a   1.        else:
-0000c690: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
-0000c6a0: 745f 7369 7a65 203d 206e 702e 7072 6f64  t_size = np.prod
-0000c6b0: 2873 697a 6529 0a0a 2020 2020 2020 2020  (size)..        
-0000c6c0: 4320 3d20 636c 732e 5f72 616e 646f 6d5f  C = cls._random_
-0000c6d0: 636f 7272 5f6d 6174 7269 7828 726e 673d  corr_matrix(rng=
-0000c6e0: 726e 672c 206e 3d6e 2c20 6574 613d 6574  rng, n=n, eta=et
-0000c6f0: 612c 2066 6c61 745f 7369 7a65 3d66 6c61  a, flat_size=fla
-0000c700: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
-0000c710: 2074 7269 755f 6964 7820 3d20 6e70 2e74   triu_idx = np.t
-0000c720: 7269 755f 696e 6469 6365 7328 6e2c 206b  riu_indices(n, k
-0000c730: 3d31 290a 2020 2020 2020 2020 7361 6d70  =1).        samp
-0000c740: 6c65 7320 3d20 435b 2e2e 2e2c 2074 7269  les = C[..., tri
-0000c750: 755f 6964 785b 305d 2c20 7472 6975 5f69  u_idx[0], triu_i
-0000c760: 6478 5b31 5d5d 0a0a 2020 2020 2020 2020  dx[1]]..        
-0000c770: 6966 2073 697a 6520 6973 204e 6f6e 653a  if size is None:
-0000c780: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
-0000c790: 706c 6573 203d 2073 616d 706c 6573 5b30  ples = samples[0
-0000c7a0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-0000c7b0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-0000c7c0: 5f73 6861 7065 203d 2028 6e20 2a20 286e  _shape = (n * (n
-0000c7d0: 202d 2031 2929 202f 2f20 320a 2020 2020   - 1)) // 2.    
-0000c7e0: 2020 2020 2020 2020 7361 6d70 6c65 7320          samples 
-0000c7f0: 3d20 6e70 2e72 6573 6861 7065 2873 616d  = np.reshape(sam
-0000c800: 706c 6573 2c20 282a 7369 7a65 2c20 6469  ples, (*size, di
-0000c810: 7374 5f73 6861 7065 2929 0a20 2020 2020  st_shape)).     
-0000c820: 2020 2072 6574 7572 6e20 7361 6d70 6c65     return sample
-0000c830: 730a 0a20 2020 2040 636c 6173 736d 6574  s..    @classmet
-0000c840: 686f 640a 2020 2020 6465 6620 5f72 616e  hod.    def _ran
-0000c850: 646f 6d5f 636f 7272 5f6d 6174 7269 7828  dom_corr_matrix(
-0000c860: 636c 732c 2072 6e67 2c20 6e2c 2065 7461  cls, rng, n, eta
-0000c870: 2c20 666c 6174 5f73 697a 6529 3a0a 2020  , flat_size):.  
-0000c880: 2020 2020 2020 2320 6f72 6967 696e 616c        # original
-0000c890: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-0000c8a0: 696e 2052 2073 6565 3a0a 2020 2020 2020  in R see:.      
-0000c8b0: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
-0000c8c0: 7562 2e63 6f6d 2f72 6d63 656c 7265 6174  ub.com/rmcelreat
-0000c8d0: 682f 7265 7468 696e 6b69 6e67 2f62 6c6f  h/rethinking/blo
-0000c8e0: 622f 6d61 7374 6572 2f52 2f64 6973 7472  b/master/R/distr
-0000c8f0: 6962 7574 696f 6e73 2e72 0a20 2020 2020  ibutions.r.     
-0000c900: 2020 2062 6574 6120 3d20 6574 6120 2d20     beta = eta - 
-0000c910: 312e 3020 2b20 6e20 2f20 322e 300a 2020  1.0 + n / 2.0.  
-0000c920: 2020 2020 2020 7231 3220 3d20 322e 3020        r12 = 2.0 
-0000c930: 2a20 7374 6174 732e 6265 7461 2e72 7673  * stats.beta.rvs
-0000c940: 2861 3d62 6574 612c 2062 3d62 6574 612c  (a=beta, b=beta,
-0000c950: 2073 697a 653d 666c 6174 5f73 697a 652c   size=flat_size,
-0000c960: 2072 616e 646f 6d5f 7374 6174 653d 726e   random_state=rn
-0000c970: 6729 202d 2031 2e30 0a20 2020 2020 2020  g) - 1.0.       
-0000c980: 2050 203d 206e 702e 6675 6c6c 2828 666c   P = np.full((fl
-0000c990: 6174 5f73 697a 652c 206e 2c20 6e29 2c20  at_size, n, n), 
-0000c9a0: 6e70 2e65 7965 286e 2929 0a20 2020 2020  np.eye(n)).     
-0000c9b0: 2020 2050 5b2e 2e2e 2c20 302c 2031 5d20     P[..., 0, 1] 
-0000c9c0: 3d20 7231 320a 2020 2020 2020 2020 505b  = r12.        P[
-0000c9d0: 2e2e 2e2c 2031 2c20 315d 203d 206e 702e  ..., 1, 1] = np.
-0000c9e0: 7371 7274 2831 2e30 202d 2072 3132 2a2a  sqrt(1.0 - r12**
-0000c9f0: 3229 0a20 2020 2020 2020 2066 6f72 206d  2).        for m
-0000ca00: 7031 2069 6e20 7261 6e67 6528 322c 206e  p1 in range(2, n
-0000ca10: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
-0000ca20: 6574 6120 2d3d 2030 2e35 0a20 2020 2020  eta -= 0.5.     
-0000ca30: 2020 2020 2020 2079 203d 2073 7461 7473         y = stats
-0000ca40: 2e62 6574 612e 7276 7328 613d 6d70 3120  .beta.rvs(a=mp1 
-0000ca50: 2f20 322e 302c 2062 3d62 6574 612c 2073  / 2.0, b=beta, s
-0000ca60: 697a 653d 666c 6174 5f73 697a 652c 2072  ize=flat_size, r
-0000ca70: 616e 646f 6d5f 7374 6174 653d 726e 6729  andom_state=rng)
-0000ca80: 0a20 2020 2020 2020 2020 2020 207a 203d  .            z =
-0000ca90: 2073 7461 7473 2e6e 6f72 6d2e 7276 7328   stats.norm.rvs(
-0000caa0: 6c6f 633d 302c 2073 6361 6c65 3d31 2c20  loc=0, scale=1, 
-0000cab0: 7369 7a65 3d28 666c 6174 5f73 697a 652c  size=(flat_size,
-0000cac0: 206d 7031 292c 2072 616e 646f 6d5f 7374   mp1), random_st
-0000cad0: 6174 653d 726e 6729 0a20 2020 2020 2020  ate=rng).       
-0000cae0: 2020 2020 207a 203d 207a 202f 206e 702e       z = z / np.
-0000caf0: 7371 7274 286e 702e 6569 6e73 756d 2822  sqrt(np.einsum("
-0000cb00: 696a 2c69 6a2d 3e69 222c 207a 2c20 7a29  ij,ij->i", z, z)
-0000cb10: 295b 2e2e 2e2c 206e 702e 6e65 7761 7869  )[..., np.newaxi
-0000cb20: 735d 0a20 2020 2020 2020 2020 2020 2050  s].            P
-0000cb30: 5b2e 2e2e 2c20 303a 6d70 312c 206d 7031  [..., 0:mp1, mp1
-0000cb40: 5d20 3d20 6e70 2e73 7172 7428 795b 2e2e  ] = np.sqrt(y[..
-0000cb50: 2e2c 206e 702e 6e65 7761 7869 735d 2920  ., np.newaxis]) 
-0000cb60: 2a20 7a0a 2020 2020 2020 2020 2020 2020  * z.            
-0000cb70: 505b 2e2e 2e2c 206d 7031 2c20 6d70 315d  P[..., mp1, mp1]
-0000cb80: 203d 206e 702e 7371 7274 2831 2e30 202d   = np.sqrt(1.0 -
-0000cb90: 2079 290a 2020 2020 2020 2020 4320 3d20   y).        C = 
-0000cba0: 6e70 2e65 696e 7375 6d28 222e 2e2e 6a69  np.einsum("...ji
-0000cbb0: 2c2e 2e2e 6a6b 2d3e 2e2e 2e69 6b22 2c20  ,...jk->...ik", 
-0000cbc0: 502c 2050 290a 2020 2020 2020 2020 7265  P, P).        re
-0000cbd0: 7475 726e 2043 0a0a 0a6c 6b6a 636f 7272  turn C...lkjcorr
-0000cbe0: 203d 204c 4b4a 436f 7272 5256 2829 0a0a   = LKJCorrRV()..
-0000cbf0: 0a63 6c61 7373 204c 4b4a 436f 7272 2842  .class LKJCorr(B
-0000cc00: 6f75 6e64 6564 436f 6e74 696e 756f 7573  oundedContinuous
-0000cc10: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
-0000cc20: 5468 6520 4c4b 4a20 284c 6577 616e 646f  The LKJ (Lewando
-0000cc30: 7773 6b69 2c20 4b75 726f 7769 636b 6120  wski, Kurowicka 
-0000cc40: 616e 6420 4a6f 6529 206c 6f67 2d6c 696b  and Joe) log-lik
-0000cc50: 656c 6968 6f6f 642e 0a0a 2020 2020 5468  elihood...    Th
-0000cc60: 6520 4c4b 4a20 6469 7374 7269 6275 7469  e LKJ distributi
-0000cc70: 6f6e 2069 7320 6120 7072 696f 7220 6469  on is a prior di
-0000cc80: 7374 7269 6275 7469 6f6e 2066 6f72 2063  stribution for c
-0000cc90: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
-0000cca0: 6365 732e 0a20 2020 2049 6620 6574 6120  ces..    If eta 
-0000ccb0: 3d20 3120 7468 6973 2063 6f72 7265 7370  = 1 this corresp
-0000ccc0: 6f6e 6473 2074 6f20 7468 6520 756e 6966  onds to the unif
-0000ccd0: 6f72 6d20 6469 7374 7269 6275 7469 6f6e  orm distribution
-0000cce0: 206f 7665 7220 636f 7272 656c 6174 696f   over correlatio
-0000ccf0: 6e0a 2020 2020 6d61 7472 6963 6573 2e20  n.    matrices. 
-0000cd00: 466f 7220 6574 6120 2d3e 206f 6f20 7468  For eta -> oo th
-0000cd10: 6520 4c4b 4a20 7072 696f 7220 6170 7072  e LKJ prior appr
-0000cd20: 6f61 6368 6573 2074 6865 2069 6465 6e74  oaches the ident
-0000cd30: 6974 7920 6d61 7472 6978 2e0a 0a20 2020  ity matrix...   
-0000cd40: 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d   ========  =====
-0000cd50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cd60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cd70: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 5375  =========.    Su
-0000cd80: 7070 6f72 7420 2020 5570 7065 7220 7472  pport   Upper tr
-0000cd90: 6961 6e67 756c 6172 206d 6174 7269 7820  iangular matrix 
-0000cda0: 7769 7468 2076 616c 7565 7320 696e 205b  with values in [
-0000cdb0: 2d31 2c20 315d 0a20 2020 203d 3d3d 3d3d  -1, 1].    =====
-0000cdc0: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
-0000cdd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cde0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cdf0: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
-0000ce00: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0000ce10: 2d2d 0a20 2020 206e 203a 2074 656e 736f  --.    n : tenso
-0000ce20: 725f 6c69 6b65 206f 6620 696e 740a 2020  r_like of int.  
-0000ce30: 2020 2020 2020 4469 6d65 6e73 696f 6e20        Dimension 
-0000ce40: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
-0000ce50: 6520 6d61 7472 6978 2028 6e20 3e20 3129  e matrix (n > 1)
-0000ce60: 2e0a 2020 2020 6574 6120 3a20 7465 6e73  ..    eta : tens
-0000ce70: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-0000ce80: 0a20 2020 2020 2020 2054 6865 2073 6861  .        The sha
-0000ce90: 7065 2070 6172 616d 6574 6572 2028 6574  pe parameter (et
-0000cea0: 6120 3e20 3029 206f 6620 7468 6520 4c4b  a > 0) of the LK
-0000ceb0: 4a20 6469 7374 7269 6275 7469 6f6e 2e20  J distribution. 
-0000cec0: 6574 6120 3d20 310a 2020 2020 2020 2020  eta = 1.        
-0000ced0: 696d 706c 6965 7320 6120 756e 6966 6f72  implies a unifor
-0000cee0: 6d20 6469 7374 7269 6275 7469 6f6e 206f  m distribution o
-0000cef0: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
-0000cf00: 6e20 6d61 7472 6963 6573 3b0a 2020 2020  n matrices;.    
-0000cf10: 2020 2020 6c61 7267 6572 2076 616c 7565      larger value
-0000cf20: 7320 7075 7420 6d6f 7265 2077 6569 6768  s put more weigh
-0000cf30: 7420 6f6e 206d 6174 7269 6365 7320 7769  t on matrices wi
-0000cf40: 7468 2066 6577 2063 6f72 7265 6c61 7469  th few correlati
-0000cf50: 6f6e 732e 0a0a 2020 2020 4e6f 7465 730a  ons...    Notes.
-0000cf60: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
-0000cf70: 6973 2069 6d70 6c65 6d65 6e74 6174 696f  is implementatio
-0000cf80: 6e20 6f6e 6c79 2072 6574 7572 6e73 2074  n only returns t
-0000cf90: 6865 2076 616c 7565 7320 6f66 2074 6865  he values of the
-0000cfa0: 2075 7070 6572 2074 7269 616e 6775 6c61   upper triangula
-0000cfb0: 720a 2020 2020 6d61 7472 6978 2065 7863  r.    matrix exc
-0000cfc0: 6c75 6469 6e67 2074 6865 2064 6961 676f  luding the diago
-0000cfd0: 6e61 6c2e 2048 6572 6520 6973 2061 2073  nal. Here is a s
-0000cfe0: 6368 656d 6174 6963 2066 6f72 206e 203d  chematic for n =
-0000cff0: 2035 2c20 7368 6f77 696e 670a 2020 2020   5, showing.    
-0000d000: 7468 6520 696e 6465 7865 7320 6f66 2074  the indexes of t
-0000d010: 6865 2065 6c65 6d65 6e74 733a 3a0a 0a20  he elements::.. 
-0000d020: 2020 2020 2020 205b 5b2d 2030 2031 2032         [[- 0 1 2
-0000d030: 2033 5d0a 2020 2020 2020 2020 205b 2d20   3].         [- 
-0000d040: 2d20 3420 3520 365d 0a20 2020 2020 2020  - 4 5 6].       
-0000d050: 2020 5b2d 202d 202d 2037 2038 5d0a 2020    [- - - 7 8].  
-0000d060: 2020 2020 2020 205b 2d20 2d20 2d20 2d20         [- - - - 
-0000d070: 395d 0a20 2020 2020 2020 2020 5b2d 202d  9].         [- -
-0000d080: 202d 202d 202d 5d5d 0a0a 0a20 2020 2052   - - -]]...    R
-0000d090: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
-0000d0a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
-0000d0b0: 5b4c 4b4a 3230 3039 5d20 4c65 7761 6e64  [LKJ2009] Lewand
-0000d0c0: 6f77 736b 692c 2044 2e2c 204b 7572 6f77  owski, D., Kurow
-0000d0d0: 6963 6b61 2c20 442e 2061 6e64 204a 6f65  icka, D. and Joe
-0000d0e0: 2c20 482e 2028 3230 3039 292e 0a20 2020  , H. (2009)..   
-0000d0f0: 2020 2020 2022 4765 6e65 7261 7469 6e67       "Generating
-0000d100: 2072 616e 646f 6d20 636f 7272 656c 6174   random correlat
-0000d110: 696f 6e20 6d61 7472 6963 6573 2062 6173  ion matrices bas
-0000d120: 6564 206f 6e20 7669 6e65 7320 616e 640a  ed on vines and.
-0000d130: 2020 2020 2020 2020 6578 7465 6e64 6564          extended
-0000d140: 206f 6e69 6f6e 206d 6574 686f 642e 2220   onion method." 
-0000d150: 4a6f 7572 6e61 6c20 6f66 206d 756c 7469  Journal of multi
-0000d160: 7661 7269 6174 6520 616e 616c 7973 6973  variate analysis
-0000d170: 2c0a 2020 2020 2020 2020 3130 3028 3929  ,.        100(9)
-0000d180: 2c20 7070 2e31 3938 392d 3230 3031 2e0a  , pp.1989-2001..
-0000d190: 2020 2020 2222 220a 0a20 2020 2072 765f      """..    rv_
-0000d1a0: 6f70 203d 206c 6b6a 636f 7272 0a0a 2020  op = lkjcorr..  
-0000d1b0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0000d1c0: 2020 2064 6566 2064 6973 7428 636c 732c     def dist(cls,
-0000d1d0: 206e 2c20 6574 612c 202a 2a6b 7761 7267   n, eta, **kwarg
-0000d1e0: 7329 3a0a 2020 2020 2020 2020 6e20 3d20  s):.        n = 
-0000d1f0: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
-0000d200: 6961 626c 6528 696e 7458 286e 2929 0a20  iable(intX(n)). 
-0000d210: 2020 2020 2020 2065 7461 203d 2070 742e         eta = pt.
-0000d220: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-0000d230: 6c65 2866 6c6f 6174 5828 6574 6129 290a  le(floatX(eta)).
-0000d240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000d250: 7570 6572 2829 2e64 6973 7428 5b6e 2c20  uper().dist([n, 
-0000d260: 6574 615d 2c20 2a2a 6b77 6172 6773 290a  eta], **kwargs).
-0000d270: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
-0000d280: 7276 2c20 2a61 7267 7329 3a0a 2020 2020  rv, *args):.    
-0000d290: 2020 2020 7265 7475 726e 2070 742e 7a65      return pt.ze
-0000d2a0: 726f 735f 6c69 6b65 2872 7629 0a0a 2020  ros_like(rv)..  
-0000d2b0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
-0000d2c0: 2c20 6e2c 2065 7461 293a 0a20 2020 2020  , n, eta):.     
-0000d2d0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000d2e0: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
-0000d2f0: 6261 6269 6c69 7479 206f 6620 4c4b 4a20  bability of LKJ 
-0000d300: 6469 7374 7269 6275 7469 6f6e 2061 7420  distribution at 
-0000d310: 7370 6563 6966 6965 640a 2020 2020 2020  specified.      
-0000d320: 2020 7661 6c75 652e 0a0a 2020 2020 2020    value...      
-0000d330: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000d340: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-0000d350: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
-0000d360: 756d 6572 6963 0a20 2020 2020 2020 2020  umeric.         
-0000d370: 2020 2056 616c 7565 2066 6f72 2077 6869     Value for whi
-0000d380: 6368 206c 6f67 2d70 726f 6261 6269 6c69  ch log-probabili
-0000d390: 7479 2069 7320 6361 6c63 756c 6174 6564  ty is calculated
-0000d3a0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000d3b0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-0000d3c0: 2d2d 0a20 2020 2020 2020 2054 656e 736f  --.        Tenso
-0000d3d0: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
-0000d3e0: 2020 2222 220a 0a20 2020 2020 2020 2023    """..        #
-0000d3f0: 2054 4f44 4f3a 2050 7954 656e 736f 7220   TODO: PyTensor 
-0000d400: 646f 6573 206e 6f74 2068 6176 6520 6120  does not have a 
-0000d410: 6074 7269 755f 696e 6469 6365 7360 2c20  `triu_indices`, 
-0000d420: 736f 2077 6520 6361 6e20 6f6e 6c79 2077  so we can only w
-0000d430: 6f72 6b20 7769 7468 2063 6f6e 7374 616e  ork with constan
-0000d440: 740a 2020 2020 2020 2020 2320 206e 2028  t.        #  n (
-0000d450: 6f72 2065 6c73 6520 6669 6e64 2061 2064  or else find a d
-0000d460: 6966 6665 7265 6e74 2065 7870 7265 7373  ifferent express
-0000d470: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
-0000d480: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
-0000d490: 2c20 436f 6e73 7461 6e74 293a 0a20 2020  , Constant):.   
-0000d4a0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-0000d4b0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-0000d4c0: 6f72 2822 6c6f 6770 206f 6e6c 7920 696d  or("logp only im
-0000d4d0: 706c 656d 656e 7465 6420 666f 7220 636f  plemented for co
-0000d4e0: 6e73 7461 6e74 2060 6e60 2229 0a0a 2020  nstant `n`")..  
-0000d4f0: 2020 2020 2020 6e20 3d20 696e 7428 6e2e        n = int(n.
-0000d500: 6461 7461 290a 2020 2020 2020 2020 7368  data).        sh
-0000d510: 6170 6520 3d20 6e20 2a20 286e 202d 2031  ape = n * (n - 1
-0000d520: 2920 2f2f 2032 0a20 2020 2020 2020 2074  ) // 2.        t
-0000d530: 7269 5f69 6e64 6578 203d 206e 702e 7a65  ri_index = np.ze
-0000d540: 726f 7328 286e 2c20 6e29 2c20 6474 7970  ros((n, n), dtyp
-0000d550: 653d 2269 6e74 3332 2229 0a20 2020 2020  e="int32").     
-0000d560: 2020 2074 7269 5f69 6e64 6578 5b6e 702e     tri_index[np.
-0000d570: 7472 6975 5f69 6e64 6963 6573 286e 2c20  triu_indices(n, 
-0000d580: 6b3d 3129 5d20 3d20 6e70 2e61 7261 6e67  k=1)] = np.arang
-0000d590: 6528 7368 6170 6529 0a20 2020 2020 2020  e(shape).       
-0000d5a0: 2074 7269 5f69 6e64 6578 5b6e 702e 7472   tri_index[np.tr
-0000d5b0: 6975 5f69 6e64 6963 6573 286e 2c20 6b3d  iu_indices(n, k=
-0000d5c0: 3129 5b3a 3a2d 315d 5d20 3d20 6e70 2e61  1)[::-1]] = np.a
-0000d5d0: 7261 6e67 6528 7368 6170 6529 0a0a 2020  range(shape)..  
-0000d5e0: 2020 2020 2020 7661 6c75 6520 3d20 7074        value = pt
-0000d5f0: 2e74 616b 6528 7661 6c75 652c 2074 7269  .take(value, tri
-0000d600: 5f69 6e64 6578 290a 2020 2020 2020 2020  _index).        
-0000d610: 7661 6c75 6520 3d20 7074 2e66 696c 6c5f  value = pt.fill_
-0000d620: 6469 6167 6f6e 616c 2876 616c 7565 2c20  diagonal(value, 
-0000d630: 3129 0a0a 2020 2020 2020 2020 2320 544f  1)..        # TO
-0000d640: 444f 3a20 5f6c 6b6a 5f6e 6f72 6d61 6c69  DO: _lkj_normali
-0000d650: 7a69 6e67 5f63 6f6e 7374 616e 7420 6375  zing_constant cu
-0000d660: 7272 656e 746c 7920 7265 7175 6972 6573  rrently requires
-0000d670: 2060 6574 6160 2061 6e64 2060 6e60 2074   `eta` and `n` t
-0000d680: 6f20 6265 2063 6f6e 7374 616e 7473 0a20  o be constants. 
-0000d690: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0000d6a0: 696e 7374 616e 6365 2865 7461 2c20 436f  instance(eta, Co
-0000d6b0: 6e73 7461 6e74 293a 0a20 2020 2020 2020  nstant):.       
-0000d6c0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-0000d6d0: 706c 656d 656e 7465 6445 7272 6f72 2822  plementedError("
-0000d6e0: 6c6f 6770 206f 6e6c 7920 696d 706c 656d  logp only implem
-0000d6f0: 656e 7465 6420 666f 7220 636f 6e73 7461  ented for consta
-0000d700: 6e74 2060 6574 6160 2229 0a20 2020 2020  nt `eta`").     
-0000d710: 2020 2065 7461 203d 2066 6c6f 6174 2865     eta = float(e
-0000d720: 7461 2e64 6174 6129 0a20 2020 2020 2020  ta.data).       
-0000d730: 2072 6573 756c 7420 3d20 5f6c 6b6a 5f6e   result = _lkj_n
-0000d740: 6f72 6d61 6c69 7a69 6e67 5f63 6f6e 7374  ormalizing_const
-0000d750: 616e 7428 6574 612c 206e 290a 2020 2020  ant(eta, n).    
-0000d760: 2020 2020 7265 7375 6c74 202b 3d20 2865      result += (e
-0000d770: 7461 202d 2031 2e30 2920 2a20 7074 2e6c  ta - 1.0) * pt.l
-0000d780: 6f67 2864 6574 2876 616c 7565 2929 0a20  og(det(value)). 
-0000d790: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
-0000d7a0: 6563 6b5f 7061 7261 6d65 7465 7273 280a  eck_parameters(.
-0000d7b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000d7c0: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
-0000d7d0: 7661 6c75 6520 3e3d 202d 312c 0a20 2020  value >= -1,.   
-0000d7e0: 2020 2020 2020 2020 2076 616c 7565 203c           value <
-0000d7f0: 3d20 312c 0a20 2020 2020 2020 2020 2020  = 1,.           
-0000d800: 206d 6174 7269 785f 706f 735f 6465 6628   matrix_pos_def(
-0000d810: 7661 6c75 6529 2c0a 2020 2020 2020 2020  value),.        
-0000d820: 2020 2020 6574 6120 3e20 302c 0a20 2020      eta > 0,.   
-0000d830: 2020 2020 2029 0a0a 0a40 5f64 6566 6175       )...@_defau
-0000d840: 6c74 5f74 7261 6e73 666f 726d 2e72 6567  lt_transform.reg
-0000d850: 6973 7465 7228 4c4b 4a43 6f72 7229 0a64  ister(LKJCorr).d
-0000d860: 6566 206c 6b6a 636f 7272 5f64 6566 6175  ef lkjcorr_defau
-0000d870: 6c74 5f74 7261 6e73 666f 726d 286f 702c  lt_transform(op,
-0000d880: 2072 7629 3a0a 2020 2020 7265 7475 726e   rv):.    return
-0000d890: 2049 6e74 6572 7661 6c28 666c 6f61 7458   Interval(floatX
-0000d8a0: 282d 312e 3029 2c20 666c 6f61 7458 2831  (-1.0), floatX(1
-0000d8b0: 2e30 2929 0a0a 0a63 6c61 7373 204d 6174  .0))...class Mat
-0000d8c0: 7269 784e 6f72 6d61 6c52 5628 5261 6e64  rixNormalRV(Rand
-0000d8d0: 6f6d 5661 7269 6162 6c65 293a 0a20 2020  omVariable):.   
-0000d8e0: 206e 616d 6520 3d20 226d 6174 7269 786e   name = "matrixn
-0000d8f0: 6f72 6d61 6c22 0a20 2020 206e 6469 6d5f  ormal".    ndim_
-0000d900: 7375 7070 203d 2032 0a20 2020 206e 6469  supp = 2.    ndi
-0000d910: 6d73 5f70 6172 616d 7320 3d20 5b32 2c20  ms_params = [2, 
-0000d920: 322c 2032 5d0a 2020 2020 6474 7970 6520  2, 2].    dtype 
-0000d930: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
-0000d940: 7072 696e 745f 6e61 6d65 203d 2028 224d  print_name = ("M
-0000d950: 6174 7269 784e 6f72 6d61 6c22 2c20 225c  atrixNormal", "\
-0000d960: 5c6f 7065 7261 746f 726e 616d 657b 4d61  \operatorname{Ma
-0000d970: 7472 6978 4e6f 726d 616c 7d22 290a 0a20  trixNormal}").. 
-0000d980: 2020 2064 6566 205f 696e 6665 725f 7368     def _infer_sh
-0000d990: 6170 6528 7365 6c66 2c20 7369 7a65 2c20  ape(self, size, 
-0000d9a0: 6469 7374 5f70 6172 616d 732c 2070 6172  dist_params, par
-0000d9b0: 616d 5f73 6861 7065 733d 4e6f 6e65 293a  am_shapes=None):
-0000d9c0: 0a20 2020 2020 2020 2073 6861 7065 203d  .        shape =
-0000d9d0: 2074 7570 6c65 2873 697a 6529 202b 2074   tuple(size) + t
-0000d9e0: 7570 6c65 2864 6973 745f 7061 7261 6d73  uple(dist_params
-0000d9f0: 5b30 5d2e 7368 6170 655b 2d32 3a5d 290a  [0].shape[-2:]).
-0000da00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000da10: 6861 7065 0a0a 2020 2020 4063 6c61 7373  hape..    @class
-0000da20: 6d65 7468 6f64 0a20 2020 2064 6566 2072  method.    def r
-0000da30: 6e67 5f66 6e28 636c 732c 2072 6e67 2c20  ng_fn(cls, rng, 
-0000da40: 6d75 2c20 726f 7763 686f 6c2c 2063 6f6c  mu, rowchol, col
-0000da50: 6368 6f6c 2c20 7369 7a65 3d4e 6f6e 6529  chol, size=None)
-0000da60: 3a0a 2020 2020 2020 2020 7369 7a65 203d  :.        size =
-0000da70: 2074 6f5f 7475 706c 6528 7369 7a65 290a   to_tuple(size).
-0000da80: 2020 2020 2020 2020 6469 7374 5f73 6861          dist_sha
-0000da90: 7065 203d 2074 6f5f 7475 706c 6528 5b72  pe = to_tuple([r
-0000daa0: 6f77 6368 6f6c 2e73 6861 7065 5b30 5d2c  owchol.shape[0],
-0000dab0: 2063 6f6c 6368 6f6c 2e73 6861 7065 5b30   colchol.shape[0
-0000dac0: 5d5d 290a 2020 2020 2020 2020 6f75 7470  ]]).        outp
-0000dad0: 7574 5f73 6861 7065 203d 2073 697a 6520  ut_shape = size 
-0000dae0: 2b20 6469 7374 5f73 6861 7065 0a0a 2020  + dist_shape..  
-0000daf0: 2020 2020 2020 2320 4272 6f61 6463 6173        # Broadcas
-0000db00: 7469 6e67 2061 6c6c 2070 6172 616d 6574  ting all paramet
-0000db10: 6572 730a 2020 2020 2020 2020 7368 6170  ers.        shap
-0000db20: 6573 203d 205b 6d75 2e73 6861 7065 2c20  es = [mu.shape, 
-0000db30: 6f75 7470 7574 5f73 6861 7065 5d0a 2020  output_shape].  
-0000db40: 2020 2020 2020 6272 6f61 6463 6173 7461        broadcasta
-0000db50: 626c 655f 7368 6170 6520 3d20 6272 6f61  ble_shape = broa
-0000db60: 6463 6173 745f 6469 7374 5f73 616d 706c  dcast_dist_sampl
-0000db70: 6573 5f73 6861 7065 2873 6861 7065 732c  es_shape(shapes,
-0000db80: 2073 697a 653d 7369 7a65 290a 2020 2020   size=size).    
-0000db90: 2020 2020 6d75 203d 206e 702e 6272 6f61      mu = np.broa
-0000dba0: 6463 6173 745f 746f 286d 752c 2073 6861  dcast_to(mu, sha
-0000dbb0: 7065 3d62 726f 6164 6361 7374 6162 6c65  pe=broadcastable
-0000dbc0: 5f73 6861 7065 290a 2020 2020 2020 2020  _shape).        
-0000dbd0: 726f 7763 686f 6c20 3d20 6e70 2e62 726f  rowchol = np.bro
-0000dbe0: 6164 6361 7374 5f74 6f28 726f 7763 686f  adcast_to(rowcho
-0000dbf0: 6c2c 2073 6861 7065 3d73 697a 6520 2b20  l, shape=size + 
-0000dc00: 726f 7763 686f 6c2e 7368 6170 655b 2d32  rowchol.shape[-2
-0000dc10: 3a5d 290a 0a20 2020 2020 2020 2063 6f6c  :])..        col
-0000dc20: 6368 6f6c 203d 206e 702e 6272 6f61 6463  chol = np.broadc
-0000dc30: 6173 745f 746f 2863 6f6c 6368 6f6c 2c20  ast_to(colchol, 
-0000dc40: 7368 6170 653d 7369 7a65 202b 2063 6f6c  shape=size + col
-0000dc50: 6368 6f6c 2e73 6861 7065 5b2d 323a 5d29  chol.shape[-2:])
-0000dc60: 0a20 2020 2020 2020 2063 6f6c 6368 6f6c  .        colchol
-0000dc70: 203d 206e 702e 7377 6170 6178 6573 2863   = np.swapaxes(c
-0000dc80: 6f6c 6368 6f6c 2c20 2d31 2c20 2d32 2920  olchol, -1, -2) 
-0000dc90: 2023 2054 616b 6520 7472 616e 7370 6f73   # Take transpos
-0000dca0: 650a 0a20 2020 2020 2020 2073 7461 6e64  e..        stand
-0000dcb0: 6172 645f 6e6f 726d 616c 203d 2072 6e67  ard_normal = rng
-0000dcc0: 2e73 7461 6e64 6172 645f 6e6f 726d 616c  .standard_normal
-0000dcd0: 286f 7574 7075 745f 7368 6170 6529 0a20  (output_shape). 
-0000dce0: 2020 2020 2020 2073 616d 706c 6573 203d         samples =
-0000dcf0: 206d 7520 2b20 6e70 2e6d 6174 6d75 6c28   mu + np.matmul(
-0000dd00: 726f 7763 686f 6c2c 206e 702e 6d61 746d  rowchol, np.matm
-0000dd10: 756c 2873 7461 6e64 6172 645f 6e6f 726d  ul(standard_norm
-0000dd20: 616c 2c20 636f 6c63 686f 6c29 290a 0a20  al, colchol)).. 
-0000dd30: 2020 2020 2020 2072 6574 7572 6e20 7361         return sa
-0000dd40: 6d70 6c65 730a 0a0a 6d61 7472 6978 6e6f  mples...matrixno
-0000dd50: 726d 616c 203d 204d 6174 7269 784e 6f72  rmal = MatrixNor
-0000dd60: 6d61 6c52 5628 290a 0a0a 636c 6173 7320  malRV()...class 
-0000dd70: 4d61 7472 6978 4e6f 726d 616c 2843 6f6e  MatrixNormal(Con
-0000dd80: 7469 6e75 6f75 7329 3a0a 2020 2020 7222  tinuous):.    r"
-0000dd90: 2222 0a20 2020 204d 6174 7269 782d 7661  "".    Matrix-va
-0000dda0: 6c75 6564 206e 6f72 6d61 6c20 6c6f 672d  lued normal log-
-0000ddb0: 6c69 6b65 6c69 686f 6f64 2e0a 0a20 2020  likelihood...   
-0000ddc0: 202e 2e20 6d61 7468 3a3a 0a20 2020 2020   .. math::.     
-0000ddd0: 2020 6628 7820 5c6d 6964 205c 6d75 2c20    f(x \mid \mu, 
-0000dde0: 552c 2056 2920 3d0a 2020 2020 2020 2020  U, V) =.        
-0000ddf0: 2020 205c 6672 6163 7b31 7d7b 2832 5c70     \frac{1}{(2\p
-0000de00: 695e 7b6d 206e 7d20 7c55 7c5e 6e20 7c56  i^{m n} |U|^n |V
-0000de10: 7c5e 6d29 5e7b 312f 327d 7d0a 2020 2020  |^m)^{1/2}}.    
-0000de20: 2020 2020 2020 205c 6578 705c 6c65 6674         \exp\left
-0000de30: 5c7b 0a20 2020 2020 2020 2020 2020 2020  \{.             
-0000de40: 2020 202d 5c66 7261 637b 317d 7b32 7d20     -\frac{1}{2} 
-0000de50: 5c6d 6174 6872 6d7b 5472 7d5b 2056 5e7b  \mathrm{Tr}[ V^{
-0000de60: 2d31 7d20 2878 2d5c 6d75 295e 7b5c 7072  -1} (x-\mu)^{\pr
-0000de70: 696d 657d 2055 5e7b 2d31 7d20 2878 2d5c  ime} U^{-1} (x-\
-0000de80: 6d75 295d 0a20 2020 2020 2020 2020 2020  mu)].           
-0000de90: 205c 7269 6768 745c 7d0a 0a20 2020 203d   \right\}..    =
-0000dea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020  ==============  
-0000deb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000dec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ded0: 3d3d 3d3d 3d0a 2020 2020 5375 7070 6f72  =====.    Suppor
-0000dee0: 7420 2020 2020 2020 2020 203a 6d61 7468  t          :math
-0000def0: 3a60 7820 5c69 6e20 5c6d 6174 6862 627b  :`x \in \mathbb{
-0000df00: 527d 5e7b 6d20 5c74 696d 6573 206e 7d60  R}^{m \times n}`
-0000df10: 0a20 2020 204d 6561 6e20 2020 2020 2020  .    Mean       
-0000df20: 2020 2020 2020 3a6d 6174 683a 605c 6d75        :math:`\mu
-0000df30: 600a 2020 2020 526f 7720 5661 7269 616e  `.    Row Varian
-0000df40: 6365 2020 2020 203a 6d61 7468 3a60 5560  ce     :math:`U`
-0000df50: 0a20 2020 2043 6f6c 756d 6e20 5661 7269  .    Column Vari
-0000df60: 616e 6365 2020 3a6d 6174 683a 6056 600a  ance  :math:`V`.
-0000df70: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d      ============
-0000df80: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
-0000df90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000dfa0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
-0000dfb0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-0000dfc0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6d75  ---------.    mu
-0000dfd0: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-0000dfe0: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
-0000dff0: 4172 7261 7920 6f66 206d 6561 6e73 2e20  Array of means. 
-0000e000: 4d75 7374 2062 6520 6272 6f61 6463 6173  Must be broadcas
-0000e010: 7461 626c 6520 7769 7468 2074 6865 2072  table with the r
-0000e020: 616e 646f 6d20 7661 7269 6162 6c65 2058  andom variable X
-0000e030: 2073 7563 680a 2020 2020 2020 2020 7468   such.        th
-0000e040: 6174 2074 6865 2073 6861 7065 206f 6620  at the shape of 
-0000e050: 6d75 202b 2058 2069 7320 284d 2c20 4e29  mu + X is (M, N)
-0000e060: 2e0a 2020 2020 726f 7763 6f76 203a 2028  ..    rowcov : (
-0000e070: 4d2c 204d 2920 7465 6e73 6f72 5f6c 696b  M, M) tensor_lik
-0000e080: 6520 6f66 2066 6c6f 6174 2c20 6f70 7469  e of float, opti
-0000e090: 6f6e 616c 0a20 2020 2020 2020 2041 6d6f  onal.        Amo
-0000e0a0: 6e67 2d72 6f77 2063 6f76 6172 6961 6e63  ng-row covarianc
-0000e0b0: 6520 6d61 7472 6978 2e20 4465 6669 6e65  e matrix. Define
-0000e0c0: 7320 7661 7269 616e 6365 2077 6974 6869  s variance withi
-0000e0d0: 6e0a 2020 2020 2020 2020 636f 6c75 6d6e  n.        column
-0000e0e0: 732e 2045 7861 6374 6c79 206f 6e65 206f  s. Exactly one o
-0000e0f0: 6620 726f 7763 6f76 206f 7220 726f 7763  f rowcov or rowc
-0000e100: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
-0000e110: 2020 2072 6f77 6368 6f6c 203a 2028 4d2c     rowchol : (M,
-0000e120: 204d 2920 7465 6e73 6f72 5f6c 696b 6520   M) tensor_like 
-0000e130: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
-0000e140: 616c 0a20 2020 2020 2020 2043 686f 6c65  al.        Chole
-0000e150: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
-0000e160: 6e20 6f66 2061 6d6f 6e67 2d72 6f77 2063  n of among-row c
-0000e170: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-0000e180: 2e20 4578 6163 746c 7920 6f6e 6520 6f66  . Exactly one of
-0000e190: 0a20 2020 2020 2020 2072 6f77 636f 7620  .        rowcov 
-0000e1a0: 6f72 2072 6f77 6368 6f6c 2069 7320 6e65  or rowchol is ne
-0000e1b0: 6564 6564 2e0a 2020 2020 636f 6c63 6f76  eded..    colcov
-0000e1c0: 203a 2028 4e2c 204e 2920 7465 6e73 6f72   : (N, N) tensor
-0000e1d0: 5f6c 696b 6520 6f66 2066 6c6f 6174 2c20  _like of float, 
-0000e1e0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0000e1f0: 2041 6d6f 6e67 2d63 6f6c 756d 6e20 636f   Among-column co
-0000e200: 7661 7269 616e 6365 206d 6174 7269 782e  variance matrix.
-0000e210: 2049 6620 726f 7763 6f76 2069 7320 7468   If rowcov is th
-0000e220: 6520 6964 656e 7469 7479 206d 6174 7269  e identity matri
-0000e230: 782c 0a20 2020 2020 2020 2074 6869 7320  x,.        this 
-0000e240: 6675 6e63 7469 6f6e 7320 6173 2060 636f  functions as `co
-0000e250: 7660 2069 6e20 4d76 4e6f 726d 616c 2e0a  v` in MvNormal..
-0000e260: 2020 2020 2020 2020 4578 6163 746c 7920          Exactly 
-0000e270: 6f6e 6520 6f66 2063 6f6c 636f 7620 6f72  one of colcov or
-0000e280: 2063 6f6c 6368 6f6c 2069 7320 6e65 6564   colchol is need
-0000e290: 6564 2e0a 2020 2020 636f 6c63 686f 6c20  ed..    colchol 
-0000e2a0: 3a20 284e 2c20 4e29 2074 656e 736f 725f  : (N, N) tensor_
-0000e2b0: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
-0000e2c0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000e2d0: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
-0000e2e0: 7369 7469 6f6e 206f 6620 616d 6f6e 672d  sition of among-
-0000e2f0: 636f 6c75 6d6e 2063 6f76 6172 6961 6e63  column covarianc
-0000e300: 6520 6d61 7472 6978 2e20 4578 6163 746c  e matrix. Exactl
-0000e310: 7920 6f6e 650a 2020 2020 2020 2020 6f66  y one.        of
-0000e320: 2063 6f6c 636f 7620 6f72 2063 6f6c 6368   colcov or colch
-0000e330: 6f6c 2069 7320 6e65 6564 6564 2e0a 0a20  ol is needed... 
-0000e340: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-0000e350: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6566  --------.    Def
-0000e360: 696e 6520 6120 6d61 7472 6978 7661 7269  ine a matrixvari
-0000e370: 6174 6520 6e6f 726d 616c 2076 6172 6961  ate normal varia
-0000e380: 626c 6520 666f 7220 6769 7665 6e20 726f  ble for given ro
-0000e390: 7720 616e 6420 636f 6c75 6d6e 2063 6f76  w and column cov
-0000e3a0: 6172 6961 6e63 650a 2020 2020 6d61 7472  ariance.    matr
-0000e3b0: 6963 6573 3a3a 0a0a 2020 2020 2020 2020  ices::..        
-0000e3c0: 636f 6c63 6f76 203d 206e 702e 6172 7261  colcov = np.arra
-0000e3d0: 7928 5b5b 312e 2c20 302e 355d 2c20 5b30  y([[1., 0.5], [0
-0000e3e0: 2e35 2c20 325d 5d29 0a20 2020 2020 2020  .5, 2]]).       
-0000e3f0: 2072 6f77 636f 7620 3d20 6e70 2e61 7272   rowcov = np.arr
-0000e400: 6179 285b 5b31 2c20 302c 2030 5d2c 205b  ay([[1, 0, 0], [
-0000e410: 302c 2034 2c20 305d 2c20 5b30 2c20 302c  0, 4, 0], [0, 0,
-0000e420: 2031 365d 5d29 0a20 2020 2020 2020 206d   16]]).        m
-0000e430: 203d 2072 6f77 636f 762e 7368 6170 655b   = rowcov.shape[
-0000e440: 305d 0a20 2020 2020 2020 206e 203d 2063  0].        n = c
-0000e450: 6f6c 636f 762e 7368 6170 655b 305d 0a20  olcov.shape[0]. 
-0000e460: 2020 2020 2020 206d 7520 3d20 6e70 2e7a         mu = np.z
-0000e470: 6572 6f73 2828 6d2c 206e 2929 0a20 2020  eros((m, n)).   
-0000e480: 2020 2020 2076 616c 7320 3d20 706d 2e4d       vals = pm.M
-0000e490: 6174 7269 784e 6f72 6d61 6c28 2776 616c  atrixNormal('val
-0000e4a0: 7327 2c20 6d75 3d6d 752c 2063 6f6c 636f  s', mu=mu, colco
-0000e4b0: 763d 636f 6c63 6f76 2c0a 2020 2020 2020  v=colcov,.      
-0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 2020 2020 2020 2020 2072 6f77 636f 763d           rowcov=
-0000e4e0: 726f 7763 6f76 290a 0a20 2020 2041 626f  rowcov)..    Abo
-0000e4f0: 7665 2c20 7468 6520 6974 6820 726f 7720  ve, the ith row 
-0000e500: 696e 2076 616c 7320 6861 7320 6120 7661  in vals has a va
-0000e510: 7269 616e 6365 2074 6861 7420 6973 2073  riance that is s
-0000e520: 6361 6c65 6420 6279 2034 5e69 2e0a 2020  caled by 4^i..  
-0000e530: 2020 416c 7465 726e 6174 6976 656c 792c    Alternatively,
-0000e540: 2072 6f77 206f 7220 636f 6c75 6d6e 2063   row or column c
-0000e550: 686f 6c65 736b 7920 6d61 7472 6963 6573  holesky matrices
-0000e560: 2063 6f75 6c64 2062 6520 7375 6273 7469   could be substi
-0000e570: 7475 7465 6420 666f 720a 2020 2020 6569  tuted for.    ei
-0000e580: 7468 6572 2063 6f76 6172 6961 6e63 6520  ther covariance 
-0000e590: 6d61 7472 6978 2e20 5468 6520 4d61 7472  matrix. The Matr
-0000e5a0: 6978 4e6f 726d 616c 2069 7320 7175 6963  ixNormal is quic
-0000e5b0: 6b65 7220 7761 7920 636f 6d70 7574 650a  ker way compute.
-0000e5c0: 2020 2020 4d76 4e6f 726d 616c 286d 752c      MvNormal(mu,
-0000e5d0: 206e 702e 6b72 6f6e 2872 6f77 636f 762c   np.kron(rowcov,
-0000e5e0: 2063 6f6c 636f 7629 2920 7468 6174 2074   colcov)) that t
-0000e5f0: 616b 6573 2061 6476 616e 7461 6765 206f  akes advantage o
-0000e600: 6620 6b72 6f6e 6563 6b65 7220 7072 6f64  f kronecker prod
-0000e610: 7563 740a 2020 2020 7072 6f70 6572 7469  uct.    properti
-0000e620: 6573 2066 6f72 2069 6e76 6572 7369 6f6e  es for inversion
-0000e630: 2e20 466f 7220 6578 616d 706c 652c 2069  . For example, i
-0000e640: 6620 6472 6177 7320 6672 6f6d 204d 764e  f draws from MvN
-0000e650: 6f72 6d61 6c20 6861 6420 7468 6520 7361  ormal had the sa
-0000e660: 6d65 0a20 2020 2063 6f76 6172 6961 6e63  me.    covarianc
-0000e670: 6520 7374 7275 6374 7572 652c 2062 7574  e structure, but
-0000e680: 2077 6572 6520 7363 616c 6564 2062 7920   were scaled by 
-0000e690: 6469 6666 6572 656e 7420 706f 7765 7273  different powers
-0000e6a0: 206f 6620 616e 2075 6e6b 6e6f 776e 0a20   of an unknown. 
-0000e6b0: 2020 2063 6f6e 7374 616e 742c 2062 6f74     constant, bot
-0000e6c0: 6820 7468 6520 636f 7661 7269 616e 6365  h the covariance
-0000e6d0: 2061 6e64 2073 6361 6c69 6e67 2063 6f75   and scaling cou
-0000e6e0: 6c64 2062 6520 6c65 6172 6e65 6420 6173  ld be learned as
-0000e6f0: 2066 6f6c 6c6f 7773 0a20 2020 2028 7365   follows.    (se
-0000e700: 6520 7468 6520 646f 6373 7472 696e 6720  e the docstring 
-0000e710: 6f66 2060 4c4b 4a43 686f 6c65 736b 7943  of `LKJCholeskyC
-0000e720: 6f76 6020 666f 7220 6d6f 7265 2069 6e66  ov` for more inf
-0000e730: 6f72 6d61 7469 6f6e 2061 626f 7574 2074  ormation about t
-0000e740: 6869 7329 0a0a 2020 2020 2e2e 2063 6f64  his)..    .. cod
-0000e750: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-0000e760: 2020 2020 2320 5365 7475 7020 6461 7461      # Setup data
-0000e770: 0a20 2020 2020 2020 2074 7275 655f 636f  .        true_co
-0000e780: 6c63 6f76 203d 206e 702e 6172 7261 7928  lcov = np.array(
-0000e790: 5b5b 312e 302c 2030 2e35 2c20 302e 315d  [[1.0, 0.5, 0.1]
-0000e7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 5b30 2e35 2c20 312e 302c 2030 2e32    [0.5, 1.0, 0.2
-0000e7d0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7f0: 2020 205b 302e 312c 2030 2e32 2c20 312e     [0.1, 0.2, 1.
-0000e800: 305d 5d29 0a20 2020 2020 2020 206d 203d  0]]).        m =
-0000e810: 2033 0a20 2020 2020 2020 206e 203d 2074   3.        n = t
-0000e820: 7275 655f 636f 6c63 6f76 2e73 6861 7065  rue_colcov.shape
-0000e830: 5b30 5d0a 2020 2020 2020 2020 7472 7565  [0].        true
-0000e840: 5f73 6361 6c65 203d 2033 0a20 2020 2020  _scale = 3.     
-0000e850: 2020 2074 7275 655f 726f 7763 6f76 203d     true_rowcov =
-0000e860: 206e 702e 6469 6167 285b 7472 7565 5f73   np.diag([true_s
-0000e870: 6361 6c65 2a2a 2832 2a69 2920 666f 7220  cale**(2*i) for 
-0000e880: 6920 696e 2072 616e 6765 286d 295d 290a  i in range(m)]).
-0000e890: 2020 2020 2020 2020 6d75 203d 206e 702e          mu = np.
-0000e8a0: 7a65 726f 7328 286d 2c20 6e29 290a 2020  zeros((m, n)).  
-0000e8b0: 2020 2020 2020 7472 7565 5f6b 726f 6e20        true_kron 
-0000e8c0: 3d20 6e70 2e6b 726f 6e28 7472 7565 5f72  = np.kron(true_r
-0000e8d0: 6f77 636f 762c 2074 7275 655f 636f 6c63  owcov, true_colc
-0000e8e0: 6f76 290a 2020 2020 2020 2020 6461 7461  ov).        data
-0000e8f0: 203d 206e 702e 7261 6e64 6f6d 2e6d 756c   = np.random.mul
-0000e900: 7469 7661 7269 6174 655f 6e6f 726d 616c  tivariate_normal
-0000e910: 286d 752e 666c 6174 7465 6e28 292c 2074  (mu.flatten(), t
-0000e920: 7275 655f 6b72 6f6e 290a 2020 2020 2020  rue_kron).      
-0000e930: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-0000e940: 7368 6170 6528 6d2c 206e 290a 0a20 2020  shape(m, n)..   
-0000e950: 2020 2020 2077 6974 6820 706d 2e4d 6f64       with pm.Mod
-0000e960: 656c 2829 2061 7320 6d6f 6465 6c3a 0a20  el() as model:. 
-0000e970: 2020 2020 2020 2020 2020 2023 2053 6574             # Set
-0000e980: 7570 2072 6967 6874 2063 686f 6c65 736b  up right cholesk
-0000e990: 7920 6d61 7472 6978 0a20 2020 2020 2020  y matrix.       
-0000e9a0: 2020 2020 2073 645f 6469 7374 203d 2070       sd_dist = p
-0000e9b0: 6d2e 4861 6c66 4361 7563 6879 2e64 6973  m.HalfCauchy.dis
-0000e9c0: 7428 6265 7461 3d32 2e35 2c20 7368 6170  t(beta=2.5, shap
-0000e9d0: 653d 3329 0a20 2020 2020 2020 2020 2020  e=3).           
-0000e9e0: 2063 6f6c 6368 6f6c 5f70 6163 6b65 6420   colchol_packed 
-0000e9f0: 3d20 706d 2e4c 4b4a 4368 6f6c 6573 6b79  = pm.LKJCholesky
-0000ea00: 436f 7628 2763 6f6c 6368 6f6c 7061 636b  Cov('colcholpack
-0000ea10: 6564 272c 206e 3d33 2c20 6574 613d 322c  ed', n=3, eta=2,
-0000ea20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 7364 5f64 6973 743d 7364 5f64 6973 7429  sd_dist=sd_dist)
-0000ea60: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0000ea70: 6368 6f6c 203d 2070 6d2e 6578 7061 6e64  chol = pm.expand
-0000ea80: 5f70 6163 6b65 645f 7472 6961 6e67 756c  _packed_triangul
-0000ea90: 6172 2833 2c20 636f 6c63 686f 6c5f 7061  ar(3, colchol_pa
-0000eaa0: 636b 6564 290a 0a20 2020 2020 2020 2020  cked)..         
-0000eab0: 2020 2023 2053 6574 7570 206c 6566 7420     # Setup left 
-0000eac0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-0000ead0: 780a 2020 2020 2020 2020 2020 2020 7363  x.            sc
-0000eae0: 616c 6520 3d20 706d 2e4c 6f67 4e6f 726d  ale = pm.LogNorm
-0000eaf0: 616c 2827 7363 616c 6527 2c20 6d75 3d6e  al('scale', mu=n
-0000eb00: 702e 6c6f 6728 7472 7565 5f73 6361 6c65  p.log(true_scale
-0000eb10: 292c 2073 6967 6d61 3d30 2e35 290a 2020  ), sigma=0.5).  
-0000eb20: 2020 2020 2020 2020 2020 726f 7763 6f76            rowcov
-0000eb30: 203d 2070 742e 6469 6167 285b 7363 616c   = pt.diag([scal
-0000eb40: 652a 2a28 322a 6929 2066 6f72 2069 2069  e**(2*i) for i i
-0000eb50: 6e20 7261 6e67 6528 6d29 5d29 0a0a 2020  n range(m)])..  
-0000eb60: 2020 2020 2020 2020 2020 7661 6c73 203d            vals =
-0000eb70: 2070 6d2e 4d61 7472 6978 4e6f 726d 616c   pm.MatrixNormal
-0000eb80: 2827 7661 6c73 272c 206d 753d 6d75 2c20  ('vals', mu=mu, 
-0000eb90: 636f 6c63 686f 6c3d 636f 6c63 686f 6c2c  colchol=colchol,
-0000eba0: 2072 6f77 636f 763d 726f 7763 6f76 2c0a   rowcov=rowcov,.
+00003020: 616c 0a20 2020 2020 2020 2054 6865 2070  al.        The p
+00003030: 7265 6369 7369 6f6e 206d 6174 7269 782e  recision matrix.
+00003040: 0a20 2020 2063 686f 6c20 3a20 7465 6e73  .    chol : tens
+00003050: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+00003060: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00003070: 2020 2054 6865 2063 686f 6c65 736b 7920     The cholesky 
+00003080: 6661 6374 6f72 206f 6620 7468 6520 7363  factor of the sc
+00003090: 616c 6520 6d61 7472 6978 2e0a 2020 2020  ale matrix..    
+000030a0: 6c6f 7765 7220 3a20 626f 6f6c 2c20 6465  lower : bool, de
+000030b0: 6661 756c 743d 5472 7565 0a20 2020 2020  fault=True.     
+000030c0: 2020 2057 6865 7468 6572 2074 6865 2063     Whether the c
+000030d0: 686f 6c65 736b 7920 6661 7463 6f72 2069  holesky fatcor i
+000030e0: 7320 6769 7665 6e20 6173 2061 206c 6f77  s given as a low
+000030f0: 6572 2074 7269 616e 6775 6c61 7220 6d61  er triangular ma
+00003100: 7472 6978 2e0a 2020 2020 2222 220a 2020  trix..    """.  
+00003110: 2020 7276 5f6f 7020 3d20 6d76 5f73 7475    rv_op = mv_stu
+00003120: 6465 6e74 740a 0a20 2020 2040 636c 6173  dentt..    @clas
+00003130: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00003140: 6469 7374 2863 6c73 2c20 6e75 2c20 5369  dist(cls, nu, Si
+00003150: 676d 613d 4e6f 6e65 2c20 6d75 3d4e 6f6e  gma=None, mu=Non
+00003160: 652c 2073 6361 6c65 3d4e 6f6e 652c 2074  e, scale=None, t
+00003170: 6175 3d4e 6f6e 652c 2063 686f 6c3d 4e6f  au=None, chol=No
+00003180: 6e65 2c20 6c6f 7765 723d 5472 7565 2c20  ne, lower=True, 
+00003190: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+000031a0: 2020 2063 6f76 203d 206b 7761 7267 732e     cov = kwargs.
+000031b0: 706f 7028 2263 6f76 222c 204e 6f6e 6529  pop("cov", None)
+000031c0: 0a20 2020 2020 2020 2069 6620 636f 7620  .        if cov 
+000031d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000031e0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+000031f0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00003200: 2020 2020 2020 2020 2255 7365 2074 6865          "Use the
+00003210: 2073 6361 6c65 2061 7267 756d 656e 7420   scale argument 
+00003220: 746f 2073 7065 6369 6679 2074 6865 2073  to specify the s
+00003230: 6361 6c65 206d 6174 7269 782e 2022 0a20  cale matrix. ". 
+00003240: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003250: 636f 7620 7769 6c6c 2062 6520 7265 6d6f  cov will be remo
+00003260: 7665 6420 696e 2066 7574 7572 6520 7665  ved in future ve
+00003270: 7273 696f 6e73 2e22 2c0a 2020 2020 2020  rsions.",.      
+00003280: 2020 2020 2020 2020 2020 4675 7475 7265            Future
+00003290: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
+000032a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000032b0: 2020 2073 6361 6c65 203d 2063 6f76 0a20     scale = cov. 
+000032c0: 2020 2020 2020 2069 6620 5369 676d 6120         if Sigma 
+000032d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000032e0: 2020 2020 2020 2020 2069 6620 7363 616c           if scal
+000032f0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00003300: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003310: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00003320: 2253 7065 6369 6679 206f 6e6c 7920 6f6e  "Specify only on
+00003330: 6520 6f66 2073 6361 6c65 2061 6e64 2053  e of scale and S
+00003340: 6967 6d61 2229 0a20 2020 2020 2020 2020  igma").         
+00003350: 2020 2073 6361 6c65 203d 2053 6967 6d61     scale = Sigma
+00003360: 0a20 2020 2020 2020 206e 7520 3d20 7074  .        nu = pt
+00003370: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+00003380: 626c 6528 666c 6f61 7458 286e 7529 290a  ble(floatX(nu)).
+00003390: 2020 2020 2020 2020 6d75 203d 2070 742e          mu = pt.
+000033a0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+000033b0: 6c65 2866 6c6f 6174 5828 6d75 2929 0a20  le(floatX(mu)). 
+000033c0: 2020 2020 2020 2073 6361 6c65 203d 2071         scale = q
+000033d0: 7561 6464 6973 745f 6d61 7472 6978 2873  uaddist_matrix(s
+000033e0: 6361 6c65 2c20 6368 6f6c 2c20 7461 752c  cale, chol, tau,
+000033f0: 206c 6f77 6572 290a 2020 2020 2020 2020   lower).        
+00003400: 2320 5079 5465 6e73 6f72 2069 7320 7374  # PyTensor is st
+00003410: 7269 6374 6572 2061 626f 7574 2074 6865  ricter about the
+00003420: 2073 6861 7065 206f 6620 6d75 2c20 7468   shape of mu, th
+00003430: 616e 2050 794d 4320 7573 6564 2074 6f20  an PyMC used to 
+00003440: 6265 0a20 2020 2020 2020 206d 7520 3d20  be.        mu = 
+00003450: 7074 2e62 726f 6164 6361 7374 5f61 7272  pt.broadcast_arr
+00003460: 6179 7328 6d75 2c20 7363 616c 655b 2e2e  ays(mu, scale[..
+00003470: 2e2c 202d 315d 295b 305d 0a0a 2020 2020  ., -1])[0]..    
+00003480: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00003490: 2829 2e64 6973 7428 5b6e 752c 206d 752c  ().dist([nu, mu,
+000034a0: 2073 6361 6c65 5d2c 202a 2a6b 7761 7267   scale], **kwarg
+000034b0: 7329 0a0a 2020 2020 6465 6620 6d6f 6d65  s)..    def mome
+000034c0: 6e74 2872 762c 2073 697a 652c 206e 752c  nt(rv, size, nu,
+000034d0: 206d 752c 2073 6361 6c65 293a 0a20 2020   mu, scale):.   
+000034e0: 2020 2020 206d 6f6d 656e 7420 3d20 6d75       moment = mu
+000034f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00003500: 7276 5f73 697a 655f 6973 5f6e 6f6e 6528  rv_size_is_none(
+00003510: 7369 7a65 293a 0a20 2020 2020 2020 2020  size):.         
+00003520: 2020 206d 6f6d 656e 745f 7369 7a65 203d     moment_size =
+00003530: 2070 742e 636f 6e63 6174 656e 6174 6528   pt.concatenate(
+00003540: 5b73 697a 652c 205b 6d75 2e73 6861 7065  [size, [mu.shape
+00003550: 5b2d 315d 5d5d 290a 2020 2020 2020 2020  [-1]]]).        
+00003560: 2020 2020 6d6f 6d65 6e74 203d 2070 742e      moment = pt.
+00003570: 6675 6c6c 286d 6f6d 656e 745f 7369 7a65  full(moment_size
+00003580: 2c20 6d6f 6d65 6e74 290a 2020 2020 2020  , moment).      
+00003590: 2020 7265 7475 726e 206d 6f6d 656e 740a    return moment.
+000035a0: 0a20 2020 2064 6566 206c 6f67 7028 7661  .    def logp(va
+000035b0: 6c75 652c 206e 752c 206d 752c 2073 6361  lue, nu, mu, sca
+000035c0: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+000035d0: 0a20 2020 2020 2020 2043 616c 6375 6c61  .        Calcula
+000035e0: 7465 206c 6f67 2d70 726f 6261 6269 6c69  te log-probabili
+000035f0: 7479 206f 6620 4d75 6c74 6976 6172 6961  ty of Multivaria
+00003600: 7465 2053 7475 6465 6e74 2773 2054 2064  te Student's T d
+00003610: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
+00003620: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
+00003630: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+00003640: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00003650: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00003660: 2020 2020 2020 2076 616c 7565 3a20 6e75         value: nu
+00003670: 6d65 7269 630a 2020 2020 2020 2020 2020  meric.          
+00003680: 2020 5661 6c75 6520 666f 7220 7768 6963    Value for whic
+00003690: 6820 6c6f 672d 7072 6f62 6162 696c 6974  h log-probabilit
+000036a0: 7920 6973 2063 616c 6375 6c61 7465 642e  y is calculated.
+000036b0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000036c0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000036d0: 2d0a 2020 2020 2020 2020 5465 6e73 6f72  -.        Tensor
+000036e0: 5661 7269 6162 6c65 0a20 2020 2020 2020  Variable.       
+000036f0: 2022 2222 0a20 2020 2020 2020 2071 7561   """.        qua
+00003700: 6464 6973 742c 206c 6f67 6465 742c 206f  ddist, logdet, o
+00003710: 6b20 3d20 7175 6164 6469 7374 5f70 6172  k = quaddist_par
+00003720: 7365 2876 616c 7565 2c20 6d75 2c20 7363  se(value, mu, sc
+00003730: 616c 6529 0a20 2020 2020 2020 206b 203d  ale).        k =
+00003740: 2066 6c6f 6174 5828 7661 6c75 652e 7368   floatX(value.sh
+00003750: 6170 655b 2d31 5d29 0a0a 2020 2020 2020  ape[-1])..      
+00003760: 2020 6e6f 726d 203d 2067 616d 6d61 6c6e    norm = gammaln
+00003770: 2828 6e75 202b 206b 2920 2f20 322e 3029  ((nu + k) / 2.0)
+00003780: 202d 2067 616d 6d61 6c6e 286e 7520 2f20   - gammaln(nu / 
+00003790: 322e 3029 202d 2030 2e35 202a 206b 202a  2.0) - 0.5 * k *
+000037a0: 2070 742e 6c6f 6728 6e75 202a 206e 702e   pt.log(nu * np.
+000037b0: 7069 290a 2020 2020 2020 2020 696e 6e65  pi).        inne
+000037c0: 7220 3d20 2d28 6e75 202b 206b 2920 2f20  r = -(nu + k) / 
+000037d0: 322e 3020 2a20 7074 2e6c 6f67 3170 2871  2.0 * pt.log1p(q
+000037e0: 7561 6464 6973 7420 2f20 6e75 290a 2020  uaddist / nu).  
+000037f0: 2020 2020 2020 7265 7320 3d20 6e6f 726d        res = norm
+00003800: 202b 2069 6e6e 6572 202d 206c 6f67 6465   + inner - logde
+00003810: 740a 0a20 2020 2020 2020 2072 6574 7572  t..        retur
+00003820: 6e20 6368 6563 6b5f 7061 7261 6d65 7465  n check_paramete
+00003830: 7273 2872 6573 2c20 6f6b 2c20 6e75 203e  rs(res, ok, nu >
+00003840: 2030 2c20 6d73 673d 2270 6f73 6465 662c   0, msg="posdef,
+00003850: 206e 7520 3e20 3022 290a 0a0a 636c 6173   nu > 0")...clas
+00003860: 7320 4469 7269 6368 6c65 7428 5369 6d70  s Dirichlet(Simp
+00003870: 6c65 7843 6f6e 7469 6e75 6f75 7329 3a0a  lexContinuous):.
+00003880: 2020 2020 7222 2222 0a20 2020 2044 6972      r""".    Dir
+00003890: 6963 686c 6574 206c 6f67 2d6c 696b 656c  ichlet log-likel
+000038a0: 6968 6f6f 642e 0a0a 2020 2020 2e2e 206d  ihood...    .. m
+000038b0: 6174 683a 3a0a 0a20 2020 2020 2020 6628  ath::..       f(
+000038c0: 5c6d 6174 6862 667b 787d 7c5c 6d61 7468  \mathbf{x}|\math
+000038d0: 6266 7b61 7d29 203d 0a20 2020 2020 2020  bf{a}) =.       
+000038e0: 2020 2020 5c66 7261 637b 5c47 616d 6d61      \frac{\Gamma
+000038f0: 285c 7375 6d5f 7b69 3d31 7d5e 6b20 615f  (\sum_{i=1}^k a_
+00003900: 6929 7d7b 5c70 726f 645f 7b69 3d31 7d5e  i)}{\prod_{i=1}^
+00003910: 6b20 5c47 616d 6d61 2861 5f69 297d 0a20  k \Gamma(a_i)}. 
+00003920: 2020 2020 2020 2020 2020 5c70 726f 645f            \prod_
+00003930: 7b69 3d31 7d5e 6b20 785f 695e 7b61 5f69  {i=1}^k x_i^{a_i
+00003940: 202d 2031 7d0a 0a20 2020 203d 3d3d 3d3d   - 1}..    =====
+00003950: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+00003960: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003970: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003980: 3d3d 3d3d 0a20 2020 2053 7570 706f 7274  ====.    Support
+00003990: 2020 203a 6d61 7468 3a60 785f 6920 5c69     :math:`x_i \i
+000039a0: 6e20 2830 2c20 3129 6020 666f 7220 3a6d  n (0, 1)` for :m
+000039b0: 6174 683a 6069 205c 696e 205c 7b31 2c20  ath:`i \in \{1, 
+000039c0: 5c6c 646f 7473 2c20 4b5c 7d60 0a20 2020  \ldots, K\}`.   
+000039d0: 2020 2020 2020 2020 2020 2073 7563 6820             such 
+000039e0: 7468 6174 203a 6d61 7468 3a60 5c73 756d  that :math:`\sum
+000039f0: 2078 5f69 203d 2031 600a 2020 2020 4d65   x_i = 1`.    Me
+00003a00: 616e 2020 2020 2020 3a6d 6174 683a 605c  an      :math:`\
+00003a10: 6466 7261 637b 615f 697d 7b5c 7375 6d20  dfrac{a_i}{\sum 
+00003a20: 615f 697d 600a 2020 2020 5661 7269 616e  a_i}`.    Varian
+00003a30: 6365 2020 3a6d 6174 683a 605c 6466 7261  ce  :math:`\dfra
+00003a40: 637b 615f 6920 2d20 5c73 756d 2061 5f30  c{a_i - \sum a_0
+00003a50: 7d7b 615f 305e 3220 2861 5f30 202b 2031  }{a_0^2 (a_0 + 1
+00003a60: 297d 600a 2020 2020 2020 2020 2020 2020  )}`.            
+00003a70: 2020 7768 6572 6520 3a6d 6174 683a 6061    where :math:`a
+00003a80: 5f30 203d 205c 7375 6d20 615f 6960 0a20  _0 = \sum a_i`. 
+00003a90: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
+00003aa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003ab0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003ac0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020  ============..  
+00003ad0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00003ae0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00003af0: 6120 3a20 7465 6e73 6f72 5f6c 696b 6520  a : tensor_like 
+00003b00: 6f66 2066 6c6f 6174 0a20 2020 2020 2020  of float.       
+00003b10: 2043 6f6e 6365 6e74 7261 7469 6f6e 2070   Concentration p
+00003b20: 6172 616d 6574 6572 7320 2861 203e 2030  arameters (a > 0
+00003b30: 292e 2054 6865 206e 756d 6265 7220 6f66  ). The number of
+00003b40: 2063 6174 6567 6f72 6965 7320 6973 2067   categories is g
+00003b50: 6976 656e 2062 7920 7468 650a 2020 2020  iven by the.    
+00003b60: 2020 2020 6c65 6e67 7468 206f 6620 7468      length of th
+00003b70: 6520 6c61 7374 2061 7869 732e 0a20 2020  e last axis..   
+00003b80: 2022 2222 0a20 2020 2072 765f 6f70 203d   """.    rv_op =
+00003b90: 2064 6972 6963 686c 6574 0a0a 2020 2020   dirichlet..    
+00003ba0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00003bb0: 2064 6566 2064 6973 7428 636c 732c 2061   def dist(cls, a
+00003bc0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00003bd0: 2020 2020 2061 203d 2070 742e 6173 5f74       a = pt.as_t
+00003be0: 656e 736f 725f 7661 7269 6162 6c65 2861  ensor_variable(a
+00003bf0: 290a 2020 2020 2020 2020 2320 6d65 616e  ).        # mean
+00003c00: 203d 2061 202f 2070 742e 7375 6d28 6129   = a / pt.sum(a)
+00003c10: 0a20 2020 2020 2020 2023 206d 6f64 6520  .        # mode 
+00003c20: 3d20 7074 2e73 7769 7463 6828 7074 2e61  = pt.switch(pt.a
+00003c30: 6c6c 2861 203e 2031 292c 2028 6120 2d20  ll(a > 1), (a - 
+00003c40: 3129 202f 2070 742e 7375 6d28 6120 2d20  1) / pt.sum(a - 
+00003c50: 3129 2c20 6e70 2e6e 616e 290a 0a20 2020  1), np.nan)..   
+00003c60: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00003c70: 7228 292e 6469 7374 285b 615d 2c20 2a2a  r().dist([a], **
+00003c80: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+00003c90: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
+00003ca0: 2c20 6129 3a0a 2020 2020 2020 2020 6e6f  , a):.        no
+00003cb0: 726d 5f63 6f6e 7374 616e 7420 3d20 7074  rm_constant = pt
+00003cc0: 2e73 756d 2861 2c20 6178 6973 3d2d 3129  .sum(a, axis=-1)
+00003cd0: 5b2e 2e2e 2c20 4e6f 6e65 5d0a 2020 2020  [..., None].    
+00003ce0: 2020 2020 6d6f 6d65 6e74 203d 2061 202f      moment = a /
+00003cf0: 206e 6f72 6d5f 636f 6e73 7461 6e74 0a20   norm_constant. 
+00003d00: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
+00003d10: 5f73 697a 655f 6973 5f6e 6f6e 6528 7369  _size_is_none(si
+00003d20: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
+00003d30: 206d 6f6d 656e 7420 3d20 7074 2e66 756c   moment = pt.ful
+00003d40: 6c28 7074 2e63 6f6e 6361 7465 6e61 7465  l(pt.concatenate
+00003d50: 285b 7369 7a65 2c20 5b61 2e73 6861 7065  ([size, [a.shape
+00003d60: 5b2d 315d 5d5d 292c 206d 6f6d 656e 7429  [-1]]]), moment)
+00003d70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003d80: 6d6f 6d65 6e74 0a0a 2020 2020 6465 6620  moment..    def 
+00003d90: 6c6f 6770 2876 616c 7565 2c20 6129 3a0a  logp(value, a):.
+00003da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003db0: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
+00003dc0: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
+00003dd0: 2044 6972 6963 686c 6574 2064 6973 7472   Dirichlet distr
+00003de0: 6962 7574 696f 6e0a 2020 2020 2020 2020  ibution.        
+00003df0: 6174 2073 7065 6369 6669 6564 2076 616c  at specified val
+00003e00: 7565 2e0a 0a20 2020 2020 2020 2050 6172  ue...        Par
+00003e10: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00003e20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00003e30: 2020 2076 616c 7565 3a20 6e75 6d65 7269     value: numeri
+00003e40: 630a 2020 2020 2020 2020 2020 2020 5661  c.            Va
+00003e50: 6c75 6520 666f 7220 7768 6963 6820 6c6f  lue for which lo
+00003e60: 672d 7072 6f62 6162 696c 6974 7920 6973  g-probability is
+00003e70: 2063 616c 6375 6c61 7465 642e 0a0a 2020   calculated...  
+00003e80: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00003e90: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00003ea0: 2020 2020 2020 5465 6e73 6f72 5661 7269        TensorVari
+00003eb0: 6162 6c65 0a20 2020 2020 2020 2022 2222  able.        """
+00003ec0: 0a20 2020 2020 2020 2023 206f 6e6c 7920  .        # only 
+00003ed0: 6465 6669 6e65 6420 666f 7220 7375 6d28  defined for sum(
+00003ee0: 7661 6c75 6529 203d 3d20 310a 2020 2020  value) == 1.    
+00003ef0: 2020 2020 7265 7320 3d20 7074 2e73 756d      res = pt.sum
+00003f00: 286c 6f67 706f 7728 7661 6c75 652c 2061  (logpow(value, a
+00003f10: 202d 2031 2920 2d20 6761 6d6d 616c 6e28   - 1) - gammaln(
+00003f20: 6129 2c20 6178 6973 3d2d 3129 202b 2067  a), axis=-1) + g
+00003f30: 616d 6d61 6c6e 2870 742e 7375 6d28 612c  ammaln(pt.sum(a,
+00003f40: 2061 7869 733d 2d31 2929 0a20 2020 2020   axis=-1)).     
+00003f50: 2020 2072 6573 203d 2070 742e 7377 6974     res = pt.swit
+00003f60: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
+00003f70: 7074 2e6f 725f 280a 2020 2020 2020 2020  pt.or_(.        
+00003f80: 2020 2020 2020 2020 7074 2e61 6e79 2870          pt.any(p
+00003f90: 742e 6c74 2876 616c 7565 2c20 3029 2c20  t.lt(value, 0), 
+00003fa0: 6178 6973 3d2d 3129 2c0a 2020 2020 2020  axis=-1),.      
+00003fb0: 2020 2020 2020 2020 2020 7074 2e61 6e79            pt.any
+00003fc0: 2870 742e 6774 2876 616c 7565 2c20 3129  (pt.gt(value, 1)
+00003fd0: 2c20 6178 6973 3d2d 3129 2c0a 2020 2020  , axis=-1),.    
+00003fe0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00003ff0: 2020 2020 2020 202d 6e70 2e69 6e66 2c0a         -np.inf,.
+00004000: 2020 2020 2020 2020 2020 2020 7265 732c              res,
+00004010: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00004020: 2020 2072 6574 7572 6e20 6368 6563 6b5f     return check_
+00004030: 7061 7261 6d65 7465 7273 280a 2020 2020  parameters(.    
+00004040: 2020 2020 2020 2020 7265 732c 0a20 2020          res,.   
+00004050: 2020 2020 2020 2020 2061 203e 2030 2c0a           a > 0,.
+00004060: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+00004070: 2261 203e 2030 222c 0a20 2020 2020 2020  "a > 0",.       
+00004080: 2029 0a0a 0a63 6c61 7373 204d 756c 7469   )...class Multi
+00004090: 6e6f 6d69 616c 2844 6973 6372 6574 6529  nomial(Discrete)
+000040a0: 3a0a 2020 2020 7222 2222 0a20 2020 204d  :.    r""".    M
+000040b0: 756c 7469 6e6f 6d69 616c 206c 6f67 2d6c  ultinomial log-l
+000040c0: 696b 656c 6968 6f6f 642e 0a0a 2020 2020  ikelihood...    
+000040d0: 4765 6e65 7261 6c69 7a65 7320 6269 6e6f  Generalizes bino
+000040e0: 6d69 616c 2064 6973 7472 6962 7574 696f  mial distributio
+000040f0: 6e2c 2062 7574 2069 6e73 7465 6164 206f  n, but instead o
+00004100: 6620 6561 6368 2074 7269 616c 2072 6573  f each trial res
+00004110: 756c 7469 6e67 0a20 2020 2069 6e20 2273  ulting.    in "s
+00004120: 7563 6365 7373 2220 6f72 2022 6661 696c  uccess" or "fail
+00004130: 7572 6522 2c20 6561 6368 206f 6e65 2072  ure", each one r
+00004140: 6573 756c 7473 2069 6e20 6578 6163 746c  esults in exactl
+00004150: 7920 6f6e 6520 6f66 2073 6f6d 650a 2020  y one of some.  
+00004160: 2020 6669 7865 6420 6669 6e69 7465 206e    fixed finite n
+00004170: 756d 6265 7220 6b20 6f66 2070 6f73 7369  umber k of possi
+00004180: 626c 6520 6f75 7463 6f6d 6573 206f 7665  ble outcomes ove
+00004190: 7220 6e20 696e 6465 7065 6e64 656e 7420  r n independent 
+000041a0: 7472 6961 6c73 2e0a 2020 2020 2778 5b69  trials..    'x[i
+000041b0: 5d27 2069 6e64 6963 6174 6573 2074 6865  ]' indicates the
+000041c0: 206e 756d 6265 7220 6f66 2074 696d 6573   number of times
+000041d0: 206f 7574 636f 6d65 206e 756d 6265 7220   outcome number 
+000041e0: 6920 7761 7320 6f62 7365 7276 6564 0a20  i was observed. 
+000041f0: 2020 206f 7665 7220 7468 6520 6e20 7472     over the n tr
+00004200: 6961 6c73 2e0a 0a20 2020 202e 2e20 6d61  ials...    .. ma
+00004210: 7468 3a3a 0a0a 2020 2020 2020 2066 2878  th::..       f(x
+00004220: 205c 6d69 6420 6e2c 2070 2920 3d20 5c66   \mid n, p) = \f
+00004230: 7261 637b 6e21 7d7b 5c70 726f 645f 7b69  rac{n!}{\prod_{i
+00004240: 3d31 7d5e 6b20 785f 6921 7d20 5c70 726f  =1}^k x_i!} \pro
+00004250: 645f 7b69 3d31 7d5e 6b20 705f 695e 7b78  d_{i=1}^k p_i^{x
+00004260: 5f69 7d0a 0a20 2020 203d 3d3d 3d3d 3d3d  _i}..    =======
+00004270: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+00004280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000042a0: 0a20 2020 2053 7570 706f 7274 2020 2020  .    Support    
+000042b0: 203a 6d61 7468 3a60 7820 5c69 6e20 5c7b   :math:`x \in \{
+000042c0: 302c 2031 2c20 5c6c 646f 7473 2c20 6e5c  0, 1, \ldots, n\
+000042d0: 7d60 2073 7563 6820 7468 6174 0a20 2020  }` such that.   
+000042e0: 2020 2020 2020 2020 2020 2020 203a 6d61               :ma
+000042f0: 7468 3a60 5c73 756d 2078 5f69 203d 206e  th:`\sum x_i = n
+00004300: 600a 2020 2020 4d65 616e 2020 2020 2020  `.    Mean      
+00004310: 2020 3a6d 6174 683a 606e 2070 5f69 600a    :math:`n p_i`.
+00004320: 2020 2020 5661 7269 616e 6365 2020 2020      Variance    
+00004330: 3a6d 6174 683a 606e 2070 5f69 2028 3120  :math:`n p_i (1 
+00004340: 2d20 705f 6929 600a 2020 2020 436f 7661  - p_i)`.    Cova
+00004350: 7269 616e 6365 2020 3a6d 6174 683a 602d  riance  :math:`-
+00004360: 6e20 705f 6920 705f 6a60 2066 6f72 203a  n p_i p_j` for :
+00004370: 6d61 7468 3a60 6920 5c6e 6520 6a60 0a20  math:`i \ne j`. 
+00004380: 2020 203d 3d3d 3d3d 3d3d 3d3d 3d20 203d     ==========  =
+00004390: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000043a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000043b0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
+000043c0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000043d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6e20  ---------.    n 
+000043e0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+000043f0: 2069 6e74 0a20 2020 2020 2020 2054 6f74   int.        Tot
+00004400: 616c 2063 6f75 6e74 7320 696e 2065 6163  al counts in eac
+00004410: 6820 7265 706c 6963 6174 6520 286e 203e  h replicate (n >
+00004420: 2030 292e 0a20 2020 2070 203a 2074 656e   0)..    p : ten
+00004430: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
+00004440: 740a 2020 2020 2020 2020 5072 6f62 6162  t.        Probab
+00004450: 696c 6974 7920 6f66 2065 6163 6820 6f6e  ility of each on
+00004460: 6520 6f66 2074 6865 2064 6966 6665 7265  e of the differe
+00004470: 6e74 206f 7574 636f 6d65 7320 2830 203c  nt outcomes (0 <
+00004480: 3d20 7020 3c3d 2031 292e 2054 6865 206e  = p <= 1). The n
+00004490: 756d 6265 7220 6f66 0a20 2020 2020 2020  umber of.       
+000044a0: 2063 6174 6567 6f72 6965 7320 6973 2067   categories is g
+000044b0: 6976 656e 2062 7920 7468 6520 6c65 6e67  iven by the leng
+000044c0: 7468 206f 6620 7468 6520 6c61 7374 2061  th of the last a
+000044d0: 7869 732e 2045 6c65 6d65 6e74 7320 6172  xis. Elements ar
+000044e0: 6520 6578 7065 6374 6564 2074 6f20 7375  e expected to su
+000044f0: 6d0a 2020 2020 2020 2020 746f 2031 2061  m.        to 1 a
+00004500: 6c6f 6e67 2074 6865 206c 6173 7420 6178  long the last ax
+00004510: 6973 2e0a 2020 2020 2222 220a 2020 2020  is..    """.    
+00004520: 7276 5f6f 7020 3d20 6d75 6c74 696e 6f6d  rv_op = multinom
+00004530: 6961 6c0a 0a20 2020 2040 636c 6173 736d  ial..    @classm
+00004540: 6574 686f 640a 2020 2020 6465 6620 6469  ethod.    def di
+00004550: 7374 2863 6c73 2c20 6e2c 2070 2c20 2a61  st(cls, n, p, *a
+00004560: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00004570: 2020 2020 2020 2020 7020 3d20 7074 2e61          p = pt.a
+00004580: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
+00004590: 6528 7029 0a20 2020 2020 2020 2069 6620  e(p).        if 
+000045a0: 6973 696e 7374 616e 6365 2870 2c20 5465  isinstance(p, Te
+000045b0: 6e73 6f72 436f 6e73 7461 6e74 293a 0a20  nsorConstant):. 
+000045c0: 2020 2020 2020 2020 2020 2070 5f20 3d20             p_ = 
+000045d0: 6e70 2e61 7361 7272 6179 2870 2e64 6174  np.asarray(p.dat
+000045e0: 6129 0a20 2020 2020 2020 2020 2020 2069  a).            i
+000045f0: 6620 6e70 2e61 6e79 2870 5f20 3c20 3029  f np.any(p_ < 0)
+00004600: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004610: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00004620: 6f72 2866 224e 6567 6174 6976 6520 6070  or(f"Negative `p
+00004630: 6020 7061 7261 6d65 7465 7273 2061 7265  ` parameters are
+00004640: 206e 6f74 2076 616c 6964 2c20 676f 743a   not valid, got:
+00004650: 207b 705f 7d22 290a 2020 2020 2020 2020   {p_}").        
+00004660: 2020 2020 705f 7375 6d5f 203d 206e 702e      p_sum_ = np.
+00004670: 7375 6d28 5b70 5f5d 2c20 6178 6973 3d2d  sum([p_], axis=-
+00004680: 3129 0a20 2020 2020 2020 2020 2020 2069  1).            i
+00004690: 6620 6e6f 7420 6e70 2e61 6c6c 286e 702e  f not np.all(np.
+000046a0: 6973 636c 6f73 6528 705f 7375 6d5f 2c20  isclose(p_sum_, 
+000046b0: 312e 3029 293a 0a20 2020 2020 2020 2020  1.0)):.         
+000046c0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+000046d0: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
+000046e0: 2020 2020 2020 2020 2020 6622 6070 6020            f"`p` 
+000046f0: 7061 7261 6d65 7465 7273 2073 756d 2074  parameters sum t
+00004700: 6f20 7b70 5f73 756d 5f7d 2c20 696e 7374  o {p_sum_}, inst
+00004710: 6561 6420 6f66 2031 2e30 2e20 220a 2020  ead of 1.0. ".  
+00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004730: 2020 2254 6865 7920 7769 6c6c 2062 6520    "They will be 
+00004740: 6175 746f 6d61 7469 6361 6c6c 7920 7265  automatically re
+00004750: 7363 616c 6564 2e20 220a 2020 2020 2020  scaled. ".      
+00004760: 2020 2020 2020 2020 2020 2020 2020 2259                "Y
+00004770: 6f75 2063 616e 2072 6573 6361 6c65 2074  ou can rescale t
+00004780: 6865 6d20 6469 7265 6374 6c79 2074 6f20  hem directly to 
+00004790: 6765 7420 7269 6420 6f66 2074 6869 7320  get rid of this 
+000047a0: 7761 726e 696e 672e 222c 0a20 2020 2020  warning.",.     
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2055                 U
+000047c0: 7365 7257 6172 6e69 6e67 2c0a 2020 2020  serWarning,.    
+000047d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000047e0: 2020 2020 2020 2020 2020 2020 2020 705f                p_
+000047f0: 203d 2070 5f20 2f20 7074 2e73 756d 2870   = p_ / pt.sum(p
+00004800: 5f2c 2061 7869 733d 2d31 2c20 6b65 6570  _, axis=-1, keep
+00004810: 6469 6d73 3d54 7275 6529 0a20 2020 2020  dims=True).     
+00004820: 2020 2020 2020 2020 2020 2070 203d 2070             p = p
+00004830: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00004840: 6162 6c65 2870 5f29 0a20 2020 2020 2020  able(p_).       
+00004850: 206e 203d 2070 742e 6173 5f74 656e 736f   n = pt.as_tenso
+00004860: 725f 7661 7269 6162 6c65 286e 290a 2020  r_variable(n).  
+00004870: 2020 2020 2020 7020 3d20 7074 2e61 735f        p = pt.as_
+00004880: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
+00004890: 7029 0a20 2020 2020 2020 2072 6574 7572  p).        retur
+000048a0: 6e20 7375 7065 7228 292e 6469 7374 285b  n super().dist([
+000048b0: 6e2c 2070 5d2c 202a 6172 6773 2c20 2a2a  n, p], *args, **
+000048c0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+000048d0: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
+000048e0: 2c20 6e2c 2070 293a 0a20 2020 2020 2020  , n, p):.       
+000048f0: 206e 203d 2070 742e 7368 6170 655f 7061   n = pt.shape_pa
+00004900: 6472 6967 6874 286e 290a 2020 2020 2020  dright(n).      
+00004910: 2020 6d6f 6465 203d 2070 742e 726f 756e    mode = pt.roun
+00004920: 6428 6e20 2a20 7029 0a20 2020 2020 2020  d(n * p).       
+00004930: 2064 6966 6620 3d20 6e20 2d20 7074 2e73   diff = n - pt.s
+00004940: 756d 286d 6f64 652c 2061 7869 733d 2d31  um(mode, axis=-1
+00004950: 2c20 6b65 6570 6469 6d73 3d54 7275 6529  , keepdims=True)
+00004960: 0a20 2020 2020 2020 2069 6e63 5f62 6f6f  .        inc_boo
+00004970: 6c5f 6172 7220 3d20 7074 2e61 6273 2864  l_arr = pt.abs(d
+00004980: 6966 6629 203e 2030 0a20 2020 2020 2020  iff) > 0.       
+00004990: 206d 6f64 6520 3d20 7074 2e69 6e63 5f73   mode = pt.inc_s
+000049a0: 7562 7465 6e73 6f72 286d 6f64 655b 696e  ubtensor(mode[in
+000049b0: 635f 626f 6f6c 5f61 7272 2e6e 6f6e 7a65  c_bool_arr.nonze
+000049c0: 726f 2829 5d2c 2064 6966 665b 696e 635f  ro()], diff[inc_
+000049d0: 626f 6f6c 5f61 7272 2e6e 6f6e 7a65 726f  bool_arr.nonzero
+000049e0: 2829 5d29 0a20 2020 2020 2020 2069 6620  ()]).        if 
+000049f0: 6e6f 7420 7276 5f73 697a 655f 6973 5f6e  not rv_size_is_n
+00004a00: 6f6e 6528 7369 7a65 293a 0a20 2020 2020  one(size):.     
+00004a10: 2020 2020 2020 206f 7574 7075 745f 7369         output_si
+00004a20: 7a65 203d 2070 742e 636f 6e63 6174 656e  ze = pt.concaten
+00004a30: 6174 6528 5b73 697a 652c 205b 702e 7368  ate([size, [p.sh
+00004a40: 6170 655b 2d31 5d5d 5d29 0a20 2020 2020  ape[-1]]]).     
+00004a50: 2020 2020 2020 206d 6f64 6520 3d20 7074         mode = pt
+00004a60: 2e66 756c 6c28 6f75 7470 7574 5f73 697a  .full(output_siz
+00004a70: 652c 206d 6f64 6529 0a20 2020 2020 2020  e, mode).       
+00004a80: 2072 6574 7572 6e20 6d6f 6465 0a0a 2020   return mode..  
+00004a90: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
+00004aa0: 2c20 6e2c 2070 293a 0a20 2020 2020 2020  , n, p):.       
+00004ab0: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+00004ac0: 6375 6c61 7465 206c 6f67 2d70 726f 6261  culate log-proba
+00004ad0: 6269 6c69 7479 206f 6620 4d75 6c74 696e  bility of Multin
+00004ae0: 6f6d 6961 6c20 6469 7374 7269 6275 7469  omial distributi
+00004af0: 6f6e 0a20 2020 2020 2020 2061 7420 7370  on.        at sp
+00004b00: 6563 6966 6965 6420 7661 6c75 652e 0a0a  ecified value...
+00004b10: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00004b20: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00004b30: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
+00004b40: 6c75 653a 206e 756d 6572 6963 0a20 2020  lue: numeric.   
+00004b50: 2020 2020 2020 2020 2056 616c 7565 2066           Value f
+00004b60: 6f72 2077 6869 6368 206c 6f67 2d70 726f  or which log-pro
+00004b70: 6261 6269 6c69 7479 2069 7320 6361 6c63  bability is calc
+00004b80: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
+00004b90: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00004ba0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00004bb0: 2054 656e 736f 7256 6172 6961 626c 650a   TensorVariable.
+00004bc0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00004bd0: 2020 2020 2072 6573 203d 2066 6163 746c       res = factl
+00004be0: 6e28 6e29 202b 2070 742e 7375 6d28 2d66  n(n) + pt.sum(-f
+00004bf0: 6163 746c 6e28 7661 6c75 6529 202b 206c  actln(value) + l
+00004c00: 6f67 706f 7728 702c 2076 616c 7565 292c  ogpow(p, value),
+00004c10: 2061 7869 733d 2d31 290a 2020 2020 2020   axis=-1).      
+00004c20: 2020 7265 7320 3d20 7074 2e73 7769 7463    res = pt.switc
+00004c30: 6828 0a20 2020 2020 2020 2020 2020 2070  h(.            p
+00004c40: 742e 6f72 5f28 7074 2e61 6e79 2870 742e  t.or_(pt.any(pt.
+00004c50: 6c74 2876 616c 7565 2c20 3029 2c20 6178  lt(value, 0), ax
+00004c60: 6973 3d2d 3129 2c20 7074 2e6e 6571 2870  is=-1), pt.neq(p
+00004c70: 742e 7375 6d28 7661 6c75 652c 2061 7869  t.sum(value, axi
+00004c80: 733d 2d31 292c 206e 2929 2c0a 2020 2020  s=-1), n)),.    
+00004c90: 2020 2020 2020 2020 2d6e 702e 696e 662c          -np.inf,
+00004ca0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00004cb0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00004cc0: 2020 2020 7265 7475 726e 2063 6865 636b      return check
+00004cd0: 5f70 6172 616d 6574 6572 7328 0a20 2020  _parameters(.   
+00004ce0: 2020 2020 2020 2020 2072 6573 2c0a 2020           res,.  
+00004cf0: 2020 2020 2020 2020 2020 3020 3c3d 2070            0 <= p
+00004d00: 2c0a 2020 2020 2020 2020 2020 2020 7020  ,.            p 
+00004d10: 3c3d 2031 2c0a 2020 2020 2020 2020 2020  <= 1,.          
+00004d20: 2020 7074 2e69 7363 6c6f 7365 2870 742e    pt.isclose(pt.
+00004d30: 7375 6d28 702c 2061 7869 733d 2d31 292c  sum(p, axis=-1),
+00004d40: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
+00004d50: 2070 742e 6765 286e 2c20 3029 2c0a 2020   pt.ge(n, 0),.  
+00004d60: 2020 2020 2020 2020 2020 6d73 673d 2230            msg="0
+00004d70: 203c 3d20 7020 3c3d 2031 2c20 7375 6d28   <= p <= 1, sum(
+00004d80: 7029 203d 2031 2c20 6e20 3e3d 2030 222c  p) = 1, n >= 0",
+00004d90: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00004da0: 7373 2044 6972 6963 686c 6574 4d75 6c74  ss DirichletMult
+00004db0: 696e 6f6d 6961 6c52 5628 5261 6e64 6f6d  inomialRV(Random
+00004dc0: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
+00004dd0: 616d 6520 3d20 2264 6972 6963 686c 6574  ame = "dirichlet
+00004de0: 5f6d 756c 7469 6e6f 6d69 616c 220a 2020  _multinomial".  
+00004df0: 2020 6e64 696d 5f73 7570 7020 3d20 310a    ndim_supp = 1.
+00004e00: 2020 2020 6e64 696d 735f 7061 7261 6d73      ndims_params
+00004e10: 203d 205b 302c 2031 5d0a 2020 2020 6474   = [0, 1].    dt
+00004e20: 7970 6520 3d20 2269 6e74 3634 220a 2020  ype = "int64".  
+00004e30: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
+00004e40: 2822 4469 7269 6368 6c65 744d 4e22 2c20  ("DirichletMN", 
+00004e50: 225c 5c6f 7065 7261 746f 726e 616d 657b  "\\operatorname{
+00004e60: 4469 7269 6368 6c65 744d 4e7d 2229 0a0a  DirichletMN}")..
+00004e70: 2020 2020 6465 6620 5f73 7570 705f 7368      def _supp_sh
+00004e80: 6170 655f 6672 6f6d 5f70 6172 616d 7328  ape_from_params(
+00004e90: 7365 6c66 2c20 6469 7374 5f70 6172 616d  self, dist_param
+00004ea0: 732c 2070 6172 616d 5f73 6861 7065 733d  s, param_shapes=
+00004eb0: 4e6f 6e65 293a 0a20 2020 2020 2020 2072  None):.        r
+00004ec0: 6574 7572 6e20 7375 7070 5f73 6861 7065  eturn supp_shape
+00004ed0: 5f66 726f 6d5f 7265 665f 7061 7261 6d5f  _from_ref_param_
+00004ee0: 7368 6170 6528 0a20 2020 2020 2020 2020  shape(.         
+00004ef0: 2020 206e 6469 6d5f 7375 7070 3d73 656c     ndim_supp=sel
+00004f00: 662e 6e64 696d 5f73 7570 702c 0a20 2020  f.ndim_supp,.   
+00004f10: 2020 2020 2020 2020 2064 6973 745f 7061           dist_pa
+00004f20: 7261 6d73 3d64 6973 745f 7061 7261 6d73  rams=dist_params
+00004f30: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+00004f40: 7261 6d5f 7368 6170 6573 3d70 6172 616d  ram_shapes=param
+00004f50: 5f73 6861 7065 732c 0a20 2020 2020 2020  _shapes,.       
+00004f60: 2020 2020 2072 6566 5f70 6172 616d 5f69       ref_param_i
+00004f70: 6478 3d31 2c0a 2020 2020 2020 2020 290a  dx=1,.        ).
+00004f80: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00004f90: 640a 2020 2020 6465 6620 726e 675f 666e  d.    def rng_fn
+00004fa0: 2863 6c73 2c20 726e 672c 206e 2c20 612c  (cls, rng, n, a,
+00004fb0: 2073 697a 6529 3a0a 2020 2020 2020 2020   size):.        
+00004fc0: 6966 206e 2e6e 6469 6d20 3e20 3020 6f72  if n.ndim > 0 or
+00004fd0: 2061 2e6e 6469 6d20 3e20 313a 0a20 2020   a.ndim > 1:.   
+00004fe0: 2020 2020 2020 2020 206e 2c20 6120 3d20           n, a = 
+00004ff0: 6272 6f61 6463 6173 745f 7061 7261 6d73  broadcast_params
+00005000: 285b 6e2c 2061 5d2c 2063 6c73 2e6e 6469  ([n, a], cls.ndi
+00005010: 6d73 5f70 6172 616d 7329 0a20 2020 2020  ms_params).     
+00005020: 2020 2020 2020 2073 697a 6520 3d20 7475         size = tu
+00005030: 706c 6528 7369 7a65 206f 7220 2829 290a  ple(size or ()).
+00005040: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00005050: 7369 7a65 3a0a 2020 2020 2020 2020 2020  size:.          
+00005060: 2020 2020 2020 6e20 3d20 6e70 2e62 726f        n = np.bro
+00005070: 6164 6361 7374 5f74 6f28 6e2c 2073 697a  adcast_to(n, siz
+00005080: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00005090: 2020 2061 203d 206e 702e 6272 6f61 6463     a = np.broadc
+000050a0: 6173 745f 746f 2861 2c20 7369 7a65 202b  ast_to(a, size +
+000050b0: 2028 612e 7368 6170 655b 2d31 5d2c 2929   (a.shape[-1],))
+000050c0: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000050d0: 7320 3d20 6e70 2e65 6d70 7479 2861 2e73  s = np.empty(a.s
+000050e0: 6861 7065 290a 2020 2020 2020 2020 2020  hape).          
+000050f0: 2020 666f 7220 6964 7820 696e 206e 702e    for idx in np.
+00005100: 6e64 696e 6465 7828 612e 7368 6170 655b  ndindex(a.shape[
+00005110: 3a2d 315d 293a 0a20 2020 2020 2020 2020  :-1]):.         
+00005120: 2020 2020 2020 2070 203d 2072 6e67 2e64         p = rng.d
+00005130: 6972 6963 686c 6574 2861 5b69 6478 5d29  irichlet(a[idx])
+00005140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005150: 2072 6573 5b69 6478 5d20 3d20 726e 672e   res[idx] = rng.
+00005160: 6d75 6c74 696e 6f6d 6961 6c28 6e5b 6964  multinomial(n[id
+00005170: 785d 2c20 7029 0a20 2020 2020 2020 2020  x], p).         
+00005180: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
+00005190: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000051a0: 2020 2020 2020 2020 2320 6e20 6973 2061          # n is a
+000051b0: 2073 6361 6c61 722c 2061 2069 7320 6120   scalar, a is a 
+000051c0: 3164 2061 7272 6179 0a20 2020 2020 2020  1d array.       
+000051d0: 2020 2020 2070 203d 2072 6e67 2e64 6972       p = rng.dir
+000051e0: 6963 686c 6574 2861 2c20 7369 7a65 3d73  ichlet(a, size=s
+000051f0: 697a 6529 2020 2320 2873 697a 652c 2061  ize)  # (size, a
+00005200: 2e73 6861 7065 290a 0a20 2020 2020 2020  .shape)..       
+00005210: 2020 2020 2072 6573 203d 206e 702e 656d       res = np.em
+00005220: 7074 7928 702e 7368 6170 6529 0a20 2020  pty(p.shape).   
+00005230: 2020 2020 2020 2020 2066 6f72 2069 6478           for idx
+00005240: 2069 6e20 6e70 2e6e 6469 6e64 6578 2870   in np.ndindex(p
+00005250: 2e73 6861 7065 5b3a 2d31 5d29 3a0a 2020  .shape[:-1]):.  
+00005260: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00005270: 735b 6964 785d 203d 2072 6e67 2e6d 756c  s[idx] = rng.mul
+00005280: 7469 6e6f 6d69 616c 286e 2c20 705b 6964  tinomial(n, p[id
+00005290: 785d 290a 0a20 2020 2020 2020 2020 2020  x])..           
+000052a0: 2072 6574 7572 6e20 7265 730a 0a0a 6469   return res...di
+000052b0: 7269 6368 6c65 745f 6d75 6c74 696e 6f6d  richlet_multinom
+000052c0: 6961 6c20 3d20 4469 7269 6368 6c65 744d  ial = DirichletM
+000052d0: 756c 7469 6e6f 6d69 616c 5256 2829 0a0a  ultinomialRV()..
+000052e0: 0a63 6c61 7373 2044 6972 6963 686c 6574  .class Dirichlet
+000052f0: 4d75 6c74 696e 6f6d 6961 6c28 4469 7363  Multinomial(Disc
+00005300: 7265 7465 293a 0a20 2020 2072 2222 2244  rete):.    r"""D
+00005310: 6972 6963 686c 6574 204d 756c 7469 6e6f  irichlet Multino
+00005320: 6d69 616c 206c 6f67 2d6c 696b 656c 6968  mial log-likelih
+00005330: 6f6f 642e 0a0a 2020 2020 4469 7269 6368  ood...    Dirich
+00005340: 6c65 7420 6d69 7874 7572 6520 6f66 204d  let mixture of M
+00005350: 756c 7469 6e6f 6d69 616c 7320 6469 7374  ultinomials dist
+00005360: 7269 6275 7469 6f6e 2c20 7769 7468 2061  ribution, with a
+00005370: 206d 6172 6769 6e61 6c69 7a65 6420 504d   marginalized PM
+00005380: 462e 0a0a 2020 2020 2e2e 206d 6174 683a  F...    .. math:
+00005390: 3a0a 0a20 2020 2020 2020 2066 2878 205c  :..        f(x \
+000053a0: 6d69 6420 6e2c 2061 2920 3d20 5c66 7261  mid n, a) = \fra
+000053b0: 637b 5c47 616d 6d61 286e 202b 2031 295c  c{\Gamma(n + 1)\
+000053c0: 4761 6d6d 6128 5c73 756d 2061 5f6b 297d  Gamma(\sum a_k)}
+000053d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000053e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000053f0: 5c47 616d 6d61 286e 202b 205c 7375 6d20  \Gamma(n + \sum 
+00005400: 615f 6b29 7d0a 2020 2020 2020 2020 2020  a_k)}.          
+00005410: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00005420: 7072 6f64 5f7b 6b3d 317d 5e4b 0a20 2020  prod_{k=1}^K.   
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2020 2020 2020 5c66 7261 637b 5c47 616d        \frac{\Gam
+00005450: 6d61 2878 5f6b 202b 2020 615f 6b29 7d0a  ma(x_k +  a_k)}.
+00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005470: 2020 2020 2020 2020 2020 2020 2020 7b5c                {\
+00005480: 4761 6d6d 6128 785f 6b20 2b20 3129 5c47  Gamma(x_k + 1)\G
+00005490: 616d 6d61 2861 5f6b 297d 0a0a 2020 2020  amma(a_k)}..    
+000054a0: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
+000054b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000054c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000054d0: 3d3d 3d3d 3d3d 3d0a 2020 2020 5375 7070  =======.    Supp
+000054e0: 6f72 7420 2020 2020 3a6d 6174 683a 6078  ort     :math:`x
+000054f0: 205c 696e 205c 7b30 2c20 312c 205c 6c64   \in \{0, 1, \ld
+00005500: 6f74 732c 206e 5c7d 6020 7375 6368 2074  ots, n\}` such t
+00005510: 6861 740a 2020 2020 2020 2020 2020 2020  hat.            
+00005520: 2020 2020 3a6d 6174 683a 605c 7375 6d20      :math:`\sum 
+00005530: 785f 6920 3d20 6e60 0a20 2020 204d 6561  x_i = n`.    Mea
+00005540: 6e20 2020 2020 2020 203a 6d61 7468 3a60  n        :math:`
+00005550: 6e20 5c66 7261 637b 615f 697d 7b5c 7375  n \frac{a_i}{\su
+00005560: 6d7b 615f 6b7d 7d60 0a20 2020 203d 3d3d  m{a_k}}`.    ===
+00005570: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
+00005580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000055a0: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
+000055b0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+000055c0: 2d2d 2d0a 2020 2020 6e20 3a20 7465 6e73  ---.    n : tens
+000055d0: 6f72 5f6c 696b 6520 6f66 2069 6e74 0a20  or_like of int. 
+000055e0: 2020 2020 2020 2054 6f74 616c 2063 6f75         Total cou
+000055f0: 6e74 7320 696e 2065 6163 6820 7265 706c  nts in each repl
+00005600: 6963 6174 6520 286e 203e 2030 292e 0a0a  icate (n > 0)...
+00005610: 2020 2020 6120 3a20 7465 6e73 6f72 5f6c      a : tensor_l
+00005620: 696b 6520 6f66 2066 6c6f 6174 0a20 2020  ike of float.   
+00005630: 2020 2020 2044 6972 6963 686c 6574 2063       Dirichlet c
+00005640: 6f6e 6365 6e74 7261 7469 6f6e 2070 6172  oncentration par
+00005650: 616d 6574 6572 7320 2861 203e 2030 292e  ameters (a > 0).
+00005660: 2054 6865 206e 756d 6265 7220 6f66 2063   The number of c
+00005670: 6174 6567 6f72 6965 7320 6973 2067 6976  ategories is giv
+00005680: 656e 2062 790a 2020 2020 2020 2020 7468  en by.        th
+00005690: 6520 6c65 6e67 7468 206f 6620 7468 6520  e length of the 
+000056a0: 6c61 7374 2061 7869 732e 0a20 2020 2022  last axis..    "
+000056b0: 2222 0a20 2020 2072 765f 6f70 203d 2064  "".    rv_op = d
+000056c0: 6972 6963 686c 6574 5f6d 756c 7469 6e6f  irichlet_multino
+000056d0: 6d69 616c 0a0a 2020 2020 4063 6c61 7373  mial..    @class
+000056e0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+000056f0: 6973 7428 636c 732c 206e 2c20 612c 202a  ist(cls, n, a, *
+00005700: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
+00005710: 0a20 2020 2020 2020 206e 203d 2069 6e74  .        n = int
+00005720: 5828 6e29 0a20 2020 2020 2020 2061 203d  X(n).        a =
+00005730: 2066 6c6f 6174 5828 6129 0a0a 2020 2020   floatX(a)..    
+00005740: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00005750: 2829 2e64 6973 7428 5b6e 2c20 615d 2c20  ().dist([n, a], 
+00005760: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
+00005770: 6566 206d 6f6d 656e 7428 7276 2c20 7369  ef moment(rv, si
+00005780: 7a65 2c20 6e2c 2061 293a 0a20 2020 2020  ze, n, a):.     
+00005790: 2020 2070 203d 2061 202f 2070 742e 7375     p = a / pt.su
+000057a0: 6d28 612c 2061 7869 733d 2d31 2c20 6b65  m(a, axis=-1, ke
+000057b0: 6570 6469 6d73 3d54 7275 6529 0a20 2020  epdims=True).   
+000057c0: 2020 2020 2072 6574 7572 6e20 6d6f 6d65       return mome
+000057d0: 6e74 284d 756c 7469 6e6f 6d69 616c 2e64  nt(Multinomial.d
+000057e0: 6973 7428 6e3d 6e2c 2070 3d70 2c20 7369  ist(n=n, p=p, si
+000057f0: 7a65 3d73 697a 6529 290a 0a20 2020 2064  ze=size))..    d
+00005800: 6566 206c 6f67 7028 7661 6c75 652c 206e  ef logp(value, n
+00005810: 2c20 6129 3a0a 2020 2020 2020 2020 2222  , a):.        ""
+00005820: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
+00005830: 6174 6520 6c6f 672d 7072 6f62 6162 696c  ate log-probabil
+00005840: 6974 7920 6f66 2044 6972 6963 686c 6574  ity of Dirichlet
+00005850: 4d75 6c74 696e 6f6d 6961 6c20 6469 7374  Multinomial dist
+00005860: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
+00005870: 2061 7420 7370 6563 6966 6965 6420 7661   at specified va
+00005880: 6c75 652e 0a0a 2020 2020 2020 2020 5061  lue...        Pa
+00005890: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+000058a0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000058b0: 2020 2020 7661 6c75 653a 2069 6e74 6567      value: integ
+000058c0: 6572 2061 7272 6179 0a20 2020 2020 2020  er array.       
+000058d0: 2020 2020 2056 616c 7565 2066 6f72 2077       Value for w
+000058e0: 6869 6368 206c 6f67 2d70 726f 6261 6269  hich log-probabi
+000058f0: 6c69 7479 2069 7320 6361 6c63 756c 6174  lity is calculat
+00005900: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+00005910: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00005920: 2d2d 2d2d 0a20 2020 2020 2020 2054 656e  ----.        Ten
+00005930: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
+00005940: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005950: 7375 6d5f 6120 3d20 612e 7375 6d28 6178  sum_a = a.sum(ax
+00005960: 6973 3d2d 3129 0a20 2020 2020 2020 2063  is=-1).        c
+00005970: 6f6e 7374 203d 2028 6761 6d6d 616c 6e28  onst = (gammaln(
+00005980: 6e20 2b20 3129 202b 2067 616d 6d61 6c6e  n + 1) + gammaln
+00005990: 2873 756d 5f61 2929 202d 2067 616d 6d61  (sum_a)) - gamma
+000059a0: 6c6e 286e 202b 2073 756d 5f61 290a 2020  ln(n + sum_a).  
+000059b0: 2020 2020 2020 7365 7269 6573 203d 2067        series = g
+000059c0: 616d 6d61 6c6e 2876 616c 7565 202b 2061  ammaln(value + a
+000059d0: 2920 2d20 2867 616d 6d61 6c6e 2876 616c  ) - (gammaln(val
+000059e0: 7565 202b 2031 2920 2b20 6761 6d6d 616c  ue + 1) + gammal
+000059f0: 6e28 6129 290a 2020 2020 2020 2020 7265  n(a)).        re
+00005a00: 7320 3d20 636f 6e73 7420 2b20 7365 7269  s = const + seri
+00005a10: 6573 2e73 756d 2861 7869 733d 2d31 290a  es.sum(axis=-1).
+00005a20: 0a20 2020 2020 2020 2072 6573 203d 2070  .        res = p
+00005a30: 742e 7377 6974 6368 280a 2020 2020 2020  t.switch(.      
+00005a40: 2020 2020 2020 7074 2e6f 725f 280a 2020        pt.or_(.  
+00005a50: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+00005a60: 2e61 6e79 2870 742e 6c74 2876 616c 7565  .any(pt.lt(value
+00005a70: 2c20 3029 2c20 6178 6973 3d2d 3129 2c0a  , 0), axis=-1),.
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 7074 2e6e 6571 2870 742e 7375 6d28 7661  pt.neq(pt.sum(va
+00005aa0: 6c75 652c 2061 7869 733d 2d31 292c 206e  lue, axis=-1), n
+00005ab0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
+00005ac0: 2c0a 2020 2020 2020 2020 2020 2020 2d6e  ,.            -n
+00005ad0: 702e 696e 662c 0a20 2020 2020 2020 2020  p.inf,.         
+00005ae0: 2020 2072 6573 2c0a 2020 2020 2020 2020     res,.        
+00005af0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00005b00: 6e20 6368 6563 6b5f 7061 7261 6d65 7465  n check_paramete
+00005b10: 7273 280a 2020 2020 2020 2020 2020 2020  rs(.            
+00005b20: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+00005b30: 2061 203e 2030 2c0a 2020 2020 2020 2020   a > 0,.        
+00005b40: 2020 2020 6e20 3e3d 2030 2c0a 2020 2020      n >= 0,.    
+00005b50: 2020 2020 2020 2020 6d73 673d 2261 203e          msg="a >
+00005b60: 2030 2c20 6e20 3e3d 2030 222c 0a20 2020   0, n >= 0",.   
+00005b70: 2020 2020 2029 0a0a 0a63 6c61 7373 205f       )...class _
+00005b80: 4f72 6465 7265 644d 756c 7469 6e6f 6d69  OrderedMultinomi
+00005b90: 616c 284d 756c 7469 6e6f 6d69 616c 293a  al(Multinomial):
+00005ba0: 0a20 2020 2072 2222 220a 2020 2020 556e  .    r""".    Un
+00005bb0: 6465 726c 7969 6e67 2063 6c61 7373 2066  derlying class f
+00005bc0: 6f72 206f 7264 6572 6564 206d 756c 7469  or ordered multi
+00005bd0: 6e6f 6d69 616c 2064 6973 7472 6962 7574  nomial distribut
+00005be0: 696f 6e73 2e0a 2020 2020 5365 6520 646f  ions..    See do
+00005bf0: 6373 2066 6f72 2074 6865 204f 7264 6572  cs for the Order
+00005c00: 6564 4d75 6c74 696e 6f6d 6961 6c20 7772  edMultinomial wr
+00005c10: 6170 7065 7220 636c 6173 7320 666f 7220  apper class for 
+00005c20: 6d6f 7265 2064 6574 6169 6c73 206f 6e20  more details on 
+00005c30: 686f 7720 746f 2075 7365 2069 7420 696e  how to use it in
+00005c40: 206d 6f64 656c 732e 0a20 2020 2022 2222   models..    """
+00005c50: 0a20 2020 2072 765f 6f70 203d 206d 756c  .    rv_op = mul
+00005c60: 7469 6e6f 6d69 616c 0a0a 2020 2020 4063  tinomial..    @c
+00005c70: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00005c80: 6566 2064 6973 7428 636c 732c 2065 7461  ef dist(cls, eta
+00005c90: 2c20 6375 7470 6f69 6e74 732c 206e 2c20  , cutpoints, n, 
+00005ca0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00005cb0: 3a0a 2020 2020 2020 2020 6574 6120 3d20  :.        eta = 
+00005cc0: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+00005cd0: 6961 626c 6528 666c 6f61 7458 2865 7461  iable(floatX(eta
+00005ce0: 2929 0a20 2020 2020 2020 2063 7574 706f  )).        cutpo
+00005cf0: 696e 7473 203d 2070 742e 6173 5f74 656e  ints = pt.as_ten
+00005d00: 736f 725f 7661 7269 6162 6c65 2863 7574  sor_variable(cut
+00005d10: 706f 696e 7473 290a 2020 2020 2020 2020  points).        
+00005d20: 6e20 3d20 7074 2e61 735f 7465 6e73 6f72  n = pt.as_tensor
+00005d30: 5f76 6172 6961 626c 6528 696e 7458 286e  _variable(intX(n
+00005d40: 2929 0a0a 2020 2020 2020 2020 7061 203d  ))..        pa =
+00005d50: 2073 6967 6d6f 6964 2863 7574 706f 696e   sigmoid(cutpoin
+00005d60: 7473 202d 2070 742e 7368 6170 655f 7061  ts - pt.shape_pa
+00005d70: 6472 6967 6874 2865 7461 2929 0a20 2020  dright(eta)).   
+00005d80: 2020 2020 2070 5f63 756d 203d 2070 742e       p_cum = pt.
+00005d90: 636f 6e63 6174 656e 6174 6528 0a20 2020  concatenate(.   
+00005da0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
+00005db0: 2020 2020 2020 2020 2020 2070 742e 7a65             pt.ze
+00005dc0: 726f 735f 6c69 6b65 2870 742e 7368 6170  ros_like(pt.shap
+00005dd0: 655f 7061 6472 6967 6874 2870 615b 2e2e  e_padright(pa[..
+00005de0: 2e2c 2030 5d29 292c 0a20 2020 2020 2020  ., 0])),.       
+00005df0: 2020 2020 2020 2020 2070 612c 0a20 2020           pa,.   
+00005e00: 2020 2020 2020 2020 2020 2020 2070 742e               pt.
+00005e10: 6f6e 6573 5f6c 696b 6528 7074 2e73 6861  ones_like(pt.sha
+00005e20: 7065 5f70 6164 7269 6768 7428 7061 5b2e  pe_padright(pa[.
+00005e30: 2e2e 2c20 305d 2929 2c0a 2020 2020 2020  .., 0])),.      
+00005e40: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00005e50: 2020 2020 2061 7869 733d 2d31 2c0a 2020       axis=-1,.  
+00005e60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005e70: 7020 3d20 705f 6375 6d5b 2e2e 2e2c 2031  p = p_cum[..., 1
+00005e80: 3a5d 202d 2070 5f63 756d 5b2e 2e2e 2c20  :] - p_cum[..., 
+00005e90: 3a2d 315d 0a0a 2020 2020 2020 2020 7265  :-1]..        re
+00005ea0: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
+00005eb0: 7428 6e2c 2070 2c20 2a61 7267 732c 202a  t(n, p, *args, *
+00005ec0: 2a6b 7761 7267 7329 0a0a 0a63 6c61 7373  *kwargs)...class
+00005ed0: 204f 7264 6572 6564 4d75 6c74 696e 6f6d   OrderedMultinom
+00005ee0: 6961 6c3a 0a20 2020 2072 2222 220a 2020  ial:.    r""".  
+00005ef0: 2020 5772 6170 7065 7220 636c 6173 7320    Wrapper class 
+00005f00: 666f 7220 4f72 6465 7265 6420 4d75 6c74  for Ordered Mult
+00005f10: 696e 6f6d 6961 6c20 6469 7374 7269 6275  inomial distribu
+00005f20: 7469 6f6e 732e 0a0a 2020 2020 5573 6566  tions...    Usef
+00005f30: 756c 2066 6f72 2072 6567 7265 7373 696f  ul for regressio
+00005f40: 6e20 6f6e 206f 7264 696e 616c 2064 6174  n on ordinal dat
+00005f50: 6120 7768 6f73 6520 7661 6c75 6573 2072  a whose values r
+00005f60: 616e 6765 0a20 2020 2066 726f 6d20 3120  ange.    from 1 
+00005f70: 746f 204b 2061 7320 6120 6675 6e63 7469  to K as a functi
+00005f80: 6f6e 206f 6620 736f 6d65 2070 7265 6469  on of some predi
+00005f90: 6374 6f72 2c20 3a6d 6174 683a 605c 6574  ctor, :math:`\et
+00005fa0: 6160 2c20 6275 740a 2020 2020 7768 6963  a`, but.    whic
+00005fb0: 6820 6172 6520 5f61 6767 7265 6761 7465  h are _aggregate
+00005fc0: 645f 2062 7920 7472 6961 6c2c 206c 696b  d_ by trial, lik
+00005fd0: 6520 6d75 6c74 696e 6f6d 6961 6c20 6f62  e multinomial ob
+00005fe0: 7365 7276 6174 696f 6e73 2028 696e 0a20  servations (in. 
+00005ff0: 2020 2063 6f6e 7472 6173 7420 746f 2060     contrast to `
+00006000: 706d 2e4f 7264 6572 6564 4c6f 6769 7374  pm.OrderedLogist
+00006010: 6963 602c 2077 6869 6368 206f 6e6c 7920  ic`, which only 
+00006020: 6163 6365 7074 7320 6f72 6469 6e61 6c20  accepts ordinal 
+00006030: 6461 7461 0a20 2020 2069 6e20 6120 5f64  data.    in a _d
+00006040: 6973 6167 6772 6567 6174 6564 5f20 666f  isaggregated_ fo
+00006050: 726d 6174 2c20 6c69 6b65 2063 6174 6567  rmat, like categ
+00006060: 6f72 6963 616c 206f 6273 6572 7661 7469  orical observati
+00006070: 6f6e 7329 2e0a 2020 2020 5468 6520 6375  ons)..    The cu
+00006080: 7470 6f69 6e74 732c 203a 6d61 7468 3a60  tpoints, :math:`
+00006090: 6360 2c20 7365 7061 7261 7465 2077 6869  c`, separate whi
+000060a0: 6368 2072 616e 6765 7320 6f66 203a 6d61  ch ranges of :ma
+000060b0: 7468 3a60 5c65 7461 6020 6172 650a 2020  th:`\eta` are.  
+000060c0: 2020 6d61 7070 6564 2074 6f20 7768 6963    mapped to whic
+000060d0: 6820 6f66 2074 6865 204b 206f 6273 6572  h of the K obser
+000060e0: 7665 6420 6465 7065 6e64 656e 7420 7661  ved dependent va
+000060f0: 7269 6162 6c65 732e 2054 6865 206e 756d  riables. The num
+00006100: 6265 720a 2020 2020 6f66 2063 7574 706f  ber.    of cutpo
+00006110: 696e 7473 2069 7320 4b20 2d20 312e 2049  ints is K - 1. I
+00006120: 7420 6973 2072 6563 6f6d 6d65 6e64 6564  t is recommended
+00006130: 2074 6861 7420 7468 6520 6375 7470 6f69   that the cutpoi
+00006140: 6e74 7320 6172 650a 2020 2020 636f 6e73  nts are.    cons
+00006150: 7472 6169 6e65 6420 746f 2062 6520 6f72  trained to be or
+00006160: 6465 7265 642e 0a0a 2020 2020 2e2e 206d  dered...    .. m
+00006170: 6174 683a 3a0a 0a20 2020 2020 2020 6628  ath::..       f(
+00006180: 6b20 5c6d 6964 205c 6574 612c 2063 2920  k \mid \eta, c) 
+00006190: 3d20 5c6c 6566 745c 7b0a 2020 2020 2020  = \left\{.      
+000061a0: 2020 205c 6265 6769 6e7b 6172 7261 797d     \begin{array}
+000061b0: 7b6c 7d0a 2020 2020 2020 2020 2020 2031  {l}.           1
+000061c0: 202d 205c 7465 7874 7b6c 6f67 6974 7d5e   - \text{logit}^
+000061d0: 7b2d 317d 285c 6574 6120 2d20 635f 3129  {-1}(\eta - c_1)
+000061e0: 0a20 2020 2020 2020 2020 2020 2020 5c2c  .             \,
+000061f0: 2c20 5c74 6578 747b 6966 207d 206b 203d  , \text{if } k =
+00006200: 2030 205c 5c0a 2020 2020 2020 2020 2020   0 \\.          
+00006210: 205c 7465 7874 7b6c 6f67 6974 7d5e 7b2d   \text{logit}^{-
+00006220: 317d 285c 6574 6120 2d20 635f 7b6b 202d  1}(\eta - c_{k -
+00006230: 2031 7d29 202d 0a20 2020 2020 2020 2020   1}) -.         
+00006240: 2020 5c74 6578 747b 6c6f 6769 747d 5e7b    \text{logit}^{
+00006250: 2d31 7d28 5c65 7461 202d 2063 5f7b 6b7d  -1}(\eta - c_{k}
+00006260: 290a 2020 2020 2020 2020 2020 2020 205c  ).             \
+00006270: 2c2c 205c 7465 7874 7b69 6620 7d20 3020  ,, \text{if } 0 
+00006280: 3c20 6b20 3c20 4b20 5c5c 0a20 2020 2020  < k < K \\.     
+00006290: 2020 2020 2020 5c74 6578 747b 6c6f 6769        \text{logi
+000062a0: 747d 5e7b 2d31 7d28 5c65 7461 202d 2063  t}^{-1}(\eta - c
+000062b0: 5f7b 4b20 2d20 317d 290a 2020 2020 2020  _{K - 1}).      
+000062c0: 2020 2020 2020 205c 2c2c 205c 7465 7874         \,, \text
+000062d0: 7b69 6620 7d20 6b20 3d20 4b20 5c5c 0a20  {if } k = K \\. 
+000062e0: 2020 2020 2020 2020 5c65 6e64 7b61 7272          \end{arr
+000062f0: 6179 7d0a 2020 2020 2020 205c 7269 6768  ay}.       \righ
+00006300: 742e 0a0a 2020 2020 5061 7261 6d65 7465  t...    Paramete
+00006310: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00006320: 2d0a 2020 2020 6574 6120 3a20 7465 6e73  -.    eta : tens
+00006330: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+00006340: 0a20 2020 2020 2020 2054 6865 2070 7265  .        The pre
+00006350: 6469 6374 6f72 2e0a 2020 2020 6375 7470  dictor..    cutp
+00006360: 6f69 6e74 7320 3a20 7465 6e73 6f72 5f6c  oints : tensor_l
+00006370: 696b 6520 6f66 2066 6c6f 6174 0a20 2020  ike of float.   
+00006380: 2020 2020 2054 6865 206c 656e 6774 6820       The length 
+00006390: 4b20 2d20 3120 6172 7261 7920 6f66 2063  K - 1 array of c
+000063a0: 7574 706f 696e 7473 2077 6869 6368 2062  utpoints which b
+000063b0: 7265 616b 203a 6d61 7468 3a60 5c65 7461  reak :math:`\eta
+000063c0: 6020 696e 746f 0a20 2020 2020 2020 2072  ` into.        r
+000063d0: 616e 6765 732e 2044 6f20 6e6f 7420 6578  anges. Do not ex
+000063e0: 706c 6963 6974 6c79 2073 6574 2074 6865  plicitly set the
+000063f0: 2066 6972 7374 2061 6e64 206c 6173 7420   first and last 
+00006400: 656c 656d 656e 7473 206f 660a 2020 2020  elements of.    
+00006410: 2020 2020 3a6d 6174 683a 6063 6020 746f      :math:`c` to
+00006420: 206e 6567 6174 6976 6520 616e 6420 706f   negative and po
+00006430: 7369 7469 7665 2069 6e66 696e 6974 792e  sitive infinity.
+00006440: 0a20 2020 206e 203a 2074 656e 736f 725f  .    n : tensor_
+00006450: 6c69 6b65 206f 6620 696e 740a 2020 2020  like of int.    
+00006460: 2020 2020 5468 6520 746f 7461 6c20 6e75      The total nu
+00006470: 6d62 6572 206f 6620 6d75 6c74 696e 6f6d  mber of multinom
+00006480: 6961 6c20 7472 6961 6c73 2e0a 2020 2020  ial trials..    
+00006490: 636f 6d70 7574 655f 7020 3a20 626f 6f6c  compute_p : bool
+000064a0: 6561 6e2c 2064 6566 6175 6c74 3d54 7275  ean, default=Tru
+000064b0: 650a 2020 2020 2020 2020 5768 6574 6865  e.        Whethe
+000064c0: 7220 746f 2063 6f6d 7075 7465 2061 6e64  r to compute and
+000064d0: 2073 746f 7265 2069 6e20 7468 6520 7472   store in the tr
+000064e0: 6163 6520 7468 6520 696e 6665 7272 6564  ace the inferred
+000064f0: 2070 726f 6261 6269 6c69 7469 6573 206f   probabilities o
+00006500: 6620 6561 6368 0a20 2020 2020 2020 2063  f each.        c
+00006510: 6174 6567 6f72 6965 732c 0a20 2020 2020  ategories,.     
+00006520: 2020 2062 6173 6564 206f 6e20 7468 6520     based on the 
+00006530: 6375 7470 6f69 6e74 7327 2076 616c 7565  cutpoints' value
+00006540: 732e 2044 6566 6175 6c74 7320 746f 2054  s. Defaults to T
+00006550: 7275 652e 0a20 2020 2020 2020 204d 6967  rue..        Mig
+00006560: 6874 2062 6520 7573 6566 756c 2074 6f20  ht be useful to 
+00006570: 6469 7361 626c 6520 6974 2069 6620 6d65  disable it if me
+00006580: 6d6f 7279 2075 7361 6765 2069 7320 6f66  mory usage is of
+00006590: 2069 6e74 6572 6573 742e 0a0a 2020 2020   interest...    
+000065a0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
+000065b0: 2d2d 2d2d 2d0a 2020 2020 2e2e 2063 6f64  -----.    .. cod
+000065c0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+000065d0: 0a0a 2020 2020 2020 2020 2320 4765 6e65  ..        # Gene
+000065e0: 7261 7465 2064 6174 6120 666f 7220 6120  rate data for a 
+000065f0: 7369 6d70 6c65 2031 2064 696d 656e 7369  simple 1 dimensi
+00006600: 6f6e 616c 2065 7861 6d70 6c65 2070 726f  onal example pro
+00006610: 626c 656d 0a20 2020 2020 2020 2074 7275  blem.        tru
+00006620: 655f 6375 6d5f 7020 3d20 6e70 2e61 7272  e_cum_p = np.arr
+00006630: 6179 285b 302e 312c 2030 2e31 352c 2030  ay([0.1, 0.15, 0
+00006640: 2e32 352c 2030 2e35 302c 2030 2e36 352c  .25, 0.50, 0.65,
+00006650: 2030 2e39 302c 2031 2e30 5d29 0a20 2020   0.90, 1.0]).   
+00006660: 2020 2020 2074 7275 655f 7020 3d20 6e70       true_p = np
+00006670: 2e68 7374 6163 6b28 5b74 7275 655f 6375  .hstack([true_cu
+00006680: 6d5f 705b 305d 2c20 7472 7565 5f63 756d  m_p[0], true_cum
+00006690: 5f70 5b31 3a5d 202d 2074 7275 655f 6375  _p[1:] - true_cu
+000066a0: 6d5f 705b 3a2d 315d 5d29 0a20 2020 2020  m_p[:-1]]).     
+000066b0: 2020 2066 616b 655f 656c 6563 7469 6f6e     fake_election
+000066c0: 7320 3d20 6e70 2e72 616e 646f 6d2e 6d75  s = np.random.mu
+000066d0: 6c74 696e 6f6d 6961 6c28 6e3d 315f 3030  ltinomial(n=1_00
+000066e0: 302c 2070 7661 6c73 3d74 7275 655f 702c  0, pvals=true_p,
+000066f0: 2073 697a 653d 3630 290a 0a20 2020 2020   size=60)..     
+00006700: 2020 2023 204f 7264 6572 6564 206d 756c     # Ordered mul
+00006710: 7469 6e6f 6d69 616c 2072 6567 7265 7373  tinomial regress
+00006720: 696f 6e0a 2020 2020 2020 2020 7769 7468  ion.        with
+00006730: 2070 6d2e 4d6f 6465 6c28 2920 6173 206d   pm.Model() as m
+00006740: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
+00006750: 2020 6375 7470 6f69 6e74 7320 3d20 706d    cutpoints = pm
+00006760: 2e4e 6f72 6d61 6c28 0a20 2020 2020 2020  .Normal(.       
+00006770: 2020 2020 2020 2020 2022 6375 7470 6f69           "cutpoi
+00006780: 6e74 7322 2c0a 2020 2020 2020 2020 2020  nts",.          
+00006790: 2020 2020 2020 6d75 3d6e 702e 6172 616e        mu=np.aran
+000067a0: 6765 2836 2920 2d20 322e 352c 0a20 2020  ge(6) - 2.5,.   
+000067b0: 2020 2020 2020 2020 2020 2020 2073 6967               sig
+000067c0: 6d61 3d31 2e35 2c0a 2020 2020 2020 2020  ma=1.5,.        
+000067d0: 2020 2020 2020 2020 696e 6974 7661 6c3d          initval=
+000067e0: 6e70 2e61 7261 6e67 6528 3629 202d 2032  np.arange(6) - 2
+000067f0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
+00006800: 2020 2020 7472 616e 7366 6f72 6d3d 706d      transform=pm
+00006810: 2e64 6973 7472 6962 7574 696f 6e73 2e74  .distributions.t
+00006820: 7261 6e73 666f 726d 732e 6f72 6465 7265  ransforms.ordere
+00006830: 642c 0a20 2020 2020 2020 2020 2020 2029  d,.            )
+00006840: 0a0a 2020 2020 2020 2020 2020 2020 706d  ..            pm
+00006850: 2e4f 7264 6572 6564 4d75 6c74 696e 6f6d  .OrderedMultinom
+00006860: 6961 6c28 0a20 2020 2020 2020 2020 2020  ial(.           
+00006870: 2020 2020 2022 7265 7375 6c74 7322 2c0a       "results",.
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 6574 613d 302e 302c 0a20 2020 2020 2020  eta=0.0,.       
+000068a0: 2020 2020 2020 2020 2063 7574 706f 696e           cutpoin
+000068b0: 7473 3d63 7574 706f 696e 7473 2c0a 2020  ts=cutpoints,.  
+000068c0: 2020 2020 2020 2020 2020 2020 2020 6e3d                n=
+000068d0: 6661 6b65 5f65 6c65 6374 696f 6e73 2e73  fake_elections.s
+000068e0: 756d 2831 292c 0a20 2020 2020 2020 2020  um(1),.         
+000068f0: 2020 2020 2020 206f 6273 6572 7665 643d         observed=
+00006900: 6661 6b65 5f65 6c65 6374 696f 6e73 2c0a  fake_elections,.
+00006910: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00006920: 2020 2020 2020 2020 2020 2074 7261 6365             trace
+00006930: 203d 2070 6d2e 7361 6d70 6c65 2829 0a0a   = pm.sample()..
+00006940: 2020 2020 2020 2020 2320 506c 6f74 2074          # Plot t
+00006950: 6865 2072 6573 756c 7473 0a20 2020 2020  he results.     
+00006960: 2020 2061 7276 697a 2e70 6c6f 745f 706f     arviz.plot_po
+00006970: 7374 6572 696f 7228 7472 6163 655f 3132  sterior(trace_12
+00006980: 5f34 2c20 7661 725f 6e61 6d65 733d 5b22  _4, var_names=["
+00006990: 636f 6d70 6c65 7465 5f70 225d 2c20 7265  complete_p"], re
+000069a0: 665f 7661 6c3d 6c69 7374 2874 7275 655f  f_val=list(true_
+000069b0: 7029 293b 0a20 2020 2022 2222 0a0a 2020  p));.    """..  
+000069c0: 2020 6465 6620 5f5f 6e65 775f 5f28 636c    def __new__(cl
+000069d0: 732c 206e 616d 652c 202a 6172 6773 2c20  s, name, *args, 
+000069e0: 636f 6d70 7574 655f 703d 5472 7565 2c20  compute_p=True, 
+000069f0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00006a00: 2020 206f 7574 5f72 7620 3d20 5f4f 7264     out_rv = _Ord
+00006a10: 6572 6564 4d75 6c74 696e 6f6d 6961 6c28  eredMultinomial(
+00006a20: 6e61 6d65 2c20 2a61 7267 732c 202a 2a6b  name, *args, **k
+00006a30: 7761 7267 7329 0a20 2020 2020 2020 2069  wargs).        i
+00006a40: 6620 636f 6d70 7574 655f 703a 0a20 2020  f compute_p:.   
+00006a50: 2020 2020 2020 2020 2070 6d2e 4465 7465           pm.Dete
+00006a60: 726d 696e 6973 7469 6328 6622 7b6e 616d  rministic(f"{nam
+00006a70: 657d 5f70 726f 6273 222c 206f 7574 5f72  e}_probs", out_r
+00006a80: 762e 6f77 6e65 722e 696e 7075 7473 5b34  v.owner.inputs[4
+00006a90: 5d2c 2064 696d 733d 6b77 6172 6773 2e67  ], dims=kwargs.g
+00006aa0: 6574 2822 6469 6d73 2229 290a 2020 2020  et("dims")).    
+00006ab0: 2020 2020 7265 7475 726e 206f 7574 5f72      return out_r
+00006ac0: 760a 0a20 2020 2040 636c 6173 736d 6574  v..    @classmet
+00006ad0: 686f 640a 2020 2020 6465 6620 6469 7374  hod.    def dist
+00006ae0: 2863 6c73 2c20 2a61 7267 732c 202a 2a6b  (cls, *args, **k
+00006af0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00006b00: 7265 7475 726e 205f 4f72 6465 7265 644d  return _OrderedM
+00006b10: 756c 7469 6e6f 6d69 616c 2e64 6973 7428  ultinomial.dist(
+00006b20: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00006b30: 0a0a 0a64 6566 2070 6f73 6465 6628 4141  ...def posdef(AA
+00006b40: 293a 0a20 2020 2074 7279 3a0a 2020 2020  ):.    try:.    
+00006b50: 2020 2020 6c69 6e61 6c67 2e63 686f 6c65      linalg.chole
+00006b60: 736b 7928 4141 290a 2020 2020 2020 2020  sky(AA).        
+00006b70: 7265 7475 726e 2031 0a20 2020 2065 7863  return 1.    exc
+00006b80: 6570 7420 6c69 6e61 6c67 2e4c 696e 416c  ept linalg.LinAl
+00006b90: 6745 7272 6f72 3a0a 2020 2020 2020 2020  gError:.        
+00006ba0: 7265 7475 726e 2030 0a0a 0a63 6c61 7373  return 0...class
+00006bb0: 2050 6f73 4465 664d 6174 7269 7828 4f70   PosDefMatrix(Op
+00006bc0: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
+00006bd0: 6865 636b 2069 6620 696e 7075 7420 6973  heck if input is
+00006be0: 2070 6f73 6974 6976 6520 6465 6669 6e69   positive defini
+00006bf0: 7465 2e20 496e 7075 7420 7368 6f75 6c64  te. Input should
+00006c00: 2062 6520 6120 7371 7561 7265 206d 6174   be a square mat
+00006c10: 7269 782e 0a0a 2020 2020 2222 220a 0a20  rix...    """.. 
+00006c20: 2020 2023 2050 726f 7065 7274 6965 7320     # Properties 
+00006c30: 6174 7472 6962 7574 650a 2020 2020 5f5f  attribute.    __
+00006c40: 7072 6f70 735f 5f20 3d20 2829 0a0a 2020  props__ = ()..  
+00006c50: 2020 2320 436f 6d70 756c 736f 7279 2069    # Compulsory i
+00006c60: 6620 6974 7970 6573 2061 6e64 206f 7479  f itypes and oty
+00006c70: 7065 7320 6172 6520 6e6f 7420 6465 6669  pes are not defi
+00006c80: 6e65 640a 0a20 2020 2064 6566 206d 616b  ned..    def mak
+00006c90: 655f 6e6f 6465 2873 656c 662c 2078 293a  e_node(self, x):
+00006ca0: 0a20 2020 2020 2020 2078 203d 2070 742e  .        x = pt.
+00006cb0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+00006cc0: 6c65 2878 290a 2020 2020 2020 2020 6173  le(x).        as
+00006cd0: 7365 7274 2078 2e6e 6469 6d20 3d3d 2032  sert x.ndim == 2
+00006ce0: 0a20 2020 2020 2020 206f 203d 2054 656e  .        o = Ten
+00006cf0: 736f 7254 7970 6528 6474 7970 653d 2269  sorType(dtype="i
+00006d00: 6e74 3822 2c20 7368 6170 653d 5b5d 2928  nt8", shape=[])(
+00006d10: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00006d20: 2041 7070 6c79 2873 656c 662c 205b 785d   Apply(self, [x]
+00006d30: 2c20 5b6f 5d29 0a0a 2020 2020 2320 5079  , [o])..    # Py
+00006d40: 7468 6f6e 2069 6d70 6c65 6d65 6e74 6174  thon implementat
+00006d50: 696f 6e3a 0a20 2020 2064 6566 2070 6572  ion:.    def per
+00006d60: 666f 726d 2873 656c 662c 206e 6f64 652c  form(self, node,
+00006d70: 2069 6e70 7574 732c 206f 7574 7075 7473   inputs, outputs
+00006d80: 293a 0a20 2020 2020 2020 2028 782c 2920  ):.        (x,) 
+00006d90: 3d20 696e 7075 7473 0a20 2020 2020 2020  = inputs.       
+00006da0: 2028 7a2c 2920 3d20 6f75 7470 7574 730a   (z,) = outputs.
+00006db0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00006dc0: 2020 2020 2020 2020 207a 5b30 5d20 3d20           z[0] = 
+00006dd0: 6e70 2e61 7272 6179 2870 6f73 6465 6628  np.array(posdef(
+00006de0: 7829 2c20 6474 7970 653d 2269 6e74 3822  x), dtype="int8"
+00006df0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00006e00: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
+00006e10: 2020 2020 2020 2020 706d 2e5f 6c6f 672e          pm._log.
+00006e20: 6578 6365 7074 696f 6e28 2246 6169 6c65  exception("Faile
+00006e30: 6420 746f 2063 6865 636b 2069 6620 2573  d to check if %s
+00006e40: 2070 6f73 6974 6976 6520 6465 6669 6e69   positive defini
+00006e50: 7465 222c 2078 290a 2020 2020 2020 2020  te", x).        
+00006e60: 2020 2020 7261 6973 650a 0a20 2020 2064      raise..    d
+00006e70: 6566 2069 6e66 6572 5f73 6861 7065 2873  ef infer_shape(s
+00006e80: 656c 662c 2066 6772 6170 682c 206e 6f64  elf, fgraph, nod
+00006e90: 652c 2073 6861 7065 7329 3a0a 2020 2020  e, shapes):.    
+00006ea0: 2020 2020 7265 7475 726e 205b 5b5d 5d0a      return [[]].
+00006eb0: 0a20 2020 2064 6566 2067 7261 6428 7365  .    def grad(se
+00006ec0: 6c66 2c20 696e 702c 2067 7261 6473 293a  lf, inp, grads):
+00006ed0: 0a20 2020 2020 2020 2028 782c 2920 3d20  .        (x,) = 
+00006ee0: 696e 700a 2020 2020 2020 2020 7265 7475  inp.        retu
+00006ef0: 726e 205b 782e 7a65 726f 735f 6c69 6b65  rn [x.zeros_like
+00006f00: 2870 7974 656e 736f 722e 636f 6e66 6967  (pytensor.config
+00006f10: 2e66 6c6f 6174 5829 5d0a 0a20 2020 2064  .floatX)]..    d
+00006f20: 6566 205f 5f73 7472 5f5f 2873 656c 6629  ef __str__(self)
+00006f30: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00006f40: 2022 4d61 7472 6978 4973 506f 7369 7469   "MatrixIsPositi
+00006f50: 7665 4465 6669 6e69 7465 220a 0a0a 6d61  veDefinite"...ma
+00006f60: 7472 6978 5f70 6f73 5f64 6566 203d 2050  trix_pos_def = P
+00006f70: 6f73 4465 664d 6174 7269 7828 290a 0a0a  osDefMatrix()...
+00006f80: 636c 6173 7320 5769 7368 6172 7452 5628  class WishartRV(
+00006f90: 5261 6e64 6f6d 5661 7269 6162 6c65 293a  RandomVariable):
+00006fa0: 0a20 2020 206e 616d 6520 3d20 2277 6973  .    name = "wis
+00006fb0: 6861 7274 220a 2020 2020 6e64 696d 5f73  hart".    ndim_s
+00006fc0: 7570 7020 3d20 320a 2020 2020 6e64 696d  upp = 2.    ndim
+00006fd0: 735f 7061 7261 6d73 203d 205b 302c 2032  s_params = [0, 2
+00006fe0: 5d0a 2020 2020 6474 7970 6520 3d20 2266  ].    dtype = "f
+00006ff0: 6c6f 6174 5822 0a20 2020 205f 7072 696e  loatX".    _prin
+00007000: 745f 6e61 6d65 203d 2028 2257 6973 6861  t_name = ("Wisha
+00007010: 7274 222c 2022 5c5c 6f70 6572 6174 6f72  rt", "\\operator
+00007020: 6e61 6d65 7b57 6973 6861 7274 7d22 290a  name{Wishart}").
+00007030: 0a20 2020 2064 6566 205f 7375 7070 5f73  .    def _supp_s
+00007040: 6861 7065 5f66 726f 6d5f 7061 7261 6d73  hape_from_params
+00007050: 2873 656c 662c 2064 6973 745f 7061 7261  (self, dist_para
+00007060: 6d73 2c20 7061 7261 6d5f 7368 6170 6573  ms, param_shapes
+00007070: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00007080: 2320 5468 6520 7368 6170 6520 6f66 2073  # The shape of s
+00007090: 6563 6f6e 6420 7061 7261 6d65 7465 7220  econd parameter 
+000070a0: 6056 6020 6465 6669 6e65 7320 7468 6520  `V` defines the 
+000070b0: 7368 6170 6520 6f66 2074 6865 206f 7574  shape of the out
+000070c0: 7075 742e 0a20 2020 2020 2020 2072 6574  put..        ret
+000070d0: 7572 6e20 7375 7070 5f73 6861 7065 5f66  urn supp_shape_f
+000070e0: 726f 6d5f 7265 665f 7061 7261 6d5f 7368  rom_ref_param_sh
+000070f0: 6170 6528 0a20 2020 2020 2020 2020 2020  ape(.           
+00007100: 206e 6469 6d5f 7375 7070 3d73 656c 662e   ndim_supp=self.
+00007110: 6e64 696d 5f73 7570 702c 0a20 2020 2020  ndim_supp,.     
+00007120: 2020 2020 2020 2064 6973 745f 7061 7261         dist_para
+00007130: 6d73 3d64 6973 745f 7061 7261 6d73 2c0a  ms=dist_params,.
+00007140: 2020 2020 2020 2020 2020 2020 7061 7261              para
+00007150: 6d5f 7368 6170 6573 3d70 6172 616d 5f73  m_shapes=param_s
+00007160: 6861 7065 732c 0a20 2020 2020 2020 2020  hapes,.         
+00007170: 2020 2072 6566 5f70 6172 616d 5f69 6478     ref_param_idx
+00007180: 3d31 2c0a 2020 2020 2020 2020 290a 0a20  =1,.        ).. 
+00007190: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000071a0: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
+000071b0: 6c73 2c20 726e 672c 206e 752c 2056 2c20  ls, rng, nu, V, 
+000071c0: 7369 7a65 293a 0a20 2020 2020 2020 2073  size):.        s
+000071d0: 6369 7079 5f73 697a 6520 3d20 7369 7a65  cipy_size = size
+000071e0: 2069 6620 7369 7a65 2065 6c73 6520 3120   if size else 1 
+000071f0: 2023 2044 6566 6175 6c74 2073 697a 6520   # Default size 
+00007200: 666f 7220 5363 6970 7927 7320 7769 7368  for Scipy's wish
+00007210: 6172 742e 7276 7320 6973 2031 0a20 2020  art.rvs is 1.   
+00007220: 2020 2020 2072 6573 756c 7420 3d20 7374       result = st
+00007230: 6174 732e 7769 7368 6172 742e 7276 7328  ats.wishart.rvs(
+00007240: 696e 7428 6e75 292c 2056 2c20 7369 7a65  int(nu), V, size
+00007250: 3d73 6369 7079 5f73 697a 652c 2072 616e  =scipy_size, ran
+00007260: 646f 6d5f 7374 6174 653d 726e 6729 0a20  dom_state=rng). 
+00007270: 2020 2020 2020 2069 6620 7369 7a65 203d         if size =
+00007280: 3d20 2831 2c29 3a0a 2020 2020 2020 2020  = (1,):.        
+00007290: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000072a0: 745b 6e70 2e6e 6577 6178 6973 2c20 2e2e  t[np.newaxis, ..
+000072b0: 2e5d 0a20 2020 2020 2020 2065 6c73 653a  .].        else:
+000072c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000072d0: 7572 6e20 7265 7375 6c74 0a0a 0a77 6973  urn result...wis
+000072e0: 6861 7274 203d 2057 6973 6861 7274 5256  hart = WishartRV
+000072f0: 2829 0a0a 0a63 6c61 7373 2057 6973 6861  ()...class Wisha
+00007300: 7274 2843 6f6e 7469 6e75 6f75 7329 3a0a  rt(Continuous):.
+00007310: 2020 2020 7222 2222 0a20 2020 2057 6973      r""".    Wis
+00007320: 6861 7274 206c 6f67 2d6c 696b 656c 6968  hart log-likelih
+00007330: 6f6f 642e 0a0a 2020 2020 5468 6520 5769  ood...    The Wi
+00007340: 7368 6172 7420 6469 7374 7269 6275 7469  shart distributi
+00007350: 6f6e 2069 7320 7468 6520 7072 6f62 6162  on is the probab
+00007360: 696c 6974 7920 6469 7374 7269 6275 7469  ility distributi
+00007370: 6f6e 206f 6620 7468 650a 2020 2020 6d61  on of the.    ma
+00007380: 7869 6d75 6d2d 6c69 6b65 6c69 686f 6f64  ximum-likelihood
+00007390: 2065 7374 696d 6174 6f72 2028 4d4c 4529   estimator (MLE)
+000073a0: 206f 6620 7468 6520 7072 6563 6973 696f   of the precisio
+000073b0: 6e20 6d61 7472 6978 206f 6620 610a 2020  n matrix of a.  
+000073c0: 2020 6d75 6c74 6976 6172 6961 7465 206e    multivariate n
+000073d0: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
+000073e0: 6f6e 2e20 2049 6620 563d 312c 2074 6865  on.  If V=1, the
+000073f0: 2064 6973 7472 6962 7574 696f 6e20 6973   distribution is
+00007400: 0a20 2020 2069 6465 6e74 6963 616c 2074  .    identical t
+00007410: 6f20 7468 6520 6368 692d 7371 7561 7265  o the chi-square
+00007420: 2064 6973 7472 6962 7574 696f 6e20 7769   distribution wi
+00007430: 7468 206e 7520 6465 6772 6565 7320 6f66  th nu degrees of
+00007440: 0a20 2020 2066 7265 6564 6f6d 2e0a 0a20  .    freedom... 
+00007450: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
+00007460: 2020 2020 2066 2858 205c 6d69 6420 6e75       f(X \mid nu
+00007470: 2c20 5429 203d 0a20 2020 2020 2020 2020  , T) =.         
+00007480: 2020 5c66 7261 637b 7b5c 6d69 6420 5420    \frac{{\mid T 
+00007490: 5c6d 6964 7d5e 7b6e 752f 327d 7b5c 6d69  \mid}^{nu/2}{\mi
+000074a0: 6420 5820 5c6d 6964 7d5e 7b28 6e75 2d6b  d X \mid}^{(nu-k
+000074b0: 2d31 292f 327d 7d7b 325e 7b6e 7520 6b2f  -1)/2}}{2^{nu k/
+000074c0: 327d 0a20 2020 2020 2020 2020 2020 5c47  2}.           \G
+000074d0: 616d 6d61 5f70 286e 752f 3229 7d20 5c65  amma_p(nu/2)} \e
+000074e0: 7870 5c6c 6566 745c 7b20 2d5c 6672 6163  xp\left\{ -\frac
+000074f0: 7b31 7d7b 327d 2054 7228 5458 2920 5c72  {1}{2} Tr(TX) \r
+00007500: 6967 6874 5c7d 0a0a 2020 2020 7768 6572  ight\}..    wher
+00007510: 6520 3a6d 6174 683a 606b 6020 6973 2074  e :math:`k` is t
+00007520: 6865 2072 616e 6b20 6f66 203a 6d61 7468  he rank of :math
+00007530: 3a60 5860 2e0a 0a20 2020 203d 3d3d 3d3d  :`X`...    =====
+00007540: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+00007550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
+00007570: 2020 2053 7570 706f 7274 2020 203a 6d61     Support   :ma
+00007580: 7468 3a60 5828 7020 7820 7029 6020 706f  th:`X(p x p)` po
+00007590: 7369 7469 7665 2064 6566 696e 6974 6520  sitive definite 
+000075a0: 6d61 7472 6978 0a20 2020 204d 6561 6e20  matrix.    Mean 
+000075b0: 2020 2020 203a 6d61 7468 3a60 6e75 2056       :math:`nu V
+000075c0: 600a 2020 2020 5661 7269 616e 6365 2020  `.    Variance  
+000075d0: 3a6d 6174 683a 606e 7520 2876 5f7b 696a  :math:`nu (v_{ij
+000075e0: 7d5e 3220 2b20 765f 7b69 697d 2076 5f7b  }^2 + v_{ii} v_{
+000075f0: 6a6a 7d29 600a 2020 2020 3d3d 3d3d 3d3d  jj})`.    ======
+00007600: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+00007610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a20  =============.. 
+00007630: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00007640: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00007650: 206e 7520 3a20 7465 6e73 6f72 5f6c 696b   nu : tensor_lik
+00007660: 6520 6f66 2069 6e74 0a20 2020 2020 2020  e of int.       
+00007670: 2044 6567 7265 6573 206f 6620 6672 6565   Degrees of free
+00007680: 646f 6d2c 203e 2030 2e0a 2020 2020 5620  dom, > 0..    V 
+00007690: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+000076a0: 2066 6c6f 6174 0a20 2020 2020 2020 2070   float.        p
+000076b0: 2078 2070 2070 6f73 6974 6976 6520 6465   x p positive de
+000076c0: 6669 6e69 7465 206d 6174 7269 782e 0a0a  finite matrix...
+000076d0: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
+000076e0: 2d2d 2d0a 2020 2020 5468 6973 2064 6973  ---.    This dis
+000076f0: 7472 6962 7574 696f 6e20 6973 2075 6e75  tribution is unu
+00007700: 7361 626c 6520 696e 2061 2050 794d 4320  sable in a PyMC 
+00007710: 6d6f 6465 6c2e 2059 6f75 2073 686f 756c  model. You shoul
+00007720: 6420 696e 7374 6561 640a 2020 2020 7573  d instead.    us
+00007730: 6520 4c4b 4a43 686f 6c65 736b 7943 6f76  e LKJCholeskyCov
+00007740: 206f 7220 4c4b 4a43 6f72 722e 0a20 2020   or LKJCorr..   
+00007750: 2022 2222 0a20 2020 2072 765f 6f70 203d   """.    rv_op =
+00007760: 2077 6973 6861 7274 0a0a 2020 2020 4063   wishart..    @c
+00007770: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00007780: 6566 2064 6973 7428 636c 732c 206e 752c  ef dist(cls, nu,
+00007790: 2056 2c20 2a61 7267 732c 202a 2a6b 7761   V, *args, **kwa
+000077a0: 7267 7329 3a0a 2020 2020 2020 2020 6e75  rgs):.        nu
+000077b0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
+000077c0: 7661 7269 6162 6c65 2869 6e74 5828 6e75  variable(intX(nu
+000077d0: 2929 0a20 2020 2020 2020 2056 203d 2070  )).        V = p
+000077e0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+000077f0: 6162 6c65 2866 6c6f 6174 5828 5629 290a  able(floatX(V)).
+00007800: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
+00007810: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00007820: 2020 2020 2254 6865 2057 6973 6861 7274      "The Wishart
+00007830: 2064 6973 7472 6962 7574 696f 6e20 6361   distribution ca
+00007840: 6e20 6375 7272 656e 746c 7920 6e6f 7420  n currently not 
+00007850: 6265 2075 7365 6420 220a 2020 2020 2020  be used ".      
+00007860: 2020 2020 2020 2266 6f72 204d 434d 4320        "for MCMC 
+00007870: 7361 6d70 6c69 6e67 2e20 5468 6520 7072  sampling. The pr
+00007880: 6f62 6162 696c 6974 7920 6f66 2073 616d  obability of sam
+00007890: 706c 696e 6720 6120 220a 2020 2020 2020  pling a ".      
+000078a0: 2020 2020 2020 2273 796d 6d65 7472 6963        "symmetric
+000078b0: 206d 6174 7269 7820 6973 2062 6173 6963   matrix is basic
+000078c0: 616c 6c79 207a 6572 6f2e 2049 6e73 7465  ally zero. Inste
+000078d0: 6164 2c20 706c 6561 7365 2022 0a20 2020  ad, please ".   
+000078e0: 2020 2020 2020 2020 2022 7573 6520 4c4b           "use LK
+000078f0: 4a43 686f 6c65 736b 7943 6f76 206f 7220  JCholeskyCov or 
+00007900: 4c4b 4a43 6f72 722e 2046 6f72 206d 6f72  LKJCorr. For mor
+00007910: 6520 696e 666f 726d 6174 696f 6e20 220a  e information ".
+00007920: 2020 2020 2020 2020 2020 2020 226f 6e20              "on 
+00007930: 7468 6520 6973 7375 6573 2073 7572 726f  the issues surro
+00007940: 756e 6469 6e67 2074 6865 2057 6973 6861  unding the Wisha
+00007950: 7274 2073 6565 2068 6572 653a 2022 0a20  rt see here: ". 
+00007960: 2020 2020 2020 2020 2020 2022 6874 7470             "http
+00007970: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00007980: 796d 632d 6465 7673 2f70 796d 632f 6973  ymc-devs/pymc/is
+00007990: 7375 6573 2f35 3338 2e22 2c0a 2020 2020  sues/538.",.    
+000079a0: 2020 2020 2020 2020 5573 6572 5761 726e          UserWarn
+000079b0: 696e 672c 0a20 2020 2020 2020 2029 0a0a  ing,.        )..
+000079c0: 2020 2020 2020 2020 2320 6d65 616e 203d          # mean =
+000079d0: 206e 7520 2a20 560a 2020 2020 2020 2020   nu * V.        
+000079e0: 2320 7020 3d20 562e 7368 6170 655b 305d  # p = V.shape[0]
+000079f0: 0a20 2020 2020 2020 2023 206d 6f64 6520  .        # mode 
+00007a00: 3d20 7074 2e73 7769 7463 6828 7074 2e67  = pt.switch(pt.g
+00007a10: 6528 6e75 2c20 7020 2b20 3129 2c20 286e  e(nu, p + 1), (n
+00007a20: 7520 2d20 7020 2d20 3129 202a 2056 2c20  u - p - 1) * V, 
+00007a30: 6e70 2e6e 616e 290a 2020 2020 2020 2020  np.nan).        
+00007a40: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
+00007a50: 6973 7428 5b6e 752c 2056 5d2c 202a 6172  ist([nu, V], *ar
+00007a60: 6773 2c20 2a2a 6b77 6172 6773 290a 0a20  gs, **kwargs).. 
+00007a70: 2020 2064 6566 206c 6f67 7028 582c 206e     def logp(X, n
+00007a80: 752c 2056 293a 0a20 2020 2020 2020 2022  u, V):.        "
+00007a90: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
+00007aa0: 6c61 7465 206c 6f67 2d70 726f 6261 6269  late log-probabi
+00007ab0: 6c69 7479 206f 6620 5769 7368 6172 7420  lity of Wishart 
+00007ac0: 6469 7374 7269 6275 7469 6f6e 0a20 2020  distribution.   
+00007ad0: 2020 2020 2061 7420 7370 6563 6966 6965       at specifie
+00007ae0: 6420 7661 6c75 652e 0a0a 2020 2020 2020  d value...      
+00007af0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00007b00: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00007b10: 2020 2020 2020 2020 583a 206e 756d 6572          X: numer
+00007b20: 6963 0a20 2020 2020 2020 2020 2020 2056  ic.            V
+00007b30: 616c 7565 2066 6f72 2077 6869 6368 206c  alue for which l
+00007b40: 6f67 2d70 726f 6261 6269 6c69 7479 2069  og-probability i
+00007b50: 7320 6361 6c63 756c 6174 6564 2e0a 0a20  s calculated... 
+00007b60: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00007b70: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00007b80: 2020 2020 2020 2054 656e 736f 7256 6172         TensorVar
+00007b90: 6961 626c 650a 2020 2020 2020 2020 2222  iable.        ""
+00007ba0: 220a 0a20 2020 2020 2020 2070 203d 2056  "..        p = V
+00007bb0: 2e73 6861 7065 5b30 5d0a 0a20 2020 2020  .shape[0]..     
+00007bc0: 2020 2049 5649 203d 2064 6574 2856 290a     IVI = det(V).
+00007bd0: 2020 2020 2020 2020 4958 4920 3d20 6465          IXI = de
+00007be0: 7428 5829 0a0a 2020 2020 2020 2020 7265  t(X)..        re
+00007bf0: 7475 726e 2063 6865 636b 5f70 6172 616d  turn check_param
+00007c00: 6574 6572 7328 0a20 2020 2020 2020 2020  eters(.         
+00007c10: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00007c20: 2020 2020 2028 6e75 202d 2070 202d 2031       (nu - p - 1
+00007c30: 2920 2a20 7074 2e6c 6f67 2849 5849 290a  ) * pt.log(IXI).
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2d20 7472 6163 6528 6d61 7472 6978 5f69  - trace(matrix_i
+00007c60: 6e76 6572 7365 2856 292e 646f 7428 5829  nverse(V).dot(X)
+00007c70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007c80: 2020 2d20 6e75 202a 2070 202a 2070 742e    - nu * p * pt.
+00007c90: 6c6f 6728 3229 0a20 2020 2020 2020 2020  log(2).         
+00007ca0: 2020 2020 2020 202d 206e 7520 2a20 7074         - nu * pt
+00007cb0: 2e6c 6f67 2849 5649 290a 2020 2020 2020  .log(IVI).      
+00007cc0: 2020 2020 2020 2020 2020 2d20 3220 2a20            - 2 * 
+00007cd0: 6d75 6c74 6967 616d 6d61 6c6e 286e 7520  multigammaln(nu 
+00007ce0: 2f20 322e 302c 2070 290a 2020 2020 2020  / 2.0, p).      
+00007cf0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00007d00: 2020 2020 2f20 322c 0a20 2020 2020 2020      / 2,.       
+00007d10: 2020 2020 206d 6174 7269 785f 706f 735f       matrix_pos_
+00007d20: 6465 6628 5829 2c0a 2020 2020 2020 2020  def(X),.        
+00007d30: 2020 2020 7074 2e65 7128 582c 2058 2e54      pt.eq(X, X.T
+00007d40: 292c 0a20 2020 2020 2020 2020 2020 206e  ),.            n
+00007d50: 7520 3e20 2870 202d 2031 292c 0a20 2020  u > (p - 1),.   
+00007d60: 2020 2020 2029 0a0a 0a64 6566 2057 6973       )...def Wis
+00007d70: 6861 7274 4261 7274 6c65 7474 286e 616d  hartBartlett(nam
+00007d80: 652c 2053 2c20 6e75 2c20 6973 5f63 686f  e, S, nu, is_cho
+00007d90: 6c65 736b 793d 4661 6c73 652c 2072 6574  lesky=False, ret
+00007da0: 7572 6e5f 6368 6f6c 6573 6b79 3d46 616c  urn_cholesky=Fal
+00007db0: 7365 2c20 696e 6974 7661 6c3d 4e6f 6e65  se, initval=None
+00007dc0: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
+00007dd0: 4261 7274 6c65 7474 2064 6563 6f6d 706f  Bartlett decompo
+00007de0: 7369 7469 6f6e 206f 6620 7468 6520 5769  sition of the Wi
+00007df0: 7368 6172 7420 6469 7374 7269 6275 7469  shart distributi
+00007e00: 6f6e 2e20 4173 2074 6865 2057 6973 6861  on. As the Wisha
+00007e10: 7274 0a20 2020 2064 6973 7472 6962 7574  rt.    distribut
+00007e20: 696f 6e20 7265 7175 6972 6573 2074 6865  ion requires the
+00007e30: 206d 6174 7269 7820 746f 2062 6520 7379   matrix to be sy
+00007e40: 6d6d 6574 7269 6320 706f 7369 7469 7665  mmetric positive
+00007e50: 2073 656d 692d 6465 6669 6e69 7465 0a20   semi-definite. 
+00007e60: 2020 2069 7420 6973 2069 6d70 6f73 7369     it is impossi
+00007e70: 626c 6520 666f 7220 4d43 4d43 2074 6f20  ble for MCMC to 
+00007e80: 6576 6572 2070 726f 706f 7365 2061 6363  ever propose acc
+00007e90: 6570 7461 626c 6520 6d61 7472 6963 6573  eptable matrices
+00007ea0: 2e0a 0a20 2020 2049 6e73 7465 6164 2c20  ...    Instead, 
+00007eb0: 7765 2063 616e 2075 7365 2074 6865 2042  we can use the B
+00007ec0: 6172 6c65 7474 2064 6563 6f6d 706f 7369  arlett decomposi
+00007ed0: 7469 6f6e 2077 6869 6368 2073 616d 706c  tion which sampl
+00007ee0: 6573 2061 206c 6f77 6572 0a20 2020 2064  es a lower.    d
+00007ef0: 6961 676f 6e61 6c20 6d61 7472 6978 2e20  iagonal matrix. 
+00007f00: 5370 6563 6966 6963 616c 6c79 3a0a 0a20  Specifically:.. 
+00007f10: 2020 202e 2e20 6d61 7468 3a3a 0a20 2020     .. math::.   
+00007f20: 2020 2020 205c 7465 7874 7b49 667d 204c       \text{If} L
+00007f30: 205c 7369 6d20 5c62 6567 696e 7b70 6d61   \sim \begin{pma
+00007f40: 7472 6978 7d0a 2020 2020 2020 2020 5c73  trix}.        \s
+00007f50: 7172 747b 635f 317d 2026 2030 2026 2030  qrt{c_1} & 0 & 0
+00007f60: 205c 5c0a 2020 2020 2020 2020 7a5f 7b32   \\.        z_{2
+00007f70: 317d 2026 205c 7371 7274 7b63 5f32 7d20  1} & \sqrt{c_2} 
+00007f80: 2620 3020 5c5c 0a20 2020 2020 2020 207a  & 0 \\.        z
+00007f90: 5f7b 3331 7d20 2620 7a5f 7b33 327d 2026  _{31} & z_{32} &
+00007fa0: 205c 7371 7274 7b63 5f33 7d0a 2020 2020   \sqrt{c_3}.    
+00007fb0: 2020 2020 5c65 6e64 7b70 6d61 7472 6978      \end{pmatrix
+00007fc0: 7d0a 0a20 2020 2020 2020 205c 7465 7874  }..        \text
+00007fd0: 7b77 6974 687d 2063 5f69 205c 7369 6d20  {with} c_i \sim 
+00007fe0: 5c63 6869 5e32 286e 2d69 2b31 2920 5c74  \chi^2(n-i+1) \t
+00007ff0: 6578 747b 2061 6e64 207d 206e 5f7b 696a  ext{ and } n_{ij
+00008000: 7d20 5c73 696d 205c 6d61 7468 6361 6c7b  } \sim \mathcal{
+00008010: 4e7d 2830 2c20 3129 2c20 5c74 6578 747b  N}(0, 1), \text{
+00008020: 7468 656e 7d20 5c5c 0a20 2020 2020 2020  then} \\.       
+00008030: 204c 205c 7469 6d65 7320 4120 5c74 696d   L \times A \tim
+00008040: 6573 2041 2e54 205c 7469 6d65 7320 4c2e  es A.T \times L.
+00008050: 5420 5c73 696d 205c 7465 7874 7b57 6973  T \sim \text{Wis
+00008060: 6861 7274 7d28 4c20 5c74 696d 6573 204c  hart}(L \times L
+00008070: 2e54 2c20 5c6e 7529 0a0a 2020 2020 5365  .T, \nu)..    Se
+00008080: 6520 6874 7470 3a2f 2f65 6e2e 7769 6b69  e http://en.wiki
+00008090: 7065 6469 612e 6f72 672f 7769 6b69 2f57  pedia.org/wiki/W
+000080a0: 6973 6861 7274 5f64 6973 7472 6962 7574  ishart_distribut
+000080b0: 696f 6e23 4261 7274 6c65 7474 5f64 6563  ion#Bartlett_dec
+000080c0: 6f6d 706f 7369 7469 6f6e 0a20 2020 2066  omposition.    f
+000080d0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+000080e0: 696f 6e2e 0a0a 2020 2020 5061 7261 6d65  ion...    Parame
+000080f0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00008100: 2d2d 2d0a 2020 2020 5320 3a20 6e64 6172  ---.    S : ndar
+00008110: 7261 790a 2020 2020 2020 2020 7020 7820  ray.        p x 
+00008120: 7020 706f 7369 7469 7665 2064 6566 696e  p positive defin
+00008130: 6974 6520 6d61 7472 6978 0a20 2020 2020  ite matrix.     
+00008140: 2020 204f 723a 0a20 2020 2020 2020 2070     Or:.        p
+00008150: 2078 2070 206c 6f77 6572 2d74 7269 616e   x p lower-trian
+00008160: 6775 6c61 7220 6d61 7472 6978 2074 6861  gular matrix tha
+00008170: 7420 6973 2074 6865 2043 686f 6c65 736b  t is the Cholesk
+00008180: 7920 6661 6374 6f72 0a20 2020 2020 2020  y factor.       
+00008190: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
+000081a0: 6365 206d 6174 7269 782e 0a20 2020 206e  ce matrix..    n
+000081b0: 7520 3a20 7465 6e73 6f72 5f6c 696b 6520  u : tensor_like 
+000081c0: 6f66 2069 6e74 0a20 2020 2020 2020 2044  of int.        D
+000081d0: 6567 7265 6573 206f 6620 6672 6565 646f  egrees of freedo
+000081e0: 6d2c 203e 2064 696d 2853 292e 0a20 2020  m, > dim(S)..   
+000081f0: 2069 735f 6368 6f6c 6573 6b79 203a 2062   is_cholesky : b
+00008200: 6f6f 6c2c 2064 6566 6175 6c74 3d46 616c  ool, default=Fal
+00008210: 7365 0a20 2020 2020 2020 2049 6e70 7574  se.        Input
+00008220: 206d 6174 7269 7820 5320 6973 2061 6c72   matrix S is alr
+00008230: 6561 6479 2043 686f 6c65 736b 7920 6465  eady Cholesky de
+00008240: 636f 6d70 6f73 6564 2061 7320 532e 5420  composed as S.T 
+00008250: 2a20 530a 2020 2020 7265 7475 726e 5f63  * S.    return_c
+00008260: 686f 6c65 736b 7920 3a20 626f 6f6c 2c20  holesky : bool, 
+00008270: 6465 6661 756c 743d 4661 6c73 650a 2020  default=False.  
+00008280: 2020 2020 2020 4f6e 6c79 2072 6574 7572        Only retur
+00008290: 6e20 7468 6520 4368 6f6c 6573 6b79 2064  n the Cholesky d
+000082a0: 6563 6f6d 706f 7365 6420 6d61 7472 6978  ecomposed matrix
+000082b0: 2e0a 2020 2020 696e 6974 7661 6c20 3a20  ..    initval : 
+000082c0: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+000082d0: 7020 7820 7020 706f 7369 7469 7665 2064  p x p positive d
+000082e0: 6566 696e 6974 6520 6d61 7472 6978 2075  efinite matrix u
+000082f0: 7365 6420 746f 2069 6e69 7469 616c 697a  sed to initializ
+00008300: 650a 0a20 2020 204e 6f74 6573 0a20 2020  e..    Notes.   
+00008310: 202d 2d2d 2d2d 0a20 2020 2054 6869 7320   -----.    This 
+00008320: 6973 206e 6f74 2061 2073 7461 6e64 6172  is not a standar
+00008330: 6420 4469 7374 7269 6275 7469 6f6e 2063  d Distribution c
+00008340: 6c61 7373 2062 7574 2066 6f6c 6c6f 7773  lass but follows
+00008350: 2061 2073 696d 696c 6172 0a20 2020 2069   a similar.    i
+00008360: 6e74 6572 6661 6365 2e20 4265 7369 6465  nterface. Beside
+00008370: 7320 7468 6520 5769 7368 6172 7420 6469  s the Wishart di
+00008380: 7374 7269 6275 7469 6f6e 2c20 6974 2077  stribution, it w
+00008390: 696c 6c20 6164 6420 5256 730a 2020 2020  ill add RVs.    
+000083a0: 6e61 6d65 5f63 2061 6e64 206e 616d 655f  name_c and name_
+000083b0: 7a20 746f 2079 6f75 7220 6d6f 6465 6c20  z to your model 
+000083c0: 7768 6963 6820 6d61 6b65 2075 7020 7468  which make up th
+000083d0: 6520 6d61 7472 6978 2e0a 0a20 2020 2054  e matrix...    T
+000083e0: 6869 7320 6469 7374 7269 6275 7469 6f6e  his distribution
+000083f0: 2069 7320 7573 7561 6c6c 7920 6120 6261   is usually a ba
+00008400: 6420 6964 6561 2074 6f20 7573 6520 6173  d idea to use as
+00008410: 2061 2070 7269 6f72 2066 6f72 206d 756c   a prior for mul
+00008420: 7469 7661 7269 6174 650a 2020 2020 6e6f  tivariate.    no
+00008430: 726d 616c 2e20 596f 7520 7368 6f75 6c64  rmal. You should
+00008440: 2069 6e73 7465 6164 2075 7365 204c 4b4a   instead use LKJ
+00008450: 4368 6f6c 6573 6b79 436f 7620 6f72 204c  CholeskyCov or L
+00008460: 4b4a 436f 7272 2e0a 2020 2020 2222 220a  KJCorr..    """.
+00008470: 0a20 2020 204c 203d 2053 2069 6620 6973  .    L = S if is
+00008480: 5f63 686f 6c65 736b 7920 656c 7365 2073  _cholesky else s
+00008490: 6369 7079 2e6c 696e 616c 672e 6368 6f6c  cipy.linalg.chol
+000084a0: 6573 6b79 2853 290a 2020 2020 6469 6167  esky(S).    diag
+000084b0: 5f69 6478 203d 206e 702e 6469 6167 5f69  _idx = np.diag_i
+000084c0: 6e64 6963 6573 5f66 726f 6d28 5329 0a20  ndices_from(S). 
+000084d0: 2020 2074 7269 6c5f 6964 7820 3d20 6e70     tril_idx = np
+000084e0: 2e74 7269 6c5f 696e 6469 6365 735f 6672  .tril_indices_fr
+000084f0: 6f6d 2853 2c20 6b3d 2d31 290a 2020 2020  om(S, k=-1).    
+00008500: 6e5f 6469 6167 203d 206c 656e 2864 6961  n_diag = len(dia
+00008510: 675f 6964 785b 305d 290a 2020 2020 6e5f  g_idx[0]).    n_
+00008520: 7472 696c 203d 206c 656e 2874 7269 6c5f  tril = len(tril_
+00008530: 6964 785b 305d 290a 0a20 2020 2069 6620  idx[0])..    if 
+00008540: 696e 6974 7661 6c20 6973 206e 6f74 204e  initval is not N
+00008550: 6f6e 653a 0a20 2020 2020 2020 2023 2049  one:.        # I
+00008560: 6e76 6572 7365 2074 7261 6e73 666f 726d  nverse transform
+00008570: 0a20 2020 2020 2020 2069 6e69 7476 616c  .        initval
+00008580: 203d 206e 702e 646f 7428 6e70 2e64 6f74   = np.dot(np.dot
+00008590: 286e 702e 6c69 6e61 6c67 2e69 6e76 284c  (np.linalg.inv(L
+000085a0: 292c 2069 6e69 7476 616c 292c 206e 702e  ), initval), np.
+000085b0: 6c69 6e61 6c67 2e69 6e76 284c 2e54 2929  linalg.inv(L.T))
+000085c0: 0a20 2020 2020 2020 2069 6e69 7476 616c  .        initval
+000085d0: 203d 206c 696e 616c 672e 6368 6f6c 6573   = linalg.choles
+000085e0: 6b79 2869 6e69 7476 616c 2c20 6c6f 7765  ky(initval, lowe
+000085f0: 723d 5472 7565 290a 2020 2020 2020 2020  r=True).        
+00008600: 6469 6167 5f74 6573 7476 616c 203d 2069  diag_testval = i
+00008610: 6e69 7476 616c 5b64 6961 675f 6964 785d  nitval[diag_idx]
+00008620: 202a 2a20 320a 2020 2020 2020 2020 7472   ** 2.        tr
+00008630: 696c 5f74 6573 7476 616c 203d 2069 6e69  il_testval = ini
+00008640: 7476 616c 5b74 7269 6c5f 6964 785d 0a20  tval[tril_idx]. 
+00008650: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008660: 2064 6961 675f 7465 7374 7661 6c20 3d20   diag_testval = 
+00008670: 4e6f 6e65 0a20 2020 2020 2020 2074 7269  None.        tri
+00008680: 6c5f 7465 7374 7661 6c20 3d20 4e6f 6e65  l_testval = None
+00008690: 0a0a 2020 2020 6320 3d20 7074 2e73 7172  ..    c = pt.sqr
+000086a0: 7428 0a20 2020 2020 2020 2043 6869 5371  t(.        ChiSq
+000086b0: 7561 7265 6428 2225 735f 6322 2025 206e  uared("%s_c" % n
+000086c0: 616d 652c 206e 7520 2d20 6e70 2e61 7261  ame, nu - np.ara
+000086d0: 6e67 6528 322c 2032 202b 206e 5f64 6961  nge(2, 2 + n_dia
+000086e0: 6729 2c20 7368 6170 653d 6e5f 6469 6167  g), shape=n_diag
+000086f0: 2c20 696e 6974 7661 6c3d 6469 6167 5f74  , initval=diag_t
+00008700: 6573 7476 616c 290a 2020 2020 290a 2020  estval).    ).  
+00008710: 2020 706d 2e5f 6c6f 672e 696e 666f 2822    pm._log.info("
+00008720: 4164 6465 6420 6e65 7720 7661 7269 6162  Added new variab
+00008730: 6c65 2025 735f 6320 746f 206d 6f64 656c  le %s_c to model
+00008740: 2064 6961 676f 6e61 6c20 6f66 2057 6973   diagonal of Wis
+00008750: 6861 7274 2e22 2025 206e 616d 6529 0a20  hart." % name). 
+00008760: 2020 207a 203d 204e 6f72 6d61 6c28 2225     z = Normal("%
+00008770: 735f 7a22 2025 206e 616d 652c 2030 2e30  s_z" % name, 0.0
+00008780: 2c20 312e 302c 2073 6861 7065 3d6e 5f74  , 1.0, shape=n_t
+00008790: 7269 6c2c 2069 6e69 7476 616c 3d74 7269  ril, initval=tri
+000087a0: 6c5f 7465 7374 7661 6c29 0a20 2020 2070  l_testval).    p
+000087b0: 6d2e 5f6c 6f67 2e69 6e66 6f28 2241 6464  m._log.info("Add
+000087c0: 6564 206e 6577 2076 6172 6961 626c 6520  ed new variable 
+000087d0: 2573 5f7a 2074 6f20 6d6f 6465 6c20 6f66  %s_z to model of
+000087e0: 662d 6469 6167 6f6e 616c 7320 6f66 2057  f-diagonals of W
+000087f0: 6973 6861 7274 2e22 2025 206e 616d 6529  ishart." % name)
+00008800: 0a20 2020 2023 2043 6f6e 7374 7275 6374  .    # Construct
+00008810: 2041 206d 6174 7269 780a 2020 2020 4120   A matrix.    A 
+00008820: 3d20 7074 2e7a 6572 6f73 2853 2e73 6861  = pt.zeros(S.sha
+00008830: 7065 2c20 6474 7970 653d 6e70 2e66 6c6f  pe, dtype=np.flo
+00008840: 6174 3332 290a 2020 2020 4120 3d20 7074  at32).    A = pt
+00008850: 2e73 6574 5f73 7562 7465 6e73 6f72 2841  .set_subtensor(A
+00008860: 5b64 6961 675f 6964 785d 2c20 6329 0a20  [diag_idx], c). 
+00008870: 2020 2041 203d 2070 742e 7365 745f 7375     A = pt.set_su
+00008880: 6274 656e 736f 7228 415b 7472 696c 5f69  btensor(A[tril_i
+00008890: 6478 5d2c 207a 290a 0a20 2020 2023 204c  dx], z)..    # L
+000088a0: 202a 2041 202a 2041 2e54 202a 204c 2e54   * A * A.T * L.T
+000088b0: 207e 2057 6973 6861 7274 284c 2a4c 2e54   ~ Wishart(L*L.T
+000088c0: 2c20 6e75 290a 2020 2020 6966 2072 6574  , nu).    if ret
+000088d0: 7572 6e5f 6368 6f6c 6573 6b79 3a0a 2020  urn_cholesky:.  
+000088e0: 2020 2020 2020 7265 7475 726e 2070 6d2e        return pm.
+000088f0: 4465 7465 726d 696e 6973 7469 6328 6e61  Deterministic(na
+00008900: 6d65 2c20 7074 2e64 6f74 284c 2c20 4129  me, pt.dot(L, A)
+00008910: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00008920: 2020 2020 7265 7475 726e 2070 6d2e 4465      return pm.De
+00008930: 7465 726d 696e 6973 7469 6328 6e61 6d65  terministic(name
+00008940: 2c20 7074 2e64 6f74 2870 742e 646f 7428  , pt.dot(pt.dot(
+00008950: 7074 2e64 6f74 284c 2c20 4129 2c20 412e  pt.dot(L, A), A.
+00008960: 5429 2c20 4c2e 5429 290a 0a0a 6465 6620  T), L.T))...def 
+00008970: 5f6c 6b6a 5f6e 6f72 6d61 6c69 7a69 6e67  _lkj_normalizing
+00008980: 5f63 6f6e 7374 616e 7428 6574 612c 206e  _constant(eta, n
+00008990: 293a 0a20 2020 2023 2054 4f44 4f3a 2054  ):.    # TODO: T
+000089a0: 6869 7320 6973 206d 6978 696e 6720 7079  his is mixing py
+000089b0: 7468 6f6e 2062 7261 6e63 6869 6e67 2077  thon branching w
+000089c0: 6974 6820 7468 6520 706f 7465 6e74 6961  ith the potentia
+000089d0: 6c6c 7920 7379 6d62 6f6c 6963 206e 2061  lly symbolic n a
+000089e0: 6e64 2065 7461 2076 6172 6961 626c 6573  nd eta variables
+000089f0: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
+00008a00: 7374 616e 6365 2865 7461 2c20 2869 6e74  stance(eta, (int
+00008a10: 2c20 666c 6f61 7429 293a 0a20 2020 2020  , float)):.     
+00008a20: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00008a30: 656d 656e 7465 6445 7272 6f72 2822 6574  ementedError("et
+00008a40: 6120 6d75 7374 2062 6520 616e 2069 6e74  a must be an int
+00008a50: 206f 7220 666c 6f61 7422 290a 2020 2020   or float").    
+00008a60: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00008a70: 6528 6e2c 2069 6e74 293a 0a20 2020 2020  e(n, int):.     
+00008a80: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00008a90: 656d 656e 7465 6445 7272 6f72 2822 6e20  ementedError("n 
+00008aa0: 6d75 7374 2062 6520 616e 2069 6e74 6567  must be an integ
+00008ab0: 6572 2229 0a20 2020 2069 6620 6574 6120  er").    if eta 
+00008ac0: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
+00008ad0: 7375 6c74 203d 2067 616d 6d61 6c6e 2832  sult = gammaln(2
+00008ae0: 2e30 202a 2070 742e 6172 616e 6765 2831  .0 * pt.arange(1
+00008af0: 2c20 696e 7428 286e 202d 2031 2920 2f20  , int((n - 1) / 
+00008b00: 3229 202b 2031 2929 2e73 756d 2829 0a20  2) + 1)).sum(). 
+00008b10: 2020 2020 2020 2069 6620 6e20 2520 3220         if n % 2 
+00008b20: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00008b30: 2020 7265 7375 6c74 202b 3d20 280a 2020    result += (.  
+00008b40: 2020 2020 2020 2020 2020 2020 2020 302e                0.
+00008b50: 3235 202a 2028 6e2a 2a32 202d 2031 2920  25 * (n**2 - 1) 
+00008b60: 2a20 7074 2e6c 6f67 286e 702e 7069 290a  * pt.log(np.pi).
+00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2d20 302e 3235 202a 2028 6e20 2d20 3129  - 0.25 * (n - 1)
+00008b90: 202a 2a20 3220 2a20 7074 2e6c 6f67 2832   ** 2 * pt.log(2
+00008ba0: 2e30 290a 2020 2020 2020 2020 2020 2020  .0).            
+00008bb0: 2020 2020 2d20 286e 202d 2031 2920 2a20      - (n - 1) * 
+00008bc0: 6761 6d6d 616c 6e28 696e 7428 286e 202b  gammaln(int((n +
+00008bd0: 2031 2920 2f20 3229 290a 2020 2020 2020   1) / 2)).      
+00008be0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008bf0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008c00: 2020 7265 7375 6c74 202b 3d20 280a 2020    result += (.  
+00008c10: 2020 2020 2020 2020 2020 2020 2020 302e                0.
+00008c20: 3235 202a 206e 202a 2028 6e20 2d20 3229  25 * n * (n - 2)
+00008c30: 202a 2070 742e 6c6f 6728 6e70 2e70 6929   * pt.log(np.pi)
+00008c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c50: 202b 2030 2e32 3520 2a20 2833 202a 206e   + 0.25 * (3 * n
+00008c60: 2a2a 3220 2d20 3420 2a20 6e29 202a 2070  **2 - 4 * n) * p
+00008c70: 742e 6c6f 6728 322e 3029 0a20 2020 2020  t.log(2.0).     
+00008c80: 2020 2020 2020 2020 2020 202b 206e 202a             + n *
+00008c90: 2067 616d 6d61 6c6e 286e 202f 2032 290a   gammaln(n / 2).
+00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cb0: 2d20 286e 202d 2031 2920 2a20 6761 6d6d  - (n - 1) * gamm
+00008cc0: 616c 6e28 6e29 0a20 2020 2020 2020 2020  aln(n).         
+00008cd0: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
+00008ce0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00008cf0: 2d28 6e20 2d20 3129 202a 2067 616d 6d61  -(n - 1) * gamma
+00008d00: 6c6e 2865 7461 202b 2030 2e35 202a 2028  ln(eta + 0.5 * (
+00008d10: 6e20 2d20 3129 290a 2020 2020 2020 2020  n - 1)).        
+00008d20: 6b20 3d20 7074 2e61 7261 6e67 6528 312c  k = pt.arange(1,
+00008d30: 206e 290a 2020 2020 2020 2020 7265 7375   n).        resu
+00008d40: 6c74 202b 3d20 2830 2e35 202a 206b 202a  lt += (0.5 * k *
+00008d50: 2070 742e 6c6f 6728 6e70 2e70 6929 202b   pt.log(np.pi) +
+00008d60: 2067 616d 6d61 6c6e 2865 7461 202b 2030   gammaln(eta + 0
+00008d70: 2e35 202a 2028 6e20 2d20 3120 2d20 6b29  .5 * (n - 1 - k)
+00008d80: 2929 2e73 756d 2829 0a20 2020 2072 6574  )).sum().    ret
+00008d90: 7572 6e20 7265 7375 6c74 0a0a 0a63 6c61  urn result...cla
+00008da0: 7373 205f 4c4b 4a43 686f 6c65 736b 7943  ss _LKJCholeskyC
+00008db0: 6f76 4261 7365 5256 2852 616e 646f 6d56  ovBaseRV(RandomV
+00008dc0: 6172 6961 626c 6529 3a0a 2020 2020 6e61  ariable):.    na
+00008dd0: 6d65 203d 2022 5f6c 6b6a 6368 6f6c 6573  me = "_lkjcholes
+00008de0: 6b79 636f 7662 6173 6522 0a20 2020 206e  kycovbase".    n
+00008df0: 6469 6d5f 7375 7070 203d 2031 0a20 2020  dim_supp = 1.   
+00008e00: 206e 6469 6d73 5f70 6172 616d 7320 3d20   ndims_params = 
+00008e10: 5b30 2c20 302c 2031 5d0a 2020 2020 6474  [0, 0, 1].    dt
+00008e20: 7970 6520 3d20 2266 6c6f 6174 5822 0a20  ype = "floatX". 
+00008e30: 2020 205f 7072 696e 745f 6e61 6d65 203d     _print_name =
+00008e40: 2028 225f 6c6b 6a63 686f 6c65 736b 7963   ("_lkjcholeskyc
+00008e50: 6f76 6261 7365 222c 2022 5c5c 6f70 6572  ovbase", "\\oper
+00008e60: 6174 6f72 6e61 6d65 7b5f 6c6b 6a63 686f  atorname{_lkjcho
+00008e70: 6c65 736b 7963 6f76 6261 7365 7d22 290a  leskycovbase}").
+00008e80: 0a20 2020 2064 6566 206d 616b 655f 6e6f  .    def make_no
+00008e90: 6465 2873 656c 662c 2072 6e67 2c20 7369  de(self, rng, si
+00008ea0: 7a65 2c20 6474 7970 652c 206e 2c20 6574  ze, dtype, n, et
+00008eb0: 612c 2044 293a 0a20 2020 2020 2020 206e  a, D):.        n
+00008ec0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
+00008ed0: 7661 7269 6162 6c65 286e 290a 2020 2020  variable(n).    
+00008ee0: 2020 2020 6966 206e 6f74 206e 2e6e 6469      if not n.ndi
+00008ef0: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
+00008f00: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00008f10: 7272 6f72 2822 6e20 6d75 7374 2062 6520  rror("n must be 
+00008f20: 6120 7363 616c 6172 2028 6e64 696d 3d30  a scalar (ndim=0
+00008f30: 292e 2229 0a0a 2020 2020 2020 2020 6574  ).")..        et
+00008f40: 6120 3d20 7074 2e61 735f 7465 6e73 6f72  a = pt.as_tensor
+00008f50: 5f76 6172 6961 626c 6528 6574 6129 0a20  _variable(eta). 
+00008f60: 2020 2020 2020 2069 6620 6e6f 7420 6574         if not et
+00008f70: 612e 6e64 696d 203d 3d20 303a 0a20 2020  a.ndim == 0:.   
+00008f80: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00008f90: 616c 7565 4572 726f 7228 2265 7461 206d  alueError("eta m
+00008fa0: 7573 7420 6265 2061 2073 6361 6c61 7220  ust be a scalar 
+00008fb0: 286e 6469 6d3d 3029 2e22 290a 0a20 2020  (ndim=0).")..   
+00008fc0: 2020 2020 2044 203d 2070 742e 6173 5f74       D = pt.as_t
+00008fd0: 656e 736f 725f 7661 7269 6162 6c65 2844  ensor_variable(D
+00008fe0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00008ff0: 6e20 7375 7065 7228 292e 6d61 6b65 5f6e  n super().make_n
+00009000: 6f64 6528 726e 672c 2073 697a 652c 2064  ode(rng, size, d
+00009010: 7479 7065 2c20 6e2c 2065 7461 2c20 4429  type, n, eta, D)
+00009020: 0a0a 2020 2020 6465 6620 5f73 7570 705f  ..    def _supp_
+00009030: 7368 6170 655f 6672 6f6d 5f70 6172 616d  shape_from_param
+00009040: 7328 7365 6c66 2c20 6469 7374 5f70 6172  s(self, dist_par
+00009050: 616d 732c 2070 6172 616d 5f73 6861 7065  ams, param_shape
+00009060: 7329 3a0a 2020 2020 2020 2020 6e20 3d20  s):.        n = 
+00009070: 6469 7374 5f70 6172 616d 735b 305d 0a20  dist_params[0]. 
+00009080: 2020 2020 2020 2072 6574 7572 6e20 2828         return ((
+00009090: 6e20 2a20 286e 202b 2031 2929 202f 2f20  n * (n + 1)) // 
+000090a0: 322c 290a 0a20 2020 2064 6566 2072 6e67  2,)..    def rng
+000090b0: 5f66 6e28 7365 6c66 2c20 726e 672c 206e  _fn(self, rng, n
+000090c0: 2c20 6574 612c 2044 2c20 7369 7a65 293a  , eta, D, size):
+000090d0: 0a20 2020 2020 2020 2023 2057 6520 666c  .        # We fl
+000090e0: 6174 7465 6e20 7468 6520 7369 7a65 2074  atten the size t
+000090f0: 6f20 6d61 6b65 206f 7065 7261 7469 6f6e  o make operation
+00009100: 7320 6561 7369 6572 2c20 616e 6420 7468  s easier, and th
+00009110: 656e 2072 6562 7569 6c64 2069 740a 2020  en rebuild it.  
+00009120: 2020 2020 2020 6966 2073 697a 6520 6973        if size is
+00009130: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009140: 2020 2073 697a 6520 3d20 442e 7368 6170     size = D.shap
+00009150: 655b 3a2d 315d 0a20 2020 2020 2020 2066  e[:-1].        f
+00009160: 6c61 745f 7369 7a65 203d 206e 702e 7072  lat_size = np.pr
+00009170: 6f64 2873 697a 6529 2e61 7374 7970 6528  od(size).astype(
+00009180: 696e 7429 0a0a 2020 2020 2020 2020 4320  int)..        C 
+00009190: 3d20 4c4b 4a43 6f72 7252 562e 5f72 616e  = LKJCorrRV._ran
+000091a0: 646f 6d5f 636f 7272 5f6d 6174 7269 7828  dom_corr_matrix(
+000091b0: 726e 673d 726e 672c 206e 3d6e 2c20 6574  rng=rng, n=n, et
+000091c0: 613d 6574 612c 2066 6c61 745f 7369 7a65  a=eta, flat_size
+000091d0: 3d66 6c61 745f 7369 7a65 290a 2020 2020  =flat_size).    
+000091e0: 2020 2020 4420 3d20 442e 7265 7368 6170      D = D.reshap
+000091f0: 6528 666c 6174 5f73 697a 652c 206e 290a  e(flat_size, n).
+00009200: 2020 2020 2020 2020 4320 2a3d 2044 5b2e          C *= D[.
+00009210: 2e2e 2c20 3a2c 206e 702e 6e65 7761 7869  .., :, np.newaxi
+00009220: 735d 202a 2044 5b2e 2e2e 2c20 6e70 2e6e  s] * D[..., np.n
+00009230: 6577 6178 6973 2c20 3a5d 0a0a 2020 2020  ewaxis, :]..    
+00009240: 2020 2020 7472 696c 5f69 6478 203d 206e      tril_idx = n
+00009250: 702e 7472 696c 5f69 6e64 6963 6573 286e  p.tril_indices(n
+00009260: 2c20 6b3d 3029 0a20 2020 2020 2020 2073  , k=0).        s
+00009270: 616d 706c 6573 203d 206e 702e 6c69 6e61  amples = np.lina
+00009280: 6c67 2e63 686f 6c65 736b 7928 4329 5b2e  lg.cholesky(C)[.
+00009290: 2e2e 2c20 7472 696c 5f69 6478 5b30 5d2c  .., tril_idx[0],
+000092a0: 2074 7269 6c5f 6964 785b 315d 5d0a 0a20   tril_idx[1]].. 
+000092b0: 2020 2020 2020 2069 6620 7369 7a65 2069         if size i
+000092c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000092d0: 2020 2020 7361 6d70 6c65 7320 3d20 7361      samples = sa
+000092e0: 6d70 6c65 735b 305d 0a20 2020 2020 2020  mples[0].       
+000092f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009300: 2020 2064 6973 745f 7368 6170 6520 3d20     dist_shape = 
+00009310: 286e 202a 2028 6e20 2b20 3129 2920 2f2f  (n * (n + 1)) //
+00009320: 2032 0a20 2020 2020 2020 2020 2020 2073   2.            s
+00009330: 616d 706c 6573 203d 206e 702e 7265 7368  amples = np.resh
+00009340: 6170 6528 7361 6d70 6c65 732c 2028 2a73  ape(samples, (*s
+00009350: 697a 652c 2064 6973 745f 7368 6170 6529  ize, dist_shape)
+00009360: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00009370: 6e20 7361 6d70 6c65 730a 0a0a 5f6c 6a6b  n samples..._ljk
+00009380: 5f63 686f 6c65 736b 795f 636f 765f 6261  _cholesky_cov_ba
+00009390: 7365 203d 205f 4c4b 4a43 686f 6c65 736b  se = _LKJCholesk
+000093a0: 7943 6f76 4261 7365 5256 2829 0a0a 0a23  yCovBaseRV()...#
+000093b0: 205f 4c4b 4a43 686f 6c65 736b 7943 6f76   _LKJCholeskyCov
+000093c0: 4261 7365 5256 2072 6571 7569 7265 7320  BaseRV requires 
+000093d0: 6120 7072 6f70 6572 6c79 2073 6861 7065  a properly shape
+000093e0: 6420 6044 602c 2077 6869 6368 206d 6561  d `D`, which mea
+000093f0: 6e73 2074 6865 2076 6172 6961 626c 6520  ns the variable 
+00009400: 6361 6e27 740a 2320 6265 2073 6166 656c  can't.# be safel
+00009410: 7920 7265 7369 7a65 642e 2042 6563 6175  y resized. Becau
+00009420: 7365 206f 6620 7468 6973 2c20 7765 2061  se of this, we a
+00009430: 6464 2074 6865 2074 6869 6e20 5379 6d62  dd the thin Symb
+00009440: 6f6c 6963 5261 6e64 6f6d 5661 7269 6162  olicRandomVariab
+00009450: 6c65 2077 7261 7070 6572 0a63 6c61 7373  le wrapper.class
+00009460: 205f 4c4b 4a43 686f 6c65 736b 7943 6f76   _LKJCholeskyCov
+00009470: 5256 2853 796d 626f 6c69 6352 616e 646f  RV(SymbolicRando
+00009480: 6d56 6172 6961 626c 6529 3a0a 2020 2020  mVariable):.    
+00009490: 6465 6661 756c 745f 6f75 7470 7574 203d  default_output =
+000094a0: 2031 0a20 2020 205f 7072 696e 745f 6e61   1.    _print_na
+000094b0: 6d65 203d 2028 225f 6c6b 6a63 686f 6c65  me = ("_lkjchole
+000094c0: 736b 7963 6f76 222c 2022 5c5c 6f70 6572  skycov", "\\oper
+000094d0: 6174 6f72 6e61 6d65 7b5f 6c6b 6a63 686f  atorname{_lkjcho
+000094e0: 6c65 736b 7963 6f76 7d22 290a 0a20 2020  leskycov}")..   
+000094f0: 2064 6566 2075 7064 6174 6528 7365 6c66   def update(self
+00009500: 2c20 6e6f 6465 293a 0a20 2020 2020 2020  , node):.       
+00009510: 2072 6574 7572 6e20 7b6e 6f64 652e 696e   return {node.in
+00009520: 7075 7473 5b30 5d3a 206e 6f64 652e 6f75  puts[0]: node.ou
+00009530: 7470 7574 735b 305d 7d0a 0a0a 636c 6173  tputs[0]}...clas
+00009540: 7320 5f4c 4b4a 4368 6f6c 6573 6b79 436f  s _LKJCholeskyCo
+00009550: 7628 4469 7374 7269 6275 7469 6f6e 293a  v(Distribution):
+00009560: 0a20 2020 2072 2222 2255 6e64 6572 6c79  .    r"""Underly
+00009570: 696e 6720 636c 6173 7320 666f 7220 636f  ing class for co
+00009580: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+00009590: 7769 7468 204c 4b4a 2064 6973 7472 6962  with LKJ distrib
+000095a0: 7574 6564 2063 6f72 7265 6c61 7469 6f6e  uted correlation
+000095b0: 732e 0a20 2020 2053 6565 2064 6f63 7320  s..    See docs 
+000095c0: 666f 7220 4c4b 4a43 686f 6c65 736b 7943  for LKJCholeskyC
+000095d0: 6f76 2066 756e 6374 696f 6e20 666f 7220  ov function for 
+000095e0: 6d6f 7265 2064 6574 6169 6c73 206f 6e20  more details on 
+000095f0: 686f 7720 746f 2075 7365 2069 7420 696e  how to use it in
+00009600: 206d 6f64 656c 732e 0a20 2020 2022 2222   models..    """
+00009610: 0a0a 2020 2020 7276 5f74 7970 6520 3d20  ..    rv_type = 
+00009620: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7652  _LKJCholeskyCovR
+00009630: 560a 0a20 2020 2040 636c 6173 736d 6574  V..    @classmet
+00009640: 686f 640a 2020 2020 6465 6620 6469 7374  hod.    def dist
+00009650: 2863 6c73 2c20 6e2c 2065 7461 2c20 7364  (cls, n, eta, sd
+00009660: 5f64 6973 742c 202a 2a6b 7761 7267 7329  _dist, **kwargs)
+00009670: 3a0a 2020 2020 2020 2020 6e20 3d20 7074  :.        n = pt
+00009680: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+00009690: 626c 6528 696e 7458 286e 2929 0a20 2020  ble(intX(n)).   
+000096a0: 2020 2020 2065 7461 203d 2070 742e 6173       eta = pt.as
+000096b0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+000096c0: 2866 6c6f 6174 5828 6574 6129 290a 0a20  (floatX(eta)).. 
+000096d0: 2020 2020 2020 2069 6620 6e6f 7420 280a         if not (.
+000096e0: 2020 2020 2020 2020 2020 2020 6973 696e              isin
+000096f0: 7374 616e 6365 2873 645f 6469 7374 2c20  stance(sd_dist, 
+00009700: 5661 7269 6162 6c65 290a 2020 2020 2020  Variable).      
+00009710: 2020 2020 2020 616e 6420 7364 5f64 6973        and sd_dis
+00009720: 742e 6f77 6e65 7220 6973 206e 6f74 204e  t.owner is not N
+00009730: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00009740: 616e 6420 6973 696e 7374 616e 6365 2873  and isinstance(s
+00009750: 645f 6469 7374 2e6f 776e 6572 2e6f 702c  d_dist.owner.op,
+00009760: 2028 5261 6e64 6f6d 5661 7269 6162 6c65   (RandomVariable
+00009770: 2c20 5379 6d62 6f6c 6963 5261 6e64 6f6d  , SymbolicRandom
+00009780: 5661 7269 6162 6c65 2929 0a20 2020 2020  Variable)).     
+00009790: 2020 2020 2020 2061 6e64 2073 645f 6469         and sd_di
+000097a0: 7374 2e6f 776e 6572 2e6f 702e 6e64 696d  st.owner.op.ndim
+000097b0: 5f73 7570 7020 3c20 320a 2020 2020 2020  _supp < 2.      
+000097c0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+000097d0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000097e0: 2822 7364 5f64 6973 7420 6d75 7374 2062  ("sd_dist must b
+000097f0: 6520 6120 7363 616c 6172 206f 7220 7665  e a scalar or ve
+00009800: 6374 6f72 2064 6973 7472 6962 7574 696f  ctor distributio
+00009810: 6e20 7661 7269 6162 6c65 2229 0a0a 2020  n variable")..  
+00009820: 2020 2020 2020 6368 6563 6b5f 6469 7374        check_dist
+00009830: 5f6e 6f74 5f72 6567 6973 7465 7265 6428  _not_registered(
+00009840: 7364 5f64 6973 7429 0a20 2020 2020 2020  sd_dist).       
+00009850: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00009860: 6469 7374 285b 6e2c 2065 7461 2c20 7364  dist([n, eta, sd
+00009870: 5f64 6973 745d 2c20 2a2a 6b77 6172 6773  _dist], **kwargs
+00009880: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+00009890: 686f 640a 2020 2020 6465 6620 7276 5f6f  hod.    def rv_o
+000098a0: 7028 636c 732c 206e 2c20 6574 612c 2073  p(cls, n, eta, s
+000098b0: 645f 6469 7374 2c20 7369 7a65 3d4e 6f6e  d_dist, size=Non
+000098c0: 6529 3a0a 2020 2020 2020 2020 2320 5765  e):.        # We
+000098d0: 2072 6573 697a 6520 7468 6520 7364 5f64   resize the sd_d
+000098e0: 6973 7420 6175 746f 6d61 7469 6361 6c6c  ist automaticall
+000098f0: 7920 736f 2074 6861 7420 6974 2068 6173  y so that it has
+00009900: 2028 7369 7a65 2078 206e 2920 696e 6465   (size x n) inde
+00009910: 7065 6e64 656e 740a 2020 2020 2020 2020  pendent.        
+00009920: 2320 6472 6177 7320 7768 6963 6820 6973  # draws which is
+00009930: 2077 6861 7420 7468 6520 605f 4c4b 4a43   what the `_LKJC
+00009940: 686f 6c65 736b 7943 6f76 4261 7365 5256  holeskyCovBaseRV
+00009950: 2e72 6e67 5f66 6e60 2065 7870 6563 7473  .rng_fn` expects
+00009960: 2e20 5468 6973 206d 616b 6573 2074 6865  . This makes the
+00009970: 0a20 2020 2020 2020 2023 2072 616e 646f  .        # rando
+00009980: 6d20 616e 6420 6c6f 6770 206d 6574 686f  m and logp metho
+00009990: 6473 2065 7175 6976 616c 656e 742c 2061  ds equivalent, a
+000099a0: 7320 7468 6520 6c61 7474 6572 2061 6c73  s the latter als
+000099b0: 6f20 6173 7375 6d65 7320 6120 756e 6971  o assumes a uniq
+000099c0: 7565 2076 616c 7565 0a20 2020 2020 2020  ue value.       
+000099d0: 2023 2066 6f72 2065 6163 6820 6469 6167   # for each diag
+000099e0: 6f6e 616c 2065 6c65 6d65 6e74 2e0a 2020  onal element..  
+000099f0: 2020 2020 2020 2320 5369 6e63 6520 6065        # Since `e
+00009a00: 7461 6020 616e 6420 606e 6020 6172 6520  ta` and `n` are 
+00009a10: 666f 7263 6564 2074 6f20 6265 2073 6361  forced to be sca
+00009a20: 6c61 7273 2077 6520 646f 6e27 7420 6e65  lars we don't ne
+00009a30: 6564 2074 6f20 776f 7272 7920 6162 6f75  ed to worry abou
+00009a40: 740a 2020 2020 2020 2020 2320 696d 706c  t.        # impl
+00009a50: 6965 6420 6261 7463 6865 6420 6469 6d65  ied batched dime
+00009a60: 6e73 696f 6e73 2066 726f 6d20 7468 6f73  nsions from thos
+00009a70: 6520 666f 7220 7468 6520 7469 6d65 2062  e for the time b
+00009a80: 6569 6e67 2e0a 2020 2020 2020 2020 6966  eing..        if
+00009a90: 2073 697a 6520 6973 204e 6f6e 653a 0a20   size is None:. 
+00009aa0: 2020 2020 2020 2020 2020 2073 697a 6520             size 
+00009ab0: 3d20 7364 5f64 6973 742e 7368 6170 655b  = sd_dist.shape[
+00009ac0: 3a2d 315d 0a20 2020 2020 2020 2073 6861  :-1].        sha
+00009ad0: 7065 203d 2074 7570 6c65 2873 697a 6529  pe = tuple(size)
+00009ae0: 202b 2028 6e2c 290a 2020 2020 2020 2020   + (n,).        
+00009af0: 6966 2073 645f 6469 7374 2e6f 776e 6572  if sd_dist.owner
+00009b00: 2e6f 702e 6e64 696d 5f73 7570 7020 3d3d  .op.ndim_supp ==
+00009b10: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00009b20: 7364 5f64 6973 7420 3d20 6368 616e 6765  sd_dist = change
+00009b30: 5f64 6973 745f 7369 7a65 2873 645f 6469  _dist_size(sd_di
+00009b40: 7374 2c20 7368 6170 6529 0a20 2020 2020  st, shape).     
+00009b50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009b60: 2020 2020 2023 2054 6865 2073 7570 706f       # The suppo
+00009b70: 7274 2073 6861 7065 206d 7573 7420 6265  rt shape must be
+00009b80: 2060 6e60 2062 7574 2077 6520 6861 7665   `n` but we have
+00009b90: 206e 6f20 7761 7920 6f66 2063 6f6e 7472   no way of contr
+00009ba0: 6f6c 6c69 6e67 2069 740a 2020 2020 2020  olling it.      
+00009bb0: 2020 2020 2020 7364 5f64 6973 7420 3d20        sd_dist = 
+00009bc0: 6368 616e 6765 5f64 6973 745f 7369 7a65  change_dist_size
+00009bd0: 2873 645f 6469 7374 2c20 7368 6170 655b  (sd_dist, shape[
+00009be0: 3a2d 315d 290a 0a20 2020 2020 2020 2023  :-1])..        #
+00009bf0: 2043 7265 6174 6520 6e65 7720 726e 6720   Create new rng 
+00009c00: 666f 7220 7468 6520 5f6c 6b6a 6368 6f6c  for the _lkjchol
+00009c10: 6573 6b79 636f 7620 696e 7465 726e 616c  eskycov internal
+00009c20: 2052 560a 2020 2020 2020 2020 726e 6720   RV.        rng 
+00009c30: 3d20 7079 7465 6e73 6f72 2e73 6861 7265  = pytensor.share
+00009c40: 6428 6e70 2e72 616e 646f 6d2e 6465 6661  d(np.random.defa
+00009c50: 756c 745f 726e 6728 2929 0a0a 2020 2020  ult_rng())..    
+00009c60: 2020 2020 726e 675f 2c20 6e5f 2c20 6574      rng_, n_, et
+00009c70: 615f 2c20 7364 5f64 6973 745f 203d 2072  a_, sd_dist_ = r
+00009c80: 6e67 2e74 7970 6528 292c 206e 2e74 7970  ng.type(), n.typ
+00009c90: 6528 292c 2065 7461 2e74 7970 6528 292c  e(), eta.type(),
+00009ca0: 2073 645f 6469 7374 2e74 7970 6528 290a   sd_dist.type().
+00009cb0: 2020 2020 2020 2020 6e65 7874 5f72 6e67          next_rng
+00009cc0: 5f2c 206c 6b6a 636f 765f 203d 205f 6c6a  _, lkjcov_ = _lj
+00009cd0: 6b5f 6368 6f6c 6573 6b79 5f63 6f76 5f62  k_cholesky_cov_b
+00009ce0: 6173 6528 6e5f 2c20 6574 615f 2c20 7364  ase(n_, eta_, sd
+00009cf0: 5f64 6973 745f 2c20 726e 673d 726e 675f  _dist_, rng=rng_
+00009d00: 292e 6f77 6e65 722e 6f75 7470 7574 730a  ).owner.outputs.
+00009d10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009d20: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7652  _LKJCholeskyCovR
+00009d30: 5628 0a20 2020 2020 2020 2020 2020 2069  V(.            i
+00009d40: 6e70 7574 733d 5b72 6e67 5f2c 206e 5f2c  nputs=[rng_, n_,
+00009d50: 2065 7461 5f2c 2073 645f 6469 7374 5f5d   eta_, sd_dist_]
+00009d60: 2c0a 2020 2020 2020 2020 2020 2020 6f75  ,.            ou
+00009d70: 7470 7574 733d 5b6e 6578 745f 726e 675f  tputs=[next_rng_
+00009d80: 2c20 6c6b 6a63 6f76 5f5d 2c0a 2020 2020  , lkjcov_],.    
+00009d90: 2020 2020 2020 2020 6e64 696d 5f73 7570          ndim_sup
+00009da0: 703d 312c 0a20 2020 2020 2020 2029 2872  p=1,.        )(r
+00009db0: 6e67 2c20 6e2c 2065 7461 2c20 7364 5f64  ng, n, eta, sd_d
+00009dc0: 6973 7429 0a0a 0a40 5f63 6861 6e67 655f  ist)...@_change_
+00009dd0: 6469 7374 5f73 697a 652e 7265 6769 7374  dist_size.regist
+00009de0: 6572 285f 4c4b 4a43 686f 6c65 736b 7943  er(_LKJCholeskyC
+00009df0: 6f76 5256 290a 6465 6620 6368 616e 6765  ovRV).def change
+00009e00: 5f4c 4b4a 4368 6f6c 656b 7379 436f 7652  _LKJCholeksyCovR
+00009e10: 565f 7369 7a65 286f 702c 2064 6973 742c  V_size(op, dist,
+00009e20: 206e 6577 5f73 697a 652c 2065 7870 616e   new_size, expan
+00009e30: 643d 4661 6c73 6529 3a0a 2020 2020 6e2c  d=False):.    n,
+00009e40: 2065 7461 2c20 7364 5f64 6973 7420 3d20   eta, sd_dist = 
+00009e50: 6469 7374 2e6f 776e 6572 2e69 6e70 7574  dist.owner.input
+00009e60: 735b 313a 5d0a 0a20 2020 2069 6620 6578  s[1:]..    if ex
+00009e70: 7061 6e64 3a0a 2020 2020 2020 2020 6f6c  pand:.        ol
+00009e80: 645f 7369 7a65 203d 2073 645f 6469 7374  d_size = sd_dist
+00009e90: 2e73 6861 7065 5b3a 2d31 5d0a 2020 2020  .shape[:-1].    
+00009ea0: 2020 2020 6e65 775f 7369 7a65 203d 2074      new_size = t
+00009eb0: 7570 6c65 286e 6577 5f73 697a 6529 202b  uple(new_size) +
+00009ec0: 2074 7570 6c65 286f 6c64 5f73 697a 6529   tuple(old_size)
+00009ed0: 0a0a 2020 2020 7265 7475 726e 205f 4c4b  ..    return _LK
+00009ee0: 4a43 686f 6c65 736b 7943 6f76 2e72 765f  JCholeskyCov.rv_
+00009ef0: 6f70 286e 2c20 6574 612c 2073 645f 6469  op(n, eta, sd_di
+00009f00: 7374 2c20 7369 7a65 3d6e 6577 5f73 697a  st, size=new_siz
+00009f10: 6529 0a0a 0a40 5f6d 6f6d 656e 742e 7265  e)...@_moment.re
+00009f20: 6769 7374 6572 285f 4c4b 4a43 686f 6c65  gister(_LKJChole
+00009f30: 736b 7943 6f76 5256 290a 6465 6620 5f4c  skyCovRV).def _L
+00009f40: 4b4a 4368 6f6c 656b 7379 436f 7652 565f  KJCholeksyCovRV_
+00009f50: 6d6f 6d65 6e74 286f 702c 2072 762c 2072  moment(op, rv, r
+00009f60: 6e67 2c20 6e2c 2065 7461 2c20 7364 5f64  ng, n, eta, sd_d
+00009f70: 6973 7429 3a0a 2020 2020 6469 6167 5f69  ist):.    diag_i
+00009f80: 6478 7320 3d20 2870 742e 6375 6d73 756d  dxs = (pt.cumsum
+00009f90: 2870 742e 6172 616e 6765 2831 2c20 6e20  (pt.arange(1, n 
+00009fa0: 2b20 3129 2920 2d20 3129 2e61 7374 7970  + 1)) - 1).astyp
+00009fb0: 6528 2269 6e74 3332 2229 0a20 2020 206d  e("int32").    m
+00009fc0: 6f6d 656e 7420 3d20 7074 2e7a 6572 6f73  oment = pt.zeros
+00009fd0: 5f6c 696b 6528 7276 290a 2020 2020 6d6f  _like(rv).    mo
+00009fe0: 6d65 6e74 203d 2070 742e 7365 745f 7375  ment = pt.set_su
+00009ff0: 6274 656e 736f 7228 6d6f 6d65 6e74 5b2e  btensor(moment[.
+0000a000: 2e2e 2c20 6469 6167 5f69 6478 735d 2c20  .., diag_idxs], 
+0000a010: 3129 0a20 2020 2072 6574 7572 6e20 6d6f  1).    return mo
+0000a020: 6d65 6e74 0a0a 0a40 5f64 6566 6175 6c74  ment...@_default
+0000a030: 5f74 7261 6e73 666f 726d 2e72 6567 6973  _transform.regis
+0000a040: 7465 7228 5f4c 4b4a 4368 6f6c 6573 6b79  ter(_LKJCholesky
+0000a050: 436f 7652 5629 0a64 6566 205f 4c4b 4a43  CovRV).def _LKJC
+0000a060: 686f 6c65 6b73 7943 6f76 5256 5f64 6566  holeksyCovRV_def
+0000a070: 6175 6c74 5f74 7261 6e73 666f 726d 286f  ault_transform(o
+0000a080: 702c 2072 7629 3a0a 2020 2020 5f2c 206e  p, rv):.    _, n
+0000a090: 2c20 5f2c 205f 203d 2072 762e 6f77 6e65  , _, _ = rv.owne
+0000a0a0: 722e 696e 7075 7473 0a20 2020 2072 6574  r.inputs.    ret
+0000a0b0: 7572 6e20 7472 616e 7366 6f72 6d73 2e43  urn transforms.C
+0000a0c0: 686f 6c65 736b 7943 6f76 5061 636b 6564  holeskyCovPacked
+0000a0d0: 286e 290a 0a0a 405f 6c6f 6770 726f 622e  (n)...@_logprob.
+0000a0e0: 7265 6769 7374 6572 285f 4c4b 4a43 686f  register(_LKJCho
+0000a0f0: 6c65 736b 7943 6f76 5256 290a 6465 6620  leskyCovRV).def 
+0000a100: 5f4c 4b4a 4368 6f6c 656b 7379 436f 7652  _LKJCholeksyCovR
+0000a110: 565f 6c6f 6770 286f 702c 2076 616c 7565  V_logp(op, value
+0000a120: 732c 2072 6e67 2c20 6e2c 2065 7461 2c20  s, rng, n, eta, 
+0000a130: 7364 5f64 6973 742c 202a 2a6b 7761 7267  sd_dist, **kwarg
+0000a140: 7329 3a0a 2020 2020 2876 616c 7565 2c29  s):.    (value,)
+0000a150: 203d 2076 616c 7565 730a 0a20 2020 2069   = values..    i
+0000a160: 6620 7661 6c75 652e 6e64 696d 203e 2031  f value.ndim > 1
+0000a170: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+0000a180: 5661 6c75 6545 7272 6f72 2822 5f4c 4b4a  ValueError("_LKJ
+0000a190: 4368 6f6c 6573 6b79 436f 7620 6c6f 6770  CholeskyCov logp
+0000a1a0: 2069 7320 6f6e 6c79 2069 6d70 6c65 6d65   is only impleme
+0000a1b0: 6e74 6564 2066 6f72 2076 6563 746f 7220  nted for vector 
+0000a1c0: 7661 6c75 6573 2028 6e64 696d 3d31 2922  values (ndim=1)"
+0000a1d0: 290a 0a20 2020 2064 6961 675f 6964 7873  )..    diag_idxs
+0000a1e0: 203d 2070 742e 6375 6d73 756d 2870 742e   = pt.cumsum(pt.
+0000a1f0: 6172 616e 6765 2831 2c20 6e20 2b20 3129  arange(1, n + 1)
+0000a200: 2920 2d20 310a 2020 2020 6375 6d73 756d  ) - 1.    cumsum
+0000a210: 203d 2070 742e 6375 6d73 756d 2876 616c   = pt.cumsum(val
+0000a220: 7565 2a2a 3229 0a20 2020 2076 6172 6961  ue**2).    varia
+0000a230: 6e63 6520 3d20 7074 2e7a 6572 6f73 2870  nce = pt.zeros(p
+0000a240: 742e 6174 6c65 6173 745f 3164 286e 2929  t.atleast_1d(n))
+0000a250: 0a20 2020 2076 6172 6961 6e63 6520 3d20  .    variance = 
+0000a260: 7074 2e69 6e63 5f73 7562 7465 6e73 6f72  pt.inc_subtensor
+0000a270: 2876 6172 6961 6e63 655b 305d 2c20 7661  (variance[0], va
+0000a280: 6c75 655b 305d 202a 2a20 3229 0a20 2020  lue[0] ** 2).   
+0000a290: 2076 6172 6961 6e63 6520 3d20 7074 2e69   variance = pt.i
+0000a2a0: 6e63 5f73 7562 7465 6e73 6f72 2876 6172  nc_subtensor(var
+0000a2b0: 6961 6e63 655b 313a 5d2c 2063 756d 7375  iance[1:], cumsu
+0000a2c0: 6d5b 6469 6167 5f69 6478 735b 313a 5d5d  m[diag_idxs[1:]]
+0000a2d0: 202d 2063 756d 7375 6d5b 6469 6167 5f69   - cumsum[diag_i
+0000a2e0: 6478 735b 3a2d 315d 5d29 0a20 2020 2073  dxs[:-1]]).    s
+0000a2f0: 645f 7661 6c73 203d 2070 742e 7371 7274  d_vals = pt.sqrt
+0000a300: 2876 6172 6961 6e63 6529 0a0a 2020 2020  (variance)..    
+0000a310: 6c6f 6770 5f73 6420 3d20 706d 2e6c 6f67  logp_sd = pm.log
+0000a320: 7028 7364 5f64 6973 742c 2073 645f 7661  p(sd_dist, sd_va
+0000a330: 6c73 292e 7375 6d28 290a 2020 2020 636f  ls).sum().    co
+0000a340: 7272 5f64 6961 6720 3d20 7661 6c75 655b  rr_diag = value[
+0000a350: 6469 6167 5f69 6478 735d 202f 2073 645f  diag_idxs] / sd_
+0000a360: 7661 6c73 0a0a 2020 2020 6c6f 6770 5f6c  vals..    logp_l
+0000a370: 6b6a 203d 2028 3220 2a20 6574 6120 2d20  kj = (2 * eta - 
+0000a380: 3320 2b20 6e20 2d20 7074 2e61 7261 6e67  3 + n - pt.arang
+0000a390: 6528 6e29 2920 2a20 7074 2e6c 6f67 2863  e(n)) * pt.log(c
+0000a3a0: 6f72 725f 6469 6167 290a 2020 2020 6c6f  orr_diag).    lo
+0000a3b0: 6770 5f6c 6b6a 203d 2070 742e 7375 6d28  gp_lkj = pt.sum(
+0000a3c0: 6c6f 6770 5f6c 6b6a 290a 0a20 2020 2023  logp_lkj)..    #
+0000a3d0: 2043 6f6d 7075 7465 2074 6865 206c 6f67   Compute the log
+0000a3e0: 2064 6574 206a 6163 6f62 6961 6e20 6f66   det jacobian of
+0000a3f0: 2074 6865 2073 6563 6f6e 6420 7472 616e   the second tran
+0000a400: 7366 6f72 6d61 7469 6f6e 0a20 2020 2023  sformation.    #
+0000a410: 2064 6573 6372 6962 6564 2069 6e20 7468   described in th
+0000a420: 6520 646f 6373 7472 696e 672e 0a20 2020  e docstring..   
+0000a430: 2069 6478 203d 2070 742e 6172 616e 6765   idx = pt.arange
+0000a440: 286e 290a 2020 2020 6465 745f 696e 766a  (n).    det_invj
+0000a450: 6163 203d 2070 742e 6c6f 6728 636f 7272  ac = pt.log(corr
+0000a460: 5f64 6961 6729 202d 2069 6478 202a 2070  _diag) - idx * p
+0000a470: 742e 6c6f 6728 7364 5f76 616c 7329 0a20  t.log(sd_vals). 
+0000a480: 2020 2064 6574 5f69 6e76 6a61 6320 3d20     det_invjac = 
+0000a490: 6465 745f 696e 766a 6163 2e73 756d 2829  det_invjac.sum()
+0000a4a0: 0a0a 2020 2020 2320 544f 444f 3a20 5f6c  ..    # TODO: _l
+0000a4b0: 6b6a 5f6e 6f72 6d61 6c69 7a69 6e67 5f63  kj_normalizing_c
+0000a4c0: 6f6e 7374 616e 7420 6375 7272 656e 746c  onstant currentl
+0000a4d0: 7920 7265 7175 6972 6573 2060 6574 6160  y requires `eta`
+0000a4e0: 2061 6e64 2060 6e60 2074 6f20 6265 2063   and `n` to be c
+0000a4f0: 6f6e 7374 616e 7473 0a20 2020 2069 6620  onstants.    if 
+0000a500: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
+0000a510: 2c20 436f 6e73 7461 6e74 293a 0a20 2020  , Constant):.   
+0000a520: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+0000a530: 706c 656d 656e 7465 6445 7272 6f72 2822  plementedError("
+0000a540: 6c6f 6770 206f 6e6c 7920 696d 706c 656d  logp only implem
+0000a550: 656e 7465 6420 666f 7220 636f 6e73 7461  ented for consta
+0000a560: 6e74 2060 6e60 2229 0a20 2020 206e 203d  nt `n`").    n =
+0000a570: 2069 6e74 286e 2e64 6174 6129 0a0a 2020   int(n.data)..  
+0000a580: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+0000a590: 6e63 6528 6574 612c 2043 6f6e 7374 616e  nce(eta, Constan
+0000a5a0: 7429 3a0a 2020 2020 2020 2020 7261 6973  t):.        rais
+0000a5b0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+0000a5c0: 4572 726f 7228 226c 6f67 7020 6f6e 6c79  Error("logp only
+0000a5d0: 2069 6d70 6c65 6d65 6e74 6564 2066 6f72   implemented for
+0000a5e0: 2063 6f6e 7374 616e 7420 6065 7461 6022   constant `eta`"
+0000a5f0: 290a 2020 2020 6574 6120 3d20 666c 6f61  ).    eta = floa
+0000a600: 7428 6574 612e 6461 7461 290a 0a20 2020  t(eta.data)..   
+0000a610: 206e 6f72 6d20 3d20 5f6c 6b6a 5f6e 6f72   norm = _lkj_nor
+0000a620: 6d61 6c69 7a69 6e67 5f63 6f6e 7374 616e  malizing_constan
+0000a630: 7428 6574 612c 206e 290a 0a20 2020 2072  t(eta, n)..    r
+0000a640: 6574 7572 6e20 6e6f 726d 202b 206c 6f67  eturn norm + log
+0000a650: 705f 6c6b 6a20 2b20 6c6f 6770 5f73 6420  p_lkj + logp_sd 
+0000a660: 2b20 6465 745f 696e 766a 6163 0a0a 0a63  + det_invjac...c
+0000a670: 6c61 7373 204c 4b4a 4368 6f6c 6573 6b79  lass LKJCholesky
+0000a680: 436f 763a 0a20 2020 2072 2222 2257 7261  Cov:.    r"""Wra
+0000a690: 7070 6572 2063 6c61 7373 2066 6f72 2063  pper class for c
+0000a6a0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000a6b0: 2077 6974 6820 4c4b 4a20 6469 7374 7269   with LKJ distri
+0000a6c0: 6275 7465 6420 636f 7272 656c 6174 696f  buted correlatio
+0000a6d0: 6e73 2e0a 0a20 2020 2054 6869 7320 6465  ns...    This de
+0000a6e0: 6669 6e65 7320 6120 6469 7374 7269 6275  fines a distribu
+0000a6f0: 7469 6f6e 206f 7665 7220 4368 6f6c 6573  tion over Choles
+0000a700: 6b79 2064 6563 6f6d 706f 7365 6420 636f  ky decomposed co
+0000a710: 7661 7269 616e 6365 0a20 2020 206d 6174  variance.    mat
+0000a720: 7269 6365 732c 2073 7563 6820 7468 6174  rices, such that
+0000a730: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
+0000a740: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
+0000a750: 6963 6573 2066 6f6c 6c6f 7720 616e 0a20  ices follow an. 
+0000a760: 2020 204c 4b4a 2064 6973 7472 6962 7574     LKJ distribut
+0000a770: 696f 6e20 5b31 5d20 616e 6420 7468 6520  ion [1] and the 
+0000a780: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+0000a790: 6f6e 7320 666f 6c6c 6f77 2061 6e20 6172  ons follow an ar
+0000a7a0: 6269 7472 6172 790a 2020 2020 6469 7374  bitrary.    dist
+0000a7b0: 7269 6275 7469 6f6e 2073 7065 6369 6669  ribution specifi
+0000a7c0: 6564 2062 7920 7468 6520 7573 6572 2e0a  ed by the user..
+0000a7d0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0000a7e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000a7f0: 2020 206e 616d 6520 3a20 7374 720a 2020     name : str.  
+0000a800: 2020 2020 2020 5468 6520 6e61 6d65 2067        The name g
+0000a810: 6976 656e 2074 6f20 7468 6520 7661 7269  iven to the vari
+0000a820: 6162 6c65 2069 6e20 7468 6520 6d6f 6465  able in the mode
+0000a830: 6c2e 0a20 2020 2065 7461 203a 2074 656e  l..    eta : ten
+0000a840: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
+0000a850: 740a 2020 2020 2020 2020 5468 6520 7368  t.        The sh
+0000a860: 6170 6520 7061 7261 6d65 7465 7220 2865  ape parameter (e
+0000a870: 7461 203e 2030 2920 6f66 2074 6865 204c  ta > 0) of the L
+0000a880: 4b4a 2064 6973 7472 6962 7574 696f 6e2e  KJ distribution.
+0000a890: 2065 7461 203d 2031 0a20 2020 2020 2020   eta = 1.       
+0000a8a0: 2069 6d70 6c69 6573 2061 2075 6e69 666f   implies a unifo
+0000a8b0: 726d 2064 6973 7472 6962 7574 696f 6e20  rm distribution 
+0000a8c0: 6f66 2074 6865 2063 6f72 7265 6c61 7469  of the correlati
+0000a8d0: 6f6e 206d 6174 7269 6365 733b 0a20 2020  on matrices;.   
+0000a8e0: 2020 2020 206c 6172 6765 7220 7661 6c75       larger valu
+0000a8f0: 6573 2070 7574 206d 6f72 6520 7765 6967  es put more weig
+0000a900: 6874 206f 6e20 6d61 7472 6963 6573 2077  ht on matrices w
+0000a910: 6974 6820 6665 7720 636f 7272 656c 6174  ith few correlat
+0000a920: 696f 6e73 2e0a 2020 2020 6e20 3a20 7465  ions..    n : te
+0000a930: 6e73 6f72 5f6c 696b 6520 6f66 2069 6e74  nsor_like of int
+0000a940: 0a20 2020 2020 2020 2044 696d 656e 7369  .        Dimensi
+0000a950: 6f6e 206f 6620 7468 6520 636f 7661 7269  on of the covari
+0000a960: 616e 6365 206d 6174 7269 7820 286e 203e  ance matrix (n >
+0000a970: 2031 292e 0a20 2020 2073 645f 6469 7374   1)..    sd_dist
+0000a980: 203a 2044 6973 7472 6962 7574 696f 6e0a   : Distribution.
+0000a990: 2020 2020 2020 2020 4120 706f 7369 7469          A positi
+0000a9a0: 7665 2073 6361 6c61 7220 6f72 2076 6563  ve scalar or vec
+0000a9b0: 746f 7220 6469 7374 7269 6275 7469 6f6e  tor distribution
+0000a9c0: 2066 6f72 2074 6865 2073 7461 6e64 6172   for the standar
+0000a9d0: 6420 6465 7669 6174 696f 6e73 2c20 6372  d deviations, cr
+0000a9e0: 6561 7465 640a 2020 2020 2020 2020 7769  eated.        wi
+0000a9f0: 7468 2074 6865 2060 2e64 6973 7428 2960  th the `.dist()`
+0000aa00: 2041 5049 2e20 5368 6f75 6c64 2068 6176   API. Should hav
+0000aa10: 6520 6073 6861 7065 5b2d 315d 3d6e 602e  e `shape[-1]=n`.
+0000aa20: 2053 6361 6c61 7220 6469 7374 7269 6275   Scalar distribu
+0000aa30: 7469 6f6e 7320 7769 6c6c 2062 650a 2020  tions will be.  
+0000aa40: 2020 2020 2020 6175 746f 6d61 7469 6361        automatica
+0000aa50: 6c6c 7920 7265 7369 7a65 6420 746f 2065  lly resized to e
+0000aa60: 6e73 7572 6520 7468 6973 2e0a 0a20 2020  nsure this...   
+0000aa70: 2020 2020 202e 2e20 7761 726e 696e 673a       .. warning:
+0000aa80: 3a20 7364 5f64 6973 7420 7769 6c6c 2062  : sd_dist will b
+0000aa90: 6520 636c 6f6e 6564 2c20 7265 6e64 6572  e cloned, render
+0000aaa0: 696e 6720 6974 2069 6e64 6570 656e 6465  ing it independe
+0000aab0: 6e74 206f 6620 7468 6520 6f6e 6520 7061  nt of the one pa
+0000aac0: 7373 6564 2061 7320 696e 7075 742e 0a0a  ssed as input...
+0000aad0: 2020 2020 636f 6d70 7574 655f 636f 7272      compute_corr
+0000aae0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0000aaf0: 3d54 7275 650a 2020 2020 2020 2020 4966  =True.        If
+0000ab00: 2060 5472 7565 602c 2072 6574 7572 6e73   `True`, returns
+0000ab10: 2074 6872 6565 2076 616c 7565 733a 2074   three values: t
+0000ab20: 6865 2043 686f 6c65 736b 7920 6465 636f  he Cholesky deco
+0000ab30: 6d70 6f73 6974 696f 6e2c 2074 6865 2063  mposition, the c
+0000ab40: 6f72 7265 6c61 7469 6f6e 730a 2020 2020  orrelations.    
+0000ab50: 2020 2020 616e 6420 7468 6520 7374 616e      and the stan
+0000ab60: 6461 7264 2064 6576 6961 7469 6f6e 7320  dard deviations 
+0000ab70: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
+0000ab80: 6520 6d61 7472 6978 2e20 4f74 6865 7277  e matrix. Otherw
+0000ab90: 6973 652c 206f 6e6c 7920 7265 7475 726e  ise, only return
+0000aba0: 730a 2020 2020 2020 2020 7468 6520 7061  s.        the pa
+0000abb0: 636b 6564 2043 686f 6c65 736b 7920 6465  cked Cholesky de
+0000abc0: 636f 6d70 6f73 6974 696f 6e2e 2044 6566  composition. Def
+0000abd0: 6175 6c74 7320 746f 2060 5472 7565 602e  aults to `True`.
+0000abe0: 0a20 2020 2020 2020 2063 6f6d 7061 7469  .        compati
+0000abf0: 6269 6c69 7479 2e0a 2020 2020 7374 6f72  bility..    stor
+0000ac00: 655f 696e 5f74 7261 6365 203a 2062 6f6f  e_in_trace : boo
+0000ac10: 6c2c 2064 6566 6175 6c74 3d54 7275 650a  l, default=True.
+0000ac20: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+0000ac30: 746f 2073 746f 7265 2074 6865 2063 6f72  to store the cor
+0000ac40: 7265 6c61 7469 6f6e 7320 616e 6420 7374  relations and st
+0000ac50: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+0000ac60: 7320 6f66 2074 6865 2063 6f76 6172 6961  s of the covaria
+0000ac70: 6e63 650a 2020 2020 2020 2020 6d61 7472  nce.        matr
+0000ac80: 6978 2069 6e20 7468 6520 706f 7374 6572  ix in the poster
+0000ac90: 696f 7220 7472 6163 652e 2049 6620 6054  ior trace. If `T
+0000aca0: 7275 6560 2c20 7468 6579 2077 696c 6c20  rue`, they will 
+0000acb0: 6175 746f 6d61 7469 6361 6c6c 7920 6265  automatically be
+0000acc0: 206e 616d 6564 2061 730a 2020 2020 2020   named as.      
+0000acd0: 2020 607b 6e61 6d65 7d5f 636f 7272 6020    `{name}_corr` 
+0000ace0: 616e 6420 607b 6e61 6d65 7d5f 7374 6473  and `{name}_stds
+0000acf0: 6020 7265 7370 6563 7469 7665 6c79 2e20  ` respectively. 
+0000ad00: 4566 6665 6374 6976 6520 6f6e 6c79 2077  Effective only w
+0000ad10: 6865 6e0a 2020 2020 2020 2020 6063 6f6d  hen.        `com
+0000ad20: 7075 7465 5f63 6f72 723d 5472 7565 602e  pute_corr=True`.
+0000ad30: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+0000ad40: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6368    -------.    ch
+0000ad50: 6f6c 203a 2020 5465 6e73 6f72 5661 7269  ol :  TensorVari
+0000ad60: 6162 6c65 0a20 2020 2020 2020 2049 6620  able.        If 
+0000ad70: 6063 6f6d 7075 7465 5f63 6f72 723d 5472  `compute_corr=Tr
+0000ad80: 7565 602e 2054 6865 2075 6e70 6163 6b65  ue`. The unpacke
+0000ad90: 6420 4368 6f6c 6573 6b79 2063 6f76 6172  d Cholesky covar
+0000ada0: 6961 6e63 6520 6465 636f 6d70 6f73 6974  iance decomposit
+0000adb0: 696f 6e2e 0a20 2020 2063 6f72 7220 3a20  ion..    corr : 
+0000adc0: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
+0000add0: 2020 2020 2020 2049 6620 6063 6f6d 7075         If `compu
+0000ade0: 7465 5f63 6f72 723d 5472 7565 602e 2054  te_corr=True`. T
+0000adf0: 6865 2063 6f72 7265 6c61 7469 6f6e 7320  he correlations 
+0000ae00: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
+0000ae10: 6520 6d61 7472 6978 2e0a 2020 2020 7374  e matrix..    st
+0000ae20: 6473 203a 2054 656e 736f 7256 6172 6961  ds : TensorVaria
+0000ae30: 626c 650a 2020 2020 2020 2020 4966 2060  ble.        If `
+0000ae40: 636f 6d70 7574 655f 636f 7272 3d54 7275  compute_corr=Tru
+0000ae50: 6560 2e20 5468 6520 7374 616e 6461 7264  e`. The standard
+0000ae60: 2064 6576 6961 7469 6f6e 7320 6f66 2074   deviations of t
+0000ae70: 6865 2063 6f76 6172 6961 6e63 6520 6d61  he covariance ma
+0000ae80: 7472 6978 2e0a 2020 2020 7061 636b 6564  trix..    packed
+0000ae90: 5f63 686f 6c20 3a20 5465 6e73 6f72 5661  _chol : TensorVa
+0000aea0: 7269 6162 6c65 0a20 2020 2020 2020 2049  riable.        I
+0000aeb0: 6620 6063 6f6d 7075 7465 5f63 6f72 723d  f `compute_corr=
+0000aec0: 4661 6c73 6560 2054 6865 2070 6163 6b65  False` The packe
+0000aed0: 6420 4368 6f6c 6573 6b79 2063 6f76 6172  d Cholesky covar
+0000aee0: 6961 6e63 6520 6465 636f 6d70 6f73 6974  iance decomposit
+0000aef0: 696f 6e2e 0a0a 2020 2020 4e6f 7465 730a  ion...    Notes.
+0000af00: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5369      -----.    Si
+0000af10: 6e63 6520 7468 6520 4368 6f6c 6573 6b79  nce the Cholesky
+0000af20: 2066 6163 746f 7220 6973 2061 206c 6f77   factor is a low
+0000af30: 6572 2074 7269 616e 6775 6c61 7220 6d61  er triangular ma
+0000af40: 7472 6978 2c20 7765 2075 7365 2070 6163  trix, we use pac
+0000af50: 6b65 6420 7374 6f72 6167 6520 666f 720a  ked storage for.
+0000af60: 2020 2020 7468 6520 6d61 7472 6978 3a20      the matrix: 
+0000af70: 5765 2073 746f 7265 2074 6865 2076 616c  We store the val
+0000af80: 7565 7320 6f66 2074 6865 206c 6f77 6572  ues of the lower
+0000af90: 2074 7269 616e 6775 6c61 7220 6d61 7472   triangular matr
+0000afa0: 6978 2069 6e20 6120 6f6e 652d 6469 6d65  ix in a one-dime
+0000afb0: 6e73 696f 6e61 6c0a 2020 2020 6172 7261  nsional.    arra
+0000afc0: 792c 206e 756d 6265 7265 6420 6279 2072  y, numbered by r
+0000afd0: 6f77 3a3a 0a0a 2020 2020 2020 2020 5b5b  ow::..        [[
+0000afe0: 3020 2d20 2d20 2d5d 0a20 2020 2020 2020  0 - - -].       
+0000aff0: 2020 5b31 2032 202d 202d 5d0a 2020 2020    [1 2 - -].    
+0000b000: 2020 2020 205b 3320 3420 3520 2d5d 0a20       [3 4 5 -]. 
+0000b010: 2020 2020 2020 2020 5b36 2037 2038 2039          [6 7 8 9
+0000b020: 5d5d 0a0a 2020 2020 5468 6520 756e 7061  ]]..    The unpa
+0000b030: 636b 6564 2043 686f 6c65 736b 7920 636f  cked Cholesky co
+0000b040: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+0000b050: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+0000b060: 2063 6f6d 7075 7465 6420 616e 6420 7265   computed and re
+0000b070: 7475 726e 6564 2077 6865 6e0a 2020 2020  turned when.    
+0000b080: 796f 7520 7370 6563 6966 7920 6063 6f6d  you specify `com
+0000b090: 7075 7465 5f63 6f72 723d 5472 7565 6020  pute_corr=True` 
+0000b0a0: 696e 2060 706d 2e4c 4b4a 4368 6f6c 6573  in `pm.LKJCholes
+0000b0b0: 6b79 436f 7660 2028 7365 6520 6578 616d  kyCov` (see exam
+0000b0c0: 706c 6520 6265 6c6f 7729 2e0a 2020 2020  ple below)..    
+0000b0d0: 4f74 6865 7277 6973 652c 2079 6f75 2063  Otherwise, you c
+0000b0e0: 616e 2075 7365 2060 706d 2e65 7870 616e  an use `pm.expan
+0000b0f0: 645f 7061 636b 6564 5f74 7269 616e 6775  d_packed_triangu
+0000b100: 6c61 7228 7061 636b 6564 5f63 6f76 2c20  lar(packed_cov, 
+0000b110: 6c6f 7765 723d 5472 7565 2960 0a20 2020  lower=True)`.   
+0000b120: 2074 6f20 636f 6e76 6572 7420 7468 6520   to convert the 
+0000b130: 7061 636b 6564 2043 686f 6c65 736b 7920  packed Cholesky 
+0000b140: 6d61 7472 6978 2074 6f20 6120 7265 6775  matrix to a regu
+0000b150: 6c61 7220 7477 6f2d 6469 6d65 6e73 696f  lar two-dimensio
+0000b160: 6e61 6c20 6172 7261 792e 0a0a 2020 2020  nal array...    
+0000b170: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
+0000b180: 2d2d 2d2d 2d0a 2020 2020 2e2e 2063 6f64  -----.    .. cod
+0000b190: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+0000b1a0: 2020 2020 7769 7468 2070 6d2e 4d6f 6465      with pm.Mode
+0000b1b0: 6c28 2920 6173 206d 6f64 656c 3a0a 2020  l() as model:.  
+0000b1c0: 2020 2020 2020 2020 2020 2320 4e6f 7465            # Note
+0000b1d0: 2074 6861 7420 7765 2061 6363 6573 7320   that we access 
+0000b1e0: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
+0000b1f0: 2066 6f72 2074 6865 2073 7461 6e64 6172   for the standar
+0000b200: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
+0000b210: 6465 7669 6174 696f 6e73 2c20 616e 6420  deviations, and 
+0000b220: 646f 206e 6f74 2063 7265 6174 6520 6120  do not create a 
+0000b230: 6e65 7720 7261 6e64 6f6d 2076 6172 6961  new random varia
+0000b240: 626c 652e 0a20 2020 2020 2020 2020 2020  ble..           
+0000b250: 2073 645f 6469 7374 203d 2070 6d2e 4578   sd_dist = pm.Ex
+0000b260: 706f 6e65 6e74 6961 6c2e 6469 7374 2831  ponential.dist(1
+0000b270: 2e30 2c20 7369 7a65 3d31 3029 0a20 2020  .0, size=10).   
+0000b280: 2020 2020 2020 2020 2063 686f 6c2c 2063           chol, c
+0000b290: 6f72 722c 2073 6967 6d61 7320 3d20 706d  orr, sigmas = pm
+0000b2a0: 2e4c 4b4a 4368 6f6c 6573 6b79 436f 7628  .LKJCholeskyCov(
+0000b2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b2c0: 2027 6368 6f6c 5f63 6f76 272c 2065 7461   'chol_cov', eta
+0000b2d0: 3d34 2c20 6e3d 3130 2c20 7364 5f64 6973  =4, n=10, sd_dis
+0000b2e0: 743d 7364 5f64 6973 740a 2020 2020 2020  t=sd_dist.      
+0000b2f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000b300: 2020 2020 2023 2069 6620 796f 7520 6f6e       # if you on
+0000b310: 6c79 2077 616e 7420 7468 6520 7061 636b  ly want the pack
+0000b320: 6564 2043 686f 6c65 736b 793a 0a20 2020  ed Cholesky:.   
+0000b330: 2020 2020 2020 2020 2023 2070 6163 6b65           # packe
+0000b340: 645f 6368 6f6c 203d 2070 6d2e 4c4b 4a43  d_chol = pm.LKJC
+0000b350: 686f 6c65 736b 7943 6f76 280a 2020 2020  holeskyCov(.    
+0000b360: 2020 2020 2020 2020 2020 2020 2763 686f              'cho
+0000b370: 6c5f 636f 7627 2c20 6574 613d 342c 206e  l_cov', eta=4, n
+0000b380: 3d31 302c 2073 645f 6469 7374 3d73 645f  =10, sd_dist=sd_
+0000b390: 6469 7374 2c20 636f 6d70 7574 655f 636f  dist, compute_co
+0000b3a0: 7272 3d46 616c 7365 0a20 2020 2020 2020  rr=False.       
+0000b3b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000b3c0: 2020 2023 2063 686f 6c20 3d20 706d 2e65     # chol = pm.e
+0000b3d0: 7870 616e 645f 7061 636b 6564 5f74 7269  xpand_packed_tri
+0000b3e0: 616e 6775 6c61 7228 3130 2c20 7061 636b  angular(10, pack
+0000b3f0: 6564 5f63 686f 6c2c 206c 6f77 6572 3d54  ed_chol, lower=T
+0000b400: 7275 6529 0a0a 2020 2020 2020 2020 2020  rue)..          
+0000b410: 2020 2320 4465 6669 6e65 2061 206e 6577    # Define a new
+0000b420: 204d 764e 6f72 6d61 6c20 7769 7468 2074   MvNormal with t
+0000b430: 6865 2067 6976 656e 2063 6f76 6172 6961  he given covaria
+0000b440: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+0000b450: 7661 6c73 203d 2070 6d2e 4d76 4e6f 726d  vals = pm.MvNorm
+0000b460: 616c 2827 7661 6c73 272c 206d 753d 6e70  al('vals', mu=np
+0000b470: 2e7a 6572 6f73 2831 3029 2c20 6368 6f6c  .zeros(10), chol
+0000b480: 3d63 686f 6c2c 2073 6861 7065 3d31 3029  =chol, shape=10)
+0000b490: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000b4a0: 4f72 2074 7261 6e73 666f 726d 2061 6e20  Or transform an 
+0000b4b0: 756e 636f 7272 656c 6174 6564 206e 6f72  uncorrelated nor
+0000b4c0: 6d61 6c3a 0a20 2020 2020 2020 2020 2020  mal:.           
+0000b4d0: 2076 616c 735f 7261 7720 3d20 706d 2e4e   vals_raw = pm.N
+0000b4e0: 6f72 6d61 6c28 2776 616c 735f 7261 7727  ormal('vals_raw'
+0000b4f0: 2c20 6d75 3d30 2c20 7369 676d 613d 312c  , mu=0, sigma=1,
+0000b500: 2073 6861 7065 3d31 3029 0a20 2020 2020   shape=10).     
+0000b510: 2020 2020 2020 2076 616c 7320 3d20 7074         vals = pt
+0000b520: 2e64 6f74 2863 686f 6c2c 2076 616c 735f  .dot(chol, vals_
+0000b530: 7261 7729 0a0a 2020 2020 2020 2020 2020  raw)..          
+0000b540: 2020 2320 4f72 2063 6f6d 7075 7465 2074    # Or compute t
+0000b550: 6865 2063 6f76 6172 6961 6e63 6520 6d61  he covariance ma
+0000b560: 7472 6978 0a20 2020 2020 2020 2020 2020  trix.           
+0000b570: 2063 6f76 203d 2070 742e 646f 7428 6368   cov = pt.dot(ch
+0000b580: 6f6c 2c20 6368 6f6c 2e54 290a 0a20 2020  ol, chol.T)..   
+0000b590: 202a 2a49 6d70 6c65 6d65 6e74 6174 696f   **Implementatio
+0000b5a0: 6e2a 2a20 496e 2074 6865 2075 6e63 6f6e  n** In the uncon
+0000b5b0: 7374 7261 696e 6564 2073 7061 6365 2061  strained space a
+0000b5c0: 6c6c 2076 616c 7565 7320 6f66 2074 6865  ll values of the
+0000b5d0: 2063 686f 6c65 736b 7920 6661 6374 6f72   cholesky factor
+0000b5e0: 0a20 2020 2061 7265 2073 746f 7265 6420  .    are stored 
+0000b5f0: 756e 7472 616e 7366 6f72 6d65 642c 2065  untransformed, e
+0000b600: 7863 6570 7420 666f 7220 7468 6520 6469  xcept for the di
+0000b610: 6167 6f6e 616c 2065 6e74 7269 6573 2c20  agonal entries, 
+0000b620: 7768 6572 650a 2020 2020 7765 2075 7365  where.    we use
+0000b630: 2061 206c 6f67 2d74 7261 6e73 666f 726d   a log-transform
+0000b640: 2074 6f20 7265 7374 7269 6374 2074 6865   to restrict the
+0000b650: 6d20 746f 2070 6f73 6974 6976 6520 7661  m to positive va
+0000b660: 6c75 6573 2e0a 0a20 2020 2054 6f20 636f  lues...    To co
+0000b670: 7272 6563 746c 7920 636f 6d70 7574 6520  rrectly compute 
+0000b680: 6c6f 672d 6c69 6b65 6c69 686f 6f64 7320  log-likelihoods 
+0000b690: 666f 7220 7468 6520 7374 616e 6461 7264  for the standard
+0000b6a0: 2064 6576 6961 7469 6f6e 730a 2020 2020   deviations.    
+0000b6b0: 616e 6420 7468 6520 636f 7272 656c 6174  and the correlat
+0000b6c0: 696f 6e20 6d61 7472 6978 2073 6570 6172  ion matrix separ
+0000b6d0: 6174 656c 792c 2077 6520 6e65 6564 2074  ately, we need t
+0000b6e0: 6f20 636f 6e73 6964 6572 2061 0a20 2020  o consider a.   
+0000b6f0: 2073 6563 6f6e 6420 7472 616e 7366 6f72   second transfor
+0000b700: 6d61 7469 6f6e 3a20 4769 7665 6e20 6120  mation: Given a 
+0000b710: 6368 6f6c 6573 6b79 2066 6163 746f 7269  cholesky factori
+0000b720: 7a61 7469 6f6e 0a20 2020 203a 6d61 7468  zation.    :math
+0000b730: 3a60 4c4c 5e54 203d 205c 5369 676d 6160  :`LL^T = \Sigma`
+0000b740: 206f 6620 6120 636f 7661 7269 616e 6365   of a covariance
+0000b750: 206d 6174 7269 7820 7765 2063 616e 2072   matrix we can r
+0000b760: 6563 6f76 6572 2074 6865 0a20 2020 2073  ecover the.    s
+0000b770: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
+0000b780: 6e73 203a 6d61 7468 3a60 5c73 6967 6d61  ns :math:`\sigma
+0000b790: 6020 6173 2074 6865 2065 7563 6c69 6465  ` as the euclide
+0000b7a0: 616e 206c 656e 6774 6873 206f 660a 2020  an lengths of.  
+0000b7b0: 2020 7468 6520 726f 7773 206f 6620 3a6d    the rows of :m
+0000b7c0: 6174 683a 604c 602c 2061 6e64 2074 6865  ath:`L`, and the
+0000b7d0: 2063 686f 6c65 736b 7920 6661 6374 6f72   cholesky factor
+0000b7e0: 206f 6620 7468 650a 2020 2020 636f 7272   of the.    corr
+0000b7f0: 656c 6174 696f 6e20 6d61 7472 6978 2061  elation matrix a
+0000b800: 7320 3a6d 6174 683a 6055 203d 205c 7465  s :math:`U = \te
+0000b810: 7874 7b64 6961 677d 285c 7369 676d 6129  xt{diag}(\sigma)
+0000b820: 5e7b 2d31 7d4c 602e 0a20 2020 2053 696e  ^{-1}L`..    Sin
+0000b830: 6365 2065 6163 6820 726f 7720 6f66 203a  ce each row of :
+0000b840: 6d61 7468 3a60 5560 2068 6173 206c 656e  math:`U` has len
+0000b850: 6774 6820 312c 2077 6520 646f 206e 6f74  gth 1, we do not
+0000b860: 206e 6565 6420 746f 0a20 2020 2073 746f   need to.    sto
+0000b870: 7265 2074 6865 2064 6961 676f 6e61 6c2e  re the diagonal.
+0000b880: 2057 6520 6465 6669 6e65 2061 2074 7261   We define a tra
+0000b890: 6e73 666f 726d 6174 696f 6e20 3a6d 6174  nsformation :mat
+0000b8a0: 683a 605c 7068 6960 0a20 2020 2073 7563  h:`\phi`.    suc
+0000b8b0: 6820 7468 6174 203a 6d61 7468 3a60 5c70  h that :math:`\p
+0000b8c0: 6869 284c 2960 2069 7320 7468 6520 6c6f  hi(L)` is the lo
+0000b8d0: 7765 7220 7472 6961 6e67 756c 6172 206d  wer triangular m
+0000b8e0: 6174 7269 7820 636f 6e74 6169 6e69 6e67  atrix containing
+0000b8f0: 0a20 2020 2074 6865 2073 7461 6e64 6172  .    the standar
+0000b900: 6420 6465 7669 6174 696f 6e73 203a 6d61  d deviations :ma
+0000b910: 7468 3a60 5c73 6967 6d61 6020 6f6e 2074  th:`\sigma` on t
+0000b920: 6865 2064 6961 676f 6e61 6c20 616e 6420  he diagonal and 
+0000b930: 7468 650a 2020 2020 636f 7272 656c 6174  the.    correlat
+0000b940: 696f 6e20 6d61 7472 6978 203a 6d61 7468  ion matrix :math
+0000b950: 3a60 5560 2062 656c 6f77 2e20 496e 2074  :`U` below. In t
+0000b960: 6869 7320 666f 726d 2077 6520 6361 6e20  his form we can 
+0000b970: 6561 7369 6c79 0a20 2020 2063 6f6d 7075  easily.    compu
+0000b980: 7465 2074 6865 2064 6966 6665 7265 6e74  te the different
+0000b990: 206c 696b 656c 6968 6f6f 6473 2073 6570   likelihoods sep
+0000b9a0: 6172 6174 656c 792c 2061 7320 7468 6520  arately, as the 
+0000b9b0: 6c69 6b65 6c69 686f 6f64 0a20 2020 206f  likelihood.    o
+0000b9c0: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
+0000b9d0: 6e20 6d61 7472 6978 206f 6e6c 7920 6465  n matrix only de
+0000b9e0: 7065 6e64 7320 6f6e 2074 6865 2076 616c  pends on the val
+0000b9f0: 7565 7320 6265 6c6f 7720 7468 650a 2020  ues below the.  
+0000ba00: 2020 6469 6167 6f6e 616c 2c20 616e 6420    diagonal, and 
+0000ba10: 7468 6520 6c69 6b65 6c69 686f 6f64 206f  the likelihood o
+0000ba20: 6620 7468 6520 7374 616e 6461 7264 2064  f the standard d
+0000ba30: 6576 6961 7469 6f6e 2064 6570 656e 6473  eviation depends
+0000ba40: 0a20 2020 206f 6e6c 7920 6f6e 2074 6865  .    only on the
+0000ba50: 2064 6961 676f 6e61 6c20 7661 6c75 6573   diagonal values
+0000ba60: 2e0a 0a20 2020 2057 6520 7374 696c 6c20  ...    We still 
+0000ba70: 6e65 6564 2074 6865 2064 6574 6572 6d69  need the determi
+0000ba80: 6e61 6e74 206f 6620 7468 6520 6a61 636f  nant of the jaco
+0000ba90: 6269 616e 206f 6620 3a6d 6174 683a 605c  bian of :math:`\
+0000baa0: 7068 695e 7b2d 317d 602e 0a20 2020 2049  phi^{-1}`..    I
+0000bab0: 6620 7765 2074 6869 6e6b 206f 6620 3a6d  f we think of :m
+0000bac0: 6174 683a 605c 7068 6960 2061 7320 616e  ath:`\phi` as an
+0000bad0: 2061 7574 6f6d 6f72 7068 6973 6d20 6f6e   automorphism on
+0000bae0: 0a20 2020 203a 6d61 7468 3a60 5c6d 6174  .    :math:`\mat
+0000baf0: 6862 627b 527d 5e7b 5c74 6672 6163 7b6e  hbb{R}^{\tfrac{n
+0000bb00: 286e 2b31 297d 7b32 7d7d 602c 2077 6865  (n+1)}{2}}`, whe
+0000bb10: 7265 2077 6520 6f72 6465 720a 2020 2020  re we order.    
+0000bb20: 7468 6520 6469 6d65 6e73 696f 6e73 2061  the dimensions a
+0000bb30: 7320 6465 7363 7269 6265 6420 696e 2074  s described in t
+0000bb40: 6865 206e 6f74 6573 2061 626f 7665 2c20  he notes above, 
+0000bb50: 7468 6520 6a61 636f 6269 616e 0a20 2020  the jacobian.   
+0000bb60: 2069 7320 6120 626c 6f63 6b2d 6469 6167   is a block-diag
+0000bb70: 6f6e 616c 206d 6174 7269 782c 2077 6865  onal matrix, whe
+0000bb80: 7265 2065 6163 6820 626c 6f63 6b20 636f  re each block co
+0000bb90: 7272 6573 706f 6e64 7320 746f 0a20 2020  rresponds to.   
+0000bba0: 206f 6e65 2072 6f77 206f 6620 3a6d 6174   one row of :mat
+0000bbb0: 683a 6055 602e 2045 6163 6820 626c 6f63  h:`U`. Each bloc
+0000bbc0: 6b20 6861 7320 6172 726f 7768 6561 6420  k has arrowhead 
+0000bbd0: 7368 6170 652c 2061 6e64 2077 650a 2020  shape, and we.  
+0000bbe0: 2020 6361 6e20 636f 6d70 7574 6520 7468    can compute th
+0000bbf0: 6520 6465 7465 726d 696e 616e 7420 6f66  e determinant of
+0000bc00: 2074 6861 7420 6173 2064 6573 6372 6962   that as describ
+0000bc10: 6564 2069 6e20 5b32 5d2e 2053 696e 6365  ed in [2]. Since
+0000bc20: 0a20 2020 2074 6865 2064 6574 6572 6d69  .    the determi
+0000bc30: 6e61 6e74 206f 6620 6120 626c 6f63 6b2d  nant of a block-
+0000bc40: 6469 6167 6f6e 616c 206d 6174 7269 7820  diagonal matrix 
+0000bc50: 6973 2074 6865 2070 726f 6475 6374 0a20  is the product. 
+0000bc60: 2020 206f 6620 7468 6520 6465 7465 726d     of the determ
+0000bc70: 696e 616e 7473 206f 6620 7468 6520 626c  inants of the bl
+0000bc80: 6f63 6b73 2c20 7765 2067 6574 0a0a 2020  ocks, we get..  
+0000bc90: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
+0000bca0: 2020 2020 5c74 6578 747b 6465 747d 284a      \text{det}(J
+0000bcb0: 5f7b 5c70 6869 5e7b 2d31 7d7d 2855 2929  _{\phi^{-1}}(U))
+0000bcc0: 203d 0a20 2020 2020 2020 5c6c 6566 745b   =.       \left[
+0000bcd0: 0a20 2020 2020 2020 2020 5c70 726f 645f  .         \prod_
+0000bce0: 7b69 3d32 7d5e 4e20 755f 7b69 697d 5e7b  {i=2}^N u_{ii}^{
+0000bcf0: 6920 2d20 317d 204c 5f7b 6969 7d0a 2020  i - 1} L_{ii}.  
+0000bd00: 2020 2020 205c 7269 6768 745d 5e7b 2d31       \right]^{-1
+0000bd10: 7d0a 0a20 2020 2052 6566 6572 656e 6365  }..    Reference
+0000bd20: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0000bd30: 0a20 2020 202e 2e20 5b31 5d20 4c65 7761  .    .. [1] Lewa
+0000bd40: 6e64 6f77 736b 692c 2044 2e2c 204b 7572  ndowski, D., Kur
+0000bd50: 6f77 6963 6b61 2c20 442e 2061 6e64 204a  owicka, D. and J
+0000bd60: 6f65 2c20 482e 2028 3230 3039 292e 0a20  oe, H. (2009).. 
+0000bd70: 2020 2020 2020 2247 656e 6572 6174 696e        "Generatin
+0000bd80: 6720 7261 6e64 6f6d 2063 6f72 7265 6c61  g random correla
+0000bd90: 7469 6f6e 206d 6174 7269 6365 7320 6261  tion matrices ba
+0000bda0: 7365 6420 6f6e 2076 696e 6573 2061 6e64  sed on vines and
+0000bdb0: 0a20 2020 2020 2020 6578 7465 6e64 6564  .       extended
+0000bdc0: 206f 6e69 6f6e 206d 6574 686f 642e 2220   onion method." 
+0000bdd0: 4a6f 7572 6e61 6c20 6f66 206d 756c 7469  Journal of multi
+0000bde0: 7661 7269 6174 6520 616e 616c 7973 6973  variate analysis
+0000bdf0: 2c0a 2020 2020 2020 2031 3030 2839 292c  ,.       100(9),
+0000be00: 2070 702e 3139 3839 2d32 3030 312e 0a0a   pp.1989-2001...
+0000be10: 2020 2020 2e2e 205b 325d 204a 2e20 4d2e      .. [2] J. M.
+0000be20: 2069 736e 2774 2061 206d 6174 6865 6d61   isn't a mathema
+0000be30: 7469 6369 616e 2028 6874 7470 3a2f 2f6d  tician (http://m
+0000be40: 6174 682e 7374 6163 6b65 7863 6861 6e67  ath.stackexchang
+0000be50: 652e 636f 6d2f 7573 6572 732f 3439 382f  e.com/users/498/
+0000be60: 0a20 2020 2020 2020 6a2d 6d2d 6973 6e74  .       j-m-isnt
+0000be70: 2d61 2d6d 6174 6865 6d61 7469 6369 616e  -a-mathematician
+0000be80: 292c 2044 6966 6665 7265 6e74 2061 7070  ), Different app
+0000be90: 726f 6163 6865 7320 746f 2065 7661 6c75  roaches to evalu
+0000bea0: 6174 6520 7468 6973 0a20 2020 2020 2020  ate this.       
+0000beb0: 6465 7465 726d 696e 616e 742c 2055 524c  determinant, URL
+0000bec0: 2028 7665 7273 696f 6e3a 2032 3031 322d   (version: 2012-
+0000bed0: 3034 2d31 3429 3a0a 2020 2020 2020 2068  04-14):.       h
+0000bee0: 7474 703a 2f2f 6d61 7468 2e73 7461 636b  ttp://math.stack
+0000bef0: 6578 6368 616e 6765 2e63 6f6d 2f71 2f31  exchange.com/q/1
+0000bf00: 3330 3032 360a 2020 2020 2222 220a 0a20  30026.    """.. 
+0000bf10: 2020 2064 6566 205f 5f6e 6577 5f5f 2863     def __new__(c
+0000bf20: 6c73 2c20 6e61 6d65 2c20 6574 612c 206e  ls, name, eta, n
+0000bf30: 2c20 7364 5f64 6973 742c 202a 2c20 636f  , sd_dist, *, co
+0000bf40: 6d70 7574 655f 636f 7272 3d54 7275 652c  mpute_corr=True,
+0000bf50: 2073 746f 7265 5f69 6e5f 7472 6163 653d   store_in_trace=
+0000bf60: 5472 7565 2c20 2a2a 6b77 6172 6773 293a  True, **kwargs):
+0000bf70: 0a20 2020 2020 2020 2070 6163 6b65 645f  .        packed_
+0000bf80: 6368 6f6c 203d 205f 4c4b 4a43 686f 6c65  chol = _LKJChole
+0000bf90: 736b 7943 6f76 286e 616d 652c 2065 7461  skyCov(name, eta
+0000bfa0: 3d65 7461 2c20 6e3d 6e2c 2073 645f 6469  =eta, n=n, sd_di
+0000bfb0: 7374 3d73 645f 6469 7374 2c20 2a2a 6b77  st=sd_dist, **kw
+0000bfc0: 6172 6773 290a 2020 2020 2020 2020 6966  args).        if
+0000bfd0: 206e 6f74 2063 6f6d 7075 7465 5f63 6f72   not compute_cor
+0000bfe0: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+0000bff0: 6574 7572 6e20 7061 636b 6564 5f63 686f  eturn packed_cho
+0000c000: 6c0a 2020 2020 2020 2020 656c 7365 3a0a  l.        else:.
+0000c010: 2020 2020 2020 2020 2020 2020 6368 6f6c              chol
+0000c020: 2c20 636f 7272 2c20 7374 6473 203d 2063  , corr, stds = c
+0000c030: 6c73 2e68 656c 7065 725f 6465 7465 726d  ls.helper_determ
+0000c040: 696e 6973 7469 6373 286e 2c20 7061 636b  inistics(n, pack
+0000c050: 6564 5f63 686f 6c29 0a20 2020 2020 2020  ed_chol).       
+0000c060: 2020 2020 2069 6620 7374 6f72 655f 696e       if store_in
+0000c070: 5f74 7261 6365 3a0a 2020 2020 2020 2020  _trace:.        
+0000c080: 2020 2020 2020 2020 636f 7272 203d 2070          corr = p
+0000c090: 6d2e 4465 7465 726d 696e 6973 7469 6328  m.Deterministic(
+0000c0a0: 6622 7b6e 616d 657d 5f63 6f72 7222 2c20  f"{name}_corr", 
+0000c0b0: 636f 7272 290a 2020 2020 2020 2020 2020  corr).          
+0000c0c0: 2020 2020 2020 7374 6473 203d 2070 6d2e        stds = pm.
+0000c0d0: 4465 7465 726d 696e 6973 7469 6328 6622  Deterministic(f"
+0000c0e0: 7b6e 616d 657d 5f73 7464 7322 2c20 7374  {name}_stds", st
+0000c0f0: 6473 290a 2020 2020 2020 2020 2020 2020  ds).            
+0000c100: 7265 7475 726e 2063 686f 6c2c 2063 6f72  return chol, cor
+0000c110: 722c 2073 7464 730a 0a20 2020 2040 636c  r, stds..    @cl
+0000c120: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+0000c130: 6620 6469 7374 2863 6c73 2c20 6574 612c  f dist(cls, eta,
+0000c140: 206e 2c20 7364 5f64 6973 742c 202a 2c20   n, sd_dist, *, 
+0000c150: 636f 6d70 7574 655f 636f 7272 3d54 7275  compute_corr=Tru
+0000c160: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
+0000c170: 2020 2020 2020 2320 636f 6d70 7574 6520        # compute 
+0000c180: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
+0000c190: 7369 7469 6f6e 0a20 2020 2020 2020 2070  sition.        p
+0000c1a0: 6163 6b65 645f 6368 6f6c 203d 205f 4c4b  acked_chol = _LK
+0000c1b0: 4a43 686f 6c65 736b 7943 6f76 2e64 6973  JCholeskyCov.dis
+0000c1c0: 7428 6574 613d 6574 612c 206e 3d6e 2c20  t(eta=eta, n=n, 
+0000c1d0: 7364 5f64 6973 743d 7364 5f64 6973 742c  sd_dist=sd_dist,
+0000c1e0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000c1f0: 2020 2069 6620 6e6f 7420 636f 6d70 7574     if not comput
+0000c200: 655f 636f 7272 3a0a 2020 2020 2020 2020  e_corr:.        
+0000c210: 2020 2020 7265 7475 726e 2070 6163 6b65      return packe
+0000c220: 645f 6368 6f6c 0a20 2020 2020 2020 2065  d_chol.        e
+0000c230: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000c240: 2072 6574 7572 6e20 636c 732e 6865 6c70   return cls.help
+0000c250: 6572 5f64 6574 6572 6d69 6e69 7374 6963  er_deterministic
+0000c260: 7328 6e2c 2070 6163 6b65 645f 6368 6f6c  s(n, packed_chol
+0000c270: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+0000c280: 686f 640a 2020 2020 6465 6620 6865 6c70  hod.    def help
+0000c290: 6572 5f64 6574 6572 6d69 6e69 7374 6963  er_deterministic
+0000c2a0: 7328 636c 732c 206e 2c20 7061 636b 6564  s(cls, n, packed
+0000c2b0: 5f63 686f 6c29 3a0a 2020 2020 2020 2020  _chol):.        
+0000c2c0: 6368 6f6c 203d 2070 6d2e 6578 7061 6e64  chol = pm.expand
+0000c2d0: 5f70 6163 6b65 645f 7472 6961 6e67 756c  _packed_triangul
+0000c2e0: 6172 286e 2c20 7061 636b 6564 5f63 686f  ar(n, packed_cho
+0000c2f0: 6c2c 206c 6f77 6572 3d54 7275 6529 0a20  l, lower=True). 
+0000c300: 2020 2020 2020 2023 2063 6f6d 7075 7465         # compute
+0000c310: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
+0000c320: 6978 0a20 2020 2020 2020 2063 6f76 203d  ix.        cov =
+0000c330: 2070 742e 646f 7428 6368 6f6c 2c20 6368   pt.dot(chol, ch
+0000c340: 6f6c 2e54 290a 2020 2020 2020 2020 2320  ol.T).        # 
+0000c350: 6578 7472 6163 7420 7374 616e 6461 7264  extract standard
+0000c360: 2064 6576 6961 7469 6f6e 7320 616e 6420   deviations and 
+0000c370: 7268 6f0a 2020 2020 2020 2020 7374 6473  rho.        stds
+0000c380: 203d 2070 742e 7371 7274 2870 742e 6469   = pt.sqrt(pt.di
+0000c390: 6167 2863 6f76 2929 0a20 2020 2020 2020  ag(cov)).       
+0000c3a0: 2069 6e76 5f73 7464 7320 3d20 3120 2f20   inv_stds = 1 / 
+0000c3b0: 7374 6473 0a20 2020 2020 2020 2063 6f72  stds.        cor
+0000c3c0: 7220 3d20 696e 765f 7374 6473 5b4e 6f6e  r = inv_stds[Non
+0000c3d0: 652c 203a 5d20 2a20 636f 7620 2a20 696e  e, :] * cov * in
+0000c3e0: 765f 7374 6473 5b3a 2c20 4e6f 6e65 5d0a  v_stds[:, None].
+0000c3f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000c400: 686f 6c2c 2063 6f72 722c 2073 7464 730a  hol, corr, stds.
+0000c410: 0a0a 636c 6173 7320 4c4b 4a43 6f72 7252  ..class LKJCorrR
+0000c420: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
+0000c430: 293a 0a20 2020 206e 616d 6520 3d20 226c  ):.    name = "l
+0000c440: 6b6a 636f 7272 220a 2020 2020 6e64 696d  kjcorr".    ndim
+0000c450: 5f73 7570 7020 3d20 310a 2020 2020 6e64  _supp = 1.    nd
+0000c460: 696d 735f 7061 7261 6d73 203d 205b 302c  ims_params = [0,
+0000c470: 2030 5d0a 2020 2020 6474 7970 6520 3d20   0].    dtype = 
+0000c480: 2266 6c6f 6174 5822 0a20 2020 205f 7072  "floatX".    _pr
+0000c490: 696e 745f 6e61 6d65 203d 2028 224c 4b4a  int_name = ("LKJ
+0000c4a0: 436f 7272 5256 222c 2022 5c5c 6f70 6572  CorrRV", "\\oper
+0000c4b0: 6174 6f72 6e61 6d65 7b4c 4b4a 436f 7272  atorname{LKJCorr
+0000c4c0: 5256 7d22 290a 0a20 2020 2064 6566 206d  RV}")..    def m
+0000c4d0: 616b 655f 6e6f 6465 2873 656c 662c 2072  ake_node(self, r
+0000c4e0: 6e67 2c20 7369 7a65 2c20 6474 7970 652c  ng, size, dtype,
+0000c4f0: 206e 2c20 6574 6129 3a0a 2020 2020 2020   n, eta):.      
+0000c500: 2020 6e20 3d20 7074 2e61 735f 7465 6e73    n = pt.as_tens
+0000c510: 6f72 5f76 6172 6961 626c 6528 6e29 0a20  or_variable(n). 
+0000c520: 2020 2020 2020 2069 6620 6e6f 7420 6e2e         if not n.
+0000c530: 6e64 696d 203d 3d20 303a 0a20 2020 2020  ndim == 0:.     
+0000c540: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0000c550: 7565 4572 726f 7228 226e 206d 7573 7420  ueError("n must 
+0000c560: 6265 2061 2073 6361 6c61 7220 286e 6469  be a scalar (ndi
+0000c570: 6d3d 3029 2e22 290a 0a20 2020 2020 2020  m=0).")..       
+0000c580: 2065 7461 203d 2070 742e 6173 5f74 656e   eta = pt.as_ten
+0000c590: 736f 725f 7661 7269 6162 6c65 2865 7461  sor_variable(eta
+0000c5a0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+0000c5b0: 2065 7461 2e6e 6469 6d20 3d3d 2030 3a0a   eta.ndim == 0:.
+0000c5c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000c5d0: 6520 5661 6c75 6545 7272 6f72 2822 6574  e ValueError("et
+0000c5e0: 6120 6d75 7374 2062 6520 6120 7363 616c  a must be a scal
+0000c5f0: 6172 2028 6e64 696d 3d30 292e 2229 0a0a  ar (ndim=0).")..
+0000c600: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c610: 7570 6572 2829 2e6d 616b 655f 6e6f 6465  uper().make_node
+0000c620: 2872 6e67 2c20 7369 7a65 2c20 6474 7970  (rng, size, dtyp
+0000c630: 652c 206e 2c20 6574 6129 0a0a 2020 2020  e, n, eta)..    
+0000c640: 6465 6620 5f73 7570 705f 7368 6170 655f  def _supp_shape_
+0000c650: 6672 6f6d 5f70 6172 616d 7328 7365 6c66  from_params(self
+0000c660: 2c20 6469 7374 5f70 6172 616d 732c 202a  , dist_params, *
+0000c670: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+0000c680: 2020 6e20 3d20 6469 7374 5f70 6172 616d    n = dist_param
+0000c690: 735b 305d 0a20 2020 2020 2020 2064 6973  s[0].        dis
+0000c6a0: 745f 7368 6170 6520 3d20 2828 6e20 2a20  t_shape = ((n * 
+0000c6b0: 286e 202d 2031 2929 202f 2f20 322c 290a  (n - 1)) // 2,).
+0000c6c0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0000c6d0: 6973 745f 7368 6170 650a 0a20 2020 2040  ist_shape..    @
+0000c6e0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+0000c6f0: 6465 6620 726e 675f 666e 2863 6c73 2c20  def rng_fn(cls, 
+0000c700: 726e 672c 206e 2c20 6574 612c 2073 697a  rng, n, eta, siz
+0000c710: 6529 3a0a 2020 2020 2020 2020 2320 5765  e):.        # We
+0000c720: 2066 6c61 7474 656e 2074 6865 2073 697a   flatten the siz
+0000c730: 6520 746f 206d 616b 6520 6f70 6572 6174  e to make operat
+0000c740: 696f 6e73 2065 6173 6965 722c 2061 6e64  ions easier, and
+0000c750: 2074 6865 6e20 7265 6275 696c 6420 6974   then rebuild it
+0000c760: 0a20 2020 2020 2020 2069 6620 7369 7a65  .        if size
+0000c770: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000c780: 2020 2020 2020 666c 6174 5f73 697a 6520        flat_size 
+0000c790: 3d20 310a 2020 2020 2020 2020 656c 7365  = 1.        else
+0000c7a0: 3a0a 2020 2020 2020 2020 2020 2020 666c  :.            fl
+0000c7b0: 6174 5f73 697a 6520 3d20 6e70 2e70 726f  at_size = np.pro
+0000c7c0: 6428 7369 7a65 290a 0a20 2020 2020 2020  d(size)..       
+0000c7d0: 2043 203d 2063 6c73 2e5f 7261 6e64 6f6d   C = cls._random
+0000c7e0: 5f63 6f72 725f 6d61 7472 6978 2872 6e67  _corr_matrix(rng
+0000c7f0: 3d72 6e67 2c20 6e3d 6e2c 2065 7461 3d65  =rng, n=n, eta=e
+0000c800: 7461 2c20 666c 6174 5f73 697a 653d 666c  ta, flat_size=fl
+0000c810: 6174 5f73 697a 6529 0a0a 2020 2020 2020  at_size)..      
+0000c820: 2020 7472 6975 5f69 6478 203d 206e 702e    triu_idx = np.
+0000c830: 7472 6975 5f69 6e64 6963 6573 286e 2c20  triu_indices(n, 
+0000c840: 6b3d 3129 0a20 2020 2020 2020 2073 616d  k=1).        sam
+0000c850: 706c 6573 203d 2043 5b2e 2e2e 2c20 7472  ples = C[..., tr
+0000c860: 6975 5f69 6478 5b30 5d2c 2074 7269 755f  iu_idx[0], triu_
+0000c870: 6964 785b 315d 5d0a 0a20 2020 2020 2020  idx[1]]..       
+0000c880: 2069 6620 7369 7a65 2069 7320 4e6f 6e65   if size is None
+0000c890: 3a0a 2020 2020 2020 2020 2020 2020 7361  :.            sa
+0000c8a0: 6d70 6c65 7320 3d20 7361 6d70 6c65 735b  mples = samples[
+0000c8b0: 305d 0a20 2020 2020 2020 2065 6c73 653a  0].        else:
+0000c8c0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+0000c8d0: 745f 7368 6170 6520 3d20 286e 202a 2028  t_shape = (n * (
+0000c8e0: 6e20 2d20 3129 2920 2f2f 2032 0a20 2020  n - 1)) // 2.   
+0000c8f0: 2020 2020 2020 2020 2073 616d 706c 6573           samples
+0000c900: 203d 206e 702e 7265 7368 6170 6528 7361   = np.reshape(sa
+0000c910: 6d70 6c65 732c 2028 2a73 697a 652c 2064  mples, (*size, d
+0000c920: 6973 745f 7368 6170 6529 290a 2020 2020  ist_shape)).    
+0000c930: 2020 2020 7265 7475 726e 2073 616d 706c      return sampl
+0000c940: 6573 0a0a 2020 2020 4063 6c61 7373 6d65  es..    @classme
+0000c950: 7468 6f64 0a20 2020 2064 6566 205f 7261  thod.    def _ra
+0000c960: 6e64 6f6d 5f63 6f72 725f 6d61 7472 6978  ndom_corr_matrix
+0000c970: 2863 6c73 2c20 726e 672c 206e 2c20 6574  (cls, rng, n, et
+0000c980: 612c 2066 6c61 745f 7369 7a65 293a 0a20  a, flat_size):. 
+0000c990: 2020 2020 2020 2023 206f 7269 6769 6e61         # origina
+0000c9a0: 6c20 696d 706c 656d 656e 7461 7469 6f6e  l implementation
+0000c9b0: 2069 6e20 5220 7365 653a 0a20 2020 2020   in R see:.     
+0000c9c0: 2020 2023 2068 7474 7073 3a2f 2f67 6974     # https://git
+0000c9d0: 6875 622e 636f 6d2f 726d 6365 6c72 6561  hub.com/rmcelrea
+0000c9e0: 7468 2f72 6574 6869 6e6b 696e 672f 626c  th/rethinking/bl
+0000c9f0: 6f62 2f6d 6173 7465 722f 522f 6469 7374  ob/master/R/dist
+0000ca00: 7269 6275 7469 6f6e 732e 720a 2020 2020  ributions.r.    
+0000ca10: 2020 2020 6265 7461 203d 2065 7461 202d      beta = eta -
+0000ca20: 2031 2e30 202b 206e 202f 2032 2e30 0a20   1.0 + n / 2.0. 
+0000ca30: 2020 2020 2020 2072 3132 203d 2032 2e30         r12 = 2.0
+0000ca40: 202a 2073 7461 7473 2e62 6574 612e 7276   * stats.beta.rv
+0000ca50: 7328 613d 6265 7461 2c20 623d 6265 7461  s(a=beta, b=beta
+0000ca60: 2c20 7369 7a65 3d66 6c61 745f 7369 7a65  , size=flat_size
+0000ca70: 2c20 7261 6e64 6f6d 5f73 7461 7465 3d72  , random_state=r
+0000ca80: 6e67 2920 2d20 312e 300a 2020 2020 2020  ng) - 1.0.      
+0000ca90: 2020 5020 3d20 6e70 2e66 756c 6c28 2866    P = np.full((f
+0000caa0: 6c61 745f 7369 7a65 2c20 6e2c 206e 292c  lat_size, n, n),
+0000cab0: 206e 702e 6579 6528 6e29 290a 2020 2020   np.eye(n)).    
+0000cac0: 2020 2020 505b 2e2e 2e2c 2030 2c20 315d      P[..., 0, 1]
+0000cad0: 203d 2072 3132 0a20 2020 2020 2020 2050   = r12.        P
+0000cae0: 5b2e 2e2e 2c20 312c 2031 5d20 3d20 6e70  [..., 1, 1] = np
+0000caf0: 2e73 7172 7428 312e 3020 2d20 7231 322a  .sqrt(1.0 - r12*
+0000cb00: 2a32 290a 2020 2020 2020 2020 666f 7220  *2).        for 
+0000cb10: 6d70 3120 696e 2072 616e 6765 2832 2c20  mp1 in range(2, 
+0000cb20: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+0000cb30: 6265 7461 202d 3d20 302e 350a 2020 2020  beta -= 0.5.    
+0000cb40: 2020 2020 2020 2020 7920 3d20 7374 6174          y = stat
+0000cb50: 732e 6265 7461 2e72 7673 2861 3d6d 7031  s.beta.rvs(a=mp1
+0000cb60: 202f 2032 2e30 2c20 623d 6265 7461 2c20   / 2.0, b=beta, 
+0000cb70: 7369 7a65 3d66 6c61 745f 7369 7a65 2c20  size=flat_size, 
+0000cb80: 7261 6e64 6f6d 5f73 7461 7465 3d72 6e67  random_state=rng
+0000cb90: 290a 2020 2020 2020 2020 2020 2020 7a20  ).            z 
+0000cba0: 3d20 7374 6174 732e 6e6f 726d 2e72 7673  = stats.norm.rvs
+0000cbb0: 286c 6f63 3d30 2c20 7363 616c 653d 312c  (loc=0, scale=1,
+0000cbc0: 2073 697a 653d 2866 6c61 745f 7369 7a65   size=(flat_size
+0000cbd0: 2c20 6d70 3129 2c20 7261 6e64 6f6d 5f73  , mp1), random_s
+0000cbe0: 7461 7465 3d72 6e67 290a 2020 2020 2020  tate=rng).      
+0000cbf0: 2020 2020 2020 7a20 3d20 7a20 2f20 6e70        z = z / np
+0000cc00: 2e73 7172 7428 6e70 2e65 696e 7375 6d28  .sqrt(np.einsum(
+0000cc10: 2269 6a2c 696a 2d3e 6922 2c20 7a2c 207a  "ij,ij->i", z, z
+0000cc20: 2929 5b2e 2e2e 2c20 6e70 2e6e 6577 6178  ))[..., np.newax
+0000cc30: 6973 5d0a 2020 2020 2020 2020 2020 2020  is].            
+0000cc40: 505b 2e2e 2e2c 2030 3a6d 7031 2c20 6d70  P[..., 0:mp1, mp
+0000cc50: 315d 203d 206e 702e 7371 7274 2879 5b2e  1] = np.sqrt(y[.
+0000cc60: 2e2e 2c20 6e70 2e6e 6577 6178 6973 5d29  .., np.newaxis])
+0000cc70: 202a 207a 0a20 2020 2020 2020 2020 2020   * z.           
+0000cc80: 2050 5b2e 2e2e 2c20 6d70 312c 206d 7031   P[..., mp1, mp1
+0000cc90: 5d20 3d20 6e70 2e73 7172 7428 312e 3020  ] = np.sqrt(1.0 
+0000cca0: 2d20 7929 0a20 2020 2020 2020 2043 203d  - y).        C =
+0000ccb0: 206e 702e 6569 6e73 756d 2822 2e2e 2e6a   np.einsum("...j
+0000ccc0: 692c 2e2e 2e6a 6b2d 3e2e 2e2e 696b 222c  i,...jk->...ik",
+0000ccd0: 2050 2c20 5029 0a20 2020 2020 2020 2072   P, P).        r
+0000cce0: 6574 7572 6e20 430a 0a0a 6c6b 6a63 6f72  eturn C...lkjcor
+0000ccf0: 7220 3d20 4c4b 4a43 6f72 7252 5628 290a  r = LKJCorrRV().
+0000cd00: 0a0a 636c 6173 7320 4c4b 4a43 6f72 7228  ..class LKJCorr(
+0000cd10: 426f 756e 6465 6443 6f6e 7469 6e75 6f75  BoundedContinuou
+0000cd20: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
+0000cd30: 2054 6865 204c 4b4a 2028 4c65 7761 6e64   The LKJ (Lewand
+0000cd40: 6f77 736b 692c 204b 7572 6f77 6963 6b61  owski, Kurowicka
+0000cd50: 2061 6e64 204a 6f65 2920 6c6f 672d 6c69   and Joe) log-li
+0000cd60: 6b65 6c69 686f 6f64 2e0a 0a20 2020 2054  kelihood...    T
+0000cd70: 6865 204c 4b4a 2064 6973 7472 6962 7574  he LKJ distribut
+0000cd80: 696f 6e20 6973 2061 2070 7269 6f72 2064  ion is a prior d
+0000cd90: 6973 7472 6962 7574 696f 6e20 666f 7220  istribution for 
+0000cda0: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
+0000cdb0: 6963 6573 2e0a 2020 2020 4966 2065 7461  ices..    If eta
+0000cdc0: 203d 2031 2074 6869 7320 636f 7272 6573   = 1 this corres
+0000cdd0: 706f 6e64 7320 746f 2074 6865 2075 6e69  ponds to the uni
+0000cde0: 666f 726d 2064 6973 7472 6962 7574 696f  form distributio
+0000cdf0: 6e20 6f76 6572 2063 6f72 7265 6c61 7469  n over correlati
+0000ce00: 6f6e 0a20 2020 206d 6174 7269 6365 732e  on.    matrices.
+0000ce10: 2046 6f72 2065 7461 202d 3e20 6f6f 2074   For eta -> oo t
+0000ce20: 6865 204c 4b4a 2070 7269 6f72 2061 7070  he LKJ prior app
+0000ce30: 726f 6163 6865 7320 7468 6520 6964 656e  roaches the iden
+0000ce40: 7469 7479 206d 6174 7269 782e 0a0a 2020  tity matrix...  
+0000ce50: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
+0000ce60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ce70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ce80: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
+0000ce90: 7570 706f 7274 2020 2055 7070 6572 2074  upport   Upper t
+0000cea0: 7269 616e 6775 6c61 7220 6d61 7472 6978  riangular matrix
+0000ceb0: 2077 6974 6820 7661 6c75 6573 2069 6e20   with values in 
+0000cec0: 5b2d 312c 2031 5d0a 2020 2020 3d3d 3d3d  [-1, 1].    ====
+0000ced0: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+0000cee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cf00: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
+0000cf10: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0000cf20: 2d2d 2d0a 2020 2020 6e20 3a20 7465 6e73  ---.    n : tens
+0000cf30: 6f72 5f6c 696b 6520 6f66 2069 6e74 0a20  or_like of int. 
+0000cf40: 2020 2020 2020 2044 696d 656e 7369 6f6e         Dimension
+0000cf50: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
+0000cf60: 6365 206d 6174 7269 7820 286e 203e 2031  ce matrix (n > 1
+0000cf70: 292e 0a20 2020 2065 7461 203a 2074 656e  )..    eta : ten
+0000cf80: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
+0000cf90: 740a 2020 2020 2020 2020 5468 6520 7368  t.        The sh
+0000cfa0: 6170 6520 7061 7261 6d65 7465 7220 2865  ape parameter (e
+0000cfb0: 7461 203e 2030 2920 6f66 2074 6865 204c  ta > 0) of the L
+0000cfc0: 4b4a 2064 6973 7472 6962 7574 696f 6e2e  KJ distribution.
+0000cfd0: 2065 7461 203d 2031 0a20 2020 2020 2020   eta = 1.       
+0000cfe0: 2069 6d70 6c69 6573 2061 2075 6e69 666f   implies a unifo
+0000cff0: 726d 2064 6973 7472 6962 7574 696f 6e20  rm distribution 
+0000d000: 6f66 2074 6865 2063 6f72 7265 6c61 7469  of the correlati
+0000d010: 6f6e 206d 6174 7269 6365 733b 0a20 2020  on matrices;.   
+0000d020: 2020 2020 206c 6172 6765 7220 7661 6c75       larger valu
+0000d030: 6573 2070 7574 206d 6f72 6520 7765 6967  es put more weig
+0000d040: 6874 206f 6e20 6d61 7472 6963 6573 2077  ht on matrices w
+0000d050: 6974 6820 6665 7720 636f 7272 656c 6174  ith few correlat
+0000d060: 696f 6e73 2e0a 0a20 2020 204e 6f74 6573  ions...    Notes
+0000d070: 0a20 2020 202d 2d2d 2d2d 0a20 2020 2054  .    -----.    T
+0000d080: 6869 7320 696d 706c 656d 656e 7461 7469  his implementati
+0000d090: 6f6e 206f 6e6c 7920 7265 7475 726e 7320  on only returns 
+0000d0a0: 7468 6520 7661 6c75 6573 206f 6620 7468  the values of th
+0000d0b0: 6520 7570 7065 7220 7472 6961 6e67 756c  e upper triangul
+0000d0c0: 6172 0a20 2020 206d 6174 7269 7820 6578  ar.    matrix ex
+0000d0d0: 636c 7564 696e 6720 7468 6520 6469 6167  cluding the diag
+0000d0e0: 6f6e 616c 2e20 4865 7265 2069 7320 6120  onal. Here is a 
+0000d0f0: 7363 6865 6d61 7469 6320 666f 7220 6e20  schematic for n 
+0000d100: 3d20 352c 2073 686f 7769 6e67 0a20 2020  = 5, showing.   
+0000d110: 2074 6865 2069 6e64 6578 6573 206f 6620   the indexes of 
+0000d120: 7468 6520 656c 656d 656e 7473 3a3a 0a0a  the elements::..
+0000d130: 2020 2020 2020 2020 5b5b 2d20 3020 3120          [[- 0 1 
+0000d140: 3220 335d 0a20 2020 2020 2020 2020 5b2d  2 3].         [-
+0000d150: 202d 2034 2035 2036 5d0a 2020 2020 2020   - 4 5 6].      
+0000d160: 2020 205b 2d20 2d20 2d20 3720 385d 0a20     [- - - 7 8]. 
+0000d170: 2020 2020 2020 2020 5b2d 202d 202d 202d          [- - - -
+0000d180: 2039 5d0a 2020 2020 2020 2020 205b 2d20   9].         [- 
+0000d190: 2d20 2d20 2d20 2d5d 5d0a 0a0a 2020 2020  - - - -]]...    
+0000d1a0: 5265 6665 7265 6e63 6573 0a20 2020 202d  References.    -
+0000d1b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e  ---------.    ..
+0000d1c0: 205b 4c4b 4a32 3030 395d 204c 6577 616e   [LKJ2009] Lewan
+0000d1d0: 646f 7773 6b69 2c20 442e 2c20 4b75 726f  dowski, D., Kuro
+0000d1e0: 7769 636b 612c 2044 2e20 616e 6420 4a6f  wicka, D. and Jo
+0000d1f0: 652c 2048 2e20 2832 3030 3929 2e0a 2020  e, H. (2009)..  
+0000d200: 2020 2020 2020 2247 656e 6572 6174 696e        "Generatin
+0000d210: 6720 7261 6e64 6f6d 2063 6f72 7265 6c61  g random correla
+0000d220: 7469 6f6e 206d 6174 7269 6365 7320 6261  tion matrices ba
+0000d230: 7365 6420 6f6e 2076 696e 6573 2061 6e64  sed on vines and
+0000d240: 0a20 2020 2020 2020 2065 7874 656e 6465  .        extende
+0000d250: 6420 6f6e 696f 6e20 6d65 7468 6f64 2e22  d onion method."
+0000d260: 204a 6f75 726e 616c 206f 6620 6d75 6c74   Journal of mult
+0000d270: 6976 6172 6961 7465 2061 6e61 6c79 7369  ivariate analysi
+0000d280: 732c 0a20 2020 2020 2020 2031 3030 2839  s,.        100(9
+0000d290: 292c 2070 702e 3139 3839 2d32 3030 312e  ), pp.1989-2001.
+0000d2a0: 0a20 2020 2022 2222 0a0a 2020 2020 7276  .    """..    rv
+0000d2b0: 5f6f 7020 3d20 6c6b 6a63 6f72 720a 0a20  _op = lkjcorr.. 
+0000d2c0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0000d2d0: 2020 2020 6465 6620 6469 7374 2863 6c73      def dist(cls
+0000d2e0: 2c20 6e2c 2065 7461 2c20 2a2a 6b77 6172  , n, eta, **kwar
+0000d2f0: 6773 293a 0a20 2020 2020 2020 206e 203d  gs):.        n =
+0000d300: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+0000d310: 7269 6162 6c65 2869 6e74 5828 6e29 290a  riable(intX(n)).
+0000d320: 2020 2020 2020 2020 6574 6120 3d20 7074          eta = pt
+0000d330: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+0000d340: 626c 6528 666c 6f61 7458 2865 7461 2929  ble(floatX(eta))
+0000d350: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d360: 7375 7065 7228 292e 6469 7374 285b 6e2c  super().dist([n,
+0000d370: 2065 7461 5d2c 202a 2a6b 7761 7267 7329   eta], **kwargs)
+0000d380: 0a0a 2020 2020 6465 6620 6d6f 6d65 6e74  ..    def moment
+0000d390: 2872 762c 202a 6172 6773 293a 0a20 2020  (rv, *args):.   
+0000d3a0: 2020 2020 2072 6574 7572 6e20 7074 2e7a       return pt.z
+0000d3b0: 6572 6f73 5f6c 696b 6528 7276 290a 0a20  eros_like(rv).. 
+0000d3c0: 2020 2064 6566 206c 6f67 7028 7661 6c75     def logp(valu
+0000d3d0: 652c 206e 2c20 6574 6129 3a0a 2020 2020  e, n, eta):.    
+0000d3e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d3f0: 4361 6c63 756c 6174 6520 6c6f 672d 7072  Calculate log-pr
+0000d400: 6f62 6162 696c 6974 7920 6f66 204c 4b4a  obability of LKJ
+0000d410: 2064 6973 7472 6962 7574 696f 6e20 6174   distribution at
+0000d420: 2073 7065 6369 6669 6564 0a20 2020 2020   specified.     
+0000d430: 2020 2076 616c 7565 2e0a 0a20 2020 2020     value...     
+0000d440: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000d450: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000d460: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
+0000d470: 6e75 6d65 7269 630a 2020 2020 2020 2020  numeric.        
+0000d480: 2020 2020 5661 6c75 6520 666f 7220 7768      Value for wh
+0000d490: 6963 6820 6c6f 672d 7072 6f62 6162 696c  ich log-probabil
+0000d4a0: 6974 7920 6973 2063 616c 6375 6c61 7465  ity is calculate
+0000d4b0: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
+0000d4c0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000d4d0: 2d2d 2d0a 2020 2020 2020 2020 5465 6e73  ---.        Tens
+0000d4e0: 6f72 5661 7269 6162 6c65 0a20 2020 2020  orVariable.     
+0000d4f0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000d500: 2320 544f 444f 3a20 5079 5465 6e73 6f72  # TODO: PyTensor
+0000d510: 2064 6f65 7320 6e6f 7420 6861 7665 2061   does not have a
+0000d520: 2060 7472 6975 5f69 6e64 6963 6573 602c   `triu_indices`,
+0000d530: 2073 6f20 7765 2063 616e 206f 6e6c 7920   so we can only 
+0000d540: 776f 726b 2077 6974 6820 636f 6e73 7461  work with consta
+0000d550: 6e74 0a20 2020 2020 2020 2023 2020 6e20  nt.        #  n 
+0000d560: 286f 7220 656c 7365 2066 696e 6420 6120  (or else find a 
+0000d570: 6469 6666 6572 656e 7420 6578 7072 6573  different expres
+0000d580: 7369 6f6e 290a 2020 2020 2020 2020 6966  sion).        if
+0000d590: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0000d5a0: 6e2c 2043 6f6e 7374 616e 7429 3a0a 2020  n, Constant):.  
+0000d5b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d5c0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+0000d5d0: 726f 7228 226c 6f67 7020 6f6e 6c79 2069  ror("logp only i
+0000d5e0: 6d70 6c65 6d65 6e74 6564 2066 6f72 2063  mplemented for c
+0000d5f0: 6f6e 7374 616e 7420 606e 6022 290a 0a20  onstant `n`").. 
+0000d600: 2020 2020 2020 206e 203d 2069 6e74 286e         n = int(n
+0000d610: 2e64 6174 6129 0a20 2020 2020 2020 2073  .data).        s
+0000d620: 6861 7065 203d 206e 202a 2028 6e20 2d20  hape = n * (n - 
+0000d630: 3129 202f 2f20 320a 2020 2020 2020 2020  1) // 2.        
+0000d640: 7472 695f 696e 6465 7820 3d20 6e70 2e7a  tri_index = np.z
+0000d650: 6572 6f73 2828 6e2c 206e 292c 2064 7479  eros((n, n), dty
+0000d660: 7065 3d22 696e 7433 3222 290a 2020 2020  pe="int32").    
+0000d670: 2020 2020 7472 695f 696e 6465 785b 6e70      tri_index[np
+0000d680: 2e74 7269 755f 696e 6469 6365 7328 6e2c  .triu_indices(n,
+0000d690: 206b 3d31 295d 203d 206e 702e 6172 616e   k=1)] = np.aran
+0000d6a0: 6765 2873 6861 7065 290a 2020 2020 2020  ge(shape).      
+0000d6b0: 2020 7472 695f 696e 6465 785b 6e70 2e74    tri_index[np.t
+0000d6c0: 7269 755f 696e 6469 6365 7328 6e2c 206b  riu_indices(n, k
+0000d6d0: 3d31 295b 3a3a 2d31 5d5d 203d 206e 702e  =1)[::-1]] = np.
+0000d6e0: 6172 616e 6765 2873 6861 7065 290a 0a20  arange(shape).. 
+0000d6f0: 2020 2020 2020 2076 616c 7565 203d 2070         value = p
+0000d700: 742e 7461 6b65 2876 616c 7565 2c20 7472  t.take(value, tr
+0000d710: 695f 696e 6465 7829 0a20 2020 2020 2020  i_index).       
+0000d720: 2076 616c 7565 203d 2070 742e 6669 6c6c   value = pt.fill
+0000d730: 5f64 6961 676f 6e61 6c28 7661 6c75 652c  _diagonal(value,
+0000d740: 2031 290a 0a20 2020 2020 2020 2023 2054   1)..        # T
+0000d750: 4f44 4f3a 205f 6c6b 6a5f 6e6f 726d 616c  ODO: _lkj_normal
+0000d760: 697a 696e 675f 636f 6e73 7461 6e74 2063  izing_constant c
+0000d770: 7572 7265 6e74 6c79 2072 6571 7569 7265  urrently require
+0000d780: 7320 6065 7461 6020 616e 6420 606e 6020  s `eta` and `n` 
+0000d790: 746f 2062 6520 636f 6e73 7461 6e74 730a  to be constants.
+0000d7a0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0000d7b0: 7369 6e73 7461 6e63 6528 6574 612c 2043  sinstance(eta, C
+0000d7c0: 6f6e 7374 616e 7429 3a0a 2020 2020 2020  onstant):.      
+0000d7d0: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+0000d7e0: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+0000d7f0: 226c 6f67 7020 6f6e 6c79 2069 6d70 6c65  "logp only imple
+0000d800: 6d65 6e74 6564 2066 6f72 2063 6f6e 7374  mented for const
+0000d810: 616e 7420 6065 7461 6022 290a 2020 2020  ant `eta`").    
+0000d820: 2020 2020 6574 6120 3d20 666c 6f61 7428      eta = float(
+0000d830: 6574 612e 6461 7461 290a 2020 2020 2020  eta.data).      
+0000d840: 2020 7265 7375 6c74 203d 205f 6c6b 6a5f    result = _lkj_
+0000d850: 6e6f 726d 616c 697a 696e 675f 636f 6e73  normalizing_cons
+0000d860: 7461 6e74 2865 7461 2c20 6e29 0a20 2020  tant(eta, n).   
+0000d870: 2020 2020 2072 6573 756c 7420 2b3d 2028       result += (
+0000d880: 6574 6120 2d20 312e 3029 202a 2070 742e  eta - 1.0) * pt.
+0000d890: 6c6f 6728 6465 7428 7661 6c75 6529 290a  log(det(value)).
+0000d8a0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000d8b0: 6865 636b 5f70 6172 616d 6574 6572 7328  heck_parameters(
+0000d8c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000d8d0: 756c 742c 0a20 2020 2020 2020 2020 2020  ult,.           
+0000d8e0: 2076 616c 7565 203e 3d20 2d31 2c0a 2020   value >= -1,.  
+0000d8f0: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
+0000d900: 3c3d 2031 2c0a 2020 2020 2020 2020 2020  <= 1,.          
+0000d910: 2020 6d61 7472 6978 5f70 6f73 5f64 6566    matrix_pos_def
+0000d920: 2876 616c 7565 292c 0a20 2020 2020 2020  (value),.       
+0000d930: 2020 2020 2065 7461 203e 2030 2c0a 2020       eta > 0,.  
+0000d940: 2020 2020 2020 290a 0a0a 405f 6465 6661        )...@_defa
+0000d950: 756c 745f 7472 616e 7366 6f72 6d2e 7265  ult_transform.re
+0000d960: 6769 7374 6572 284c 4b4a 436f 7272 290a  gister(LKJCorr).
+0000d970: 6465 6620 6c6b 6a63 6f72 725f 6465 6661  def lkjcorr_defa
+0000d980: 756c 745f 7472 616e 7366 6f72 6d28 6f70  ult_transform(op
+0000d990: 2c20 7276 293a 0a20 2020 2072 6574 7572  , rv):.    retur
+0000d9a0: 6e20 496e 7465 7276 616c 2866 6c6f 6174  n Interval(float
+0000d9b0: 5828 2d31 2e30 292c 2066 6c6f 6174 5828  X(-1.0), floatX(
+0000d9c0: 312e 3029 290a 0a0a 636c 6173 7320 4d61  1.0))...class Ma
+0000d9d0: 7472 6978 4e6f 726d 616c 5256 2852 616e  trixNormalRV(Ran
+0000d9e0: 646f 6d56 6172 6961 626c 6529 3a0a 2020  domVariable):.  
+0000d9f0: 2020 6e61 6d65 203d 2022 6d61 7472 6978    name = "matrix
+0000da00: 6e6f 726d 616c 220a 2020 2020 6e64 696d  normal".    ndim
+0000da10: 5f73 7570 7020 3d20 320a 2020 2020 6e64  _supp = 2.    nd
+0000da20: 696d 735f 7061 7261 6d73 203d 205b 322c  ims_params = [2,
+0000da30: 2032 2c20 325d 0a20 2020 2064 7479 7065   2, 2].    dtype
+0000da40: 203d 2022 666c 6f61 7458 220a 2020 2020   = "floatX".    
+0000da50: 5f70 7269 6e74 5f6e 616d 6520 3d20 2822  _print_name = ("
+0000da60: 4d61 7472 6978 4e6f 726d 616c 222c 2022  MatrixNormal", "
+0000da70: 5c5c 6f70 6572 6174 6f72 6e61 6d65 7b4d  \\operatorname{M
+0000da80: 6174 7269 784e 6f72 6d61 6c7d 2229 0a0a  atrixNormal}")..
+0000da90: 2020 2020 6465 6620 5f73 7570 705f 7368      def _supp_sh
+0000daa0: 6170 655f 6672 6f6d 5f70 6172 616d 7328  ape_from_params(
+0000dab0: 7365 6c66 2c20 6469 7374 5f70 6172 616d  self, dist_param
+0000dac0: 732c 2070 6172 616d 5f73 6861 7065 733d  s, param_shapes=
+0000dad0: 4e6f 6e65 293a 0a20 2020 2020 2020 2072  None):.        r
+0000dae0: 6574 7572 6e20 7375 7070 5f73 6861 7065  eturn supp_shape
+0000daf0: 5f66 726f 6d5f 7265 665f 7061 7261 6d5f  _from_ref_param_
+0000db00: 7368 6170 6528 0a20 2020 2020 2020 2020  shape(.         
+0000db10: 2020 206e 6469 6d5f 7375 7070 3d73 656c     ndim_supp=sel
+0000db20: 662e 6e64 696d 5f73 7570 702c 0a20 2020  f.ndim_supp,.   
+0000db30: 2020 2020 2020 2020 2064 6973 745f 7061           dist_pa
+0000db40: 7261 6d73 3d64 6973 745f 7061 7261 6d73  rams=dist_params
+0000db50: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+0000db60: 7261 6d5f 7368 6170 6573 3d70 6172 616d  ram_shapes=param
+0000db70: 5f73 6861 7065 732c 0a20 2020 2020 2020  _shapes,.       
+0000db80: 2020 2020 2072 6566 5f70 6172 616d 5f69       ref_param_i
+0000db90: 6478 3d30 2c0a 2020 2020 2020 2020 290a  dx=0,.        ).
+0000dba0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+0000dbb0: 640a 2020 2020 6465 6620 726e 675f 666e  d.    def rng_fn
+0000dbc0: 2863 6c73 2c20 726e 672c 206d 752c 2072  (cls, rng, mu, r
+0000dbd0: 6f77 6368 6f6c 2c20 636f 6c63 686f 6c2c  owchol, colchol,
+0000dbe0: 2073 697a 653d 4e6f 6e65 293a 0a20 2020   size=None):.   
+0000dbf0: 2020 2020 2073 697a 6520 3d20 746f 5f74       size = to_t
+0000dc00: 7570 6c65 2873 697a 6529 0a20 2020 2020  uple(size).     
+0000dc10: 2020 2064 6973 745f 7368 6170 6520 3d20     dist_shape = 
+0000dc20: 746f 5f74 7570 6c65 285b 726f 7763 686f  to_tuple([rowcho
+0000dc30: 6c2e 7368 6170 655b 305d 2c20 636f 6c63  l.shape[0], colc
+0000dc40: 686f 6c2e 7368 6170 655b 305d 5d29 0a20  hol.shape[0]]). 
+0000dc50: 2020 2020 2020 206f 7574 7075 745f 7368         output_sh
+0000dc60: 6170 6520 3d20 7369 7a65 202b 2064 6973  ape = size + dis
+0000dc70: 745f 7368 6170 650a 0a20 2020 2020 2020  t_shape..       
+0000dc80: 2023 2042 726f 6164 6361 7374 696e 6720   # Broadcasting 
+0000dc90: 616c 6c20 7061 7261 6d65 7465 7273 0a20  all parameters. 
+0000dca0: 2020 2020 2020 2073 6861 7065 7320 3d20         shapes = 
+0000dcb0: 5b6d 752e 7368 6170 652c 206f 7574 7075  [mu.shape, outpu
+0000dcc0: 745f 7368 6170 655d 0a20 2020 2020 2020  t_shape].       
+0000dcd0: 2062 726f 6164 6361 7374 6162 6c65 5f73   broadcastable_s
+0000dce0: 6861 7065 203d 2062 726f 6164 6361 7374  hape = broadcast
+0000dcf0: 5f64 6973 745f 7361 6d70 6c65 735f 7368  _dist_samples_sh
+0000dd00: 6170 6528 7368 6170 6573 2c20 7369 7a65  ape(shapes, size
+0000dd10: 3d73 697a 6529 0a20 2020 2020 2020 206d  =size).        m
+0000dd20: 7520 3d20 6e70 2e62 726f 6164 6361 7374  u = np.broadcast
+0000dd30: 5f74 6f28 6d75 2c20 7368 6170 653d 6272  _to(mu, shape=br
+0000dd40: 6f61 6463 6173 7461 626c 655f 7368 6170  oadcastable_shap
+0000dd50: 6529 0a20 2020 2020 2020 2072 6f77 6368  e).        rowch
+0000dd60: 6f6c 203d 206e 702e 6272 6f61 6463 6173  ol = np.broadcas
+0000dd70: 745f 746f 2872 6f77 6368 6f6c 2c20 7368  t_to(rowchol, sh
+0000dd80: 6170 653d 7369 7a65 202b 2072 6f77 6368  ape=size + rowch
+0000dd90: 6f6c 2e73 6861 7065 5b2d 323a 5d29 0a0a  ol.shape[-2:])..
+0000dda0: 2020 2020 2020 2020 636f 6c63 686f 6c20          colchol 
+0000ddb0: 3d20 6e70 2e62 726f 6164 6361 7374 5f74  = np.broadcast_t
+0000ddc0: 6f28 636f 6c63 686f 6c2c 2073 6861 7065  o(colchol, shape
+0000ddd0: 3d73 697a 6520 2b20 636f 6c63 686f 6c2e  =size + colchol.
+0000dde0: 7368 6170 655b 2d32 3a5d 290a 2020 2020  shape[-2:]).    
+0000ddf0: 2020 2020 636f 6c63 686f 6c20 3d20 6e70      colchol = np
+0000de00: 2e73 7761 7061 7865 7328 636f 6c63 686f  .swapaxes(colcho
+0000de10: 6c2c 202d 312c 202d 3229 2020 2320 5461  l, -1, -2)  # Ta
+0000de20: 6b65 2074 7261 6e73 706f 7365 0a0a 2020  ke transpose..  
+0000de30: 2020 2020 2020 7374 616e 6461 7264 5f6e        standard_n
+0000de40: 6f72 6d61 6c20 3d20 726e 672e 7374 616e  ormal = rng.stan
+0000de50: 6461 7264 5f6e 6f72 6d61 6c28 6f75 7470  dard_normal(outp
+0000de60: 7574 5f73 6861 7065 290a 2020 2020 2020  ut_shape).      
+0000de70: 2020 7361 6d70 6c65 7320 3d20 6d75 202b    samples = mu +
+0000de80: 206e 702e 6d61 746d 756c 2872 6f77 6368   np.matmul(rowch
+0000de90: 6f6c 2c20 6e70 2e6d 6174 6d75 6c28 7374  ol, np.matmul(st
+0000dea0: 616e 6461 7264 5f6e 6f72 6d61 6c2c 2063  andard_normal, c
+0000deb0: 6f6c 6368 6f6c 2929 0a0a 2020 2020 2020  olchol))..      
+0000dec0: 2020 7265 7475 726e 2073 616d 706c 6573    return samples
+0000ded0: 0a0a 0a6d 6174 7269 786e 6f72 6d61 6c20  ...matrixnormal 
+0000dee0: 3d20 4d61 7472 6978 4e6f 726d 616c 5256  = MatrixNormalRV
+0000def0: 2829 0a0a 0a63 6c61 7373 204d 6174 7269  ()...class Matri
+0000df00: 784e 6f72 6d61 6c28 436f 6e74 696e 756f  xNormal(Continuo
+0000df10: 7573 293a 0a20 2020 2072 2222 220a 2020  us):.    r""".  
+0000df20: 2020 4d61 7472 6978 2d76 616c 7565 6420    Matrix-valued 
+0000df30: 6e6f 726d 616c 206c 6f67 2d6c 696b 656c  normal log-likel
+0000df40: 6968 6f6f 642e 0a0a 2020 2020 2e2e 206d  ihood...    .. m
+0000df50: 6174 683a 3a0a 2020 2020 2020 2066 2878  ath::.       f(x
+0000df60: 205c 6d69 6420 5c6d 752c 2055 2c20 5629   \mid \mu, U, V)
+0000df70: 203d 0a20 2020 2020 2020 2020 2020 5c66   =.           \f
+0000df80: 7261 637b 317d 7b28 325c 7069 5e7b 6d20  rac{1}{(2\pi^{m 
+0000df90: 6e7d 207c 557c 5e6e 207c 567c 5e6d 295e  n} |U|^n |V|^m)^
+0000dfa0: 7b31 2f32 7d7d 0a20 2020 2020 2020 2020  {1/2}}.         
+0000dfb0: 2020 5c65 7870 5c6c 6566 745c 7b0a 2020    \exp\left\{.  
+0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2d5c                -\
+0000dfd0: 6672 6163 7b31 7d7b 327d 205c 6d61 7468  frac{1}{2} \math
+0000dfe0: 726d 7b54 727d 5b20 565e 7b2d 317d 2028  rm{Tr}[ V^{-1} (
+0000dff0: 782d 5c6d 7529 5e7b 5c70 7269 6d65 7d20  x-\mu)^{\prime} 
+0000e000: 555e 7b2d 317d 2028 782d 5c6d 7529 5d0a  U^{-1} (x-\mu)].
+0000e010: 2020 2020 2020 2020 2020 2020 5c72 6967              \rig
+0000e020: 6874 5c7d 0a0a 2020 2020 3d3d 3d3d 3d3d  ht\}..    ======
+0000e030: 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d  =========  =====
+0000e040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000e050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000e060: 0a20 2020 2053 7570 706f 7274 2020 2020  .    Support    
+0000e070: 2020 2020 2020 3a6d 6174 683a 6078 205c        :math:`x \
+0000e080: 696e 205c 6d61 7468 6262 7b52 7d5e 7b6d  in \mathbb{R}^{m
+0000e090: 205c 7469 6d65 7320 6e7d 600a 2020 2020   \times n}`.    
+0000e0a0: 4d65 616e 2020 2020 2020 2020 2020 2020  Mean            
+0000e0b0: 203a 6d61 7468 3a60 5c6d 7560 0a20 2020   :math:`\mu`.   
+0000e0c0: 2052 6f77 2056 6172 6961 6e63 6520 2020   Row Variance   
+0000e0d0: 2020 3a6d 6174 683a 6055 600a 2020 2020    :math:`U`.    
+0000e0e0: 436f 6c75 6d6e 2056 6172 6961 6e63 6520  Column Variance 
+0000e0f0: 203a 6d61 7468 3a60 5660 0a20 2020 203d   :math:`V`.    =
+0000e100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020  ==============  
+0000e110: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000e120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000e130: 3d3d 3d3d 3d0a 0a20 2020 2050 6172 616d  =====..    Param
+0000e140: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0000e150: 2d2d 2d2d 0a20 2020 206d 7520 3a20 7465  ----.    mu : te
+0000e160: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
+0000e170: 6174 0a20 2020 2020 2020 2041 7272 6179  at.        Array
+0000e180: 206f 6620 6d65 616e 732e 204d 7573 7420   of means. Must 
+0000e190: 6265 2062 726f 6164 6361 7374 6162 6c65  be broadcastable
+0000e1a0: 2077 6974 6820 7468 6520 7261 6e64 6f6d   with the random
+0000e1b0: 2076 6172 6961 626c 6520 5820 7375 6368   variable X such
+0000e1c0: 0a20 2020 2020 2020 2074 6861 7420 7468  .        that th
+0000e1d0: 6520 7368 6170 6520 6f66 206d 7520 2b20  e shape of mu + 
+0000e1e0: 5820 6973 2028 4d2c 204e 292e 0a20 2020  X is (M, N)..   
+0000e1f0: 2072 6f77 636f 7620 3a20 284d 2c20 4d29   rowcov : (M, M)
+0000e200: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
+0000e210: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+0000e220: 2020 2020 2020 2020 416d 6f6e 672d 726f          Among-ro
+0000e230: 7720 636f 7661 7269 616e 6365 206d 6174  w covariance mat
+0000e240: 7269 782e 2044 6566 696e 6573 2076 6172  rix. Defines var
+0000e250: 6961 6e63 6520 7769 7468 696e 0a20 2020  iance within.   
+0000e260: 2020 2020 2063 6f6c 756d 6e73 2e20 4578       columns. Ex
+0000e270: 6163 746c 7920 6f6e 6520 6f66 2072 6f77  actly one of row
+0000e280: 636f 7620 6f72 2072 6f77 6368 6f6c 2069  cov or rowchol i
+0000e290: 7320 6e65 6564 6564 2e0a 2020 2020 726f  s needed..    ro
+0000e2a0: 7763 686f 6c20 3a20 284d 2c20 4d29 2074  wchol : (M, M) t
+0000e2b0: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
+0000e2c0: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
+0000e2d0: 2020 2020 2020 4368 6f6c 6573 6b79 2064        Cholesky d
+0000e2e0: 6563 6f6d 706f 7369 7469 6f6e 206f 6620  ecomposition of 
+0000e2f0: 616d 6f6e 672d 726f 7720 636f 7661 7269  among-row covari
+0000e300: 616e 6365 206d 6174 7269 782e 2045 7861  ance matrix. Exa
+0000e310: 6374 6c79 206f 6e65 206f 660a 2020 2020  ctly one of.    
+0000e320: 2020 2020 726f 7763 6f76 206f 7220 726f      rowcov or ro
+0000e330: 7763 686f 6c20 6973 206e 6565 6465 642e  wchol is needed.
+0000e340: 0a20 2020 2063 6f6c 636f 7620 3a20 284e  .    colcov : (N
+0000e350: 2c20 4e29 2074 656e 736f 725f 6c69 6b65  , N) tensor_like
+0000e360: 206f 6620 666c 6f61 742c 206f 7074 696f   of float, optio
+0000e370: 6e61 6c0a 2020 2020 2020 2020 416d 6f6e  nal.        Amon
+0000e380: 672d 636f 6c75 6d6e 2063 6f76 6172 6961  g-column covaria
+0000e390: 6e63 6520 6d61 7472 6978 2e20 4966 2072  nce matrix. If r
+0000e3a0: 6f77 636f 7620 6973 2074 6865 2069 6465  owcov is the ide
+0000e3b0: 6e74 6974 7920 6d61 7472 6978 2c0a 2020  ntity matrix,.  
+0000e3c0: 2020 2020 2020 7468 6973 2066 756e 6374        this funct
+0000e3d0: 696f 6e73 2061 7320 6063 6f76 6020 696e  ions as `cov` in
+0000e3e0: 204d 764e 6f72 6d61 6c2e 0a20 2020 2020   MvNormal..     
+0000e3f0: 2020 2045 7861 6374 6c79 206f 6e65 206f     Exactly one o
+0000e400: 6620 636f 6c63 6f76 206f 7220 636f 6c63  f colcov or colc
+0000e410: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
+0000e420: 2020 2063 6f6c 6368 6f6c 203a 2028 4e2c     colchol : (N,
+0000e430: 204e 2920 7465 6e73 6f72 5f6c 696b 6520   N) tensor_like 
+0000e440: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+0000e450: 616c 0a20 2020 2020 2020 2043 686f 6c65  al.        Chole
+0000e460: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
+0000e470: 6e20 6f66 2061 6d6f 6e67 2d63 6f6c 756d  n of among-colum
+0000e480: 6e20 636f 7661 7269 616e 6365 206d 6174  n covariance mat
+0000e490: 7269 782e 2045 7861 6374 6c79 206f 6e65  rix. Exactly one
+0000e4a0: 0a20 2020 2020 2020 206f 6620 636f 6c63  .        of colc
+0000e4b0: 6f76 206f 7220 636f 6c63 686f 6c20 6973  ov or colchol is
+0000e4c0: 206e 6565 6465 642e 0a0a 2020 2020 4578   needed...    Ex
+0000e4d0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0000e4e0: 2d2d 2d0a 2020 2020 4465 6669 6e65 2061  ---.    Define a
+0000e4f0: 206d 6174 7269 7876 6172 6961 7465 206e   matrixvariate n
+0000e500: 6f72 6d61 6c20 7661 7269 6162 6c65 2066  ormal variable f
+0000e510: 6f72 2067 6976 656e 2072 6f77 2061 6e64  or given row and
+0000e520: 2063 6f6c 756d 6e20 636f 7661 7269 616e   column covarian
+0000e530: 6365 0a20 2020 206d 6174 7269 6365 733a  ce.    matrices:
+0000e540: 3a0a 0a20 2020 2020 2020 2063 6f6c 636f  :..        colco
+0000e550: 7620 3d20 6e70 2e61 7272 6179 285b 5b31  v = np.array([[1
+0000e560: 2e2c 2030 2e35 5d2c 205b 302e 352c 2032  ., 0.5], [0.5, 2
+0000e570: 5d5d 290a 2020 2020 2020 2020 726f 7763  ]]).        rowc
+0000e580: 6f76 203d 206e 702e 6172 7261 7928 5b5b  ov = np.array([[
+0000e590: 312c 2030 2c20 305d 2c20 5b30 2c20 342c  1, 0, 0], [0, 4,
+0000e5a0: 2030 5d2c 205b 302c 2030 2c20 3136 5d5d   0], [0, 0, 16]]
+0000e5b0: 290a 2020 2020 2020 2020 6d20 3d20 726f  ).        m = ro
+0000e5c0: 7763 6f76 2e73 6861 7065 5b30 5d0a 2020  wcov.shape[0].  
+0000e5d0: 2020 2020 2020 6e20 3d20 636f 6c63 6f76        n = colcov
+0000e5e0: 2e73 6861 7065 5b30 5d0a 2020 2020 2020  .shape[0].      
+0000e5f0: 2020 6d75 203d 206e 702e 7a65 726f 7328    mu = np.zeros(
+0000e600: 286d 2c20 6e29 290a 2020 2020 2020 2020  (m, n)).        
+0000e610: 7661 6c73 203d 2070 6d2e 4d61 7472 6978  vals = pm.Matrix
+0000e620: 4e6f 726d 616c 2827 7661 6c73 272c 206d  Normal('vals', m
+0000e630: 753d 6d75 2c20 636f 6c63 6f76 3d63 6f6c  u=mu, colcov=col
+0000e640: 636f 762c 0a20 2020 2020 2020 2020 2020  cov,.           
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 726f 7763 6f76 3d72 6f77 636f      rowcov=rowco
+0000e670: 7629 0a0a 2020 2020 4162 6f76 652c 2074  v)..    Above, t
+0000e680: 6865 2069 7468 2072 6f77 2069 6e20 7661  he ith row in va
+0000e690: 6c73 2068 6173 2061 2076 6172 6961 6e63  ls has a varianc
+0000e6a0: 6520 7468 6174 2069 7320 7363 616c 6564  e that is scaled
+0000e6b0: 2062 7920 345e 692e 0a20 2020 2041 6c74   by 4^i..    Alt
+0000e6c0: 6572 6e61 7469 7665 6c79 2c20 726f 7720  ernatively, row 
+0000e6d0: 6f72 2063 6f6c 756d 6e20 6368 6f6c 6573  or column choles
+0000e6e0: 6b79 206d 6174 7269 6365 7320 636f 756c  ky matrices coul
+0000e6f0: 6420 6265 2073 7562 7374 6974 7574 6564  d be substituted
+0000e700: 2066 6f72 0a20 2020 2065 6974 6865 7220   for.    either 
+0000e710: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000e720: 782e 2054 6865 204d 6174 7269 784e 6f72  x. The MatrixNor
+0000e730: 6d61 6c20 6973 2071 7569 636b 6572 2077  mal is quicker w
+0000e740: 6179 2063 6f6d 7075 7465 0a20 2020 204d  ay compute.    M
+0000e750: 764e 6f72 6d61 6c28 6d75 2c20 6e70 2e6b  vNormal(mu, np.k
+0000e760: 726f 6e28 726f 7763 6f76 2c20 636f 6c63  ron(rowcov, colc
+0000e770: 6f76 2929 2074 6861 7420 7461 6b65 7320  ov)) that takes 
+0000e780: 6164 7661 6e74 6167 6520 6f66 206b 726f  advantage of kro
+0000e790: 6e65 636b 6572 2070 726f 6475 6374 0a20  necker product. 
+0000e7a0: 2020 2070 726f 7065 7274 6965 7320 666f     properties fo
+0000e7b0: 7220 696e 7665 7273 696f 6e2e 2046 6f72  r inversion. For
+0000e7c0: 2065 7861 6d70 6c65 2c20 6966 2064 7261   example, if dra
+0000e7d0: 7773 2066 726f 6d20 4d76 4e6f 726d 616c  ws from MvNormal
+0000e7e0: 2068 6164 2074 6865 2073 616d 650a 2020   had the same.  
+0000e7f0: 2020 636f 7661 7269 616e 6365 2073 7472    covariance str
+0000e800: 7563 7475 7265 2c20 6275 7420 7765 7265  ucture, but were
+0000e810: 2073 6361 6c65 6420 6279 2064 6966 6665   scaled by diffe
+0000e820: 7265 6e74 2070 6f77 6572 7320 6f66 2061  rent powers of a
+0000e830: 6e20 756e 6b6e 6f77 6e0a 2020 2020 636f  n unknown.    co
+0000e840: 6e73 7461 6e74 2c20 626f 7468 2074 6865  nstant, both the
+0000e850: 2063 6f76 6172 6961 6e63 6520 616e 6420   covariance and 
+0000e860: 7363 616c 696e 6720 636f 756c 6420 6265  scaling could be
+0000e870: 206c 6561 726e 6564 2061 7320 666f 6c6c   learned as foll
+0000e880: 6f77 730a 2020 2020 2873 6565 2074 6865  ows.    (see the
+0000e890: 2064 6f63 7374 7269 6e67 206f 6620 604c   docstring of `L
+0000e8a0: 4b4a 4368 6f6c 6573 6b79 436f 7660 2066  KJCholeskyCov` f
+0000e8b0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+0000e8c0: 696f 6e20 6162 6f75 7420 7468 6973 290a  ion about this).
+0000e8d0: 0a20 2020 202e 2e20 636f 6465 3a3a 2070  .    .. code:: p
+0000e8e0: 7974 686f 6e0a 0a20 2020 2020 2020 2023  ython..        #
+0000e8f0: 2053 6574 7570 2064 6174 610a 2020 2020   Setup data.    
+0000e900: 2020 2020 7472 7565 5f63 6f6c 636f 7620      true_colcov 
+0000e910: 3d20 6e70 2e61 7272 6179 285b 5b31 2e30  = np.array([[1.0
+0000e920: 2c20 302e 352c 2030 2e31 5d2c 0a20 2020  , 0.5, 0.1],.   
+0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e940: 2020 2020 2020 2020 2020 2020 205b 302e               [0.
+0000e950: 352c 2031 2e30 2c20 302e 325d 2c0a 2020  5, 1.0, 0.2],.  
+0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e970: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
+0000e980: 2e31 2c20 302e 322c 2031 2e30 5d5d 290a  .1, 0.2, 1.0]]).
+0000e990: 2020 2020 2020 2020 6d20 3d20 330a 2020          m = 3.  
+0000e9a0: 2020 2020 2020 6e20 3d20 7472 7565 5f63        n = true_c
+0000e9b0: 6f6c 636f 762e 7368 6170 655b 305d 0a20  olcov.shape[0]. 
+0000e9c0: 2020 2020 2020 2074 7275 655f 7363 616c         true_scal
+0000e9d0: 6520 3d20 330a 2020 2020 2020 2020 7472  e = 3.        tr
+0000e9e0: 7565 5f72 6f77 636f 7620 3d20 6e70 2e64  ue_rowcov = np.d
+0000e9f0: 6961 6728 5b74 7275 655f 7363 616c 652a  iag([true_scale*
+0000ea00: 2a28 322a 6929 2066 6f72 2069 2069 6e20  *(2*i) for i in 
+0000ea10: 7261 6e67 6528 6d29 5d29 0a20 2020 2020  range(m)]).     
+0000ea20: 2020 206d 7520 3d20 6e70 2e7a 6572 6f73     mu = np.zeros
+0000ea30: 2828 6d2c 206e 2929 0a20 2020 2020 2020  ((m, n)).       
+0000ea40: 2074 7275 655f 6b72 6f6e 203d 206e 702e   true_kron = np.
+0000ea50: 6b72 6f6e 2874 7275 655f 726f 7763 6f76  kron(true_rowcov
+0000ea60: 2c20 7472 7565 5f63 6f6c 636f 7629 0a20  , true_colcov). 
+0000ea70: 2020 2020 2020 2064 6174 6120 3d20 6e70         data = np
+0000ea80: 2e72 616e 646f 6d2e 6d75 6c74 6976 6172  .random.multivar
+0000ea90: 6961 7465 5f6e 6f72 6d61 6c28 6d75 2e66  iate_normal(mu.f
+0000eaa0: 6c61 7474 656e 2829 2c20 7472 7565 5f6b  latten(), true_k
+0000eab0: 726f 6e29 0a20 2020 2020 2020 2064 6174  ron).        dat
+0000eac0: 6120 3d20 6461 7461 2e72 6573 6861 7065  a = data.reshape
+0000ead0: 286d 2c20 6e29 0a0a 2020 2020 2020 2020  (m, n)..        
+0000eae0: 7769 7468 2070 6d2e 4d6f 6465 6c28 2920  with pm.Model() 
+0000eaf0: 6173 206d 6f64 656c 3a0a 2020 2020 2020  as model:.      
+0000eb00: 2020 2020 2020 2320 5365 7475 7020 7269        # Setup ri
+0000eb10: 6768 7420 6368 6f6c 6573 6b79 206d 6174  ght cholesky mat
+0000eb20: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
+0000eb30: 7364 5f64 6973 7420 3d20 706d 2e48 616c  sd_dist = pm.Hal
+0000eb40: 6643 6175 6368 792e 6469 7374 2862 6574  fCauchy.dist(bet
+0000eb50: 613d 322e 352c 2073 6861 7065 3d33 290a  a=2.5, shape=3).
+0000eb60: 2020 2020 2020 2020 2020 2020 636f 6c63              colc
+0000eb70: 686f 6c5f 7061 636b 6564 203d 2070 6d2e  hol_packed = pm.
+0000eb80: 4c4b 4a43 686f 6c65 736b 7943 6f76 2827  LKJCholeskyCov('
+0000eb90: 636f 6c63 686f 6c70 6163 6b65 6427 2c20  colcholpacked', 
+0000eba0: 6e3d 332c 2065 7461 3d32 2c0a 2020 2020  n=3, eta=2,.    
 0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebd0: 2020 206f 6273 6572 7665 643d 6461 7461     observed=data
-0000ebe0: 290a 2020 2020 2222 220a 2020 2020 7276  ).    """.    rv
-0000ebf0: 5f6f 7020 3d20 6d61 7472 6978 6e6f 726d  _op = matrixnorm
-0000ec00: 616c 0a0a 2020 2020 4063 6c61 7373 6d65  al..    @classme
-0000ec10: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
-0000ec20: 7428 0a20 2020 2020 2020 2063 6c73 2c0a  t(.        cls,.
-0000ec30: 2020 2020 2020 2020 6d75 2c0a 2020 2020          mu,.    
-0000ec40: 2020 2020 726f 7763 6f76 3d4e 6f6e 652c      rowcov=None,
-0000ec50: 0a20 2020 2020 2020 2072 6f77 6368 6f6c  .        rowchol
-0000ec60: 3d4e 6f6e 652c 0a20 2020 2020 2020 2063  =None,.        c
-0000ec70: 6f6c 636f 763d 4e6f 6e65 2c0a 2020 2020  olcov=None,.    
-0000ec80: 2020 2020 636f 6c63 686f 6c3d 4e6f 6e65      colchol=None
-0000ec90: 2c0a 2020 2020 2020 2020 2a61 7267 732c  ,.        *args,
-0000eca0: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
-0000ecb0: 732c 0a20 2020 2029 3a0a 2020 2020 2020  s,.    ):.      
-0000ecc0: 2020 6368 6f6c 6573 6b79 203d 2043 686f    cholesky = Cho
-0000ecd0: 6c65 736b 7928 6c6f 7765 723d 5472 7565  lesky(lower=True
-0000ece0: 2c20 6f6e 5f65 7272 6f72 3d22 7261 6973  , on_error="rais
-0000ecf0: 6522 290a 0a20 2020 2020 2020 2023 2041  e")..        # A
-0000ed00: 6d6f 6e67 2d72 6f77 206d 6174 7269 6365  mong-row matrice
-0000ed10: 730a 2020 2020 2020 2020 6966 206c 656e  s.        if len
-0000ed20: 285b 6920 666f 7220 6920 696e 205b 726f  ([i for i in [ro
-0000ed30: 7763 6f76 2c20 726f 7763 686f 6c5d 2069  wcov, rowchol] i
-0000ed40: 6620 6920 6973 206e 6f74 204e 6f6e 655d  f i is not None]
-0000ed50: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
-0000ed60: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000ed70: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000ed80: 2020 2020 2020 2249 6e63 6f6d 7061 7469        "Incompati
-0000ed90: 626c 6520 7061 7261 6d65 7465 7269 7a61  ble parameteriza
-0000eda0: 7469 6f6e 2e20 5370 6563 6966 7920 6578  tion. Specify ex
-0000edb0: 6163 746c 7920 6f6e 6520 6f66 2072 6f77  actly one of row
-0000edc0: 636f 762c 206f 7220 726f 7763 686f 6c2e  cov, or rowchol.
-0000edd0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-0000ede0: 2020 2020 2020 2020 6966 2072 6f77 636f          if rowco
-0000edf0: 7620 6973 206e 6f74 204e 6f6e 653a 0a20  v is not None:. 
-0000ee00: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
-0000ee10: 7763 6f76 2e6e 6469 6d20 213d 2032 3a0a  wcov.ndim != 2:.
-0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000ee40: 2822 726f 7763 6f76 206d 7573 7420 6265  ("rowcov must be
-0000ee50: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
-0000ee60: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0000ee70: 726f 7763 686f 6c5f 636f 7620 3d20 6368  rowchol_cov = ch
-0000ee80: 6f6c 6573 6b79 2872 6f77 636f 7629 0a20  olesky(rowcov). 
-0000ee90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000eea0: 2020 2020 2020 2020 2069 6620 726f 7763           if rowc
-0000eeb0: 686f 6c2e 6e64 696d 2021 3d20 323a 0a20  hol.ndim != 2:. 
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000eed0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000eee0: 2272 6f77 6368 6f6c 206d 7573 7420 6265  "rowchol must be
-0000eef0: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
-0000ef00: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0000ef10: 726f 7763 686f 6c5f 636f 7620 3d20 7074  rowchol_cov = pt
-0000ef20: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
-0000ef30: 626c 6528 726f 7763 686f 6c29 0a0a 2020  ble(rowchol)..  
-0000ef40: 2020 2020 2020 2320 416d 6f6e 672d 636f        # Among-co
-0000ef50: 6c75 6d6e 206d 6174 7269 6365 730a 2020  lumn matrices.  
-0000ef60: 2020 2020 2020 6966 206c 656e 285b 6920        if len([i 
-0000ef70: 666f 7220 6920 696e 205b 636f 6c63 6f76  for i in [colcov
-0000ef80: 2c20 636f 6c63 686f 6c5d 2069 6620 6920  , colchol] if i 
-0000ef90: 6973 206e 6f74 204e 6f6e 655d 2920 213d  is not None]) !=
-0000efa0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0000efb0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000efc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000efd0: 2020 2249 6e63 6f6d 7061 7469 626c 6520    "Incompatible 
-0000efe0: 7061 7261 6d65 7465 7269 7a61 7469 6f6e  parameterization
-0000eff0: 2e20 5370 6563 6966 7920 6578 6163 746c  . Specify exactl
-0000f000: 7920 6f6e 6520 6f66 2063 6f6c 636f 762c  y one of colcov,
-0000f010: 206f 7220 636f 6c63 686f 6c2e 220a 2020   or colchol.".  
-0000f020: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000f030: 2020 2020 6966 2063 6f6c 636f 7620 6973      if colcov is
-0000f040: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000f050: 2020 2020 2020 2063 6f6c 636f 7620 3d20         colcov = 
-0000f060: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
-0000f070: 6961 626c 6528 636f 6c63 6f76 290a 2020  iable(colcov).  
-0000f080: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
-0000f090: 636f 762e 6e64 696d 2021 3d20 323a 0a20  cov.ndim != 2:. 
-0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f0b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000f0c0: 2263 6f6c 636f 7620 6d75 7374 2062 6520  "colcov must be 
-0000f0d0: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
-0000f0e0: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
-0000f0f0: 6f6c 6368 6f6c 5f63 6f76 203d 2063 686f  olchol_cov = cho
-0000f100: 6c65 736b 7928 636f 6c63 6f76 290a 2020  lesky(colcov).  
-0000f110: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000f120: 2020 2020 2020 2020 6966 2063 6f6c 6368          if colch
-0000f130: 6f6c 2e6e 6469 6d20 213d 2032 3a0a 2020  ol.ndim != 2:.  
-0000f140: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000f150: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-0000f160: 636f 6c63 686f 6c20 6d75 7374 2062 6520  colchol must be 
-0000f170: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
-0000f180: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
-0000f190: 6f6c 6368 6f6c 5f63 6f76 203d 2070 742e  olchol_cov = pt.
-0000f1a0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-0000f1b0: 6c65 2863 6f6c 6368 6f6c 290a 0a20 2020  le(colchol)..   
-0000f1c0: 2020 2020 2064 6973 745f 7368 6170 6520       dist_shape 
-0000f1d0: 3d20 2872 6f77 6368 6f6c 5f63 6f76 2e73  = (rowchol_cov.s
-0000f1e0: 6861 7065 5b2d 315d 2c20 636f 6c63 686f  hape[-1], colcho
-0000f1f0: 6c5f 636f 762e 7368 6170 655b 2d31 5d29  l_cov.shape[-1])
-0000f200: 0a0a 2020 2020 2020 2020 2320 4272 6f61  ..        # Broa
-0000f210: 6463 6173 7469 6e67 206d 750a 2020 2020  dcasting mu.    
-0000f220: 2020 2020 6d75 203d 2070 742e 6578 7472      mu = pt.extr
-0000f230: 615f 6f70 732e 6272 6f61 6463 6173 745f  a_ops.broadcast_
-0000f240: 746f 286d 752c 2073 6861 7065 3d64 6973  to(mu, shape=dis
-0000f250: 745f 7368 6170 6529 0a20 2020 2020 2020  t_shape).       
-0000f260: 206d 7520 3d20 7074 2e61 735f 7465 6e73   mu = pt.as_tens
-0000f270: 6f72 5f76 6172 6961 626c 6528 666c 6f61  or_variable(floa
-0000f280: 7458 286d 7529 290a 0a20 2020 2020 2020  tX(mu))..       
-0000f290: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-0000f2a0: 6469 7374 285b 6d75 2c20 726f 7763 686f  dist([mu, rowcho
-0000f2b0: 6c5f 636f 762c 2063 6f6c 6368 6f6c 5f63  l_cov, colchol_c
-0000f2c0: 6f76 5d2c 202a 2a6b 7761 7267 7329 0a0a  ov], **kwargs)..
-0000f2d0: 2020 2020 6465 6620 6d6f 6d65 6e74 2872      def moment(r
-0000f2e0: 762c 2073 697a 652c 206d 752c 2072 6f77  v, size, mu, row
-0000f2f0: 6368 6f6c 2c20 636f 6c63 686f 6c29 3a0a  chol, colchol):.
-0000f300: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0000f310: 742e 6675 6c6c 5f6c 696b 6528 7276 2c20  t.full_like(rv, 
-0000f320: 6d75 290a 0a20 2020 2064 6566 206c 6f67  mu)..    def log
-0000f330: 7028 7661 6c75 652c 206d 752c 2072 6f77  p(value, mu, row
-0000f340: 6368 6f6c 2c20 636f 6c63 686f 6c29 3a0a  chol, colchol):.
-0000f350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f360: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
-0000f370: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
-0000f380: 204d 6174 7269 782d 7661 6c75 6564 204e   Matrix-valued N
-0000f390: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
-0000f3a0: 6f6e 0a20 2020 2020 2020 2061 7420 7370  on.        at sp
-0000f3b0: 6563 6966 6965 6420 7661 6c75 652e 0a0a  ecified value...
-0000f3c0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000f3d0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000f3e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
-0000f3f0: 6c75 653a 206e 756d 6572 6963 0a20 2020  lue: numeric.   
-0000f400: 2020 2020 2020 2020 2056 616c 7565 2066           Value f
-0000f410: 6f72 2077 6869 6368 206c 6f67 2d70 726f  or which log-pro
-0000f420: 6261 6269 6c69 7479 2069 7320 6361 6c63  bability is calc
-0000f430: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
-0000f440: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0000f450: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000f460: 2054 656e 736f 7256 6172 6961 626c 650a   TensorVariable.
-0000f470: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000f480: 2020 2020 2069 6620 7661 6c75 652e 6e64       if value.nd
-0000f490: 696d 2021 3d20 323a 0a20 2020 2020 2020  im != 2:.       
-0000f4a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000f4b0: 4572 726f 7228 2256 616c 7565 206d 7573  Error("Value mus
-0000f4c0: 7420 6265 2074 776f 2064 696d 656e 7369  t be two dimensi
-0000f4d0: 6f6e 616c 2e22 290a 0a20 2020 2020 2020  onal.")..       
-0000f4e0: 2023 2043 6f6d 7075 7465 2054 725b 636f   # Compute Tr[co
-0000f4f0: 6c63 6f76 5e2d 3120 4020 2878 202d 206d  lcov^-1 @ (x - m
-0000f500: 7529 2e54 2040 2072 6f77 636f 765e 2d31  u).T @ rowcov^-1
-0000f510: 2040 2028 7820 2d20 6d75 295d 2061 6e64   @ (x - mu)] and
-0000f520: 0a20 2020 2020 2020 2023 2074 6865 206c  .        # the l
-0000f530: 6f67 6465 7420 6f66 2063 6f6c 636f 7620  ogdet of colcov 
-0000f540: 616e 6420 726f 7763 6f76 2e0a 2020 2020  and rowcov..    
-0000f550: 2020 2020 6465 6c74 6120 3d20 7661 6c75      delta = valu
-0000f560: 6520 2d20 6d75 0a0a 2020 2020 2020 2020  e - mu..        
-0000f570: 2320 4669 6e64 2065 7870 6f6e 656e 7420  # Find exponent 
-0000f580: 7069 6563 6520 6279 2070 6965 6365 0a20  piece by piece. 
-0000f590: 2020 2020 2020 2072 6967 6874 5f71 7561         right_qua
-0000f5a0: 6464 6973 7420 3d20 736f 6c76 655f 6c6f  ddist = solve_lo
-0000f5b0: 7765 7228 726f 7763 686f 6c2c 2064 656c  wer(rowchol, del
-0000f5c0: 7461 290a 2020 2020 2020 2020 7175 6164  ta).        quad
-0000f5d0: 6469 7374 203d 2070 742e 6e6c 696e 616c  dist = pt.nlinal
-0000f5e0: 672e 6d61 7472 6978 5f64 6f74 2872 6967  g.matrix_dot(rig
-0000f5f0: 6874 5f71 7561 6464 6973 742e 542c 2072  ht_quaddist.T, r
-0000f600: 6967 6874 5f71 7561 6464 6973 7429 0a20  ight_quaddist). 
-0000f610: 2020 2020 2020 2071 7561 6464 6973 7420         quaddist 
-0000f620: 3d20 736f 6c76 655f 6c6f 7765 7228 636f  = solve_lower(co
-0000f630: 6c63 686f 6c2c 2071 7561 6464 6973 7429  lchol, quaddist)
-0000f640: 0a20 2020 2020 2020 2071 7561 6464 6973  .        quaddis
-0000f650: 7420 3d20 736f 6c76 655f 7570 7065 7228  t = solve_upper(
-0000f660: 636f 6c63 686f 6c2e 542c 2071 7561 6464  colchol.T, quadd
-0000f670: 6973 7429 0a20 2020 2020 2020 2074 7271  ist).        trq
-0000f680: 7561 6464 6973 7420 3d20 7074 2e6e 6c69  uaddist = pt.nli
-0000f690: 6e61 6c67 2e74 7261 6365 2871 7561 6464  nalg.trace(quadd
-0000f6a0: 6973 7429 0a0a 2020 2020 2020 2020 636f  ist)..        co
-0000f6b0: 6c64 6961 6720 3d20 7074 2e64 6961 6728  ldiag = pt.diag(
-0000f6c0: 636f 6c63 686f 6c29 0a20 2020 2020 2020  colchol).       
-0000f6d0: 2072 6f77 6469 6167 203d 2070 742e 6469   rowdiag = pt.di
-0000f6e0: 6167 2872 6f77 6368 6f6c 290a 2020 2020  ag(rowchol).    
-0000f6f0: 2020 2020 6861 6c66 5f63 6f6c 6c6f 6764      half_collogd
-0000f700: 6574 203d 2070 742e 7375 6d28 7074 2e6c  et = pt.sum(pt.l
-0000f710: 6f67 2863 6f6c 6469 6167 2929 2020 2320  og(coldiag))  # 
-0000f720: 6c6f 6764 6574 284d 2920 3d20 322a 5472  logdet(M) = 2*Tr
-0000f730: 286c 6f67 284c 2929 0a20 2020 2020 2020  (log(L)).       
-0000f740: 2068 616c 665f 726f 776c 6f67 6465 7420   half_rowlogdet 
-0000f750: 3d20 7074 2e73 756d 2870 742e 6c6f 6728  = pt.sum(pt.log(
-0000f760: 726f 7764 6961 6729 2920 2023 2055 7369  rowdiag))  # Usi
-0000f770: 6e67 2043 686f 6c65 736b 793a 204d 203d  ng Cholesky: M =
-0000f780: 204c 204c 5e54 0a0a 2020 2020 2020 2020   L L^T..        
-0000f790: 6d20 3d20 726f 7763 686f 6c2e 7368 6170  m = rowchol.shap
-0000f7a0: 655b 305d 0a20 2020 2020 2020 206e 203d  e[0].        n =
-0000f7b0: 2063 6f6c 6368 6f6c 2e73 6861 7065 5b30   colchol.shape[0
-0000f7c0: 5d0a 0a20 2020 2020 2020 206e 6f72 6d20  ]..        norm 
-0000f7d0: 3d20 2d30 2e35 202a 206d 202a 206e 202a  = -0.5 * m * n *
-0000f7e0: 2070 6d2e 666c 6f61 7458 286e 702e 6c6f   pm.floatX(np.lo
-0000f7f0: 6728 3220 2a20 6e70 2e70 6929 290a 2020  g(2 * np.pi)).  
-0000f800: 2020 2020 2020 7265 7475 726e 206e 6f72        return nor
-0000f810: 6d20 2d20 302e 3520 2a20 7472 7175 6164  m - 0.5 * trquad
-0000f820: 6469 7374 202d 206d 202a 2068 616c 665f  dist - m * half_
-0000f830: 636f 6c6c 6f67 6465 7420 2d20 6e20 2a20  collogdet - n * 
-0000f840: 6861 6c66 5f72 6f77 6c6f 6764 6574 0a0a  half_rowlogdet..
-0000f850: 0a63 6c61 7373 204b 726f 6e65 636b 6572  .class Kronecker
-0000f860: 4e6f 726d 616c 5256 2852 616e 646f 6d56  NormalRV(RandomV
-0000f870: 6172 6961 626c 6529 3a0a 2020 2020 6e61  ariable):.    na
-0000f880: 6d65 203d 2022 6b72 6f6e 6563 6b65 726e  me = "kroneckern
-0000f890: 6f72 6d61 6c22 0a20 2020 206e 6469 6d5f  ormal".    ndim_
-0000f8a0: 7375 7070 203d 2031 0a20 2020 206e 6469  supp = 1.    ndi
-0000f8b0: 6d73 5f70 6172 616d 7320 3d20 5b31 2c20  ms_params = [1, 
-0000f8c0: 302c 2032 5d0a 2020 2020 6474 7970 6520  0, 2].    dtype 
-0000f8d0: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
-0000f8e0: 7072 696e 745f 6e61 6d65 203d 2028 224b  print_name = ("K
-0000f8f0: 726f 6e65 636b 6572 4e6f 726d 616c 222c  roneckerNormal",
-0000f900: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-0000f910: 7b4b 726f 6e65 636b 6572 4e6f 726d 616c  {KroneckerNormal
-0000f920: 7d22 290a 0a20 2020 2064 6566 2072 6e67  }")..    def rng
-0000f930: 5f66 6e28 7365 6c66 2c20 726e 672c 206d  _fn(self, rng, m
-0000f940: 752c 2073 6967 6d61 2c20 2a63 6f76 732c  u, sigma, *covs,
-0000f950: 2073 697a 653d 4e6f 6e65 293a 0a20 2020   size=None):.   
-0000f960: 2020 2020 2073 697a 6520 3d20 7369 7a65       size = size
-0000f970: 2069 6620 7369 7a65 2065 6c73 6520 636f   if size else co
-0000f980: 7673 5b2d 315d 0a20 2020 2020 2020 2063  vs[-1].        c
-0000f990: 6f76 7320 3d20 636f 7673 5b3a 2d31 5d20  ovs = covs[:-1] 
-0000f9a0: 6966 2063 6f76 735b 2d31 5d20 3d3d 2073  if covs[-1] == s
-0000f9b0: 697a 6520 656c 7365 2063 6f76 730a 0a20  ize else covs.. 
-0000f9c0: 2020 2020 2020 2063 6f76 203d 2072 6564         cov = red
-0000f9d0: 7563 6528 6c69 6e61 6c67 2e6b 726f 6e2c  uce(linalg.kron,
-0000f9e0: 2063 6f76 7329 0a0a 2020 2020 2020 2020   covs)..        
-0000f9f0: 6966 2073 6967 6d61 3a0a 2020 2020 2020  if sigma:.      
-0000fa00: 2020 2020 2020 636f 7620 3d20 636f 7620        cov = cov 
-0000fa10: 2b20 7369 676d 612a 2a32 202a 206e 702e  + sigma**2 * np.
-0000fa20: 6579 6528 636f 762e 7368 6170 655b 305d  eye(cov.shape[0]
-0000fa30: 290a 0a20 2020 2020 2020 2078 203d 206d  )..        x = m
-0000fa40: 756c 7469 7661 7269 6174 655f 6e6f 726d  ultivariate_norm
-0000fa50: 616c 2e72 6e67 5f66 6e28 726e 673d 726e  al.rng_fn(rng=rn
-0000fa60: 672c 206d 6561 6e3d 6d75 2c20 636f 763d  g, mean=mu, cov=
-0000fa70: 636f 762c 2073 697a 653d 7369 7a65 290a  cov, size=size).
-0000fa80: 2020 2020 2020 2020 7265 7475 726e 2078          return x
-0000fa90: 0a0a 0a6b 726f 6e65 636b 6572 6e6f 726d  ...kroneckernorm
-0000faa0: 616c 203d 204b 726f 6e65 636b 6572 4e6f  al = KroneckerNo
-0000fab0: 726d 616c 5256 2829 0a0a 0a63 6c61 7373  rmalRV()...class
-0000fac0: 204b 726f 6e65 636b 6572 4e6f 726d 616c   KroneckerNormal
-0000fad0: 2843 6f6e 7469 6e75 6f75 7329 3a0a 2020  (Continuous):.  
-0000fae0: 2020 7222 2222 0a20 2020 204d 756c 7469    r""".    Multi
-0000faf0: 7661 7269 6174 6520 6e6f 726d 616c 206c  variate normal l
-0000fb00: 6f67 2d6c 696b 656c 6968 6f6f 6420 7769  og-likelihood wi
-0000fb10: 7468 204b 726f 6e65 636b 6572 2d73 7472  th Kronecker-str
-0000fb20: 7563 7475 7265 6420 636f 7661 7269 616e  uctured covarian
-0000fb30: 6365 2e0a 0a20 2020 202e 2e20 6d61 7468  ce...    .. math
-0000fb40: 3a3a 0a0a 2020 2020 2020 2066 2878 205c  ::..       f(x \
-0000fb50: 6d69 6420 5c6d 752c 204b 2920 3d0a 2020  mid \mu, K) =.  
-0000fb60: 2020 2020 2020 2020 205c 6672 6163 7b31           \frac{1
-0000fb70: 7d7b 2832 5c70 6920 7c4b 7c29 5e7b 312f  }{(2\pi |K|)^{1/
-0000fb80: 327d 7d0a 2020 2020 2020 2020 2020 205c  2}}.           \
-0000fb90: 6578 705c 6c65 6674 5c7b 202d 5c66 7261  exp\left\{ -\fra
-0000fba0: 637b 317d 7b32 7d20 2878 2d5c 6d75 295e  c{1}{2} (x-\mu)^
-0000fbb0: 7b5c 7072 696d 657d 204b 5e7b 2d31 7d20  {\prime} K^{-1} 
-0000fbc0: 2878 2d5c 6d75 2920 5c72 6967 6874 5c7d  (x-\mu) \right\}
-0000fbd0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  ..    ========  
-0000fbe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fbf0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
-0000fc00: 7570 706f 7274 2020 203a 6d61 7468 3a60  upport   :math:`
-0000fc10: 7820 5c69 6e20 5c6d 6174 6862 627b 527d  x \in \mathbb{R}
-0000fc20: 5e4e 600a 2020 2020 4d65 616e 2020 2020  ^N`.    Mean    
-0000fc30: 2020 3a6d 6174 683a 605c 6d75 600a 2020    :math:`\mu`.  
-0000fc40: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
-0000fc50: 683a 604b 203d 205c 6269 676f 7469 6d65  h:`K = \bigotime
-0000fc60: 7320 4b5f 6920 2b20 5c73 6967 6d61 5e32  s K_i + \sigma^2
-0000fc70: 2049 5f4e 600a 2020 2020 3d3d 3d3d 3d3d   I_N`.    ======
-0000fc80: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
-0000fc90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-0000fca0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000fcb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000fcc0: 2020 6d75 203a 2074 656e 736f 725f 6c69    mu : tensor_li
-0000fcd0: 6b65 206f 6620 666c 6f61 740a 2020 2020  ke of float.    
-0000fce0: 2020 2020 5665 6374 6f72 206f 6620 6d65      Vector of me
-0000fcf0: 616e 732c 206a 7573 7420 6173 2069 6e20  ans, just as in 
-0000fd00: 604d 764e 6f72 6d61 6c60 2e0a 2020 2020  `MvNormal`..    
-0000fd10: 636f 7673 203a 206c 6973 7420 6f66 2061  covs : list of a
-0000fd20: 7272 6179 730a 2020 2020 2020 2020 5468  rrays.        Th
-0000fd30: 6520 7365 7420 6f66 2063 6f76 6172 6961  e set of covaria
-0000fd40: 6e63 6520 6d61 7472 6963 6573 203a 6d61  nce matrices :ma
-0000fd50: 7468 3a60 5b4b 5f31 2c20 4b5f 322c 202e  th:`[K_1, K_2, .
-0000fd60: 2e2e 5d60 2074 6f20 6265 0a20 2020 2020  ..]` to be.     
-0000fd70: 2020 204b 726f 6e65 636b 6572 6564 2069     Kroneckered i
-0000fd80: 6e20 7468 6520 6f72 6465 7220 7072 6f76  n the order prov
-0000fd90: 6964 6564 203a 6d61 7468 3a60 5c62 6967  ided :math:`\big
-0000fda0: 6f74 696d 6573 204b 5f69 602e 0a20 2020  otimes K_i`..   
-0000fdb0: 2063 686f 6c73 203a 206c 6973 7420 6f66   chols : list of
-0000fdc0: 2061 7272 6179 730a 2020 2020 2020 2020   arrays.        
-0000fdd0: 5468 6520 7365 7420 6f66 206c 6f77 6572  The set of lower
-0000fde0: 2063 686f 6c65 736b 7920 6d61 7472 6963   cholesky matric
-0000fdf0: 6573 203a 6d61 7468 3a60 5b4c 5f31 2c20  es :math:`[L_1, 
-0000fe00: 4c5f 322c 202e 2e2e 5d60 2073 7563 6820  L_2, ...]` such 
-0000fe10: 7468 6174 0a20 2020 2020 2020 203a 6d61  that.        :ma
-0000fe20: 7468 3a60 4b5f 6920 3d20 4c5f 6920 4c5f  th:`K_i = L_i L_
-0000fe30: 6927 602e 0a20 2020 2065 7664 7320 3a20  i'`..    evds : 
-0000fe40: 6c69 7374 206f 6620 7475 706c 6573 0a20  list of tuples. 
-0000fe50: 2020 2020 2020 2054 6865 2073 6574 206f         The set o
-0000fe60: 6620 6569 6765 6e76 616c 7565 2d76 6563  f eigenvalue-vec
-0000fe70: 746f 722c 2065 6967 656e 7665 6374 6f72  tor, eigenvector
-0000fe80: 2d6d 6174 7269 7820 7061 6972 730a 2020  -matrix pairs.  
-0000fe90: 2020 2020 2020 3a6d 6174 683a 605b 2876        :math:`[(v
-0000fea0: 5f31 2c20 515f 3129 2c20 2876 5f32 2c20  _1, Q_1), (v_2, 
-0000feb0: 515f 3229 2c20 2e2e 2e5d 6020 7375 6368  Q_2), ...]` such
-0000fec0: 2074 6861 740a 2020 2020 2020 2020 3a6d   that.        :m
-0000fed0: 6174 683a 604b 5f69 203d 2051 5f69 205c  ath:`K_i = Q_i \
-0000fee0: 7465 7874 7b64 6961 677d 2876 5f69 2920  text{diag}(v_i) 
-0000fef0: 515f 6927 602e 2046 6f72 2065 7861 6d70  Q_i'`. For examp
-0000ff00: 6c65 3a3a 0a0a 2020 2020 2020 2020 2020  le::..          
-0000ff10: 2020 765f 692c 2051 5f69 203d 2070 742e    v_i, Q_i = pt.
-0000ff20: 6e6c 696e 616c 672e 6569 6768 284b 5f69  nlinalg.eigh(K_i
-0000ff30: 290a 2020 2020 7369 676d 6120 3a20 7363  ).    sigma : sc
-0000ff40: 616c 6172 2c20 6f70 7469 6f6e 616c 0a20  alar, optional. 
-0000ff50: 2020 2020 2020 2053 7461 6e64 6172 6420         Standard 
-0000ff60: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
-0000ff70: 2047 6175 7373 6961 6e20 7768 6974 6520   Gaussian white 
-0000ff80: 6e6f 6973 652e 0a0a 2020 2020 4578 616d  noise...    Exam
-0000ff90: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-0000ffa0: 2d0a 2020 2020 4465 6669 6e65 2061 206d  -.    Define a m
-0000ffb0: 756c 7469 7661 7269 6174 6520 6e6f 726d  ultivariate norm
-0000ffc0: 616c 2076 6172 6961 626c 6520 7769 7468  al variable with
-0000ffd0: 2061 2063 6f76 6172 6961 6e63 650a 2020   a covariance.  
-0000ffe0: 2020 3a6d 6174 683a 604b 203d 204b 5f31    :math:`K = K_1
-0000fff0: 205c 6f74 696d 6573 204b 5f32 600a 0a20   \otimes K_2`.. 
-00010000: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
-00010010: 686f 6e0a 0a20 2020 2020 2020 204b 3120  hon..        K1 
-00010020: 3d20 6e70 2e61 7272 6179 285b 5b31 2e2c  = np.array([[1.,
-00010030: 2030 2e35 5d2c 205b 302e 352c 2032 5d5d   0.5], [0.5, 2]]
-00010040: 290a 2020 2020 2020 2020 4b32 203d 206e  ).        K2 = n
-00010050: 702e 6172 7261 7928 5b5b 312e 2c20 302e  p.array([[1., 0.
-00010060: 342c 2030 2e32 5d2c 205b 302e 342c 2032  4, 0.2], [0.4, 2
-00010070: 2c20 302e 335d 2c20 5b30 2e32 2c20 302e  , 0.3], [0.2, 0.
-00010080: 332c 2031 5d5d 290a 2020 2020 2020 2020  3, 1]]).        
-00010090: 636f 7673 203d 205b 4b31 2c20 4b32 5d0a  covs = [K1, K2].
-000100a0: 2020 2020 2020 2020 4e20 3d20 360a 2020          N = 6.  
-000100b0: 2020 2020 2020 6d75 203d 206e 702e 7a65        mu = np.ze
-000100c0: 726f 7328 4e29 0a20 2020 2020 2020 2077  ros(N).        w
-000100d0: 6974 6820 706d 2e4d 6f64 656c 2829 2061  ith pm.Model() a
-000100e0: 7320 6d6f 6465 6c3a 0a20 2020 2020 2020  s model:.       
-000100f0: 2020 2020 2076 616c 7320 3d20 706d 2e4b       vals = pm.K
-00010100: 726f 6e65 636b 6572 4e6f 726d 616c 2827  roneckerNormal('
-00010110: 7661 6c73 272c 206d 753d 6d75 2c20 636f  vals', mu=mu, co
-00010120: 7673 3d63 6f76 732c 2073 6861 7065 3d4e  vs=covs, shape=N
-00010130: 290a 0a20 2020 2045 6666 6963 6965 6e63  )..    Efficienc
-00010140: 7920 6761 696e 7320 6172 6520 6d61 6465  y gains are made
-00010150: 2062 7920 6368 6f6c 6573 6b79 2064 6563   by cholesky dec
-00010160: 6f6d 706f 7369 6e67 203a 6d61 7468 3a60  omposing :math:`
-00010170: 4b5f 3160 2061 6e64 0a20 2020 203a 6d61  K_1` and.    :ma
-00010180: 7468 3a60 4b5f 3260 2069 6e64 6976 6964  th:`K_2` individ
-00010190: 7561 6c6c 7920 7261 7468 6572 2074 6861  ually rather tha
-000101a0: 6e20 7468 6520 6c61 7267 6572 203a 6d61  n the larger :ma
-000101b0: 7468 3a60 4b60 206d 6174 7269 782e 2041  th:`K` matrix. A
-000101c0: 6c74 686f 7567 680a 2020 2020 6f6e 6c79  lthough.    only
-000101d0: 2074 776f 206d 6174 7269 6365 7320 3a6d   two matrices :m
-000101e0: 6174 683a 604b 5f31 6020 616e 6420 3a6d  ath:`K_1` and :m
-000101f0: 6174 683a 604b 5f32 6020 6172 6520 7368  ath:`K_2` are sh
-00010200: 6f77 6e20 6865 7265 2c20 616e 2061 7262  own here, an arb
-00010210: 6974 7261 7279 0a20 2020 206e 756d 6265  itrary.    numbe
-00010220: 7220 6f66 2073 7562 6d61 7472 6963 6573  r of submatrices
-00010230: 2063 616e 2062 6520 636f 6d62 696e 6564   can be combined
-00010240: 2069 6e20 7468 6973 2077 6179 2e20 4368   in this way. Ch
-00010250: 6f6c 6573 6b79 7320 616e 640a 2020 2020  oleskys and.    
-00010260: 6569 6765 6e64 6563 6f6d 706f 7369 7469  eigendecompositi
-00010270: 6f6e 7320 6361 6e20 6265 2070 726f 7669  ons can be provi
-00010280: 6465 6420 696e 7374 6561 640a 0a20 2020  ded instead..   
-00010290: 202e 2e20 636f 6465 3a3a 2070 7974 686f   .. code:: pytho
-000102a0: 6e0a 0a20 2020 2020 2020 2063 686f 6c73  n..        chols
-000102b0: 203d 205b 6e70 2e6c 696e 616c 672e 6368   = [np.linalg.ch
-000102c0: 6f6c 6573 6b79 284b 6929 2066 6f72 204b  olesky(Ki) for K
-000102d0: 6920 696e 2063 6f76 735d 0a20 2020 2020  i in covs].     
-000102e0: 2020 2065 7664 7320 3d20 5b6e 702e 6c69     evds = [np.li
-000102f0: 6e61 6c67 2e65 6967 6828 4b69 2920 666f  nalg.eigh(Ki) fo
-00010300: 7220 4b69 2069 6e20 636f 7673 5d0a 2020  r Ki in covs].  
-00010310: 2020 2020 2020 7769 7468 2070 6d2e 4d6f        with pm.Mo
-00010320: 6465 6c28 2920 6173 206d 6f64 656c 3a0a  del() as model:.
-00010330: 2020 2020 2020 2020 2020 2020 7661 6c73              vals
-00010340: 3220 3d20 706d 2e4b 726f 6e65 636b 6572  2 = pm.Kronecker
-00010350: 4e6f 726d 616c 2827 7661 6c73 3227 2c20  Normal('vals2', 
-00010360: 6d75 3d6d 752c 2063 686f 6c73 3d63 686f  mu=mu, chols=cho
-00010370: 6c73 2c20 7368 6170 653d 4e29 0a20 2020  ls, shape=N).   
-00010380: 2020 2020 2020 2020 2023 206f 720a 2020           # or.  
-00010390: 2020 2020 2020 2020 2020 7661 6c73 3320            vals3 
-000103a0: 3d20 706d 2e4b 726f 6e65 636b 6572 4e6f  = pm.KroneckerNo
-000103b0: 726d 616c 2827 7661 6c73 3327 2c20 6d75  rmal('vals3', mu
-000103c0: 3d6d 752c 2065 7664 733d 6576 6473 2c20  =mu, evds=evds, 
-000103d0: 7368 6170 653d 4e29 0a0a 2020 2020 6e65  shape=N)..    ne
-000103e0: 6974 6865 7220 6f66 2077 6869 6368 2077  ither of which w
-000103f0: 696c 6c20 6265 2063 6f6e 7665 7274 6564  ill be converted
-00010400: 2e20 4469 6167 6f6e 616c 206e 6f69 7365  . Diagonal noise
-00010410: 2063 616e 2061 6c73 6f20 6265 2061 6464   can also be add
-00010420: 6564 2074 6f0a 2020 2020 7468 6520 636f  ed to.    the co
-00010430: 7661 7269 616e 6365 206d 6174 7269 782c  variance matrix,
-00010440: 203a 6d61 7468 3a60 4b20 3d20 4b5f 3120   :math:`K = K_1 
-00010450: 5c6f 7469 6d65 7320 4b5f 3220 2b20 5c73  \otimes K_2 + \s
-00010460: 6967 6d61 5e32 2049 5f4e 602e 0a20 2020  igma^2 I_N`..   
-00010470: 2044 6573 7069 7465 2074 6865 206e 6f69   Despite the noi
-00010480: 7365 2072 656d 6f76 696e 6720 7468 6520  se removing the 
-00010490: 6f76 6572 616c 6c20 4b72 6f6e 6563 6b65  overall Kronecke
-000104a0: 7220 7374 7275 6374 7572 6520 6f66 2074  r structure of t
-000104b0: 6865 206d 6174 7269 782c 0a20 2020 2060  he matrix,.    `
-000104c0: 4b72 6f6e 6563 6b65 724e 6f72 6d61 6c60  KroneckerNormal`
-000104d0: 2063 616e 2063 6f6e 7469 6e75 6520 746f   can continue to
-000104e0: 206d 616b 6520 6566 6669 6369 656e 7420   make efficient 
-000104f0: 6361 6c63 756c 6174 696f 6e73 2062 790a  calculations by.
-00010500: 2020 2020 7574 696c 697a 696e 6720 6569      utilizing ei
-00010510: 6765 6e64 6563 6f6d 706f 7369 746f 6e73  gendecompositons
-00010520: 206f 6620 7468 6520 7375 626d 6174 7269   of the submatri
-00010530: 6365 7320 6265 6869 6e64 2074 6865 2073  ces behind the s
-00010540: 6365 6e65 7320 5b31 5d2e 0a20 2020 2054  cenes [1]..    T
-00010550: 6875 732c 0a0a 2020 2020 2e2e 2063 6f64  hus,..    .. cod
-00010560: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00010570: 2020 2020 7369 676d 6120 3d20 302e 310a      sigma = 0.1.
-00010580: 2020 2020 2020 2020 7769 7468 2070 6d2e          with pm.
-00010590: 4d6f 6465 6c28 2920 6173 206e 6f69 7365  Model() as noise
-000105a0: 5f6d 6f64 656c 3a0a 2020 2020 2020 2020  _model:.        
-000105b0: 2020 2020 7661 6c73 203d 2070 6d2e 4b72      vals = pm.Kr
-000105c0: 6f6e 6563 6b65 724e 6f72 6d61 6c28 2776  oneckerNormal('v
-000105d0: 616c 7327 2c20 6d75 3d6d 752c 2063 6f76  als', mu=mu, cov
-000105e0: 733d 636f 7673 2c20 7369 676d 613d 7369  s=covs, sigma=si
-000105f0: 676d 612c 2073 6861 7065 3d4e 290a 2020  gma, shape=N).  
-00010600: 2020 2020 2020 2020 2020 7661 6c73 3220            vals2 
-00010610: 3d20 706d 2e4b 726f 6e65 636b 6572 4e6f  = pm.KroneckerNo
-00010620: 726d 616c 2827 7661 6c73 3227 2c20 6d75  rmal('vals2', mu
-00010630: 3d6d 752c 2063 686f 6c73 3d63 686f 6c73  =mu, chols=chols
-00010640: 2c20 7369 676d 613d 7369 676d 612c 2073  , sigma=sigma, s
-00010650: 6861 7065 3d4e 290a 2020 2020 2020 2020  hape=N).        
-00010660: 2020 2020 7661 6c73 3320 3d20 706d 2e4b      vals3 = pm.K
-00010670: 726f 6e65 636b 6572 4e6f 726d 616c 2827  roneckerNormal('
-00010680: 7661 6c73 3327 2c20 6d75 3d6d 752c 2065  vals3', mu=mu, e
-00010690: 7664 733d 6576 6473 2c20 7369 676d 613d  vds=evds, sigma=
-000106a0: 7369 676d 612c 2073 6861 7065 3d4e 290a  sigma, shape=N).
-000106b0: 0a20 2020 2061 7265 2069 6465 6e74 6963  .    are identic
-000106c0: 616c 2c20 7769 7468 2060 636f 7673 6020  al, with `covs` 
-000106d0: 616e 6420 6063 686f 6c73 6020 6561 6368  and `chols` each
-000106e0: 2063 6f6e 7665 7274 6564 2074 6f0a 2020   converted to.  
-000106f0: 2020 6569 6765 6e64 6563 6f6d 706f 7369    eigendecomposi
-00010700: 7469 6f6e 732e 0a0a 2020 2020 5265 6665  tions...    Refe
-00010710: 7265 6e63 6573 0a20 2020 202d 2d2d 2d2d  rences.    -----
-00010720: 2d2d 2d2d 2d0a 2020 2020 2e2e 205b 315d  -----.    .. [1]
-00010730: 2053 6161 7463 6869 2c20 592e 2028 3230   Saatchi, Y. (20
-00010740: 3131 292e 2022 5363 616c 6162 6c65 2069  11). "Scalable i
-00010750: 6e66 6572 656e 6365 2066 6f72 2073 7472  nference for str
-00010760: 7563 7475 7265 6420 4761 7573 7369 616e  uctured Gaussian
-00010770: 2070 726f 6365 7373 206d 6f64 656c 7322   process models"
-00010780: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
-00010790: 6f70 203d 206b 726f 6e65 636b 6572 6e6f  op = kroneckerno
-000107a0: 726d 616c 0a0a 2020 2020 4063 6c61 7373  rmal..    @class
-000107b0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-000107c0: 6973 7428 636c 732c 206d 752c 2063 6f76  ist(cls, mu, cov
-000107d0: 733d 4e6f 6e65 2c20 6368 6f6c 733d 4e6f  s=None, chols=No
-000107e0: 6e65 2c20 6576 6473 3d4e 6f6e 652c 2073  ne, evds=None, s
-000107f0: 6967 6d61 3d4e 6f6e 652c 202a 6172 6773  igma=None, *args
-00010800: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00010810: 2020 2020 2069 6620 6c65 6e28 5b69 2066       if len([i f
-00010820: 6f72 2069 2069 6e20 5b63 6f76 732c 2063  or i in [covs, c
-00010830: 686f 6c73 2c20 6576 6473 5d20 6966 2069  hols, evds] if i
-00010840: 2069 7320 6e6f 7420 4e6f 6e65 5d29 2021   is not None]) !
-00010850: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00010860: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00010870: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00010880: 2020 2022 496e 636f 6d70 6174 6962 6c65     "Incompatible
-00010890: 2070 6172 616d 6574 6572 697a 6174 696f   parameterizatio
-000108a0: 6e2e 2053 7065 6369 6679 2065 7861 6374  n. Specify exact
-000108b0: 6c79 206f 6e65 206f 6620 636f 7673 2c20  ly one of covs, 
-000108c0: 6368 6f6c 732c 206f 7220 6576 6473 2e22  chols, or evds."
-000108d0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000108e0: 2020 2020 2020 2020 7369 676d 6120 3d20          sigma = 
-000108f0: 7369 676d 6120 6966 2073 6967 6d61 2065  sigma if sigma e
-00010900: 6c73 6520 300a 0a20 2020 2020 2020 2069  lse 0..        i
-00010910: 6620 6368 6f6c 7320 6973 206e 6f74 204e  f chols is not N
-00010920: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00010930: 2063 6f76 7320 3d20 5b63 686f 6c2e 646f   covs = [chol.do
-00010940: 7428 6368 6f6c 2e54 2920 666f 7220 6368  t(chol.T) for ch
-00010950: 6f6c 2069 6e20 6368 6f6c 735d 0a20 2020  ol in chols].   
-00010960: 2020 2020 2065 6c69 6620 6576 6473 2069       elif evds i
-00010970: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00010980: 2020 2020 2020 2020 6569 6768 5f69 7465          eigh_ite
-00010990: 7261 626c 6520 3d20 6576 6473 0a20 2020  rable = evds.   
-000109a0: 2020 2020 2020 2020 2063 6f76 7320 3d20           covs = 
-000109b0: 5b5d 0a20 2020 2020 2020 2020 2020 2065  [].            e
-000109c0: 6967 735f 7365 702c 2051 7320 3d20 7a69  igs_sep, Qs = zi
-000109d0: 7028 2a65 6967 685f 6974 6572 6162 6c65  p(*eigh_iterable
-000109e0: 2920 2023 2055 6e7a 6970 0a20 2020 2020  )  # Unzip.     
-000109f0: 2020 2020 2020 2066 6f72 2065 6967 2c20         for eig, 
-00010a00: 5120 696e 207a 6970 2865 6967 735f 7365  Q in zip(eigs_se
-00010a10: 702c 2051 7329 3a0a 2020 2020 2020 2020  p, Qs):.        
-00010a20: 2020 2020 2020 2020 636f 765f 6920 3d20          cov_i = 
-00010a30: 7074 2e64 6f74 2851 2c20 7074 2e64 6f74  pt.dot(Q, pt.dot
-00010a40: 2870 742e 6469 6167 2865 6967 292c 2051  (pt.diag(eig), Q
-00010a50: 2e54 2929 0a20 2020 2020 2020 2020 2020  .T)).           
-00010a60: 2020 2020 2063 6f76 732e 6170 7065 6e64       covs.append
-00010a70: 2863 6f76 5f69 290a 0a20 2020 2020 2020  (cov_i)..       
-00010a80: 206d 7520 3d20 7074 2e61 735f 7465 6e73   mu = pt.as_tens
-00010a90: 6f72 5f76 6172 6961 626c 6528 6d75 290a  or_variable(mu).
-00010aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010ab0: 7375 7065 7228 292e 6469 7374 285b 6d75  super().dist([mu
-00010ac0: 2c20 7369 676d 612c 202a 636f 7673 5d2c  , sigma, *covs],
-00010ad0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-00010ae0: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
-00010af0: 697a 652c 206d 752c 2063 6f76 732c 2063  ize, mu, covs, c
-00010b00: 686f 6c73 2c20 6576 6473 293a 0a20 2020  hols, evds):.   
-00010b10: 2020 2020 206d 6561 6e20 3d20 6d75 0a20       mean = mu. 
-00010b20: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
-00010b30: 5f73 697a 655f 6973 5f6e 6f6e 6528 7369  _size_is_none(si
-00010b40: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
-00010b50: 206d 6f6d 656e 745f 7369 7a65 203d 2070   moment_size = p
-00010b60: 742e 636f 6e63 6174 656e 6174 6528 5b73  t.concatenate([s
-00010b70: 697a 652c 206d 752e 7368 6170 655d 290a  ize, mu.shape]).
-00010b80: 2020 2020 2020 2020 2020 2020 6d65 616e              mean
-00010b90: 203d 2070 742e 6675 6c6c 286d 6f6d 656e   = pt.full(momen
-00010ba0: 745f 7369 7a65 2c20 6d75 290a 2020 2020  t_size, mu).    
-00010bb0: 2020 2020 7265 7475 726e 206d 6561 6e0a      return mean.
-00010bc0: 0a20 2020 2064 6566 206c 6f67 7028 7661  .    def logp(va
-00010bd0: 6c75 652c 206d 752c 2073 6967 6d61 2c20  lue, mu, sigma, 
-00010be0: 2a63 6f76 7329 3a0a 2020 2020 2020 2020  *covs):.        
-00010bf0: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
-00010c00: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
-00010c10: 696c 6974 7920 6f66 204d 756c 7469 7661  ility of Multiva
-00010c20: 7269 6174 6520 4e6f 726d 616c 2064 6973  riate Normal dis
-00010c30: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
-00010c40: 2020 7769 7468 204b 726f 6e65 636b 6572    with Kronecker
-00010c50: 2d73 7472 7563 7475 7265 6420 636f 7661  -structured cova
-00010c60: 7269 616e 6365 2061 7420 7370 6563 6966  riance at specif
-00010c70: 6965 6420 7661 6c75 652e 0a0a 2020 2020  ied value...    
-00010c80: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00010c90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00010ca0: 2d0a 2020 2020 2020 2020 7661 6c75 653a  -.        value:
-00010cb0: 206e 756d 6572 6963 0a20 2020 2020 2020   numeric.       
-00010cc0: 2020 2020 2056 616c 7565 2066 6f72 2077       Value for w
-00010cd0: 6869 6368 206c 6f67 2d70 726f 6261 6269  hich log-probabi
-00010ce0: 6c69 7479 2069 7320 6361 6c63 756c 6174  lity is calculat
-00010cf0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
-00010d00: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00010d10: 2d2d 2d2d 0a20 2020 2020 2020 2054 656e  ----.        Ten
-00010d20: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
-00010d30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010d40: 2320 436f 6d70 7574 6573 2074 6865 2071  # Computes the q
-00010d50: 7561 6472 6174 6963 2028 782d 6d75 295e  uadratic (x-mu)^
-00010d60: 5420 4020 4b5e 2d31 2040 2028 782d 6d75  T @ K^-1 @ (x-mu
-00010d70: 2920 616e 6420 6c6f 6728 6465 7428 4b29  ) and log(det(K)
-00010d80: 290a 2020 2020 2020 2020 6966 2076 616c  ).        if val
-00010d90: 7565 2e6e 6469 6d20 3e20 3220 6f72 2076  ue.ndim > 2 or v
-00010da0: 616c 7565 2e6e 6469 6d20 3d3d 2030 3a0a  alue.ndim == 0:.
-00010db0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00010dc0: 6520 5661 6c75 6545 7272 6f72 2866 2249  e ValueError(f"I
-00010dd0: 6e76 616c 6964 2064 696d 656e 7369 6f6e  nvalid dimension
-00010de0: 2066 6f72 2076 616c 7565 3a20 7b76 616c   for value: {val
-00010df0: 7565 2e6e 6469 6d7d 2229 0a20 2020 2020  ue.ndim}").     
-00010e00: 2020 2069 6620 7661 6c75 652e 6e64 696d     if value.ndim
-00010e10: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-00010e20: 2020 206f 6e65 6469 6d20 3d20 5472 7565     onedim = True
-00010e30: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00010e40: 7565 203d 2076 616c 7565 5b4e 6f6e 652c  ue = value[None,
-00010e50: 203a 5d0a 2020 2020 2020 2020 656c 7365   :].        else
-00010e60: 3a0a 2020 2020 2020 2020 2020 2020 6f6e  :.            on
-00010e70: 6564 696d 203d 2046 616c 7365 0a0a 2020  edim = False..  
-00010e80: 2020 2020 2020 6465 6c74 6120 3d20 7661        delta = va
-00010e90: 6c75 6520 2d20 6d75 0a0a 2020 2020 2020  lue - mu..      
-00010ea0: 2020 6569 6768 5f69 7465 7261 626c 6520    eigh_iterable 
-00010eb0: 3d20 6d61 7028 6569 6768 2c20 636f 7673  = map(eigh, covs
-00010ec0: 290a 2020 2020 2020 2020 6569 6773 5f73  ).        eigs_s
-00010ed0: 6570 2c20 5173 203d 207a 6970 282a 6569  ep, Qs = zip(*ei
-00010ee0: 6768 5f69 7465 7261 626c 6529 2020 2320  gh_iterable)  # 
-00010ef0: 556e 7a69 700a 2020 2020 2020 2020 5173  Unzip.        Qs
-00010f00: 203d 206c 6973 7428 6d61 7028 7074 2e61   = list(map(pt.a
-00010f10: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-00010f20: 652c 2051 7329 290a 2020 2020 2020 2020  e, Qs)).        
-00010f30: 5154 7320 3d20 6c69 7374 286d 6170 2870  QTs = list(map(p
-00010f40: 742e 7472 616e 7370 6f73 652c 2051 7329  t.transpose, Qs)
-00010f50: 290a 0a20 2020 2020 2020 2065 6967 735f  )..        eigs_
-00010f60: 7365 7020 3d20 6c69 7374 286d 6170 2870  sep = list(map(p
-00010f70: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00010f80: 6162 6c65 2c20 6569 6773 5f73 6570 2929  able, eigs_sep))
-00010f90: 0a20 2020 2020 2020 2065 6967 7320 3d20  .        eigs = 
-00010fa0: 6b72 6f6e 5f64 6961 6728 2a65 6967 735f  kron_diag(*eigs_
-00010fb0: 7365 7029 2020 2320 436f 6d62 696e 6520  sep)  # Combine 
-00010fc0: 7365 7061 7261 7465 2065 6967 730a 2020  separate eigs.  
-00010fd0: 2020 2020 2020 6569 6773 202b 3d20 7369        eigs += si
-00010fe0: 676d 612a 2a32 0a20 2020 2020 2020 204e  gma**2.        N
-00010ff0: 203d 2065 6967 732e 7368 6170 655b 305d   = eigs.shape[0]
-00011000: 0a0a 2020 2020 2020 2020 7371 7274 5f71  ..        sqrt_q
-00011010: 7561 6420 3d20 6b72 6f6e 5f64 6f74 2851  uad = kron_dot(Q
-00011020: 5473 2c20 6465 6c74 612e 5429 0a20 2020  Ts, delta.T).   
-00011030: 2020 2020 2073 7172 745f 7175 6164 203d       sqrt_quad =
-00011040: 2073 7172 745f 7175 6164 202f 2070 742e   sqrt_quad / pt.
-00011050: 7371 7274 2865 6967 735b 3a2c 204e 6f6e  sqrt(eigs[:, Non
-00011060: 655d 290a 2020 2020 2020 2020 6c6f 6764  e]).        logd
-00011070: 6574 203d 2070 742e 7375 6d28 7074 2e6c  et = pt.sum(pt.l
-00011080: 6f67 2865 6967 7329 290a 0a20 2020 2020  og(eigs))..     
-00011090: 2020 2023 2053 7175 6172 6520 6561 6368     # Square each
-000110a0: 2073 616d 706c 650a 2020 2020 2020 2020   sample.        
-000110b0: 7175 6164 203d 2070 742e 6261 7463 6865  quad = pt.batche
-000110c0: 645f 646f 7428 7371 7274 5f71 7561 642e  d_dot(sqrt_quad.
-000110d0: 542c 2073 7172 745f 7175 6164 2e54 290a  T, sqrt_quad.T).
-000110e0: 2020 2020 2020 2020 6966 206f 6e65 6469          if onedi
-000110f0: 6d3a 0a20 2020 2020 2020 2020 2020 2071  m:.            q
-00011100: 7561 6420 3d20 7175 6164 5b30 5d0a 0a20  uad = quad[0].. 
-00011110: 2020 2020 2020 2061 203d 202d 2871 7561         a = -(qua
-00011120: 6420 2b20 6c6f 6764 6574 202b 204e 202a  d + logdet + N *
-00011130: 2070 742e 6c6f 6728 3220 2a20 6e70 2e70   pt.log(2 * np.p
-00011140: 6929 2920 2f20 322e 300a 2020 2020 2020  i)) / 2.0.      
-00011150: 2020 7265 7475 726e 2061 0a0a 0a63 6c61    return a...cla
-00011160: 7373 2043 4152 5256 2852 616e 646f 6d56  ss CARRV(RandomV
-00011170: 6172 6961 626c 6529 3a0a 2020 2020 6e61  ariable):.    na
-00011180: 6d65 203d 2022 6361 7222 0a20 2020 206e  me = "car".    n
-00011190: 6469 6d5f 7375 7070 203d 2031 0a20 2020  dim_supp = 1.   
-000111a0: 206e 6469 6d73 5f70 6172 616d 7320 3d20   ndims_params = 
-000111b0: 5b31 2c20 322c 2030 2c20 305d 0a20 2020  [1, 2, 0, 0].   
-000111c0: 2064 7479 7065 203d 2022 666c 6f61 7458   dtype = "floatX
-000111d0: 220a 2020 2020 5f70 7269 6e74 5f6e 616d  ".    _print_nam
-000111e0: 6520 3d20 2822 4341 5222 2c20 225c 5c6f  e = ("CAR", "\\o
-000111f0: 7065 7261 746f 726e 616d 657b 4341 527d  peratorname{CAR}
-00011200: 2229 0a0a 2020 2020 6465 6620 6d61 6b65  ")..    def make
-00011210: 5f6e 6f64 6528 7365 6c66 2c20 726e 672c  _node(self, rng,
-00011220: 2073 697a 652c 2064 7479 7065 2c20 6d75   size, dtype, mu
-00011230: 2c20 572c 2061 6c70 6861 2c20 7461 7529  , W, alpha, tau)
-00011240: 3a0a 2020 2020 2020 2020 6d75 203d 2070  :.        mu = p
-00011250: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00011260: 6162 6c65 2866 6c6f 6174 5828 6d75 2929  able(floatX(mu))
-00011270: 0a0a 2020 2020 2020 2020 5720 3d20 7079  ..        W = py
-00011280: 7465 6e73 6f72 2e73 7061 7273 652e 6173  tensor.sparse.as
-00011290: 5f73 7061 7273 655f 6f72 5f74 656e 736f  _sparse_or_tenso
-000112a0: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
-000112b0: 5828 5729 290a 2020 2020 2020 2020 6966  X(W)).        if
-000112c0: 206e 6f74 2057 2e6e 6469 6d20 3d3d 2032   not W.ndim == 2
-000112d0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000112e0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-000112f0: 5720 6d75 7374 2062 6520 6120 6d61 7472  W must be a matr
-00011300: 6978 2028 6e64 696d 3d32 292e 2229 0a0a  ix (ndim=2).")..
-00011310: 2020 2020 2020 2020 7370 6172 7365 203d          sparse =
-00011320: 2069 7369 6e73 7461 6e63 6528 572c 2070   isinstance(W, p
-00011330: 7974 656e 736f 722e 7370 6172 7365 2e53  ytensor.sparse.S
-00011340: 7061 7273 6556 6172 6961 626c 6529 0a20  parseVariable). 
-00011350: 2020 2020 2020 206d 7367 203d 2022 5720         msg = "W 
-00011360: 6d75 7374 2062 6520 6120 7379 6d6d 6574  must be a symmet
-00011370: 7269 6320 6164 6a61 6365 6e63 7920 6d61  ric adjacency ma
-00011380: 7472 6978 2e22 0a20 2020 2020 2020 2069  trix.".        i
-00011390: 6620 7370 6172 7365 3a0a 2020 2020 2020  f sparse:.      
-000113a0: 2020 2020 2020 6162 735f 6469 6666 203d        abs_diff =
-000113b0: 2070 7974 656e 736f 722e 7370 6172 7365   pytensor.sparse
-000113c0: 2e62 6173 6963 2e6d 756c 2870 7974 656e  .basic.mul(pyten
-000113d0: 736f 722e 7370 6172 7365 2e73 6967 6e28  sor.sparse.sign(
-000113e0: 5720 2d20 572e 5429 2c20 5720 2d20 572e  W - W.T), W - W.
-000113f0: 5429 0a20 2020 2020 2020 2020 2020 2057  T).            W
-00011400: 203d 2041 7373 6572 7428 6d73 6729 2857   = Assert(msg)(W
-00011410: 2c20 7074 2e69 7363 6c6f 7365 2870 7974  , pt.isclose(pyt
-00011420: 656e 736f 722e 7370 6172 7365 2e73 705f  ensor.sparse.sp_
-00011430: 7375 6d28 6162 735f 6469 6666 292c 2030  sum(abs_diff), 0
-00011440: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
-00011450: 0a20 2020 2020 2020 2020 2020 2057 203d  .            W =
-00011460: 2041 7373 6572 7428 6d73 6729 2857 2c20   Assert(msg)(W, 
-00011470: 7074 2e61 6c6c 636c 6f73 6528 572c 2057  pt.allclose(W, W
-00011480: 2e54 2929 0a0a 2020 2020 2020 2020 7461  .T))..        ta
-00011490: 7520 3d20 7074 2e61 735f 7465 6e73 6f72  u = pt.as_tensor
-000114a0: 5f76 6172 6961 626c 6528 666c 6f61 7458  _variable(floatX
-000114b0: 2874 6175 2929 0a20 2020 2020 2020 2061  (tau)).        a
-000114c0: 6c70 6861 203d 2070 742e 6173 5f74 656e  lpha = pt.as_ten
-000114d0: 736f 725f 7661 7269 6162 6c65 2866 6c6f  sor_variable(flo
-000114e0: 6174 5828 616c 7068 6129 290a 0a20 2020  atX(alpha))..   
-000114f0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00011500: 7228 292e 6d61 6b65 5f6e 6f64 6528 726e  r().make_node(rn
-00011510: 672c 2073 697a 652c 2064 7479 7065 2c20  g, size, dtype, 
-00011520: 6d75 2c20 572c 2061 6c70 6861 2c20 7461  mu, W, alpha, ta
-00011530: 7529 0a0a 2020 2020 6465 6620 5f69 6e66  u)..    def _inf
-00011540: 6572 5f73 6861 7065 2873 656c 662c 2073  er_shape(self, s
-00011550: 697a 652c 2064 6973 745f 7061 7261 6d73  ize, dist_params
-00011560: 2c20 7061 7261 6d5f 7368 6170 6573 3d4e  , param_shapes=N
-00011570: 6f6e 6529 3a0a 2020 2020 2020 2020 7368  one):.        sh
-00011580: 6170 6520 3d20 7475 706c 6528 7369 7a65  ape = tuple(size
-00011590: 2920 2b20 2864 6973 745f 7061 7261 6d73  ) + (dist_params
-000115a0: 5b30 5d2e 7368 6170 655b 2d31 5d2c 290a  [0].shape[-1],).
-000115b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000115c0: 6861 7065 0a0a 2020 2020 4063 6c61 7373  hape..    @class
-000115d0: 6d65 7468 6f64 0a20 2020 2064 6566 2072  method.    def r
-000115e0: 6e67 5f66 6e28 636c 732c 2072 6e67 3a20  ng_fn(cls, rng: 
-000115f0: 6e70 2e72 616e 646f 6d2e 5261 6e64 6f6d  np.random.Random
-00011600: 5374 6174 652c 206d 752c 2057 2c20 616c  State, mu, W, al
-00011610: 7068 612c 2074 6175 2c20 7369 7a65 293a  pha, tau, size):
-00011620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011630: 2020 2020 2049 6d70 6c65 6d65 6e74 6174       Implementat
-00011640: 696f 6e20 6f66 2061 6c67 6f72 6974 686d  ion of algorithm
-00011650: 2066 726f 6d20 7061 7065 720a 2020 2020   from paper.    
-00011660: 2020 2020 4861 7661 7264 2052 7565 2c20      Havard Rue, 
-00011670: 3230 3031 2e20 2246 6173 7420 7361 6d70  2001. "Fast samp
-00011680: 6c69 6e67 206f 6620 4761 7573 7369 616e  ling of Gaussian
-00011690: 204d 6172 6b6f 7620 7261 6e64 6f6d 2066   Markov random f
-000116a0: 6965 6c64 732c 220a 2020 2020 2020 2020  ields,".        
-000116b0: 4a6f 7572 6e61 6c20 6f66 2074 6865 2052  Journal of the R
-000116c0: 6f79 616c 2053 7461 7469 7374 6963 616c  oyal Statistical
-000116d0: 2053 6f63 6965 7479 2053 6572 6965 7320   Society Series 
-000116e0: 422c 2052 6f79 616c 2053 7461 7469 7374  B, Royal Statist
-000116f0: 6963 616c 2053 6f63 6965 7479 2c0a 2020  ical Society,.  
-00011700: 2020 2020 2020 766f 6c2e 2036 3328 3229        vol. 63(2)
-00011710: 2c20 7061 6765 7320 3332 352d 3333 382e  , pages 325-338.
-00011720: 2044 4f49 3a20 3130 2e31 3131 312f 3134   DOI: 10.1111/14
-00011730: 3637 2d39 3836 382e 3030 3238 380a 2020  67-9868.00288.  
-00011740: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011750: 2020 6966 206e 6f74 2073 6369 7079 2e73    if not scipy.s
-00011760: 7061 7273 652e 6973 7370 6172 7365 2857  parse.issparse(W
-00011770: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
-00011780: 203d 2073 6369 7079 2e73 7061 7273 652e   = scipy.sparse.
-00011790: 6373 725f 6d61 7472 6978 2857 290a 2020  csr_matrix(W).  
-000117a0: 2020 2020 2020 7320 3d20 6e70 2e61 7361        s = np.asa
-000117b0: 7272 6179 2857 2e73 756d 2861 7869 733d  rray(W.sum(axis=
-000117c0: 3029 295b 305d 0a20 2020 2020 2020 2044  0))[0].        D
-000117d0: 203d 2073 6369 7079 2e73 7061 7273 652e   = scipy.sparse.
-000117e0: 6469 6167 7328 7329 0a20 2020 2020 2020  diags(s).       
-000117f0: 2074 6175 203d 2073 6369 7079 2e73 7061   tau = scipy.spa
-00011800: 7273 652e 6373 725f 6d61 7472 6978 2874  rse.csr_matrix(t
-00011810: 6175 290a 2020 2020 2020 2020 616c 7068  au).        alph
-00011820: 6120 3d20 7363 6970 792e 7370 6172 7365  a = scipy.sparse
-00011830: 2e63 7372 5f6d 6174 7269 7828 616c 7068  .csr_matrix(alph
-00011840: 6129 0a0a 2020 2020 2020 2020 5120 3d20  a)..        Q = 
-00011850: 7461 752e 6d75 6c74 6970 6c79 2844 202d  tau.multiply(D -
-00011860: 2061 6c70 6861 2e6d 756c 7469 706c 7928   alpha.multiply(
-00011870: 5729 290a 0a20 2020 2020 2020 2070 6572  W))..        per
-00011880: 6d5f 6172 7261 7920 3d20 7363 6970 792e  m_array = scipy.
-00011890: 7370 6172 7365 2e63 7367 7261 7068 2e72  sparse.csgraph.r
-000118a0: 6576 6572 7365 5f63 7574 6869 6c6c 5f6d  everse_cuthill_m
-000118b0: 636b 6565 2851 2c20 7379 6d6d 6574 7269  ckee(Q, symmetri
-000118c0: 635f 6d6f 6465 3d54 7275 6529 0a20 2020  c_mode=True).   
-000118d0: 2020 2020 2069 6e76 5f70 6572 6d20 3d20       inv_perm = 
-000118e0: 6e70 2e61 7267 736f 7274 2870 6572 6d5f  np.argsort(perm_
-000118f0: 6172 7261 7929 0a0a 2020 2020 2020 2020  array)..        
-00011900: 5120 3d20 515b 7065 726d 5f61 7272 6179  Q = Q[perm_array
-00011910: 2c20 3a5d 5b3a 2c20 7065 726d 5f61 7272  , :][:, perm_arr
-00011920: 6179 5d0a 0a20 2020 2020 2020 2051 6220  ay]..        Qb 
-00011930: 3d20 512e 6469 6167 6f6e 616c 2829 0a20  = Q.diagonal(). 
-00011940: 2020 2020 2020 2075 203d 2031 0a20 2020         u = 1.   
-00011950: 2020 2020 2077 6869 6c65 206e 702e 636f       while np.co
-00011960: 756e 745f 6e6f 6e7a 6572 6f28 512e 6469  unt_nonzero(Q.di
-00011970: 6167 6f6e 616c 2875 2929 203e 2030 3a0a  agonal(u)) > 0:.
-00011980: 2020 2020 2020 2020 2020 2020 5162 203d              Qb =
-00011990: 206e 702e 7673 7461 636b 2828 6e70 2e70   np.vstack((np.p
-000119a0: 6164 2851 2e64 6961 676f 6e61 6c28 7529  ad(Q.diagonal(u)
-000119b0: 2c20 2875 2c20 3029 2c20 636f 6e73 7461  , (u, 0), consta
-000119c0: 6e74 5f76 616c 7565 733d 2830 2c20 3029  nt_values=(0, 0)
-000119d0: 292c 2051 6229 290a 2020 2020 2020 2020  ), Qb)).        
-000119e0: 2020 2020 7520 2b3d 2031 0a0a 2020 2020      u += 1..    
-000119f0: 2020 2020 4c20 3d20 7363 6970 792e 6c69      L = scipy.li
-00011a00: 6e61 6c67 2e63 686f 6c65 736b 795f 6261  nalg.cholesky_ba
-00011a10: 6e64 6564 2851 622c 206c 6f77 6572 3d46  nded(Qb, lower=F
-00011a20: 616c 7365 290a 0a20 2020 2020 2020 2073  alse)..        s
-00011a30: 697a 6520 3d20 7475 706c 6528 7369 7a65  ize = tuple(size
-00011a40: 206f 7220 2829 290a 2020 2020 2020 2020   or ()).        
-00011a50: 6966 2073 697a 653a 0a20 2020 2020 2020  if size:.       
-00011a60: 2020 2020 206d 7520 3d20 6e70 2e62 726f       mu = np.bro
-00011a70: 6164 6361 7374 5f74 6f28 6d75 2c20 7369  adcast_to(mu, si
-00011a80: 7a65 202b 2028 6d75 2e73 6861 7065 5b2d  ze + (mu.shape[-
-00011a90: 315d 2c29 290a 2020 2020 2020 2020 7a20  1],)).        z 
-00011aa0: 3d20 726e 672e 6e6f 726d 616c 2873 697a  = rng.normal(siz
-00011ab0: 653d 6d75 2e73 6861 7065 290a 2020 2020  e=mu.shape).    
-00011ac0: 2020 2020 7361 6d70 6c65 7320 3d20 6e70      samples = np
-00011ad0: 2e65 6d70 7479 287a 2e73 6861 7065 290a  .empty(z.shape).
-00011ae0: 2020 2020 2020 2020 666f 7220 6964 7820          for idx 
-00011af0: 696e 206e 702e 6e64 696e 6465 7828 6d75  in np.ndindex(mu
-00011b00: 2e73 6861 7065 5b3a 2d31 5d29 3a0a 2020  .shape[:-1]):.  
-00011b10: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
-00011b20: 735b 6964 785d 203d 2073 6369 7079 2e6c  s[idx] = scipy.l
-00011b30: 696e 616c 672e 6368 6f5f 736f 6c76 655f  inalg.cho_solve_
-00011b40: 6261 6e64 6564 2828 4c2c 2046 616c 7365  banded((L, False
-00011b50: 292c 207a 5b69 6478 5d29 202b 206d 755b  ), z[idx]) + mu[
-00011b60: 6964 785d 5b70 6572 6d5f 6172 7261 795d  idx][perm_array]
-00011b70: 0a20 2020 2020 2020 2073 616d 706c 6573  .        samples
-00011b80: 203d 2073 616d 706c 6573 5b2e 2e2e 2c20   = samples[..., 
-00011b90: 696e 765f 7065 726d 5d0a 2020 2020 2020  inv_perm].      
-00011ba0: 2020 7265 7475 726e 2073 616d 706c 6573    return samples
-00011bb0: 0a0a 0a63 6172 203d 2043 4152 5256 2829  ...car = CARRV()
-00011bc0: 0a0a 0a63 6c61 7373 2043 4152 2843 6f6e  ...class CAR(Con
-00011bd0: 7469 6e75 6f75 7329 3a0a 2020 2020 7222  tinuous):.    r"
-00011be0: 2222 0a20 2020 204c 696b 656c 6968 6f6f  "".    Likelihoo
-00011bf0: 6420 666f 7220 6120 636f 6e64 6974 696f  d for a conditio
-00011c00: 6e61 6c20 6175 746f 7265 6772 6573 7369  nal autoregressi
-00011c10: 6f6e 2e20 5468 6973 2069 7320 6120 7370  on. This is a sp
-00011c20: 6563 6961 6c20 6361 7365 206f 6620 7468  ecial case of th
-00011c30: 650a 2020 2020 6d75 6c74 6976 6172 6961  e.    multivaria
-00011c40: 7465 206e 6f72 6d61 6c20 7769 7468 2061  te normal with a
-00011c50: 6e20 6164 6a61 6365 6e63 792d 7374 7275  n adjacency-stru
-00011c60: 6374 7572 6564 2063 6f76 6172 6961 6e63  ctured covarianc
-00011c70: 6520 6d61 7472 6978 2e0a 0a20 2020 202e  e matrix...    .
-00011c80: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
-00011c90: 2066 2878 205c 6d69 6420 572c 205c 616c   f(x \mid W, \al
-00011ca0: 7068 612c 205c 7461 7529 203d 0a20 2020  pha, \tau) =.   
-00011cb0: 2020 2020 2020 2020 5c66 7261 637b 7c54          \frac{|T
-00011cc0: 7c5e 7b31 2f32 7d7d 7b28 325c 7069 295e  |^{1/2}}{(2\pi)^
-00011cd0: 7b6b 2f32 7d7d 0a20 2020 2020 2020 2020  {k/2}}.         
-00011ce0: 2020 5c65 7870 5c6c 6566 745c 7b20 2d5c    \exp\left\{ -\
-00011cf0: 6672 6163 7b31 7d7b 327d 2028 782d 5c6d  frac{1}{2} (x-\m
-00011d00: 7529 5e7b 5c70 7269 6d65 7d20 545e 7b2d  u)^{\prime} T^{-
-00011d10: 317d 2028 782d 5c6d 7529 205c 7269 6768  1} (x-\mu) \righ
-00011d20: 745c 7d0a 0a20 2020 2077 6865 7265 203a  t\}..    where :
-00011d30: 6d61 7468 3a60 5420 3d20 285c 7461 7520  math:`T = (\tau 
-00011d40: 4428 492d 5c61 6c70 6861 2057 2929 5e7b  D(I-\alpha W))^{
-00011d50: 2d31 7d60 2061 6e64 203a 6d61 7468 3a60  -1}` and :math:`
-00011d60: 4420 3d20 6469 6167 285c 7375 6d5f 6920  D = diag(\sum_i 
-00011d70: 575f 7b69 6a7d 2960 2e0a 0a20 2020 203d  W_{ij})`...    =
-00011d80: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
-00011d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011da0: 3d3d 3d0a 2020 2020 5375 7070 6f72 7420  ===.    Support 
-00011db0: 2020 3a6d 6174 683a 6078 205c 696e 205c    :math:`x \in \
-00011dc0: 6d61 7468 6262 7b52 7d5e 6b60 0a20 2020  mathbb{R}^k`.   
-00011dd0: 204d 6561 6e20 2020 2020 203a 6d61 7468   Mean      :math
-00011de0: 3a60 5c6d 7520 5c69 6e20 5c6d 6174 6862  :`\mu \in \mathb
-00011df0: 627b 527d 5e6b 600a 2020 2020 5661 7269  b{R}^k`.    Vari
-00011e00: 616e 6365 2020 3a6d 6174 683a 6028 5c74  ance  :math:`(\t
-00011e10: 6175 2044 2849 2d5c 616c 7068 6120 5729  au D(I-\alpha W)
-00011e20: 295e 7b2d 317d 600a 2020 2020 3d3d 3d3d  )^{-1}`.    ====
-00011e30: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
-00011e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011e50: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00011e60: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00011e70: 2020 2020 6d75 203a 2074 656e 736f 725f      mu : tensor_
-00011e80: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
-00011e90: 2020 2020 2020 5265 616c 2d76 616c 7565        Real-value
-00011ea0: 6420 6d65 616e 2076 6563 746f 720a 2020  d mean vector.  
-00011eb0: 2020 5720 3a20 284d 2c20 4d29 2074 656e    W : (M, M) ten
-00011ec0: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
-00011ed0: 2020 2020 2020 2020 5379 6d6d 6574 7269          Symmetri
-00011ee0: 6320 6164 6a61 6365 6e63 7920 6d61 7472  c adjacency matr
-00011ef0: 6978 206f 6620 3173 2061 6e64 2030 7320  ix of 1s and 0s 
-00011f00: 696e 6469 6361 7469 6e67 0a20 2020 2020  indicating.     
-00011f10: 2020 2061 646a 6163 656e 6379 2062 6574     adjacency bet
-00011f20: 7765 656e 2065 6c65 6d65 6e74 732e 2049  ween elements. I
-00011f30: 6620 706f 7373 6962 6c65 2c20 2a57 2a20  f possible, *W* 
-00011f40: 6973 2063 6f6e 7665 7274 6564 0a20 2020  is converted.   
-00011f50: 2020 2020 2074 6f20 6120 7370 6172 7365       to a sparse
-00011f60: 206d 6174 7269 782c 2066 616c 6c69 6e67   matrix, falling
-00011f70: 2062 6163 6b20 746f 2061 2064 656e 7365   back to a dense
-00011f80: 2076 6172 6961 626c 652e 0a20 2020 2020   variable..     
-00011f90: 2020 203a 6675 6e63 3a60 7e70 7974 656e     :func:`~pyten
-00011fa0: 736f 722e 7370 6172 7365 2e62 6173 6963  sor.sparse.basic
-00011fb0: 2e61 735f 7370 6172 7365 5f6f 725f 7465  .as_sparse_or_te
-00011fc0: 6e73 6f72 5f76 6172 6961 626c 6560 2069  nsor_variable` i
-00011fd0: 730a 2020 2020 2020 2020 7573 6564 2066  s.        used f
-00011fe0: 6f72 2074 6869 7320 7370 6172 7365 206f  or this sparse o
-00011ff0: 7220 7465 6e73 6f72 7661 7269 6162 6c65  r tensorvariable
-00012000: 2063 6f6e 7665 7273 696f 6e2e 0a20 2020   conversion..   
-00012010: 2061 6c70 6861 203a 2074 656e 736f 725f   alpha : tensor_
-00012020: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
-00012030: 2020 2020 2020 4175 746f 7265 6772 6573        Autoregres
-00012040: 7369 6f6e 2070 6172 616d 6574 6572 2074  sion parameter t
-00012050: 616b 696e 6720 7661 6c75 6573 2062 6574  aking values bet
-00012060: 7765 656e 202d 3120 616e 6420 312e 2056  ween -1 and 1. V
-00012070: 616c 7565 7320 636c 6f73 6572 2074 6f20  alues closer to 
-00012080: 3020 696e 6469 6361 7465 2077 6561 6b65  0 indicate weake
-00012090: 720a 2020 2020 2020 2020 636f 7272 656c  r.        correl
-000120a0: 6174 696f 6e20 616e 6420 7661 6c75 6573  ation and values
-000120b0: 2063 6c6f 7365 7220 746f 2031 2069 6e64   closer to 1 ind
-000120c0: 6963 6174 6520 6869 6768 6572 2061 7574  icate higher aut
-000120d0: 6f63 6f72 7265 6c61 7469 6f6e 2e20 466f  ocorrelation. Fo
-000120e0: 7220 6d6f 7374 2075 7365 2063 6173 6573  r most use cases
-000120f0: 2c20 7468 650a 2020 2020 2020 2020 7375  , the.        su
-00012100: 7070 6f72 7420 6f66 2061 6c70 6861 2073  pport of alpha s
-00012110: 686f 756c 6420 6265 2072 6573 7472 6963  hould be restric
-00012120: 7465 6420 746f 2028 302c 2031 292e 0a20  ted to (0, 1).. 
-00012130: 2020 2074 6175 203a 2074 656e 736f 725f     tau : tensor_
-00012140: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
-00012150: 2020 2020 2020 506f 7369 7469 7665 2070        Positive p
-00012160: 7265 6369 7369 6f6e 2076 6172 6961 626c  recision variabl
-00012170: 6520 636f 6e74 726f 6c6c 696e 6720 7468  e controlling th
-00012180: 6520 7363 616c 6520 6f66 2074 6865 2075  e scale of the u
-00012190: 6e64 6572 6c79 696e 6720 6e6f 726d 616c  nderlying normal
-000121a0: 2076 6172 6961 7465 732e 0a0a 2020 2020   variates...    
-000121b0: 5265 6665 7265 6e63 6573 0a20 2020 202d  References.    -
-000121c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e  ---------.    ..
-000121d0: 2020 4a69 6e2c 2058 2e2c 2043 6172 6c69    Jin, X., Carli
-000121e0: 6e2c 2042 2e2c 2042 616e 6572 6a65 652c  n, B., Banerjee,
-000121f0: 2053 2e0a 2020 2020 2020 2020 2247 656e   S..        "Gen
-00012200: 6572 616c 697a 6564 2048 6965 7261 7263  eralized Hierarc
-00012210: 6869 6361 6c20 4d75 6c74 6976 6172 6961  hical Multivaria
-00012220: 7465 2043 4152 204d 6f64 656c 7320 666f  te CAR Models fo
-00012230: 7220 4172 6561 6c20 4461 7461 220a 2020  r Areal Data".  
-00012240: 2020 2020 2020 4269 6f6d 6574 7269 6373        Biometrics
-00012250: 2c20 566f 6c2e 2036 312c 204e 6f2e 2034  , Vol. 61, No. 4
-00012260: 2028 4465 632e 2c20 3230 3035 292c 2070   (Dec., 2005), p
-00012270: 702e 2039 3530 2d39 3631 0a20 2020 2022  p. 950-961.    "
-00012280: 2222 0a20 2020 2072 765f 6f70 203d 2063  "".    rv_op = c
-00012290: 6172 0a0a 2020 2020 4063 6c61 7373 6d65  ar..    @classme
-000122a0: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
-000122b0: 7428 636c 732c 206d 752c 2057 2c20 616c  t(cls, mu, W, al
-000122c0: 7068 612c 2074 6175 2c20 2a61 7267 732c  pha, tau, *args,
-000122d0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-000122e0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-000122f0: 2829 2e64 6973 7428 5b6d 752c 2057 2c20  ().dist([mu, W, 
-00012300: 616c 7068 612c 2074 6175 5d2c 202a 2a6b  alpha, tau], **k
-00012310: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
-00012320: 6d6f 6d65 6e74 2872 762c 2073 697a 652c  moment(rv, size,
-00012330: 206d 752c 2057 2c20 616c 7068 612c 2074   mu, W, alpha, t
-00012340: 6175 293a 0a20 2020 2020 2020 2072 6574  au):.        ret
-00012350: 7572 6e20 7074 2e66 756c 6c5f 6c69 6b65  urn pt.full_like
-00012360: 2872 762c 206d 7529 0a0a 2020 2020 6465  (rv, mu)..    de
-00012370: 6620 6c6f 6770 2876 616c 7565 2c20 6d75  f logp(value, mu
-00012380: 2c20 572c 2061 6c70 6861 2c20 7461 7529  , W, alpha, tau)
-00012390: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000123a0: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
-000123b0: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
-000123c0: 6f66 2061 2043 4152 2d64 6973 7472 6962  of a CAR-distrib
-000123d0: 7574 6564 2076 6563 746f 720a 2020 2020  uted vector.    
-000123e0: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
-000123f0: 2076 616c 7565 2e20 5468 6973 206c 6f67   value. This log
-00012400: 2070 726f 6261 6269 6c69 7479 2066 756e   probability fun
-00012410: 6374 696f 6e20 6469 6666 6572 7320 6672  ction differs fr
-00012420: 6f6d 0a20 2020 2020 2020 2074 6865 2074  om.        the t
-00012430: 7275 6520 4341 5220 6c6f 6720 6465 6e73  rue CAR log dens
-00012440: 6974 7920 2841 4b41 2061 206d 756c 7469  ity (AKA a multi
-00012450: 7661 7269 6174 6520 6e6f 726d 616c 2077  variate normal w
-00012460: 6974 6820 4341 522d 7374 7275 6374 7572  ith CAR-structur
-00012470: 6564 0a20 2020 2020 2020 2063 6f76 6172  ed.        covar
-00012480: 6961 6e63 6520 6d61 7472 6978 2920 6279  iance matrix) by
-00012490: 2061 6e20 6164 6469 7469 7665 2063 6f6e   an additive con
-000124a0: 7374 616e 742e 0a0a 2020 2020 2020 2020  stant...        
-000124b0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-000124c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000124d0: 2020 2020 2020 7661 6c75 653a 2061 7272        value: arr
-000124e0: 6179 0a20 2020 2020 2020 2020 2020 2056  ay.            V
-000124f0: 616c 7565 2066 6f72 2077 6869 6368 206c  alue for which l
-00012500: 6f67 2d70 726f 6261 6269 6c69 7479 2069  og-probability i
-00012510: 7320 6361 6c63 756c 6174 6564 2e0a 0a20  s calculated... 
-00012520: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00012530: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00012540: 2020 2020 2020 2054 656e 736f 7256 6172         TensorVar
-00012550: 6961 626c 650a 2020 2020 2020 2020 2222  iable.        ""
-00012560: 220a 0a20 2020 2020 2020 2073 7061 7273  "..        spars
-00012570: 6520 3d20 6973 696e 7374 616e 6365 2857  e = isinstance(W
-00012580: 2c20 2870 7974 656e 736f 722e 7370 6172  , (pytensor.spar
-00012590: 7365 2e53 7061 7273 6543 6f6e 7374 616e  se.SparseConstan
-000125a0: 742c 2070 7974 656e 736f 722e 7370 6172  t, pytensor.spar
-000125b0: 7365 2e53 7061 7273 6556 6172 6961 626c  se.SparseVariabl
-000125c0: 6529 290a 0a20 2020 2020 2020 2069 6620  e))..        if 
-000125d0: 7370 6172 7365 3a0a 2020 2020 2020 2020  sparse:.        
-000125e0: 2020 2020 4420 3d20 7370 5f73 756d 2857      D = sp_sum(W
-000125f0: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
-00012600: 2020 2020 2020 4469 6e76 5f73 7172 7420        Dinv_sqrt 
-00012610: 3d20 7074 2e64 6961 6728 3120 2f20 7074  = pt.diag(1 / pt
-00012620: 2e73 7172 7428 4429 290a 2020 2020 2020  .sqrt(D)).      
-00012630: 2020 2020 2020 4457 4420 3d20 7074 2e64        DWD = pt.d
-00012640: 6f74 2870 7974 656e 736f 722e 7370 6172  ot(pytensor.spar
-00012650: 7365 2e64 6f74 2844 696e 765f 7371 7274  se.dot(Dinv_sqrt
-00012660: 2c20 5729 2c20 4469 6e76 5f73 7172 7429  , W), Dinv_sqrt)
-00012670: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00012680: 2020 2020 2020 2020 2020 2044 203d 2057             D = W
-00012690: 2e73 756d 2861 7869 733d 3029 0a20 2020  .sum(axis=0).   
-000126a0: 2020 2020 2020 2020 2044 696e 765f 7371           Dinv_sq
-000126b0: 7274 203d 2070 742e 6469 6167 2831 202f  rt = pt.diag(1 /
-000126c0: 2070 742e 7371 7274 2844 2929 0a20 2020   pt.sqrt(D)).   
-000126d0: 2020 2020 2020 2020 2044 5744 203d 2070           DWD = p
-000126e0: 742e 646f 7428 7074 2e64 6f74 2844 696e  t.dot(pt.dot(Din
-000126f0: 765f 7371 7274 2c20 5729 2c20 4469 6e76  v_sqrt, W), Dinv
-00012700: 5f73 7172 7429 0a20 2020 2020 2020 206c  _sqrt).        l
-00012710: 616d 203d 2070 742e 736c 696e 616c 672e  am = pt.slinalg.
-00012720: 6569 6776 616c 7368 2844 5744 2c20 7074  eigvalsh(DWD, pt
-00012730: 2e65 7965 2844 5744 2e73 6861 7065 5b30  .eye(DWD.shape[0
-00012740: 5d29 290a 0a20 2020 2020 2020 2064 2c20  ]))..        d, 
-00012750: 5f20 3d20 572e 7368 6170 650a 0a20 2020  _ = W.shape..   
-00012760: 2020 2020 2069 6620 7661 6c75 652e 6e64       if value.nd
-00012770: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
-00012780: 2020 2020 2076 616c 7565 203d 2076 616c       value = val
-00012790: 7565 5b4e 6f6e 652c 203a 5d0a 0a20 2020  ue[None, :]..   
-000127a0: 2020 2020 206c 6f67 7461 7520 3d20 6420       logtau = d 
-000127b0: 2a20 7074 2e6c 6f67 2874 6175 292e 7375  * pt.log(tau).su
-000127c0: 6d28 290a 2020 2020 2020 2020 6c6f 6764  m().        logd
-000127d0: 6574 203d 2070 742e 6c6f 6728 3120 2d20  et = pt.log(1 - 
-000127e0: 616c 7068 612e 5420 2a20 6c61 6d5b 3a2c  alpha.T * lam[:,
-000127f0: 204e 6f6e 655d 292e 7375 6d28 290a 2020   None]).sum().  
-00012800: 2020 2020 2020 6465 6c74 6120 3d20 7661        delta = va
-00012810: 6c75 6520 2d20 6d75 0a0a 2020 2020 2020  lue - mu..      
-00012820: 2020 6966 2073 7061 7273 653a 0a20 2020    if sparse:.   
-00012830: 2020 2020 2020 2020 2057 6465 6c74 6120           Wdelta 
-00012840: 3d20 7079 7465 6e73 6f72 2e73 7061 7273  = pytensor.spars
-00012850: 652e 646f 7428 6465 6c74 612c 2057 290a  e.dot(delta, W).
-00012860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00012870: 2020 2020 2020 2020 2020 5764 656c 7461            Wdelta
-00012880: 203d 2070 742e 646f 7428 6465 6c74 612c   = pt.dot(delta,
-00012890: 2057 290a 0a20 2020 2020 2020 2074 6175   W)..        tau
-000128a0: 5f64 6f74 5f64 656c 7461 203d 2044 5b4e  _dot_delta = D[N
-000128b0: 6f6e 652c 203a 5d20 2a20 6465 6c74 6120  one, :] * delta 
-000128c0: 2d20 616c 7068 6120 2a20 5764 656c 7461  - alpha * Wdelta
-000128d0: 0a20 2020 2020 2020 206c 6f67 7175 6164  .        logquad
-000128e0: 203d 2028 7461 7520 2a20 6465 6c74 6120   = (tau * delta 
-000128f0: 2a20 7461 755f 646f 745f 6465 6c74 6129  * tau_dot_delta)
-00012900: 2e73 756d 2861 7869 733d 2d31 290a 2020  .sum(axis=-1).  
-00012910: 2020 2020 2020 7265 7475 726e 2063 6865        return che
-00012920: 636b 5f70 6172 616d 6574 6572 7328 0a20  ck_parameters(. 
-00012930: 2020 2020 2020 2020 2020 2030 2e35 202a             0.5 *
-00012940: 2028 6c6f 6774 6175 202b 206c 6f67 6465   (logtau + logde
-00012950: 7420 2d20 6c6f 6771 7561 6429 2c0a 2020  t - logquad),.  
-00012960: 2020 2020 2020 2020 2020 2d31 203c 3d20            -1 <= 
-00012970: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
-00012980: 2020 2061 6c70 6861 203c 3d20 312c 0a20     alpha <= 1,. 
-00012990: 2020 2020 2020 2020 2020 2074 6175 203e             tau >
-000129a0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
-000129b0: 6d73 673d 222d 3120 3c3d 2061 6c70 6861  msg="-1 <= alpha
-000129c0: 203c 3d20 312c 2074 6175 203e 2030 222c   <= 1, tau > 0",
-000129d0: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
-000129e0: 7373 2053 7469 636b 4272 6561 6b69 6e67  ss StickBreaking
-000129f0: 5765 6967 6874 7352 5628 5261 6e64 6f6d  WeightsRV(Random
-00012a00: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
-00012a10: 616d 6520 3d20 2273 7469 636b 5f62 7265  ame = "stick_bre
-00012a20: 616b 696e 675f 7765 6967 6874 7322 0a20  aking_weights". 
-00012a30: 2020 206e 6469 6d5f 7375 7070 203d 2031     ndim_supp = 1
-00012a40: 0a20 2020 206e 6469 6d73 5f70 6172 616d  .    ndims_param
-00012a50: 7320 3d20 5b30 2c20 305d 0a20 2020 2064  s = [0, 0].    d
-00012a60: 7479 7065 203d 2022 666c 6f61 7458 220a  type = "floatX".
-00012a70: 2020 2020 5f70 7269 6e74 5f6e 616d 6520      _print_name 
-00012a80: 3d20 2822 5374 6963 6b42 7265 616b 696e  = ("StickBreakin
-00012a90: 6757 6569 6768 7473 222c 2022 5c5c 6f70  gWeights", "\\op
-00012aa0: 6572 6174 6f72 6e61 6d65 7b53 7469 636b  eratorname{Stick
-00012ab0: 4272 6561 6b69 6e67 5765 6967 6874 737d  BreakingWeights}
-00012ac0: 2229 0a0a 2020 2020 6465 6620 6d61 6b65  ")..    def make
-00012ad0: 5f6e 6f64 6528 7365 6c66 2c20 726e 672c  _node(self, rng,
-00012ae0: 2073 697a 652c 2064 7479 7065 2c20 616c   size, dtype, al
-00012af0: 7068 612c 204b 293a 0a20 2020 2020 2020  pha, K):.       
-00012b00: 2061 6c70 6861 203d 2070 742e 6173 5f74   alpha = pt.as_t
-00012b10: 656e 736f 725f 7661 7269 6162 6c65 2861  ensor_variable(a
-00012b20: 6c70 6861 290a 2020 2020 2020 2020 4b20  lpha).        K 
-00012b30: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00012b40: 6172 6961 626c 6528 696e 7458 284b 2929  ariable(intX(K))
-00012b50: 0a0a 2020 2020 2020 2020 6966 204b 2e6e  ..        if K.n
-00012b60: 6469 6d20 3e20 303a 0a20 2020 2020 2020  dim > 0:.       
-00012b70: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00012b80: 4572 726f 7228 224b 206d 7573 7420 6265  Error("K must be
-00012b90: 2061 2073 6361 6c61 722e 2229 0a0a 2020   a scalar.")..  
-00012ba0: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-00012bb0: 6572 2829 2e6d 616b 655f 6e6f 6465 2872  er().make_node(r
-00012bc0: 6e67 2c20 7369 7a65 2c20 6474 7970 652c  ng, size, dtype,
-00012bd0: 2061 6c70 6861 2c20 4b29 0a0a 2020 2020   alpha, K)..    
-00012be0: 6465 6620 5f73 7570 705f 7368 6170 655f  def _supp_shape_
-00012bf0: 6672 6f6d 5f70 6172 616d 7328 7365 6c66  from_params(self
-00012c00: 2c20 6469 7374 5f70 6172 616d 732c 202a  , dist_params, *
-00012c10: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00012c20: 2020 4b20 3d20 6469 7374 5f70 6172 616d    K = dist_param
-00012c30: 735b 315d 0a20 2020 2020 2020 2072 6574  s[1].        ret
-00012c40: 7572 6e20 284b 202b 2031 2c29 0a0a 2020  urn (K + 1,)..  
-00012c50: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-00012c60: 2020 2064 6566 2072 6e67 5f66 6e28 636c     def rng_fn(cl
-00012c70: 732c 2072 6e67 2c20 616c 7068 612c 204b  s, rng, alpha, K
-00012c80: 2c20 7369 7a65 293a 0a20 2020 2020 2020  , size):.       
-00012c90: 2069 6620 4b20 3c20 303a 0a20 2020 2020   if K < 0:.     
-00012ca0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00012cb0: 7565 4572 726f 7228 224b 206e 6565 6473  ueError("K needs
-00012cc0: 2074 6f20 6265 2070 6f73 6974 6976 652e   to be positive.
-00012cd0: 2229 0a0a 2020 2020 2020 2020 7369 7a65  ")..        size
-00012ce0: 203d 2074 6f5f 7475 706c 6528 7369 7a65   = to_tuple(size
-00012cf0: 2920 6966 2073 697a 6520 6973 206e 6f74  ) if size is not
-00012d00: 204e 6f6e 6520 656c 7365 2061 6c70 6861   None else alpha
-00012d10: 2e73 6861 7065 0a20 2020 2020 2020 2073  .shape.        s
-00012d20: 697a 6520 3d20 7369 7a65 202b 2028 4b2c  ize = size + (K,
-00012d30: 290a 2020 2020 2020 2020 616c 7068 6120  ).        alpha 
-00012d40: 3d20 616c 7068 615b 2e2e 2e2c 206e 702e  = alpha[..., np.
-00012d50: 6e65 7761 7869 735d 0a0a 2020 2020 2020  newaxis]..      
-00012d60: 2020 6265 7461 7320 3d20 726e 672e 6265    betas = rng.be
-00012d70: 7461 2831 2c20 616c 7068 612c 2073 697a  ta(1, alpha, siz
-00012d80: 653d 7369 7a65 290a 0a20 2020 2020 2020  e=size)..       
-00012d90: 2073 7469 636b 7320 3d20 6e70 2e63 6f6e   sticks = np.con
-00012da0: 6361 7465 6e61 7465 280a 2020 2020 2020  catenate(.      
-00012db0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-00012dc0: 2020 2020 2020 2020 6e70 2e6f 6e65 7328          np.ones(
-00012dd0: 7368 6170 653d 2873 697a 655b 3a2d 315d  shape=(size[:-1]
-00012de0: 202b 2028 312c 2929 292c 0a20 2020 2020   + (1,))),.     
-00012df0: 2020 2020 2020 2020 2020 206e 702e 6375             np.cu
-00012e00: 6d70 726f 6428 3120 2d20 6265 7461 735b  mprod(1 - betas[
-00012e10: 2e2e 2e2c 203a 2d31 5d2c 2061 7869 733d  ..., :-1], axis=
-00012e20: 2d31 292c 0a20 2020 2020 2020 2020 2020  -1),.           
-00012e30: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00012e40: 6178 6973 3d2d 312c 0a20 2020 2020 2020  axis=-1,.       
-00012e50: 2029 0a0a 2020 2020 2020 2020 7765 6967   )..        weig
-00012e60: 6874 7320 3d20 7374 6963 6b73 202a 2062  hts = sticks * b
-00012e70: 6574 6173 0a20 2020 2020 2020 2077 6569  etas.        wei
-00012e80: 6768 7473 203d 206e 702e 636f 6e63 6174  ghts = np.concat
-00012e90: 656e 6174 6528 0a20 2020 2020 2020 2020  enate(.         
-00012ea0: 2020 2028 7765 6967 6874 732c 2031 202d     (weights, 1 -
-00012eb0: 2077 6569 6768 7473 2e73 756d 2861 7869   weights.sum(axi
-00012ec0: 733d 2d31 295b 2e2e 2e2c 206e 702e 6e65  s=-1)[..., np.ne
-00012ed0: 7761 7869 735d 292c 0a20 2020 2020 2020  waxis]),.       
-00012ee0: 2020 2020 2061 7869 733d 2d31 2c0a 2020       axis=-1,.  
-00012ef0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00012f00: 2072 6574 7572 6e20 7765 6967 6874 730a   return weights.
-00012f10: 0a0a 7374 6963 6b62 7265 616b 696e 6777  ..stickbreakingw
-00012f20: 6569 6768 7473 203d 2053 7469 636b 4272  eights = StickBr
-00012f30: 6561 6b69 6e67 5765 6967 6874 7352 5628  eakingWeightsRV(
-00012f40: 290a 0a0a 636c 6173 7320 5374 6963 6b42  )...class StickB
-00012f50: 7265 616b 696e 6757 6569 6768 7473 2853  reakingWeights(S
-00012f60: 696d 706c 6578 436f 6e74 696e 756f 7573  implexContinuous
-00012f70: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
-00012f80: 4c69 6b65 6c69 686f 6f64 206f 6620 7472  Likelihood of tr
-00012f90: 756e 6361 7465 6420 7374 6963 6b2d 6272  uncated stick-br
-00012fa0: 6561 6b69 6e67 2077 6569 6768 7473 2e20  eaking weights. 
-00012fb0: 5468 6520 7765 6967 6874 7320 6172 6520  The weights are 
-00012fc0: 6765 6e65 7261 7465 6420 6672 6f6d 2061  generated from a
-00012fd0: 0a20 2020 2073 7469 636b 2d62 7265 616b  .    stick-break
-00012fe0: 696e 6720 7072 6f63 6564 7563 6520 7768  ing proceduce wh
-00012ff0: 6572 6520 3a6d 6174 683a 6078 5f6b 203d  ere :math:`x_k =
-00013000: 2076 5f6b 205c 7072 6f64 5f7b 5c65 6c6c   v_k \prod_{\ell
-00013010: 203c 206b 7d20 2831 202d 2076 5f5c 656c   < k} (1 - v_\el
-00013020: 6c29 6020 666f 720a 2020 2020 3a6d 6174  l)` for.    :mat
-00013030: 683a 606b 205c 696e 205c 7b31 2c20 5c6c  h:`k \in \{1, \l
-00013040: 646f 7473 2c20 4b5c 7d60 2061 6e64 203a  dots, K\}` and :
-00013050: 6d61 7468 3a60 785f 4b20 3d20 5c70 726f  math:`x_K = \pro
-00013060: 645f 7b5c 656c 6c20 3d20 317d 5e7b 4b7d  d_{\ell = 1}^{K}
-00013070: 2028 3120 2d20 765f 5c65 6c6c 2920 3d20   (1 - v_\ell) = 
-00013080: 3120 2d20 5c73 756d 5f7b 5c65 6c6c 3d31  1 - \sum_{\ell=1
-00013090: 7d5e 4b20 785f 5c65 6c6c 600a 2020 2020  }^K x_\ell`.    
-000130a0: 7769 7468 203a 6d61 7468 3a60 765f 6b20  with :math:`v_k 
-000130b0: 5c73 7461 636b 7265 6c7b 5c74 6578 747b  \stackrel{\text{
-000130c0: 692e 692e 642e 7d7d 7b5c 7369 6d7d 205c  i.i.d.}}{\sim} \
-000130d0: 7465 7874 7b42 6574 617d 2831 2c20 5c61  text{Beta}(1, \a
-000130e0: 6c70 6861 2960 2e0a 0a20 2020 202e 2e20  lpha)`...    .. 
-000130f0: 6d61 7468 3a0a 0a20 2020 2020 2020 2066  math:..        f
-00013100: 285c 6d61 7468 6266 7b78 7d7c 5c61 6c70  (\mathbf{x}|\alp
-00013110: 6861 2c20 4b29 203d 0a20 2020 2020 2020  ha, K) =.       
-00013120: 2020 2020 2042 2831 2c20 5c61 6c70 6861       B(1, \alpha
-00013130: 295e 7b2d 4b7d 785f 7b4b 2b31 7d5e 5c61  )^{-K}x_{K+1}^\a
-00013140: 6c70 6861 205c 7072 6f64 5f7b 6b3d 317d  lpha \prod_{k=1}
-00013150: 5e7b 4b2b 317d 5c6c 6566 745c 7b5c 7375  ^{K+1}\left\{\su
-00013160: 6d5f 7b6a 3d6b 7d5e 7b4b 2b31 7d20 785f  m_{j=k}^{K+1} x_
-00013170: 6a5c 7269 6768 745c 7d5e 7b2d 317d 0a0a  j\right\}^{-1}..
-00013180: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
-00013190: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000131a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000131b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
-000131c0: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
-000131d0: 683a 6078 5f6b 205c 696e 2028 302c 2031  h:`x_k \in (0, 1
-000131e0: 2960 2066 6f72 203a 6d61 7468 3a60 6b20  )` for :math:`k 
-000131f0: 5c69 6e20 5c7b 312c 205c 6c64 6f74 732c  \in \{1, \ldots,
-00013200: 204b 2b31 5c7d 600a 2020 2020 2020 2020   K+1\}`.        
-00013210: 2020 2020 2020 7375 6368 2074 6861 7420        such that 
-00013220: 3a6d 6174 683a 605c 7375 6d20 785f 6b20  :math:`\sum x_k 
-00013230: 3d20 3160 0a20 2020 204d 6561 6e20 2020  = 1`.    Mean   
-00013240: 2020 203a 6d61 7468 3a60 5c6d 6174 6862     :math:`\mathb
-00013250: 627b 457d 5b78 5f6b 5d20 3d20 5c64 6672  b{E}[x_k] = \dfr
-00013260: 6163 7b31 7d7b 3120 2b20 5c61 6c70 6861  ac{1}{1 + \alpha
-00013270: 7d5c 6c65 6674 285c 6466 7261 637b 5c61  }\left(\dfrac{\a
-00013280: 6c70 6861 7d7b 3120 2b20 5c61 6c70 6861  lpha}{1 + \alpha
-00013290: 7d5c 7269 6768 7429 5e7b 6b20 2d20 317d  }\right)^{k - 1}
-000132a0: 600a 2020 2020 2020 2020 2020 2020 2020  `.              
-000132b0: 666f 7220 3a6d 6174 683a 606b 205c 696e  for :math:`k \in
-000132c0: 205c 7b31 2c20 5c6c 646f 7473 2c20 4b5c   \{1, \ldots, K\
-000132d0: 7d60 2061 6e64 203a 6d61 7468 3a60 5c6d  }` and :math:`\m
-000132e0: 6174 6862 627b 457d 5b78 5f7b 4b2b 317d  athbb{E}[x_{K+1}
-000132f0: 5d20 3d20 5c6c 6566 7428 5c64 6672 6163  ] = \left(\dfrac
-00013300: 7b5c 616c 7068 617d 7b31 202b 205c 616c  {\alpha}{1 + \al
-00013310: 7068 617d 5c72 6967 6874 295e 7b4b 7d60  pha}\right)^{K}`
-00013320: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
-00013330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-00013360: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00013370: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00013380: 2020 616c 7068 6120 3a20 7465 6e73 6f72    alpha : tensor
-00013390: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-000133a0: 2020 2020 2020 2043 6f6e 6365 6e74 7261         Concentra
-000133b0: 7469 6f6e 2070 6172 616d 6574 6572 2028  tion parameter (
-000133c0: 616c 7068 6120 3e20 3029 2e0a 2020 2020  alpha > 0)..    
-000133d0: 4b20 3a20 7465 6e73 6f72 5f6c 696b 6520  K : tensor_like 
-000133e0: 6f66 2069 6e74 0a20 2020 2020 2020 2054  of int.        T
-000133f0: 6865 206e 756d 6265 7220 6f66 2022 7374  he number of "st
-00013400: 6963 6b73 2220 746f 2062 7265 616b 206f  icks" to break o
-00013410: 6666 2066 726f 6d20 616e 2069 6e69 7469  ff from an initi
-00013420: 616c 206f 6e65 2d75 6e69 7420 7374 6963  al one-unit stic
-00013430: 6b2e 2054 6865 206c 656e 6774 6820 6f66  k. The length of
-00013440: 2074 6865 2077 6569 6768 740a 2020 2020   the weight.    
-00013450: 2020 2020 7665 6374 6f72 2069 7320 4b20      vector is K 
-00013460: 2b20 312c 2077 6865 7265 2074 6865 206c  + 1, where the l
-00013470: 6173 7420 7765 6967 6874 2069 7320 6f6e  ast weight is on
-00013480: 6520 6d69 6e75 7320 7468 6520 7375 6d20  e minus the sum 
-00013490: 6f66 2061 6c6c 2074 6865 2066 6972 7374  of all the first
-000134a0: 2073 7469 636b 732e 0a0a 2020 2020 5265   sticks...    Re
-000134b0: 6665 7265 6e63 6573 0a20 2020 202d 2d2d  ferences.    ---
-000134c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e 205b  -------.    .. [
-000134d0: 315d 2049 7368 7761 7261 6e2c 2048 2e2c  1] Ishwaran, H.,
-000134e0: 2026 204a 616d 6573 2c20 4c2e 2046 2e20   & James, L. F. 
-000134f0: 2832 3030 3129 2e20 4769 6262 7320 7361  (2001). Gibbs sa
-00013500: 6d70 6c69 6e67 206d 6574 686f 6473 2066  mpling methods f
-00013510: 6f72 2073 7469 636b 2d62 7265 616b 696e  or stick-breakin
-00013520: 6720 7072 696f 7273 2e0a 2020 2020 2020  g priors..      
-00013530: 2020 2020 204a 6f75 726e 616c 206f 6620       Journal of 
-00013540: 7468 6520 416d 6572 6963 616e 2053 7461  the American Sta
-00013550: 7469 7374 6963 616c 2041 7373 6f63 6961  tistical Associa
-00013560: 7469 6f6e 2c20 3936 2834 3533 292c 2031  tion, 96(453), 1
-00013570: 3631 2d31 3733 2e0a 0a20 2020 202e 2e20  61-173...    .. 
-00013580: 5b32 5d20 4dc3 bc6c 6c65 722c 2050 2e2c  [2] M..ller, P.,
-00013590: 2051 7569 6e74 616e 612c 2046 2e20 412e   Quintana, F. A.
-000135a0: 2c20 4a61 7261 2c20 412e 2c20 2620 4861  , Jara, A., & Ha
-000135b0: 6e73 6f6e 2c20 542e 2028 3230 3135 292e  nson, T. (2015).
-000135c0: 2042 6179 6573 6961 6e20 6e6f 6e70 6172   Bayesian nonpar
-000135d0: 616d 6574 7269 6320 6461 7461 0a20 2020  ametric data.   
-000135e0: 2020 2020 2020 2020 616e 616c 7973 6973          analysis
-000135f0: 2e20 4e65 7720 596f 726b 3a20 5370 7269  . New York: Spri
-00013600: 6e67 6572 2e0a 2020 2020 2222 220a 2020  nger..    """.  
-00013610: 2020 7276 5f6f 7020 3d20 7374 6963 6b62    rv_op = stickb
-00013620: 7265 616b 696e 6777 6569 6768 7473 0a0a  reakingweights..
-00013630: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00013640: 0a20 2020 2064 6566 2064 6973 7428 636c  .    def dist(cl
-00013650: 732c 2061 6c70 6861 2c20 4b2c 202a 6172  s, alpha, K, *ar
-00013660: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-00013670: 2020 2020 2020 2061 6c70 6861 203d 2070         alpha = p
-00013680: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00013690: 6162 6c65 2866 6c6f 6174 5828 616c 7068  able(floatX(alph
-000136a0: 6129 290a 2020 2020 2020 2020 4b20 3d20  a)).        K = 
-000136b0: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
-000136c0: 6961 626c 6528 696e 7458 284b 2929 0a0a  iable(intX(K))..
-000136d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000136e0: 7570 6572 2829 2e64 6973 7428 5b61 6c70  uper().dist([alp
-000136f0: 6861 2c20 4b5d 2c20 2a2a 6b77 6172 6773  ha, K], **kwargs
-00013700: 290a 0a20 2020 2064 6566 206d 6f6d 656e  )..    def momen
-00013710: 7428 7276 2c20 7369 7a65 2c20 616c 7068  t(rv, size, alph
-00013720: 612c 204b 293a 0a20 2020 2020 2020 2061  a, K):.        a
-00013730: 6c70 6861 203d 2061 6c70 6861 5b2e 2e2e  lpha = alpha[...
-00013740: 2c20 6e70 2e6e 6577 6178 6973 5d0a 2020  , np.newaxis].  
-00013750: 2020 2020 2020 6d6f 6d65 6e74 203d 2028        moment = (
-00013760: 616c 7068 6120 2f20 2831 202b 2061 6c70  alpha / (1 + alp
-00013770: 6861 2929 202a 2a20 7074 2e61 7261 6e67  ha)) ** pt.arang
-00013780: 6528 4b29 0a20 2020 2020 2020 206d 6f6d  e(K).        mom
-00013790: 656e 7420 2a3d 2031 202f 2028 3120 2b20  ent *= 1 / (1 + 
-000137a0: 616c 7068 6129 0a20 2020 2020 2020 206d  alpha).        m
-000137b0: 6f6d 656e 7420 3d20 7074 2e63 6f6e 6361  oment = pt.conca
-000137c0: 7465 6e61 7465 285b 6d6f 6d65 6e74 2c20  tenate([moment, 
-000137d0: 2861 6c70 6861 202f 2028 3120 2b20 616c  (alpha / (1 + al
-000137e0: 7068 6129 2920 2a2a 204b 5d2c 2061 7869  pha)) ** K], axi
-000137f0: 733d 2d31 290a 2020 2020 2020 2020 6966  s=-1).        if
-00013800: 206e 6f74 2072 765f 7369 7a65 5f69 735f   not rv_size_is_
-00013810: 6e6f 6e65 2873 697a 6529 3a0a 2020 2020  none(size):.    
-00013820: 2020 2020 2020 2020 6d6f 6d65 6e74 5f73          moment_s
-00013830: 697a 6520 3d20 7074 2e63 6f6e 6361 7465  ize = pt.concate
-00013840: 6e61 7465 280a 2020 2020 2020 2020 2020  nate(.          
-00013850: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00013860: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00013870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013880: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138a0: 4b20 2b20 312c 0a20 2020 2020 2020 2020  K + 1,.         
-000138b0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-000138c0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-000138d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000138e0: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
-000138f0: 203d 2070 742e 6675 6c6c 286d 6f6d 656e   = pt.full(momen
-00013900: 745f 7369 7a65 2c20 6d6f 6d65 6e74 290a  t_size, moment).
-00013910: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013920: 6d6f 6d65 6e74 0a0a 2020 2020 6465 6620  moment..    def 
-00013930: 6c6f 6770 2876 616c 7565 2c20 616c 7068  logp(value, alph
-00013940: 612c 204b 293a 0a20 2020 2020 2020 2022  a, K):.        "
-00013950: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
-00013960: 6c61 7465 206c 6f67 2d70 726f 6261 6269  late log-probabi
-00013970: 6c69 7479 206f 6620 7468 6520 6469 7374  lity of the dist
-00013980: 7269 6275 7469 6f6e 2069 6e64 7563 6564  ribution induced
-00013990: 2066 726f 6d20 7468 6520 7374 6963 6b2d   from the stick-
-000139a0: 6272 6561 6b69 6e67 2070 726f 6365 7373  breaking process
-000139b0: 0a20 2020 2020 2020 2061 7420 7370 6563  .        at spec
-000139c0: 6966 6965 6420 7661 6c75 652e 0a0a 2020  ified value...  
-000139d0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000139e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000139f0: 2d2d 2d0a 2020 2020 2020 2020 7661 6c75  ---.        valu
-00013a00: 653a 206e 756d 6572 6963 0a20 2020 2020  e: numeric.     
-00013a10: 2020 2020 2020 2056 616c 7565 2066 6f72         Value for
-00013a20: 2077 6869 6368 206c 6f67 2d70 726f 6261   which log-proba
-00013a30: 6269 6c69 7479 2069 7320 6361 6c63 756c  bility is calcul
-00013a40: 6174 6564 2e0a 0a20 2020 2020 2020 2052  ated...        R
-00013a50: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00013a60: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
-00013a70: 656e 736f 7256 6172 6961 626c 650a 2020  ensorVariable.  
-00013a80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013a90: 2020 6c6f 6770 203d 202d 7074 2e73 756d    logp = -pt.sum
-00013aa0: 280a 2020 2020 2020 2020 2020 2020 7074  (.            pt
-00013ab0: 2e6c 6f67 280a 2020 2020 2020 2020 2020  .log(.          
-00013ac0: 2020 2020 2020 7074 2e63 756d 7375 6d28        pt.cumsum(
-00013ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ae0: 2020 2020 2076 616c 7565 5b2e 2e2e 2c20       value[..., 
-00013af0: 3a3a 2d31 5d2c 0a20 2020 2020 2020 2020  ::-1],.         
-00013b00: 2020 2020 2020 2020 2020 2061 7869 733d             axis=
-00013b10: 2d31 2c0a 2020 2020 2020 2020 2020 2020  -1,.            
-00013b20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00013b30: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00013b40: 2061 7869 733d 2d31 2c0a 2020 2020 2020   axis=-1,.      
-00013b50: 2020 290a 2020 2020 2020 2020 6c6f 6770    ).        logp
-00013b60: 202b 3d20 2d4b 202a 2062 6574 616c 6e28   += -K * betaln(
-00013b70: 312c 2061 6c70 6861 290a 2020 2020 2020  1, alpha).      
-00013b80: 2020 6c6f 6770 202b 3d20 616c 7068 6120    logp += alpha 
-00013b90: 2a20 7074 2e6c 6f67 2876 616c 7565 5b2e  * pt.log(value[.
-00013ba0: 2e2e 2c20 2d31 5d29 0a0a 2020 2020 2020  .., -1])..      
-00013bb0: 2020 6c6f 6770 203d 2070 742e 7377 6974    logp = pt.swit
-00013bc0: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
-00013bd0: 7074 2e6f 725f 280a 2020 2020 2020 2020  pt.or_(.        
-00013be0: 2020 2020 2020 2020 7074 2e61 6e79 280a          pt.any(.
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c00: 2020 2020 7074 2e61 6e64 5f28 7074 2e6c      pt.and_(pt.l
-00013c10: 6528 7661 6c75 652c 2030 292c 2070 742e  e(value, 0), pt.
-00013c20: 6765 2876 616c 7565 2c20 3129 292c 0a20  ge(value, 1)),. 
-00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c40: 2020 2061 7869 733d 2d31 2c0a 2020 2020     axis=-1,.    
-00013c50: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013c70: 742e 6f72 5f28 0a20 2020 2020 2020 2020  t.or_(.         
-00013c80: 2020 2020 2020 2020 2020 2070 742e 6269             pt.bi
-00013c90: 7477 6973 655f 6e6f 7428 7074 2e61 6c6c  twise_not(pt.all
-00013ca0: 636c 6f73 6528 7661 6c75 652e 7375 6d28  close(value.sum(
-00013cb0: 2d31 292c 2031 2929 2c0a 2020 2020 2020  -1), 1)),.      
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 7074                pt
-00013cd0: 2e6e 6571 2876 616c 7565 2e73 6861 7065  .neq(value.shape
-00013ce0: 5b2d 315d 2c20 4b20 2b20 3129 2c0a 2020  [-1], K + 1),.  
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-00013d00: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00013d10: 2020 2020 2020 2020 2020 2020 2d6e 702e              -np.
-00013d20: 696e 662c 0a20 2020 2020 2020 2020 2020  inf,.           
-00013d30: 206c 6f67 702c 0a20 2020 2020 2020 2029   logp,.        )
-00013d40: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00013d50: 2063 6865 636b 5f70 6172 616d 6574 6572   check_parameter
-00013d60: 7328 0a20 2020 2020 2020 2020 2020 206c  s(.            l
-00013d70: 6f67 702c 0a20 2020 2020 2020 2020 2020  ogp,.           
-00013d80: 2061 6c70 6861 203e 2030 2c0a 2020 2020   alpha > 0,.    
-00013d90: 2020 2020 2020 2020 4b20 3e20 302c 0a20          K > 0,. 
-00013da0: 2020 2020 2020 2020 2020 206d 7367 3d22             msg="
-00013db0: 616c 7068 6120 3e20 302c 204b 203e 2030  alpha > 0, K > 0
-00013dc0: 222c 0a20 2020 2020 2020 2029 0a0a 0a63  ",.        )...c
-00013dd0: 6c61 7373 205a 6572 6f53 756d 4e6f 726d  lass ZeroSumNorm
-00013de0: 616c 5256 2853 796d 626f 6c69 6352 616e  alRV(SymbolicRan
-00013df0: 646f 6d56 6172 6961 626c 6529 3a0a 2020  domVariable):.  
-00013e00: 2020 2222 225a 6572 6f53 756d 4e6f 726d    """ZeroSumNorm
-00013e10: 616c 2072 616e 646f 6d20 7661 7269 6162  al random variab
-00013e20: 6c65 2222 220a 0a20 2020 205f 7072 696e  le"""..    _prin
-00013e30: 745f 6e61 6d65 203d 2028 225a 6572 6f53  t_name = ("ZeroS
-00013e40: 756d 4e6f 726d 616c 222c 2022 5c5c 6f70  umNormal", "\\op
-00013e50: 6572 6174 6f72 6e61 6d65 7b5a 6572 6f53  eratorname{ZeroS
-00013e60: 756d 4e6f 726d 616c 7d22 290a 2020 2020  umNormal}").    
-00013e70: 6465 6661 756c 745f 6f75 7470 7574 203d  default_output =
-00013e80: 2030 0a0a 0a63 6c61 7373 205a 6572 6f53   0...class ZeroS
-00013e90: 756d 4e6f 726d 616c 2844 6973 7472 6962  umNormal(Distrib
-00013ea0: 7574 696f 6e29 3a0a 2020 2020 7222 2222  ution):.    r"""
-00013eb0: 0a20 2020 205a 6572 6f53 756d 4e6f 726d  .    ZeroSumNorm
-00013ec0: 616c 2064 6973 7472 6962 7574 696f 6e2c  al distribution,
-00013ed0: 2069 2e65 204e 6f72 6d61 6c20 6469 7374   i.e Normal dist
-00013ee0: 7269 6275 7469 6f6e 2077 6865 7265 206f  ribution where o
-00013ef0: 6e65 206f 720a 2020 2020 7365 7665 7261  ne or.    severa
-00013f00: 6c20 6178 6573 2061 7265 2063 6f6e 7374  l axes are const
-00013f10: 7261 696e 6564 2074 6f20 7375 6d20 746f  rained to sum to
-00013f20: 207a 6572 6f2e 0a20 2020 2042 7920 6465   zero..    By de
-00013f30: 6661 756c 742c 2074 6865 206c 6173 7420  fault, the last 
-00013f40: 6178 6973 2069 7320 636f 6e73 7472 6169  axis is constrai
-00013f50: 6e65 6420 746f 2073 756d 2074 6f20 7a65  ned to sum to ze
-00013f60: 726f 2e0a 2020 2020 5365 6520 606e 5f7a  ro..    See `n_z
-00013f70: 6572 6f73 756d 5f61 7865 7360 206b 7761  erosum_axes` kwa
-00013f80: 7267 2066 6f72 206d 6f72 6520 6465 7461  rg for more deta
-00013f90: 696c 732e 0a0a 2020 2020 2e2e 206d 6174  ils...    .. mat
-00013fa0: 683a 3a0a 0a20 2020 2020 2020 205c 6265  h::..        \be
-00013fb0: 6769 6e7b 616c 6967 6e2a 7d0a 2020 2020  gin{align*}.    
-00013fc0: 2020 2020 2020 2020 5a53 4e28 5c73 6967          ZSN(\sig
-00013fd0: 6d61 2920 3d20 4e20 5c42 6967 2820 302c  ma) = N \Big( 0,
-00013fe0: 205c 7369 676d 615e 3220 2849 202d 205c   \sigma^2 (I - \
-00013ff0: 7466 7261 637b 317d 7b6e 7d4a 2920 5c42  tfrac{1}{n}J) \B
-00014000: 6967 2920 5c5c 0a20 2020 2020 2020 2020  ig) \\.         
-00014010: 2020 205c 7465 7874 7b77 6865 7265 7d20     \text{where} 
-00014020: 5c20 7e20 4a5f 7b69 6a7d 203d 2031 205c  \ ~ J_{ij} = 1 \
-00014030: 207e 205c 7465 7874 7b61 6e64 7d20 5c5c   ~ \text{and} \\
-00014040: 0a20 2020 2020 2020 2020 2020 206e 203d  .            n =
-00014050: 205c 7465 7874 7b6e 6272 206f 6620 7a65   \text{nbr of ze
-00014060: 726f 2d73 756d 2061 7865 737d 0a20 2020  ro-sum axes}.   
-00014070: 2020 2020 205c 656e 647b 616c 6967 6e2a       \end{align*
-00014080: 7d0a 0a20 2020 2050 6172 616d 6574 6572  }..    Parameter
-00014090: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-000140a0: 0a20 2020 2073 6967 6d61 203a 2074 656e  .    sigma : ten
-000140b0: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
-000140c0: 740a 2020 2020 2020 2020 5363 616c 6520  t.        Scale 
-000140d0: 7061 7261 6d65 7465 7220 2873 6967 6d61  parameter (sigma
-000140e0: 203e 2030 292e 0a20 2020 2020 2020 2049   > 0)..        I
-000140f0: 7427 7320 6163 7475 616c 6c79 2074 6865  t's actually the
-00014100: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-00014110: 696f 6e20 6f66 2074 6865 2075 6e64 6572  ion of the under
-00014120: 6c79 696e 672c 2075 6e63 6f6e 7374 7261  lying, unconstra
-00014130: 696e 6564 204e 6f72 6d61 6c20 6469 7374  ined Normal dist
-00014140: 7269 6275 7469 6f6e 2e0a 2020 2020 2020  ribution..      
-00014150: 2020 4465 6661 756c 7473 2074 6f20 3120    Defaults to 1 
-00014160: 6966 206e 6f74 2073 7065 6369 6669 6564  if not specified
-00014170: 2e0a 2020 2020 2020 2020 466f 7220 6e6f  ..        For no
-00014180: 772c 2060 6073 6967 6d61 6060 2068 6173  w, ``sigma`` has
-00014190: 2074 6f20 6265 2061 2073 6361 6c61 722c   to be a scalar,
-000141a0: 2074 6f20 656e 7375 7265 2074 6865 207a   to ensure the z
-000141b0: 6572 6f2d 7375 6d20 636f 6e73 7472 6169  ero-sum constrai
-000141c0: 6e74 2e0a 2020 2020 6e5f 7a65 726f 7375  nt..    n_zerosu
-000141d0: 6d5f 6178 6573 3a20 696e 742c 2064 6566  m_axes: int, def
-000141e0: 6175 6c74 7320 746f 2031 0a20 2020 2020  aults to 1.     
-000141f0: 2020 204e 756d 6265 7220 6f66 2061 7865     Number of axe
-00014200: 7320 616c 6f6e 6720 7768 6963 6820 7468  s along which th
-00014210: 6520 7a65 726f 2d73 756d 2063 6f6e 7374  e zero-sum const
-00014220: 7261 696e 7420 6973 2065 6e66 6f72 6365  raint is enforce
-00014230: 642c 2073 7461 7274 696e 6720 6672 6f6d  d, starting from
-00014240: 2074 6865 2072 6967 6874 6d6f 7374 2070   the rightmost p
-00014250: 6f73 6974 696f 6e2e 0a20 2020 2020 2020  osition..       
-00014260: 2044 6566 6175 6c74 7320 746f 2031 2c20   Defaults to 1, 
-00014270: 692e 6520 7468 6520 7269 6768 746d 6f73  i.e the rightmos
-00014280: 7420 6178 6973 2e0a 2020 2020 7a65 726f  t axis..    zero
-00014290: 7375 6d5f 6178 6573 3a20 696e 742c 2064  sum_axes: int, d
-000142a0: 6570 7265 6361 7465 6420 706c 6561 7365  eprecated please
-000142b0: 2075 7365 206e 5f7a 6572 6f73 756d 5f61   use n_zerosum_a
-000142c0: 7865 7320 6173 2069 7473 2073 7563 6365  xes as its succe
-000142d0: 7373 6f72 0a20 2020 2064 696d 733a 2073  ssor.    dims: s
-000142e0: 6571 7565 6e63 6520 6f66 2073 7472 696e  equence of strin
-000142f0: 6773 2c20 6f70 7469 6f6e 616c 0a20 2020  gs, optional.   
-00014300: 2020 2020 2044 696d 656e 7369 6f6e 206e       Dimension n
-00014310: 616d 6573 206f 6620 7468 6520 6469 7374  ames of the dist
-00014320: 7269 6275 7469 6f6e 2e20 576f 726b 7320  ribution. Works 
-00014330: 7468 6520 7361 6d65 2061 7320 666f 7220  the same as for 
-00014340: 6f74 6865 7220 5079 4d43 2064 6973 7472  other PyMC distr
-00014350: 6962 7574 696f 6e73 2e0a 2020 2020 2020  ibutions..      
-00014360: 2020 4e65 6365 7373 6172 7920 6966 2060    Necessary if `
-00014370: 6073 6861 7065 6060 2069 7320 6e6f 7420  `shape`` is not 
-00014380: 7061 7373 6564 2e0a 2020 2020 7368 6170  passed..    shap
-00014390: 653a 2074 7570 6c65 206f 6620 696e 7465  e: tuple of inte
-000143a0: 6765 7273 2c20 6f70 7469 6f6e 616c 0a20  gers, optional. 
-000143b0: 2020 2020 2020 2053 6861 7065 206f 6620         Shape of 
-000143c0: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
-000143d0: 2e20 576f 726b 7320 7468 6520 7361 6d65  . Works the same
-000143e0: 2061 7320 666f 7220 6f74 6865 7220 5079   as for other Py
-000143f0: 4d43 2064 6973 7472 6962 7574 696f 6e73  MC distributions
-00014400: 2e0a 2020 2020 2020 2020 4e65 6365 7373  ..        Necess
-00014410: 6172 7920 6966 2060 6064 696d 7360 6020  ary if ``dims`` 
-00014420: 6f72 2060 606f 6273 6572 7665 6460 6020  or ``observed`` 
-00014430: 6973 206e 6f74 2070 6173 7365 642e 0a0a  is not passed...
-00014440: 2020 2020 5761 726e 696e 6773 0a20 2020      Warnings.   
-00014450: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 6060   --------.    ``
-00014460: 7369 676d 6160 6020 6861 7320 746f 2062  sigma`` has to b
-00014470: 6520 6120 7363 616c 6172 2c20 746f 2065  e a scalar, to e
-00014480: 6e73 7572 6520 7468 6520 7a65 726f 2d73  nsure the zero-s
-00014490: 756d 2063 6f6e 7374 7261 696e 742e 0a20  um constraint.. 
-000144a0: 2020 2054 6865 2061 6269 6c69 7479 2074     The ability t
-000144b0: 6f20 7370 6563 6966 7920 6120 7665 6374  o specify a vect
-000144c0: 6f72 206f 6620 6060 7369 676d 6160 6020  or of ``sigma`` 
-000144d0: 6d61 7920 6265 2061 6464 6564 2069 6e20  may be added in 
-000144e0: 6675 7475 7265 2076 6572 7369 6f6e 732e  future versions.
-000144f0: 0a0a 2020 2020 6060 6e5f 7a65 726f 7375  ..    ``n_zerosu
-00014500: 6d5f 6178 6573 6060 2068 6173 2074 6f20  m_axes`` has to 
-00014510: 6265 203e 2030 2e20 4966 2079 6f75 2077  be > 0. If you w
-00014520: 616e 7420 7468 6520 6265 6861 7669 6f72  ant the behavior
-00014530: 206f 6620 6060 6e5f 7a65 726f 7375 6d5f   of ``n_zerosum_
-00014540: 6178 6573 203d 2030 6060 2c0a 2020 2020  axes = 0``,.    
-00014550: 6a75 7374 2075 7365 2060 6070 6d2e 4e6f  just use ``pm.No
-00014560: 726d 616c 6060 2e0a 0a20 2020 2045 7861  rmal``...    Exa
-00014570: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
-00014580: 2d2d 0a20 2020 2044 6566 696e 6520 6120  --.    Define a 
-00014590: 605a 6572 6f53 756d 4e6f 726d 616c 6020  `ZeroSumNormal` 
-000145a0: 7661 7269 6162 6c65 2c20 7769 7468 2060  variable, with `
-000145b0: 7369 676d 613d 3160 2061 6e64 0a20 2020  sigma=1` and.   
-000145c0: 2060 6e5f 7a65 726f 7375 6d5f 6178 6573   `n_zerosum_axes
-000145d0: 3d31 6020 2062 7920 6465 6661 756c 743a  =1`  by default:
-000145e0: 3a0a 0a20 2020 2020 2020 2043 4f4f 5244  :..        COORD
-000145f0: 5320 3d20 7b0a 2020 2020 2020 2020 2020  S = {.          
-00014600: 2020 2272 6567 696f 6e73 223a 205b 2261    "regions": ["a
-00014610: 222c 2022 6222 2c20 2263 225d 2c0a 2020  ", "b", "c"],.  
-00014620: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
-00014630: 7273 223a 205b 2279 6573 222c 2022 6e6f  rs": ["yes", "no
-00014640: 222c 2022 7768 6174 6576 6572 222c 2022  ", "whatever", "
-00014650: 646f 6e27 7420 756e 6465 7273 7461 6e64  don't understand
-00014660: 2071 7565 7374 696f 6e22 5d2c 0a20 2020   question"],.   
-00014670: 2020 2020 207d 0a20 2020 2020 2020 2077       }.        w
-00014680: 6974 6820 706d 2e4d 6f64 656c 2863 6f6f  ith pm.Model(coo
-00014690: 7264 733d 434f 4f52 4453 2920 6173 206d  rds=COORDS) as m
-000146a0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000146b0: 7468 6520 7a65 726f 2073 756d 2061 7869  the zero sum axi
-000146c0: 7320 7769 6c6c 2062 6520 2761 6e73 7765  s will be 'answe
-000146d0: 7273 270a 2020 2020 2020 2020 2020 2020  rs'.            
-000146e0: 7620 3d20 706d 2e5a 6572 6f53 756d 4e6f  v = pm.ZeroSumNo
-000146f0: 726d 616c 2822 7622 2c20 6469 6d73 3d28  rmal("v", dims=(
-00014700: 2272 6567 696f 6e73 222c 2022 616e 7377  "regions", "answ
-00014710: 6572 7322 2929 0a0a 2020 2020 2020 2020  ers"))..        
-00014720: 7769 7468 2070 6d2e 4d6f 6465 6c28 636f  with pm.Model(co
-00014730: 6f72 6473 3d43 4f4f 5244 5329 2061 7320  ords=COORDS) as 
-00014740: 6d3a 0a20 2020 2020 2020 2020 2020 2023  m:.            #
-00014750: 2074 6865 207a 6572 6f20 7375 6d20 6178   the zero sum ax
-00014760: 6573 2077 696c 6c20 6265 2027 616e 7377  es will be 'answ
-00014770: 6572 7327 2061 6e64 2027 7265 6769 6f6e  ers' and 'region
-00014780: 7327 0a20 2020 2020 2020 2020 2020 2076  s'.            v
-00014790: 203d 2070 6d2e 5a65 726f 5375 6d4e 6f72   = pm.ZeroSumNor
-000147a0: 6d61 6c28 2276 222c 2064 696d 733d 2822  mal("v", dims=("
-000147b0: 7265 6769 6f6e 7322 2c20 2261 6e73 7765  regions", "answe
-000147c0: 7273 2229 2c20 6e5f 7a65 726f 7375 6d5f  rs"), n_zerosum_
-000147d0: 6178 6573 3d32 290a 0a20 2020 2020 2020  axes=2)..       
-000147e0: 2077 6974 6820 706d 2e4d 6f64 656c 2863   with pm.Model(c
-000147f0: 6f6f 7264 733d 434f 4f52 4453 2920 6173  oords=COORDS) as
-00014800: 206d 3a0a 2020 2020 2020 2020 2020 2020   m:.            
-00014810: 2320 7468 6520 7a65 726f 2073 756d 2061  # the zero sum a
-00014820: 7865 7320 7769 6c6c 2062 6520 7468 6520  xes will be the 
-00014830: 6c61 7374 2074 776f 0a20 2020 2020 2020  last two.       
-00014840: 2020 2020 2076 203d 2070 6d2e 5a65 726f       v = pm.Zero
-00014850: 5375 6d4e 6f72 6d61 6c28 2276 222c 2073  SumNormal("v", s
-00014860: 6861 7065 3d28 332c 2034 2c20 3529 2c20  hape=(3, 4, 5), 
-00014870: 6e5f 7a65 726f 7375 6d5f 6178 6573 3d32  n_zerosum_axes=2
-00014880: 290a 2020 2020 2222 220a 2020 2020 7276  ).    """.    rv
-00014890: 5f74 7970 6520 3d20 5a65 726f 5375 6d4e  _type = ZeroSumN
-000148a0: 6f72 6d61 6c52 560a 0a20 2020 2064 6566  ormalRV..    def
-000148b0: 205f 5f6e 6577 5f5f 280a 2020 2020 2020   __new__(.      
-000148c0: 2020 636c 732c 202a 6172 6773 2c20 7a65    cls, *args, ze
-000148d0: 726f 7375 6d5f 6178 6573 3d4e 6f6e 652c  rosum_axes=None,
-000148e0: 206e 5f7a 6572 6f73 756d 5f61 7865 733d   n_zerosum_axes=
-000148f0: 4e6f 6e65 2c20 7375 7070 6f72 745f 7368  None, support_sh
-00014900: 6170 653d 4e6f 6e65 2c20 6469 6d73 3d4e  ape=None, dims=N
-00014910: 6f6e 652c 202a 2a6b 7761 7267 730a 2020  one, **kwargs.  
-00014920: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
-00014930: 7a65 726f 7375 6d5f 6178 6573 2069 7320  zerosum_axes is 
-00014940: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00014950: 2020 2020 2020 6e5f 7a65 726f 7375 6d5f        n_zerosum_
-00014960: 6178 6573 203d 207a 6572 6f73 756d 5f61  axes = zerosum_a
-00014970: 7865 730a 2020 2020 2020 2020 2020 2020  xes.            
-00014980: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-00014990: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000149a0: 5468 6520 277a 6572 6f73 756d 5f61 7865  The 'zerosum_axe
-000149b0: 7327 2070 6172 616d 6574 6572 2069 7320  s' parameter is 
-000149c0: 6465 7072 6563 6174 6564 2e20 5573 6520  deprecated. Use 
-000149d0: 276e 5f7a 6572 6f73 756d 5f61 7865 7327  'n_zerosum_axes'
-000149e0: 2069 6e73 7465 6164 2e22 2c0a 2020 2020   instead.",.    
-000149f0: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-00014a00: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
-00014a10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00014a20: 2020 2020 2020 6966 2064 696d 7320 6973        if dims is
-00014a30: 206e 6f74 204e 6f6e 6520 6f72 206b 7761   not None or kwa
-00014a40: 7267 732e 6765 7428 226f 6273 6572 7665  rgs.get("observe
-00014a50: 6422 2920 6973 206e 6f74 204e 6f6e 653a  d") is not None:
-00014a60: 0a20 2020 2020 2020 2020 2020 206e 5f7a  .            n_z
-00014a70: 6572 6f73 756d 5f61 7865 7320 3d20 636c  erosum_axes = cl
-00014a80: 732e 6368 6563 6b5f 7a65 726f 7375 6d5f  s.check_zerosum_
-00014a90: 6178 6573 286e 5f7a 6572 6f73 756d 5f61  axes(n_zerosum_a
-00014aa0: 7865 7329 0a0a 2020 2020 2020 2020 2020  xes)..          
-00014ab0: 2020 7375 7070 6f72 745f 7368 6170 6520    support_shape 
-00014ac0: 3d20 6765 745f 7375 7070 6f72 745f 7368  = get_support_sh
-00014ad0: 6170 6528 0a20 2020 2020 2020 2020 2020  ape(.           
-00014ae0: 2020 2020 2073 7570 706f 7274 5f73 6861       support_sha
-00014af0: 7065 3d73 7570 706f 7274 5f73 6861 7065  pe=support_shape
-00014b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014b10: 2020 7368 6170 653d 4e6f 6e65 2c20 2023    shape=None,  #
-00014b20: 2053 6861 7065 2077 696c 6c20 6265 2063   Shape will be c
-00014b30: 6865 636b 6564 2069 6e20 6063 6c73 2e64  hecked in `cls.d
-00014b40: 6973 7460 0a20 2020 2020 2020 2020 2020  ist`.           
-00014b50: 2020 2020 2064 696d 733d 6469 6d73 2c0a       dims=dims,.
-00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b70: 6f62 7365 7276 6564 3d6b 7761 7267 732e  observed=kwargs.
-00014b80: 6765 7428 226f 6273 6572 7665 6422 2c20  get("observed", 
-00014b90: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
-00014ba0: 2020 2020 2020 206e 6469 6d5f 7375 7070         ndim_supp
-00014bb0: 3d6e 5f7a 6572 6f73 756d 5f61 7865 732c  =n_zerosum_axes,
-00014bc0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00014bd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00014be0: 7570 6572 2829 2e5f 5f6e 6577 5f5f 280a  uper().__new__(.
-00014bf0: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
-00014c00: 0a20 2020 2020 2020 2020 2020 202a 6172  .            *ar
-00014c10: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
-00014c20: 6e5f 7a65 726f 7375 6d5f 6178 6573 3d6e  n_zerosum_axes=n
-00014c30: 5f7a 6572 6f73 756d 5f61 7865 732c 0a20  _zerosum_axes,. 
-00014c40: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-00014c50: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
-00014c60: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
-00014c70: 2020 2020 6469 6d73 3d64 696d 732c 0a20      dims=dims,. 
-00014c80: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00014c90: 7267 732c 0a20 2020 2020 2020 2029 0a0a  rgs,.        )..
-00014ca0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00014cb0: 0a20 2020 2064 6566 2064 6973 7428 636c  .    def dist(cl
-00014cc0: 732c 2073 6967 6d61 3d31 2c20 6e5f 7a65  s, sigma=1, n_ze
-00014cd0: 726f 7375 6d5f 6178 6573 3d4e 6f6e 652c  rosum_axes=None,
-00014ce0: 2073 7570 706f 7274 5f73 6861 7065 3d4e   support_shape=N
-00014cf0: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0a  one, **kwargs):.
-00014d00: 2020 2020 2020 2020 6e5f 7a65 726f 7375          n_zerosu
-00014d10: 6d5f 6178 6573 203d 2063 6c73 2e63 6865  m_axes = cls.che
-00014d20: 636b 5f7a 6572 6f73 756d 5f61 7865 7328  ck_zerosum_axes(
-00014d30: 6e5f 7a65 726f 7375 6d5f 6178 6573 290a  n_zerosum_axes).
-00014d40: 0a20 2020 2020 2020 2073 6967 6d61 203d  .        sigma =
-00014d50: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00014d60: 7269 6162 6c65 2866 6c6f 6174 5828 7369  riable(floatX(si
-00014d70: 676d 6129 290a 2020 2020 2020 2020 6966  gma)).        if
-00014d80: 2073 6967 6d61 2e6e 6469 6d20 3e20 303a   sigma.ndim > 0:
-00014d90: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00014da0: 7365 2056 616c 7565 4572 726f 7228 2273  se ValueError("s
-00014db0: 6967 6d61 2068 6173 2074 6f20 6265 2061  igma has to be a
-00014dc0: 2073 6361 6c61 7222 290a 0a20 2020 2020   scalar")..     
-00014dd0: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
-00014de0: 203d 2067 6574 5f73 7570 706f 7274 5f73   = get_support_s
-00014df0: 6861 7065 280a 2020 2020 2020 2020 2020  hape(.          
-00014e00: 2020 7375 7070 6f72 745f 7368 6170 653d    support_shape=
-00014e10: 7375 7070 6f72 745f 7368 6170 652c 0a20  support_shape,. 
-00014e20: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-00014e30: 3d6b 7761 7267 732e 6765 7428 2273 6861  =kwargs.get("sha
-00014e40: 7065 2229 2c0a 2020 2020 2020 2020 2020  pe"),.          
-00014e50: 2020 6e64 696d 5f73 7570 703d 6e5f 7a65    ndim_supp=n_ze
-00014e60: 726f 7375 6d5f 6178 6573 2c0a 2020 2020  rosum_axes,.    
-00014e70: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-00014e80: 6620 7375 7070 6f72 745f 7368 6170 6520  f support_shape 
-00014e90: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00014ea0: 2020 2020 2069 6620 6e5f 7a65 726f 7375       if n_zerosu
-00014eb0: 6d5f 6178 6573 203e 2030 3a0a 2020 2020  m_axes > 0:.    
-00014ec0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00014ed0: 6520 5661 6c75 6545 7272 6f72 2822 596f  e ValueError("Yo
-00014ee0: 7520 6d75 7374 2073 7065 6369 6679 2064  u must specify d
-00014ef0: 696d 732c 2073 6861 7065 206f 7220 7375  ims, shape or su
-00014f00: 7070 6f72 745f 7368 6170 6520 7061 7261  pport_shape para
-00014f10: 6d65 7465 7222 290a 2020 2020 2020 2020  meter").        
-00014f20: 2020 2020 2320 544f 444f 3a20 6564 6765      # TODO: edge
-00014f30: 2d63 6173 6520 646f 6573 6e27 7420 776f  -case doesn't wo
-00014f40: 726b 2066 6f72 206e 6f77 2c20 6265 6361  rk for now, beca
-00014f50: 7573 6520 7074 2e73 7461 636b 2069 6e20  use pt.stack in 
-00014f60: 6765 745f 7375 7070 6f72 745f 7368 6170  get_support_shap
-00014f70: 6520 6661 696c 730a 2020 2020 2020 2020  e fails.        
-00014f80: 2020 2020 2320 656c 7365 3a0a 2020 2020      # else:.    
-00014f90: 2020 2020 2020 2020 2320 2020 2020 7375          #     su
-00014fa0: 7070 6f72 745f 7368 6170 6520 3d20 2829  pport_shape = ()
-00014fb0: 2023 2062 6563 6175 7365 2069 7427 7320   # because it's 
-00014fc0: 6a75 7374 2061 204e 6f72 6d61 6c20 696e  just a Normal in
-00014fd0: 2074 6861 7420 6361 7365 0a20 2020 2020   that case.     
-00014fe0: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
-00014ff0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-00015000: 7661 7269 6162 6c65 2869 6e74 5828 7375  variable(intX(su
-00015010: 7070 6f72 745f 7368 6170 6529 290a 0a20  pport_shape)).. 
-00015020: 2020 2020 2020 2061 7373 6572 7420 6e5f         assert n_
-00015030: 7a65 726f 7375 6d5f 6178 6573 203d 3d20  zerosum_axes == 
-00015040: 7074 2e67 6574 5f76 6563 746f 725f 6c65  pt.get_vector_le
-00015050: 6e67 7468 280a 2020 2020 2020 2020 2020  ngth(.          
-00015060: 2020 7375 7070 6f72 745f 7368 6170 650a    support_shape.
-00015070: 2020 2020 2020 2020 292c 2022 7375 7070          ), "supp
-00015080: 6f72 745f 7368 6170 6520 6861 7320 746f  ort_shape has to
-00015090: 2062 6520 6173 206c 6f6e 6720 6173 206e   be as long as n
-000150a0: 5f7a 6572 6f73 756d 5f61 7865 7322 0a0a  _zerosum_axes"..
-000150b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000150c0: 7570 6572 2829 2e64 6973 7428 0a20 2020  uper().dist(.   
-000150d0: 2020 2020 2020 2020 205b 7369 676d 615d           [sigma]
-000150e0: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
-000150f0: 3d6e 5f7a 6572 6f73 756d 5f61 7865 732c  =n_zerosum_axes,
-00015100: 2073 7570 706f 7274 5f73 6861 7065 3d73   support_shape=s
-00015110: 7570 706f 7274 5f73 6861 7065 2c20 2a2a  upport_shape, **
-00015120: 6b77 6172 6773 0a20 2020 2020 2020 2029  kwargs.        )
-00015130: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00015140: 6f64 0a20 2020 2064 6566 2063 6865 636b  od.    def check
-00015150: 5f7a 6572 6f73 756d 5f61 7865 7328 636c  _zerosum_axes(cl
-00015160: 732c 206e 5f7a 6572 6f73 756d 5f61 7865  s, n_zerosum_axe
-00015170: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-00015180: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00015190: 2020 6966 206e 5f7a 6572 6f73 756d 5f61    if n_zerosum_a
-000151a0: 7865 7320 6973 204e 6f6e 653a 0a20 2020  xes is None:.   
-000151b0: 2020 2020 2020 2020 206e 5f7a 6572 6f73           n_zeros
-000151c0: 756d 5f61 7865 7320 3d20 310a 2020 2020  um_axes = 1.    
-000151d0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-000151e0: 7461 6e63 6528 6e5f 7a65 726f 7375 6d5f  tance(n_zerosum_
-000151f0: 6178 6573 2c20 696e 7429 3a0a 2020 2020  axes, int):.    
-00015200: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-00015210: 7065 4572 726f 7228 226e 5f7a 6572 6f73  peError("n_zeros
-00015220: 756d 5f61 7865 7320 6861 7320 746f 2062  um_axes has to b
-00015230: 6520 616e 2069 6e74 6567 6572 2229 0a20  e an integer"). 
-00015240: 2020 2020 2020 2069 6620 6e6f 7420 6e5f         if not n_
-00015250: 7a65 726f 7375 6d5f 6178 6573 203e 2030  zerosum_axes > 0
-00015260: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00015270: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00015280: 6e5f 7a65 726f 7375 6d5f 6178 6573 2068  n_zerosum_axes h
-00015290: 6173 2074 6f20 6265 203e 2030 2229 0a20  as to be > 0"). 
-000152a0: 2020 2020 2020 2072 6574 7572 6e20 6e5f         return n_
-000152b0: 7a65 726f 7375 6d5f 6178 6573 0a0a 2020  zerosum_axes..  
-000152c0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-000152d0: 2020 2064 6566 2072 765f 6f70 2863 6c73     def rv_op(cls
-000152e0: 2c20 7369 676d 612c 206e 5f7a 6572 6f73  , sigma, n_zeros
-000152f0: 756d 5f61 7865 732c 2073 7570 706f 7274  um_axes, support
-00015300: 5f73 6861 7065 2c20 7369 7a65 3d4e 6f6e  _shape, size=Non
-00015310: 6529 3a0a 2020 2020 2020 2020 7368 6170  e):.        shap
-00015320: 6520 3d20 746f 5f74 7570 6c65 2873 697a  e = to_tuple(siz
-00015330: 6529 202b 2074 7570 6c65 2873 7570 706f  e) + tuple(suppo
-00015340: 7274 5f73 6861 7065 290a 2020 2020 2020  rt_shape).      
-00015350: 2020 6e6f 726d 616c 5f64 6973 7420 3d20    normal_dist = 
-00015360: 706d 2e4e 6f72 6d61 6c2e 6469 7374 2873  pm.Normal.dist(s
-00015370: 6967 6d61 3d73 6967 6d61 2c20 7368 6170  igma=sigma, shap
-00015380: 653d 7368 6170 6529 0a0a 2020 2020 2020  e=shape)..      
-00015390: 2020 6966 206e 5f7a 6572 6f73 756d 5f61    if n_zerosum_a
-000153a0: 7865 7320 3e20 6e6f 726d 616c 5f64 6973  xes > normal_dis
-000153b0: 742e 6e64 696d 3a0a 2020 2020 2020 2020  t.ndim:.        
-000153c0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-000153d0: 7272 6f72 2822 5368 6170 6520 6f66 2064  rror("Shape of d
-000153e0: 6973 7472 6962 7574 696f 6e20 6973 2074  istribution is t
-000153f0: 6f6f 2073 6d61 6c6c 2066 6f72 2074 6865  oo small for the
-00015400: 206e 756d 6265 7220 6f66 207a 6572 6f73   number of zeros
-00015410: 756d 2061 7865 7322 290a 0a20 2020 2020  um axes")..     
-00015420: 2020 206e 6f72 6d61 6c5f 6469 7374 5f2c     normal_dist_,
-00015430: 2073 6967 6d61 5f2c 2073 7570 706f 7274   sigma_, support
-00015440: 5f73 6861 7065 5f20 3d20 280a 2020 2020  _shape_ = (.    
-00015450: 2020 2020 2020 2020 6e6f 726d 616c 5f64          normal_d
-00015460: 6973 742e 7479 7065 2829 2c0a 2020 2020  ist.type(),.    
-00015470: 2020 2020 2020 2020 7369 676d 612e 7479          sigma.ty
-00015480: 7065 2829 2c0a 2020 2020 2020 2020 2020  pe(),.          
-00015490: 2020 7375 7070 6f72 745f 7368 6170 652e    support_shape.
-000154a0: 7479 7065 2829 2c0a 2020 2020 2020 2020  type(),.        
-000154b0: 290a 0a20 2020 2020 2020 2023 205a 6572  )..        # Zer
-000154c0: 6f73 756d 2d6e 6f72 6d61 6c69 6e67 2069  osum-normaling i
-000154d0: 7320 6163 6869 6576 6564 2062 7920 7375  s achieved by su
-000154e0: 6274 7261 6374 696e 6720 7468 6520 6d65  btracting the me
-000154f0: 616e 2061 6c6f 6e67 2074 6865 2067 6976  an along the giv
-00015500: 656e 206e 5f7a 6572 6f73 756d 5f61 7865  en n_zerosum_axe
-00015510: 730a 2020 2020 2020 2020 7a65 726f 7375  s.        zerosu
-00015520: 6d5f 7276 5f20 3d20 6e6f 726d 616c 5f64  m_rv_ = normal_d
-00015530: 6973 745f 0a20 2020 2020 2020 2066 6f72  ist_.        for
-00015540: 2061 7869 7320 696e 2072 616e 6765 286e   axis in range(n
-00015550: 5f7a 6572 6f73 756d 5f61 7865 7329 3a0a  _zerosum_axes):.
-00015560: 2020 2020 2020 2020 2020 2020 7a65 726f              zero
-00015570: 7375 6d5f 7276 5f20 2d3d 207a 6572 6f73  sum_rv_ -= zeros
-00015580: 756d 5f72 765f 2e6d 6561 6e28 6178 6973  um_rv_.mean(axis
-00015590: 3d2d 6178 6973 202d 2031 2c20 6b65 6570  =-axis - 1, keep
-000155a0: 6469 6d73 3d54 7275 6529 0a0a 2020 2020  dims=True)..    
-000155b0: 2020 2020 7265 7475 726e 205a 6572 6f53      return ZeroS
-000155c0: 756d 4e6f 726d 616c 5256 280a 2020 2020  umNormalRV(.    
-000155d0: 2020 2020 2020 2020 696e 7075 7473 3d5b          inputs=[
-000155e0: 6e6f 726d 616c 5f64 6973 745f 2c20 7369  normal_dist_, si
-000155f0: 676d 615f 2c20 7375 7070 6f72 745f 7368  gma_, support_sh
-00015600: 6170 655f 5d2c 0a20 2020 2020 2020 2020  ape_],.         
-00015610: 2020 206f 7574 7075 7473 3d5b 7a65 726f     outputs=[zero
-00015620: 7375 6d5f 7276 5f2c 2073 7570 706f 7274  sum_rv_, support
-00015630: 5f73 6861 7065 5f5d 2c0a 2020 2020 2020  _shape_],.      
-00015640: 2020 2020 2020 6e64 696d 5f73 7570 703d        ndim_supp=
-00015650: 6e5f 7a65 726f 7375 6d5f 6178 6573 2c0a  n_zerosum_axes,.
-00015660: 2020 2020 2020 2020 2928 6e6f 726d 616c          )(normal
-00015670: 5f64 6973 742c 2073 6967 6d61 2c20 7375  _dist, sigma, su
-00015680: 7070 6f72 745f 7368 6170 6529 0a0a 0a40  pport_shape)...@
-00015690: 5f63 6861 6e67 655f 6469 7374 5f73 697a  _change_dist_siz
-000156a0: 652e 7265 6769 7374 6572 285a 6572 6f53  e.register(ZeroS
-000156b0: 756d 4e6f 726d 616c 5256 290a 6465 6620  umNormalRV).def 
-000156c0: 6368 616e 6765 5f7a 6572 6f73 756d 5f73  change_zerosum_s
-000156d0: 697a 6528 6f70 2c20 6e6f 726d 616c 5f64  ize(op, normal_d
-000156e0: 6973 742c 206e 6577 5f73 697a 652c 2065  ist, new_size, e
-000156f0: 7870 616e 643d 4661 6c73 6529 3a0a 2020  xpand=False):.  
-00015700: 2020 6e6f 726d 616c 5f64 6973 742c 2073    normal_dist, s
-00015710: 6967 6d61 2c20 7375 7070 6f72 745f 7368  igma, support_sh
-00015720: 6170 6520 3d20 6e6f 726d 616c 5f64 6973  ape = normal_dis
-00015730: 742e 6f77 6e65 722e 696e 7075 7473 0a0a  t.owner.inputs..
-00015740: 2020 2020 6966 2065 7870 616e 643a 0a20      if expand:. 
-00015750: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
-00015760: 7368 6170 6520 3d20 7475 706c 6528 6e6f  shape = tuple(no
-00015770: 726d 616c 5f64 6973 742e 7368 6170 6529  rmal_dist.shape)
-00015780: 0a20 2020 2020 2020 206f 6c64 5f73 697a  .        old_siz
-00015790: 6520 3d20 6f72 6967 696e 616c 5f73 6861  e = original_sha
-000157a0: 7065 5b3a 206c 656e 286f 7269 6769 6e61  pe[: len(origina
-000157b0: 6c5f 7368 6170 6529 202d 206f 702e 6e64  l_shape) - op.nd
-000157c0: 696d 5f73 7570 705d 0a20 2020 2020 2020  im_supp].       
-000157d0: 206e 6577 5f73 697a 6520 3d20 7475 706c   new_size = tupl
-000157e0: 6528 6e65 775f 7369 7a65 2920 2b20 6f6c  e(new_size) + ol
-000157f0: 645f 7369 7a65 0a0a 2020 2020 7265 7475  d_size..    retu
-00015800: 726e 205a 6572 6f53 756d 4e6f 726d 616c  rn ZeroSumNormal
-00015810: 2e72 765f 6f70 280a 2020 2020 2020 2020  .rv_op(.        
-00015820: 7369 676d 613d 7369 676d 612c 206e 5f7a  sigma=sigma, n_z
-00015830: 6572 6f73 756d 5f61 7865 733d 6f70 2e6e  erosum_axes=op.n
-00015840: 6469 6d5f 7375 7070 2c20 7375 7070 6f72  dim_supp, suppor
-00015850: 745f 7368 6170 653d 7375 7070 6f72 745f  t_shape=support_
-00015860: 7368 6170 652c 2073 697a 653d 6e65 775f  shape, size=new_
-00015870: 7369 7a65 0a20 2020 2029 0a0a 0a40 5f6d  size.    )...@_m
-00015880: 6f6d 656e 742e 7265 6769 7374 6572 285a  oment.register(Z
-00015890: 6572 6f53 756d 4e6f 726d 616c 5256 290a  eroSumNormalRV).
-000158a0: 6465 6620 7a65 726f 7375 6d6e 6f72 6d61  def zerosumnorma
-000158b0: 6c5f 6d6f 6d65 6e74 286f 702c 2072 762c  l_moment(op, rv,
-000158c0: 202a 7276 5f69 6e70 7574 7329 3a0a 2020   *rv_inputs):.  
-000158d0: 2020 7265 7475 726e 2070 742e 7a65 726f    return pt.zero
-000158e0: 735f 6c69 6b65 2872 7629 0a0a 0a40 5f64  s_like(rv)...@_d
-000158f0: 6566 6175 6c74 5f74 7261 6e73 666f 726d  efault_transform
-00015900: 2e72 6567 6973 7465 7228 5a65 726f 5375  .register(ZeroSu
-00015910: 6d4e 6f72 6d61 6c52 5629 0a64 6566 207a  mNormalRV).def z
-00015920: 6572 6f73 756d 5f64 6566 6175 6c74 5f74  erosum_default_t
-00015930: 7261 6e73 666f 726d 286f 702c 2072 7629  ransform(op, rv)
-00015940: 3a0a 2020 2020 6e5f 7a65 726f 7375 6d5f  :.    n_zerosum_
-00015950: 6178 6573 203d 2074 7570 6c65 286e 702e  axes = tuple(np.
-00015960: 6172 616e 6765 282d 6f70 2e6e 6469 6d5f  arange(-op.ndim_
-00015970: 7375 7070 2c20 3029 290a 2020 2020 7265  supp, 0)).    re
-00015980: 7475 726e 205a 6572 6f53 756d 5472 616e  turn ZeroSumTran
-00015990: 7366 6f72 6d28 6e5f 7a65 726f 7375 6d5f  sform(n_zerosum_
-000159a0: 6178 6573 290a 0a0a 405f 6c6f 6770 726f  axes)...@_logpro
-000159b0: 622e 7265 6769 7374 6572 285a 6572 6f53  b.register(ZeroS
-000159c0: 756d 4e6f 726d 616c 5256 290a 6465 6620  umNormalRV).def 
-000159d0: 7a65 726f 7375 6d6e 6f72 6d61 6c5f 6c6f  zerosumnormal_lo
-000159e0: 6770 286f 702c 2076 616c 7565 732c 206e  gp(op, values, n
-000159f0: 6f72 6d61 6c5f 6469 7374 2c20 7369 676d  ormal_dist, sigm
-00015a00: 612c 2073 7570 706f 7274 5f73 6861 7065  a, support_shape
-00015a10: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00015a20: 2028 7661 6c75 652c 2920 3d20 7661 6c75   (value,) = valu
-00015a30: 6573 0a20 2020 2073 6861 7065 203d 2076  es.    shape = v
-00015a40: 616c 7565 2e73 6861 7065 0a20 2020 206e  alue.shape.    n
-00015a50: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
-00015a60: 6f70 2e6e 6469 6d5f 7375 7070 0a0a 2020  op.ndim_supp..  
-00015a70: 2020 5f64 6567 5f66 7265 655f 7375 7070    _deg_free_supp
-00015a80: 6f72 745f 7368 6170 6520 3d20 7074 2e69  ort_shape = pt.i
-00015a90: 6e63 5f73 7562 7465 6e73 6f72 2873 6861  nc_subtensor(sha
-00015aa0: 7065 5b2d 6e5f 7a65 726f 7375 6d5f 6178  pe[-n_zerosum_ax
-00015ab0: 6573 3a5d 2c20 2d31 290a 2020 2020 5f66  es:], -1).    _f
-00015ac0: 756c 6c5f 7369 7a65 203d 2070 742e 7072  ull_size = pt.pr
-00015ad0: 6f64 2873 6861 7065 290a 2020 2020 5f64  od(shape).    _d
-00015ae0: 6567 7265 6573 5f6f 665f 6672 6565 646f  egrees_of_freedo
-00015af0: 6d20 3d20 7074 2e70 726f 6428 5f64 6567  m = pt.prod(_deg
-00015b00: 5f66 7265 655f 7375 7070 6f72 745f 7368  _free_support_sh
-00015b10: 6170 6529 0a0a 2020 2020 7a65 726f 7375  ape)..    zerosu
-00015b20: 6d73 203d 205b 0a20 2020 2020 2020 2070  ms = [.        p
-00015b30: 742e 616c 6c28 7074 2e69 7363 6c6f 7365  t.all(pt.isclose
-00015b40: 2870 742e 6d65 616e 2876 616c 7565 2c20  (pt.mean(value, 
-00015b50: 6178 6973 3d2d 6178 6973 202d 2031 292c  axis=-axis - 1),
-00015b60: 2030 2c20 6174 6f6c 3d31 652d 3929 290a   0, atol=1e-9)).
-00015b70: 2020 2020 2020 2020 666f 7220 6178 6973          for axis
-00015b80: 2069 6e20 7261 6e67 6528 6e5f 7a65 726f   in range(n_zero
-00015b90: 7375 6d5f 6178 6573 290a 2020 2020 5d0a  sum_axes).    ].
-00015ba0: 0a20 2020 206f 7574 203d 2070 742e 7375  .    out = pt.su
-00015bb0: 6d28 0a20 2020 2020 2020 2070 6d2e 6c6f  m(.        pm.lo
-00015bc0: 6770 286e 6f72 6d61 6c5f 6469 7374 2c20  gp(normal_dist, 
-00015bd0: 7661 6c75 6529 202a 205f 6465 6772 6565  value) * _degree
-00015be0: 735f 6f66 5f66 7265 6564 6f6d 202f 205f  s_of_freedom / _
-00015bf0: 6675 6c6c 5f73 697a 652c 0a20 2020 2020  full_size,.     
-00015c00: 2020 2061 7869 733d 7475 706c 6528 6e70     axis=tuple(np
-00015c10: 2e61 7261 6e67 6528 2d6e 5f7a 6572 6f73  .arange(-n_zeros
-00015c20: 756d 5f61 7865 732c 2030 2929 2c0a 2020  um_axes, 0)),.  
-00015c30: 2020 290a 0a20 2020 2072 6574 7572 6e20    )..    return 
-00015c40: 6368 6563 6b5f 7061 7261 6d65 7465 7273  check_parameters
-00015c50: 286f 7574 2c20 2a7a 6572 6f73 756d 732c  (out, *zerosums,
-00015c60: 206d 7367 3d22 6d65 616e 2876 616c 7565   msg="mean(value
-00015c70: 2c20 6178 6973 3d6e 5f7a 6572 6f73 756d  , axis=n_zerosum
-00015c80: 5f61 7865 7329 203d 2030 2229 0a         _axes) = 0").
+0000ebd0: 2020 2020 2020 2020 2020 2073 645f 6469             sd_di
+0000ebe0: 7374 3d73 645f 6469 7374 290a 2020 2020  st=sd_dist).    
+0000ebf0: 2020 2020 2020 2020 636f 6c63 686f 6c20          colchol 
+0000ec00: 3d20 706d 2e65 7870 616e 645f 7061 636b  = pm.expand_pack
+0000ec10: 6564 5f74 7269 616e 6775 6c61 7228 332c  ed_triangular(3,
+0000ec20: 2063 6f6c 6368 6f6c 5f70 6163 6b65 6429   colchol_packed)
+0000ec30: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000ec40: 5365 7475 7020 6c65 6674 2063 6f76 6172  Setup left covar
+0000ec50: 6961 6e63 6520 6d61 7472 6978 0a20 2020  iance matrix.   
+0000ec60: 2020 2020 2020 2020 2073 6361 6c65 203d           scale =
+0000ec70: 2070 6d2e 4c6f 674e 6f72 6d61 6c28 2773   pm.LogNormal('s
+0000ec80: 6361 6c65 272c 206d 753d 6e70 2e6c 6f67  cale', mu=np.log
+0000ec90: 2874 7275 655f 7363 616c 6529 2c20 7369  (true_scale), si
+0000eca0: 676d 613d 302e 3529 0a20 2020 2020 2020  gma=0.5).       
+0000ecb0: 2020 2020 2072 6f77 636f 7620 3d20 7074       rowcov = pt
+0000ecc0: 2e64 6961 6728 5b73 6361 6c65 2a2a 2832  .diag([scale**(2
+0000ecd0: 2a69 2920 666f 7220 6920 696e 2072 616e  *i) for i in ran
+0000ece0: 6765 286d 295d 290a 0a20 2020 2020 2020  ge(m)])..       
+0000ecf0: 2020 2020 2076 616c 7320 3d20 706d 2e4d       vals = pm.M
+0000ed00: 6174 7269 784e 6f72 6d61 6c28 2776 616c  atrixNormal('val
+0000ed10: 7327 2c20 6d75 3d6d 752c 2063 6f6c 6368  s', mu=mu, colch
+0000ed20: 6f6c 3d63 6f6c 6368 6f6c 2c20 726f 7763  ol=colchol, rowc
+0000ed30: 6f76 3d72 6f77 636f 762c 0a20 2020 2020  ov=rowcov,.     
+0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed50: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+0000ed60: 7365 7276 6564 3d64 6174 6129 0a20 2020  served=data).   
+0000ed70: 2022 2222 0a20 2020 2072 765f 6f70 203d   """.    rv_op =
+0000ed80: 206d 6174 7269 786e 6f72 6d61 6c0a 0a20   matrixnormal.. 
+0000ed90: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0000eda0: 2020 2020 6465 6620 6469 7374 280a 2020      def dist(.  
+0000edb0: 2020 2020 2020 636c 732c 0a20 2020 2020        cls,.     
+0000edc0: 2020 206d 752c 0a20 2020 2020 2020 2072     mu,.        r
+0000edd0: 6f77 636f 763d 4e6f 6e65 2c0a 2020 2020  owcov=None,.    
+0000ede0: 2020 2020 726f 7763 686f 6c3d 4e6f 6e65      rowchol=None
+0000edf0: 2c0a 2020 2020 2020 2020 636f 6c63 6f76  ,.        colcov
+0000ee00: 3d4e 6f6e 652c 0a20 2020 2020 2020 2063  =None,.        c
+0000ee10: 6f6c 6368 6f6c 3d4e 6f6e 652c 0a20 2020  olchol=None,.   
+0000ee20: 2020 2020 202a 6172 6773 2c0a 2020 2020       *args,.    
+0000ee30: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
+0000ee40: 2020 293a 0a20 2020 2020 2020 2063 686f    ):.        cho
+0000ee50: 6c65 736b 7920 3d20 4368 6f6c 6573 6b79  lesky = Cholesky
+0000ee60: 286c 6f77 6572 3d54 7275 652c 206f 6e5f  (lower=True, on_
+0000ee70: 6572 726f 723d 2272 6169 7365 2229 0a0a  error="raise")..
+0000ee80: 2020 2020 2020 2020 2320 416d 6f6e 672d          # Among-
+0000ee90: 726f 7720 6d61 7472 6963 6573 0a20 2020  row matrices.   
+0000eea0: 2020 2020 2069 6620 6c65 6e28 5b69 2066       if len([i f
+0000eeb0: 6f72 2069 2069 6e20 5b72 6f77 636f 762c  or i in [rowcov,
+0000eec0: 2072 6f77 6368 6f6c 5d20 6966 2069 2069   rowchol] if i i
+0000eed0: 7320 6e6f 7420 4e6f 6e65 5d29 2021 3d20  s not None]) != 
+0000eee0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+0000eef0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000ef00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef10: 2022 496e 636f 6d70 6174 6962 6c65 2070   "Incompatible p
+0000ef20: 6172 616d 6574 6572 697a 6174 696f 6e2e  arameterization.
+0000ef30: 2053 7065 6369 6679 2065 7861 6374 6c79   Specify exactly
+0000ef40: 206f 6e65 206f 6620 726f 7763 6f76 2c20   one of rowcov, 
+0000ef50: 6f72 2072 6f77 6368 6f6c 2e22 0a20 2020  or rowchol.".   
+0000ef60: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000ef70: 2020 2069 6620 726f 7763 6f76 2069 7320     if rowcov is 
+0000ef80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000ef90: 2020 2020 2020 6966 2072 6f77 636f 762e        if rowcov.
+0000efa0: 6e64 696d 2021 3d20 323a 0a20 2020 2020  ndim != 2:.     
+0000efb0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000efc0: 2056 616c 7565 4572 726f 7228 2272 6f77   ValueError("row
+0000efd0: 636f 7620 6d75 7374 2062 6520 7477 6f20  cov must be two 
+0000efe0: 6469 6d65 6e73 696f 6e61 6c2e 2229 0a20  dimensional."). 
+0000eff0: 2020 2020 2020 2020 2020 2072 6f77 6368             rowch
+0000f000: 6f6c 5f63 6f76 203d 2063 686f 6c65 736b  ol_cov = cholesk
+0000f010: 7928 726f 7763 6f76 290a 2020 2020 2020  y(rowcov).      
+0000f020: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f030: 2020 2020 6966 2072 6f77 6368 6f6c 2e6e      if rowchol.n
+0000f040: 6469 6d20 213d 2032 3a0a 2020 2020 2020  dim != 2:.      
+0000f050: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000f060: 5661 6c75 6545 7272 6f72 2822 726f 7763  ValueError("rowc
+0000f070: 686f 6c20 6d75 7374 2062 6520 7477 6f20  hol must be two 
+0000f080: 6469 6d65 6e73 696f 6e61 6c2e 2229 0a20  dimensional."). 
+0000f090: 2020 2020 2020 2020 2020 2072 6f77 6368             rowch
+0000f0a0: 6f6c 5f63 6f76 203d 2070 742e 6173 5f74  ol_cov = pt.as_t
+0000f0b0: 656e 736f 725f 7661 7269 6162 6c65 2872  ensor_variable(r
+0000f0c0: 6f77 6368 6f6c 290a 0a20 2020 2020 2020  owchol)..       
+0000f0d0: 2023 2041 6d6f 6e67 2d63 6f6c 756d 6e20   # Among-column 
+0000f0e0: 6d61 7472 6963 6573 0a20 2020 2020 2020  matrices.       
+0000f0f0: 2069 6620 6c65 6e28 5b69 2066 6f72 2069   if len([i for i
+0000f100: 2069 6e20 5b63 6f6c 636f 762c 2063 6f6c   in [colcov, col
+0000f110: 6368 6f6c 5d20 6966 2069 2069 7320 6e6f  chol] if i is no
+0000f120: 7420 4e6f 6e65 5d29 2021 3d20 313a 0a20  t None]) != 1:. 
+0000f130: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f140: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+0000f150: 2020 2020 2020 2020 2020 2020 2022 496e               "In
+0000f160: 636f 6d70 6174 6962 6c65 2070 6172 616d  compatible param
+0000f170: 6574 6572 697a 6174 696f 6e2e 2053 7065  eterization. Spe
+0000f180: 6369 6679 2065 7861 6374 6c79 206f 6e65  cify exactly one
+0000f190: 206f 6620 636f 6c63 6f76 2c20 6f72 2063   of colcov, or c
+0000f1a0: 6f6c 6368 6f6c 2e22 0a20 2020 2020 2020  olchol.".       
+0000f1b0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+0000f1c0: 6620 636f 6c63 6f76 2069 7320 6e6f 7420  f colcov is not 
+0000f1d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f1e0: 2020 636f 6c63 6f76 203d 2070 742e 6173    colcov = pt.as
+0000f1f0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+0000f200: 2863 6f6c 636f 7629 0a20 2020 2020 2020  (colcov).       
+0000f210: 2020 2020 2069 6620 636f 6c63 6f76 2e6e       if colcov.n
+0000f220: 6469 6d20 213d 2032 3a0a 2020 2020 2020  dim != 2:.      
+0000f230: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000f240: 5661 6c75 6545 7272 6f72 2822 636f 6c63  ValueError("colc
+0000f250: 6f76 206d 7573 7420 6265 2074 776f 2064  ov must be two d
+0000f260: 696d 656e 7369 6f6e 616c 2e22 290a 2020  imensional.").  
+0000f270: 2020 2020 2020 2020 2020 636f 6c63 686f            colcho
+0000f280: 6c5f 636f 7620 3d20 6368 6f6c 6573 6b79  l_cov = cholesky
+0000f290: 2863 6f6c 636f 7629 0a20 2020 2020 2020  (colcov).       
+0000f2a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f2b0: 2020 2069 6620 636f 6c63 686f 6c2e 6e64     if colchol.nd
+0000f2c0: 696d 2021 3d20 323a 0a20 2020 2020 2020  im != 2:.       
+0000f2d0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000f2e0: 616c 7565 4572 726f 7228 2263 6f6c 6368  alueError("colch
+0000f2f0: 6f6c 206d 7573 7420 6265 2074 776f 2064  ol must be two d
+0000f300: 696d 656e 7369 6f6e 616c 2e22 290a 2020  imensional.").  
+0000f310: 2020 2020 2020 2020 2020 636f 6c63 686f            colcho
+0000f320: 6c5f 636f 7620 3d20 7074 2e61 735f 7465  l_cov = pt.as_te
+0000f330: 6e73 6f72 5f76 6172 6961 626c 6528 636f  nsor_variable(co
+0000f340: 6c63 686f 6c29 0a0a 2020 2020 2020 2020  lchol)..        
+0000f350: 6469 7374 5f73 6861 7065 203d 2028 726f  dist_shape = (ro
+0000f360: 7763 686f 6c5f 636f 762e 7368 6170 655b  wchol_cov.shape[
+0000f370: 2d31 5d2c 2063 6f6c 6368 6f6c 5f63 6f76  -1], colchol_cov
+0000f380: 2e73 6861 7065 5b2d 315d 290a 0a20 2020  .shape[-1])..   
+0000f390: 2020 2020 2023 2042 726f 6164 6361 7374       # Broadcast
+0000f3a0: 696e 6720 6d75 0a20 2020 2020 2020 206d  ing mu.        m
+0000f3b0: 7520 3d20 7074 2e65 7874 7261 5f6f 7073  u = pt.extra_ops
+0000f3c0: 2e62 726f 6164 6361 7374 5f74 6f28 6d75  .broadcast_to(mu
+0000f3d0: 2c20 7368 6170 653d 6469 7374 5f73 6861  , shape=dist_sha
+0000f3e0: 7065 290a 2020 2020 2020 2020 6d75 203d  pe).        mu =
+0000f3f0: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+0000f400: 7269 6162 6c65 2866 6c6f 6174 5828 6d75  riable(floatX(mu
+0000f410: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
+0000f420: 726e 2073 7570 6572 2829 2e64 6973 7428  rn super().dist(
+0000f430: 5b6d 752c 2072 6f77 6368 6f6c 5f63 6f76  [mu, rowchol_cov
+0000f440: 2c20 636f 6c63 686f 6c5f 636f 765d 2c20  , colchol_cov], 
+0000f450: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
+0000f460: 6566 206d 6f6d 656e 7428 7276 2c20 7369  ef moment(rv, si
+0000f470: 7a65 2c20 6d75 2c20 726f 7763 686f 6c2c  ze, mu, rowchol,
+0000f480: 2063 6f6c 6368 6f6c 293a 0a20 2020 2020   colchol):.     
+0000f490: 2020 2072 6574 7572 6e20 7074 2e66 756c     return pt.ful
+0000f4a0: 6c5f 6c69 6b65 2872 762c 206d 7529 0a0a  l_like(rv, mu)..
+0000f4b0: 2020 2020 6465 6620 6c6f 6770 2876 616c      def logp(val
+0000f4c0: 7565 2c20 6d75 2c20 726f 7763 686f 6c2c  ue, mu, rowchol,
+0000f4d0: 2063 6f6c 6368 6f6c 293a 0a20 2020 2020   colchol):.     
+0000f4e0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000f4f0: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
+0000f500: 6261 6269 6c69 7479 206f 6620 4d61 7472  bability of Matr
+0000f510: 6978 2d76 616c 7565 6420 4e6f 726d 616c  ix-valued Normal
+0000f520: 2064 6973 7472 6962 7574 696f 6e0a 2020   distribution.  
+0000f530: 2020 2020 2020 6174 2073 7065 6369 6669        at specifi
+0000f540: 6564 2076 616c 7565 2e0a 0a20 2020 2020  ed value...     
+0000f550: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000f560: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000f570: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
+0000f580: 6e75 6d65 7269 630a 2020 2020 2020 2020  numeric.        
+0000f590: 2020 2020 5661 6c75 6520 666f 7220 7768      Value for wh
+0000f5a0: 6963 6820 6c6f 672d 7072 6f62 6162 696c  ich log-probabil
+0000f5b0: 6974 7920 6973 2063 616c 6375 6c61 7465  ity is calculate
+0000f5c0: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
+0000f5d0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000f5e0: 2d2d 2d0a 2020 2020 2020 2020 5465 6e73  ---.        Tens
+0000f5f0: 6f72 5661 7269 6162 6c65 0a20 2020 2020  orVariable.     
+0000f600: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000f610: 6966 2076 616c 7565 2e6e 6469 6d20 213d  if value.ndim !=
+0000f620: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0000f630: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000f640: 2822 5661 6c75 6520 6d75 7374 2062 6520  ("Value must be 
+0000f650: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
+0000f660: 2229 0a0a 2020 2020 2020 2020 2320 436f  ")..        # Co
+0000f670: 6d70 7574 6520 5472 5b63 6f6c 636f 765e  mpute Tr[colcov^
+0000f680: 2d31 2040 2028 7820 2d20 6d75 292e 5420  -1 @ (x - mu).T 
+0000f690: 4020 726f 7763 6f76 5e2d 3120 4020 2878  @ rowcov^-1 @ (x
+0000f6a0: 202d 206d 7529 5d20 616e 640a 2020 2020   - mu)] and.    
+0000f6b0: 2020 2020 2320 7468 6520 6c6f 6764 6574      # the logdet
+0000f6c0: 206f 6620 636f 6c63 6f76 2061 6e64 2072   of colcov and r
+0000f6d0: 6f77 636f 762e 0a20 2020 2020 2020 2064  owcov..        d
+0000f6e0: 656c 7461 203d 2076 616c 7565 202d 206d  elta = value - m
+0000f6f0: 750a 0a20 2020 2020 2020 2023 2046 696e  u..        # Fin
+0000f700: 6420 6578 706f 6e65 6e74 2070 6965 6365  d exponent piece
+0000f710: 2062 7920 7069 6563 650a 2020 2020 2020   by piece.      
+0000f720: 2020 7269 6768 745f 7175 6164 6469 7374    right_quaddist
+0000f730: 203d 2073 6f6c 7665 5f6c 6f77 6572 2872   = solve_lower(r
+0000f740: 6f77 6368 6f6c 2c20 6465 6c74 6129 0a20  owchol, delta). 
+0000f750: 2020 2020 2020 2071 7561 6464 6973 7420         quaddist 
+0000f760: 3d20 7074 2e6e 6c69 6e61 6c67 2e6d 6174  = pt.nlinalg.mat
+0000f770: 7269 785f 646f 7428 7269 6768 745f 7175  rix_dot(right_qu
+0000f780: 6164 6469 7374 2e54 2c20 7269 6768 745f  addist.T, right_
+0000f790: 7175 6164 6469 7374 290a 2020 2020 2020  quaddist).      
+0000f7a0: 2020 7175 6164 6469 7374 203d 2073 6f6c    quaddist = sol
+0000f7b0: 7665 5f6c 6f77 6572 2863 6f6c 6368 6f6c  ve_lower(colchol
+0000f7c0: 2c20 7175 6164 6469 7374 290a 2020 2020  , quaddist).    
+0000f7d0: 2020 2020 7175 6164 6469 7374 203d 2073      quaddist = s
+0000f7e0: 6f6c 7665 5f75 7070 6572 2863 6f6c 6368  olve_upper(colch
+0000f7f0: 6f6c 2e54 2c20 7175 6164 6469 7374 290a  ol.T, quaddist).
+0000f800: 2020 2020 2020 2020 7472 7175 6164 6469          trquaddi
+0000f810: 7374 203d 2070 742e 6e6c 696e 616c 672e  st = pt.nlinalg.
+0000f820: 7472 6163 6528 7175 6164 6469 7374 290a  trace(quaddist).
+0000f830: 0a20 2020 2020 2020 2063 6f6c 6469 6167  .        coldiag
+0000f840: 203d 2070 742e 6469 6167 2863 6f6c 6368   = pt.diag(colch
+0000f850: 6f6c 290a 2020 2020 2020 2020 726f 7764  ol).        rowd
+0000f860: 6961 6720 3d20 7074 2e64 6961 6728 726f  iag = pt.diag(ro
+0000f870: 7763 686f 6c29 0a20 2020 2020 2020 2068  wchol).        h
+0000f880: 616c 665f 636f 6c6c 6f67 6465 7420 3d20  alf_collogdet = 
+0000f890: 7074 2e73 756d 2870 742e 6c6f 6728 636f  pt.sum(pt.log(co
+0000f8a0: 6c64 6961 6729 2920 2023 206c 6f67 6465  ldiag))  # logde
+0000f8b0: 7428 4d29 203d 2032 2a54 7228 6c6f 6728  t(M) = 2*Tr(log(
+0000f8c0: 4c29 290a 2020 2020 2020 2020 6861 6c66  L)).        half
+0000f8d0: 5f72 6f77 6c6f 6764 6574 203d 2070 742e  _rowlogdet = pt.
+0000f8e0: 7375 6d28 7074 2e6c 6f67 2872 6f77 6469  sum(pt.log(rowdi
+0000f8f0: 6167 2929 2020 2320 5573 696e 6720 4368  ag))  # Using Ch
+0000f900: 6f6c 6573 6b79 3a20 4d20 3d20 4c20 4c5e  olesky: M = L L^
+0000f910: 540a 0a20 2020 2020 2020 206d 203d 2072  T..        m = r
+0000f920: 6f77 6368 6f6c 2e73 6861 7065 5b30 5d0a  owchol.shape[0].
+0000f930: 2020 2020 2020 2020 6e20 3d20 636f 6c63          n = colc
+0000f940: 686f 6c2e 7368 6170 655b 305d 0a0a 2020  hol.shape[0]..  
+0000f950: 2020 2020 2020 6e6f 726d 203d 202d 302e        norm = -0.
+0000f960: 3520 2a20 6d20 2a20 6e20 2a20 706d 2e66  5 * m * n * pm.f
+0000f970: 6c6f 6174 5828 6e70 2e6c 6f67 2832 202a  loatX(np.log(2 *
+0000f980: 206e 702e 7069 2929 0a20 2020 2020 2020   np.pi)).       
+0000f990: 2072 6574 7572 6e20 6e6f 726d 202d 2030   return norm - 0
+0000f9a0: 2e35 202a 2074 7271 7561 6464 6973 7420  .5 * trquaddist 
+0000f9b0: 2d20 6d20 2a20 6861 6c66 5f63 6f6c 6c6f  - m * half_collo
+0000f9c0: 6764 6574 202d 206e 202a 2068 616c 665f  gdet - n * half_
+0000f9d0: 726f 776c 6f67 6465 740a 0a0a 636c 6173  rowlogdet...clas
+0000f9e0: 7320 4b72 6f6e 6563 6b65 724e 6f72 6d61  s KroneckerNorma
+0000f9f0: 6c52 5628 5261 6e64 6f6d 5661 7269 6162  lRV(RandomVariab
+0000fa00: 6c65 293a 0a20 2020 206e 616d 6520 3d20  le):.    name = 
+0000fa10: 226b 726f 6e65 636b 6572 6e6f 726d 616c  "kroneckernormal
+0000fa20: 220a 2020 2020 6e64 696d 5f73 7570 7020  ".    ndim_supp 
+0000fa30: 3d20 310a 2020 2020 6e64 696d 735f 7061  = 1.    ndims_pa
+0000fa40: 7261 6d73 203d 205b 312c 2030 2c20 325d  rams = [1, 0, 2]
+0000fa50: 0a20 2020 2064 7479 7065 203d 2022 666c  .    dtype = "fl
+0000fa60: 6f61 7458 220a 2020 2020 5f70 7269 6e74  oatX".    _print
+0000fa70: 5f6e 616d 6520 3d20 2822 4b72 6f6e 6563  _name = ("Kronec
+0000fa80: 6b65 724e 6f72 6d61 6c22 2c20 225c 5c6f  kerNormal", "\\o
+0000fa90: 7065 7261 746f 726e 616d 657b 4b72 6f6e  peratorname{Kron
+0000faa0: 6563 6b65 724e 6f72 6d61 6c7d 2229 0a0a  eckerNormal}")..
+0000fab0: 2020 2020 6465 6620 5f73 7570 705f 7368      def _supp_sh
+0000fac0: 6170 655f 6672 6f6d 5f70 6172 616d 7328  ape_from_params(
+0000fad0: 7365 6c66 2c20 6469 7374 5f70 6172 616d  self, dist_param
+0000fae0: 732c 2070 6172 616d 5f73 6861 7065 733d  s, param_shapes=
+0000faf0: 4e6f 6e65 293a 0a20 2020 2020 2020 2072  None):.        r
+0000fb00: 6574 7572 6e20 7375 7070 5f73 6861 7065  eturn supp_shape
+0000fb10: 5f66 726f 6d5f 7265 665f 7061 7261 6d5f  _from_ref_param_
+0000fb20: 7368 6170 6528 0a20 2020 2020 2020 2020  shape(.         
+0000fb30: 2020 206e 6469 6d5f 7375 7070 3d73 656c     ndim_supp=sel
+0000fb40: 662e 6e64 696d 5f73 7570 702c 0a20 2020  f.ndim_supp,.   
+0000fb50: 2020 2020 2020 2020 2064 6973 745f 7061           dist_pa
+0000fb60: 7261 6d73 3d64 6973 745f 7061 7261 6d73  rams=dist_params
+0000fb70: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+0000fb80: 7261 6d5f 7368 6170 6573 3d70 6172 616d  ram_shapes=param
+0000fb90: 5f73 6861 7065 732c 0a20 2020 2020 2020  _shapes,.       
+0000fba0: 2020 2020 2072 6566 5f70 6172 616d 5f69       ref_param_i
+0000fbb0: 6478 3d30 2c0a 2020 2020 2020 2020 290a  dx=0,.        ).
+0000fbc0: 0a20 2020 2064 6566 2072 6e67 5f66 6e28  .    def rng_fn(
+0000fbd0: 7365 6c66 2c20 726e 672c 206d 752c 2073  self, rng, mu, s
+0000fbe0: 6967 6d61 2c20 2a63 6f76 732c 2073 697a  igma, *covs, siz
+0000fbf0: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
+0000fc00: 2073 697a 6520 3d20 7369 7a65 2069 6620   size = size if 
+0000fc10: 7369 7a65 2065 6c73 6520 636f 7673 5b2d  size else covs[-
+0000fc20: 315d 0a20 2020 2020 2020 2063 6f76 7320  1].        covs 
+0000fc30: 3d20 636f 7673 5b3a 2d31 5d20 6966 2063  = covs[:-1] if c
+0000fc40: 6f76 735b 2d31 5d20 3d3d 2073 697a 6520  ovs[-1] == size 
+0000fc50: 656c 7365 2063 6f76 730a 0a20 2020 2020  else covs..     
+0000fc60: 2020 2063 6f76 203d 2072 6564 7563 6528     cov = reduce(
+0000fc70: 6c69 6e61 6c67 2e6b 726f 6e2c 2063 6f76  linalg.kron, cov
+0000fc80: 7329 0a0a 2020 2020 2020 2020 6966 2073  s)..        if s
+0000fc90: 6967 6d61 3a0a 2020 2020 2020 2020 2020  igma:.          
+0000fca0: 2020 636f 7620 3d20 636f 7620 2b20 7369    cov = cov + si
+0000fcb0: 676d 612a 2a32 202a 206e 702e 6579 6528  gma**2 * np.eye(
+0000fcc0: 636f 762e 7368 6170 655b 305d 290a 0a20  cov.shape[0]).. 
+0000fcd0: 2020 2020 2020 2078 203d 206d 756c 7469         x = multi
+0000fce0: 7661 7269 6174 655f 6e6f 726d 616c 2e72  variate_normal.r
+0000fcf0: 6e67 5f66 6e28 726e 673d 726e 672c 206d  ng_fn(rng=rng, m
+0000fd00: 6561 6e3d 6d75 2c20 636f 763d 636f 762c  ean=mu, cov=cov,
+0000fd10: 2073 697a 653d 7369 7a65 290a 2020 2020   size=size).    
+0000fd20: 2020 2020 7265 7475 726e 2078 0a0a 0a6b      return x...k
+0000fd30: 726f 6e65 636b 6572 6e6f 726d 616c 203d  roneckernormal =
+0000fd40: 204b 726f 6e65 636b 6572 4e6f 726d 616c   KroneckerNormal
+0000fd50: 5256 2829 0a0a 0a63 6c61 7373 204b 726f  RV()...class Kro
+0000fd60: 6e65 636b 6572 4e6f 726d 616c 2843 6f6e  neckerNormal(Con
+0000fd70: 7469 6e75 6f75 7329 3a0a 2020 2020 7222  tinuous):.    r"
+0000fd80: 2222 0a20 2020 204d 756c 7469 7661 7269  "".    Multivari
+0000fd90: 6174 6520 6e6f 726d 616c 206c 6f67 2d6c  ate normal log-l
+0000fda0: 696b 656c 6968 6f6f 6420 7769 7468 204b  ikelihood with K
+0000fdb0: 726f 6e65 636b 6572 2d73 7472 7563 7475  ronecker-structu
+0000fdc0: 7265 6420 636f 7661 7269 616e 6365 2e0a  red covariance..
+0000fdd0: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a0a  .    .. math::..
+0000fde0: 2020 2020 2020 2066 2878 205c 6d69 6420         f(x \mid 
+0000fdf0: 5c6d 752c 204b 2920 3d0a 2020 2020 2020  \mu, K) =.      
+0000fe00: 2020 2020 205c 6672 6163 7b31 7d7b 2832       \frac{1}{(2
+0000fe10: 5c70 6920 7c4b 7c29 5e7b 312f 327d 7d0a  \pi |K|)^{1/2}}.
+0000fe20: 2020 2020 2020 2020 2020 205c 6578 705c             \exp\
+0000fe30: 6c65 6674 5c7b 202d 5c66 7261 637b 317d  left\{ -\frac{1}
+0000fe40: 7b32 7d20 2878 2d5c 6d75 295e 7b5c 7072  {2} (x-\mu)^{\pr
+0000fe50: 696d 657d 204b 5e7b 2d31 7d20 2878 2d5c  ime} K^{-1} (x-\
+0000fe60: 6d75 2920 5c72 6967 6874 5c7d 0a0a 2020  mu) \right\}..  
+0000fe70: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
+0000fe80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fe90: 3d3d 3d3d 3d3d 0a20 2020 2053 7570 706f  ======.    Suppo
+0000fea0: 7274 2020 203a 6d61 7468 3a60 7820 5c69  rt   :math:`x \i
+0000feb0: 6e20 5c6d 6174 6862 627b 527d 5e4e 600a  n \mathbb{R}^N`.
+0000fec0: 2020 2020 4d65 616e 2020 2020 2020 3a6d      Mean      :m
+0000fed0: 6174 683a 605c 6d75 600a 2020 2020 5661  ath:`\mu`.    Va
+0000fee0: 7269 616e 6365 2020 3a6d 6174 683a 604b  riance  :math:`K
+0000fef0: 203d 205c 6269 676f 7469 6d65 7320 4b5f   = \bigotimes K_
+0000ff00: 6920 2b20 5c73 6967 6d61 5e32 2049 5f4e  i + \sigma^2 I_N
+0000ff10: 600a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  `.    ========  
+0000ff20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ff30: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
+0000ff40: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000ff50: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6d75  ---------.    mu
+0000ff60: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+0000ff70: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+0000ff80: 5665 6374 6f72 206f 6620 6d65 616e 732c  Vector of means,
+0000ff90: 206a 7573 7420 6173 2069 6e20 604d 764e   just as in `MvN
+0000ffa0: 6f72 6d61 6c60 2e0a 2020 2020 636f 7673  ormal`..    covs
+0000ffb0: 203a 206c 6973 7420 6f66 2061 7272 6179   : list of array
+0000ffc0: 730a 2020 2020 2020 2020 5468 6520 7365  s.        The se
+0000ffd0: 7420 6f66 2063 6f76 6172 6961 6e63 6520  t of covariance 
+0000ffe0: 6d61 7472 6963 6573 203a 6d61 7468 3a60  matrices :math:`
+0000fff0: 5b4b 5f31 2c20 4b5f 322c 202e 2e2e 5d60  [K_1, K_2, ...]`
+00010000: 2074 6f20 6265 0a20 2020 2020 2020 204b   to be.        K
+00010010: 726f 6e65 636b 6572 6564 2069 6e20 7468  roneckered in th
+00010020: 6520 6f72 6465 7220 7072 6f76 6964 6564  e order provided
+00010030: 203a 6d61 7468 3a60 5c62 6967 6f74 696d   :math:`\bigotim
+00010040: 6573 204b 5f69 602e 0a20 2020 2063 686f  es K_i`..    cho
+00010050: 6c73 203a 206c 6973 7420 6f66 2061 7272  ls : list of arr
+00010060: 6179 730a 2020 2020 2020 2020 5468 6520  ays.        The 
+00010070: 7365 7420 6f66 206c 6f77 6572 2063 686f  set of lower cho
+00010080: 6c65 736b 7920 6d61 7472 6963 6573 203a  lesky matrices :
+00010090: 6d61 7468 3a60 5b4c 5f31 2c20 4c5f 322c  math:`[L_1, L_2,
+000100a0: 202e 2e2e 5d60 2073 7563 6820 7468 6174   ...]` such that
+000100b0: 0a20 2020 2020 2020 203a 6d61 7468 3a60  .        :math:`
+000100c0: 4b5f 6920 3d20 4c5f 6920 4c5f 6927 602e  K_i = L_i L_i'`.
+000100d0: 0a20 2020 2065 7664 7320 3a20 6c69 7374  .    evds : list
+000100e0: 206f 6620 7475 706c 6573 0a20 2020 2020   of tuples.     
+000100f0: 2020 2054 6865 2073 6574 206f 6620 6569     The set of ei
+00010100: 6765 6e76 616c 7565 2d76 6563 746f 722c  genvalue-vector,
+00010110: 2065 6967 656e 7665 6374 6f72 2d6d 6174   eigenvector-mat
+00010120: 7269 7820 7061 6972 730a 2020 2020 2020  rix pairs.      
+00010130: 2020 3a6d 6174 683a 605b 2876 5f31 2c20    :math:`[(v_1, 
+00010140: 515f 3129 2c20 2876 5f32 2c20 515f 3229  Q_1), (v_2, Q_2)
+00010150: 2c20 2e2e 2e5d 6020 7375 6368 2074 6861  , ...]` such tha
+00010160: 740a 2020 2020 2020 2020 3a6d 6174 683a  t.        :math:
+00010170: 604b 5f69 203d 2051 5f69 205c 7465 7874  `K_i = Q_i \text
+00010180: 7b64 6961 677d 2876 5f69 2920 515f 6927  {diag}(v_i) Q_i'
+00010190: 602e 2046 6f72 2065 7861 6d70 6c65 3a3a  `. For example::
+000101a0: 0a0a 2020 2020 2020 2020 2020 2020 765f  ..            v_
+000101b0: 692c 2051 5f69 203d 2070 742e 6e6c 696e  i, Q_i = pt.nlin
+000101c0: 616c 672e 6569 6768 284b 5f69 290a 2020  alg.eigh(K_i).  
+000101d0: 2020 7369 676d 6120 3a20 7363 616c 6172    sigma : scalar
+000101e0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000101f0: 2020 2053 7461 6e64 6172 6420 6465 7669     Standard devi
+00010200: 6174 696f 6e20 6f66 2074 6865 2047 6175  ation of the Gau
+00010210: 7373 6961 6e20 7768 6974 6520 6e6f 6973  ssian white nois
+00010220: 652e 0a0a 2020 2020 4578 616d 706c 6573  e...    Examples
+00010230: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
+00010240: 2020 4465 6669 6e65 2061 206d 756c 7469    Define a multi
+00010250: 7661 7269 6174 6520 6e6f 726d 616c 2076  variate normal v
+00010260: 6172 6961 626c 6520 7769 7468 2061 2063  ariable with a c
+00010270: 6f76 6172 6961 6e63 650a 2020 2020 3a6d  ovariance.    :m
+00010280: 6174 683a 604b 203d 204b 5f31 205c 6f74  ath:`K = K_1 \ot
+00010290: 696d 6573 204b 5f32 600a 0a20 2020 202e  imes K_2`..    .
+000102a0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
+000102b0: 0a20 2020 2020 2020 204b 3120 3d20 6e70  .        K1 = np
+000102c0: 2e61 7272 6179 285b 5b31 2e2c 2030 2e35  .array([[1., 0.5
+000102d0: 5d2c 205b 302e 352c 2032 5d5d 290a 2020  ], [0.5, 2]]).  
+000102e0: 2020 2020 2020 4b32 203d 206e 702e 6172        K2 = np.ar
+000102f0: 7261 7928 5b5b 312e 2c20 302e 342c 2030  ray([[1., 0.4, 0
+00010300: 2e32 5d2c 205b 302e 342c 2032 2c20 302e  .2], [0.4, 2, 0.
+00010310: 335d 2c20 5b30 2e32 2c20 302e 332c 2031  3], [0.2, 0.3, 1
+00010320: 5d5d 290a 2020 2020 2020 2020 636f 7673  ]]).        covs
+00010330: 203d 205b 4b31 2c20 4b32 5d0a 2020 2020   = [K1, K2].    
+00010340: 2020 2020 4e20 3d20 360a 2020 2020 2020      N = 6.      
+00010350: 2020 6d75 203d 206e 702e 7a65 726f 7328    mu = np.zeros(
+00010360: 4e29 0a20 2020 2020 2020 2077 6974 6820  N).        with 
+00010370: 706d 2e4d 6f64 656c 2829 2061 7320 6d6f  pm.Model() as mo
+00010380: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
+00010390: 2076 616c 7320 3d20 706d 2e4b 726f 6e65   vals = pm.Krone
+000103a0: 636b 6572 4e6f 726d 616c 2827 7661 6c73  ckerNormal('vals
+000103b0: 272c 206d 753d 6d75 2c20 636f 7673 3d63  ', mu=mu, covs=c
+000103c0: 6f76 732c 2073 6861 7065 3d4e 290a 0a20  ovs, shape=N).. 
+000103d0: 2020 2045 6666 6963 6965 6e63 7920 6761     Efficiency ga
+000103e0: 696e 7320 6172 6520 6d61 6465 2062 7920  ins are made by 
+000103f0: 6368 6f6c 6573 6b79 2064 6563 6f6d 706f  cholesky decompo
+00010400: 7369 6e67 203a 6d61 7468 3a60 4b5f 3160  sing :math:`K_1`
+00010410: 2061 6e64 0a20 2020 203a 6d61 7468 3a60   and.    :math:`
+00010420: 4b5f 3260 2069 6e64 6976 6964 7561 6c6c  K_2` individuall
+00010430: 7920 7261 7468 6572 2074 6861 6e20 7468  y rather than th
+00010440: 6520 6c61 7267 6572 203a 6d61 7468 3a60  e larger :math:`
+00010450: 4b60 206d 6174 7269 782e 2041 6c74 686f  K` matrix. Altho
+00010460: 7567 680a 2020 2020 6f6e 6c79 2074 776f  ugh.    only two
+00010470: 206d 6174 7269 6365 7320 3a6d 6174 683a   matrices :math:
+00010480: 604b 5f31 6020 616e 6420 3a6d 6174 683a  `K_1` and :math:
+00010490: 604b 5f32 6020 6172 6520 7368 6f77 6e20  `K_2` are shown 
+000104a0: 6865 7265 2c20 616e 2061 7262 6974 7261  here, an arbitra
+000104b0: 7279 0a20 2020 206e 756d 6265 7220 6f66  ry.    number of
+000104c0: 2073 7562 6d61 7472 6963 6573 2063 616e   submatrices can
+000104d0: 2062 6520 636f 6d62 696e 6564 2069 6e20   be combined in 
+000104e0: 7468 6973 2077 6179 2e20 4368 6f6c 6573  this way. Choles
+000104f0: 6b79 7320 616e 640a 2020 2020 6569 6765  kys and.    eige
+00010500: 6e64 6563 6f6d 706f 7369 7469 6f6e 7320  ndecompositions 
+00010510: 6361 6e20 6265 2070 726f 7669 6465 6420  can be provided 
+00010520: 696e 7374 6561 640a 0a20 2020 202e 2e20  instead..    .. 
+00010530: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
+00010540: 2020 2020 2020 2063 686f 6c73 203d 205b         chols = [
+00010550: 6e70 2e6c 696e 616c 672e 6368 6f6c 6573  np.linalg.choles
+00010560: 6b79 284b 6929 2066 6f72 204b 6920 696e  ky(Ki) for Ki in
+00010570: 2063 6f76 735d 0a20 2020 2020 2020 2065   covs].        e
+00010580: 7664 7320 3d20 5b6e 702e 6c69 6e61 6c67  vds = [np.linalg
+00010590: 2e65 6967 6828 4b69 2920 666f 7220 4b69  .eigh(Ki) for Ki
+000105a0: 2069 6e20 636f 7673 5d0a 2020 2020 2020   in covs].      
+000105b0: 2020 7769 7468 2070 6d2e 4d6f 6465 6c28    with pm.Model(
+000105c0: 2920 6173 206d 6f64 656c 3a0a 2020 2020  ) as model:.    
+000105d0: 2020 2020 2020 2020 7661 6c73 3220 3d20          vals2 = 
+000105e0: 706d 2e4b 726f 6e65 636b 6572 4e6f 726d  pm.KroneckerNorm
+000105f0: 616c 2827 7661 6c73 3227 2c20 6d75 3d6d  al('vals2', mu=m
+00010600: 752c 2063 686f 6c73 3d63 686f 6c73 2c20  u, chols=chols, 
+00010610: 7368 6170 653d 4e29 0a20 2020 2020 2020  shape=N).       
+00010620: 2020 2020 2023 206f 720a 2020 2020 2020       # or.      
+00010630: 2020 2020 2020 7661 6c73 3320 3d20 706d        vals3 = pm
+00010640: 2e4b 726f 6e65 636b 6572 4e6f 726d 616c  .KroneckerNormal
+00010650: 2827 7661 6c73 3327 2c20 6d75 3d6d 752c  ('vals3', mu=mu,
+00010660: 2065 7664 733d 6576 6473 2c20 7368 6170   evds=evds, shap
+00010670: 653d 4e29 0a0a 2020 2020 6e65 6974 6865  e=N)..    neithe
+00010680: 7220 6f66 2077 6869 6368 2077 696c 6c20  r of which will 
+00010690: 6265 2063 6f6e 7665 7274 6564 2e20 4469  be converted. Di
+000106a0: 6167 6f6e 616c 206e 6f69 7365 2063 616e  agonal noise can
+000106b0: 2061 6c73 6f20 6265 2061 6464 6564 2074   also be added t
+000106c0: 6f0a 2020 2020 7468 6520 636f 7661 7269  o.    the covari
+000106d0: 616e 6365 206d 6174 7269 782c 203a 6d61  ance matrix, :ma
+000106e0: 7468 3a60 4b20 3d20 4b5f 3120 5c6f 7469  th:`K = K_1 \oti
+000106f0: 6d65 7320 4b5f 3220 2b20 5c73 6967 6d61  mes K_2 + \sigma
+00010700: 5e32 2049 5f4e 602e 0a20 2020 2044 6573  ^2 I_N`..    Des
+00010710: 7069 7465 2074 6865 206e 6f69 7365 2072  pite the noise r
+00010720: 656d 6f76 696e 6720 7468 6520 6f76 6572  emoving the over
+00010730: 616c 6c20 4b72 6f6e 6563 6b65 7220 7374  all Kronecker st
+00010740: 7275 6374 7572 6520 6f66 2074 6865 206d  ructure of the m
+00010750: 6174 7269 782c 0a20 2020 2060 4b72 6f6e  atrix,.    `Kron
+00010760: 6563 6b65 724e 6f72 6d61 6c60 2063 616e  eckerNormal` can
+00010770: 2063 6f6e 7469 6e75 6520 746f 206d 616b   continue to mak
+00010780: 6520 6566 6669 6369 656e 7420 6361 6c63  e efficient calc
+00010790: 756c 6174 696f 6e73 2062 790a 2020 2020  ulations by.    
+000107a0: 7574 696c 697a 696e 6720 6569 6765 6e64  utilizing eigend
+000107b0: 6563 6f6d 706f 7369 746f 6e73 206f 6620  ecompositons of 
+000107c0: 7468 6520 7375 626d 6174 7269 6365 7320  the submatrices 
+000107d0: 6265 6869 6e64 2074 6865 2073 6365 6e65  behind the scene
+000107e0: 7320 5b31 5d2e 0a20 2020 2054 6875 732c  s [1]..    Thus,
+000107f0: 0a0a 2020 2020 2e2e 2063 6f64 653a 3a20  ..    .. code:: 
+00010800: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00010810: 7369 676d 6120 3d20 302e 310a 2020 2020  sigma = 0.1.    
+00010820: 2020 2020 7769 7468 2070 6d2e 4d6f 6465      with pm.Mode
+00010830: 6c28 2920 6173 206e 6f69 7365 5f6d 6f64  l() as noise_mod
+00010840: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+00010850: 7661 6c73 203d 2070 6d2e 4b72 6f6e 6563  vals = pm.Kronec
+00010860: 6b65 724e 6f72 6d61 6c28 2776 616c 7327  kerNormal('vals'
+00010870: 2c20 6d75 3d6d 752c 2063 6f76 733d 636f  , mu=mu, covs=co
+00010880: 7673 2c20 7369 676d 613d 7369 676d 612c  vs, sigma=sigma,
+00010890: 2073 6861 7065 3d4e 290a 2020 2020 2020   shape=N).      
+000108a0: 2020 2020 2020 7661 6c73 3220 3d20 706d        vals2 = pm
+000108b0: 2e4b 726f 6e65 636b 6572 4e6f 726d 616c  .KroneckerNormal
+000108c0: 2827 7661 6c73 3227 2c20 6d75 3d6d 752c  ('vals2', mu=mu,
+000108d0: 2063 686f 6c73 3d63 686f 6c73 2c20 7369   chols=chols, si
+000108e0: 676d 613d 7369 676d 612c 2073 6861 7065  gma=sigma, shape
+000108f0: 3d4e 290a 2020 2020 2020 2020 2020 2020  =N).            
+00010900: 7661 6c73 3320 3d20 706d 2e4b 726f 6e65  vals3 = pm.Krone
+00010910: 636b 6572 4e6f 726d 616c 2827 7661 6c73  ckerNormal('vals
+00010920: 3327 2c20 6d75 3d6d 752c 2065 7664 733d  3', mu=mu, evds=
+00010930: 6576 6473 2c20 7369 676d 613d 7369 676d  evds, sigma=sigm
+00010940: 612c 2073 6861 7065 3d4e 290a 0a20 2020  a, shape=N)..   
+00010950: 2061 7265 2069 6465 6e74 6963 616c 2c20   are identical, 
+00010960: 7769 7468 2060 636f 7673 6020 616e 6420  with `covs` and 
+00010970: 6063 686f 6c73 6020 6561 6368 2063 6f6e  `chols` each con
+00010980: 7665 7274 6564 2074 6f0a 2020 2020 6569  verted to.    ei
+00010990: 6765 6e64 6563 6f6d 706f 7369 7469 6f6e  gendecomposition
+000109a0: 732e 0a0a 2020 2020 5265 6665 7265 6e63  s...    Referenc
+000109b0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  es.    ---------
+000109c0: 2d0a 2020 2020 2e2e 205b 315d 2053 6161  -.    .. [1] Saa
+000109d0: 7463 6869 2c20 592e 2028 3230 3131 292e  tchi, Y. (2011).
+000109e0: 2022 5363 616c 6162 6c65 2069 6e66 6572   "Scalable infer
+000109f0: 656e 6365 2066 6f72 2073 7472 7563 7475  ence for structu
+00010a00: 7265 6420 4761 7573 7369 616e 2070 726f  red Gaussian pro
+00010a10: 6365 7373 206d 6f64 656c 7322 0a20 2020  cess models".   
+00010a20: 2022 2222 0a20 2020 2072 765f 6f70 203d   """.    rv_op =
+00010a30: 206b 726f 6e65 636b 6572 6e6f 726d 616c   kroneckernormal
+00010a40: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00010a50: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
+00010a60: 636c 732c 206d 752c 2063 6f76 733d 4e6f  cls, mu, covs=No
+00010a70: 6e65 2c20 6368 6f6c 733d 4e6f 6e65 2c20  ne, chols=None, 
+00010a80: 6576 6473 3d4e 6f6e 652c 2073 6967 6d61  evds=None, sigma
+00010a90: 3d4e 6f6e 652c 202a 6172 6773 2c20 2a2a  =None, *args, **
+00010aa0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00010ab0: 2069 6620 6c65 6e28 5b69 2066 6f72 2069   if len([i for i
+00010ac0: 2069 6e20 5b63 6f76 732c 2063 686f 6c73   in [covs, chols
+00010ad0: 2c20 6576 6473 5d20 6966 2069 2069 7320  , evds] if i is 
+00010ae0: 6e6f 7420 4e6f 6e65 5d29 2021 3d20 313a  not None]) != 1:
+00010af0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00010b00: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00010b20: 496e 636f 6d70 6174 6962 6c65 2070 6172  Incompatible par
+00010b30: 616d 6574 6572 697a 6174 696f 6e2e 2053  ameterization. S
+00010b40: 7065 6369 6679 2065 7861 6374 6c79 206f  pecify exactly o
+00010b50: 6e65 206f 6620 636f 7673 2c20 6368 6f6c  ne of covs, chol
+00010b60: 732c 206f 7220 6576 6473 2e22 0a20 2020  s, or evds.".   
+00010b70: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00010b80: 2020 2020 7369 676d 6120 3d20 7369 676d      sigma = sigm
+00010b90: 6120 6966 2073 6967 6d61 2065 6c73 6520  a if sigma else 
+00010ba0: 300a 0a20 2020 2020 2020 2069 6620 6368  0..        if ch
+00010bb0: 6f6c 7320 6973 206e 6f74 204e 6f6e 653a  ols is not None:
+00010bc0: 0a20 2020 2020 2020 2020 2020 2063 6f76  .            cov
+00010bd0: 7320 3d20 5b63 686f 6c2e 646f 7428 6368  s = [chol.dot(ch
+00010be0: 6f6c 2e54 2920 666f 7220 6368 6f6c 2069  ol.T) for chol i
+00010bf0: 6e20 6368 6f6c 735d 0a20 2020 2020 2020  n chols].       
+00010c00: 2065 6c69 6620 6576 6473 2069 7320 6e6f   elif evds is no
+00010c10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00010c20: 2020 2020 6569 6768 5f69 7465 7261 626c      eigh_iterabl
+00010c30: 6520 3d20 6576 6473 0a20 2020 2020 2020  e = evds.       
+00010c40: 2020 2020 2063 6f76 7320 3d20 5b5d 0a20       covs = []. 
+00010c50: 2020 2020 2020 2020 2020 2065 6967 735f             eigs_
+00010c60: 7365 702c 2051 7320 3d20 7a69 7028 2a65  sep, Qs = zip(*e
+00010c70: 6967 685f 6974 6572 6162 6c65 2920 2023  igh_iterable)  #
+00010c80: 2055 6e7a 6970 0a20 2020 2020 2020 2020   Unzip.         
+00010c90: 2020 2066 6f72 2065 6967 2c20 5120 696e     for eig, Q in
+00010ca0: 207a 6970 2865 6967 735f 7365 702c 2051   zip(eigs_sep, Q
+00010cb0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00010cc0: 2020 2020 636f 765f 6920 3d20 7074 2e64      cov_i = pt.d
+00010cd0: 6f74 2851 2c20 7074 2e64 6f74 2870 742e  ot(Q, pt.dot(pt.
+00010ce0: 6469 6167 2865 6967 292c 2051 2e54 2929  diag(eig), Q.T))
+00010cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d00: 2063 6f76 732e 6170 7065 6e64 2863 6f76   covs.append(cov
+00010d10: 5f69 290a 0a20 2020 2020 2020 206d 7520  _i)..        mu 
+00010d20: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00010d30: 6172 6961 626c 6528 6d75 290a 0a20 2020  ariable(mu)..   
+00010d40: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00010d50: 7228 292e 6469 7374 285b 6d75 2c20 7369  r().dist([mu, si
+00010d60: 676d 612c 202a 636f 7673 5d2c 202a 2a6b  gma, *covs], **k
+00010d70: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+00010d80: 6d6f 6d65 6e74 2872 762c 2073 697a 652c  moment(rv, size,
+00010d90: 206d 752c 2063 6f76 732c 2063 686f 6c73   mu, covs, chols
+00010da0: 2c20 6576 6473 293a 0a20 2020 2020 2020  , evds):.       
+00010db0: 206d 6561 6e20 3d20 6d75 0a20 2020 2020   mean = mu.     
+00010dc0: 2020 2069 6620 6e6f 7420 7276 5f73 697a     if not rv_siz
+00010dd0: 655f 6973 5f6e 6f6e 6528 7369 7a65 293a  e_is_none(size):
+00010de0: 0a20 2020 2020 2020 2020 2020 206d 6f6d  .            mom
+00010df0: 656e 745f 7369 7a65 203d 2070 742e 636f  ent_size = pt.co
+00010e00: 6e63 6174 656e 6174 6528 5b73 697a 652c  ncatenate([size,
+00010e10: 206d 752e 7368 6170 655d 290a 2020 2020   mu.shape]).    
+00010e20: 2020 2020 2020 2020 6d65 616e 203d 2070          mean = p
+00010e30: 742e 6675 6c6c 286d 6f6d 656e 745f 7369  t.full(moment_si
+00010e40: 7a65 2c20 6d75 290a 2020 2020 2020 2020  ze, mu).        
+00010e50: 7265 7475 726e 206d 6561 6e0a 0a20 2020  return mean..   
+00010e60: 2064 6566 206c 6f67 7028 7661 6c75 652c   def logp(value,
+00010e70: 206d 752c 2073 6967 6d61 2c20 2a63 6f76   mu, sigma, *cov
+00010e80: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
+00010e90: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+00010ea0: 6520 6c6f 672d 7072 6f62 6162 696c 6974  e log-probabilit
+00010eb0: 7920 6f66 204d 756c 7469 7661 7269 6174  y of Multivariat
+00010ec0: 6520 4e6f 726d 616c 2064 6973 7472 6962  e Normal distrib
+00010ed0: 7574 696f 6e0a 2020 2020 2020 2020 7769  ution.        wi
+00010ee0: 7468 204b 726f 6e65 636b 6572 2d73 7472  th Kronecker-str
+00010ef0: 7563 7475 7265 6420 636f 7661 7269 616e  uctured covarian
+00010f00: 6365 2061 7420 7370 6563 6966 6965 6420  ce at specified 
+00010f10: 7661 6c75 652e 0a0a 2020 2020 2020 2020  value...        
+00010f20: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00010f30: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00010f40: 2020 2020 2020 7661 6c75 653a 206e 756d        value: num
+00010f50: 6572 6963 0a20 2020 2020 2020 2020 2020  eric.           
+00010f60: 2056 616c 7565 2066 6f72 2077 6869 6368   Value for which
+00010f70: 206c 6f67 2d70 726f 6261 6269 6c69 7479   log-probability
+00010f80: 2069 7320 6361 6c63 756c 6174 6564 2e0a   is calculated..
+00010f90: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00010fa0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00010fb0: 0a20 2020 2020 2020 2054 656e 736f 7256  .        TensorV
+00010fc0: 6172 6961 626c 650a 2020 2020 2020 2020  ariable.        
+00010fd0: 2222 220a 2020 2020 2020 2020 2320 436f  """.        # Co
+00010fe0: 6d70 7574 6573 2074 6865 2071 7561 6472  mputes the quadr
+00010ff0: 6174 6963 2028 782d 6d75 295e 5420 4020  atic (x-mu)^T @ 
+00011000: 4b5e 2d31 2040 2028 782d 6d75 2920 616e  K^-1 @ (x-mu) an
+00011010: 6420 6c6f 6728 6465 7428 4b29 290a 2020  d log(det(K)).  
+00011020: 2020 2020 2020 6966 2076 616c 7565 2e6e        if value.n
+00011030: 6469 6d20 3e20 3220 6f72 2076 616c 7565  dim > 2 or value
+00011040: 2e6e 6469 6d20 3d3d 2030 3a0a 2020 2020  .ndim == 0:.    
+00011050: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00011060: 6c75 6545 7272 6f72 2866 2249 6e76 616c  lueError(f"Inval
+00011070: 6964 2064 696d 656e 7369 6f6e 2066 6f72  id dimension for
+00011080: 2076 616c 7565 3a20 7b76 616c 7565 2e6e   value: {value.n
+00011090: 6469 6d7d 2229 0a20 2020 2020 2020 2069  dim}").        i
+000110a0: 6620 7661 6c75 652e 6e64 696d 203d 3d20  f value.ndim == 
+000110b0: 313a 0a20 2020 2020 2020 2020 2020 206f  1:.            o
+000110c0: 6e65 6469 6d20 3d20 5472 7565 0a20 2020  nedim = True.   
+000110d0: 2020 2020 2020 2020 2076 616c 7565 203d           value =
+000110e0: 2076 616c 7565 5b4e 6f6e 652c 203a 5d0a   value[None, :].
+000110f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00011100: 2020 2020 2020 2020 2020 6f6e 6564 696d            onedim
+00011110: 203d 2046 616c 7365 0a0a 2020 2020 2020   = False..      
+00011120: 2020 6465 6c74 6120 3d20 7661 6c75 6520    delta = value 
+00011130: 2d20 6d75 0a0a 2020 2020 2020 2020 6569  - mu..        ei
+00011140: 6768 5f69 7465 7261 626c 6520 3d20 6d61  gh_iterable = ma
+00011150: 7028 6569 6768 2c20 636f 7673 290a 2020  p(eigh, covs).  
+00011160: 2020 2020 2020 6569 6773 5f73 6570 2c20        eigs_sep, 
+00011170: 5173 203d 207a 6970 282a 6569 6768 5f69  Qs = zip(*eigh_i
+00011180: 7465 7261 626c 6529 2020 2320 556e 7a69  terable)  # Unzi
+00011190: 700a 2020 2020 2020 2020 5173 203d 206c  p.        Qs = l
+000111a0: 6973 7428 6d61 7028 7074 2e61 735f 7465  ist(map(pt.as_te
+000111b0: 6e73 6f72 5f76 6172 6961 626c 652c 2051  nsor_variable, Q
+000111c0: 7329 290a 2020 2020 2020 2020 5154 7320  s)).        QTs 
+000111d0: 3d20 6c69 7374 286d 6170 2870 742e 7472  = list(map(pt.tr
+000111e0: 616e 7370 6f73 652c 2051 7329 290a 0a20  anspose, Qs)).. 
+000111f0: 2020 2020 2020 2065 6967 735f 7365 7020         eigs_sep 
+00011200: 3d20 6c69 7374 286d 6170 2870 742e 6173  = list(map(pt.as
+00011210: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00011220: 2c20 6569 6773 5f73 6570 2929 0a20 2020  , eigs_sep)).   
+00011230: 2020 2020 2065 6967 7320 3d20 6b72 6f6e       eigs = kron
+00011240: 5f64 6961 6728 2a65 6967 735f 7365 7029  _diag(*eigs_sep)
+00011250: 2020 2320 436f 6d62 696e 6520 7365 7061    # Combine sepa
+00011260: 7261 7465 2065 6967 730a 2020 2020 2020  rate eigs.      
+00011270: 2020 6569 6773 202b 3d20 7369 676d 612a    eigs += sigma*
+00011280: 2a32 0a20 2020 2020 2020 204e 203d 2065  *2.        N = e
+00011290: 6967 732e 7368 6170 655b 305d 0a0a 2020  igs.shape[0]..  
+000112a0: 2020 2020 2020 7371 7274 5f71 7561 6420        sqrt_quad 
+000112b0: 3d20 6b72 6f6e 5f64 6f74 2851 5473 2c20  = kron_dot(QTs, 
+000112c0: 6465 6c74 612e 5429 0a20 2020 2020 2020  delta.T).       
+000112d0: 2073 7172 745f 7175 6164 203d 2073 7172   sqrt_quad = sqr
+000112e0: 745f 7175 6164 202f 2070 742e 7371 7274  t_quad / pt.sqrt
+000112f0: 2865 6967 735b 3a2c 204e 6f6e 655d 290a  (eigs[:, None]).
+00011300: 2020 2020 2020 2020 6c6f 6764 6574 203d          logdet =
+00011310: 2070 742e 7375 6d28 7074 2e6c 6f67 2865   pt.sum(pt.log(e
+00011320: 6967 7329 290a 0a20 2020 2020 2020 2023  igs))..        #
+00011330: 2053 7175 6172 6520 6561 6368 2073 616d   Square each sam
+00011340: 706c 650a 2020 2020 2020 2020 7175 6164  ple.        quad
+00011350: 203d 2070 742e 6261 7463 6865 645f 646f   = pt.batched_do
+00011360: 7428 7371 7274 5f71 7561 642e 542c 2073  t(sqrt_quad.T, s
+00011370: 7172 745f 7175 6164 2e54 290a 2020 2020  qrt_quad.T).    
+00011380: 2020 2020 6966 206f 6e65 6469 6d3a 0a20      if onedim:. 
+00011390: 2020 2020 2020 2020 2020 2071 7561 6420             quad 
+000113a0: 3d20 7175 6164 5b30 5d0a 0a20 2020 2020  = quad[0]..     
+000113b0: 2020 2061 203d 202d 2871 7561 6420 2b20     a = -(quad + 
+000113c0: 6c6f 6764 6574 202b 204e 202a 2070 742e  logdet + N * pt.
+000113d0: 6c6f 6728 3220 2a20 6e70 2e70 6929 2920  log(2 * np.pi)) 
+000113e0: 2f20 322e 300a 2020 2020 2020 2020 7265  / 2.0.        re
+000113f0: 7475 726e 2061 0a0a 0a63 6c61 7373 2043  turn a...class C
+00011400: 4152 5256 2852 616e 646f 6d56 6172 6961  ARRV(RandomVaria
+00011410: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
+00011420: 2022 6361 7222 0a20 2020 206e 6469 6d5f   "car".    ndim_
+00011430: 7375 7070 203d 2031 0a20 2020 206e 6469  supp = 1.    ndi
+00011440: 6d73 5f70 6172 616d 7320 3d20 5b31 2c20  ms_params = [1, 
+00011450: 322c 2030 2c20 305d 0a20 2020 2064 7479  2, 0, 0].    dty
+00011460: 7065 203d 2022 666c 6f61 7458 220a 2020  pe = "floatX".  
+00011470: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
+00011480: 2822 4341 5222 2c20 225c 5c6f 7065 7261  ("CAR", "\\opera
+00011490: 746f 726e 616d 657b 4341 527d 2229 0a0a  torname{CAR}")..
+000114a0: 2020 2020 6465 6620 6d61 6b65 5f6e 6f64      def make_nod
+000114b0: 6528 7365 6c66 2c20 726e 672c 2073 697a  e(self, rng, siz
+000114c0: 652c 2064 7479 7065 2c20 6d75 2c20 572c  e, dtype, mu, W,
+000114d0: 2061 6c70 6861 2c20 7461 7529 3a0a 2020   alpha, tau):.  
+000114e0: 2020 2020 2020 6d75 203d 2070 742e 6173        mu = pt.as
+000114f0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00011500: 2866 6c6f 6174 5828 6d75 2929 0a0a 2020  (floatX(mu))..  
+00011510: 2020 2020 2020 5720 3d20 7079 7465 6e73        W = pytens
+00011520: 6f72 2e73 7061 7273 652e 6173 5f73 7061  or.sparse.as_spa
+00011530: 7273 655f 6f72 5f74 656e 736f 725f 7661  rse_or_tensor_va
+00011540: 7269 6162 6c65 2866 6c6f 6174 5828 5729  riable(floatX(W)
+00011550: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00011560: 2057 2e6e 6469 6d20 3d3d 2032 3a0a 2020   W.ndim == 2:.  
+00011570: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00011580: 5661 6c75 6545 7272 6f72 2822 5720 6d75  ValueError("W mu
+00011590: 7374 2062 6520 6120 6d61 7472 6978 2028  st be a matrix (
+000115a0: 6e64 696d 3d32 292e 2229 0a0a 2020 2020  ndim=2).")..    
+000115b0: 2020 2020 7370 6172 7365 203d 2069 7369      sparse = isi
+000115c0: 6e73 7461 6e63 6528 572c 2070 7974 656e  nstance(W, pyten
+000115d0: 736f 722e 7370 6172 7365 2e53 7061 7273  sor.sparse.Spars
+000115e0: 6556 6172 6961 626c 6529 0a20 2020 2020  eVariable).     
+000115f0: 2020 206d 7367 203d 2022 5720 6d75 7374     msg = "W must
+00011600: 2062 6520 6120 7379 6d6d 6574 7269 6320   be a symmetric 
+00011610: 6164 6a61 6365 6e63 7920 6d61 7472 6978  adjacency matrix
+00011620: 2e22 0a20 2020 2020 2020 2069 6620 7370  .".        if sp
+00011630: 6172 7365 3a0a 2020 2020 2020 2020 2020  arse:.          
+00011640: 2020 6162 735f 6469 6666 203d 2070 7974    abs_diff = pyt
+00011650: 656e 736f 722e 7370 6172 7365 2e62 6173  ensor.sparse.bas
+00011660: 6963 2e6d 756c 2870 7974 656e 736f 722e  ic.mul(pytensor.
+00011670: 7370 6172 7365 2e73 6967 6e28 5720 2d20  sparse.sign(W - 
+00011680: 572e 5429 2c20 5720 2d20 572e 5429 0a20  W.T), W - W.T). 
+00011690: 2020 2020 2020 2020 2020 2057 203d 2041             W = A
+000116a0: 7373 6572 7428 6d73 6729 2857 2c20 7074  ssert(msg)(W, pt
+000116b0: 2e69 7363 6c6f 7365 2870 7974 656e 736f  .isclose(pytenso
+000116c0: 722e 7370 6172 7365 2e73 705f 7375 6d28  r.sparse.sp_sum(
+000116d0: 6162 735f 6469 6666 292c 2030 2929 0a20  abs_diff), 0)). 
+000116e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000116f0: 2020 2020 2020 2020 2057 203d 2041 7373           W = Ass
+00011700: 6572 7428 6d73 6729 2857 2c20 7074 2e61  ert(msg)(W, pt.a
+00011710: 6c6c 636c 6f73 6528 572c 2057 2e54 2929  llclose(W, W.T))
+00011720: 0a0a 2020 2020 2020 2020 7461 7520 3d20  ..        tau = 
+00011730: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+00011740: 6961 626c 6528 666c 6f61 7458 2874 6175  iable(floatX(tau
+00011750: 2929 0a0a 2020 2020 2020 2020 616c 7068  ))..        alph
+00011760: 6120 3d20 7074 2e61 735f 7465 6e73 6f72  a = pt.as_tensor
+00011770: 5f76 6172 6961 626c 6528 666c 6f61 7458  _variable(floatX
+00011780: 2861 6c70 6861 2929 0a0a 2020 2020 2020  (alpha))..      
+00011790: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000117a0: 2e6d 616b 655f 6e6f 6465 2872 6e67 2c20  .make_node(rng, 
+000117b0: 7369 7a65 2c20 6474 7970 652c 206d 752c  size, dtype, mu,
+000117c0: 2057 2c20 616c 7068 612c 2074 6175 290a   W, alpha, tau).
+000117d0: 0a20 2020 2064 6566 205f 7375 7070 5f73  .    def _supp_s
+000117e0: 6861 7065 5f66 726f 6d5f 7061 7261 6d73  hape_from_params
+000117f0: 2873 656c 662c 2064 6973 745f 7061 7261  (self, dist_para
+00011800: 6d73 2c20 7061 7261 6d5f 7368 6170 6573  ms, param_shapes
+00011810: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00011820: 7265 7475 726e 2073 7570 705f 7368 6170  return supp_shap
+00011830: 655f 6672 6f6d 5f72 6566 5f70 6172 616d  e_from_ref_param
+00011840: 5f73 6861 7065 280a 2020 2020 2020 2020  _shape(.        
+00011850: 2020 2020 6e64 696d 5f73 7570 703d 7365      ndim_supp=se
+00011860: 6c66 2e6e 6469 6d5f 7375 7070 2c0a 2020  lf.ndim_supp,.  
+00011870: 2020 2020 2020 2020 2020 6469 7374 5f70            dist_p
+00011880: 6172 616d 733d 6469 7374 5f70 6172 616d  arams=dist_param
+00011890: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
+000118a0: 6172 616d 5f73 6861 7065 733d 7061 7261  aram_shapes=para
+000118b0: 6d5f 7368 6170 6573 2c0a 2020 2020 2020  m_shapes,.      
+000118c0: 2020 2020 2020 7265 665f 7061 7261 6d5f        ref_param_
+000118d0: 6964 783d 302c 0a20 2020 2020 2020 2029  idx=0,.        )
+000118e0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+000118f0: 6f64 0a20 2020 2064 6566 2072 6e67 5f66  od.    def rng_f
+00011900: 6e28 636c 732c 2072 6e67 3a20 6e70 2e72  n(cls, rng: np.r
+00011910: 616e 646f 6d2e 5261 6e64 6f6d 5374 6174  andom.RandomStat
+00011920: 652c 206d 752c 2057 2c20 616c 7068 612c  e, mu, W, alpha,
+00011930: 2074 6175 2c20 7369 7a65 293a 0a20 2020   tau, size):.   
+00011940: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011950: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
+00011960: 6f66 2061 6c67 6f72 6974 686d 2066 726f  of algorithm fro
+00011970: 6d20 7061 7065 720a 2020 2020 2020 2020  m paper.        
+00011980: 4861 7661 7264 2052 7565 2c20 3230 3031  Havard Rue, 2001
+00011990: 2e20 2246 6173 7420 7361 6d70 6c69 6e67  . "Fast sampling
+000119a0: 206f 6620 4761 7573 7369 616e 204d 6172   of Gaussian Mar
+000119b0: 6b6f 7620 7261 6e64 6f6d 2066 6965 6c64  kov random field
+000119c0: 732c 220a 2020 2020 2020 2020 4a6f 7572  s,".        Jour
+000119d0: 6e61 6c20 6f66 2074 6865 2052 6f79 616c  nal of the Royal
+000119e0: 2053 7461 7469 7374 6963 616c 2053 6f63   Statistical Soc
+000119f0: 6965 7479 2053 6572 6965 7320 422c 2052  iety Series B, R
+00011a00: 6f79 616c 2053 7461 7469 7374 6963 616c  oyal Statistical
+00011a10: 2053 6f63 6965 7479 2c0a 2020 2020 2020   Society,.      
+00011a20: 2020 766f 6c2e 2036 3328 3229 2c20 7061    vol. 63(2), pa
+00011a30: 6765 7320 3332 352d 3333 382e 2044 4f49  ges 325-338. DOI
+00011a40: 3a20 3130 2e31 3131 312f 3134 3637 2d39  : 10.1111/1467-9
+00011a50: 3836 382e 3030 3238 380a 2020 2020 2020  868.00288.      
+00011a60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00011a70: 206e 702e 616e 7928 616c 7068 6120 3e3d   np.any(alpha >=
+00011a80: 2031 2920 6f72 206e 702e 616e 7928 616c   1) or np.any(al
+00011a90: 7068 6120 3c3d 202d 3129 3a0a 2020 2020  pha <= -1):.    
+00011aa0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00011ab0: 6c75 6545 7272 6f72 2822 7468 6520 646f  lueError("the do
+00011ac0: 6d61 696e 206f 6620 616c 7068 6120 6973  main of alpha is
+00011ad0: 3a20 2d31 203c 2061 6c70 6861 203c 2031  : -1 < alpha < 1
+00011ae0: 2229 0a0a 2020 2020 2020 2020 6966 206e  ")..        if n
+00011af0: 6f74 2073 6369 7079 2e73 7061 7273 652e  ot scipy.sparse.
+00011b00: 6973 7370 6172 7365 2857 293a 0a20 2020  issparse(W):.   
+00011b10: 2020 2020 2020 2020 2057 203d 2073 6369           W = sci
+00011b20: 7079 2e73 7061 7273 652e 6373 725f 6d61  py.sparse.csr_ma
+00011b30: 7472 6978 2857 290a 2020 2020 2020 2020  trix(W).        
+00011b40: 7320 3d20 6e70 2e61 7361 7272 6179 2857  s = np.asarray(W
+00011b50: 2e73 756d 2861 7869 733d 3029 295b 305d  .sum(axis=0))[0]
+00011b60: 0a20 2020 2020 2020 2044 203d 2073 6369  .        D = sci
+00011b70: 7079 2e73 7061 7273 652e 6469 6167 7328  py.sparse.diags(
+00011b80: 7329 0a20 2020 2020 2020 2074 6175 203d  s).        tau =
+00011b90: 2073 6369 7079 2e73 7061 7273 652e 6373   scipy.sparse.cs
+00011ba0: 725f 6d61 7472 6978 2874 6175 290a 2020  r_matrix(tau).  
+00011bb0: 2020 2020 2020 616c 7068 6120 3d20 7363        alpha = sc
+00011bc0: 6970 792e 7370 6172 7365 2e63 7372 5f6d  ipy.sparse.csr_m
+00011bd0: 6174 7269 7828 616c 7068 6129 0a0a 2020  atrix(alpha)..  
+00011be0: 2020 2020 2020 5120 3d20 7461 752e 6d75        Q = tau.mu
+00011bf0: 6c74 6970 6c79 2844 202d 2061 6c70 6861  ltiply(D - alpha
+00011c00: 2e6d 756c 7469 706c 7928 5729 290a 0a20  .multiply(W)).. 
+00011c10: 2020 2020 2020 2070 6572 6d5f 6172 7261         perm_arra
+00011c20: 7920 3d20 7363 6970 792e 7370 6172 7365  y = scipy.sparse
+00011c30: 2e63 7367 7261 7068 2e72 6576 6572 7365  .csgraph.reverse
+00011c40: 5f63 7574 6869 6c6c 5f6d 636b 6565 2851  _cuthill_mckee(Q
+00011c50: 2c20 7379 6d6d 6574 7269 635f 6d6f 6465  , symmetric_mode
+00011c60: 3d54 7275 6529 0a20 2020 2020 2020 2069  =True).        i
+00011c70: 6e76 5f70 6572 6d20 3d20 6e70 2e61 7267  nv_perm = np.arg
+00011c80: 736f 7274 2870 6572 6d5f 6172 7261 7929  sort(perm_array)
+00011c90: 0a0a 2020 2020 2020 2020 5120 3d20 515b  ..        Q = Q[
+00011ca0: 7065 726d 5f61 7272 6179 2c20 3a5d 5b3a  perm_array, :][:
+00011cb0: 2c20 7065 726d 5f61 7272 6179 5d0a 0a20  , perm_array].. 
+00011cc0: 2020 2020 2020 2051 6220 3d20 512e 6469         Qb = Q.di
+00011cd0: 6167 6f6e 616c 2829 0a20 2020 2020 2020  agonal().       
+00011ce0: 2075 203d 2031 0a20 2020 2020 2020 2077   u = 1.        w
+00011cf0: 6869 6c65 206e 702e 636f 756e 745f 6e6f  hile np.count_no
+00011d00: 6e7a 6572 6f28 512e 6469 6167 6f6e 616c  nzero(Q.diagonal
+00011d10: 2875 2929 203e 2030 3a0a 2020 2020 2020  (u)) > 0:.      
+00011d20: 2020 2020 2020 5162 203d 206e 702e 7673        Qb = np.vs
+00011d30: 7461 636b 2828 6e70 2e70 6164 2851 2e64  tack((np.pad(Q.d
+00011d40: 6961 676f 6e61 6c28 7529 2c20 2875 2c20  iagonal(u), (u, 
+00011d50: 3029 2c20 636f 6e73 7461 6e74 5f76 616c  0), constant_val
+00011d60: 7565 733d 2830 2c20 3029 292c 2051 6229  ues=(0, 0)), Qb)
+00011d70: 290a 2020 2020 2020 2020 2020 2020 7520  ).            u 
+00011d80: 2b3d 2031 0a0a 2020 2020 2020 2020 4c20  += 1..        L 
+00011d90: 3d20 7363 6970 792e 6c69 6e61 6c67 2e63  = scipy.linalg.c
+00011da0: 686f 6c65 736b 795f 6261 6e64 6564 2851  holesky_banded(Q
+00011db0: 622c 206c 6f77 6572 3d46 616c 7365 290a  b, lower=False).
+00011dc0: 0a20 2020 2020 2020 2073 697a 6520 3d20  .        size = 
+00011dd0: 7475 706c 6528 7369 7a65 206f 7220 2829  tuple(size or ()
+00011de0: 290a 2020 2020 2020 2020 6966 2073 697a  ).        if siz
+00011df0: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+00011e00: 7520 3d20 6e70 2e62 726f 6164 6361 7374  u = np.broadcast
+00011e10: 5f74 6f28 6d75 2c20 7369 7a65 202b 2028  _to(mu, size + (
+00011e20: 6d75 2e73 6861 7065 5b2d 315d 2c29 290a  mu.shape[-1],)).
+00011e30: 2020 2020 2020 2020 7a20 3d20 726e 672e          z = rng.
+00011e40: 6e6f 726d 616c 2873 697a 653d 6d75 2e73  normal(size=mu.s
+00011e50: 6861 7065 290a 2020 2020 2020 2020 7361  hape).        sa
+00011e60: 6d70 6c65 7320 3d20 6e70 2e65 6d70 7479  mples = np.empty
+00011e70: 287a 2e73 6861 7065 290a 2020 2020 2020  (z.shape).      
+00011e80: 2020 666f 7220 6964 7820 696e 206e 702e    for idx in np.
+00011e90: 6e64 696e 6465 7828 6d75 2e73 6861 7065  ndindex(mu.shape
+00011ea0: 5b3a 2d31 5d29 3a0a 2020 2020 2020 2020  [:-1]):.        
+00011eb0: 2020 2020 7361 6d70 6c65 735b 6964 785d      samples[idx]
+00011ec0: 203d 2073 6369 7079 2e6c 696e 616c 672e   = scipy.linalg.
+00011ed0: 6368 6f5f 736f 6c76 655f 6261 6e64 6564  cho_solve_banded
+00011ee0: 2828 4c2c 2046 616c 7365 292c 207a 5b69  ((L, False), z[i
+00011ef0: 6478 5d29 202b 206d 755b 6964 785d 5b70  dx]) + mu[idx][p
+00011f00: 6572 6d5f 6172 7261 795d 0a20 2020 2020  erm_array].     
+00011f10: 2020 2073 616d 706c 6573 203d 2073 616d     samples = sam
+00011f20: 706c 6573 5b2e 2e2e 2c20 696e 765f 7065  ples[..., inv_pe
+00011f30: 726d 5d0a 2020 2020 2020 2020 7265 7475  rm].        retu
+00011f40: 726e 2073 616d 706c 6573 0a0a 0a63 6172  rn samples...car
+00011f50: 203d 2043 4152 5256 2829 0a0a 0a63 6c61   = CARRV()...cla
+00011f60: 7373 2043 4152 2843 6f6e 7469 6e75 6f75  ss CAR(Continuou
+00011f70: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
+00011f80: 204c 696b 656c 6968 6f6f 6420 666f 7220   Likelihood for 
+00011f90: 6120 636f 6e64 6974 696f 6e61 6c20 6175  a conditional au
+00011fa0: 746f 7265 6772 6573 7369 6f6e 2e20 5468  toregression. Th
+00011fb0: 6973 2069 7320 6120 7370 6563 6961 6c20  is is a special 
+00011fc0: 6361 7365 206f 6620 7468 650a 2020 2020  case of the.    
+00011fd0: 6d75 6c74 6976 6172 6961 7465 206e 6f72  multivariate nor
+00011fe0: 6d61 6c20 7769 7468 2061 6e20 6164 6a61  mal with an adja
+00011ff0: 6365 6e63 792d 7374 7275 6374 7572 6564  cency-structured
+00012000: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
+00012010: 6978 2e0a 0a20 2020 202e 2e20 6d61 7468  ix...    .. math
+00012020: 3a3a 0a0a 2020 2020 2020 2066 2878 205c  ::..       f(x \
+00012030: 6d69 6420 572c 205c 616c 7068 612c 205c  mid W, \alpha, \
+00012040: 7461 7529 203d 0a20 2020 2020 2020 2020  tau) =.         
+00012050: 2020 5c66 7261 637b 7c54 7c5e 7b31 2f32    \frac{|T|^{1/2
+00012060: 7d7d 7b28 325c 7069 295e 7b6b 2f32 7d7d  }}{(2\pi)^{k/2}}
+00012070: 0a20 2020 2020 2020 2020 2020 5c65 7870  .           \exp
+00012080: 5c6c 6566 745c 7b20 2d5c 6672 6163 7b31  \left\{ -\frac{1
+00012090: 7d7b 327d 2028 782d 5c6d 7529 5e7b 5c70  }{2} (x-\mu)^{\p
+000120a0: 7269 6d65 7d20 545e 7b2d 317d 2028 782d  rime} T^{-1} (x-
+000120b0: 5c6d 7529 205c 7269 6768 745c 7d0a 0a20  \mu) \right\}.. 
+000120c0: 2020 2077 6865 7265 203a 6d61 7468 3a60     where :math:`
+000120d0: 5420 3d20 285c 7461 7520 4428 492d 5c61  T = (\tau D(I-\a
+000120e0: 6c70 6861 2057 2929 5e7b 2d31 7d60 2061  lpha W))^{-1}` a
+000120f0: 6e64 203a 6d61 7468 3a60 4420 3d20 6469  nd :math:`D = di
+00012100: 6167 285c 7375 6d5f 6920 575f 7b69 6a7d  ag(\sum_i W_{ij}
+00012110: 2960 2e0a 0a20 2020 203d 3d3d 3d3d 3d3d  )`...    =======
+00012120: 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =  =============
+00012130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00012140: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
+00012150: 683a 6078 205c 696e 205c 6d61 7468 6262  h:`x \in \mathbb
+00012160: 7b52 7d5e 6b60 0a20 2020 204d 6561 6e20  {R}^k`.    Mean 
+00012170: 2020 2020 203a 6d61 7468 3a60 5c6d 7520       :math:`\mu 
+00012180: 5c69 6e20 5c6d 6174 6862 627b 527d 5e6b  \in \mathbb{R}^k
+00012190: 600a 2020 2020 5661 7269 616e 6365 2020  `.    Variance  
+000121a0: 3a6d 6174 683a 6028 5c74 6175 2044 2849  :math:`(\tau D(I
+000121b0: 2d5c 616c 7068 6120 5729 295e 7b2d 317d  -\alpha W))^{-1}
+000121c0: 600a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  `.    ========  
+000121d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000121e0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
+000121f0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00012200: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6d75  ---------.    mu
+00012210: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+00012220: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+00012230: 5265 616c 2d76 616c 7565 6420 6d65 616e  Real-valued mean
+00012240: 2076 6563 746f 720a 2020 2020 5720 3a20   vector.    W : 
+00012250: 284d 2c20 4d29 2074 656e 736f 725f 6c69  (M, M) tensor_li
+00012260: 6b65 206f 6620 696e 740a 2020 2020 2020  ke of int.      
+00012270: 2020 5379 6d6d 6574 7269 6320 6164 6a61    Symmetric adja
+00012280: 6365 6e63 7920 6d61 7472 6978 206f 6620  cency matrix of 
+00012290: 3173 2061 6e64 2030 7320 696e 6469 6361  1s and 0s indica
+000122a0: 7469 6e67 0a20 2020 2020 2020 2061 646a  ting.        adj
+000122b0: 6163 656e 6379 2062 6574 7765 656e 2065  acency between e
+000122c0: 6c65 6d65 6e74 732e 2049 6620 706f 7373  lements. If poss
+000122d0: 6962 6c65 2c20 2a57 2a20 6973 2063 6f6e  ible, *W* is con
+000122e0: 7665 7274 6564 0a20 2020 2020 2020 2074  verted.        t
+000122f0: 6f20 6120 7370 6172 7365 206d 6174 7269  o a sparse matri
+00012300: 782c 2066 616c 6c69 6e67 2062 6163 6b20  x, falling back 
+00012310: 746f 2061 2064 656e 7365 2076 6172 6961  to a dense varia
+00012320: 626c 652e 0a20 2020 2020 2020 203a 6675  ble..        :fu
+00012330: 6e63 3a60 7e70 7974 656e 736f 722e 7370  nc:`~pytensor.sp
+00012340: 6172 7365 2e62 6173 6963 2e61 735f 7370  arse.basic.as_sp
+00012350: 6172 7365 5f6f 725f 7465 6e73 6f72 5f76  arse_or_tensor_v
+00012360: 6172 6961 626c 6560 2069 730a 2020 2020  ariable` is.    
+00012370: 2020 2020 7573 6564 2066 6f72 2074 6869      used for thi
+00012380: 7320 7370 6172 7365 206f 7220 7465 6e73  s sparse or tens
+00012390: 6f72 7661 7269 6162 6c65 2063 6f6e 7665  orvariable conve
+000123a0: 7273 696f 6e2e 0a20 2020 2061 6c70 6861  rsion..    alpha
+000123b0: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+000123c0: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+000123d0: 4175 746f 7265 6772 6573 7369 6f6e 2070  Autoregression p
+000123e0: 6172 616d 6574 6572 2074 616b 696e 6720  arameter taking 
+000123f0: 7661 6c75 6573 2067 7265 6174 6572 2074  values greater t
+00012400: 6861 6e20 2d31 2061 6e64 206c 6573 7320  han -1 and less 
+00012410: 7468 616e 2031 2e0a 2020 2020 2020 2020  than 1..        
+00012420: 5661 6c75 6573 2063 6c6f 7365 7220 746f  Values closer to
+00012430: 2030 2069 6e64 6963 6174 6520 7765 616b   0 indicate weak
+00012440: 6572 2063 6f72 7265 6c61 7469 6f6e 2061  er correlation a
+00012450: 6e64 2076 616c 7565 7320 636c 6f73 6572  nd values closer
+00012460: 2074 6f0a 2020 2020 2020 2020 3120 696e   to.        1 in
+00012470: 6469 6361 7465 2068 6967 6865 7220 6175  dicate higher au
+00012480: 746f 636f 7272 656c 6174 696f 6e2e 2046  tocorrelation. F
+00012490: 6f72 206d 6f73 7420 7573 6520 6361 7365  or most use case
+000124a0: 732c 2074 6865 0a20 2020 2020 2020 2073  s, the.        s
+000124b0: 7570 706f 7274 206f 6620 616c 7068 6120  upport of alpha 
+000124c0: 7368 6f75 6c64 2062 6520 7265 7374 7269  should be restri
+000124d0: 6374 6564 2074 6f20 2830 2c20 3129 2e0a  cted to (0, 1)..
+000124e0: 2020 2020 7461 7520 3a20 7465 6e73 6f72      tau : tensor
+000124f0: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
+00012500: 2020 2020 2020 2050 6f73 6974 6976 6520         Positive 
+00012510: 7072 6563 6973 696f 6e20 7661 7269 6162  precision variab
+00012520: 6c65 2063 6f6e 7472 6f6c 6c69 6e67 2074  le controlling t
+00012530: 6865 2073 6361 6c65 206f 6620 7468 6520  he scale of the 
+00012540: 756e 6465 726c 7969 6e67 206e 6f72 6d61  underlying norma
+00012550: 6c20 7661 7269 6174 6573 2e0a 0a20 2020  l variates...   
+00012560: 2052 6566 6572 656e 6365 730a 2020 2020   References.    
+00012570: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e  ----------.    .
+00012580: 2e20 204a 696e 2c20 582e 2c20 4361 726c  .  Jin, X., Carl
+00012590: 696e 2c20 422e 2c20 4261 6e65 726a 6565  in, B., Banerjee
+000125a0: 2c20 532e 0a20 2020 2020 2020 2022 4765  , S..        "Ge
+000125b0: 6e65 7261 6c69 7a65 6420 4869 6572 6172  neralized Hierar
+000125c0: 6368 6963 616c 204d 756c 7469 7661 7269  chical Multivari
+000125d0: 6174 6520 4341 5220 4d6f 6465 6c73 2066  ate CAR Models f
+000125e0: 6f72 2041 7265 616c 2044 6174 6122 0a20  or Areal Data". 
+000125f0: 2020 2020 2020 2042 696f 6d65 7472 6963         Biometric
+00012600: 732c 2056 6f6c 2e20 3631 2c20 4e6f 2e20  s, Vol. 61, No. 
+00012610: 3420 2844 6563 2e2c 2032 3030 3529 2c20  4 (Dec., 2005), 
+00012620: 7070 2e20 3935 302d 3936 310a 2020 2020  pp. 950-961.    
+00012630: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
+00012640: 6361 720a 0a20 2020 2040 636c 6173 736d  car..    @classm
+00012650: 6574 686f 640a 2020 2020 6465 6620 6469  ethod.    def di
+00012660: 7374 2863 6c73 2c20 6d75 2c20 572c 2061  st(cls, mu, W, a
+00012670: 6c70 6861 2c20 7461 752c 202a 6172 6773  lpha, tau, *args
+00012680: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00012690: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+000126a0: 7228 292e 6469 7374 285b 6d75 2c20 572c  r().dist([mu, W,
+000126b0: 2061 6c70 6861 2c20 7461 755d 2c20 2a2a   alpha, tau], **
+000126c0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+000126d0: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
+000126e0: 2c20 6d75 2c20 572c 2061 6c70 6861 2c20  , mu, W, alpha, 
+000126f0: 7461 7529 3a0a 2020 2020 2020 2020 7265  tau):.        re
+00012700: 7475 726e 2070 742e 6675 6c6c 5f6c 696b  turn pt.full_lik
+00012710: 6528 7276 2c20 6d75 290a 0a20 2020 2064  e(rv, mu)..    d
+00012720: 6566 206c 6f67 7028 7661 6c75 652c 206d  ef logp(value, m
+00012730: 752c 2057 2c20 616c 7068 612c 2074 6175  u, W, alpha, tau
+00012740: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012750: 2020 2020 2020 2043 616c 6375 6c61 7465         Calculate
+00012760: 206c 6f67 2d70 726f 6261 6269 6c69 7479   log-probability
+00012770: 206f 6620 6120 4341 522d 6469 7374 7269   of a CAR-distri
+00012780: 6275 7465 6420 7665 6374 6f72 0a20 2020  buted vector.   
+00012790: 2020 2020 2061 7420 7370 6563 6966 6965       at specifie
+000127a0: 6420 7661 6c75 652e 2054 6869 7320 6c6f  d value. This lo
+000127b0: 6720 7072 6f62 6162 696c 6974 7920 6675  g probability fu
+000127c0: 6e63 7469 6f6e 2064 6966 6665 7273 2066  nction differs f
+000127d0: 726f 6d0a 2020 2020 2020 2020 7468 6520  rom.        the 
+000127e0: 7472 7565 2043 4152 206c 6f67 2064 656e  true CAR log den
+000127f0: 7369 7479 2028 414b 4120 6120 6d75 6c74  sity (AKA a mult
+00012800: 6976 6172 6961 7465 206e 6f72 6d61 6c20  ivariate normal 
+00012810: 7769 7468 2043 4152 2d73 7472 7563 7475  with CAR-structu
+00012820: 7265 640a 2020 2020 2020 2020 636f 7661  red.        cova
+00012830: 7269 616e 6365 206d 6174 7269 7829 2062  riance matrix) b
+00012840: 7920 616e 2061 6464 6974 6976 6520 636f  y an additive co
+00012850: 6e73 7461 6e74 2e0a 0a20 2020 2020 2020  nstant...       
+00012860: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00012870: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00012880: 2020 2020 2020 2076 616c 7565 3a20 6172         value: ar
+00012890: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+000128a0: 5661 6c75 6520 666f 7220 7768 6963 6820  Value for which 
+000128b0: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
+000128c0: 6973 2063 616c 6375 6c61 7465 642e 0a0a  is calculated...
+000128d0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000128e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000128f0: 2020 2020 2020 2020 5465 6e73 6f72 5661          TensorVa
+00012900: 7269 6162 6c65 0a20 2020 2020 2020 2022  riable.        "
+00012910: 2222 0a0a 2020 2020 2020 2020 7370 6172  ""..        spar
+00012920: 7365 203d 2069 7369 6e73 7461 6e63 6528  se = isinstance(
+00012930: 572c 2028 7079 7465 6e73 6f72 2e73 7061  W, (pytensor.spa
+00012940: 7273 652e 5370 6172 7365 436f 6e73 7461  rse.SparseConsta
+00012950: 6e74 2c20 7079 7465 6e73 6f72 2e73 7061  nt, pytensor.spa
+00012960: 7273 652e 5370 6172 7365 5661 7269 6162  rse.SparseVariab
+00012970: 6c65 2929 0a0a 2020 2020 2020 2020 6966  le))..        if
+00012980: 2073 7061 7273 653a 0a20 2020 2020 2020   sparse:.       
+00012990: 2020 2020 2044 203d 2073 705f 7375 6d28       D = sp_sum(
+000129a0: 572c 2061 7869 733d 3029 0a20 2020 2020  W, axis=0).     
+000129b0: 2020 2020 2020 2044 696e 765f 7371 7274         Dinv_sqrt
+000129c0: 203d 2070 742e 6469 6167 2831 202f 2070   = pt.diag(1 / p
+000129d0: 742e 7371 7274 2844 2929 0a20 2020 2020  t.sqrt(D)).     
+000129e0: 2020 2020 2020 2044 5744 203d 2070 742e         DWD = pt.
+000129f0: 646f 7428 7079 7465 6e73 6f72 2e73 7061  dot(pytensor.spa
+00012a00: 7273 652e 646f 7428 4469 6e76 5f73 7172  rse.dot(Dinv_sqr
+00012a10: 742c 2057 292c 2044 696e 765f 7371 7274  t, W), Dinv_sqrt
+00012a20: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00012a30: 2020 2020 2020 2020 2020 2020 4420 3d20              D = 
+00012a40: 572e 7375 6d28 6178 6973 3d30 290a 2020  W.sum(axis=0).  
+00012a50: 2020 2020 2020 2020 2020 4469 6e76 5f73            Dinv_s
+00012a60: 7172 7420 3d20 7074 2e64 6961 6728 3120  qrt = pt.diag(1 
+00012a70: 2f20 7074 2e73 7172 7428 4429 290a 2020  / pt.sqrt(D)).  
+00012a80: 2020 2020 2020 2020 2020 4457 4420 3d20            DWD = 
+00012a90: 7074 2e64 6f74 2870 742e 646f 7428 4469  pt.dot(pt.dot(Di
+00012aa0: 6e76 5f73 7172 742c 2057 292c 2044 696e  nv_sqrt, W), Din
+00012ab0: 765f 7371 7274 290a 2020 2020 2020 2020  v_sqrt).        
+00012ac0: 6c61 6d20 3d20 7074 2e73 6c69 6e61 6c67  lam = pt.slinalg
+00012ad0: 2e65 6967 7661 6c73 6828 4457 442c 2070  .eigvalsh(DWD, p
+00012ae0: 742e 6579 6528 4457 442e 7368 6170 655b  t.eye(DWD.shape[
+00012af0: 305d 2929 0a0a 2020 2020 2020 2020 642c  0]))..        d,
+00012b00: 205f 203d 2057 2e73 6861 7065 0a0a 2020   _ = W.shape..  
+00012b10: 2020 2020 2020 6966 2076 616c 7565 2e6e        if value.n
+00012b20: 6469 6d20 3d3d 2031 3a0a 2020 2020 2020  dim == 1:.      
+00012b30: 2020 2020 2020 7661 6c75 6520 3d20 7661        value = va
+00012b40: 6c75 655b 4e6f 6e65 2c20 3a5d 0a0a 2020  lue[None, :]..  
+00012b50: 2020 2020 2020 6c6f 6774 6175 203d 2064        logtau = d
+00012b60: 202a 2070 742e 6c6f 6728 7461 7529 2e73   * pt.log(tau).s
+00012b70: 756d 2829 0a20 2020 2020 2020 206c 6f67  um().        log
+00012b80: 6465 7420 3d20 7074 2e6c 6f67 2831 202d  det = pt.log(1 -
+00012b90: 2061 6c70 6861 2e54 202a 206c 616d 5b3a   alpha.T * lam[:
+00012ba0: 2c20 4e6f 6e65 5d29 2e73 756d 2829 0a20  , None]).sum(). 
+00012bb0: 2020 2020 2020 2064 656c 7461 203d 2076         delta = v
+00012bc0: 616c 7565 202d 206d 750a 0a20 2020 2020  alue - mu..     
+00012bd0: 2020 2069 6620 7370 6172 7365 3a0a 2020     if sparse:.  
+00012be0: 2020 2020 2020 2020 2020 5764 656c 7461            Wdelta
+00012bf0: 203d 2070 7974 656e 736f 722e 7370 6172   = pytensor.spar
+00012c00: 7365 2e64 6f74 2864 656c 7461 2c20 5729  se.dot(delta, W)
+00012c10: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00012c20: 2020 2020 2020 2020 2020 2057 6465 6c74             Wdelt
+00012c30: 6120 3d20 7074 2e64 6f74 2864 656c 7461  a = pt.dot(delta
+00012c40: 2c20 5729 0a0a 2020 2020 2020 2020 7461  , W)..        ta
+00012c50: 755f 646f 745f 6465 6c74 6120 3d20 445b  u_dot_delta = D[
+00012c60: 4e6f 6e65 2c20 3a5d 202a 2064 656c 7461  None, :] * delta
+00012c70: 202d 2061 6c70 6861 202a 2057 6465 6c74   - alpha * Wdelt
+00012c80: 610a 2020 2020 2020 2020 6c6f 6771 7561  a.        logqua
+00012c90: 6420 3d20 2874 6175 202a 2064 656c 7461  d = (tau * delta
+00012ca0: 202a 2074 6175 5f64 6f74 5f64 656c 7461   * tau_dot_delta
+00012cb0: 292e 7375 6d28 6178 6973 3d2d 3129 0a20  ).sum(axis=-1). 
+00012cc0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+00012cd0: 6563 6b5f 7061 7261 6d65 7465 7273 280a  eck_parameters(.
+00012ce0: 2020 2020 2020 2020 2020 2020 302e 3520              0.5 
+00012cf0: 2a20 286c 6f67 7461 7520 2b20 6c6f 6764  * (logtau + logd
+00012d00: 6574 202d 206c 6f67 7175 6164 292c 0a20  et - logquad),. 
+00012d10: 2020 2020 2020 2020 2020 202d 3120 3c20             -1 < 
+00012d20: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
+00012d30: 2020 2061 6c70 6861 203c 2031 2c0a 2020     alpha < 1,.  
+00012d40: 2020 2020 2020 2020 2020 7461 7520 3e20            tau > 
+00012d50: 302c 0a20 2020 2020 2020 2020 2020 206d  0,.            m
+00012d60: 7367 3d22 2d31 203c 2061 6c70 6861 203c  sg="-1 < alpha <
+00012d70: 2031 2c20 7461 7520 3e20 3022 2c0a 2020   1, tau > 0",.  
+00012d80: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+00012d90: 5374 6963 6b42 7265 616b 696e 6757 6569  StickBreakingWei
+00012da0: 6768 7473 5256 2852 616e 646f 6d56 6172  ghtsRV(RandomVar
+00012db0: 6961 626c 6529 3a0a 2020 2020 6e61 6d65  iable):.    name
+00012dc0: 203d 2022 7374 6963 6b5f 6272 6561 6b69   = "stick_breaki
+00012dd0: 6e67 5f77 6569 6768 7473 220a 2020 2020  ng_weights".    
+00012de0: 6e64 696d 5f73 7570 7020 3d20 310a 2020  ndim_supp = 1.  
+00012df0: 2020 6e64 696d 735f 7061 7261 6d73 203d    ndims_params =
+00012e00: 205b 302c 2030 5d0a 2020 2020 6474 7970   [0, 0].    dtyp
+00012e10: 6520 3d20 2266 6c6f 6174 5822 0a20 2020  e = "floatX".   
+00012e20: 205f 7072 696e 745f 6e61 6d65 203d 2028   _print_name = (
+00012e30: 2253 7469 636b 4272 6561 6b69 6e67 5765  "StickBreakingWe
+00012e40: 6967 6874 7322 2c20 225c 5c6f 7065 7261  ights", "\\opera
+00012e50: 746f 726e 616d 657b 5374 6963 6b42 7265  torname{StickBre
+00012e60: 616b 696e 6757 6569 6768 7473 7d22 290a  akingWeights}").
+00012e70: 0a20 2020 2064 6566 206d 616b 655f 6e6f  .    def make_no
+00012e80: 6465 2873 656c 662c 2072 6e67 2c20 7369  de(self, rng, si
+00012e90: 7a65 2c20 6474 7970 652c 2061 6c70 6861  ze, dtype, alpha
+00012ea0: 2c20 4b29 3a0a 2020 2020 2020 2020 616c  , K):.        al
+00012eb0: 7068 6120 3d20 7074 2e61 735f 7465 6e73  pha = pt.as_tens
+00012ec0: 6f72 5f76 6172 6961 626c 6528 616c 7068  or_variable(alph
+00012ed0: 6129 0a20 2020 2020 2020 204b 203d 2070  a).        K = p
+00012ee0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00012ef0: 6162 6c65 2869 6e74 5828 4b29 290a 0a20  able(intX(K)).. 
+00012f00: 2020 2020 2020 2069 6620 4b2e 6e64 696d         if K.ndim
+00012f10: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00012f20: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00012f30: 6f72 2822 4b20 6d75 7374 2062 6520 6120  or("K must be a 
+00012f40: 7363 616c 6172 2e22 290a 0a20 2020 2020  scalar.")..     
+00012f50: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00012f60: 292e 6d61 6b65 5f6e 6f64 6528 726e 672c  ).make_node(rng,
+00012f70: 2073 697a 652c 2064 7479 7065 2c20 616c   size, dtype, al
+00012f80: 7068 612c 204b 290a 0a20 2020 2064 6566  pha, K)..    def
+00012f90: 205f 7375 7070 5f73 6861 7065 5f66 726f   _supp_shape_fro
+00012fa0: 6d5f 7061 7261 6d73 2873 656c 662c 2064  m_params(self, d
+00012fb0: 6973 745f 7061 7261 6d73 2c20 7061 7261  ist_params, para
+00012fc0: 6d5f 7368 6170 6573 293a 0a20 2020 2020  m_shapes):.     
+00012fd0: 2020 204b 203d 2064 6973 745f 7061 7261     K = dist_para
+00012fe0: 6d73 5b31 5d0a 2020 2020 2020 2020 7265  ms[1].        re
+00012ff0: 7475 726e 2028 4b20 2b20 312c 290a 0a20  turn (K + 1,).. 
+00013000: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00013010: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
+00013020: 6c73 2c20 726e 672c 2061 6c70 6861 2c20  ls, rng, alpha, 
+00013030: 4b2c 2073 697a 6529 3a0a 2020 2020 2020  K, size):.      
+00013040: 2020 6966 204b 203c 2030 3a0a 2020 2020    if K < 0:.    
+00013050: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00013060: 6c75 6545 7272 6f72 2822 4b20 6e65 6564  lueError("K need
+00013070: 7320 746f 2062 6520 706f 7369 7469 7665  s to be positive
+00013080: 2e22 290a 0a20 2020 2020 2020 2073 697a  .")..        siz
+00013090: 6520 3d20 746f 5f74 7570 6c65 2873 697a  e = to_tuple(siz
+000130a0: 6529 2069 6620 7369 7a65 2069 7320 6e6f  e) if size is no
+000130b0: 7420 4e6f 6e65 2065 6c73 6520 616c 7068  t None else alph
+000130c0: 612e 7368 6170 650a 2020 2020 2020 2020  a.shape.        
+000130d0: 7369 7a65 203d 2073 697a 6520 2b20 284b  size = size + (K
+000130e0: 2c29 0a20 2020 2020 2020 2061 6c70 6861  ,).        alpha
+000130f0: 203d 2061 6c70 6861 5b2e 2e2e 2c20 6e70   = alpha[..., np
+00013100: 2e6e 6577 6178 6973 5d0a 0a20 2020 2020  .newaxis]..     
+00013110: 2020 2062 6574 6173 203d 2072 6e67 2e62     betas = rng.b
+00013120: 6574 6128 312c 2061 6c70 6861 2c20 7369  eta(1, alpha, si
+00013130: 7a65 3d73 697a 6529 0a0a 2020 2020 2020  ze=size)..      
+00013140: 2020 7374 6963 6b73 203d 206e 702e 636f    sticks = np.co
+00013150: 6e63 6174 656e 6174 6528 0a20 2020 2020  ncatenate(.     
+00013160: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+00013170: 2020 2020 2020 2020 206e 702e 6f6e 6573           np.ones
+00013180: 2873 6861 7065 3d28 7369 7a65 5b3a 2d31  (shape=(size[:-1
+00013190: 5d20 2b20 2831 2c29 2929 2c0a 2020 2020  ] + (1,))),.    
+000131a0: 2020 2020 2020 2020 2020 2020 6e70 2e63              np.c
+000131b0: 756d 7072 6f64 2831 202d 2062 6574 6173  umprod(1 - betas
+000131c0: 5b2e 2e2e 2c20 3a2d 315d 2c20 6178 6973  [..., :-1], axis
+000131d0: 3d2d 3129 2c0a 2020 2020 2020 2020 2020  =-1),.          
+000131e0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+000131f0: 2061 7869 733d 2d31 2c0a 2020 2020 2020   axis=-1,.      
+00013200: 2020 290a 0a20 2020 2020 2020 2077 6569    )..        wei
+00013210: 6768 7473 203d 2073 7469 636b 7320 2a20  ghts = sticks * 
+00013220: 6265 7461 730a 2020 2020 2020 2020 7765  betas.        we
+00013230: 6967 6874 7320 3d20 6e70 2e63 6f6e 6361  ights = np.conca
+00013240: 7465 6e61 7465 280a 2020 2020 2020 2020  tenate(.        
+00013250: 2020 2020 2877 6569 6768 7473 2c20 3120      (weights, 1 
+00013260: 2d20 7765 6967 6874 732e 7375 6d28 6178  - weights.sum(ax
+00013270: 6973 3d2d 3129 5b2e 2e2e 2c20 6e70 2e6e  is=-1)[..., np.n
+00013280: 6577 6178 6973 5d29 2c0a 2020 2020 2020  ewaxis]),.      
+00013290: 2020 2020 2020 6178 6973 3d2d 312c 0a20        axis=-1,. 
+000132a0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000132b0: 2020 7265 7475 726e 2077 6569 6768 7473    return weights
+000132c0: 0a0a 0a73 7469 636b 6272 6561 6b69 6e67  ...stickbreaking
+000132d0: 7765 6967 6874 7320 3d20 5374 6963 6b42  weights = StickB
+000132e0: 7265 616b 696e 6757 6569 6768 7473 5256  reakingWeightsRV
+000132f0: 2829 0a0a 0a63 6c61 7373 2053 7469 636b  ()...class Stick
+00013300: 4272 6561 6b69 6e67 5765 6967 6874 7328  BreakingWeights(
+00013310: 5369 6d70 6c65 7843 6f6e 7469 6e75 6f75  SimplexContinuou
+00013320: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
+00013330: 204c 696b 656c 6968 6f6f 6420 6f66 2074   Likelihood of t
+00013340: 7275 6e63 6174 6564 2073 7469 636b 2d62  runcated stick-b
+00013350: 7265 616b 696e 6720 7765 6967 6874 732e  reaking weights.
+00013360: 2054 6865 2077 6569 6768 7473 2061 7265   The weights are
+00013370: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
+00013380: 610a 2020 2020 7374 6963 6b2d 6272 6561  a.    stick-brea
+00013390: 6b69 6e67 2070 726f 6365 6475 6365 2077  king proceduce w
+000133a0: 6865 7265 203a 6d61 7468 3a60 785f 6b20  here :math:`x_k 
+000133b0: 3d20 765f 6b20 5c70 726f 645f 7b5c 656c  = v_k \prod_{\el
+000133c0: 6c20 3c20 6b7d 2028 3120 2d20 765f 5c65  l < k} (1 - v_\e
+000133d0: 6c6c 2960 2066 6f72 0a20 2020 203a 6d61  ll)` for.    :ma
+000133e0: 7468 3a60 6b20 5c69 6e20 5c7b 312c 205c  th:`k \in \{1, \
+000133f0: 6c64 6f74 732c 204b 5c7d 6020 616e 6420  ldots, K\}` and 
+00013400: 3a6d 6174 683a 6078 5f4b 203d 205c 7072  :math:`x_K = \pr
+00013410: 6f64 5f7b 5c65 6c6c 203d 2031 7d5e 7b4b  od_{\ell = 1}^{K
+00013420: 7d20 2831 202d 2076 5f5c 656c 6c29 203d  } (1 - v_\ell) =
+00013430: 2031 202d 205c 7375 6d5f 7b5c 656c 6c3d   1 - \sum_{\ell=
+00013440: 317d 5e4b 2078 5f5c 656c 6c60 0a20 2020  1}^K x_\ell`.   
+00013450: 2077 6974 6820 3a6d 6174 683a 6076 5f6b   with :math:`v_k
+00013460: 205c 7374 6163 6b72 656c 7b5c 7465 7874   \stackrel{\text
+00013470: 7b69 2e69 2e64 2e7d 7d7b 5c73 696d 7d20  {i.i.d.}}{\sim} 
+00013480: 5c74 6578 747b 4265 7461 7d28 312c 205c  \text{Beta}(1, \
+00013490: 616c 7068 6129 602e 0a0a 2020 2020 2e2e  alpha)`...    ..
+000134a0: 206d 6174 683a 0a0a 2020 2020 2020 2020   math:..        
+000134b0: 6628 5c6d 6174 6862 667b 787d 7c5c 616c  f(\mathbf{x}|\al
+000134c0: 7068 612c 204b 2920 3d0a 2020 2020 2020  pha, K) =.      
+000134d0: 2020 2020 2020 4228 312c 205c 616c 7068        B(1, \alph
+000134e0: 6129 5e7b 2d4b 7d78 5f7b 4b2b 317d 5e5c  a)^{-K}x_{K+1}^\
+000134f0: 616c 7068 6120 5c70 726f 645f 7b6b 3d31  alpha \prod_{k=1
+00013500: 7d5e 7b4b 2b31 7d5c 6c65 6674 5c7b 5c73  }^{K+1}\left\{\s
+00013510: 756d 5f7b 6a3d 6b7d 5e7b 4b2b 317d 2078  um_{j=k}^{K+1} x
+00013520: 5f6a 5c72 6967 6874 5c7d 5e7b 2d31 7d0a  _j\right\}^{-1}.
+00013530: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
+00013540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
+00013570: 2020 2053 7570 706f 7274 2020 203a 6d61     Support   :ma
+00013580: 7468 3a60 785f 6b20 5c69 6e20 2830 2c20  th:`x_k \in (0, 
+00013590: 3129 6020 666f 7220 3a6d 6174 683a 606b  1)` for :math:`k
+000135a0: 205c 696e 205c 7b31 2c20 5c6c 646f 7473   \in \{1, \ldots
+000135b0: 2c20 4b2b 315c 7d60 0a20 2020 2020 2020  , K+1\}`.       
+000135c0: 2020 2020 2020 2073 7563 6820 7468 6174         such that
+000135d0: 203a 6d61 7468 3a60 5c73 756d 2078 5f6b   :math:`\sum x_k
+000135e0: 203d 2031 600a 2020 2020 4d65 616e 2020   = 1`.    Mean  
+000135f0: 2020 2020 3a6d 6174 683a 605c 6d61 7468      :math:`\math
+00013600: 6262 7b45 7d5b 785f 6b5d 203d 205c 6466  bb{E}[x_k] = \df
+00013610: 7261 637b 317d 7b31 202b 205c 616c 7068  rac{1}{1 + \alph
+00013620: 617d 5c6c 6566 7428 5c64 6672 6163 7b5c  a}\left(\dfrac{\
+00013630: 616c 7068 617d 7b31 202b 205c 616c 7068  alpha}{1 + \alph
+00013640: 617d 5c72 6967 6874 295e 7b6b 202d 2031  a}\right)^{k - 1
+00013650: 7d60 0a20 2020 2020 2020 2020 2020 2020  }`.             
+00013660: 2066 6f72 203a 6d61 7468 3a60 6b20 5c69   for :math:`k \i
+00013670: 6e20 5c7b 312c 205c 6c64 6f74 732c 204b  n \{1, \ldots, K
+00013680: 5c7d 6020 616e 6420 3a6d 6174 683a 605c  \}` and :math:`\
+00013690: 6d61 7468 6262 7b45 7d5b 785f 7b4b 2b31  mathbb{E}[x_{K+1
+000136a0: 7d5d 203d 205c 6c65 6674 285c 6466 7261  }] = \left(\dfra
+000136b0: 637b 5c61 6c70 6861 7d7b 3120 2b20 5c61  c{\alpha}{1 + \a
+000136c0: 6c70 6861 7d5c 7269 6768 7429 5e7b 4b7d  lpha}\right)^{K}
+000136d0: 600a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  `.    ========  
+000136e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000136f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013700: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00013710: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00013720: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00013730: 2020 2061 6c70 6861 203a 2074 656e 736f     alpha : tenso
+00013740: 725f 6c69 6b65 206f 6620 666c 6f61 740a  r_like of float.
+00013750: 2020 2020 2020 2020 436f 6e63 656e 7472          Concentr
+00013760: 6174 696f 6e20 7061 7261 6d65 7465 7220  ation parameter 
+00013770: 2861 6c70 6861 203e 2030 292e 0a20 2020  (alpha > 0)..   
+00013780: 204b 203a 2074 656e 736f 725f 6c69 6b65   K : tensor_like
+00013790: 206f 6620 696e 740a 2020 2020 2020 2020   of int.        
+000137a0: 5468 6520 6e75 6d62 6572 206f 6620 2273  The number of "s
+000137b0: 7469 636b 7322 2074 6f20 6272 6561 6b20  ticks" to break 
+000137c0: 6f66 6620 6672 6f6d 2061 6e20 696e 6974  off from an init
+000137d0: 6961 6c20 6f6e 652d 756e 6974 2073 7469  ial one-unit sti
+000137e0: 636b 2e20 5468 6520 6c65 6e67 7468 206f  ck. The length o
+000137f0: 6620 7468 6520 7765 6967 6874 0a20 2020  f the weight.   
+00013800: 2020 2020 2076 6563 746f 7220 6973 204b       vector is K
+00013810: 202b 2031 2c20 7768 6572 6520 7468 6520   + 1, where the 
+00013820: 6c61 7374 2077 6569 6768 7420 6973 206f  last weight is o
+00013830: 6e65 206d 696e 7573 2074 6865 2073 756d  ne minus the sum
+00013840: 206f 6620 616c 6c20 7468 6520 6669 7273   of all the firs
+00013850: 7420 7374 6963 6b73 2e0a 0a20 2020 2052  t sticks...    R
+00013860: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
+00013870: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
+00013880: 5b31 5d20 4973 6877 6172 616e 2c20 482e  [1] Ishwaran, H.
+00013890: 2c20 2620 4a61 6d65 732c 204c 2e20 462e  , & James, L. F.
+000138a0: 2028 3230 3031 292e 2047 6962 6273 2073   (2001). Gibbs s
+000138b0: 616d 706c 696e 6720 6d65 7468 6f64 7320  ampling methods 
+000138c0: 666f 7220 7374 6963 6b2d 6272 6561 6b69  for stick-breaki
+000138d0: 6e67 2070 7269 6f72 732e 0a20 2020 2020  ng priors..     
+000138e0: 2020 2020 2020 4a6f 7572 6e61 6c20 6f66        Journal of
+000138f0: 2074 6865 2041 6d65 7269 6361 6e20 5374   the American St
+00013900: 6174 6973 7469 6361 6c20 4173 736f 6369  atistical Associ
+00013910: 6174 696f 6e2c 2039 3628 3435 3329 2c20  ation, 96(453), 
+00013920: 3136 312d 3137 332e 0a0a 2020 2020 2e2e  161-173...    ..
+00013930: 205b 325d 204d c3bc 6c6c 6572 2c20 502e   [2] M..ller, P.
+00013940: 2c20 5175 696e 7461 6e61 2c20 462e 2041  , Quintana, F. A
+00013950: 2e2c 204a 6172 612c 2041 2e2c 2026 2048  ., Jara, A., & H
+00013960: 616e 736f 6e2c 2054 2e20 2832 3031 3529  anson, T. (2015)
+00013970: 2e20 4261 7965 7369 616e 206e 6f6e 7061  . Bayesian nonpa
+00013980: 7261 6d65 7472 6963 2064 6174 610a 2020  rametric data.  
+00013990: 2020 2020 2020 2020 2061 6e61 6c79 7369           analysi
+000139a0: 732e 204e 6577 2059 6f72 6b3a 2053 7072  s. New York: Spr
+000139b0: 696e 6765 722e 0a20 2020 2022 2222 0a20  inger..    """. 
+000139c0: 2020 2072 765f 6f70 203d 2073 7469 636b     rv_op = stick
+000139d0: 6272 6561 6b69 6e67 7765 6967 6874 730a  breakingweights.
+000139e0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+000139f0: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
+00013a00: 6c73 2c20 616c 7068 612c 204b 2c20 2a61  ls, alpha, K, *a
+00013a10: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00013a20: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
+00013a30: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+00013a40: 6961 626c 6528 666c 6f61 7458 2861 6c70  iable(floatX(alp
+00013a50: 6861 2929 0a20 2020 2020 2020 204b 203d  ha)).        K =
+00013a60: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+00013a70: 7269 6162 6c65 2869 6e74 5828 4b29 290a  riable(intX(K)).
+00013a80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013a90: 7375 7065 7228 292e 6469 7374 285b 616c  super().dist([al
+00013aa0: 7068 612c 204b 5d2c 202a 2a6b 7761 7267  pha, K], **kwarg
+00013ab0: 7329 0a0a 2020 2020 6465 6620 6d6f 6d65  s)..    def mome
+00013ac0: 6e74 2872 762c 2073 697a 652c 2061 6c70  nt(rv, size, alp
+00013ad0: 6861 2c20 4b29 3a0a 2020 2020 2020 2020  ha, K):.        
+00013ae0: 616c 7068 6120 3d20 616c 7068 615b 2e2e  alpha = alpha[..
+00013af0: 2e2c 206e 702e 6e65 7761 7869 735d 0a20  ., np.newaxis]. 
+00013b00: 2020 2020 2020 206d 6f6d 656e 7420 3d20         moment = 
+00013b10: 2861 6c70 6861 202f 2028 3120 2b20 616c  (alpha / (1 + al
+00013b20: 7068 6129 2920 2a2a 2070 742e 6172 616e  pha)) ** pt.aran
+00013b30: 6765 284b 290a 2020 2020 2020 2020 6d6f  ge(K).        mo
+00013b40: 6d65 6e74 202a 3d20 3120 2f20 2831 202b  ment *= 1 / (1 +
+00013b50: 2061 6c70 6861 290a 2020 2020 2020 2020   alpha).        
+00013b60: 6d6f 6d65 6e74 203d 2070 742e 636f 6e63  moment = pt.conc
+00013b70: 6174 656e 6174 6528 5b6d 6f6d 656e 742c  atenate([moment,
+00013b80: 2028 616c 7068 6120 2f20 2831 202b 2061   (alpha / (1 + a
+00013b90: 6c70 6861 2929 202a 2a20 4b5d 2c20 6178  lpha)) ** K], ax
+00013ba0: 6973 3d2d 3129 0a20 2020 2020 2020 2069  is=-1).        i
+00013bb0: 6620 6e6f 7420 7276 5f73 697a 655f 6973  f not rv_size_is
+00013bc0: 5f6e 6f6e 6528 7369 7a65 293a 0a20 2020  _none(size):.   
+00013bd0: 2020 2020 2020 2020 206d 6f6d 656e 745f           moment_
+00013be0: 7369 7a65 203d 2070 742e 636f 6e63 6174  size = pt.concat
+00013bf0: 656e 6174 6528 0a20 2020 2020 2020 2020  enate(.         
+00013c00: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00013c10: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+00013c20: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00013c30: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c50: 204b 202b 2031 2c0a 2020 2020 2020 2020   K + 1,.        
+00013c60: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00013c70: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00013c80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00013c90: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
+00013ca0: 7420 3d20 7074 2e66 756c 6c28 6d6f 6d65  t = pt.full(mome
+00013cb0: 6e74 5f73 697a 652c 206d 6f6d 656e 7429  nt_size, moment)
+00013cc0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00013cd0: 206d 6f6d 656e 740a 0a20 2020 2064 6566   moment..    def
+00013ce0: 206c 6f67 7028 7661 6c75 652c 2061 6c70   logp(value, alp
+00013cf0: 6861 2c20 4b29 3a0a 2020 2020 2020 2020  ha, K):.        
+00013d00: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
+00013d10: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
+00013d20: 696c 6974 7920 6f66 2074 6865 2064 6973  ility of the dis
+00013d30: 7472 6962 7574 696f 6e20 696e 6475 6365  tribution induce
+00013d40: 6420 6672 6f6d 2074 6865 2073 7469 636b  d from the stick
+00013d50: 2d62 7265 616b 696e 6720 7072 6f63 6573  -breaking proces
+00013d60: 730a 2020 2020 2020 2020 6174 2073 7065  s.        at spe
+00013d70: 6369 6669 6564 2076 616c 7565 2e0a 0a20  cified value... 
+00013d80: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00013d90: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00013da0: 2d2d 2d2d 0a20 2020 2020 2020 2076 616c  ----.        val
+00013db0: 7565 3a20 6e75 6d65 7269 630a 2020 2020  ue: numeric.    
+00013dc0: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
+00013dd0: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
+00013de0: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
+00013df0: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
+00013e00: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00013e10: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00013e20: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
+00013e30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013e40: 2020 206c 6f67 7020 3d20 2d70 742e 7375     logp = -pt.su
+00013e50: 6d28 0a20 2020 2020 2020 2020 2020 2070  m(.            p
+00013e60: 742e 6c6f 6728 0a20 2020 2020 2020 2020  t.log(.         
+00013e70: 2020 2020 2020 2070 742e 6375 6d73 756d         pt.cumsum
+00013e80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013e90: 2020 2020 2020 7661 6c75 655b 2e2e 2e2c        value[...,
+00013ea0: 203a 3a2d 315d 2c0a 2020 2020 2020 2020   ::-1],.        
+00013eb0: 2020 2020 2020 2020 2020 2020 6178 6973              axis
+00013ec0: 3d2d 312c 0a20 2020 2020 2020 2020 2020  =-1,.           
+00013ed0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00013ee0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00013ef0: 2020 6178 6973 3d2d 312c 0a20 2020 2020    axis=-1,.     
+00013f00: 2020 2029 0a20 2020 2020 2020 206c 6f67     ).        log
+00013f10: 7020 2b3d 202d 4b20 2a20 6265 7461 6c6e  p += -K * betaln
+00013f20: 2831 2c20 616c 7068 6129 0a20 2020 2020  (1, alpha).     
+00013f30: 2020 206c 6f67 7020 2b3d 2061 6c70 6861     logp += alpha
+00013f40: 202a 2070 742e 6c6f 6728 7661 6c75 655b   * pt.log(value[
+00013f50: 2e2e 2e2c 202d 315d 290a 0a20 2020 2020  ..., -1])..     
+00013f60: 2020 206c 6f67 7020 3d20 7074 2e73 7769     logp = pt.swi
+00013f70: 7463 6828 0a20 2020 2020 2020 2020 2020  tch(.           
+00013f80: 2070 742e 6f72 5f28 0a20 2020 2020 2020   pt.or_(.       
+00013f90: 2020 2020 2020 2020 2070 742e 616e 7928           pt.any(
+00013fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013fb0: 2020 2020 2070 742e 616e 645f 2870 742e       pt.and_(pt.
+00013fc0: 6c65 2876 616c 7565 2c20 3029 2c20 7074  le(value, 0), pt
+00013fd0: 2e67 6528 7661 6c75 652c 2031 2929 2c0a  .ge(value, 1)),.
+00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ff0: 2020 2020 6178 6973 3d2d 312c 0a20 2020      axis=-1,.   
+00014000: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014020: 7074 2e6f 725f 280a 2020 2020 2020 2020  pt.or_(.        
+00014030: 2020 2020 2020 2020 2020 2020 7074 2e62              pt.b
+00014040: 6974 7769 7365 5f6e 6f74 2870 742e 616c  itwise_not(pt.al
+00014050: 6c63 6c6f 7365 2876 616c 7565 2e73 756d  lclose(value.sum
+00014060: 282d 3129 2c20 3129 292c 0a20 2020 2020  (-1), 1)),.     
+00014070: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00014080: 742e 6e65 7128 7661 6c75 652e 7368 6170  t.neq(value.shap
+00014090: 655b 2d31 5d2c 204b 202b 2031 292c 0a20  e[-1], K + 1),. 
+000140a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000140b0: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
+000140c0: 0a20 2020 2020 2020 2020 2020 202d 6e70  .            -np
+000140d0: 2e69 6e66 2c0a 2020 2020 2020 2020 2020  .inf,.          
+000140e0: 2020 6c6f 6770 2c0a 2020 2020 2020 2020    logp,.        
+000140f0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00014100: 6e20 6368 6563 6b5f 7061 7261 6d65 7465  n check_paramete
+00014110: 7273 280a 2020 2020 2020 2020 2020 2020  rs(.            
+00014120: 6c6f 6770 2c0a 2020 2020 2020 2020 2020  logp,.          
+00014130: 2020 616c 7068 6120 3e20 302c 0a20 2020    alpha > 0,.   
+00014140: 2020 2020 2020 2020 204b 203e 2030 2c0a           K > 0,.
+00014150: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+00014160: 2261 6c70 6861 203e 2030 2c20 4b20 3e20  "alpha > 0, K > 
+00014170: 3022 2c0a 2020 2020 2020 2020 290a 0a0a  0",.        )...
+00014180: 636c 6173 7320 5a65 726f 5375 6d4e 6f72  class ZeroSumNor
+00014190: 6d61 6c52 5628 5379 6d62 6f6c 6963 5261  malRV(SymbolicRa
+000141a0: 6e64 6f6d 5661 7269 6162 6c65 293a 0a20  ndomVariable):. 
+000141b0: 2020 2022 2222 5a65 726f 5375 6d4e 6f72     """ZeroSumNor
+000141c0: 6d61 6c20 7261 6e64 6f6d 2076 6172 6961  mal random varia
+000141d0: 626c 6522 2222 0a0a 2020 2020 5f70 7269  ble"""..    _pri
+000141e0: 6e74 5f6e 616d 6520 3d20 2822 5a65 726f  nt_name = ("Zero
+000141f0: 5375 6d4e 6f72 6d61 6c22 2c20 225c 5c6f  SumNormal", "\\o
+00014200: 7065 7261 746f 726e 616d 657b 5a65 726f  peratorname{Zero
+00014210: 5375 6d4e 6f72 6d61 6c7d 2229 0a20 2020  SumNormal}").   
+00014220: 2064 6566 6175 6c74 5f6f 7574 7075 7420   default_output 
+00014230: 3d20 300a 0a0a 636c 6173 7320 5a65 726f  = 0...class Zero
+00014240: 5375 6d4e 6f72 6d61 6c28 4469 7374 7269  SumNormal(Distri
+00014250: 6275 7469 6f6e 293a 0a20 2020 2072 2222  bution):.    r""
+00014260: 220a 2020 2020 5a65 726f 5375 6d4e 6f72  ".    ZeroSumNor
+00014270: 6d61 6c20 6469 7374 7269 6275 7469 6f6e  mal distribution
+00014280: 2c20 692e 6520 4e6f 726d 616c 2064 6973  , i.e Normal dis
+00014290: 7472 6962 7574 696f 6e20 7768 6572 6520  tribution where 
+000142a0: 6f6e 6520 6f72 0a20 2020 2073 6576 6572  one or.    sever
+000142b0: 616c 2061 7865 7320 6172 6520 636f 6e73  al axes are cons
+000142c0: 7472 6169 6e65 6420 746f 2073 756d 2074  trained to sum t
+000142d0: 6f20 7a65 726f 2e0a 2020 2020 4279 2064  o zero..    By d
+000142e0: 6566 6175 6c74 2c20 7468 6520 6c61 7374  efault, the last
+000142f0: 2061 7869 7320 6973 2063 6f6e 7374 7261   axis is constra
+00014300: 696e 6564 2074 6f20 7375 6d20 746f 207a  ined to sum to z
+00014310: 6572 6f2e 0a20 2020 2053 6565 2060 6e5f  ero..    See `n_
+00014320: 7a65 726f 7375 6d5f 6178 6573 6020 6b77  zerosum_axes` kw
+00014330: 6172 6720 666f 7220 6d6f 7265 2064 6574  arg for more det
+00014340: 6169 6c73 2e0a 0a20 2020 202e 2e20 6d61  ails...    .. ma
+00014350: 7468 3a3a 0a0a 2020 2020 2020 2020 5c62  th::..        \b
+00014360: 6567 696e 7b61 6c69 676e 2a7d 0a20 2020  egin{align*}.   
+00014370: 2020 2020 2020 2020 205a 534e 285c 7369           ZSN(\si
+00014380: 676d 6129 203d 204e 205c 4269 6728 2030  gma) = N \Big( 0
+00014390: 2c20 5c73 6967 6d61 5e32 2028 4920 2d20  , \sigma^2 (I - 
+000143a0: 5c74 6672 6163 7b31 7d7b 6e7d 4a29 205c  \tfrac{1}{n}J) \
+000143b0: 4269 6729 205c 5c0a 2020 2020 2020 2020  Big) \\.        
+000143c0: 2020 2020 5c74 6578 747b 7768 6572 657d      \text{where}
+000143d0: 205c 207e 204a 5f7b 696a 7d20 3d20 3120   \ ~ J_{ij} = 1 
+000143e0: 5c20 7e20 5c74 6578 747b 616e 647d 205c  \ ~ \text{and} \
+000143f0: 5c0a 2020 2020 2020 2020 2020 2020 6e20  \.            n 
+00014400: 3d20 5c74 6578 747b 6e62 7220 6f66 207a  = \text{nbr of z
+00014410: 6572 6f2d 7375 6d20 6178 6573 7d0a 2020  ero-sum axes}.  
+00014420: 2020 2020 2020 5c65 6e64 7b61 6c69 676e        \end{align
+00014430: 2a7d 0a0a 2020 2020 5061 7261 6d65 7465  *}..    Paramete
+00014440: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00014450: 2d0a 2020 2020 7369 676d 6120 3a20 7465  -.    sigma : te
+00014460: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
+00014470: 6174 0a20 2020 2020 2020 2053 6361 6c65  at.        Scale
+00014480: 2070 6172 616d 6574 6572 2028 7369 676d   parameter (sigm
+00014490: 6120 3e20 3029 2e0a 2020 2020 2020 2020  a > 0)..        
+000144a0: 4974 2773 2061 6374 7561 6c6c 7920 7468  It's actually th
+000144b0: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
+000144c0: 7469 6f6e 206f 6620 7468 6520 756e 6465  tion of the unde
+000144d0: 726c 7969 6e67 2c20 756e 636f 6e73 7472  rlying, unconstr
+000144e0: 6169 6e65 6420 4e6f 726d 616c 2064 6973  ained Normal dis
+000144f0: 7472 6962 7574 696f 6e2e 0a20 2020 2020  tribution..     
+00014500: 2020 2044 6566 6175 6c74 7320 746f 2031     Defaults to 1
+00014510: 2069 6620 6e6f 7420 7370 6563 6966 6965   if not specifie
+00014520: 642e 0a20 2020 2020 2020 2046 6f72 206e  d..        For n
+00014530: 6f77 2c20 6060 7369 676d 6160 6020 6861  ow, ``sigma`` ha
+00014540: 7320 746f 2062 6520 6120 7363 616c 6172  s to be a scalar
+00014550: 2c20 746f 2065 6e73 7572 6520 7468 6520  , to ensure the 
+00014560: 7a65 726f 2d73 756d 2063 6f6e 7374 7261  zero-sum constra
+00014570: 696e 742e 0a20 2020 206e 5f7a 6572 6f73  int..    n_zeros
+00014580: 756d 5f61 7865 733a 2069 6e74 2c20 6465  um_axes: int, de
+00014590: 6661 756c 7473 2074 6f20 310a 2020 2020  faults to 1.    
+000145a0: 2020 2020 4e75 6d62 6572 206f 6620 6178      Number of ax
+000145b0: 6573 2061 6c6f 6e67 2077 6869 6368 2074  es along which t
+000145c0: 6865 207a 6572 6f2d 7375 6d20 636f 6e73  he zero-sum cons
+000145d0: 7472 6169 6e74 2069 7320 656e 666f 7263  traint is enforc
+000145e0: 6564 2c20 7374 6172 7469 6e67 2066 726f  ed, starting fro
+000145f0: 6d20 7468 6520 7269 6768 746d 6f73 7420  m the rightmost 
+00014600: 706f 7369 7469 6f6e 2e0a 2020 2020 2020  position..      
+00014610: 2020 4465 6661 756c 7473 2074 6f20 312c    Defaults to 1,
+00014620: 2069 2e65 2074 6865 2072 6967 6874 6d6f   i.e the rightmo
+00014630: 7374 2061 7869 732e 0a20 2020 207a 6572  st axis..    zer
+00014640: 6f73 756d 5f61 7865 733a 2069 6e74 2c20  osum_axes: int, 
+00014650: 6465 7072 6563 6174 6564 2070 6c65 6173  deprecated pleas
+00014660: 6520 7573 6520 6e5f 7a65 726f 7375 6d5f  e use n_zerosum_
+00014670: 6178 6573 2061 7320 6974 7320 7375 6363  axes as its succ
+00014680: 6573 736f 720a 2020 2020 6469 6d73 3a20  essor.    dims: 
+00014690: 7365 7175 656e 6365 206f 6620 7374 7269  sequence of stri
+000146a0: 6e67 732c 206f 7074 696f 6e61 6c0a 2020  ngs, optional.  
+000146b0: 2020 2020 2020 4469 6d65 6e73 696f 6e20        Dimension 
+000146c0: 6e61 6d65 7320 6f66 2074 6865 2064 6973  names of the dis
+000146d0: 7472 6962 7574 696f 6e2e 2057 6f72 6b73  tribution. Works
+000146e0: 2074 6865 2073 616d 6520 6173 2066 6f72   the same as for
+000146f0: 206f 7468 6572 2050 794d 4320 6469 7374   other PyMC dist
+00014700: 7269 6275 7469 6f6e 732e 0a20 2020 2020  ributions..     
+00014710: 2020 204e 6563 6573 7361 7279 2069 6620     Necessary if 
+00014720: 6060 7368 6170 6560 6020 6973 206e 6f74  ``shape`` is not
+00014730: 2070 6173 7365 642e 0a20 2020 2073 6861   passed..    sha
+00014740: 7065 3a20 7475 706c 6520 6f66 2069 6e74  pe: tuple of int
+00014750: 6567 6572 732c 206f 7074 696f 6e61 6c0a  egers, optional.
+00014760: 2020 2020 2020 2020 5368 6170 6520 6f66          Shape of
+00014770: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
+00014780: 6e2e 2057 6f72 6b73 2074 6865 2073 616d  n. Works the sam
+00014790: 6520 6173 2066 6f72 206f 7468 6572 2050  e as for other P
+000147a0: 794d 4320 6469 7374 7269 6275 7469 6f6e  yMC distribution
+000147b0: 732e 0a20 2020 2020 2020 204e 6563 6573  s..        Neces
+000147c0: 7361 7279 2069 6620 6060 6469 6d73 6060  sary if ``dims``
+000147d0: 206f 7220 6060 6f62 7365 7276 6564 6060   or ``observed``
+000147e0: 2069 7320 6e6f 7420 7061 7373 6564 2e0a   is not passed..
+000147f0: 0a20 2020 2057 6172 6e69 6e67 730a 2020  .    Warnings.  
+00014800: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2060    --------.    `
+00014810: 6073 6967 6d61 6060 2068 6173 2074 6f20  `sigma`` has to 
+00014820: 6265 2061 2073 6361 6c61 722c 2074 6f20  be a scalar, to 
+00014830: 656e 7375 7265 2074 6865 207a 6572 6f2d  ensure the zero-
+00014840: 7375 6d20 636f 6e73 7472 6169 6e74 2e0a  sum constraint..
+00014850: 2020 2020 5468 6520 6162 696c 6974 7920      The ability 
+00014860: 746f 2073 7065 6369 6679 2061 2076 6563  to specify a vec
+00014870: 746f 7220 6f66 2060 6073 6967 6d61 6060  tor of ``sigma``
+00014880: 206d 6179 2062 6520 6164 6465 6420 696e   may be added in
+00014890: 2066 7574 7572 6520 7665 7273 696f 6e73   future versions
+000148a0: 2e0a 0a20 2020 2060 606e 5f7a 6572 6f73  ...    ``n_zeros
+000148b0: 756d 5f61 7865 7360 6020 6861 7320 746f  um_axes`` has to
+000148c0: 2062 6520 3e20 302e 2049 6620 796f 7520   be > 0. If you 
+000148d0: 7761 6e74 2074 6865 2062 6568 6176 696f  want the behavio
+000148e0: 7220 6f66 2060 606e 5f7a 6572 6f73 756d  r of ``n_zerosum
+000148f0: 5f61 7865 7320 3d20 3060 602c 0a20 2020  _axes = 0``,.   
+00014900: 206a 7573 7420 7573 6520 6060 706d 2e4e   just use ``pm.N
+00014910: 6f72 6d61 6c60 602e 0a0a 2020 2020 4578  ormal``...    Ex
+00014920: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00014930: 2d2d 2d0a 2020 2020 4465 6669 6e65 2061  ---.    Define a
+00014940: 2060 5a65 726f 5375 6d4e 6f72 6d61 6c60   `ZeroSumNormal`
+00014950: 2076 6172 6961 626c 652c 2077 6974 6820   variable, with 
+00014960: 6073 6967 6d61 3d31 6020 616e 640a 2020  `sigma=1` and.  
+00014970: 2020 606e 5f7a 6572 6f73 756d 5f61 7865    `n_zerosum_axe
+00014980: 733d 3160 2020 6279 2064 6566 6175 6c74  s=1`  by default
+00014990: 3a3a 0a0a 2020 2020 2020 2020 434f 4f52  ::..        COOR
+000149a0: 4453 203d 207b 0a20 2020 2020 2020 2020  DS = {.         
+000149b0: 2020 2022 7265 6769 6f6e 7322 3a20 5b22     "regions": ["
+000149c0: 6122 2c20 2262 222c 2022 6322 5d2c 0a20  a", "b", "c"],. 
+000149d0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
+000149e0: 6572 7322 3a20 5b22 7965 7322 2c20 226e  ers": ["yes", "n
+000149f0: 6f22 2c20 2277 6861 7465 7665 7222 2c20  o", "whatever", 
+00014a00: 2264 6f6e 2774 2075 6e64 6572 7374 616e  "don't understan
+00014a10: 6420 7175 6573 7469 6f6e 225d 2c0a 2020  d question"],.  
+00014a20: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00014a30: 7769 7468 2070 6d2e 4d6f 6465 6c28 636f  with pm.Model(co
+00014a40: 6f72 6473 3d43 4f4f 5244 5329 2061 7320  ords=COORDS) as 
+00014a50: 6d3a 0a20 2020 2020 2020 2020 2020 2023  m:.            #
+00014a60: 2074 6865 207a 6572 6f20 7375 6d20 6178   the zero sum ax
+00014a70: 6973 2077 696c 6c20 6265 2027 616e 7377  is will be 'answ
+00014a80: 6572 7327 0a20 2020 2020 2020 2020 2020  ers'.           
+00014a90: 2076 203d 2070 6d2e 5a65 726f 5375 6d4e   v = pm.ZeroSumN
+00014aa0: 6f72 6d61 6c28 2276 222c 2064 696d 733d  ormal("v", dims=
+00014ab0: 2822 7265 6769 6f6e 7322 2c20 2261 6e73  ("regions", "ans
+00014ac0: 7765 7273 2229 290a 0a20 2020 2020 2020  wers"))..       
+00014ad0: 2077 6974 6820 706d 2e4d 6f64 656c 2863   with pm.Model(c
+00014ae0: 6f6f 7264 733d 434f 4f52 4453 2920 6173  oords=COORDS) as
+00014af0: 206d 3a0a 2020 2020 2020 2020 2020 2020   m:.            
+00014b00: 2320 7468 6520 7a65 726f 2073 756d 2061  # the zero sum a
+00014b10: 7865 7320 7769 6c6c 2062 6520 2761 6e73  xes will be 'ans
+00014b20: 7765 7273 2720 616e 6420 2772 6567 696f  wers' and 'regio
+00014b30: 6e73 270a 2020 2020 2020 2020 2020 2020  ns'.            
+00014b40: 7620 3d20 706d 2e5a 6572 6f53 756d 4e6f  v = pm.ZeroSumNo
+00014b50: 726d 616c 2822 7622 2c20 6469 6d73 3d28  rmal("v", dims=(
+00014b60: 2272 6567 696f 6e73 222c 2022 616e 7377  "regions", "answ
+00014b70: 6572 7322 292c 206e 5f7a 6572 6f73 756d  ers"), n_zerosum
+00014b80: 5f61 7865 733d 3229 0a0a 2020 2020 2020  _axes=2)..      
+00014b90: 2020 7769 7468 2070 6d2e 4d6f 6465 6c28    with pm.Model(
+00014ba0: 636f 6f72 6473 3d43 4f4f 5244 5329 2061  coords=COORDS) a
+00014bb0: 7320 6d3a 0a20 2020 2020 2020 2020 2020  s m:.           
+00014bc0: 2023 2074 6865 207a 6572 6f20 7375 6d20   # the zero sum 
+00014bd0: 6178 6573 2077 696c 6c20 6265 2074 6865  axes will be the
+00014be0: 206c 6173 7420 7477 6f0a 2020 2020 2020   last two.      
+00014bf0: 2020 2020 2020 7620 3d20 706d 2e5a 6572        v = pm.Zer
+00014c00: 6f53 756d 4e6f 726d 616c 2822 7622 2c20  oSumNormal("v", 
+00014c10: 7368 6170 653d 2833 2c20 342c 2035 292c  shape=(3, 4, 5),
+00014c20: 206e 5f7a 6572 6f73 756d 5f61 7865 733d   n_zerosum_axes=
+00014c30: 3229 0a20 2020 2022 2222 0a20 2020 2072  2).    """.    r
+00014c40: 765f 7479 7065 203d 205a 6572 6f53 756d  v_type = ZeroSum
+00014c50: 4e6f 726d 616c 5256 0a0a 2020 2020 6465  NormalRV..    de
+00014c60: 6620 5f5f 6e65 775f 5f28 0a20 2020 2020  f __new__(.     
+00014c70: 2020 2063 6c73 2c20 2a61 7267 732c 207a     cls, *args, z
+00014c80: 6572 6f73 756d 5f61 7865 733d 4e6f 6e65  erosum_axes=None
+00014c90: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
+00014ca0: 3d4e 6f6e 652c 2073 7570 706f 7274 5f73  =None, support_s
+00014cb0: 6861 7065 3d4e 6f6e 652c 2064 696d 733d  hape=None, dims=
+00014cc0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 0a20  None, **kwargs. 
+00014cd0: 2020 2029 3a0a 2020 2020 2020 2020 6966     ):.        if
+00014ce0: 207a 6572 6f73 756d 5f61 7865 7320 6973   zerosum_axes is
+00014cf0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00014d00: 2020 2020 2020 206e 5f7a 6572 6f73 756d         n_zerosum
+00014d10: 5f61 7865 7320 3d20 7a65 726f 7375 6d5f  _axes = zerosum_
+00014d20: 6178 6573 0a20 2020 2020 2020 2020 2020  axes.           
+00014d30: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d50: 2254 6865 2027 7a65 726f 7375 6d5f 6178  "The 'zerosum_ax
+00014d60: 6573 2720 7061 7261 6d65 7465 7220 6973  es' parameter is
+00014d70: 2064 6570 7265 6361 7465 642e 2055 7365   deprecated. Use
+00014d80: 2027 6e5f 7a65 726f 7375 6d5f 6178 6573   'n_zerosum_axes
+00014d90: 2720 696e 7374 6561 642e 222c 0a20 2020  ' instead.",.   
+00014da0: 2020 2020 2020 2020 2020 2020 2044 6570               Dep
+00014db0: 7265 6361 7469 6f6e 5761 726e 696e 672c  recationWarning,
+00014dc0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00014dd0: 2020 2020 2020 2069 6620 6469 6d73 2069         if dims i
+00014de0: 7320 6e6f 7420 4e6f 6e65 206f 7220 6b77  s not None or kw
+00014df0: 6172 6773 2e67 6574 2822 6f62 7365 7276  args.get("observ
+00014e00: 6564 2229 2069 7320 6e6f 7420 4e6f 6e65  ed") is not None
+00014e10: 3a0a 2020 2020 2020 2020 2020 2020 6e5f  :.            n_
+00014e20: 7a65 726f 7375 6d5f 6178 6573 203d 2063  zerosum_axes = c
+00014e30: 6c73 2e63 6865 636b 5f7a 6572 6f73 756d  ls.check_zerosum
+00014e40: 5f61 7865 7328 6e5f 7a65 726f 7375 6d5f  _axes(n_zerosum_
+00014e50: 6178 6573 290a 0a20 2020 2020 2020 2020  axes)..         
+00014e60: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
+00014e70: 203d 2067 6574 5f73 7570 706f 7274 5f73   = get_support_s
+00014e80: 6861 7065 280a 2020 2020 2020 2020 2020  hape(.          
+00014e90: 2020 2020 2020 7375 7070 6f72 745f 7368        support_sh
+00014ea0: 6170 653d 7375 7070 6f72 745f 7368 6170  ape=support_shap
+00014eb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00014ec0: 2020 2073 6861 7065 3d4e 6f6e 652c 2020     shape=None,  
+00014ed0: 2320 5368 6170 6520 7769 6c6c 2062 6520  # Shape will be 
+00014ee0: 6368 6563 6b65 6420 696e 2060 636c 732e  checked in `cls.
+00014ef0: 6469 7374 600a 2020 2020 2020 2020 2020  dist`.          
+00014f00: 2020 2020 2020 6469 6d73 3d64 696d 732c        dims=dims,
+00014f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014f20: 206f 6273 6572 7665 643d 6b77 6172 6773   observed=kwargs
+00014f30: 2e67 6574 2822 6f62 7365 7276 6564 222c  .get("observed",
+00014f40: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
+00014f50: 2020 2020 2020 2020 6e64 696d 5f73 7570          ndim_sup
+00014f60: 703d 6e5f 7a65 726f 7375 6d5f 6178 6573  p=n_zerosum_axes
+00014f70: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00014f80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014f90: 7375 7065 7228 292e 5f5f 6e65 775f 5f28  super().__new__(
+00014fa0: 0a20 2020 2020 2020 2020 2020 2063 6c73  .            cls
+00014fb0: 2c0a 2020 2020 2020 2020 2020 2020 2a61  ,.            *a
+00014fc0: 7267 732c 0a20 2020 2020 2020 2020 2020  rgs,.           
+00014fd0: 206e 5f7a 6572 6f73 756d 5f61 7865 733d   n_zerosum_axes=
+00014fe0: 6e5f 7a65 726f 7375 6d5f 6178 6573 2c0a  n_zerosum_axes,.
+00014ff0: 2020 2020 2020 2020 2020 2020 7375 7070              supp
+00015000: 6f72 745f 7368 6170 653d 7375 7070 6f72  ort_shape=suppor
+00015010: 745f 7368 6170 652c 0a20 2020 2020 2020  t_shape,.       
+00015020: 2020 2020 2064 696d 733d 6469 6d73 2c0a       dims=dims,.
+00015030: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+00015040: 6172 6773 2c0a 2020 2020 2020 2020 290a  args,.        ).
+00015050: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00015060: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
+00015070: 6c73 2c20 7369 676d 613d 312c 206e 5f7a  ls, sigma=1, n_z
+00015080: 6572 6f73 756d 5f61 7865 733d 4e6f 6e65  erosum_axes=None
+00015090: 2c20 7375 7070 6f72 745f 7368 6170 653d  , support_shape=
+000150a0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
+000150b0: 0a20 2020 2020 2020 206e 5f7a 6572 6f73  .        n_zeros
+000150c0: 756d 5f61 7865 7320 3d20 636c 732e 6368  um_axes = cls.ch
+000150d0: 6563 6b5f 7a65 726f 7375 6d5f 6178 6573  eck_zerosum_axes
+000150e0: 286e 5f7a 6572 6f73 756d 5f61 7865 7329  (n_zerosum_axes)
+000150f0: 0a0a 2020 2020 2020 2020 7369 676d 6120  ..        sigma 
+00015100: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00015110: 6172 6961 626c 6528 666c 6f61 7458 2873  ariable(floatX(s
+00015120: 6967 6d61 2929 0a20 2020 2020 2020 2069  igma)).        i
+00015130: 6620 7369 676d 612e 6e64 696d 203e 2030  f sigma.ndim > 0
+00015140: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00015150: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00015160: 7369 676d 6120 6861 7320 746f 2062 6520  sigma has to be 
+00015170: 6120 7363 616c 6172 2229 0a0a 2020 2020  a scalar")..    
+00015180: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
+00015190: 6520 3d20 6765 745f 7375 7070 6f72 745f  e = get_support_
+000151a0: 7368 6170 6528 0a20 2020 2020 2020 2020  shape(.         
+000151b0: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
+000151c0: 3d73 7570 706f 7274 5f73 6861 7065 2c0a  =support_shape,.
+000151d0: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+000151e0: 653d 6b77 6172 6773 2e67 6574 2822 7368  e=kwargs.get("sh
+000151f0: 6170 6522 292c 0a20 2020 2020 2020 2020  ape"),.         
+00015200: 2020 206e 6469 6d5f 7375 7070 3d6e 5f7a     ndim_supp=n_z
+00015210: 6572 6f73 756d 5f61 7865 732c 0a20 2020  erosum_axes,.   
+00015220: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00015230: 6966 2073 7570 706f 7274 5f73 6861 7065  if support_shape
+00015240: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00015250: 2020 2020 2020 6966 206e 5f7a 6572 6f73        if n_zeros
+00015260: 756d 5f61 7865 7320 3e20 303a 0a20 2020  um_axes > 0:.   
+00015270: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00015280: 7365 2056 616c 7565 4572 726f 7228 2259  se ValueError("Y
+00015290: 6f75 206d 7573 7420 7370 6563 6966 7920  ou must specify 
+000152a0: 6469 6d73 2c20 7368 6170 6520 6f72 2073  dims, shape or s
+000152b0: 7570 706f 7274 5f73 6861 7065 2070 6172  upport_shape par
+000152c0: 616d 6574 6572 2229 0a20 2020 2020 2020  ameter").       
+000152d0: 2020 2020 2023 2054 4f44 4f3a 2065 6467       # TODO: edg
+000152e0: 652d 6361 7365 2064 6f65 736e 2774 2077  e-case doesn't w
+000152f0: 6f72 6b20 666f 7220 6e6f 772c 2062 6563  ork for now, bec
+00015300: 6175 7365 2070 742e 7374 6163 6b20 696e  ause pt.stack in
+00015310: 2067 6574 5f73 7570 706f 7274 5f73 6861   get_support_sha
+00015320: 7065 2066 6169 6c73 0a20 2020 2020 2020  pe fails.       
+00015330: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+00015340: 2020 2020 2020 2020 2023 2020 2020 2073           #     s
+00015350: 7570 706f 7274 5f73 6861 7065 203d 2028  upport_shape = (
+00015360: 2920 2320 6265 6361 7573 6520 6974 2773  ) # because it's
+00015370: 206a 7573 7420 6120 4e6f 726d 616c 2069   just a Normal i
+00015380: 6e20 7468 6174 2063 6173 650a 2020 2020  n that case.    
+00015390: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
+000153a0: 6520 3d20 7074 2e61 735f 7465 6e73 6f72  e = pt.as_tensor
+000153b0: 5f76 6172 6961 626c 6528 696e 7458 2873  _variable(intX(s
+000153c0: 7570 706f 7274 5f73 6861 7065 2929 0a0a  upport_shape))..
+000153d0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+000153e0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d3d  _zerosum_axes ==
+000153f0: 2070 742e 6765 745f 7665 6374 6f72 5f6c   pt.get_vector_l
+00015400: 656e 6774 6828 0a20 2020 2020 2020 2020  ength(.         
+00015410: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
+00015420: 0a20 2020 2020 2020 2029 2c20 2273 7570  .        ), "sup
+00015430: 706f 7274 5f73 6861 7065 2068 6173 2074  port_shape has t
+00015440: 6f20 6265 2061 7320 6c6f 6e67 2061 7320  o be as long as 
+00015450: 6e5f 7a65 726f 7375 6d5f 6178 6573 220a  n_zerosum_axes".
+00015460: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00015470: 7375 7065 7228 292e 6469 7374 280a 2020  super().dist(.  
+00015480: 2020 2020 2020 2020 2020 5b73 6967 6d61            [sigma
+00015490: 5d2c 206e 5f7a 6572 6f73 756d 5f61 7865  ], n_zerosum_axe
+000154a0: 733d 6e5f 7a65 726f 7375 6d5f 6178 6573  s=n_zerosum_axes
+000154b0: 2c20 7375 7070 6f72 745f 7368 6170 653d  , support_shape=
+000154c0: 7375 7070 6f72 745f 7368 6170 652c 202a  support_shape, *
+000154d0: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
+000154e0: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+000154f0: 686f 640a 2020 2020 6465 6620 6368 6563  hod.    def chec
+00015500: 6b5f 7a65 726f 7375 6d5f 6178 6573 2863  k_zerosum_axes(c
+00015510: 6c73 2c20 6e5f 7a65 726f 7375 6d5f 6178  ls, n_zerosum_ax
+00015520: 6573 3a20 4f70 7469 6f6e 616c 5b69 6e74  es: Optional[int
+00015530: 5d29 202d 3e20 696e 743a 0a20 2020 2020  ]) -> int:.     
+00015540: 2020 2069 6620 6e5f 7a65 726f 7375 6d5f     if n_zerosum_
+00015550: 6178 6573 2069 7320 4e6f 6e65 3a0a 2020  axes is None:.  
+00015560: 2020 2020 2020 2020 2020 6e5f 7a65 726f            n_zero
+00015570: 7375 6d5f 6178 6573 203d 2031 0a20 2020  sum_axes = 1.   
+00015580: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+00015590: 7374 616e 6365 286e 5f7a 6572 6f73 756d  stance(n_zerosum
+000155a0: 5f61 7865 732c 2069 6e74 293a 0a20 2020  _axes, int):.   
+000155b0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+000155c0: 7970 6545 7272 6f72 2822 6e5f 7a65 726f  ypeError("n_zero
+000155d0: 7375 6d5f 6178 6573 2068 6173 2074 6f20  sum_axes has to 
+000155e0: 6265 2061 6e20 696e 7465 6765 7222 290a  be an integer").
+000155f0: 2020 2020 2020 2020 6966 206e 6f74 206e          if not n
+00015600: 5f7a 6572 6f73 756d 5f61 7865 7320 3e20  _zerosum_axes > 
+00015610: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00015620: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00015630: 226e 5f7a 6572 6f73 756d 5f61 7865 7320  "n_zerosum_axes 
+00015640: 6861 7320 746f 2062 6520 3e20 3022 290a  has to be > 0").
+00015650: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00015660: 5f7a 6572 6f73 756d 5f61 7865 730a 0a20  _zerosum_axes.. 
+00015670: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00015680: 2020 2020 6465 6620 7276 5f6f 7028 636c      def rv_op(cl
+00015690: 732c 2073 6967 6d61 2c20 6e5f 7a65 726f  s, sigma, n_zero
+000156a0: 7375 6d5f 6178 6573 2c20 7375 7070 6f72  sum_axes, suppor
+000156b0: 745f 7368 6170 652c 2073 697a 653d 4e6f  t_shape, size=No
+000156c0: 6e65 293a 0a20 2020 2020 2020 2073 6861  ne):.        sha
+000156d0: 7065 203d 2074 6f5f 7475 706c 6528 7369  pe = to_tuple(si
+000156e0: 7a65 2920 2b20 7475 706c 6528 7375 7070  ze) + tuple(supp
+000156f0: 6f72 745f 7368 6170 6529 0a20 2020 2020  ort_shape).     
+00015700: 2020 206e 6f72 6d61 6c5f 6469 7374 203d     normal_dist =
+00015710: 2070 6d2e 4e6f 726d 616c 2e64 6973 7428   pm.Normal.dist(
+00015720: 7369 676d 613d 7369 676d 612c 2073 6861  sigma=sigma, sha
+00015730: 7065 3d73 6861 7065 290a 0a20 2020 2020  pe=shape)..     
+00015740: 2020 2069 6620 6e5f 7a65 726f 7375 6d5f     if n_zerosum_
+00015750: 6178 6573 203e 206e 6f72 6d61 6c5f 6469  axes > normal_di
+00015760: 7374 2e6e 6469 6d3a 0a20 2020 2020 2020  st.ndim:.       
+00015770: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00015780: 4572 726f 7228 2253 6861 7065 206f 6620  Error("Shape of 
+00015790: 6469 7374 7269 6275 7469 6f6e 2069 7320  distribution is 
+000157a0: 746f 6f20 736d 616c 6c20 666f 7220 7468  too small for th
+000157b0: 6520 6e75 6d62 6572 206f 6620 7a65 726f  e number of zero
+000157c0: 7375 6d20 6178 6573 2229 0a0a 2020 2020  sum axes")..    
+000157d0: 2020 2020 6e6f 726d 616c 5f64 6973 745f      normal_dist_
+000157e0: 2c20 7369 676d 615f 2c20 7375 7070 6f72  , sigma_, suppor
+000157f0: 745f 7368 6170 655f 203d 2028 0a20 2020  t_shape_ = (.   
+00015800: 2020 2020 2020 2020 206e 6f72 6d61 6c5f           normal_
+00015810: 6469 7374 2e74 7970 6528 292c 0a20 2020  dist.type(),.   
+00015820: 2020 2020 2020 2020 2073 6967 6d61 2e74           sigma.t
+00015830: 7970 6528 292c 0a20 2020 2020 2020 2020  ype(),.         
+00015840: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
+00015850: 2e74 7970 6528 292c 0a20 2020 2020 2020  .type(),.       
+00015860: 2029 0a0a 2020 2020 2020 2020 2320 5a65   )..        # Ze
+00015870: 726f 7375 6d2d 6e6f 726d 616c 696e 6720  rosum-normaling 
+00015880: 6973 2061 6368 6965 7665 6420 6279 2073  is achieved by s
+00015890: 7562 7472 6163 7469 6e67 2074 6865 206d  ubtracting the m
+000158a0: 6561 6e20 616c 6f6e 6720 7468 6520 6769  ean along the gi
+000158b0: 7665 6e20 6e5f 7a65 726f 7375 6d5f 6178  ven n_zerosum_ax
+000158c0: 6573 0a20 2020 2020 2020 207a 6572 6f73  es.        zeros
+000158d0: 756d 5f72 765f 203d 206e 6f72 6d61 6c5f  um_rv_ = normal_
+000158e0: 6469 7374 5f0a 2020 2020 2020 2020 666f  dist_.        fo
+000158f0: 7220 6178 6973 2069 6e20 7261 6e67 6528  r axis in range(
+00015900: 6e5f 7a65 726f 7375 6d5f 6178 6573 293a  n_zerosum_axes):
+00015910: 0a20 2020 2020 2020 2020 2020 207a 6572  .            zer
+00015920: 6f73 756d 5f72 765f 202d 3d20 7a65 726f  osum_rv_ -= zero
+00015930: 7375 6d5f 7276 5f2e 6d65 616e 2861 7869  sum_rv_.mean(axi
+00015940: 733d 2d61 7869 7320 2d20 312c 206b 6565  s=-axis - 1, kee
+00015950: 7064 696d 733d 5472 7565 290a 0a20 2020  pdims=True)..   
+00015960: 2020 2020 2072 6574 7572 6e20 5a65 726f       return Zero
+00015970: 5375 6d4e 6f72 6d61 6c52 5628 0a20 2020  SumNormalRV(.   
+00015980: 2020 2020 2020 2020 2069 6e70 7574 733d           inputs=
+00015990: 5b6e 6f72 6d61 6c5f 6469 7374 5f2c 2073  [normal_dist_, s
+000159a0: 6967 6d61 5f2c 2073 7570 706f 7274 5f73  igma_, support_s
+000159b0: 6861 7065 5f5d 2c0a 2020 2020 2020 2020  hape_],.        
+000159c0: 2020 2020 6f75 7470 7574 733d 5b7a 6572      outputs=[zer
+000159d0: 6f73 756d 5f72 765f 2c20 7375 7070 6f72  osum_rv_, suppor
+000159e0: 745f 7368 6170 655f 5d2c 0a20 2020 2020  t_shape_],.     
+000159f0: 2020 2020 2020 206e 6469 6d5f 7375 7070         ndim_supp
+00015a00: 3d6e 5f7a 6572 6f73 756d 5f61 7865 732c  =n_zerosum_axes,
+00015a10: 0a20 2020 2020 2020 2029 286e 6f72 6d61  .        )(norma
+00015a20: 6c5f 6469 7374 2c20 7369 676d 612c 2073  l_dist, sigma, s
+00015a30: 7570 706f 7274 5f73 6861 7065 290a 0a0a  upport_shape)...
+00015a40: 405f 6368 616e 6765 5f64 6973 745f 7369  @_change_dist_si
+00015a50: 7a65 2e72 6567 6973 7465 7228 5a65 726f  ze.register(Zero
+00015a60: 5375 6d4e 6f72 6d61 6c52 5629 0a64 6566  SumNormalRV).def
+00015a70: 2063 6861 6e67 655f 7a65 726f 7375 6d5f   change_zerosum_
+00015a80: 7369 7a65 286f 702c 206e 6f72 6d61 6c5f  size(op, normal_
+00015a90: 6469 7374 2c20 6e65 775f 7369 7a65 2c20  dist, new_size, 
+00015aa0: 6578 7061 6e64 3d46 616c 7365 293a 0a20  expand=False):. 
+00015ab0: 2020 206e 6f72 6d61 6c5f 6469 7374 2c20     normal_dist, 
+00015ac0: 7369 676d 612c 2073 7570 706f 7274 5f73  sigma, support_s
+00015ad0: 6861 7065 203d 206e 6f72 6d61 6c5f 6469  hape = normal_di
+00015ae0: 7374 2e6f 776e 6572 2e69 6e70 7574 730a  st.owner.inputs.
+00015af0: 0a20 2020 2069 6620 6578 7061 6e64 3a0a  .    if expand:.
+00015b00: 2020 2020 2020 2020 6f72 6967 696e 616c          original
+00015b10: 5f73 6861 7065 203d 2074 7570 6c65 286e  _shape = tuple(n
+00015b20: 6f72 6d61 6c5f 6469 7374 2e73 6861 7065  ormal_dist.shape
+00015b30: 290a 2020 2020 2020 2020 6f6c 645f 7369  ).        old_si
+00015b40: 7a65 203d 206f 7269 6769 6e61 6c5f 7368  ze = original_sh
+00015b50: 6170 655b 3a20 6c65 6e28 6f72 6967 696e  ape[: len(origin
+00015b60: 616c 5f73 6861 7065 2920 2d20 6f70 2e6e  al_shape) - op.n
+00015b70: 6469 6d5f 7375 7070 5d0a 2020 2020 2020  dim_supp].      
+00015b80: 2020 6e65 775f 7369 7a65 203d 2074 7570    new_size = tup
+00015b90: 6c65 286e 6577 5f73 697a 6529 202b 206f  le(new_size) + o
+00015ba0: 6c64 5f73 697a 650a 0a20 2020 2072 6574  ld_size..    ret
+00015bb0: 7572 6e20 5a65 726f 5375 6d4e 6f72 6d61  urn ZeroSumNorma
+00015bc0: 6c2e 7276 5f6f 7028 0a20 2020 2020 2020  l.rv_op(.       
+00015bd0: 2073 6967 6d61 3d73 6967 6d61 2c20 6e5f   sigma=sigma, n_
+00015be0: 7a65 726f 7375 6d5f 6178 6573 3d6f 702e  zerosum_axes=op.
+00015bf0: 6e64 696d 5f73 7570 702c 2073 7570 706f  ndim_supp, suppo
+00015c00: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
+00015c10: 5f73 6861 7065 2c20 7369 7a65 3d6e 6577  _shape, size=new
+00015c20: 5f73 697a 650a 2020 2020 290a 0a0a 405f  _size.    )...@_
+00015c30: 6d6f 6d65 6e74 2e72 6567 6973 7465 7228  moment.register(
+00015c40: 5a65 726f 5375 6d4e 6f72 6d61 6c52 5629  ZeroSumNormalRV)
+00015c50: 0a64 6566 207a 6572 6f73 756d 6e6f 726d  .def zerosumnorm
+00015c60: 616c 5f6d 6f6d 656e 7428 6f70 2c20 7276  al_moment(op, rv
+00015c70: 2c20 2a72 765f 696e 7075 7473 293a 0a20  , *rv_inputs):. 
+00015c80: 2020 2072 6574 7572 6e20 7074 2e7a 6572     return pt.zer
+00015c90: 6f73 5f6c 696b 6528 7276 290a 0a0a 405f  os_like(rv)...@_
+00015ca0: 6465 6661 756c 745f 7472 616e 7366 6f72  default_transfor
+00015cb0: 6d2e 7265 6769 7374 6572 285a 6572 6f53  m.register(ZeroS
+00015cc0: 756d 4e6f 726d 616c 5256 290a 6465 6620  umNormalRV).def 
+00015cd0: 7a65 726f 7375 6d5f 6465 6661 756c 745f  zerosum_default_
+00015ce0: 7472 616e 7366 6f72 6d28 6f70 2c20 7276  transform(op, rv
+00015cf0: 293a 0a20 2020 206e 5f7a 6572 6f73 756d  ):.    n_zerosum
+00015d00: 5f61 7865 7320 3d20 7475 706c 6528 6e70  _axes = tuple(np
+00015d10: 2e61 7261 6e67 6528 2d6f 702e 6e64 696d  .arange(-op.ndim
+00015d20: 5f73 7570 702c 2030 2929 0a20 2020 2072  _supp, 0)).    r
+00015d30: 6574 7572 6e20 5a65 726f 5375 6d54 7261  eturn ZeroSumTra
+00015d40: 6e73 666f 726d 286e 5f7a 6572 6f73 756d  nsform(n_zerosum
+00015d50: 5f61 7865 7329 0a0a 0a40 5f6c 6f67 7072  _axes)...@_logpr
+00015d60: 6f62 2e72 6567 6973 7465 7228 5a65 726f  ob.register(Zero
+00015d70: 5375 6d4e 6f72 6d61 6c52 5629 0a64 6566  SumNormalRV).def
+00015d80: 207a 6572 6f73 756d 6e6f 726d 616c 5f6c   zerosumnormal_l
+00015d90: 6f67 7028 6f70 2c20 7661 6c75 6573 2c20  ogp(op, values, 
+00015da0: 6e6f 726d 616c 5f64 6973 742c 2073 6967  normal_dist, sig
+00015db0: 6d61 2c20 7375 7070 6f72 745f 7368 6170  ma, support_shap
+00015dc0: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
+00015dd0: 2020 2876 616c 7565 2c29 203d 2076 616c    (value,) = val
+00015de0: 7565 730a 2020 2020 7368 6170 6520 3d20  ues.    shape = 
+00015df0: 7661 6c75 652e 7368 6170 650a 2020 2020  value.shape.    
+00015e00: 6e5f 7a65 726f 7375 6d5f 6178 6573 203d  n_zerosum_axes =
+00015e10: 206f 702e 6e64 696d 5f73 7570 700a 0a20   op.ndim_supp.. 
+00015e20: 2020 205f 6465 675f 6672 6565 5f73 7570     _deg_free_sup
+00015e30: 706f 7274 5f73 6861 7065 203d 2070 742e  port_shape = pt.
+00015e40: 696e 635f 7375 6274 656e 736f 7228 7368  inc_subtensor(sh
+00015e50: 6170 655b 2d6e 5f7a 6572 6f73 756d 5f61  ape[-n_zerosum_a
+00015e60: 7865 733a 5d2c 202d 3129 0a20 2020 205f  xes:], -1).    _
+00015e70: 6675 6c6c 5f73 697a 6520 3d20 7074 2e70  full_size = pt.p
+00015e80: 726f 6428 7368 6170 6529 0a20 2020 205f  rod(shape).    _
+00015e90: 6465 6772 6565 735f 6f66 5f66 7265 6564  degrees_of_freed
+00015ea0: 6f6d 203d 2070 742e 7072 6f64 285f 6465  om = pt.prod(_de
+00015eb0: 675f 6672 6565 5f73 7570 706f 7274 5f73  g_free_support_s
+00015ec0: 6861 7065 290a 0a20 2020 207a 6572 6f73  hape)..    zeros
+00015ed0: 756d 7320 3d20 5b0a 2020 2020 2020 2020  ums = [.        
+00015ee0: 7074 2e61 6c6c 2870 742e 6973 636c 6f73  pt.all(pt.isclos
+00015ef0: 6528 7074 2e6d 6561 6e28 7661 6c75 652c  e(pt.mean(value,
+00015f00: 2061 7869 733d 2d61 7869 7320 2d20 3129   axis=-axis - 1)
+00015f10: 2c20 302c 2061 746f 6c3d 3165 2d39 2929  , 0, atol=1e-9))
+00015f20: 0a20 2020 2020 2020 2066 6f72 2061 7869  .        for axi
+00015f30: 7320 696e 2072 616e 6765 286e 5f7a 6572  s in range(n_zer
+00015f40: 6f73 756d 5f61 7865 7329 0a20 2020 205d  osum_axes).    ]
+00015f50: 0a0a 2020 2020 6f75 7420 3d20 7074 2e73  ..    out = pt.s
+00015f60: 756d 280a 2020 2020 2020 2020 706d 2e6c  um(.        pm.l
+00015f70: 6f67 7028 6e6f 726d 616c 5f64 6973 742c  ogp(normal_dist,
+00015f80: 2076 616c 7565 2920 2a20 5f64 6567 7265   value) * _degre
+00015f90: 6573 5f6f 665f 6672 6565 646f 6d20 2f20  es_of_freedom / 
+00015fa0: 5f66 756c 6c5f 7369 7a65 2c0a 2020 2020  _full_size,.    
+00015fb0: 2020 2020 6178 6973 3d74 7570 6c65 286e      axis=tuple(n
+00015fc0: 702e 6172 616e 6765 282d 6e5f 7a65 726f  p.arange(-n_zero
+00015fd0: 7375 6d5f 6178 6573 2c20 3029 292c 0a20  sum_axes, 0)),. 
+00015fe0: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
+00015ff0: 2063 6865 636b 5f70 6172 616d 6574 6572   check_parameter
+00016000: 7328 6f75 742c 202a 7a65 726f 7375 6d73  s(out, *zerosums
+00016010: 2c20 6d73 673d 226d 6561 6e28 7661 6c75  , msg="mean(valu
+00016020: 652c 2061 7869 733d 6e5f 7a65 726f 7375  e, axis=n_zerosu
+00016030: 6d5f 6178 6573 2920 3d20 3022 290a       m_axes) = 0").
```

### Comparing `pymc-5.6.1/pymc/distributions/shape_utils.py` & `pymc-5.7.0/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/simulator.py` & `pymc-5.7.0/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/timeseries.py` & `pymc-5.7.0/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/transforms.py` & `pymc-5.7.0/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/distributions/truncated.py` & `pymc-5.7.0/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/exceptions.py` & `pymc-5.7.0/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/func_utils.py` & `pymc-5.7.0/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/gp/__init__.py` & `pymc-5.7.0/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/gp/cov.py` & `pymc-5.7.0/pymc/gp/cov.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import numbers
 import warnings
 
 from collections import Counter
 from functools import reduce
 from operator import add, mul
-from typing import Optional, Sequence
+from typing import Any, Callable, List, Optional, Sequence, Union
 
 import numpy as np
 import pytensor.tensor as pt
 
 from pytensor.graph.basic import Variable
 from pytensor.tensor.sharedvar import TensorSharedVariable
 from pytensor.tensor.var import TensorConstant, TensorVariable
@@ -37,27 +37,36 @@
     "Matern32",
     "Matern12",
     "Linear",
     "Polynomial",
     "Cosine",
     "Periodic",
     "WarpedInput",
+    "WrappedPeriodic",
     "Gibbs",
     "Coregion",
     "ScaledCov",
     "Kron",
 ]
 
+TensorLike = Union[np.ndarray, TensorVariable]
+IntSequence = Union[np.ndarray, Sequence[int]]
+
 
 class BaseCovariance:
     """
     Base class for kernels/covariance functions.
     """
 
-    def __call__(self, X, Xs=None, diag=False):
+    def __call__(
+        self,
+        X: TensorLike,
+        Xs: Optional[TensorLike] = None,
+        diag: bool = False,
+    ) -> TensorVariable:
         r"""
         Evaluate the kernel/covariance function.
 
         Parameters
         ----------
         X: The training inputs to the kernel.
         Xs: The optional prediction set of inputs the kernel.
@@ -67,40 +76,44 @@
             Default is False.
         """
         if diag:
             return self.diag(X)
         else:
             return self.full(X, Xs)
 
-    def diag(self, X):
+    def diag(self, X: TensorLike) -> TensorVariable:
         raise NotImplementedError
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         raise NotImplementedError
 
-    def __add__(self, other):
+    def __add__(self, other) -> "Add":
         # If it's a scalar, cast as Constant covariance.  This allows validation for power spectral
         # density calc.
         if isinstance(other, numbers.Real):
             other = Constant(c=other)
         return Add([self, other])
 
-    def __mul__(self, other):
+    def __mul__(self, other) -> "Prod":
         return Prod([self, other])
 
-    def __radd__(self, other):
+    def __radd__(self, other) -> "Add":
         return self.__add__(other)
 
-    def __rmul__(self, other):
+    def __rmul__(self, other) -> "Prod":
         return self.__mul__(other)
 
-    def __pow__(self, other):
+    def __pow__(self, other) -> "Exponentiated":
         other = pt.as_tensor_variable(other).squeeze()
         if not other.ndim == 0:
             raise ValueError("A covariance function can only be exponentiated by a scalar value")
+        if not isinstance(self, Covariance):
+            raise TypeError(
+                "Can only exponentiate covariance functions which inherit from `Covariance`"
+            )
         return Exponentiated(self, other)
 
     def __array_wrap__(self, result):
         """
         Required to allow radd/rmul by numpy arrays.
         """
         result = np.squeeze(result)
@@ -125,14 +138,18 @@
             return result[0][0]._factor_list[0] * A
         else:
             raise TypeError(
                 f"Unknown Covariance combination type {result[0][0]}.  "
                 "Known types are `Add` or `Prod`."
             )
 
+    @staticmethod
+    def _alloc(X, *shape: int) -> TensorVariable:
+        return pt.alloc(X, *shape)  # type: ignore
+
 
 class Covariance(BaseCovariance):
     """
     Base class for kernels/covariance functions with input_dim and active_dims, which excludes
     kernels like `Constant` and `WhiteNoise`.
 
     Parameters
@@ -141,36 +158,39 @@
         The number of input dimensions, or columns of X (or Xs)
         the kernel will operate on.
     active_dims: List of integers
         Indicate which dimension or column of X the covariance
         function operates on.
     """
 
-    def __init__(self, input_dim: int, active_dims: Optional[Sequence[int]] = None):
+    def __init__(self, input_dim: int, active_dims: Optional[IntSequence] = None):
         self.input_dim = input_dim
         if active_dims is None:
             self.active_dims = np.arange(input_dim)
         else:
             self.active_dims = np.asarray(active_dims, int)
 
         if max(self.active_dims) > self.input_dim:
             raise ValueError("Values in `active_dims` can't be larger than `input_dim`.")
 
     @property
-    def n_dims(self):
+    def n_dims(self) -> int:
         """The dimensionality of the input, as taken from the
         `active_dims`.
         """
         # Evaluate lazily in-case this changes.
         return len(self.active_dims)
 
     def _slice(self, X, Xs=None):
         xdims = X.shape[-1]
         if isinstance(xdims, Variable):
-            xdims = xdims.eval()
+            # Circular dependency
+            from pymc.pytensorf import constant_fold
+
+            [xdims] = constant_fold([xdims])
         if self.input_dim != xdims:
             warnings.warn(
                 f"Only {self.input_dim} column(s) out of {xdims} are"
                 " being used to compute the covariance function. If this"
                 " is not intended, increase 'input_dim' parameter to"
                 " the number of columns to use. Ignore otherwise.",
                 UserWarning,
@@ -178,15 +198,15 @@
         X = pt.as_tensor_variable(X[:, self.active_dims])
         if Xs is not None:
             Xs = pt.as_tensor_variable(Xs[:, self.active_dims])
         return X, Xs
 
 
 class Combination(Covariance):
-    def __init__(self, factor_list):
+    def __init__(self, factor_list: Sequence):
         """Use constituent factors to get input_dim and active_dims for the Combination covariance."""
 
         # Check if all input_dim are the same in factor_list
         input_dims = {factor.input_dim for factor in factor_list if isinstance(factor, Covariance)}
 
         if len(input_dims) != 1:
             raise ValueError("All covariances must have the same `input_dim`.")
@@ -203,19 +223,18 @@
                             if isinstance(factor, Covariance)
                         ]
                     )
                 ),
                 dtype=int,
             )
         )
-
         super().__init__(input_dim=input_dim, active_dims=active_dims)
 
         # Set up combination kernel, flatten out factor_list so that
-        self._factor_list = []
+        self._factor_list: List[Any] = []
         for factor in factor_list:
             if isinstance(factor, self.__class__):
                 self._factor_list.extend(factor._factor_list)
             else:
                 self._factor_list.append(factor)
 
     def _merge_factors_cov(self, X, Xs=None, diag=False):
@@ -291,43 +310,54 @@
                 # Otherwise defer the reduction to later
                 factor_list.append(factor)
 
         return factor_list
 
 
 class Add(Combination):
-    def __call__(self, X, Xs=None, diag=False):
+    def __call__(
+        self,
+        X: TensorLike,
+        Xs: Optional[TensorLike] = None,
+        diag: bool = False,
+    ) -> TensorVariable:
         return reduce(add, self._merge_factors_cov(X, Xs, diag))
 
-    def power_spectral_density(self, omega):
+    def power_spectral_density(self, omega: TensorLike) -> TensorVariable:
         return reduce(add, self._merge_factors_psd(omega))
 
 
 class Prod(Combination):
-    def __call__(self, X, Xs=None, diag=False):
+    def __call__(
+        self,
+        X: TensorLike,
+        Xs: Optional[TensorLike] = None,
+        diag: bool = False,
+    ) -> TensorVariable:
         return reduce(mul, self._merge_factors_cov(X, Xs, diag))
 
-    def power_spectral_density(self, omega):
+    def power_spectral_density(self, omega: TensorLike) -> TensorVariable:
         check = Counter([isinstance(factor, Covariance) for factor in self._factor_list])
-        if check.get(True) >= 2:
+        if check.get(True, 0) >= 2:
             raise NotImplementedError(
                 "The power spectral density of products of covariance "
                 "functions is not implemented."
             )
-
         return reduce(mul, self._merge_factors_psd(omega))
 
 
 class Exponentiated(Covariance):
-    def __init__(self, kernel, power):
+    def __init__(self, kernel: Covariance, power):
         self.kernel = kernel
         self.power = power
         super().__init__(input_dim=self.kernel.input_dim, active_dims=self.kernel.active_dims)
 
-    def __call__(self, X, Xs=None, diag=False):
+    def __call__(
+        self, X: TensorLike, Xs: Optional[TensorLike] = None, diag: bool = False
+    ) -> TensorVariable:
         return self.kernel(X, Xs, diag=diag) ** self.power
 
 
 class Kron(Covariance):
     r"""Form a covariance object that is the kronecker product of other covariances.
 
     In contrast to standard multiplication, where each covariance is given the
@@ -339,30 +369,32 @@
 
     Factors must be covariances or their combinations, arrays will not work.
 
     Generally utilized by the `gp.MarginalKron` and gp.LatentKron`
     implementations.
     """
 
-    def __init__(self, factor_list):
+    def __init__(self, factor_list: Sequence[Covariance]):
         self.input_dims = [factor.input_dim for factor in factor_list]
         input_dim = sum(self.input_dims)
         super().__init__(input_dim=input_dim)
         self._factor_list = factor_list
 
     def _split(self, X, Xs):
         indices = np.cumsum(self.input_dims)
         X_split = np.hsplit(X, indices)
         if Xs is not None:
             Xs_split = np.hsplit(Xs, indices)
         else:
             Xs_split = [None] * len(X_split)
         return X_split, Xs_split
 
-    def __call__(self, X, Xs=None, diag=False):
+    def __call__(
+        self, X: TensorLike, Xs: Optional[TensorLike] = None, diag: bool = False
+    ) -> TensorVariable:
         X_split, Xs_split = self._split(X, Xs)
         covs = [cov(x, xs, diag) for cov, x, xs in zip(self._factor_list, X_split, Xs_split)]
         return reduce(mul, covs)
 
 
 class Constant(BaseCovariance):
     r"""
@@ -372,44 +404,44 @@
 
        k(x, x') = c
     """
 
     def __init__(self, c):
         self.c = c
 
-    def diag(self, X):
-        return pt.alloc(self.c, X.shape[0])
+    def diag(self, X: TensorLike) -> TensorVariable:
+        return self._alloc(self.c, X.shape[0])
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         if Xs is None:
-            return pt.alloc(self.c, X.shape[0], X.shape[0])
+            return self._alloc(self.c, X.shape[0], X.shape[0])
         else:
-            return pt.alloc(self.c, X.shape[0], Xs.shape[0])
+            return self._alloc(self.c, X.shape[0], Xs.shape[0])
 
 
 class WhiteNoise(BaseCovariance):
     r"""
     White noise covariance function.
 
     .. math::
 
        k(x, x') = \sigma^2 \mathrm{I}
     """
 
     def __init__(self, sigma):
         self.sigma = sigma
 
-    def diag(self, X):
-        return pt.alloc(pt.square(self.sigma), X.shape[0])
+    def diag(self, X: TensorLike) -> TensorVariable:
+        return self._alloc(pt.square(self.sigma), X.shape[0])
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         if Xs is None:
             return pt.diag(self.diag(X))
         else:
-            return pt.alloc(0.0, X.shape[0], Xs.shape[0])
+            return self._alloc(0.0, X.shape[0], Xs.shape[0])
 
 
 class Circular(Covariance):
     R"""
     Circular Kernel.
 
     .. math::
@@ -436,49 +468,61 @@
 
     References
     ----------
     .. [1] Espéran Padonou, O Roustant, "Polar Gaussian Processes for Predicting on Circular Domains"
     https://hal.archives-ouvertes.fr/hal-01119942v1/document
     """
 
-    def __init__(self, input_dim, period, tau=4, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        period,
+        tau=4,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, active_dims)
         self.c = pt.as_tensor_variable(period / 2)
         self.tau = tau
 
     def dist(self, X, Xs):
         if Xs is None:
             Xs = pt.transpose(X)
         else:
             Xs = pt.transpose(Xs)
         return pt.abs((X - Xs + self.c) % (self.c * 2) - self.c)
 
     def weinland(self, t):
         return (1 + self.tau * t / self.c) * pt.clip(1 - t / self.c, 0, np.inf) ** self.tau
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xs = self._slice(X, Xs)
         return self.weinland(self.dist(X, Xs))
 
-    def diag(self, X):
-        return pt.alloc(1.0, X.shape[0])
+    def diag(self, X: TensorLike) -> TensorVariable:
+        return self._alloc(1.0, X.shape[0])
 
 
 class Stationary(Covariance):
     r"""
     Base class for stationary kernels/covariance functions.
 
     Parameters
     ----------
     ls: Lengthscale.  If input_dim > 1, a list or array of scalars or PyMC random
-    variables.  If input_dim == 1, a scalar or PyMC random variable.
+        variables.  If input_dim == 1, a scalar or PyMC random variable.
     ls_inv: Inverse lengthscale.  1 / ls.  One of ls or ls_inv must be provided.
     """
 
-    def __init__(self, input_dim, ls=None, ls_inv=None, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        ls=None,
+        ls_inv=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, active_dims)
         if (ls is None and ls_inv is None) or (ls is not None and ls_inv is not None):
             raise ValueError("Only one of 'ls' or 'ls_inv' must be provided")
         elif ls_inv is not None:
             if isinstance(ls_inv, (list, tuple)):
                 ls = 1.0 / np.asarray(ls_inv)
             else:
@@ -498,76 +542,50 @@
             sqd = -2.0 * pt.dot(X, pt.transpose(Xs)) + (
                 pt.reshape(X2, (-1, 1)) + pt.reshape(Xs2, (1, -1))
             )
         return pt.clip(sqd, 0.0, np.inf)
 
     def euclidean_dist(self, X, Xs):
         r2 = self.square_dist(X, Xs)
+        return self._sqrt(r2)
+
+    def _sqrt(self, r2):
         return pt.sqrt(r2 + 1e-12)
 
-    def diag(self, X):
-        return pt.alloc(1.0, X.shape[0])
+    def diag(self, X: TensorLike) -> TensorVariable:
+        return self._alloc(1.0, X.shape[0])
 
-    def full(self, X, Xs=None):
-        raise NotImplementedError
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
+        X, Xs = self._slice(X, Xs)
+        r2 = self.square_dist(X, Xs)
+        return self.full_from_distance(r2, squared=True)
 
-    def power_spectral_density(self, omega):
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
         raise NotImplementedError
 
-
-class Periodic(Stationary):
-    r"""
-    The Periodic kernel.
-
-    .. math::
-       k(x, x') = \mathrm{exp}\left( -\frac{\mathrm{sin}^2(\pi |x-x'| \frac{1}{T})}{2\ell^2} \right)
-
-    Notes
-    -----
-    Note that the scaling factor for this kernel is different compared to the more common
-    definition (see [1]_). Here, 0.5 is in the exponent instead of the more common value, 2.
-    Divide the length-scale by 2 when initializing the kernel to recover the standard definition.
-
-    References
-    ----------
-    .. [1] David Duvenaud, "The Kernel Cookbook"
-       https://www.cs.toronto.edu/~duvenaud/cookbook/
-    """
-
-    def __init__(self, input_dim, period, ls=None, ls_inv=None, active_dims=None):
-        super().__init__(input_dim, ls, ls_inv, active_dims)
-        self.period = period
-
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
-        if Xs is None:
-            Xs = X
-        f1 = X.dimshuffle(0, "x", 1)
-        f2 = Xs.dimshuffle("x", 0, 1)
-        r = np.pi * (f1 - f2) / self.period
-        r = pt.sum(pt.square(pt.sin(r) / self.ls), 2)
-        return pt.exp(-0.5 * r)
+    def power_spectral_density(self, omega: TensorLike) -> TensorVariable:
+        raise NotImplementedError
 
 
 class ExpQuad(Stationary):
     r"""
     The Exponentiated Quadratic kernel.  Also referred to as the Squared
     Exponential, or Radial Basis Function kernel.
 
     .. math::
 
        k(x, x') = \mathrm{exp}\left[ -\frac{(x - x')^2}{2 \ell^2} \right]
 
     """
 
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
-        return pt.exp(-0.5 * self.square_dist(X, Xs))
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r2 = dist if squared else dist**2
+        return pt.exp(-0.5 * r2)
 
-    def power_spectral_density(self, omega):
+    def power_spectral_density(self, omega: TensorLike) -> TensorVariable:
         r"""
         The power spectral density for the ExpQuad kernel is:
 
         .. math::
 
            S(\boldsymbol\omega) =
                (\sqrt(2 \pi)^D \prod_{i}^{D}\ell_i
@@ -584,22 +602,29 @@
     The Rational Quadratic kernel.
 
     .. math::
 
        k(x, x') = \left(1 + \frac{(x - x')^2}{2\alpha\ell^2} \right)^{-\alpha}
     """
 
-    def __init__(self, input_dim, alpha, ls=None, ls_inv=None, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        alpha,
+        ls=None,
+        ls_inv=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, ls, ls_inv, active_dims)
         self.alpha = alpha
 
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r2 = dist if squared else dist**2
         return pt.power(
-            (1.0 + 0.5 * self.square_dist(X, Xs) * (1.0 / self.alpha)),
+            (1.0 + 0.5 * r2 * (1.0 / self.alpha)),
             -1.0 * self.alpha,
         )
 
 
 class Matern52(Stationary):
     r"""
     The Matern kernel with nu = 5/2.
@@ -607,20 +632,19 @@
     .. math::
 
        k(x, x') = \left(1 + \frac{\sqrt{5(x - x')^2}}{\ell} +
                    \frac{5(x-x')^2}{3\ell^2}\right)
                    \mathrm{exp}\left[ - \frac{\sqrt{5(x - x')^2}}{\ell} \right]
     """
 
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
-        r = self.euclidean_dist(X, Xs)
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r = self._sqrt(dist) if squared else dist
         return (1.0 + np.sqrt(5.0) * r + 5.0 / 3.0 * pt.square(r)) * pt.exp(-1.0 * np.sqrt(5.0) * r)
 
-    def power_spectral_density(self, omega):
+    def power_spectral_density(self, omega: TensorLike) -> TensorVariable:
         r"""
         The power spectral density for the Matern52 kernel is:
 
         .. math::
 
            S(\boldsymbol\omega) =
                \frac{2^D \pi^{\frac{D}{2}} \Gamma(\frac{D+5}{2}) 5^{5/2}}
@@ -647,20 +671,19 @@
 
     .. math::
 
        k(x, x') = \left(1 + \frac{\sqrt{3(x - x')^2}}{\ell}\right)
                   \mathrm{exp}\left[ - \frac{\sqrt{3(x - x')^2}}{\ell} \right]
     """
 
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
-        r = self.euclidean_dist(X, Xs)
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r = self._sqrt(dist) if squared else dist
         return (1.0 + np.sqrt(3.0) * r) * pt.exp(-np.sqrt(3.0) * r)
 
-    def power_spectral_density(self, omega):
+    def power_spectral_density(self, omega: TensorLike) -> TensorVariable:
         r"""
         The power spectral density for the Matern32 kernel is:
 
         .. math::
 
             S(\boldsymbol\omega) =
                 \frac{2^D \pi^{D/2} \Gamma\left(\frac{D+3}{2}\right) 3^{3/2}}
@@ -686,95 +709,141 @@
     The Matern kernel with nu = 1/2
 
     .. math::
 
         k(x, x') = \mathrm{exp}\left[ -\frac{(x - x')^2}{\ell} \right]
     """
 
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
-        r = self.euclidean_dist(X, Xs)
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r = self._sqrt(dist) if squared else dist
         return pt.exp(-r)
 
 
 class Exponential(Stationary):
     r"""
     The Exponential kernel.
 
     .. math::
 
        k(x, x') = \mathrm{exp}\left[ -\frac{||x - x'||}{2\ell} \right]
     """
 
-    def full(self, X, Xs=None):
-        X, Xs = self._slice(X, Xs)
-        return pt.exp(-0.5 * self.euclidean_dist(X, Xs))
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r = self._sqrt(dist) if squared else dist
+        return pt.exp(-0.5 * r)
 
 
 class Cosine(Stationary):
     r"""
     The Cosine kernel.
 
     .. math::
        k(x, x') = \mathrm{cos}\left( 2 \pi \frac{||x - x'||}{ \ell^2} \right)
     """
 
-    def full(self, X, Xs=None):
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        r = self._sqrt(dist) if squared else dist
+        return pt.cos(2.0 * np.pi * r)
+
+
+class Periodic(Stationary):
+    r"""
+    The Periodic kernel.
+
+    .. math::
+       k(x, x') = \mathrm{exp}\left( -\frac{\mathrm{sin}^2(\pi |x-x'| \frac{1}{T})}{2\ell^2} \right)
+
+    Notes
+    -----
+    Note that the scaling factor for this kernel is different compared to the more common
+    definition (see [1]_). Here, 0.5 is in the exponent instead of the more common value, 2.
+    Divide the length-scale by 2 when initializing the kernel to recover the standard definition.
+
+    References
+    ----------
+    .. [1] David Duvenaud, "The Kernel Cookbook"
+       https://www.cs.toronto.edu/~duvenaud/cookbook/
+    """
+
+    def __init__(
+        self,
+        input_dim: int,
+        period,
+        ls=None,
+        ls_inv=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
+        super().__init__(input_dim, ls, ls_inv, active_dims)
+        self.period = period
+
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xs = self._slice(X, Xs)
-        return pt.cos(2.0 * np.pi * self.euclidean_dist(X, Xs))
+        if Xs is None:
+            Xs = X
+        f1 = pt.expand_dims(X, axis=(0,))
+        f2 = pt.expand_dims(Xs, axis=(1,))
+        r = np.pi * (f1 - f2) / self.period
+        r2 = pt.sum(pt.square(pt.sin(r) / self.ls), 2)
+        return self.full_from_distance(r2, squared=True)
+
+    def full_from_distance(self, dist: TensorLike, squared: bool = False) -> TensorVariable:
+        # NOTE: This is the same as the ExpQuad as we assume the periodicity
+        # has already been accounted for in the distance
+        r2 = dist if squared else dist**2
+        return pt.exp(-0.5 * r2)
 
 
 class Linear(Covariance):
     r"""
     The Linear kernel.
 
     .. math::
        k(x, x') = (x - c)(x' - c)
     """
 
-    def __init__(self, input_dim, c, active_dims=None):
+    def __init__(self, input_dim: int, c, active_dims: Optional[IntSequence] = None):
         super().__init__(input_dim, active_dims)
         self.c = c
 
     def _common(self, X, Xs=None):
         X, Xs = self._slice(X, Xs)
         Xc = pt.sub(X, self.c)
         return X, Xc, Xs
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xc, Xs = self._common(X, Xs)
         if Xs is None:
             return pt.dot(Xc, pt.transpose(Xc))
         else:
             Xsc = pt.sub(Xs, self.c)
             return pt.dot(Xc, pt.transpose(Xsc))
 
-    def diag(self, X):
+    def diag(self, X: TensorLike) -> TensorVariable:
         X, Xc, _ = self._common(X, None)
         return pt.sum(pt.square(Xc), 1)
 
 
 class Polynomial(Linear):
     r"""
     The Polynomial kernel.
 
     .. math::
        k(x, x') = [(x - c)(x' - c) + \mathrm{offset}]^{d}
     """
 
-    def __init__(self, input_dim, c, d, offset, active_dims=None):
+    def __init__(self, input_dim: int, c, d, offset, active_dims: Optional[IntSequence] = None):
         super().__init__(input_dim, c, active_dims)
         self.d = d
         self.offset = offset
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         linear = super().full(X, Xs)
         return pt.power(linear + self.offset, self.d)
 
-    def diag(self, X):
+    def diag(self, X: TensorLike) -> TensorVariable:
         linear = super().diag(X)
         return pt.power(linear + self.offset, self.d)
 
 
 class WarpedInput(Covariance):
     r"""
     Warp the inputs of any kernel using an arbitrary function
@@ -788,36 +857,109 @@
     cov_func: Covariance
     warp_func: callable
         PyTensor function of X and additional optional arguments.
     args: optional, tuple or list of scalars or PyMC variables
         Additional inputs (besides X or Xs) to warp_func.
     """
 
-    def __init__(self, input_dim, cov_func, warp_func, args=None, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        cov_func: Covariance,
+        warp_func: Callable,
+        args=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, active_dims)
         if not callable(warp_func):
             raise TypeError("warp_func must be callable")
         if not isinstance(cov_func, Covariance):
             raise TypeError("Must be or inherit from the Covariance class")
-        self.w = handle_args(warp_func, args)
+        self.w = handle_args(warp_func)
         self.args = args
         self.cov_func = cov_func
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xs = self._slice(X, Xs)
         if Xs is None:
             return self.cov_func(self.w(X, self.args), Xs)
         else:
             return self.cov_func(self.w(X, self.args), self.w(Xs, self.args))
 
-    def diag(self, X):
+    def diag(self, X: TensorLike) -> TensorVariable:
         X, _ = self._slice(X, None)
         return self.cov_func(self.w(X, self.args), diag=True)
 
 
+class WrappedPeriodic(Covariance):
+    r"""
+    The `WrappedPeriodic` kernel constructs periodic kernels from any `Stationary` kernel.
+
+    This is done by warping the input with the function
+
+    .. math::
+        \mathbf{u}(x) = \left(
+            \mathrm{sin} \left( \frac{2\pi x}{T} \right),
+            \mathrm{cos} \left( \frac{2\pi x}{T} \right)
+        \right)
+
+    The original derivation as applied to the squared exponential kernel can
+    be found in [1] or referenced in Chapter 4, page 92 of [2].
+
+    Notes
+    -----
+    Note that we drop the resulting scaling by 4 found in the original derivation
+    so that the interpretation of the length scales is consistent between the
+    underlying kernel and the periodic version.
+
+    Examples
+    --------
+    In order to construct a kernel equivalent to the `Periodic` kernel you
+    can do the following (though using `Periodic` will likely be a bit faster):
+
+    .. code:: python
+
+        exp_quad = pm.gp.cov.ExpQuad(1, ls=0.5)
+        cov = pm.gp.cov.WrappedPeriodic(exp_quad, period=5)
+
+    References
+    ----------
+    .. [1] MacKay, D. J. C. (1998). Introduction to Gaussian Processes.
+       In Bishop, C. M., editor, Neural Networks and Machine Learning. Springer-Verlag
+    .. [2] Rasmussen, C. E., & Williams, C. K. I. (2006). Gaussian processes for machine learning. MIT Press.
+       http://gaussianprocess.org/gpml/chapters/
+
+    Parameters
+    ----------
+    cov_func: Stationary
+        Base kernel or covariance function
+    period: Period
+    """
+
+    def __init__(self, cov_func: Stationary, period):
+        super().__init__(cov_func.input_dim, cov_func.active_dims)
+        if not isinstance(cov_func, Stationary):
+            raise TypeError("Must inherit from the Stationary class")
+        self.cov_func = cov_func
+        self.period = period
+
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
+        X, Xs = self._slice(X, Xs)
+        if Xs is None:
+            Xs = X
+        f1 = pt.expand_dims(X, axis=(0,))
+        f2 = pt.expand_dims(Xs, axis=(1,))
+        r = np.pi * (f1 - f2) / self.period
+        r2 = pt.sum(pt.square(pt.sin(r) / self.cov_func.ls), 2)
+        return self.cov_func.full_from_distance(r2, squared=True)
+
+    def diag(self, X: TensorLike) -> TensorVariable:
+        return self._alloc(1.0, X.shape[0])
+
+
 class Gibbs(Covariance):
     r"""
     The Gibbs kernel.  Use an arbitrary lengthscale function defined
     using PyTensor.  Only tested in one dimension.
 
     .. math::
        k(x, x') = \sqrt{\frac{2\ell(x)\ell(x')}{\ell^2(x) + \ell^2(x')}}
@@ -828,25 +970,31 @@
     ----------
     lengthscale_func: callable
         PyTensor function of X and additional optional arguments.
     args: optional, tuple or list of scalars or PyMC variables
         Additional inputs (besides X or Xs) to lengthscale_func.
     """
 
-    def __init__(self, input_dim, lengthscale_func, args=None, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        lengthscale_func: Callable,
+        args=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, active_dims)
         if active_dims is not None:
             if len(active_dims) > 1:
                 raise NotImplementedError(("Higher dimensional inputs ", "are untested"))
         else:
             if input_dim != 1:
                 raise NotImplementedError(("Higher dimensional inputs ", "are untested"))
         if not callable(lengthscale_func):
             raise TypeError("lengthscale_func must be callable")
-        self.lfunc = handle_args(lengthscale_func, args)
+        self.lfunc = handle_args(lengthscale_func)
         self.args = args
 
     def square_dist(self, X, Xs=None):
         X2 = pt.sum(pt.square(X), 1)
         if Xs is None:
             sqd = -2.0 * pt.dot(X, pt.transpose(X)) + (
                 pt.reshape(X2, (-1, 1)) + pt.reshape(X2, (1, -1))
@@ -854,29 +1002,29 @@
         else:
             Xs2 = pt.sum(pt.square(Xs), 1)
             sqd = -2.0 * pt.dot(X, pt.transpose(Xs)) + (
                 pt.reshape(X2, (-1, 1)) + pt.reshape(Xs2, (1, -1))
             )
         return pt.clip(sqd, 0.0, np.inf)
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xs = self._slice(X, Xs)
         rx = self.lfunc(pt.as_tensor_variable(X), self.args)
         if Xs is None:
             rz = self.lfunc(pt.as_tensor_variable(X), self.args)
             r2 = self.square_dist(X, X)
         else:
             rz = self.lfunc(pt.as_tensor_variable(Xs), self.args)
             r2 = self.square_dist(X, Xs)
         rx2 = pt.reshape(pt.square(rx), (-1, 1))
         rz2 = pt.reshape(pt.square(rz), (1, -1))
         return pt.sqrt((2.0 * pt.outer(rx, rz)) / (rx2 + rz2)) * pt.exp(-1.0 * r2 / (rx2 + rz2))
 
-    def diag(self, X):
-        return pt.alloc(1.0, X.shape[0])
+    def diag(self, X: TensorLike) -> TensorVariable:
+        return self._alloc(1.0, X.shape[0])
 
 
 class ScaledCov(Covariance):
     r"""
     Construct a kernel by multiplying a base kernel with a scaling
     function defined using PyTensor.  The scaling function is
     non-negative, and can be parameterized.
@@ -890,31 +1038,38 @@
         Base kernel or covariance function
     scaling_func: callable
         PyTensor function of X and additional optional arguments.
     args: optional, tuple or list of scalars or PyMC variables
         Additional inputs (besides X or Xs) to lengthscale_func.
     """
 
-    def __init__(self, input_dim, cov_func, scaling_func, args=None, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        cov_func: Covariance,
+        scaling_func: Callable,
+        args=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, active_dims)
         if not callable(scaling_func):
             raise TypeError("scaling_func must be callable")
         if not isinstance(cov_func, Covariance):
             raise TypeError("Must be or inherit from the Covariance class")
         self.cov_func = cov_func
-        self.scaling_func = handle_args(scaling_func, args)
+        self.scaling_func = handle_args(scaling_func)
         self.args = args
 
-    def diag(self, X):
+    def diag(self, X: TensorLike) -> TensorVariable:
         X, _ = self._slice(X, None)
         cov_diag = self.cov_func(X, diag=True)
         scf_diag = pt.square(pt.flatten(self.scaling_func(X, self.args)))
         return cov_diag * scf_diag
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xs = self._slice(X, Xs)
         scf_x = self.scaling_func(X, self.args)
         if Xs is None:
             return pt.outer(scf_x, scf_x) * self.cov_func(X)
         else:
             scf_xs = self.scaling_func(Xs, self.args)
             return pt.outer(scf_x, scf_xs) * self.cov_func(X, Xs)
@@ -949,15 +1104,22 @@
 
     Notes
     -----
     Exactly one dimension must be active for this kernel. Thus, if
     `input_dim != 1`, then `active_dims` must have a length of one.
     """
 
-    def __init__(self, input_dim, W=None, kappa=None, B=None, active_dims=None):
+    def __init__(
+        self,
+        input_dim: int,
+        W=None,
+        kappa=None,
+        B=None,
+        active_dims: Optional[IntSequence] = None,
+    ):
         super().__init__(input_dim, active_dims)
         if len(self.active_dims) != 1:
             raise ValueError("Coregion requires exactly one dimension to be active")
         make_B = W is not None or kappa is not None
         if make_B and B is not None:
             raise ValueError("Exactly one of (W, kappa) and B must be provided to Coregion")
         if make_B:
@@ -965,30 +1127,30 @@
             self.kappa = pt.as_tensor_variable(kappa)
             self.B = pt.dot(self.W, self.W.T) + pt.diag(self.kappa)
         elif B is not None:
             self.B = pt.as_tensor_variable(B)
         else:
             raise ValueError("Exactly one of (W, kappa) and B must be provided to Coregion")
 
-    def full(self, X, Xs=None):
+    def full(self, X: TensorLike, Xs: Optional[TensorLike] = None) -> TensorVariable:
         X, Xs = self._slice(X, Xs)
         index = pt.cast(X, "int32")
         if Xs is None:
             index2 = index.T
         else:
             index2 = pt.cast(Xs, "int32").T
         return self.B[index, index2]
 
-    def diag(self, X):
+    def diag(self, X: TensorLike) -> TensorVariable:
         X, _ = self._slice(X, None)
         index = pt.cast(X, "int32")
         return pt.diag(self.B)[index.ravel()]
 
 
-def handle_args(func, args):
+def handle_args(func: Callable) -> Callable:
     def f(x, args):
         if args is None:
             return func(x)
         else:
             if not isinstance(args, tuple):
                 args = (args,)
             return func(x, *args)
```

### Comparing `pymc-5.6.1/pymc/gp/gp.py` & `pymc-5.7.0/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/gp/hsgp_approx.py` & `pymc-5.7.0/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/gp/mean.py` & `pymc-5.7.0/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/gp/util.py` & `pymc-5.7.0/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/initial_point.py` & `pymc-5.7.0/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/__init__.py` & `pymc-5.7.0/pymc/logprob/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 # isort: off
 # Add rewrites to the DBs
 import pymc.logprob.binary
 import pymc.logprob.censoring
 import pymc.logprob.cumsum
 import pymc.logprob.checks
 import pymc.logprob.mixture
+import pymc.logprob.order
 import pymc.logprob.scan
 import pymc.logprob.tensor
 import pymc.logprob.transforms
 
 # isort: on
 
 __all__ = (
```

### Comparing `pymc-5.6.1/pymc/logprob/abstract.py` & `pymc-5.7.0/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/basic.py` & `pymc-5.7.0/pymc/logprob/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/binary.py` & `pymc-5.7.0/pymc/logprob/binary.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/censoring.py` & `pymc-5.7.0/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/checks.py` & `pymc-5.7.0/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/cumsum.py` & `pymc-5.7.0/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/mixture.py` & `pymc-5.7.0/pymc/logprob/mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,25 @@
 
 import pytensor
 import pytensor.tensor as pt
 
 from pytensor.graph.basic import Apply, Constant, Variable
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.op import Op, compute_test_value
-from pytensor.graph.rewriting.basic import node_rewriter, pre_greedy_node_rewriter
+from pytensor.graph.rewriting.basic import EquilibriumGraphRewriter, node_rewriter
 from pytensor.ifelse import IfElse, ifelse
 from pytensor.scalar import Switch
 from pytensor.scalar import switch as scalar_switch
 from pytensor.tensor.basic import Join, MakeVector, switch
 from pytensor.tensor.random.rewriting import (
     local_dimshuffle_rv_lift,
     local_rv_size_lift,
     local_subtensor_rv_lift,
 )
+from pytensor.tensor.rewriting.shape import ShapeFeature
 from pytensor.tensor.shape import shape_tuple
 from pytensor.tensor.subtensor import (
     AdvancedSubtensor,
     AdvancedSubtensor1,
     as_index_literal,
     get_canonical_form_slice,
     is_basic_idx,
@@ -73,15 +74,14 @@
 from pymc.logprob.rewriting import (
     PreserveRVMappings,
     assume_measured_ir_outputs,
     local_lift_DiracDelta,
     measurable_ir_rewrites_db,
     subtensor_ops,
 )
-from pymc.logprob.tensor import naive_bcast_rv_lift
 from pymc.logprob.utils import check_potential_measurability
 
 
 def is_newaxis(x):
     return isinstance(x, type(None)) or isinstance(getattr(x, "type", None), NoneTypeT)
 
 
@@ -199,29 +199,25 @@
         assert expanded_idx.ndim <= n_output_dims
 
         adv_indices.append(expanded_idx)
 
     return cast(Tuple[TensorVariable], tuple(pt.broadcast_arrays(*adv_indices)))
 
 
-def rv_pull_down(x: TensorVariable, dont_touch_vars=None) -> TensorVariable:
+def rv_pull_down(x: TensorVariable) -> TensorVariable:
     """Pull a ``RandomVariable`` ``Op`` down through a graph, when possible."""
-    fgraph = FunctionGraph(outputs=dont_touch_vars or [], clone=False)
-
-    return pre_greedy_node_rewriter(
-        fgraph,
-        [
-            local_rv_size_lift,
-            local_dimshuffle_rv_lift,
-            local_subtensor_rv_lift,
-            naive_bcast_rv_lift,
-            local_lift_DiracDelta,
-        ],
-        x,
-    )
+    fgraph = FunctionGraph(outputs=[x], clone=False, features=[ShapeFeature()])
+    rewrites = [
+        local_rv_size_lift,
+        local_dimshuffle_rv_lift,
+        local_subtensor_rv_lift,
+        local_lift_DiracDelta,
+    ]
+    EquilibriumGraphRewriter(rewrites, max_use_ratio=100).rewrite(fgraph)
+    return fgraph.outputs[0]
 
 
 class MixtureRV(Op):
     """A placeholder used to specify a log-likelihood for a mixture sub-graph."""
 
     __props__ = ("indices_end_idx", "out_dtype", "out_broadcastable")
```

### Comparing `pymc-5.6.1/pymc/logprob/rewriting.py` & `pymc-5.7.0/pymc/logprob/rewriting.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,27 +53,29 @@
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.replace import clone_replace
 from pytensor.graph.rewriting.basic import (
     ChangeTracker,
     EquilibriumGraphRewriter,
     GraphRewriter,
     node_rewriter,
+    out2in,
 )
 from pytensor.graph.rewriting.db import (
     LocalGroupDB,
     RewriteDatabase,
     RewriteDatabaseQuery,
     SequenceDB,
     TopoDB,
 )
 from pytensor.tensor.elemwise import DimShuffle, Elemwise
 from pytensor.tensor.extra_ops import BroadcastTo
 from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
 from pytensor.tensor.rewriting.basic import register_canonicalize
 from pytensor.tensor.rewriting.shape import ShapeFeature
+from pytensor.tensor.rewriting.uncanonicalize import local_max_and_argmax
 from pytensor.tensor.subtensor import (
     AdvancedIncSubtensor,
     AdvancedIncSubtensor1,
     AdvancedSubtensor,
     AdvancedSubtensor1,
     IncSubtensor,
     Subtensor,
@@ -354,14 +356,15 @@
     # Return the `RandomVariable` being indexed
     return [base_rv_var]
 
 
 logprob_rewrites_db = SequenceDB()
 logprob_rewrites_db.name = "logprob_rewrites_db"
 logprob_rewrites_db.register("pre-canonicalize", optdb.query("+canonicalize"), "basic")
+logprob_rewrites_db.register("local_max_and_argmax", out2in(local_max_and_argmax), "basic")
 
 # These rewrites convert un-measurable variables into their measurable forms,
 # but they need to be reapplied, because some of the measurable forms require
 # their inputs to be measurable.
 measurable_ir_rewrites_db = MeasurableEquilibriumDB()
 measurable_ir_rewrites_db.name = "measurable_ir_rewrites_db"
```

### Comparing `pymc-5.6.1/pymc/logprob/scan.py` & `pymc-5.7.0/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/tensor.py` & `pymc-5.7.0/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/transforms.py` & `pymc-5.7.0/pymc/logprob/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/logprob/utils.py` & `pymc-5.7.0/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/math.py` & `pymc-5.7.0/pymc/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,21 +71,22 @@
     sum,
     switch,
     tan,
     tanh,
     where,
     zeros_like,
 )
+from pytensor.tensor.special import log_softmax, softmax
 
 try:
     from pytensor.tensor.basic import extract_diag
 except ImportError:
     from pytensor.tensor.nlinalg import extract_diag
 
-from pytensor.tensor.nlinalg import det, matrix_dot, matrix_inverse, trace
+from pytensor.tensor.nlinalg import matrix_inverse
 from scipy.linalg import block_diag as scipy_block_diag
 
 from pymc.pytensorf import floatX, ix_, largest_common_dtype
 
 # pylint: enable=unused-import
 
 __all__ = [
@@ -263,39 +264,15 @@
 
 
 def logdiffexp_numpy(a, b):
     """log(exp(a) - exp(b))"""
     return a + log1mexp_numpy(b - a, negative_input=True)
 
 
-def invlogit(x, eps=None):
-    """The inverse of the logit function, 1 / (1 + exp(-x))."""
-    if eps is not None:
-        warnings.warn(
-            "pymc.math.invlogit no longer supports the ``eps`` argument and it will be ignored.",
-            FutureWarning,
-            stacklevel=2,
-        )
-    return pt.sigmoid(x)
-
-
-def softmax(x, axis=None):
-    # Ignore vector case UserWarning issued by PyTensor. This can be removed once PyTensor
-    # drops that warning
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", UserWarning)
-        return pt.special.softmax(x, axis=axis)
-
-
-def log_softmax(x, axis=None):
-    # Ignore vector case UserWarning issued by PyTensor. This can be removed once PyTensor
-    # drops that warning
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", UserWarning)
-        return pt.special.log_softmax(x, axis=axis)
+invlogit = sigmoid
 
 
 def logbern(log_p):
     if np.isnan(log_p):
         raise FloatingPointError("log_p can't be nan.")
     return np.log(np.random.uniform()) < log_p
```

### Comparing `pymc-5.6.1/pymc/model.py` & `pymc-5.7.0/pymc/model.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/model_graph.py` & `pymc-5.7.0/pymc/model_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pytensor import function
 from pytensor.compile.sharedvalue import SharedVariable
 from pytensor.graph import Apply
 from pytensor.graph.basic import ancestors, walk
 from pytensor.scalar.basic import Cast
 from pytensor.tensor.elemwise import Elemwise
 from pytensor.tensor.random.op import RandomVariable
+from pytensor.tensor.shape import Shape
 from pytensor.tensor.var import TensorConstant, TensorVariable
 
 import pymc as pm
 
 from pymc.util import get_default_varnames, get_var_name
 
 VarName = NewType("VarName", str)
@@ -51,14 +52,17 @@
 
     def get_parent_names(self, var: TensorVariable) -> Set[VarName]:
         if var.owner is None or var.owner.inputs is None:
             return set()
 
         def _filter_non_parameter_inputs(var):
             node = var.owner
+            if isinstance(node.op, Shape):
+                # Don't show shape-related dependencies
+                return []
             if isinstance(node.op, RandomVariable):
                 # Filter out rng, dtype and size parameters or RandomVariable nodes
                 return node.inputs[3:]
             else:
                 # Otherwise return all inputs
                 return node.inputs
```

### Comparing `pymc-5.6.1/pymc/ode/__init__.py` & `pymc-5.7.0/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/ode/ode.py` & `pymc-5.7.0/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/ode/utils.py` & `pymc-5.7.0/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/plots/__init__.py` & `pymc-5.7.0/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/printing.py` & `pymc-5.7.0/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/pytensorf.py` & `pymc-5.7.0/pymc/pytensorf.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     "jacobian",
     "CallableTensor",
     "join_nonshared_inputs",
     "make_shared_replacements",
     "generator",
     "convert_observed_data",
     "compile_pymc",
-    "constant_fold",
 ]
 
 
 def convert_observed_data(data):
     """Convert user provided dataset to accepted formats."""
 
     if hasattr(data, "to_numpy") and hasattr(data, "isnull"):
```

### Comparing `pymc-5.6.1/pymc/sampling/__init__.py` & `pymc-5.7.0/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/sampling/forward.py` & `pymc-5.7.0/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/sampling/jax.py` & `pymc-5.7.0/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/sampling/mcmc.py` & `pymc-5.7.0/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/sampling/parallel.py` & `pymc-5.7.0/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/sampling/population.py` & `pymc-5.7.0/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/sampling_jax.py` & `pymc-5.7.0/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/smc/__init__.py` & `pymc-5.7.0/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/smc/kernels.py` & `pymc-5.7.0/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/smc/sampling.py` & `pymc-5.7.0/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/stats/__init__.py` & `pymc-5.7.0/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/stats/convergence.py` & `pymc-5.7.0/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/stats/log_likelihood.py` & `pymc-5.7.0/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/__init__.py` & `pymc-5.7.0/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/arraystep.py` & `pymc-5.7.0/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/compound.py` & `pymc-5.7.0/pymc/step_methods/compound.py`

 * *Files 6% similar despite different names*

```diff
@@ -258,14 +258,24 @@
     if not isinstance(step, CompoundStep):
         raise ValueError(f"Unexpected type of step method: {step}")
     for sm in step.methods:
         steps += flatten_steps(sm)
     return steps
 
 
+def check_step_emits_tune(step: Union[CompoundStep, BlockedStep]):
+    if isinstance(step, BlockedStep) and "tune" not in step.stats_dtypes_shapes:
+        raise TypeError(f"{type(step)} does not emit the required 'tune' stat.")
+    elif isinstance(step, CompoundStep):
+        for sstep in step.methods:
+            if "tune" not in sstep.stats_dtypes_shapes:
+                raise TypeError(f"{type(sstep)} does not emit the required 'tune' stat.")
+    return
+
+
 class StatsBijection:
     """Map between a `list` of stats to `dict` of stats."""
 
     def __init__(self, sampler_stats_dtypes: Sequence[Mapping[str, type]]) -> None:
         # Keep a list of flat vs. original stat names
         stat_groups = []
         for s, names_dtypes in enumerate(sampler_stats_dtypes):
```

### Comparing `pymc-5.6.1/pymc/step_methods/hmc/__init__.py` & `pymc-5.7.0/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.7.0/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/hmc/hmc.py` & `pymc-5.7.0/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/hmc/integration.py` & `pymc-5.7.0/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/hmc/nuts.py` & `pymc-5.7.0/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.7.0/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/metropolis.py` & `pymc-5.7.0/pymc/step_methods/metropolis.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,17 +454,24 @@
     model: PyMC Model
         Optional model for sampling step. Defaults to None (taken from context).
 
     """
 
     name = "binary_gibbs_metropolis"
 
+    stats_dtypes_shapes = {
+        "tune": (bool, []),
+    }
+
     def __init__(self, vars, order="random", transit_p=0.8, model=None):
         model = pm.modelcontext(model)
 
+        # Doesn't actually tune, but it's required to emit a sampler stat
+        # that indicates whether a draw was done in a tuning phase.
+        self.tune = True
         # transition probabilities
         self.transit_p = transit_p
 
         vars = get_value_vars_from_user_vars(vars, model)
 
         initial_point = model.initial_point()
         self.dim = sum(initial_point[v.name].size for v in vars)
@@ -479,14 +486,19 @@
             self.order = order
 
         if not all([v.dtype in pm.discrete_types for v in vars]):
             raise ValueError("All variables must be binary for BinaryGibbsMetropolis")
 
         super().__init__(vars, [model.compile_logp()])
 
+    def reset_tuning(self):
+        # There are no tuning parameters in this step method.
+        self.tune = False
+        return
+
     def astep(self, apoint: RaveledVars, *args) -> Tuple[RaveledVars, StatsType]:
         logp: Callable[[RaveledVars], np.ndarray] = args[0]
         order = self.order
         if self.shuffle_dims:
             nr.shuffle(order)
 
         q = RaveledVars(np.copy(apoint.data), apoint.point_map_info)
@@ -499,15 +511,18 @@
             if nr.rand() < self.transit_p:
                 curr_val, q.data[idx] = q.data[idx], True - q.data[idx]
                 logp_prop = logp(q)
                 q.data[idx], accepted = metrop_select(logp_prop - logp_curr, q.data[idx], curr_val)
                 if accepted:
                     logp_curr = logp_prop
 
-        return q, []
+        stats = {
+            "tune": self.tune,
+        }
+        return q, [stats]
 
     @staticmethod
     def competence(var):
         """
         BinaryMetropolis is only suitable for Bernoulli
         and Categorical variables with k=2.
         """
@@ -539,14 +554,18 @@
     two types of proposals: A uniform proposal and a proportional proposal,
     which was introduced by Liu in his 1996 technical report
     "Metropolized Gibbs Sampler: An Improvement".
     """
 
     name = "categorical_gibbs_metropolis"
 
+    stats_dtypes_shapes = {
+        "tune": (bool, []),
+    }
+
     def __init__(self, vars, proposal="uniform", order="random", model=None):
         model = pm.modelcontext(model)
 
         vars = get_value_vars_from_user_vars(vars, model)
 
         initial_point = model.initial_point()
 
@@ -589,16 +608,25 @@
             self.astep = self.astep_unif
         elif proposal == "proportional":
             # Use the optimized "Metropolized Gibbs Sampler" described in Liu96.
             self.astep = self.astep_prop
         else:
             raise ValueError("Argument 'proposal' should either be 'uniform' or 'proportional'")
 
+        # Doesn't actually tune, but it's required to emit a sampler stat
+        # that indicates whether a draw was done in a tuning phase.
+        self.tune = True
+
         super().__init__(vars, [model.compile_logp()])
 
+    def reset_tuning(self):
+        # There are no tuning parameters in this step method.
+        self.tune = False
+        return
+
     def astep_unif(self, apoint: RaveledVars, *args) -> Tuple[RaveledVars, StatsType]:
         logp = args[0]
         point_map_info = apoint.point_map_info
         q0 = apoint.data
 
         dimcats = self.dimcats
         if self.shuffle_dims:
@@ -610,15 +638,18 @@
         for dim, k in dimcats:
             curr_val, q.data[dim] = q.data[dim], sample_except(k, q.data[dim])
             logp_prop = logp(q)
             q.data[dim], accepted = metrop_select(logp_prop - logp_curr, q.data[dim], curr_val)
             if accepted:
                 logp_curr = logp_prop
 
-        return q, []
+        stats = {
+            "tune": self.tune,
+        }
+        return q, [stats]
 
     def astep_prop(self, apoint: RaveledVars, *args) -> Tuple[RaveledVars, StatsType]:
         logp = args[0]
         point_map_info = apoint.point_map_info
         q0 = apoint.data
 
         dimcats = self.dimcats
```

### Comparing `pymc-5.6.1/pymc/step_methods/slicer.py` & `pymc-5.7.0/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/step_methods/step_sizes.py` & `pymc-5.7.0/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/testing.py` & `pymc-5.7.0/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/tuning/__init__.py` & `pymc-5.7.0/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/tuning/scaling.py` & `pymc-5.7.0/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/tuning/starting.py` & `pymc-5.7.0/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/util.py` & `pymc-5.7.0/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/__init__.py` & `pymc-5.7.0/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/approximations.py` & `pymc-5.7.0/pymc/variational/approximations.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import numpy as np
 import pytensor
 
 from arviz import InferenceData
 from pytensor import tensor as pt
 from pytensor.graph.basic import Variable
+from pytensor.graph.replace import graph_replace
 from pytensor.tensor.var import TensorVariable
 
 import pymc as pm
 
 from pymc.blocking import DictToArrayBijection
 from pymc.distributions.dist_math import rho2sigma
 from pymc.util import makeiter
@@ -386,13 +387,13 @@
         Returns
         -------
         evaluated node(s) over the posterior trace contained in the empirical approximation
         """
         node = self.to_flat_input(node)
 
         def sample(post, *_):
-            return pytensor.clone_replace(node, {self.input: post})
+            return graph_replace(node, {self.input: post}, strict=False)
 
         nodes, _ = pytensor.scan(
             sample, self.histogram, non_sequences=_known_scan_ignored_inputs(makeiter(node))
         )
         return nodes
```

### Comparing `pymc-5.6.1/pymc/variational/callbacks.py` & `pymc-5.7.0/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/inference.py` & `pymc-5.7.0/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/minibatch_rv.py` & `pymc-5.7.0/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/operators.py` & `pymc-5.7.0/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/opvi.py` & `pymc-5.7.0/pymc/variational/opvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 import numpy as np
 import pytensor
 import pytensor.tensor as pt
 import xarray
 
 from pytensor.graph.basic import Variable
+from pytensor.graph.replace import graph_replace
+from pytensor.tensor.shape import unbroadcast
 
 import pymc as pm
 
 from pymc.backends.base import MultiTrace
 from pymc.backends.ndarray import NDArray
 from pymc.blocking import DictToArrayBijection
 from pymc.initial_point import make_initial_point_fn
@@ -998,51 +1000,51 @@
 
         Returns
         -------
         :class:`Variable` with applied replacements, ready to use
         """
 
         flat2rand = self.make_size_and_deterministic_replacements(s, d, more_replacements)
-        node_out = pytensor.clone_replace(node, flat2rand)
+        node_out = graph_replace(node, flat2rand, strict=False)
         assert not (
             set(makeiter(self.input)) & set(pytensor.graph.graph_inputs(makeiter(node_out)))
         )
         try_to_set_test_value(node, node_out, s)
         assert self.symbolic_random not in set(pytensor.graph.graph_inputs(makeiter(node_out)))
         return node_out
 
     def to_flat_input(self, node):
         """*Dev* - replace vars with flattened view stored in `self.inputs`"""
-        return pytensor.clone_replace(node, self.replacements)
+        return graph_replace(node, self.replacements, strict=False)
 
     def symbolic_sample_over_posterior(self, node):
         """*Dev* - performs sampling of node applying independent samples from posterior each time.
         Note that it is done symbolically and this node needs :func:`set_size_and_deterministic` call
         """
         node = self.to_flat_input(node)
         random = self.symbolic_random.astype(self.symbolic_initial.dtype)
         random = pt.specify_shape(random, self.symbolic_initial.type.shape)
 
         def sample(post, *_):
-            return pytensor.clone_replace(node, {self.input: post})
+            return graph_replace(node, {self.input: post}, strict=False)
 
         nodes, _ = pytensor.scan(
             sample, random, non_sequences=_known_scan_ignored_inputs(makeiter(random))
         )
         assert self.input not in set(pytensor.graph.graph_inputs(makeiter(nodes)))
         return nodes
 
     def symbolic_single_sample(self, node):
         """*Dev* - performs sampling of node applying single sample from posterior.
         Note that it is done symbolically and this node needs
         :func:`set_size_and_deterministic` call with `size=1`
         """
         node = self.to_flat_input(node)
         random = self.symbolic_random.astype(self.symbolic_initial.dtype)
-        return pytensor.clone_replace(node, {self.input: random[0]})
+        return graph_replace(node, {self.input: random[0]}, strict=False)
 
     def make_size_and_deterministic_replacements(self, s, d, more_replacements=None):
         """*Dev* - creates correct replacements for initial depending on
         sample size and deterministic flag
 
         Parameters
         ----------
@@ -1055,16 +1057,23 @@
 
         Returns
         -------
         dict with replacements for initial
         """
         initial = self._new_initial(s, d, more_replacements)
         initial = pt.specify_shape(initial, self.symbolic_initial.type.shape)
+        # The static shape of initial may be more precise than self.symbolic_initial,
+        # and reveal previously unknown broadcastable dimensions. We have to mask those again.
+        if initial.type.broadcastable != self.symbolic_initial.type.broadcastable:
+            unbroadcast_axes = (
+                i for i, b in enumerate(self.symbolic_initial.type.broadcastable) if not b
+            )
+            initial = unbroadcast(initial, *unbroadcast_axes)
         if more_replacements:
-            initial = pytensor.clone_replace(initial, more_replacements)
+            initial = graph_replace(initial, more_replacements, strict=False)
         return {self.symbolic_initial: initial}
 
     @node_property
     def symbolic_normalizing_constant(self):
         """*Dev* - normalizing constant for `self.logq`, scales it to `minibatch_size` instead of `total_size`"""
         t = self.to_flat_input(
             pt.max(
@@ -1390,34 +1399,34 @@
         Returns
         -------
         :class:`Variable` with applied replacements, ready to use
         """
         _node = node
         optimizations = self.get_optimization_replacements(s, d)
         flat2rand = self.make_size_and_deterministic_replacements(s, d, more_replacements)
-        node = pytensor.clone_replace(node, optimizations)
-        node = pytensor.clone_replace(node, flat2rand)
+        node = graph_replace(node, optimizations, strict=False)
+        node = graph_replace(node, flat2rand, strict=False)
         assert not (set(self.symbolic_randoms) & set(pytensor.graph.graph_inputs(makeiter(node))))
         try_to_set_test_value(_node, node, s)
         return node
 
     def to_flat_input(self, node, more_replacements=None):
         """*Dev* - replace vars with flattened view stored in `self.inputs`"""
         more_replacements = more_replacements or {}
-        node = pytensor.clone_replace(node, more_replacements)
-        return pytensor.clone_replace(node, self.replacements)
+        node = graph_replace(node, more_replacements, strict=False)
+        return graph_replace(node, self.replacements, strict=False)
 
     def symbolic_sample_over_posterior(self, node, more_replacements=None):
         """*Dev* - performs sampling of node applying independent samples from posterior each time.
         Note that it is done symbolically and this node needs :func:`set_size_and_deterministic` call
         """
         node = self.to_flat_input(node)
 
         def sample(*post):
-            return pytensor.clone_replace(node, dict(zip(self.inputs, post)))
+            return graph_replace(node, dict(zip(self.inputs, post)), strict=False)
 
         nodes, _ = pytensor.scan(
             sample, self.symbolic_randoms, non_sequences=_known_scan_ignored_inputs(makeiter(node))
         )
         assert not (set(self.inputs) & set(pytensor.graph.graph_inputs(makeiter(nodes))))
         return nodes
 
@@ -1425,15 +1434,15 @@
         """*Dev* - performs sampling of node applying single sample from posterior.
         Note that it is done symbolically and this node needs
         :func:`set_size_and_deterministic` call with `size=1`
         """
         node = self.to_flat_input(node, more_replacements=more_replacements)
         post = [v[0] for v in self.symbolic_randoms]
         inp = self.inputs
-        return pytensor.clone_replace(node, dict(zip(inp, post)))
+        return graph_replace(node, dict(zip(inp, post)), strict=False)
 
     def get_optimization_replacements(self, s, d):
         """*Dev* - optimizations for logP. If sample size is static and equal to 1:
         then `pytensor.scan` MC estimate is replaced with single sample without call to `pytensor.scan`.
         """
         repl = collections.OrderedDict()
         # avoid scan if size is constant and equal to one
@@ -1459,15 +1468,15 @@
 
         Returns
         -------
         sampled node(s) with replacements
         """
         node_in = node
         if more_replacements:
-            node = pytensor.clone_replace(node, more_replacements)
+            node = graph_replace(node, more_replacements, strict=False)
         if not isinstance(node, (list, tuple)):
             node = [node]
         node = self.model.replace_rvs_by_values(node)
         if not isinstance(node_in, (list, tuple)):
             node = node[0]
         if size is None:
             node_out = self.symbolic_single_sample(node)
```

### Comparing `pymc-5.6.1/pymc/variational/stein.py` & `pymc-5.7.0/pymc/variational/stein.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-import pytensor
 import pytensor.tensor as pt
 
+from pytensor.graph.replace import graph_replace
+
 from pymc.pytensorf import floatX
 from pymc.util import WithMemoization, locally_cachedmethod
 from pymc.variational.opvi import node_property
 from pymc.variational.test_functions import rbf
 
 __all__ = ["Stein"]
 
@@ -81,16 +82,17 @@
     def dxkxy(self):
         return self._kernel()[1]
 
     @node_property
     def logp_norm(self):
         sized_symbolic_logp = self.approx.sized_symbolic_logp
         if self.use_histogram:
-            sized_symbolic_logp = pytensor.clone_replace(
+            sized_symbolic_logp = graph_replace(
                 sized_symbolic_logp,
                 dict(zip(self.approx.symbolic_randoms, self.approx.collect("histogram"))),
+                strict=False,
             )
         return sized_symbolic_logp / self.approx.symbolic_normalizing_constant
 
     @locally_cachedmethod
     def _kernel(self):
         return self._kernel_f(self.input_joint_matrix)
```

### Comparing `pymc-5.6.1/pymc/variational/test_functions.py` & `pymc-5.7.0/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/variational/updates.py` & `pymc-5.7.0/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc/vartypes.py` & `pymc-5.7.0/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/pymc.egg-info/PKG-INFO` & `pymc-5.7.0/pymc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.6.1
+Version: 5.7.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
@@ -182,18 +182,17 @@
         .. |ODSC| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/odsc/sponsor_odsc.png?raw=true
            :target: https://odsc.com/california/?utm_source=pymc&utm_medium=referral
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `pymc-5.6.1/pymc.egg-info/SOURCES.txt` & `pymc-5.7.0/pymc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 pymc/logprob/abstract.py
 pymc/logprob/basic.py
 pymc/logprob/binary.py
 pymc/logprob/censoring.py
 pymc/logprob/checks.py
 pymc/logprob/cumsum.py
 pymc/logprob/mixture.py
+pymc/logprob/order.py
 pymc/logprob/rewriting.py
 pymc/logprob/scan.py
 pymc/logprob/tensor.py
 pymc/logprob/transforms.py
 pymc/logprob/utils.py
 pymc/ode/__init__.py
 pymc/ode/ode.py
```

### Comparing `pymc-5.6.1/scripts/docker_container.sh` & `pymc-5.7.0/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.6.1/setup.py` & `pymc-5.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 URL = "http://github.com/pymc-devs/pymc"
 LICENSE = "Apache License, Version 2.0"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
@@ -67,11 +66,11 @@
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/x-rst",
         packages=find_packages(exclude=["tests*"]),
         # because of an upload-size limit by PyPI, we're temporarily removing docs from the tarball.
         # Also see MANIFEST.in
         # package_data={'docs': ['*']},
         classifiers=classifiers,
-        python_requires=">=3.8",
+        python_requires=">=3.9",
         install_requires=install_reqs,
         tests_require=test_reqs,
     )
```

### Comparing `pymc-5.6.1/versioneer.py` & `pymc-5.7.0/versioneer.py`

 * *Files identical despite different names*

