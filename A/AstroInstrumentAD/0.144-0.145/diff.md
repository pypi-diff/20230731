# Comparing `tmp/AstroInstrumentAD-0.144.tar.gz` & `tmp/AstroInstrumentAD-0.145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroInstrumentAD-0.144.tar", last modified: Fri Jul 28 14:17:28 2023, max compression
+gzip compressed data, was "AstroInstrumentAD-0.145.tar", last modified: Mon Jul 31 11:18:19 2023, max compression
```

## Comparing `AstroInstrumentAD-0.144.tar` & `AstroInstrumentAD-0.145.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 14:17:28.769009 AstroInstrumentAD-0.144/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 14:17:28.768188 AstroInstrumentAD-0.144/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    16791 2023-07-28 14:15:46.000000 AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 14:17:28.768878 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.144/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-28 14:17:28.769073 AstroInstrumentAD-0.144/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.144/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-28 14:17:28.769300 AstroInstrumentAD-0.144/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1711 2023-07-28 14:17:08.000000 AstroInstrumentAD-0.144/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 11:18:19.217567 AstroInstrumentAD-0.145/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 11:18:19.216712 AstroInstrumentAD-0.145/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21226 2023-07-31 11:17:43.000000 AstroInstrumentAD-0.145/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.145/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 11:18:19.217437 AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-31 11:18:19.000000 AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 11:18:19.000000 AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 11:18:19.000000 AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 11:18:19.000000 AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 11:18:19.000000 AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.145/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-31 11:18:19.217629 AstroInstrumentAD-0.145/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.145/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 11:18:19.217833 AstroInstrumentAD-0.145/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1711 2023-07-31 11:17:53.000000 AstroInstrumentAD-0.145/setup.py
```

### Comparing `AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.145/AstroInstrumentAD/dispersion_analysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,23 +21,40 @@
         'temperature':10, #deg C
         'humidity':14.5, #%
         'pressure':750.0 #mBa
         }
         
         self.config.update(kwargs)
         
+        #note: for a slit spectrograph, this relative_plate_PA_angle becomes vital. will need to implement a slit aperture using "width" and "height",
+        #and implement 
+        
     def load_wavelengths(self,wavelengths=[]):
         """
+        Input the wavelengths to find the atmospheric dispersion effects for
 
+        ### Parameters
+        wavelengths : list of floats
+            Simulation wavelengths in units of micro-meters (um)
         """
         self.output['wavelengths']=np.array(wavelengths)
 
     def load_hour_angles(self,HA_start=0,HA_end=1,declination=-30):
         """
+        Determine the observation details: hour angle start, end, and declination
+        
+        This information is used to calculate the airmasses and parallatic angles the observation occurs over
         
+        ### Parameters
+        HA_start : float
+            Observation starting hour angle
+        HA_end : float
+            Observation ending hour angle
+        declination : float
+            Declination of the observation, units of degrees
         """
         HA_range=np.linspace(HA_start,HA_end,self.config['HA_intervals'])
         self.input['HA_range']=HA_range
         self.input['declination']=declination
 
         #latitude needs to be negative for now
         lat = float(self.config['latitude']) * np.pi/180
@@ -60,14 +77,27 @@
 
         self.input['ZA_range']=diff_func.airmass_to_ZA(airmasses)
         
         para_angles=diff_func.parallatic_angle(np.array(HA_range),dec,lat)
         self.output['raw_para_angles']=np.array(para_angles) #actual PAs    
         
     def calculate_integration_shifts(self, guide_wavelength=0, aperture_wavelength=0):
+        """
+        Calculates the shift for each wavelength for an integration simulation
+        
+        These are dependent on two reference wavelengths, 1) the guide wavelength the telescope operates on, which
+        remains fixed on the focal plane, and 2) the aperture wavelength the aperture is positioned on. They are calculated
+        using the Fillipenko 1982 model
+        
+        ### Parameters
+        guide_wavelength : float
+            Observation's guide wavelength
+        aperture_wavelength : float
+            Wavelength the aperture is centred on (by default this refers to dispersion half-way through the integration)
+        """
         self.input['guide_wavelength']=guide_wavelength
         self.input['aperture_wavelength']=aperture_wavelength
 
         airmasses=self.output['airmasses']
         wavelengths=self.output['wavelengths']
 
         #centring refers to the index of the hour angles at which we centre the aperture/guiding on a wavelength
