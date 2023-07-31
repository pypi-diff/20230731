# Comparing `tmp/lqg-0.2.1.tar.gz` & `tmp/lqg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqg-0.2.1.tar", max compression
+gzip compressed data, was "lqg-0.2.2.tar", max compression
```

## Comparing `lqg-0.2.1.tar` & `lqg-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-27 11:26:54.134688 lqg-0.2.1/LICENSE
--rw-r--r--   0        0        0     2675 2023-07-26 10:09:43.575186 lqg-0.2.1/README.md
--rw-r--r--   0        0        0      127 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/belief/__init__.py
--rw-r--r--   0        0        0      426 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/belief/kf.py
--rw-r--r--   0        0        0     2028 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/ccg.py
--rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/control/__init__.py
--rw-r--r--   0        0        0     1243 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/control/glqr.py
--rw-r--r--   0        0        0     1078 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/control/lqr.py
--rw-r--r--   0        0        0     7298 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/glqg.py
--rw-r--r--   0        0        0      121 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/infer/__init__.py
--rw-r--r--   0        0        0     1758 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/infer/map.py
--rw-r--r--   0        0        0     1732 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/infer/mle.py
--rw-r--r--   0        0        0     2058 2023-07-27 12:53:29.114840 lqg-0.2.1/lqg/infer/models.py
--rw-r--r--   0        0        0     1764 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/infer/prior.py
--rw-r--r--   0        0        0     1908 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/infer/utils.py
--rw-r--r--   0        0        0     3014 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/io.py
--rw-r--r--   0        0        0     7846 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/lqg.py
--rw-r--r--   0        0        0     7607 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/optim.py
--rw-r--r--   0        0        0     1904 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/spec.py
--rw-r--r--   0        0        0      178 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/tracking/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/basic.py
--rw-r--r--   0        0        0     2094 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/delay.py
--rw-r--r--   0        0        0     2824 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/signal_dependent.py
--rw-r--r--   0        0        0     1068 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/subjective.py
--rw-r--r--   0        0        0     1724 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/utils.py
--rw-r--r--   0        0        0      554 2023-07-27 12:56:25.271663 lqg-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 lqg-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-27 11:26:54.134688 lqg-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2675 2023-07-26 10:09:43.575186 lqg-0.2.2/README.md
+-rw-r--r--   0        0        0      127 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/belief/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/belief/kf.py
+-rw-r--r--   0        0        0     2028 2023-04-27 11:26:54.148021 lqg-0.2.2/lqg/ccg.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/control/__init__.py
+-rw-r--r--   0        0        0     1243 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/control/glqr.py
+-rw-r--r--   0        0        0     1078 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/control/lqr.py
+-rw-r--r--   0        0        0     7341 2023-07-31 16:01:05.596082 lqg-0.2.2/lqg/glqg.py
+-rw-r--r--   0        0        0      121 2023-04-27 11:26:54.148021 lqg-0.2.2/lqg/infer/__init__.py
+-rw-r--r--   0        0        0     1758 2023-04-27 11:26:54.148021 lqg-0.2.2/lqg/infer/map.py
+-rw-r--r--   0        0        0     1732 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/infer/mle.py
+-rw-r--r--   0        0        0     2058 2023-07-27 14:45:56.521524 lqg-0.2.2/lqg/infer/models.py
+-rw-r--r--   0        0        0     1764 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/infer/prior.py
+-rw-r--r--   0        0        0     1908 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/infer/utils.py
+-rw-r--r--   0        0        0     3014 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/io.py
+-rw-r--r--   0        0        0     7997 2023-07-31 16:01:05.596082 lqg-0.2.2/lqg/lqg.py
+-rw-r--r--   0        0        0     7607 2023-04-27 11:26:54.148021 lqg-0.2.2/lqg/optim.py
+-rw-r--r--   0        0        0     1904 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/spec.py
+-rw-r--r--   0        0        0      178 2023-07-25 14:39:35.745375 lqg-0.2.2/lqg/tracking/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-25 14:39:35.748708 lqg-0.2.2/lqg/tracking/basic.py
+-rw-r--r--   0        0        0     2094 2023-07-25 14:39:35.748708 lqg-0.2.2/lqg/tracking/delay.py
+-rw-r--r--   0        0        0     2824 2023-07-25 14:39:35.748708 lqg-0.2.2/lqg/tracking/signal_dependent.py
+-rw-r--r--   0        0        0     1068 2023-07-25 14:39:35.748708 lqg-0.2.2/lqg/tracking/subjective.py
+-rw-r--r--   0        0        0     1724 2023-07-25 14:39:35.748708 lqg-0.2.2/lqg/utils.py
+-rw-r--r--   0        0        0      554 2023-07-31 16:08:41.373670 lqg-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 lqg-0.2.2/PKG-INFO
```

### Comparing `lqg-0.2.1/LICENSE` & `lqg-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/README.md` & `lqg-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/ccg.py` & `lqg-0.2.2/lqg/ccg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/control/glqr.py` & `lqg-0.2.2/lqg/control/glqr.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/control/lqr.py` & `lqg-0.2.2/lqg/control/lqr.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/glqg.py` & `lqg-0.2.2/lqg/glqg.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         x, x_hat, y, u = vmap(lambda key: simulate_trial(key, x0=x0, xhat0=xhat0))(random.split(rng_key, num=n))
 
         if return_all:
             return x, x_hat, y, u
         else:
             return x
 
