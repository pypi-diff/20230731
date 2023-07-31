# Comparing `tmp/pyapep-0.1.2.tar.gz` & `tmp/pyapep-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapep-0.1.2.tar", last modified: Sun May 14 14:42:15 2023, max compression
+gzip compressed data, was "pyapep-0.1.3.tar", last modified: Mon Jul 31 17:52:40 2023, max compression
```

## Comparing `pyapep-0.1.2.tar` & `pyapep-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:42:15.107047 pyapep-0.1.2/
--rw-rw-rw-   0        0        0      352 2023-05-14 14:42:15.107047 pyapep-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      367 2022-05-27 15:52:19.000000 pyapep-0.1.2/README
-drwxrwxrwx   0        0        0        0 2023-05-14 14:42:15.107047 pyapep-0.1.2/pyapep/
--rw-rw-rw-   0        0        0        0 2022-10-19 06:19:02.000000 pyapep-0.1.2/pyapep/__init__.py
--rw-rw-rw-   0        0        0    22187 2022-12-20 03:37:29.000000 pyapep-0.1.2/pyapep/isofit.py
--rw-rw-rw-   0        0        0     8353 2022-05-27 15:52:19.000000 pyapep-0.1.2/pyapep/simide.py
--rw-rw-rw-   0        0        0   116098 2023-05-13 11:52:01.000000 pyapep-0.1.2/pyapep/simsep.py
--rw-rw-rw-   0        0        0    87603 2022-10-19 06:19:02.000000 pyapep-0.1.2/pyapep/simsep_backup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:42:15.107047 pyapep-0.1.2/pyapep.egg-info/
--rw-rw-rw-   0        0        0      352 2023-05-14 14:42:13.000000 pyapep-0.1.2/pyapep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-14 14:42:14.000000 pyapep-0.1.2/pyapep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:42:13.000000 pyapep-0.1.2/pyapep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-14 14:42:14.000000 pyapep-0.1.2/pyapep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-14 14:42:14.000000 pyapep-0.1.2/pyapep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 14:42:15.122571 pyapep-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      931 2023-05-14 14:41:22.000000 pyapep-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:40.550582 pyapep-0.1.3/
+-rw-rw-rw-   0        0        0      329 2023-07-31 17:52:40.548582 pyapep-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2022-05-27 15:52:19.000000 pyapep-0.1.3/README
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:40.536204 pyapep-0.1.3/pyAPEP/
+-rw-rw-rw-   0        0        0     2453 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_blowdown.py
+-rw-rw-rw-   0        0        0     2460 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_blowdown_reverse.py
+-rw-rw-rw-   0        0        0     2369 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_flowthrough.py
+-rw-rw-rw-   0        0        0     2380 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_flowthrough_reverse.py
+-rw-rw-rw-   0        0        0     2459 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_pressurization.py
+-rw-rw-rw-   0        0        0     2460 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_pressurization_reverse.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/__init__.py
+-rw-rw-rw-   0        0        0    22187 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/isofit.py
+-rw-rw-rw-   0        0        0     8353 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/simide.py
+-rw-rw-rw-   0        0        0   140667 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/simsep.py
+-rw-rw-rw-   0        0        0    87603 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/simsep_backup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:40.546581 pyapep-0.1.3/pyapep.egg-info/
+-rw-rw-rw-   0        0        0      329 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-31 17:52:40.000000 pyapep-0.1.3/pyapep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 17:52:40.550582 pyapep-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-07-31 17:51:55.000000 pyapep-0.1.3/setup.py
```

### Comparing `pyapep-0.1.2/pyapep/isofit.py` & `pyapep-0.1.3/pyAPEP/isofit.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.2/pyapep/simide.py` & `pyapep-0.1.3/pyAPEP/simide.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.2/pyapep/simsep.py` & `pyapep-0.1.3/pyAPEP/simsep.py`

 * *Files 10% similar despite different names*

```diff
@@ -1723,23 +1723,556 @@
         ax.set_ylabel(yaxis_label, fontsize = 15)
         plt.xticks(fontsize = 13)
         plt.yticks(fontsize = 13)
         plt.grid(linestyle = ':')
         if file_name != None:
             fig.savefig(file_name, bbox_inches='tight')
         return fig, ax    
-    ## Copy the         
+    ## Copy the column
     def copy(self):
         import copy
         self_new = copy.deepcopy(self)
         return self_new