@@ -101,15 +131,25 @@
         centre_shift_para=[-centre_shift*np.sin(centring_q),-centre_shift*np.cos(centring_q)]
         centre_shift_para=[centre_shift_para[0]*np.cos(phi)-centre_shift_para[1]*np.sin(phi),
                            centre_shift_para[1]*np.cos(phi)+centre_shift_para[0]*np.sin(phi)]
         self.output['centre_shift']=centre_shift_para
         
     def load_PSFs(self,PSF_type="moffat",moffat_beta=2.5):
         """
+        Determine the PSF form for use in the transmission calculations
+        
+        These will be generated with airmass and wavelength dependences
         
+        ## Parameters
+        PSF_type : string, default = "moffat"
+            Form of the PSF to use in the simulations. Can be one of moffat, gaussian.
+        
+        ## Extra-Parameters
+        moffat_beta : float, default = 2.5
+            The power value of the moffat PSF
         """
         self.input['PSF_type']=PSF_type
         all_PSFs=[]
         all_aligned_PSFs=[]
         
         zero_shifts=np.zeros(np.shape(self.output['shifts'][0]))
 
@@ -121,14 +161,27 @@
             all_PSFs.append(PSFs)
             all_aligned_PSFs.append(aligned_PSFs)
 
         self.output['PSFs']=all_PSFs
         self.output['aligned_PSFs']=all_aligned_PSFs
         
     def load_aperture(self,aperture_major_axis=0,aperture_type="hexagons",hexagon_radius=1):
+        """
+        Define the spectrograph aperture to use in transmisson calculations
+        
+        ## Parameters
+        aperture_major_axis : float
+            major axis length of the aperture, units of arcseconds
+        aperture_type: string
+            The type of aperture to use in the simulation, can be one of hexagons, circle, (TBD: slit, square?)
+        
+        ## Extra-Parameters
+        hexagon_radius : int, default = 1
+            The number of rings in the hexagons aperture array
+        """
         self.input['aperture_major_axis']=aperture_major_axis
         aperture=diff_func.make_aperture(aperture_type,aperture_major_axis,self.config,hexagon_radius=hexagon_radius)
         self.output['aperture']=aperture
         
     def calculate_integration_transmissions(self):
         convolved_arrays=self.output['PSFs']*self.output['aperture']
         convolved_aligned_arrays=self.output['aligned_PSFs']*self.output['aperture']
@@ -147,17 +200,23 @@
         raw_integration_transmissions=np.mean(raw_transmissions,axis=0)
         self.output['raw_integration_transmissions']=raw_integration_transmissions
         self.output['no_AD_integration_transmissions']=no_AD_integration_transmissions
         self.output['relative_integration_transmissions']=relative_integration_transmissions
 
     def integration_plots(self,y_axis='relative',track_indexes=[0,-1]):
         """
-        Function to illustrate simulation results
+        Illustrates simulation results with two graphs:
         1) Transmission vs wavelength curves for individual fibres and entire bundle
         2) Track plot of monochromatic spot PSFs on the aperture over an integration
+        
+        ## Extra-Parameters
+        y_axis : string, default "relative"
+            Set to "relative" for transmissions to be relative to no-AD, and "raw" for raw transmissions
+        track_indexes : list of floats, default [0,-1]
+            Airmass indexes to plot on the track plot
         """
         plt.style.use('bmh')
         fig=plt.figure(figsize=[7,5])
         if y_axis=='relative':
             y_axis_data=self.output['relative_integration_transmissions']
             plt.axhline(y=1,label='No AD Transmission, {}'.format(self.input['PSF_type']),color='black',linestyle='--')
             plt.ylabel("Transmission Relative to No-AD")
@@ -190,83 +249,72 @@
                 xs.append(shifts[o][i][0])
                 ys.append(shifts[o][i][1]) 
             plt.plot(xs,ys,marker='x',color=cmap.to_rgba(weights[count]),label="{}um".format(round(self.output['wavelengths'][i],4)))
         plt.legend()
         plt.xlabel("x (arcsec)")
         plt.ylabel("y (arcsec)")
 
-    def load_ZA(self, ZA_range=[]):
-        """
-        """
-        airmasses=diff_func.ZA_to_airmass(ZA_range)
-        self.output['airmasses']=airmasses
-        self.input['ZA_range']=ZA_range
-    
-    def calculate_snapshot_shifts(self,aperture_wavelength):
-        self.input['aperture_wavelength']=aperture_wavelength
-    
-        airmasses=self.output['airmasses']
-        wavelengths=self.output['wavelengths']
-        
-        shifts=[]
-        for count,airmass in enumerate(airmasses):
-            centre_shift=diff_func.diff_shift(aperture_wavelength,airmass,1,self.config)
-            airmass_shifts=diff_func.diff_shift(wavelengths,airmass,1,self.config)-centre_shift
-            airmass_shifts=np.append(np.resize(airmass_shifts,(len(airmass_shifts),1)),np.zeros((len(airmass_shifts),1)),axis=-1)
-            shifts.append(airmass_shifts)
-        self.output['shifts']=shifts
-        
-    def calculate_snapshot_transmissions(self):
-        convolved_arrays=self.output['PSFs']*self.output['aperture']
-        convolved_aligned_arrays=self.output['aligned_PSFs']*self.output['aperture']
-        self.output['PSFs_through_aperture']=convolved_arrays
-        self.output['aligned_PSFs_through_aperture']=convolved_aligned_arrays
 