-    def conditional_moments(self, x):
+    def conditional_moments(self, x, Sigma0=None):
         """ Conditional distribution p(x | theta)
 
         Args:
             self: LQG
             x: time series of shape T (time steps), n (trials), d (dimensionality)
 
         Returns:
@@ -101,15 +101,15 @@
         """
         T, obs_dim = x.shape
         xdim = self.dynamics.A.shape[1]
         bdim = self.actor.A.shape[1]
 
         # compute control and estimator gains
         gains = glqr.backward(self.actor)
-        K = kf.forward(self.actor, Sigma0=self.actor.V[0] @ self.actor.V[0].T)
+        K = kf.forward(self.actor, Sigma0=self.actor.V[0] @ self.actor.V[0].T if Sigma0 is None else Sigma0)
 
         # initialize p(x_t, xhat_t | x_{1:t-1})
         # TODO: initialization should not always be zero for the unobserved dims
         mu = jnp.hstack([x[0], jnp.zeros(xdim - obs_dim + bdim)])
         # TODO: is there a smarter way to initialize Sigma?
         #  For example, with zeros in the covariances, we get problems
         Sigma = jnp.eye(xdim * 2) * 1e-1
```

### Comparing `lqg-0.2.1/lqg/infer/map.py` & `lqg-0.2.2/lqg/infer/map.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/infer/mle.py` & `lqg-0.2.2/lqg/infer/mle.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/infer/models.py` & `lqg-0.2.2/lqg/infer/models.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/infer/prior.py` & `lqg-0.2.2/lqg/infer/prior.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/infer/utils.py` & `lqg-0.2.2/lqg/infer/utils.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/io.py` & `lqg-0.2.2/lqg/io.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/lqg.py` & `lqg-0.2.2/lqg/lqg.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         x, x_hat, y, u = vmap(lambda key: simulate_trial(key, x0=x0, xhat0=xhat0))(random.split(rng_key, num=n))
 
         if return_all:
             return x, x_hat, y, u
         else:
             return x
 
-    def conditional_moments(self, x):
+    def conditional_moments(self, x, Sigma0=None):
         """ Conditional distribution p(x | theta)
 
         Args:
             self: LQG
             x: time series of shape T (time steps), n (trials), d (dimensionality)
 
         Returns:
@@ -146,15 +146,15 @@
         """
         T, obs_dim = x.shape
         xdim = self.dynamics.A.shape[1]
         bdim = self.actor.A.shape[1]
 
         # compute control and estimator gains
         gains = lqr.backward(self.actor)
