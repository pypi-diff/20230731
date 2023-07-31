# Comparing `tmp/AstroInstrumentAD-0.146.tar.gz` & `tmp/AstroInstrumentAD-0.147.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Jay.Stephan/Library/CloudStorage/OneDrive-ScienceandTechnologyFacilitiesCouncil/Documents/General/AD/Package/dist/.tmp-8", last modified: Mon Jul 31 14:17:37 2023, max compression
+gzip compressed data, was "/Users/Jay.Stephan/Library/CloudStorage/OneDrive-ScienceandTechnologyFacilitiesCouncil/Documents/General/AD/Package/dist/.tmp-g", last modified: Mon Jul 31 14:20:48 2023, max compression
```

## Comparing `AstroInstrumentAD-0.146.tar` & `AstroInstrumentAD-0.147.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21226 2023-07-31 11:17:43.000000 AstroInstrumentAD-0.146/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.146/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      725 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.146/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      725 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.146/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 14:17:37.000000 AstroInstrumentAD-0.146/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1722 2023-07-31 14:17:09.000000 AstroInstrumentAD-0.146/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21104 2023-07-31 14:20:41.000000 AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.147/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.147/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1732 2023-07-31 14:20:42.000000 AstroInstrumentAD-0.147/setup.py
```

### Comparing `AstroInstrumentAD-0.146/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,33 +26,35 @@
         self.config.update(kwargs)
         
         #note: for a slit spectrograph, this relative_plate_PA_angle becomes vital. will need to implement a slit aperture using "width" and "height",
         #and implement 
         
     def load_wavelengths(self,wavelengths=[]):
         """
-        Input the wavelengths to find the atmospheric dispersion effects for
+        Input the desired simulation wavelengths.
+        
+        Shifts and transmissions will be calculated for these wavelengths.
 
         ### Parameters
         wavelengths : list of floats
-            Simulation wavelengths in units of micro-meters (um)
+            Simulation wavelengths, units of micrometers (um)
         """
         self.output['wavelengths']=np.array(wavelengths)
 
     def load_hour_angles(self,HA_start=0,HA_end=1,declination=-30):
         """
-        Determine the observation details: hour angle start, end, and declination
+        Input the observation parameters.
         
-        This information is used to calculate the airmasses and parallatic angles the observation occurs over
+        This calculates the airmasses and parallatic angles for the observation.
         
         ### Parameters
         HA_start : float
-            Observation starting hour angle
+            Starting hour angle
         HA_end : float
-            Observation ending hour angle
+            Ending hour angle
         declination : float
             Declination of the observation, units of degrees
         """
         HA_range=np.linspace(HA_start,HA_end,self.config['HA_intervals'])
         self.input['HA_range']=HA_range
         self.input['declination']=declination
 
@@ -78,25 +80,25 @@
         self.input['ZA_range']=diff_func.airmass_to_ZA(airmasses)
         
         para_angles=diff_func.parallatic_angle(np.array(HA_range),dec,lat)
         self.output['raw_para_angles']=np.array(para_angles) #actual PAs    
         
     def calculate_integration_shifts(self, guide_wavelength=0, aperture_wavelength=0):
         """
-        Calculates the shift for each wavelength for an integration simulation
+        Calculates the shift for each wavelength during an integration.
         
-        These are dependent on two reference wavelengths, 1) the guide wavelength the telescope operates on, which
-        remains fixed on the focal plane, and 2) the aperture wavelength the aperture is positioned on. They are calculated
-        using the Fillipenko 1982 model
+        This are dependent on two reference wavelengths, 1) the guide wavelength the telescope operates on, which
+        remains fixed on the focal plane, and 2) the aperture wavelength the aperture is positioned on. Shifts calculated
+        using the Fillipenko 1982 model.
         
         ### Parameters
         guide_wavelength : float
-            Observation's guide wavelength
+            Observation's guide wavelength, units of micrometers (um)
         aperture_wavelength : float
-            Wavelength the aperture is centred on (by default this refers to dispersion half-way through the integration)
+            Wavelength the aperture is centred on (by default this refers to dispersion half-way through the integration), units of micrometers (um)
         """
         self.input['guide_wavelength']=guide_wavelength
         self.input['aperture_wavelength']=aperture_wavelength
 
         airmasses=self.output['airmasses']
         wavelengths=self.output['wavelengths']
 
@@ -131,21 +133,21 @@
         centre_shift_para=[-centre_shift*np.sin(centring_q),-centre_shift*np.cos(centring_q)]
         centre_shift_para=[centre_shift_para[0]*np.cos(phi)-centre_shift_para[1]*np.sin(phi),
                            centre_shift_para[1]*np.cos(phi)+centre_shift_para[0]*np.sin(phi)]
         self.output['centre_shift']=centre_shift_para
         
     def load_PSFs(self,PSF_type="moffat",moffat_beta=2.5):
         """
-        Determine the PSF form for use in the transmission calculations
+        Determine the PSF form.
         
-        These will be generated with airmass and wavelength dependences
+        These will be generated with airmass and wavelength dependences.
         
         ## Parameters
         PSF_type : string, default = "moffat"
-            Form of the PSF to use in the simulations. Can be one of moffat, gaussian.
+            Form of the PSF to use in the simulations. Can be one of "moffat", "gaussian".
         
         ## Extra-Parameters
         moffat_beta : float, default = 2.5
             The power value of the moffat PSF
         """
         self.input['PSF_type']=PSF_type
         all_PSFs=[]