-        raw_transmissions=np.sum(convolved_arrays,axis=(-1,-2))
-        no_AD_transmissions=np.sum(convolved_aligned_arrays,axis=(-1,-2))
-        relative_transmissions=raw_transmissions/no_AD_transmissions
-        self.output['raw_transmissions']=raw_transmissions
-        self.output['no_AD_transmissions']=no_AD_transmissions
-        self.output['relative_transmissions']=relative_transmissions
+    
+    def run(self,HA_start=0,HA_end=1,declination=-30,wavelengths=[],aperture_major_axis=[],guide_wavelength=0,aperture_wavelength=0,**kwargs):
+        """
+        A simple but limited way to run an atmospheric dispersion simulation
         
-    def snapshot_plots(self,y_axis='relative'):
-        plt.style.use('bmh')
-        fig=plt.figure(figsize=[7,5])
-        if y_axis=='relative':
-            y_data=self.output['relative_transmissions']
-            plt.axhline(y=1,label='No AD Transmission, {}'.format(self.input['PSF_type']),color='black',linestyle='--')
-            plt.ylabel("Transmission Relative to No-AD")
-        if y_axis=='raw':
-            y_data=self.output['raw_transmissions']
-            plt.ylabel("Raw Transmission")
+        By default, the guide and aperture will be optimised to the nearest 0.1um - add an input other than 0 for custom values. 
+        The simulation in this setup is a circular fibre with atmopsheric moffat PSFs
         
-        plt.axvline(self.input['aperture_wavelength'],label="Aperture = {}um".format(self.input['aperture_wavelength']),color='C0',linestyle='--',linewidth=0.5)
-        for count,trans in enumerate(y_data):
-            plt.plot(self.output['wavelengths'],trans,label="ZA = {} deg".format(round(self.input['ZA_range'][count],1)))
-        plt.ylabel("Transmission Relative to No-AD")
-        plt.ylim(0,1.1)
-        plt.xlabel("Wavelength (um)")
-        plt.legend()   
-    
-    def run(self,HA_start=0,HA_end=1,declination=-30,wavelengths=[],aperture_major_axis=[],guide_wavelength=0,aperture_wavelength=0,aperture_type="hexagons",hexagon_radius=1,PSF_type="moffat",moffat_beta=2.5,y_axis="relative",track_indexes=[0,-1],**kwargs):
+        ## Parameters
+        HA_start : float
+            Observation starting hour angle
+        HA_end : float
+            Observation ending hour angle
+        declination : float
+            Declination of the observation, units of degrees
+        wavelengths : list of floats
+            Simulation wavelengths in units of micro-meters (um)
+        aperture_major_axis : float
+            major axis length of the aperture, units of arcseconds
+
+        ## Extra-Parameters
+        guide_wavelength : float, default = 0
+            Observation's guide wavelength
+        aperture_wavelength : float, default = 0
+            Wavelength the aperture is centred on (by default this refers to dispersion half-way through the integration) 
+               
+        """
         self.config.update(kwargs)
         self.load_hour_angles(HA_start=HA_start,HA_end=HA_end,declination=declination)
         self.load_wavelengths(wavelengths=wavelengths)
-        self.load_aperture(aperture_major_axis=aperture_major_axis)
+        self.load_aperture(aperture_major_axis=aperture_major_axis,aperture_type="circle")
         if guide_wavelength==0 or aperture_wavelength ==0:
             print("Optimising Guide/Aperture Wavelength")
             self.optimise_integration(np.arange(wavelengths[0],wavelengths[-1],0.1),np.arange(wavelengths[0],wavelengths[-1],0.1),guide_aperture="equal")
             print("Optimal Guide/Aperture = {}um (nearest 0.1um)".format(self.input['guide_wavelength']))
         else:
             self.calculate_integration_shifts(guide_wavelength=guide_wavelength,aperture_wavelength=aperture_wavelength)
             self.load_PSFs()
             self.calculate_integration_transmissions()
         self.integration_plots()
             
     def optimise_integration(self,guide_options=[],aperture_options=[],guide_aperture="independent"):