+    
+    ##### Linear velocity assumptions #####
+    ## Run mass balance only with linear velocity assumption ##
+    def run_ma_linvel(self, t_max, n_sec = 5, CPUtime_print = False):
+        # t domain
+        tic = time.time()/60 # in minute
+        t_max_int = np.int32(np.floor(t_max))
+        self._n_sec = n_sec
+        n_t = t_max_int*n_sec+ 1
+        
+        t_dom = np.linspace(0,t_max_int, n_t)
+        if t_max_int < t_max:
+            t_dom = np.concatenate((t_dom, [t_max]))
+        
+        # z axis
+        N = self._N
+        h = self._h
+        L = self._L
+        z = np.linspace(0,L,N)
+        # Geometry
+        A_cros = self._A
+        V_tot = L*self._A
+        epsi = self._epsi
+        dp = self._D_p
+        a_surf = self._a_surf
+        rho_s = self._rho_s
+        # n_comp
+        n_comp = self._n_comp
+        # Initial Conditions
+        y_av = []
+        mu_av = 0
+        for ii in range(n_comp):
+            y_av_tmp = np.mean(self._y_init[ii])
+            mu_av = mu_av + y_av_tmp*self._mu[ii]
+            y_av.append(y_av_tmp)
+        # Boundary (feed) conditions
+        P_feed = self._P_in
+        P_out = self._P_out
+        T_feed = self._T_in
+        y_feed = self._y_in      
+        # Three diff cases
+        # Case 1: Flowing through (both open valve)
+        if (self._Cv_in > 1E-10) and (self._Cv_out > 1E-10):
+            ########### IF "BACKWARD" ???? ########
+            # Velocity (constant)
+            u_feed = self._Q_in/epsi/self._A
+            P_L = P_out + self._Q_in/self._Cv_out # in bar # Note Cv_out in (m^3/s/bar)
+            Rgas = 8.3145    # J/mol/K
+            # Pressure profiles
+            P_av = (P_out+P_feed)/2     # in bar
+            DPDz_term1 = -1.75*P_av*1E5/R_gas/T_feed*(1-epsi)/epsi*u_feed**2
+            DPDz_term2 = -150*mu_av/dp**2*(1-epsi)**2/epsi**2*u_feed
+            DPDz = DPDz_term1 + DPDz_term2          # in (Pa/m)
+            P_0 = P_L + DPDz*1E-5                   # in bar
+            P_in = P_0 + self._Q_in/self._Cv_in     # in bar # in bar # Note Cv_out in (m^3/s/bar)
+            # P profile once again
+            P_av = (P_out+P_in)/2
+            DPDz_term1 = -1.75*P_av*1E5/R_gas/T_feed*(1-epsi)/epsi*u_feed**2
+            DPDz_term2 = -150*mu_av/dp**2*(1-epsi)**2/epsi**2*u_feed
+            DPDz = DPDz_term1 + DPDz_term2 # in (Pa/m)
+            P_0 = P_L + DPDz*1E-5
+            P_in = P_0 + self._Q_in/self._Cv_in
+            P = DPDz*1E-5*z + P_0   # bar
+            # C profile
+            C = P*1E5/R_gas/T_feed   # mol/m^3
+            # Mass transfer ...
+            k_mtc = self._k_mtc
+            D_AB = self._D_disp
+            a_surf = self._a_surf
+
+            def massbal_linvel(y,t):
+                y_comp = []
+                P_part = []
+                dy_comp = []
+                ddy_comp = []
+                for ii in range(n_comp-1):
+                    y_tmp = np.array(y[ii*N:(ii+1)*N])
+                    y_tmp[y_tmp<1E-6] = 0
+                    dy_tmp = self._d@y_tmp
+                    ddy_tmp =self._dd@y_tmp
+                    P_part_tmp = y_tmp*P
+                    #y_tmp[y_tmp<1E-6] = 0
+                    y_comp.append(y_tmp)
+                    P_part.append(P_part_tmp)
+                    dy_comp.append(dy_tmp)
+                    ddy_comp.append(ddy_tmp)
+                y_rest = 1-np.sum(y_comp, 0)
+                P_part.append(P*y_rest)
+                #print('Shape of P_part[0]',P_part[0].shape)
+                q = []
+                for ii in range(n_comp-1, 2*n_comp-1):
+                    q.append(y[ii*N:(ii+1)*N])
+                # Solid uptake component
+                dqdt = []
+                qstar = self._iso(P_part,T_feed)
+                for ii in range(n_comp):
+                    dqdt_tmp = k_mtc[ii]*a_surf*(qstar[ii] - q[ii])
+                    dqdt.append(dqdt_tmp)
+                # Solid uptake total
+                Sig_dqdt = np.sum(dqdt, 0)
+                #print(Sig_dqdt)
+                dy_compdt = []
+                for ii in range(n_comp-1):
+                    term1 = -u_feed*dy_comp[ii]
+                    term2 = D_AB[ii]*0 # How to calculate d(yC)dz
+                    term3 = -rho_s*(1-epsi)/epsi*dqdt[ii]
+                    term4 = 0
+                    term5 = +y_comp[ii]*rho_s*Sig_dqdt*(1-epsi)/epsi
+                    
+                    #term1[0] = 0
+                    term1[0] = u_feed*self._d[1,1]*(y_feed[ii]-y_comp[ii][0])
+                    #term5[0] = 0
+                    #term1[-1] = -u_feed*d[1,1]*C[-1]*(y_comp[ii][-2]-y_comp[ii][-1])
+                    #term3[-1] = 0
+                    #term5[-1] = 0
+
+                    #dydt_tmp = term1+(term2 + term3+ term4 + term5)/C
+                    dydt_tmp = term1 + term3/C + term5/C
+                    #dydt_tmp[0] = 0
+                    #dydt_tmp[N-1] = 0 
+                    #ind_both = ((y_comp[ii]<1E-6) + (dydt_tmp < 0))>1.5
+                    #dydt_tmp[ind_both] = 0 
+                    dy_compdt.append(dydt_tmp)
+                dydt = []
+                for yy in dy_compdt:
+                    dydt.append(yy)
+                    #print(yy.shape)
+                for qq in dqdt:
+                    dydt.append(qq)
+                    #print(qq.shape)
+                dydt_arr = np.concatenate(dydt)
+                
+                return dydt_arr
+            
+            # Initial value again
+            y0 = np.zeros(N*(n_comp*2-1))
+            for ii in range(n_comp-1):
+                y0[ii*N : (ii+1)*N] = self._y_init[ii]
+                y0[(n_comp-1)*N+ii*N:(n_comp-1)*N+(ii+1)*N] = self._q_init[ii]
+            y0[2*(n_comp-1)*N:2*(n_comp-1)*N+N] = self._q_init[-1]
+            
+            # Backward flow case
+            if self._required['Flow direction'] == 'Backward':
+                y0_tmp = []
+                for ii in range(2*n_comp-1):
+                    mat_y0_pre_tmp = y0[ii*N:(ii+1)*N]
+                    mat_y0_rev_tmp = self._A_flip@mat_y0_pre_tmp
+                    y0_tmp.append(mat_y0_rev_tmp)
+                y0_rev = np.concatenate(y0_tmp)
+                y0 = y0_rev
+                
+            # Solve ode
+            y_result = odeint(massbal_linvel, y0, t_dom,)
+            
+            # BACKWARD FLOW !! #
+            # Flipped one for backward flow
+            if self._required['Flow direction'] == 'Backward':
+                y_tmp = []
+                q_tmp = []
+                for ii in range(n_comp-1):
+                    mat_y_tmp = y_result[:, ii*N : (ii+1)*N]
+                    mat_q_tmp = y_result[:, (n_comp-1+ii)*N : (n_comp+ii)*N]
+                    y_tmp.append(mat_y_tmp@self._A_flip)
+                    q_tmp.append(mat_q_tmp@self._A_flip)
+                mat_q_tmp = y_result[:, (2*n_comp-2)*N:(2*n_comp-1)*N]
+                q_tmp.append(mat_q_tmp@self._A_flip)
+                y_flip = np.concatenate(y_tmp+q_tmp, axis = 1)
+                y_result = y_flip
+            
+            # Assign the results (packaging the results)
+            C_tmp = []
+            q_tmp = []
+            y_tmp = []
+            mat_y_rest = np.zeros([len(t_dom), N])
+            for ii in range(n_comp-1):
+                mat_y_tmp = y_result[:, ii*N:(ii+1)*N]
+                mat_q_tmp = y_result[:, (n_comp-1+ii)*N : (n_comp+ii)*N]
+                mat_C_tmp = mat_y_tmp@np.diag(C)
+                
+                C_tmp.append(mat_C_tmp)
+                q_tmp.append(mat_q_tmp)
+                y_tmp.append(mat_y_tmp)
+                mat_y_rest = mat_y_rest + mat_y_tmp
+
+            C_tmp.append((1- mat_y_rest)@np.diag(C))
+            q_tmp.append(y_result[:, (2*n_comp-2)*N: (2*n_comp-1)*N])
+            
+            self._y_fra = y_tmp
+
+            Tg_tmp = T_feed*np.ones([len(t_dom), N])
+            Ts_tmp = T_feed*np.ones([len(t_dom), N])
+            y_result = np.concatenate(C_tmp + q_tmp + [Tg_tmp, Ts_tmp], axis=1)
+            self._y = y_result
+            self._t = t_dom
+
+            toc = time.time()/60 - tic
+            self._CPU_min = toc
+            if CPUtime_print:
+                print('Simulation of this step is completed.')
+                print('This took {0:9.3f} mins to run. \n'.format(toc))
+            
+            return y_result, self._z, t_dom
+
+        # Pressurization (open inlet only)
+        elif (self._Cv_in > 1E-10) and (self._Cv_out < 1E-10): 
+            # Initial Pressure and initial overal concentration
+            Rgas = 8.3145   # J/mol/K
+            P_av0 = np.mean(self._P_init)
+            C_av0 = P_av0*1E5/R_gas/T_feed   # mol/m^3
+            # Mass transfer
+            k_mtc = self._k_mtc
+            D_AB = self._D_disp
+            a_surf = self._a_surf
+
+            def massbal_linvel(y,t):
+                y_comp = []
+                P_part = []
+                dy_comp = []
+                ddy_comp = []
+                C = y[(2*n_comp-1)*N]
+                P_av = C*Rgas*T_feed/1E5   # mol/m^3
+                Q_feed = self._Cv_in*(P_feed - P_av)
+                u_max = Q_feed/self._A/epsi
+                u_vel = u_max*(1-z/L)
+                if u_max > 0:
+                    F_feed = Q_feed*(P_feed/Rgas/T_feed)*1E5
+                else:
+                    F_feed = Q_feed*(P_av/Rgas/T_feed)*1E5
+                
+                #Q_feed = P_av0*
+                for ii in range(n_comp-1):
+                    y_tmp = np.array(y[ii*N:(ii+1)*N])
+                    y_tmp[y_tmp<1E-6] = 0
+                    dy_tmp = self._d@y_tmp
+                    ddy_tmp = self._dd@y_tmp
+                    P_part_tmp = y_tmp*P_av
+                    #y_tmp[y_tmp<1E-6] = 0
+                    y_comp.append(y_tmp)
+                    P_part.append(P_part_tmp)
+                    dy_comp.append(dy_tmp)
+                    ddy_comp.append(ddy_tmp)
+
+                y_rest = 1-np.sum(y_comp, 0)
+                P_part.append(P_av*y_rest)
+                #print('Shape of P_part[0]',P_part[0].shape)
+                q = []
+                for ii in range(n_comp-1, 2*n_comp-1):
+                    q.append(y[ii*N:(ii+1)*N])
+                # Solid uptake component
+                dqdt = []
+                qstar = self._iso(P_part,T_feed)
+                for ii in range(n_comp):
+                    dqdt_tmp = k_mtc[ii]*a_surf*(qstar[ii] - q[ii])
+                    dqdt.append(dqdt_tmp)
+                # Solid uptake total
+                Sig_dqdt = np.sum(dqdt, 0)
+                dqdt_av = np.sum(Sig_dqdt)/len(Sig_dqdt)
+                
+                # dCdt: 1st derv term of average overall gas concentration 
+                dCdt = 1/epsi/V_tot*F_feed -(1-epsi)/epsi*rho_s*dqdt_av
+                dy_compdt = []
+                for ii in range(n_comp-1):
+                    term1 = -u_vel*dy_comp[ii]
+                    term2 = D_AB[ii]*0 # How to calculate d(yC)dz
+                    term3 = -rho_s*(1-epsi)/epsi*dqdt[ii]
+                    term4 = 0
+                    term5 = +y_comp[ii]*rho_s*Sig_dqdt*(1-epsi)/epsi
+                    
+                    #term1[0] = 0
+                    term1[0] = u_vel[0]*self._d[1,1]*(y_feed[ii]-y_comp[ii][0])
+                    #term5[0] = 0
+                    #term1[-1] = -u_feed*d[1,1]*C[-1]*(y_comp[ii][-2]-y_comp[ii][-1])
+                    #term3[-1] = 0
+                    #term5[-1] = 0
+
+                    #dydt_tmp = term1+(term2 + term3+ term4 + term5)/C
+                    dydt_tmp = term1 + term3/C + term5/C
+                    #dydt_tmp[0] = 0
+                    #dydt_tmp[N-1] = 0 
+                    #ind_both = ((y_comp[ii]<1E-6) + (dydt_tmp < 0))>1.5
+                    #dydt_tmp[ind_both] = 0 
+                    dy_compdt.append(dydt_tmp) # dy_i/dt i = 1,2, ...
+
+                dydt = []
+                for yy in dy_compdt:
+                    dydt.append(yy)
+                    #print(yy.shape)
+                for qq in dqdt:
+                    dydt.append(qq)
+                    #print(qq.shape)
+                dydt.append([dCdt])
+                dydt_arr = np.concatenate(dydt)
+                
+                return dydt_arr
+            
+            # Initial value again
+            y0 = np.zeros(N*(n_comp*2-1)+1)
+            for ii in range(n_comp-1):
+                y0[ii*N : (ii+1)*N] = self._y_init[ii]
+                y0[(n_comp-1+ii)*N : (n_comp+ii)*N]= self._q_init[ii]
+            y0[2*(n_comp-1)*N : 2*(n_comp-1)*N+N] = self._q_init[-1]
+            y0[(2*n_comp-1)*N] = C_av0
+
+            # BACKWARD FLOW !! Flip initial conditions #
+            if self._required['Flow direction'] == 'Backward':
+                y0_tmp = []
+                for ii in range(2*n_comp-1):
+                    mat_y0_pre_tmp = y0[ii*N:(ii+1)*N]
+                    mat_y0_rev_tmp = self._A_flip@mat_y0_pre_tmp
+                    y0_tmp.append(mat_y0_rev_tmp)
+                y0_tmp.append([y0[-1]])
+                y0_rev = np.concatenate(y0_tmp)
+                y0 = y0_rev
+                
+            # Solve ode
+            y_result = odeint(massbal_linvel, y0, t_dom)
+
+            # BACKWARD FLOW !! Flip the results#
+            if self._required['Flow direction'] == 'Backward':
+                y_tmp = []
+                q_tmp = []
+                for ii in range(n_comp-1):
+                    mat_y_tmp = y_result[:, ii*N : (ii+1)*N]
+                    mat_q_tmp = y_result[:, (n_comp-1+ii)*N : (n_comp+ii)*N]
+                    y_tmp.append(mat_y_tmp@self._A_flip)
+                    q_tmp.append(mat_q_tmp@self._A_flip)
+                mat_q_tmp = y_result[:, (2*n_comp-2)*N:(2*n_comp-1)*N]
+                q_tmp.append(mat_q_tmp@self._A_flip)
+                y_flip = np.concatenate(y_tmp+q_tmp + [y_result[:,-1:]], axis = 1)
+                y_result = y_flip
+
+            C_t_dom = y_result[:, -1]
+            C_tmp = []
+            q_tmp = []
+            y_tmp = []
+            mat_y_rest = np.zeros([len(t_dom), N])
+            for ii in range(n_comp-1):
+                mat_y_tmp = y_result[:, ii*N:(ii+1)*N]
+                mat_q_tmp = y_result[:, (n_comp-1+ii)*N : (n_comp+ii)*N]
+                mat_C_tmp = np.diag(C_t_dom)@mat_y_tmp
+                
+                C_tmp.append(mat_C_tmp)
+                q_tmp.append(mat_q_tmp)
+                y_tmp.append(mat_y_tmp)
+                mat_y_rest = mat_y_rest + mat_y_tmp
+
+            C_tmp.append(np.diag(C_t_dom)@(1- mat_y_rest))
+            q_tmp.append(y_result[:, (2*n_comp-2)*N: (2*n_comp-1)*N])
+
+            self._y_fra = y_tmp
+
+            Tg_tmp = T_feed*np.ones([len(t_dom), N])
+            Ts_tmp = T_feed*np.ones([len(t_dom), N])
+            y_result = np.concatenate(C_tmp + q_tmp + [Tg_tmp, Ts_tmp], axis=1)
+            self._y = y_result
+            self._t = t_dom
+
+            toc = time.time()/60 - tic
+            self._CPU_min = toc
+            if CPUtime_print:
+                print('Simulation of this step is completed.')
+                print('This took {0:9.3f} mins to run. \n'.format(toc))
+
+            return y_result, self._z, t_dom
+        
+        # Depressurization (=Blowdown) (Open outlet only)
+        elif (self._Cv_in < 1E-10) and (self._Cv_out > 1E-10): 
+            # Initial Pressure and initial overal concentration
+            Rgas = 8.3145   # J/mol/K
+            P_av0 = np.mean(self._P_init)
+            C_av0 = P_av0*1E5/R_gas/T_feed   # mol/m^3
+            # Mass transfer
+            k_mtc = self._k_mtc
+            D_AB = self._D_disp
+            a_surf = self._a_surf
+
+            def massbal_linvel(y,t):
+                y_comp = []
+                P_part = []
+                dy_comp = []
+                ddy_comp = []
+                C = y[(2*n_comp-1)*N]
+                P_av = C*Rgas*T_feed/1E5   # mol/m^3
+                Q_feed = self._Cv_out*(P_av - P_out)
+                u_max = Q_feed/self._A/epsi
+                u_vel = u_max*z/L
+                if u_max > 0:
+                    F_feed = Q_feed*(P_av/Rgas/T_feed)*1E5
+                else:
+                    F_feed = Q_feed*(P_out/Rgas/T_feed)*1E5
+                
+                #Q_feed = P_av0*
+                for ii in range(n_comp-1):
+                    y_tmp = np.array(y[ii*N:(ii+1)*N])
+                    y_tmp[y_tmp<1E-6] = 0
+                    dy_tmp = self._d@y_tmp
+                    ddy_tmp = self._dd@y_tmp
+                    P_part_tmp = y_tmp*P_av
+                    #y_tmp[y_tmp<1E-6] = 0
+                    y_comp.append(y_tmp)
+                    P_part.append(P_part_tmp)
+                    dy_comp.append(dy_tmp)
+                    ddy_comp.append(ddy_tmp)
+
+                y_rest = 1-np.sum(y_comp, 0)
+                P_part.append(P_av*y_rest)
+                q = []
+                for ii in range(n_comp-1, 2*n_comp-1):
+                    q.append(y[ii*N:(ii+1)*N])
+                # Solid uptake component
+                dqdt = []
+                qstar = self._iso(P_part,T_feed)
+                for ii in range(n_comp):
+                    dqdt_tmp = k_mtc[ii]*a_surf*(qstar[ii] - q[ii])
+                    dqdt.append(dqdt_tmp)
+                # Solid uptake total
+                Sig_dqdt = np.sum(dqdt, 0)
+                dqdt_av = np.sum(Sig_dqdt)/len(Sig_dqdt)
+                
+                # dCdt: 1st derv term of average overall gas concentration 
+                dCdt = -1/epsi/V_tot*F_feed -(1-epsi)/epsi*rho_s*dqdt_av
+                dy_compdt = []
+                for ii in range(n_comp-1):
+                    term1 = -u_vel*dy_comp[ii]
+                    term2 = D_AB[ii]*0 # How to calculate d(yC)dz
+                    term3 = -rho_s*(1-epsi)/epsi*dqdt[ii]
+                    term4 = 0
+                    term5 = +y_comp[ii]*rho_s*Sig_dqdt*(1-epsi)/epsi
+                    
+                    term1[0] = 0
+                    # Because u_vel[0] = 0 ... 
+                    # [???] term1[0] = u_vel[0]*self._d[1,1]*(y_feed[ii]-y_comp[ii][0])
+
+                    #term5[0] = 0
+                    #term1[-1] = -u_feed*d[1,1]*C[-1]*(y_comp[ii][-2]-y_comp[ii][-1])
+                    #term3[-1] = 0
+                    #term5[-1] = 0
+
+                    #dydt_tmp = term1+(term2 + term3+ term4 + term5)/C
+                    dydt_tmp = term1 + term3/C + term5/C
+                    #dydt_tmp[0] = 0
+                    #dydt_tmp[N-1] = 0 
+                    #ind_both = ((y_comp[ii]<1E-6) + (dydt_tmp < 0))>1.5
+                    #dydt_tmp[ind_both] = 0 
+                    dy_compdt.append(dydt_tmp) # dy_i/dt i = 1,2, ...
+
+                dydt = []
+                for yy in dy_compdt:
+                    dydt.append(yy)
+                    #print(yy.shape)
+                for qq in dqdt:
+                    dydt.append(qq)
+                    #print(qq.shape)
+                dydt.append([dCdt])
+                dydt_arr = np.concatenate(dydt)
+                
+                return dydt_arr
+            
+            # Initial value again
+            y0 = np.zeros(N*(n_comp*2-1)+1)
+            for ii in range(n_comp-1):
+                y0[ii*N : (ii+1)*N] = self._y_init[ii]
+                y0[(n_comp-1+ii)*N : (n_comp+ii)*N]= self._q_init[ii]
+            y0[2*(n_comp-1)*N : 2*(n_comp-1)*N+N] = self._q_init[-1]
+            y0[(2*n_comp-1)*N] = C_av0
+            
+            # BACKWARD FLOW !! Flip initial conditions #
+            if self._required['Flow direction'] == 'Backward':
+                y0_tmp = []
+                for ii in range(2*n_comp-1):
+                    mat_y0_pre_tmp = y0[ii*N:(ii+1)*N]
+                    mat_y0_rev_tmp = self._A_flip@mat_y0_pre_tmp
+                    y0_tmp.append(mat_y0_rev_tmp)
+                y0_tmp.append([y0[-1]])
+                y0_rev = np.concatenate(y0_tmp)
+                y0 = y0_rev
+                
+            # Solve ode
+            y_result = odeint(massbal_linvel, y0, t_dom)
 