@@ -162,21 +164,21 @@
             all_aligned_PSFs.append(aligned_PSFs)
 
         self.output['PSFs']=all_PSFs
         self.output['aligned_PSFs']=all_aligned_PSFs
         
     def load_aperture(self,aperture_major_axis=0,aperture_type="hexagons",hexagon_radius=1):
         """
-        Define the spectrograph aperture to use in transmisson calculations
+        Define the spectrograph aperture.
         
         ## Parameters
         aperture_major_axis : float
             major axis length of the aperture, units of arcseconds
         aperture_type: string
-            The type of aperture to use in the simulation, can be one of hexagons, circle, (TBD: slit, square?)
+            The aperture shape to use in the simulation, can be one of "hexagons", "circle", (TBD: slit, square?)
         
         ## Extra-Parameters
         hexagon_radius : int, default = 1
             The number of rings in the hexagons aperture array
         """
         self.input['aperture_major_axis']=aperture_major_axis
         aperture=diff_func.make_aperture(aperture_type,aperture_major_axis,self.config,hexagon_radius=hexagon_radius)
@@ -201,22 +203,22 @@
         self.output['raw_integration_transmissions']=raw_integration_transmissions
         self.output['no_AD_integration_transmissions']=no_AD_integration_transmissions
         self.output['relative_integration_transmissions']=relative_integration_transmissions
 
     def integration_plots(self,y_axis='relative',track_indexes=[0,-1]):
         """
         Illustrates simulation results with two graphs:
-        1) Transmission vs wavelength curves for individual fibres and entire bundle
-        2) Track plot of monochromatic spot PSFs on the aperture over an integration
+        1) Transmission vs wavelength curves for individual fibres and entire bundle.
+        2) Track plot of monochromatic spot PSFs on the aperture over an integration.
         
         ## Extra-Parameters
         y_axis : string, default "relative"
             Set to "relative" for transmissions to be relative to no-AD, and "raw" for raw transmissions
         track_indexes : list of floats, default [0,-1]
-            Airmass indexes to plot on the track plot
+            Indexes of the wavelengths to use on the track plot
         """
         plt.style.use('bmh')
         fig=plt.figure(figsize=[7,5])
         if y_axis=='relative':
             y_axis_data=self.output['relative_integration_transmissions']
             plt.axhline(y=1,label='No AD Transmission, {}'.format(self.input['PSF_type']),color='black',linestyle='--')
             plt.ylabel("Transmission Relative to No-AD")
@@ -253,28 +255,28 @@
         plt.xlabel("x (arcsec)")
         plt.ylabel("y (arcsec)")
 
 
     
     def run(self,HA_start=0,HA_end=1,declination=-30,wavelengths=[],aperture_major_axis=[],guide_wavelength=0,aperture_wavelength=0,**kwargs):
         """
-        A simple but limited way to run an atmospheric dispersion simulation
+        A simple in-built (but limited) atmospheric dispersion simulation.
         
-        By default, the guide and aperture will be optimised to the nearest 0.1um - add an input other than 0 for custom values. 
-        The simulation in this setup is a circular fibre with atmopsheric moffat PSFs
+        The guide and aperture will be optimised to the nearest 0.1um if values are not input.
+        The simulation in this setup is a circular fibre with atmopsheric moffat PSFs.
         
         ## Parameters
         HA_start : float
-            Observation starting hour angle
+            Starting hour angle
         HA_end : float
-            Observation ending hour angle
+            Ending hour angle
         declination : float
             Declination of the observation, units of degrees
         wavelengths : list of floats
-            Simulation wavelengths in units of micro-meters (um)
+            Simulation wavelengths, units of micrometers (um)
         aperture_major_axis : float
             major axis length of the aperture, units of arcseconds
 
         ## Extra-Parameters
         guide_wavelength : float, default = 0
             Observation's guide wavelength
         aperture_wavelength : float, default = 0
@@ -293,17 +295,17 @@
             self.calculate_integration_shifts(guide_wavelength=guide_wavelength,aperture_wavelength=aperture_wavelength)
             self.load_PSFs()
             self.calculate_integration_transmissions()
         self.integration_plots()
             
     def optimise_integration(self,guide_options=[],aperture_options=[],guide_aperture="independent"):
         """
-        Optimise the aperture and guide wavelengths transmission curves
+        Optimise the aperture and guide wavelengths.
         
-        The metric optimised is the minimum transmission multiplied by the throughput squared
+        The metric optimised is the transmission curve's minimum multiplied by the throughput squared.
         
         ## Parameters
         guide_options : list of floats
             Guide wavelength values to iterate over
         aperture_options : list of floats
             Aperture wavelength values to iterate over
```

### Comparing `AstroInstrumentAD-0.146/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.146/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.146
+Version: 0.147
 Summary: A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE.txt
+
+README.md
```

### Comparing `AstroInstrumentAD-0.146/PKG-INFO` & `AstroInstrumentAD-0.147/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.146
+Version: 0.147
 Summary: A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE.txt
+
+README.md
```

### Comparing `AstroInstrumentAD-0.146/setup.py` & `AstroInstrumentAD-0.147/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.146',      # Start with a small number and increase it with every change you make
+  version = '0.147',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
-  readme='README.md',
+  long_description='README.md',
   keywords = ['Astronomy', 'Instrumentation', 'Atmospheric Dispersion'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'matplotlib',
           'astropy',
           'scipy',
       ],
```