+        """
+        Optimise the aperture and guide wavelengths transmission curves
+        
+        The metric optimised is the minimum transmission multiplied by the throughput squared
+        
+        ## Parameters
+        guide_options : list of floats
+            Guide wavelength values to iterate over
+        aperture_options : list of floats
+            Aperture wavelength values to iterate over
+            
+        ## Extra-Parameters
+        guide_aperture : string
+            If "independent", the guide and aperture wavelength values can be different. If "equal" they are are set equal.
+        """
         if guide_aperture=="independent":
             metrics=np.zeros((len(guide_options),len(aperture_options),3))
             performance_metrics=np.zeros((len(guide_options),len(aperture_options),3))
             best_performance_metric=0
             for guide_count,guide in enumerate(guide_options):
                 for aperture_count,aperture in enumerate(aperture_options):
                     self.calculate_integration_shifts(guide_wavelength=guide,aperture_wavelength=aperture)
@@ -309,8 +357,67 @@
         print("Max Transmission = {}%".format(round(100*best_metric[1])))
         print("Throughput = {}%".format(round(100*best_metric[2])))
          
         self.calculate_integration_shifts(round(best_guide,5),round(best_aperture,5))
         self.load_PSFs()
         self.calculate_integration_transmissions()
  
-        return
+        return
+    
+    def load_ZA(self, ZA_range=[]):
+        """
+        """
+        airmasses=diff_func.ZA_to_airmass(ZA_range)
+        self.output['airmasses']=airmasses
+        self.input['ZA_range']=ZA_range
+    
+    def calculate_snapshot_shifts(self,aperture_wavelength):
+        """
+        """
+        self.input['aperture_wavelength']=aperture_wavelength
+    
+        airmasses=self.output['airmasses']
+        wavelengths=self.output['wavelengths']
+        
+        shifts=[]
+        for count,airmass in enumerate(airmasses):
+            centre_shift=diff_func.diff_shift(aperture_wavelength,airmass,1,self.config)
+            airmass_shifts=diff_func.diff_shift(wavelengths,airmass,1,self.config)-centre_shift
+            airmass_shifts=np.append(np.resize(airmass_shifts,(len(airmass_shifts),1)),np.zeros((len(airmass_shifts),1)),axis=-1)
+            shifts.append(airmass_shifts)
+        self.output['shifts']=shifts
+        
+    def calculate_snapshot_transmissions(self):
+        """
+        """
+        convolved_arrays=self.output['PSFs']*self.output['aperture']
+        convolved_aligned_arrays=self.output['aligned_PSFs']*self.output['aperture']
+        self.output['PSFs_through_aperture']=convolved_arrays
+        self.output['aligned_PSFs_through_aperture']=convolved_aligned_arrays
+
+        raw_transmissions=np.sum(convolved_arrays,axis=(-1,-2))
+        no_AD_transmissions=np.sum(convolved_aligned_arrays,axis=(-1,-2))
+        relative_transmissions=raw_transmissions/no_AD_transmissions
+        self.output['raw_transmissions']=raw_transmissions
+        self.output['no_AD_transmissions']=no_AD_transmissions
+        self.output['relative_transmissions']=relative_transmissions
+        
+    def snapshot_plots(self,y_axis='relative'):
+        """
+        """
+        plt.style.use('bmh')
+        fig=plt.figure(figsize=[7,5])
+        if y_axis=='relative':
+            y_data=self.output['relative_transmissions']
+            plt.axhline(y=1,label='No AD Transmission, {}'.format(self.input['PSF_type']),color='black',linestyle='--')
+            plt.ylabel("Transmission Relative to No-AD")
+        if y_axis=='raw':
+            y_data=self.output['raw_transmissions']
+            plt.ylabel("Raw Transmission")
+        
+        plt.axvline(self.input['aperture_wavelength'],label="Aperture = {}um".format(self.input['aperture_wavelength']),color='C0',linestyle='--',linewidth=0.5)
+        for count,trans in enumerate(y_data):
+            plt.plot(self.output['wavelengths'],trans,label="ZA = {} deg".format(round(self.input['ZA_range'][count],1)))
+        plt.ylabel("Transmission Relative to No-AD")
+        plt.ylim(0,1.1)
+        plt.xlabel("Wavelength (um)")
+        plt.legend()
```

### Comparing `AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.145/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.145/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.144
+Version: 0.145
 Summary: A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
```

### Comparing `AstroInstrumentAD-0.144/PKG-INFO` & `AstroInstrumentAD-0.145/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.144
+Version: 0.145
 Summary: A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
```

### Comparing `AstroInstrumentAD-0.144/setup.py` & `AstroInstrumentAD-0.145/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.144',      # Start with a small number and increase it with every change you make
+  version = '0.145',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
   keywords = ['Astronomy', 'Instrumentation', 'Atmospheric Dispersion'],   # Keywords that define your package best
```