-        K = kf.forward(self.actor, Sigma0=self.actor.V[0] @ self.actor.V[0].T)
+        K = kf.forward(self.actor, Sigma0=self.actor.V[0] @ self.actor.V[0].T if Sigma0 is None else Sigma0)
 
         # set up joint dynamical system for state and belief
         # p(x_t, xhat_t | x_{t-1}, xhat_{t-1})
 
         # joint dynamics
         F = jnp.concatenate([
             jnp.concatenate([self.dynamics.A,
@@ -187,32 +187,32 @@
                                                                                             (Sigma @ F.T)[:obs_dim, :])
             return (mu, Sigma), (mu, Sigma)
 
         _, (mu, Sigma) = scan(scan_fn, (mu0, Sigma0), (F, G, x[:-1]))
         # return jnp.vstack((mu0, mu)), jnp.vstack((Sigma0[jnp.newaxis], Sigma))
         return mu, Sigma
 
-    def conditional_distribution(self, x):
+    def conditional_distribution(self, x, Sigma0=None):
         n, T, d = x.shape
 
         # compute p(x_{t+1}, xhat_{t+1} | x_{1:t})
-        mu, Sigma = vmap(self.conditional_moments)(x)
+        mu, Sigma = vmap(self.conditional_moments, in_axes=(0, None))(x, Sigma0)
 
         # marginalize out xhat by using only those entries of mu and Sigma that correspond to x
         return dist.MultivariateNormal(mu[:, :, :d], Sigma[:, :, :d, :d])
 
-    def log_likelihood(self, x):
+    def log_likelihood(self, x, Sigma0=None):
         # log likelihood of the states at time t+1 given all previous states up to time t
-        return self.conditional_distribution(x[:, :-1]).log_prob(x[:, 1:])
+        return self.conditional_distribution(x[:, :-1], Sigma0=Sigma0).log_prob(x[:, 1:])
 
-    def belief_tracking_distribution(self, x):
+    def belief_tracking_distribution(self, x, Sigma0=None):
         d = self.xdim
 
         # compute p(x_{t+1}, xhat_{t+1} | x_{1:t})
-        mu, Sigma = vmap(self.conditional_moments)(x)
+        mu, Sigma = vmap(self.conditional_moments, in_axes=(0, None))(x, Sigma0)
 
         # return those elements of mu and Sigma that correspond to xhat
         return dist.MultivariateNormal(mu[:, :, d:], Sigma[:, :, d:, d:])
 
 
 def Dynamics(A, B, F, V, W, T=1000):
     xdim = A.shape[0]
```

### Comparing `lqg-0.2.1/lqg/optim.py` & `lqg-0.2.2/lqg/optim.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/spec.py` & `lqg-0.2.2/lqg/spec.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/tracking/basic.py` & `lqg-0.2.2/lqg/tracking/basic.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/tracking/delay.py` & `lqg-0.2.2/lqg/tracking/delay.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/tracking/signal_dependent.py` & `lqg-0.2.2/lqg/tracking/signal_dependent.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/tracking/subjective.py` & `lqg-0.2.2/lqg/tracking/subjective.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/lqg/utils.py` & `lqg-0.2.2/lqg/utils.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.1/pyproject.toml` & `lqg-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lqg"
-version = "0.2.1"
+version = "0.2.2"
 description = "(Inverse) optimal control for linear-quadratic Gaussian systems"
 authors = ["Dominik Straub <dominikstrb@mailbox.org>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `lqg-0.2.1/PKG-INFO` & `lqg-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.2.1
+Version: 0.2.2
 Summary: (Inverse) optimal control for linear-quadratic Gaussian systems
 License: AGPL-3.0-only
 Author: Dominik Straub
 Author-email: dominikstrb@mailbox.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