+            # BACKWARD FLOW !! Flip the results#
+            if self._required['Flow direction'] == 'Backward':
+                y_tmp = []
+                q_tmp = []
+                for ii in range(n_comp-1):
+                    mat_y_tmp = y_result[:, ii*N : (ii+1)*N]
+                    mat_q_tmp = y_result[:, (n_comp-1+ii)*N : (n_comp+ii)*N]
+                    y_tmp.append(mat_y_tmp@self._A_flip)
+                    q_tmp.append(mat_q_tmp@self._A_flip)
+                mat_q_tmp = y_result[:, (2*n_comp-2)*N:(2*n_comp-1)*N]
+                q_tmp.append(mat_q_tmp@self._A_flip)
+                y_flip = np.concatenate(y_tmp+q_tmp + [y_result[:,-1:]], axis = 1)
+                y_result = y_flip
+
+            C_t_dom = y_result[:, -1]
+            C_tmp = []
+            q_tmp = []
+            y_tmp = []
+            mat_y_rest = np.zeros([len(t_dom), N])
+            for ii in range(n_comp-1):
+                mat_y_tmp = y_result[:, ii*N:(ii+1)*N]
+                mat_q_tmp = y_result[:, (n_comp-1+ii)*N : (n_comp+ii)*N]
+                mat_C_tmp = np.diag(C_t_dom)@mat_y_tmp
+                
+                C_tmp.append(mat_C_tmp)
+                q_tmp.append(mat_q_tmp)
+                y_tmp.append(mat_y_tmp)
+                mat_y_rest = mat_y_rest + mat_y_tmp
+
+            C_tmp.append(np.diag(C_t_dom)@(1- mat_y_rest))
+            q_tmp.append(y_result[:, (2*n_comp-2)*N: (2*n_comp-1)*N])
+
+            self._y_fra = y_tmp
+
+            Tg_tmp = T_feed*np.ones([len(t_dom), N])
+            Ts_tmp = T_feed*np.ones([len(t_dom), N])
+            y_result = np.concatenate(C_tmp + q_tmp + [Tg_tmp, Ts_tmp], axis=1)
+            self._y = y_result
+            self._t = t_dom
 
