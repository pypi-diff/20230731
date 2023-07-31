# Comparing `tmp/bettermdptools-0.3.0.tar.gz` & `tmp/bettermdptools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettermdptools-0.3.0.tar", last modified: Sun Jan 15 08:25:30 2023, max compression
+gzip compressed data, was "dist/bettermdptools-0.4.0.tar", last modified: Mon Jul 31 18:15:20 2023, max compression
```

## Comparing `bettermdptools-0.3.0.tar` & `bettermdptools-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-15 08:25:30.549943 bettermdptools-0.3.0/
--rw-rw-rw-   0        0        0      243 2023-01-15 08:25:30.549943 bettermdptools-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-15 08:25:30.463528 bettermdptools-0.3.0/algorithms/
--rw-rw-rw-   0        0        0        0 2022-12-28 08:26:56.000000 bettermdptools-0.3.0/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5800 2023-01-15 07:44:21.000000 bettermdptools-0.3.0/algorithms/planner.py
--rw-rw-rw-   0        0        0    12543 2023-01-15 07:36:22.000000 bettermdptools-0.3.0/algorithms/rl.py
-drwxrwxrwx   0        0        0        0 2023-01-15 08:25:30.486065 bettermdptools-0.3.0/bettermdptools.egg-info/
--rw-rw-rw-   0        0        0      243 2023-01-15 08:25:30.000000 bettermdptools-0.3.0/bettermdptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-01-15 08:25:30.000000 bettermdptools-0.3.0/bettermdptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-15 08:25:30.000000 bettermdptools-0.3.0/bettermdptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-01-15 08:25:30.000000 bettermdptools-0.3.0/bettermdptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-01-15 08:25:30.000000 bettermdptools-0.3.0/bettermdptools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-15 08:25:30.486065 bettermdptools-0.3.0/callbacks/
--rw-rw-rw-   0        0        0        0 2022-12-28 08:26:56.000000 bettermdptools-0.3.0/callbacks/__init__.py
--rw-rw-rw-   0        0        0      796 2022-08-13 18:12:17.000000 bettermdptools-0.3.0/callbacks/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-01-15 08:25:30.501795 bettermdptools-0.3.0/decorators/
--rw-rw-rw-   0        0        0        0 2022-12-28 08:26:56.000000 bettermdptools-0.3.0/decorators/__init__.py
--rw-rw-rw-   0        0        0     1225 2022-08-13 18:12:17.000000 bettermdptools-0.3.0/decorators/decorators.py
-drwxrwxrwx   0        0        0        0 2023-01-15 08:25:30.549943 bettermdptools-0.3.0/examples/
--rw-rw-rw-   0        0        0        0 2022-12-28 08:26:56.000000 bettermdptools-0.3.0/examples/__init__.py
--rw-rw-rw-   0        0        0     2721 2023-01-15 07:58:07.000000 bettermdptools-0.3.0/examples/blackjack.py
--rw-rw-rw-   0        0        0      683 2023-01-15 07:56:57.000000 bettermdptools-0.3.0/examples/frozen_lake.py
--rw-rw-rw-   0        0        0      733 2023-01-15 07:56:08.000000 bettermdptools-0.3.0/examples/grid_search.py
--rw-rw-rw-   0        0        0     3522 2023-01-15 08:07:17.000000 bettermdptools-0.3.0/examples/plots.py
--rw-rw-rw-   0        0        0      627 2023-01-15 07:57:27.000000 bettermdptools-0.3.0/examples/taxi.py
--rw-rw-rw-   0        0        0     3051 2022-12-26 09:44:59.000000 bettermdptools-0.3.0/examples/test_env.py
--rw-rw-rw-   0        0        0       42 2023-01-15 08:25:30.557461 bettermdptools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-01-15 08:24:01.000000 bettermdptools-0.3.0/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/
+-rw-rw-r--   0 john      (1000) john      (1000)      233 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/PKG-INFO
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/algorithms/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/algorithms/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5628 2023-07-31 17:46:46.000000 bettermdptools-0.4.0/algorithms/planner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12167 2023-07-31 17:46:46.000000 bettermdptools-0.4.0/algorithms/rl.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/bettermdptools.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)      233 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/bettermdptools.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      463 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/bettermdptools.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/bettermdptools.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       63 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/bettermdptools.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       26 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/bettermdptools.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/examples/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/examples/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2626 2023-07-31 17:53:11.000000 bettermdptools-0.4.0/examples/blackjack.py
+-rw-rw-r--   0 john      (1000) john      (1000)      657 2023-07-24 07:37:45.000000 bettermdptools-0.4.0/examples/frozen_lake.py
+-rw-rw-r--   0 john      (1000) john      (1000)      711 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/examples/grid_search.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3455 2023-07-25 17:19:07.000000 bettermdptools-0.4.0/examples/plots.py
+-rw-rw-r--   0 john      (1000) john      (1000)      601 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/examples/taxi.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2964 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/examples/test_env.py
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)      717 2023-07-31 18:13:07.000000 bettermdptools-0.4.0/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-31 18:15:20.000000 bettermdptools-0.4.0/utils/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/utils/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1435 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/utils/callbacks.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1187 2023-07-24 06:40:33.000000 bettermdptools-0.4.0/utils/decorators.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bettermdptools-0.3.0/algorithms/planner.py` & `bettermdptools-0.4.0/algorithms/planner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-"""
-Author: Miguel Morales
-BSD 3-Clause License
-
-Copyright (c) 2018, Miguel Morales
-All rights reserved.
-https://github.com/mimoralea/gdrl/blob/master/LICENSE
-"""
-
-"""
-modified by: John Mansfield
-
-documentation added by: Gagandeep Randhawa
-"""
-
-"""
-Model-based learning algorithms: Value Iteration and Policy Iteration
-
-Assumes prior knowledge of the type of reward available to the agent
-for iterating to an optimal policy and reward value for a given MDP.
-"""
-
-import numpy as np
-import warnings
-from decorators.decorators import print_runtime
-
-
-class Planner:
-    def __init__(self, P):
-        self.P = P
-
-    @print_runtime
-    def value_iteration(self, gamma=1.0, n_iters=1000, theta=1e-10):
-        """
-        PARAMETERS:
-
-        gamma {float}:
-            Discount factor
-
-        n_iters {int}:
-            Number of iterations
-
-        theta {float}:
-            Convergence criterion for value iteration.
-            State values are considered to be converged when the maximum difference between new and previous state values is less than theta.
-            Stops at n_iters or theta convergence - whichever comes first.
-
-
-        RETURNS:
-
-        V {numpy array}, shape(possible states):
-            State values array
-
-        V_track {numpy array}, shape(n_episodes, nS):
-            Log of V(s) for each iteration
-
-        pi {lambda}, input state value, output action value:
-            Policy which maps state action value
-        """
-        V = np.zeros(len(self.P), dtype=np.float64)
-        V_track = np.zeros((n_iters, len(self.P)), dtype=np.float64)
-        i = 0
-        converged = False
-        while i < n_iters-1 and not converged:
-            i += 1
-            Q = np.zeros((len(self.P), len(self.P[0])), dtype=np.float64)
-            for s in range(len(self.P)):
-                for a in range(len(self.P[s])):
-                    for prob, next_state, reward, done in self.P[s][a]:
-                        Q[s][a] += prob * (reward + gamma * V[next_state] * (not done))
-            if np.max(np.abs(V - np.max(Q, axis=1))) < theta:
-                converged = True
-            V = np.max(Q, axis=1)
-            V_track[i] = V
-        if not converged:
-            warnings.warn("Max iterations reached before convergence.  Check theta and n_iters.  ")
-        # Explanation of lambda:
-        # def pi(s):
-        #   policy = dict()
-        #   for state, action in enumerate(np.argmax(Q, axis=1)):
-        #       policy[state] = action
-        #   return policy[s]
-        pi = lambda s: {s:a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
-        return V, V_track, pi
-
-    @print_runtime
-    def policy_iteration(self, gamma=1.0, n_iters=50, theta=1e-10):
-        """
-        PARAMETERS:
-
-        gamma {float}:
-            Discount factor
-
-        n_iters {int}:
-            Number of iterations
-
-        theta {float}:
-            Convergence criterion for policy evaluation.
-            State values are considered to be converged when the maximum difference between new and previous state
-            values is less than theta.
-
-
-        RETURNS:
-
-        V {numpy array}, shape(possible states):
-            State values array
-
-        V_track {numpy array}, shape(n_episodes, nS):
-            Log of V(s) for each iteration
-
-        pi {lambda}, input state value, output action value:
-            Policy which maps state action value
-        """
-        random_actions = np.random.choice(tuple(self.P[0].keys()), len(self.P))
-        # Explanation of lambda:
-        # def pi(s):
-        #   policy = dict()
-        #   for state, action in enumerate(np.argmax(Q, axis=1)):
-        #       policy[state] = action
-        #   return policy[s]
-        pi = lambda s: {s: a for s, a in enumerate(random_actions)}[s]
-        # initial V to give to `policy_evaluation` for the first time
-        V = np.zeros(len(self.P), dtype=np.float64)
-        V_track = np.zeros((n_iters, len(self.P)), dtype=np.float64)
-        i = 0
-        converged = False
-        while i < n_iters and not converged:
-            i += 1
-            old_pi = {s: pi(s) for s in range(len(self.P))}
-            V = self.policy_evaluation(pi, V, gamma, theta)
-            V_track[i] = V
-            pi = self.policy_improvement(V, gamma)
-            if old_pi == {s: pi(s) for s in range(len(self.P))}:
-                converged = True
-        if not converged:
-            warnings.warn("Max iterations reached before convergence.  Check n_iters.")
-        return V, V_track, pi
-
-    def policy_evaluation(self, pi, prev_V, gamma=1.0, theta=1e-10):
-        while True:
-            V = np.zeros(len(self.P), dtype=np.float64)
-            for s in range(len(self.P)):
-                for prob, next_state, reward, done in self.P[s][pi(s)]:
-                    V[s] += prob * (reward + gamma * prev_V[next_state] * (not done))
-            if np.max(np.abs(prev_V - V)) < theta:
-                break
-            prev_V = V.copy()
-        return V
-
-    def policy_improvement(self, V, gamma=1.0):
-        Q = np.zeros((len(self.P), len(self.P[0])), dtype=np.float64)
-        for s in range(len(self.P)):
-            for a in range(len(self.P[s])):
-                for prob, next_state, reward, done in self.P[s][a]:
-                    Q[s][a] += prob * (reward + gamma * V[next_state] * (not done))
-        # Explanation of lambda:
-        # def new_pi(s):
-        #   policy = dict()
-        #   for state, action in enumerate(np.argmax(Q, axis=1)):
-        #       policy[state] = action
-        #   return policy[s]
-        new_pi = lambda s: {s: a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
-        return new_pi
+"""
+Author: Miguel Morales
+BSD 3-Clause License
+
+Copyright (c) 2018, Miguel Morales
+All rights reserved.
+https://github.com/mimoralea/gdrl/blob/master/LICENSE
+"""
+
+"""
+modified by: John Mansfield
+
+documentation added by: Gagandeep Randhawa
+"""
+
+"""
+Model-based learning algorithms: Value Iteration and Policy Iteration
+
+Assumes prior knowledge of the type of reward available to the agent
+for iterating to an optimal policy and reward value for a given MDP.
+"""
+
+import numpy as np
+import warnings
+from utils.decorators import print_runtime
+
+
+class Planner:
+    def __init__(self, P):
+        self.P = P
+
+    @print_runtime
+    def value_iteration(self, gamma=1.0, n_iters=1000, theta=1e-10):
+        """
+        PARAMETERS:
+
+        gamma {float}:
+            Discount factor
+
+        n_iters {int}:
+            Number of iterations
+
+        theta {float}:
+            Convergence criterion for value iteration.
+            State values are considered to be converged when the maximum difference between new and previous state values is less than theta.
+            Stops at n_iters or theta convergence - whichever comes first.
+
+
+        RETURNS:
+
+        V {numpy array}, shape(possible states):
+            State values array
+
+        V_track {numpy array}, shape(n_episodes, nS):
+            Log of V(s) for each iteration
+
+        pi {lambda}, input state value, output action value:
+            Policy mapping states to actions.
+        """
+        V = np.zeros(len(self.P), dtype=np.float64)
+        V_track = np.zeros((n_iters, len(self.P)), dtype=np.float64)
+        i = 0
+        converged = False
+        while i < n_iters-1 and not converged:
+            i += 1
+            Q = np.zeros((len(self.P), len(self.P[0])), dtype=np.float64)
+            for s in range(len(self.P)):
+                for a in range(len(self.P[s])):
+                    for prob, next_state, reward, done in self.P[s][a]:
+                        Q[s][a] += prob * (reward + gamma * V[next_state] * (not done))
+            if np.max(np.abs(V - np.max(Q, axis=1))) < theta:
+                converged = True
+            V = np.max(Q, axis=1)
+            V_track[i] = V
+        if not converged:
+            warnings.warn("Max iterations reached before convergence.  Check theta and n_iters.  ")
+        # Explanation of lambda:
+        # def pi(s):
+        #   policy = dict()
+        #   for state, action in enumerate(np.argmax(Q, axis=1)):
+        #       policy[state] = action
+        #   return policy[s]
+        pi = lambda s: {s:a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
+        return V, V_track, pi
+
+    @print_runtime
+    def policy_iteration(self, gamma=1.0, n_iters=50, theta=1e-10):
+        """
+        PARAMETERS:
+
+        gamma {float}:
+            Discount factor
+
+        n_iters {int}:
+            Number of iterations
+
+        theta {float}:
+            Convergence criterion for policy evaluation.
+            State values are considered to be converged when the maximum difference between new and previous state
+            values is less than theta.
+
+
+        RETURNS:
+
+        V {numpy array}, shape(possible states):
+            State values array
+
+        V_track {numpy array}, shape(n_episodes, nS):
+            Log of V(s) for each iteration
+
+        pi {lambda}, input state value, output action value:
+            Policy mapping states to actions.
+        """
+        random_actions = np.random.choice(tuple(self.P[0].keys()), len(self.P))
+        # Explanation of lambda:
+        # def pi(s):
+        #   policy = dict()
+        #   for state, action in enumerate(np.argmax(Q, axis=1)):
+        #       policy[state] = action
+        #   return policy[s]
+        pi = lambda s: {s: a for s, a in enumerate(random_actions)}[s]
+        # initial V to give to `policy_evaluation` for the first time
+        V = np.zeros(len(self.P), dtype=np.float64)
+        V_track = np.zeros((n_iters, len(self.P)), dtype=np.float64)
+        i = 0
+        converged = False
+        while i < n_iters-1 and not converged:
+            i += 1
+            old_pi = {s: pi(s) for s in range(len(self.P))}
+            V = self.policy_evaluation(pi, V, gamma, theta)
+            V_track[i] = V
+            pi = self.policy_improvement(V, gamma)
+            if old_pi == {s: pi(s) for s in range(len(self.P))}:
+                converged = True
+        if not converged:
+            warnings.warn("Max iterations reached before convergence.  Check n_iters.")
+        return V, V_track, pi
+
+    def policy_evaluation(self, pi, prev_V, gamma=1.0, theta=1e-10):
+        while True:
+            V = np.zeros(len(self.P), dtype=np.float64)
+            for s in range(len(self.P)):
+                for prob, next_state, reward, done in self.P[s][pi(s)]:
+                    V[s] += prob * (reward + gamma * prev_V[next_state] * (not done))
+            if np.max(np.abs(prev_V - V)) < theta:
+                break
+            prev_V = V.copy()
+        return V
+
+    def policy_improvement(self, V, gamma=1.0):
+        Q = np.zeros((len(self.P), len(self.P[0])), dtype=np.float64)
+        for s in range(len(self.P)):
+            for a in range(len(self.P[s])):
+                for prob, next_state, reward, done in self.P[s][a]:
+                    Q[s][a] += prob * (reward + gamma * V[next_state] * (not done))
+        # Explanation of lambda:
+        # def new_pi(s):
+        #   policy = dict()
+        #   for state, action in enumerate(np.argmax(Q, axis=1)):
+        #       policy[state] = action
+        #   return policy[s]
+        new_pi = lambda s: {s: a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
+        return new_pi
```

### Comparing `bettermdptools-0.3.0/algorithms/rl.py` & `bettermdptools-0.4.0/algorithms/rl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,332 +1,331 @@
-"""
-Author: Miguel Morales
-BSD 3-Clause License
-
-Copyright (c) 2018, Miguel Morales
-All rights reserved.
-https://github.com/mimoralea/gdrl/blob/master/LICENSE
-"""
-
-"""
-modified by: John Mansfield
-
-documentation added by: Gagandeep Randhawa
-"""
-
-"""
-Model-free learning algorithms: Q-Learning and SARSA
-
-Assumes no prior knowledge of the type of reward available to the agent.
-Given enough episodes, tries to find an estimate of the optimal policy.
-"""
-
-import numpy as np
-from tqdm import tqdm
-from callbacks.callbacks import MyCallbacks
-from decorators.decorators import print_runtime
-import gym
-import warnings
-
-
-class RL:
-    def __init__(self, env):
-        self.env = env
-        self.callbacks = MyCallbacks()
-        self.render = False
-
-    @staticmethod
-    def decay_schedule(init_value, min_value, decay_ratio, max_steps, log_start=-2, log_base=10):
-        """
-        Parameters
-        ----------------------------
-        init_value {float}:
-            Initial value of the quantity being decayed
-        
-        min_value {float}:
-            Minimum value init_value is allowed to decay to
-            
-        decay_ratio {float}:
-            The exponential factor exp(decay_ratio).
-            Updated decayed value is calculated as 
-        
-        max_steps {int}:
-            Max iteration steps for decaying init_value
-        
-        log_start {array-like}, default = -2:
-            Starting value of the decay sequence.
-            Default value starts it at 0.01
-        
-        log_base {array-like}, default = 10:
-            Base of the log space.
-        
-        
-        Returns
-        ----------------------------
-        values {array-like}, shape(max_steps):
-            Decay values where values[i] is the value used at i-th step
-        """
-        decay_steps = int(max_steps * decay_ratio)
-        rem_steps = max_steps - decay_steps
-        values = np.logspace(log_start, 0, decay_steps, base=log_base, endpoint=True)[::-1]
-        values = (values - values.min()) / (values.max() - values.min())
-        values = (init_value - min_value) * values + min_value
-        values = np.pad(values, (0, rem_steps), 'edge')
-        return values
-
-    @print_runtime
-    def q_learning(self,
-                   nS=None,
-                   nA=None,
-                   convert_state_obs=lambda state, done: state,
-                   gamma=.99,
-                   init_alpha=0.5,
-                   min_alpha=0.01,
-                   alpha_decay_ratio=0.5,
-                   init_epsilon=1.0,
-                   min_epsilon=0.1,
-                   epsilon_decay_ratio=0.9,
-                   n_episodes=10000):
-        """
-        Parameters
-        ----------------------------
-        nS {int}:
-            Number of states
-        
-        nA {int}:
-            Number of available actions
-            
-        convert_state_obs {lambda}:
-            The state conversion utilized in BlackJack ToyText problem.
-            Returns three state tuple as one of the 280 converted states.
-        
-        gamma {float}, default = 0.99:
-            Discount factor
-        
-        init_alpha {float}, default = 0.5:
-            Learning rate
-        
-        min_alpha {float}, default = 0.01:
-            Minimum learning rate
-        
-        alpha_decay_ratio {float}, default = 0.5:
-            Decay schedule of learing rate for future iterations
-        
-        init_epsilon {float}, default = 0.1:
-            Initial epsilon value for epsilon greedy strategy.
-            Chooses max(Q) over available actions with probability 1-epsilon.
-        
-        min_epsilon {float}, default = 0.1:
-            Minimum epsilon. Used to balance exploration in later stages.
-        
-        epsilon_decay_ratio {float}, default = 0.9:
-            Decay schedule of epsilon for future iterations
-            
-        n_episodes {int}, default = 10000:
-            Number of episodes for the agent
-
-
-        Returns
-        ----------------------------
-        Q {numpy array}, shape(nS, nA):
-            Final action-value function Q(s,a)
-
-        pi {lambda}, input state value, output action value:
-            Optimal policy which maps state action value
-
-        V {numpy array}, shape(nS):
-            Optimal value array
-
-        Q_track {numpy array}, shape(n_episodes, nS, nA):
-            Log of Q(s,a) for each episode
-
-        pi_track {list}, len(n_episodes):
-            Log of complete policy for each episode
-        """
-        if nS is None:
-            nS=self.env.observation_space.n
-        if nA is None:
-            nA=self.env.action_space.n
-        pi_track = []
-        Q = np.zeros((nS, nA), dtype=np.float64)
-        Q_track = np.zeros((n_episodes, nS, nA), dtype=np.float64)
-        # Explanation of lambda:
-        # def select_action(state, Q, epsilon):
-        #   if np.random.random() > epsilon:
-        #       return np.argmax(Q[state])
-        #   else:
-        #       return np.random.randint(len(Q[state]))
-        select_action = lambda state, Q, epsilon: np.argmax(Q[state]) \
-            if np.random.random() > epsilon \
-            else np.random.randint(len(Q[state]))
-        alphas = RL.decay_schedule(init_alpha,
-                                min_alpha,
-                                alpha_decay_ratio,
-                                n_episodes)
-        epsilons = RL.decay_schedule(init_epsilon,
-                                  min_epsilon,
-                                  epsilon_decay_ratio,
-                                  n_episodes)
-        for e in tqdm(range(n_episodes), leave=False):
-            self.callbacks.on_episode_begin(self)
-            self.callbacks.on_episode(self, episode=e)
-            state, info = self.env.reset()
-            done = False
-            state = convert_state_obs(state, done)
-            while not done:
-                if self.render:
-                    warnings.warn("Occasional render has been deprecated by openAI.  Use test_env.py to render.")
-                action = select_action(state, Q, epsilons[e])
-                next_state, reward, terminated, truncated, _ = self.env.step(action)
-                if truncated:
-                    warnings.warn("Episode was truncated.  Bootstrapping 0 reward.")
-                done = terminated or truncated
-                self.callbacks.on_env_step(self)
-                next_state = convert_state_obs(next_state,done)
-                td_target = reward + gamma * Q[next_state].max() * (not done)
-                td_error = td_target - Q[state][action]
-                Q[state][action] = Q[state][action] + alphas[e] * td_error
-                state = next_state
-            Q_track[e] = Q
-            pi_track.append(np.argmax(Q, axis=1))
-            self.render = False
-            self.callbacks.on_episode_end(self)
-
-        V = np.max(Q, axis=1)
-        # Explanation of lambda:
-        # def pi(s):
-        #   policy = dict()
-        #   for state, action in enumerate(np.argmax(Q, axis=1)):
-        #       policy[state] = action
-        #   return policy[s]
-        pi = lambda s: {s: a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
-        return Q, V, pi, Q_track, pi_track
-
-    @print_runtime
-    def sarsa(self,
-              nS=None,
-              nA=None,
-              convert_state_obs=lambda state, done: state,
-              gamma=.99,
-              init_alpha=0.5,
-              min_alpha=0.01,
-              alpha_decay_ratio=0.5,
-              init_epsilon=1.0,
-              min_epsilon=0.1,
-              epsilon_decay_ratio=0.9,
-              n_episodes=10000):
-        """
-        Parameters
-        ----------------------------
-        nS {int}:
-            Number of states
-        
-        nA {int}:
-            Number of available actions
-            
-        convert_state_obs {lambda}:
-            The state conversion utilized in BlackJack ToyText problem.
-            Returns three state tuple as one of the 280 converted states.
-        
-        gamma {float}, default = 0.99:
-            Discount factor
-        
-        init_alpha {float}, default = 0.5:
-            Learning rate
-        
-        min_alpha {float}, default = 0.01:
-            Minimum learning rate
-        
-        alpha_decay_ratio {float}, default = 0.5:
-            Decay schedule of learing rate for future iterations
-        
-        init_epsilon {float}, default = 0.1:
-            Initial epsilon value for epsilon greedy strategy.
-            Chooses max(Q) over available actions with probability 1-epsilon.
-        
-        min_epsilon {float}, default = 0.1:
-            Minimum epsilon. Used to balance exploration in later stages.
-        
-        epsilon_decay_ratio {float}, default = 0.9:
-            Decay schedule of epsilon for future iterations
-            
-        n_episodes {int}, default = 10000:
-            Number of episodes for the agent
-
-
-        Returns
-        ----------------------------
-        Q {numpy array}, shape(nS, nA):
-            Final action-value function Q(s,a)
-
-        pi {lambda}, input state value, output action value:
-            Optimal policy which maps state action value
-
-        V {numpy array}, shape(nS):
-            Optimal value array
-
-        Q_track {numpy array}, shape(n_episodes, nS, nA):
-            Log of Q(s,a) for each episode
-
-        pi_track {list}, len(n_episodes):
-            Log of complete policy for each episode
-        """
-        if nS is None:
-            nS = self.env.observation_space.n
-        if nA is None:
-            nA = self.env.action_space.n
-        pi_track = []
-        Q = np.zeros((nS, nA), dtype=np.float64)
-        Q_track = np.zeros((n_episodes, nS, nA), dtype=np.float64)
-        # Explanation of lambda:
-        # def select_action(state, Q, epsilon):
-        #   if np.random.random() > epsilon:
-        #       return np.argmax(Q[state])
-        #   else:
-        #       return np.random.randint(len(Q[state]))
-        select_action = lambda state, Q, epsilon: np.argmax(Q[state]) \
-            if np.random.random() > epsilon \
-            else np.random.randint(len(Q[state]))
-        alphas = RL.decay_schedule(init_alpha,
-                                min_alpha,
-                                alpha_decay_ratio,
-                                n_episodes)
-        epsilons = RL.decay_schedule(init_epsilon,
-                                  min_epsilon,
-                                  epsilon_decay_ratio,
-                                  n_episodes)
-
-        for e in tqdm(range(n_episodes), leave=False):
-            self.callbacks.on_episode_begin(self)
-            self.callbacks.on_episode(self, episode=e)
-            state, info = self.env.reset()
-            done = False
-            state = convert_state_obs(state, done)
-            action = select_action(state, Q, epsilons[e])
-            while not done:
-                if self.render:
-                    warnings.warn("Occasional render has been deprecated by openAI.  Use test_env.py to render.")
-                next_state, reward, terminated, truncated, _ = self.env.step(action)
-                if truncated:
-                    warnings.warn("Episode was truncated.  Bootstrapping 0 reward.")
-                done = terminated or truncated
-                self.callbacks.on_env_step(self)
-                next_state = convert_state_obs(next_state, done)
-                next_action = select_action(next_state, Q, epsilons[e])
-                td_target = reward + gamma * Q[next_state][next_action] * (not done)
-                td_error = td_target - Q[state][action]
-                Q[state][action] = Q[state][action] + alphas[e] * td_error
-                state, action = next_state, next_action
-            Q_track[e] = Q
-            pi_track.append(np.argmax(Q, axis=1))
-            self.render = False
-            self.callbacks.on_episode_end(self)
-
-        V = np.max(Q, axis=1)
-        # Explanation of lambda:
-        # def pi(s):
-        #   policy = dict()
-        #   for state, action in enumerate(np.argmax(Q, axis=1)):
-        #       policy[state] = action
-        #   return policy[s]
-        pi = lambda s: {s: a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
-        return Q, V, pi, Q_track, pi_track
+"""
+Author: Miguel Morales
+BSD 3-Clause License
+
+Copyright (c) 2018, Miguel Morales
+All rights reserved.
+https://github.com/mimoralea/gdrl/blob/master/LICENSE
+"""
+
+"""
+modified by: John Mansfield
+
+documentation added by: Gagandeep Randhawa
+"""
+
+"""
+Model-free learning algorithms: Q-Learning and SARSA
+
+Assumes no prior knowledge of the type of reward available to the agent.
+Given enough episodes, tries to find an estimate of the optimal policy.
+"""
+
+import numpy as np
+from tqdm import tqdm
+from utils.callbacks import MyCallbacks
+from utils.decorators import print_runtime
+import warnings
+
+
+class RL:
+    def __init__(self, env):
+        self.env = env
+        self.callbacks = MyCallbacks()
+        self.render = False
+
+    @staticmethod
+    def decay_schedule(init_value, min_value, decay_ratio, max_steps, log_start=-2, log_base=10):
+        """
+        Parameters
+        ----------------------------
+        init_value {float}:
+            Initial value of the quantity being decayed
+        
+        min_value {float}:
+            Minimum value init_value is allowed to decay to
+            
+        decay_ratio {float}:
+            The exponential factor exp(decay_ratio).
+            Updated decayed value is calculated as 
+        
+        max_steps {int}:
+            Max iteration steps for decaying init_value
+        
+        log_start {array-like}, default = -2:
+            Starting value of the decay sequence.
+            Default value starts it at 0.01
+        
+        log_base {array-like}, default = 10:
+            Base of the log space.
+        
+        
+        Returns
+        ----------------------------
+        values {array-like}, shape(max_steps):
+            Decay values where values[i] is the value used at i-th step
+        """
+        decay_steps = int(max_steps * decay_ratio)
+        rem_steps = max_steps - decay_steps
+        values = np.logspace(log_start, 0, decay_steps, base=log_base, endpoint=True)[::-1]
+        values = (values - values.min()) / (values.max() - values.min())
+        values = (init_value - min_value) * values + min_value
+        values = np.pad(values, (0, rem_steps), 'edge')
+        return values
+
+    @print_runtime
+    def q_learning(self,
+                   nS=None,
+                   nA=None,
+                   convert_state_obs=lambda state, done: state,
+                   gamma=.99,
+                   init_alpha=0.5,
+                   min_alpha=0.01,
+                   alpha_decay_ratio=0.5,
+                   init_epsilon=1.0,
+                   min_epsilon=0.1,
+                   epsilon_decay_ratio=0.9,
+                   n_episodes=10000):
+        """
+        Parameters
+        ----------------------------
+        nS {int}:
+            Number of states
+        
+        nA {int}:
+            Number of available actions
+            
+        convert_state_obs {lambda}:
+            The state conversion utilized in BlackJack ToyText problem.
+            Returns three state tuple as one of the 280 converted states.
+        
+        gamma {float}, default = 0.99:
+            Discount factor
+        
+        init_alpha {float}, default = 0.5:
+            Learning rate
+        
+        min_alpha {float}, default = 0.01:
+            Minimum learning rate
+        
+        alpha_decay_ratio {float}, default = 0.5:
+            Decay schedule of learing rate for future iterations
+        
+        init_epsilon {float}, default = 1.0:
+            Initial epsilon value for epsilon greedy strategy.
+            Chooses max(Q) over available actions with probability 1-epsilon.
+        
+        min_epsilon {float}, default = 0.1:
+            Minimum epsilon. Used to balance exploration in later stages.
+        
+        epsilon_decay_ratio {float}, default = 0.9:
+            Decay schedule of epsilon for future iterations
+            
+        n_episodes {int}, default = 10000:
+            Number of episodes for the agent
+
+
+        Returns
+        ----------------------------
+        Q {numpy array}, shape(nS, nA):
+            Final action-value function Q(s,a)
+
+        pi {lambda}, input state value, output action value:
+            Policy mapping states to actions.
+
+        V {numpy array}, shape(nS):
+            State values array
+
+        Q_track {numpy array}, shape(n_episodes, nS, nA):
+            Log of Q(s,a) for each episode
+
+        pi_track {list}, len(n_episodes):
+            Log of complete policy for each episode
+        """
+        if nS is None:
+            nS=self.env.observation_space.n
+        if nA is None:
+            nA=self.env.action_space.n
+        pi_track = []
+        Q = np.zeros((nS, nA), dtype=np.float64)
+        Q_track = np.zeros((n_episodes, nS, nA), dtype=np.float64)
+        # Explanation of lambda:
+        # def select_action(state, Q, epsilon):
+        #   if np.random.random() > epsilon:
+        #       return np.argmax(Q[state])
+        #   else:
+        #       return np.random.randint(len(Q[state]))
+        select_action = lambda state, Q, epsilon: np.argmax(Q[state]) \
+            if np.random.random() > epsilon \
+            else np.random.randint(len(Q[state]))
+        alphas = RL.decay_schedule(init_alpha,
+                                min_alpha,
+                                alpha_decay_ratio,
+                                n_episodes)
+        epsilons = RL.decay_schedule(init_epsilon,
+                                  min_epsilon,
+                                  epsilon_decay_ratio,
+                                  n_episodes)
+        for e in tqdm(range(n_episodes), leave=False):
+            self.callbacks.on_episode_begin(self)
+            self.callbacks.on_episode(self, episode=e)
+            state, info = self.env.reset()
+            done = False
+            state = convert_state_obs(state, done)
+            while not done:
+                if self.render:
+                    warnings.warn("Occasional render has been deprecated by openAI.  Use test_env.py to render.")
+                action = select_action(state, Q, epsilons[e])
+                next_state, reward, terminated, truncated, _ = self.env.step(action)
+                if truncated:
+                    warnings.warn("Episode was truncated.  Bootstrapping 0 reward.")
+                done = terminated or truncated
+                self.callbacks.on_env_step(self)
+                next_state = convert_state_obs(next_state,done)
+                td_target = reward + gamma * Q[next_state].max() * (not done)
+                td_error = td_target - Q[state][action]
+                Q[state][action] = Q[state][action] + alphas[e] * td_error
+                state = next_state
+            Q_track[e] = Q
+            pi_track.append(np.argmax(Q, axis=1))
+            self.render = False
+            self.callbacks.on_episode_end(self)
+
+        V = np.max(Q, axis=1)
+        # Explanation of lambda:
+        # def pi(s):
+        #   policy = dict()
+        #   for state, action in enumerate(np.argmax(Q, axis=1)):
+        #       policy[state] = action
+        #   return policy[s]
+        pi = lambda s: {s: a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
+        return Q, V, pi, Q_track, pi_track
+
+    @print_runtime
+    def sarsa(self,
+              nS=None,
+              nA=None,
+              convert_state_obs=lambda state, done: state,
+              gamma=.99,
+              init_alpha=0.5,
+              min_alpha=0.01,
+              alpha_decay_ratio=0.5,
+              init_epsilon=1.0,
+              min_epsilon=0.1,
+              epsilon_decay_ratio=0.9,
+              n_episodes=10000):
+        """
+        Parameters
+        ----------------------------
+        nS {int}:
+            Number of states
+        
+        nA {int}:
+            Number of available actions
+            
+        convert_state_obs {lambda}:
+            The state conversion utilized in BlackJack ToyText problem.
+            Returns three state tuple as one of the 280 converted states.
+        
+        gamma {float}, default = 0.99:
+            Discount factor
+        
+        init_alpha {float}, default = 0.5:
+            Learning rate
+        
+        min_alpha {float}, default = 0.01:
+            Minimum learning rate
+        
+        alpha_decay_ratio {float}, default = 0.5:
+            Decay schedule of learing rate for future iterations
+        
+        init_epsilon {float}, default = 1.0:
+            Initial epsilon value for epsilon greedy strategy.
+            Chooses max(Q) over available actions with probability 1-epsilon.
+        
+        min_epsilon {float}, default = 0.1:
+            Minimum epsilon. Used to balance exploration in later stages.
+        
+        epsilon_decay_ratio {float}, default = 0.9:
+            Decay schedule of epsilon for future iterations
+            
+        n_episodes {int}, default = 10000:
+            Number of episodes for the agent
+
+
+        Returns
+        ----------------------------
+        Q {numpy array}, shape(nS, nA):
+            Final action-value function Q(s,a)
+
+        pi {lambda}, input state value, output action value:
+            Policy mapping states to actions.
+
+        V {numpy array}, shape(nS):
+            State values array
+
+        Q_track {numpy array}, shape(n_episodes, nS, nA):
+            Log of Q(s,a) for each episode
+
+        pi_track {list}, len(n_episodes):
+            Log of complete policy for each episode
+        """
+        if nS is None:
+            nS = self.env.observation_space.n
+        if nA is None:
+            nA = self.env.action_space.n
+        pi_track = []
+        Q = np.zeros((nS, nA), dtype=np.float64)
+        Q_track = np.zeros((n_episodes, nS, nA), dtype=np.float64)
+        # Explanation of lambda:
+        # def select_action(state, Q, epsilon):
+        #   if np.random.random() > epsilon:
+        #       return np.argmax(Q[state])
+        #   else:
+        #       return np.random.randint(len(Q[state]))
+        select_action = lambda state, Q, epsilon: np.argmax(Q[state]) \
+            if np.random.random() > epsilon \
+            else np.random.randint(len(Q[state]))
+        alphas = RL.decay_schedule(init_alpha,
+                                min_alpha,
+                                alpha_decay_ratio,
+                                n_episodes)
+        epsilons = RL.decay_schedule(init_epsilon,
+                                  min_epsilon,
+                                  epsilon_decay_ratio,
+                                  n_episodes)
+
+        for e in tqdm(range(n_episodes), leave=False):
+            self.callbacks.on_episode_begin(self)
+            self.callbacks.on_episode(self, episode=e)
+            state, info = self.env.reset()
+            done = False
+            state = convert_state_obs(state, done)
+            action = select_action(state, Q, epsilons[e])
+            while not done:
+                if self.render:
+                    warnings.warn("Occasional render has been deprecated by openAI.  Use test_env.py to render.")
+                next_state, reward, terminated, truncated, _ = self.env.step(action)
+                if truncated:
+                    warnings.warn("Episode was truncated.  Bootstrapping 0 reward.")
+                done = terminated or truncated
+                self.callbacks.on_env_step(self)
+                next_state = convert_state_obs(next_state, done)
+                next_action = select_action(next_state, Q, epsilons[e])
+                td_target = reward + gamma * Q[next_state][next_action] * (not done)
+                td_error = td_target - Q[state][action]
+                Q[state][action] = Q[state][action] + alphas[e] * td_error
+                state, action = next_state, next_action
+            Q_track[e] = Q
+            pi_track.append(np.argmax(Q, axis=1))
+            self.render = False
+            self.callbacks.on_episode_end(self)
+
+        V = np.max(Q, axis=1)
+        # Explanation of lambda:
+        # def pi(s):
+        #   policy = dict()
+        #   for state, action in enumerate(np.argmax(Q, axis=1)):
+        #       policy[state] = action
+        #   return policy[s]
+        pi = lambda s: {s: a for s, a in enumerate(np.argmax(Q, axis=1))}[s]
+        return Q, V, pi, Q_track, pi_track
```

### Comparing `bettermdptools-0.3.0/decorators/decorators.py` & `bettermdptools-0.4.0/utils/decorators.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import functools
-import time
-
-
-def print_runtime(func):
-    @functools.wraps(func)
-    def wrapper_print_runtime(*args, **kwargs):
-        start = time.time()
-        value = func(*args, **kwargs)
-        end = time.time()
-        running_time = end - start
-        print("runtime = %.2f seconds" % running_time)
-        return value
-    return wrapper_print_runtime
-
-
-# from https://wiki.python.org/moin/PythonDecoratorLibrary
-def add_to(func):
-    @functools.wraps(func)
-    def decorator(*args, **kwargs):
-        setattr(func, args[0].__name__, args[0])
-        return func
-    return decorator
-
-
-# from https://realpython.com/
-def debug(func):
-    """Print the function signature and return value"""
-    @functools.wraps(func)
-    def wrapper_debug(*args, **kwargs):
-        args_repr = [repr(a) for a in args]                      # 1
-        kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]  # 2
-        signature = ", ".join(args_repr + kwargs_repr)           # 3
-        print(f"Calling {func.__name__}({signature})")
-        value = func(*args, **kwargs)
-        print(f"{func.__name__!r} returned {value!r}")           # 4
-        return value
-    return wrapper_debug
+import functools
+import time
+
+
+def print_runtime(func):
+    @functools.wraps(func)
+    def wrapper_print_runtime(*args, **kwargs):
+        start = time.time()
+        value = func(*args, **kwargs)
+        end = time.time()
+        running_time = end - start
+        print("runtime = %.2f seconds" % running_time)
+        return value
+    return wrapper_print_runtime
+
+
+# from https://wiki.python.org/moin/PythonDecoratorLibrary
+def add_to(func):
+    @functools.wraps(func)
+    def decorator(*args, **kwargs):
+        setattr(func, args[0].__name__, args[0])
+        return func
+    return decorator
+
+
+# from https://realpython.com/
+def debug(func):
+    """Print the function signature and return value"""
+    @functools.wraps(func)
+    def wrapper_debug(*args, **kwargs):
+        args_repr = [repr(a) for a in args]                      # 1
+        kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]  # 2
+        signature = ", ".join(args_repr + kwargs_repr)           # 3
+        print(f"Calling {func.__name__}({signature})")
+        value = func(*args, **kwargs)
+        print(f"{func.__name__!r} returned {value!r}")           # 4
+        return value
+    return wrapper_debug
```

### Comparing `bettermdptools-0.3.0/examples/grid_search.py` & `bettermdptools-0.4.0/examples/grid_search.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# -*- coding: utf-8 -*-
-
-import gym
-import pygame
-from examples.test_env import TestEnv
-from algorithms.rl import RL
-import itertools
-
-
-class GridSearch:
-    @staticmethod
-    def Q_learning_grid_search(env, epsilon_decay, iters):
-        for i in itertools.product(epsilon_decay, iters):
-            print("running -- with epsilon decay: ", i[0],  " iterations: ", i[1])
-            Q, V, pi, Q_track, pi_track = RL(env).q_learning(epsilon_decay_ratio=i[0], n_episodes=i[1])
-
-
-if __name__ == "__main__":
-    frozen_lake = gym.make('FrozenLake8x8-v1', render_mode=None)
-    epsilon_decay = [.4, .7, .9]
-    iters = [500, 5000, 50000]
-    GridSearch.Q_learning_grid_search(frozen_lake.env, epsilon_decay, iters)
+# -*- coding: utf-8 -*-
+
+import gym
+import pygame
+from examples.test_env import TestEnv
+from algorithms.rl import RL
+import itertools
+
+
+class GridSearch:
+    @staticmethod
+    def Q_learning_grid_search(env, epsilon_decay, iters):
+        for i in itertools.product(epsilon_decay, iters):
+            print("running -- with epsilon decay: ", i[0],  " iterations: ", i[1])
+            Q, V, pi, Q_track, pi_track = RL(env).q_learning(epsilon_decay_ratio=i[0], n_episodes=i[1])
+
+
+if __name__ == "__main__":
+    frozen_lake = gym.make('FrozenLake8x8-v1', render_mode=None)
+    epsilon_decay = [.4, .7, .9]
+    iters = [500, 5000, 50000]
+    GridSearch.Q_learning_grid_search(frozen_lake.env, epsilon_decay, iters)
```

### Comparing `bettermdptools-0.3.0/examples/plots.py` & `bettermdptools-0.4.0/examples/plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# -*- coding: utf-8 -*-
-import math
-
-import gym
-import pygame
-from algorithms.rl import RL
-from algorithms.planner import Planner
-from examples.test_env import TestEnv
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-import warnings
-from matplotlib.colors import LinearSegmentedColormap
-
-
-class Plots:
-    @staticmethod
-    def grid_world_policy_plot(data, label):
-        if not math.modf(math.sqrt(len(data)))[0] == 0.0:
-            warnings.warn("Grid map expected.  Check data length")
-        else:
-            data = np.around(np.array(data).reshape((8, 8)), 2)
-            df = pd.DataFrame(data=data)
-            my_colors = ((0.0, 0.0, 0.0, 1.0), (0.8, 0.0, 0.0, 1.0), (0.0, 0.8, 0.0, 1.0), (0.0, 0.0, 0.8, 1.0))
-            cmap = LinearSegmentedColormap.from_list('Custom', my_colors, len(my_colors))
-            ax = sns.heatmap(df, cmap=cmap, linewidths=1.0)
-            colorbar = ax.collections[0].colorbar
-            colorbar.set_ticks([.4, 1.1, 1.9, 2.6])
-            colorbar.set_ticklabels(['Left', 'Down', 'Right', 'Up'])
-            plt.title(label)
-            plt.show()
-
-    @staticmethod
-    def grid_values_heat_map(data, label):
-        if not math.modf(math.sqrt(len(data)))[0] == 0.0:
-            warnings.warn("Grid map expected.  Check data length")
-        else:
-            data = np.around(np.array(data).reshape((8, 8)), 2)
-            df = pd.DataFrame(data=data)
-            sns.heatmap(df, annot=True).set_title(label)
-            plt.show()
-
-    @staticmethod
-    def v_iters_plot(data, label):
-        df = pd.DataFrame(data=data)
-        df.columns = [label]
-        sns.set_theme(style="whitegrid")
-        title = label + " v Iterations"
-        sns.lineplot(x=df.index, y=label, data=df).set_title(title)
-        plt.show()
-
-if __name__ == "__main__":
-    frozen_lake = gym.make('FrozenLake8x8-v1', render_mode=None)
-
-    # VI/PI grid_world_policy_plot
-    # V, V_track, pi = Planner(frozen_lake.env.P).value_iteration()
-    # n_states = frozen_lake.env.observation_space.n
-    # new_pi = list(map(lambda x: pi(x), range(n_states)))
-    # s = int(math.sqrt(n_states))
-    # Plots.grid_world_policy_plot(np.array(new_pi), "Grid World Policy")
-
-    # Q-learning grid_world_policy_plot
-    # Q, V, pi, Q_track, pi_track = RL(frozen_lake.env).q_learning()
-    # n_states = frozen_lake.env.observation_space.n
-    # new_pi = list(map(lambda x: pi(x), range(n_states)))
-    # s = int(math.sqrt(n_states))
-    # Plots.grid_world_policy_plot(np.array(new_pi), "Grid World Policy")
-
-    # Q-learning v_iters_plot
-    # Q, V, pi, Q_track, pi_track = RL(frozen_lake.env).q_learning()
-    # max_reward_per_iter = np.amax(np.amax(Q_track, axis=2), axis=1)
-    # Plots.v_iters_plot(max_reward_per_iter, "Reward")
-
-    # VI/PI v_iters_plot
-    # V, V_track, pi = Planner(frozen_lake.env.P).value_iteration()
-    # V, V_track, pi = Planner(frozen_lake.env.P).policy_iteration()
-    # max_value_per_iter = np.amax(V_track, axis=1)
-    # Plots.v_iters_plot(max_value_per_iter, "Value")
-
-    # Q-learning grid_values_heat_map
-    # Q, V, pi, Q_track, pi_track = RL(frozen_lake.env).q_learning()
-    # Plots.grid_values_heat_map(V, "State Values")
-
-    # VI/PI grid_values_heat_map
-    V, V_track, pi = Planner(frozen_lake.env.P).value_iteration()
-    V, V_track, pi = Planner(frozen_lake.env.P).policy_iteration()
-    Plots.grid_values_heat_map(V, "State Values")
+# -*- coding: utf-8 -*-
+import math
+
+import gym
+import pygame
+from algorithms.rl import RL
+from algorithms.planner import Planner
+from examples.test_env import TestEnv
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
+import warnings
+from matplotlib.colors import LinearSegmentedColormap
+
+
+class Plots:
+    @staticmethod
+    def grid_world_policy_plot(data, label):
+        if not math.modf(math.sqrt(len(data)))[0] == 0.0:
+            warnings.warn("Grid map expected.  Check data length")
+        else:
+            data = np.around(np.array(data).reshape((8, 8)), 2)
+            df = pd.DataFrame(data=data)
+            my_colors = ((0.0, 0.0, 0.0, 1.0), (0.8, 0.0, 0.0, 1.0), (0.0, 0.8, 0.0, 1.0), (0.0, 0.0, 0.8, 1.0))
+            cmap = LinearSegmentedColormap.from_list('Custom', my_colors, len(my_colors))
+            ax = sns.heatmap(df, cmap=cmap, linewidths=1.0)
+            colorbar = ax.collections[0].colorbar
+            colorbar.set_ticks([.4, 1.1, 1.9, 2.6])
+            colorbar.set_ticklabels(['Left', 'Down', 'Right', 'Up'])
+            plt.title(label)
+            plt.show()
+
+    @staticmethod
+    def grid_values_heat_map(data, label):
+        if not math.modf(math.sqrt(len(data)))[0] == 0.0:
+            warnings.warn("Grid map expected.  Check data length")
+        else:
+            data = np.around(np.array(data).reshape((8, 8)), 2)
+            df = pd.DataFrame(data=data)
+            sns.heatmap(df, annot=True).set_title(label)
+            plt.show()
+
+    @staticmethod
+    def v_iters_plot(data, label):
+        df = pd.DataFrame(data=data)
+        df.columns = [label]
+        sns.set_theme(style="whitegrid")
+        title = label + " v Iterations"
+        sns.lineplot(x=df.index, y=label, data=df).set_title(title)
+        plt.show()
+
+if __name__ == "__main__":
+    frozen_lake = gym.make('FrozenLake8x8-v1', render_mode=None)
+
+    # VI/PI grid_world_policy_plot
+    # V, V_track, pi = Planner(frozen_lake.env.P).value_iteration()
+    # n_states = frozen_lake.env.observation_space.n
+    # new_pi = list(map(lambda x: pi(x), range(n_states)))
+    # s = int(math.sqrt(n_states))
+    # Plots.grid_world_policy_plot(np.array(new_pi), "Grid World Policy")
+
+    # Q-learning grid_world_policy_plot
+    # Q, V, pi, Q_track, pi_track = RL(frozen_lake.env).q_learning()
+    # n_states = frozen_lake.env.observation_space.n
+    # new_pi = list(map(lambda x: pi(x), range(n_states)))
+    # s = int(math.sqrt(n_states))
+    # Plots.grid_world_policy_plot(np.array(new_pi), "Grid World Policy")
+
+    # Q-learning v_iters_plot
+    # Q, V, pi, Q_track, pi_track = RL(frozen_lake.env).q_learning()
+    # max_q_value_per_iter = np.amax(np.amax(Q_track, axis=2), axis=1)
+    # Plots.v_iters_plot(max_q_value_per_iter, "Max Q-Values")
+
+    # VI/PI v_iters_plot
+    # V, V_track, pi = Planner(frozen_lake.env.P).value_iteration()
+    # V, V_track, pi = Planner(frozen_lake.env.P).policy_iteration()
+    # max_value_per_iter = np.amax(V_track, axis=1)
+    # Plots.v_iters_plot(max_value_per_iter, "Max State Values")
+
+    # Q-learning grid_values_heat_map
+    # Q, V, pi, Q_track, pi_track = RL(frozen_lake.env).q_learning()
+    # Plots.grid_values_heat_map(V, "State Values")
+
+    # VI/PI grid_values_heat_map
+    # V, V_track, pi = Planner(frozen_lake.env.P).value_iteration()
+    V, V_track, pi = Planner(frozen_lake.env.P).policy_iteration()
+    Plots.grid_values_heat_map(V, "State Values")
```

### Comparing `bettermdptools-0.3.0/setup.py` & `bettermdptools-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup, find_packages
-
-"""
-"pip install pygame" error warning:
-if you're facing trouble installing pygame with Python 3.11, you need to install with following command:
-'pip install pygame --pre'
-
-More discussion:
-https://stackoverflow.com/questions/74188013/python-pygame-not-installing
-"""
-
-setup(
-    name='bettermdptools',
-    url='https://github.com/jlm429/bettermdptools',
-    version='0.3.0',
-    platforms=['Any'],
-    license='New BSD',
-    author='John Mansfield',
-    author_email='jlm429@gmail.com',
-    packages=["algorithms", "callbacks", "decorators", "examples"],
-    install_requires=['gym>=0.26, <=0.26.2', 'pygame', 'numpy', 'tqdm', 'pandas', 'seaborn', 'matplotlib'],
-)
+# -*- coding: utf-8 -*-
+from setuptools import setup, find_packages
+
+"""
+"pip install pygame" error warning:
+if you're facing trouble installing pygame with Python 3.11, you need to install with following command:
+'pip install pygame --pre'
+
+More discussion:
+https://stackoverflow.com/questions/74188013/python-pygame-not-installing
+"""
+
+setup(
+    name='bettermdptools',
+    url='https://github.com/jlm429/bettermdptools',
+    version='0.4.0',
+    platforms=['Any'],
+    license='New BSD',
+    author='John Mansfield',
+    author_email='jlm429@gmail.com',
+    packages=["algorithms", "utils", "examples"],
+    install_requires=['gym>=0.26, <=0.26.2', 'pygame', 'numpy', 'tqdm', 'pandas', 'seaborn', 'matplotlib'],
+)
```