+            toc = time.time()/60 - tic
+            self._CPU_min = toc
+            if CPUtime_print:
+                print('Simulation of this step is completed.')
+                print('This took {0:9.3f} mins to run. \n'.format(toc))
+
+            return y_result, self._z, t_dom
+            
+            
+        
+        
+
+        
 
 
+
+#### P equalization ??? ####
 def step_P_eq_alt1(column1, column2, t_max,
 n_sec=5, Cv_btw=0.1, valve_select = [1,1], CPUtime_print = False):
     tic = time.time() / 60 # in minute
     P_sum1 = np.mean(column1._P_init)
     P_sum2 = np.mean(column2._P_init)
     P_mean = (P_sum1+P_sum2)/2
     T_mean = (np.mean(column1._Tg_init)+np.mean(column2._Tg_init))/2
@@ -2490,17 +3023,14 @@
     else:
         column1._y = y_res1
         column2._y = y_res2
         column1._Tg_res = y_res1[:,n_comp*2*N1 : n_comp*2*N1+N1]
         column2._Tg_res = y_res2[:,n_comp*2*N2 : n_comp*2*N2+N2]
         return [[y_res1,column1._z, t_dom], [y_res2,column2._z, t_dom]]
 
-
-
-
 def step_P_eq(column1, column2, t_max,
 n_sec=5, Cv_btw=0.1, valve_select = [1,1], CPUtime_print = False):
     tic = time.time() / 60 # in minute
     P_sum1 = np.mean(column1._P_init)
     P_sum2 = np.mean(column2._P_init)
     if P_sum1 > P_sum2:
         c1_tmp = column1.copy()
@@ -2842,32 +3372,114 @@
         return [[y_res2,column1._z, t_dom], [y_res1,column2._z, t_dom]]
     else:
         column1._y = y_res1
         column2._y = y_res2
         column1._Tg_res = y_res1[:,n_comp*2*N1 : n_comp*2*N1+N1]
         column2._Tg_res = y_res2[:,n_comp*2*N2 : n_comp*2*N2+N2]
         return [[y_res1,column1._z, t_dom], [y_res2,column2._z, t_dom]]
+
+    
     
 # %% When only this code is run (name == main)
 if __name__ == '__main__':
+    N = 101
+    
+    D = 0.2
+    A_cros = D**2/4*np.pi
+    epsi = 0.4      # m^3/m^3
+    rho_s = 1000    # kg/m^3
+    dp = 0.02       # m (particle diameter)
+    mu = [1.81E-5, 1.81E-5, 1.81E-5] # Pa sec (visocisty of gas)
+    #mu_av = 1.81E-5
+    n_comp = 3
+    
+    # Column Geometry
+    L = 1
+    D = 0.2
+    N = 101
+    A_cros = D**2/4*np.pi
+    epsi = 0.4      # m^3/m^3
+    # Define a column    
+    n_comp = 3
+    c1 = column(L, A_cros,n_comp, N, E_balance=False)
+
+    # Adsorbent info
+    def isomix(P_in,T):
+        pp = []
+        for ii in range(len(P_in)):
+            p_tmp = P_in[ii][:]
+            #ind_tmp = P_in[ii] < 1E-4
+            #p_tmp[ind_tmp] = 0
+            pp.append(p_tmp)
+        q1 = 1*pp[0]*0.1/(1 + 0.1*pp[0] + 0.3*pp[1] + 0.4*pp[2])
+        q2 = 3*pp[1]*0.3/(1 + 0.1*pp[0] + 0.3*pp[1] + 0.4*pp[2])
+        q3 = 4*pp[2]*0.4/(1 + 0.1*pp[0] + 0.3*pp[1] + 0.4*pp[2])
+        return [q1, q2, q3]
+    c1.adsorbent_info(isomix, epsi, dp, rho_s,)
+    
+    # Gas properties
+    Mw = [28, 32, 44]
+    c1.gas_prop_info(Mw,mu)
+
+    # Mass transfer
+    k_MTC = [2.5, 2.5, 20.5]
+    D_disp = [1E-7, 1E-7, 1E-7] 
+    a_surf = 1
+    c1.mass_trans_info(k_MTC, a_surf, D_disp)
+
+    # Boundary conditions
+    P_out = 1.2
+    P_in = 1.7 # Ignore this
+    T_in = 300
+    y_in = [0.45, 0.3, 0.25]
+    Cv_in = 5E-3        # m^3/sec/bar
+    Cv_out = 5E-3       # m^3/sec/bar
+    u_feed = 0.1            # m/s
+    Q_in = u_feed*A_cros*epsi  # volumetric flowrate
+    c1.boundaryC_info(P_out, P_in, T_in, y_in, Cv_in,Cv_out,Q_in, 
+                      assigned_v_option = True, foward_flow_direction=True)
+    # Initial conditions
+    P_init = 2*np.ones([N,])
+    
+    y_init = [0.75*np.ones([N,]),
+              0.25*np.ones([N,]),
+              0.00*np.ones([N,])]
+    P_part = [0.75*np.ones([N,])*P_init,
+              0.25*np.ones([N,])*P_init,
+              0.00*np.ones([N,])*P_init]
+    Tg_init = 300*np.ones([N,])
+    Ts_init = 300*np.ones([N,])
+    q1,q2,q3 = isomix(P_part, Tg_init)
+    q_init = [q1,q2,q3]
+
+    c1.initialC_info(P_init, Tg_init, Ts_init, y_init, q_init )
+    print(c1)
+    
+    y_res, z_res, t_res = c1.run_ma_linvel(100,10)
+    c1.Graph(20, 0)
+
+    '''
     N = 11
     A_cros = 0.031416
     L = 1
     c1 = column(L,A_cros, n_component = 2,N_node = N)
     '''
+    '''
     dP = np.linspace(-100, 100)
     M_m_test  = [0.044, 0.028]      ## molar mass    (kg/mol)
     mu_test = [1.47E-5, 1.74E-5]    ## gas viscosity (Pa sec)
     D_particle_dia = 0.01   # particle diameter (m)
     epsi_test = 0.4         # macroscopic void fraction (m^3/m^3)
     v_test = Ergun_test(dP,M_m_test[0],mu_test[0],D_particle_dia,epsi_test)
     plt.plot(dP,v_test)
     plt.grid()
     plt.show()
     '''
+
+    '''
     ## Adsorbent
     isopar1 = [3.0, 1]
     isopar2 = [1.0, 0.5]
     def iso_fn_test(P,T):
         b1 = isopar1[1]*np.exp(30E3/8.3145*(1/T-1/300))
         b2 = isopar2[1]*np.exp(20E3/8.3145*(1/T-1/300))
         denom = 1 + b1*P[0] + b2*P[1]
@@ -2934,14 +3546,16 @@
     c1.next_init()
 
     c1.boundaryC_info(Pout_test,Pin_test,Tin_test,yin_test,
     0.0*Cvin_test,Cvout_test,Q_in_test,False, foward_flow_direction=True)
     c2.boundaryC_info(Pout_test,Pin_test,Tin_test,yin_test,
     0.0*Cvin_test,0,Q_in_test,False, foward_flow_direction=True)
     '''
+
+    '''
     step_P_eq(
         c1,c2,100,n_sec = 50,
         valve_select = [1,1],
         Cv_btw=0.05,CPUtime_print=True)
     plt.show()
     Legend_loc = [1.15, 0.9]
     c1.Graph_P(10, loc = Legend_loc)
```

### Comparing `pyapep-0.1.2/pyapep/simsep_backup.py` & `pyapep-0.1.3/pyAPEP/simsep_backup.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.2/setup.py` & `pyapep-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open('README', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name='pyapep',
-        version='0.1.2',
+        version='0.1.3',
         author_email='sgasga@ulsan.ac.kr',
         description='Python package for adsorption process simulations',
         long_description_content_type='text/markdown',
-        url='https://nahyeonan.github.io/pyAPEP/build/html/index.html',
+        url='https://sebygaa.github.io/pyAPEP/',
         packages=setuptools.find_packages(),
         classifieres=[
             'Programming Language :: Python :: 3',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             ],
         python_requires='>=3.6',
```

