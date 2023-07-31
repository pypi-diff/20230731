# Comparing `tmp/plot-antenna-1.6.tar.gz` & `tmp/plot-antenna-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-antenna-1.6.tar", last modified: Wed May 31 14:48:06 2023, max compression
+gzip compressed data, was "plot-antenna-1.7.tar", last modified: Mon Jul 31 16:46:23 2023, max compression
```

## Comparing `plot-antenna-1.6.tar` & `plot-antenna-1.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.841402 plot-antenna-1.6/
--rw-r--r--   0 ralf      (1000) priv      (1011)    11232 2023-05-31 14:48:06.841402 plot-antenna-1.6/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     9024 2023-05-31 14:46:42.000000 plot-antenna-1.6/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.809402 plot-antenna-1.6/plot_antenna/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-31 14:47:28.000000 plot-antenna-1.6/plot_antenna/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.6/plot_antenna/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    51994 2023-05-31 07:31:41.000000 plot-antenna-1.6/plot_antenna/plot_antenna.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.833402 plot-antenna-1.6/plot_antenna.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)    11232 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-31 14:48:06.000000 plot-antenna-1.6/plot_antenna.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-31 14:48:06.841402 plot-antenna-1.6/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.6/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-31 14:48:06.837402 plot-antenna-1.6/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.6/test/test_plot.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-31 16:46:23.457515 plot-antenna-1.7/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1357 2023-07-26 16:30:04.000000 plot-antenna-1.7/LICENSE
+-rw-r--r--   0 ralf      (1000) priv      (1011)    11307 2023-07-31 16:46:23.457515 plot-antenna-1.7/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10463 2023-07-31 16:43:51.000000 plot-antenna-1.7/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-31 16:46:23.421515 plot-antenna-1.7/plot_antenna/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-07-31 16:46:20.000000 plot-antenna-1.7/plot_antenna/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.7/plot_antenna/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    75270 2023-07-31 16:07:47.000000 plot-antenna-1.7/plot_antenna/plot_antenna.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-31 16:46:23.445515 plot-antenna-1.7/plot_antenna.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    11307 2023-07-31 16:46:23.000000 plot-antenna-1.7/plot_antenna.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      356 2023-07-31 16:46:23.000000 plot-antenna-1.7/plot_antenna.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-07-31 16:46:23.000000 plot-antenna-1.7/plot_antenna.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       64 2023-07-31 16:46:23.000000 plot-antenna-1.7/plot_antenna.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)      120 2023-07-31 16:46:23.000000 plot-antenna-1.7/plot_antenna.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-07-31 16:46:23.000000 plot-antenna-1.7/plot_antenna.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2709 2023-07-28 11:44:13.000000 plot-antenna-1.7/pyproject.toml
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-07-31 16:46:23.457515 plot-antenna-1.7/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2836 2023-07-28 11:46:33.000000 plot-antenna-1.7/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-31 16:46:23.449515 plot-antenna-1.7/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    21451 2023-07-31 16:39:30.000000 plot-antenna-1.7/test/test_plot.py
```

### Comparing `plot-antenna-1.6/PKG-INFO` & `plot-antenna-1.7/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,215 +1,227 @@
-Metadata-Version: 2.1
-Name: plot-antenna
-Version: 1.6
-Summary: Antenna plotting program for plotting antenna simulation results
-Home-page: https://github.com/schlatterbeck/plot-antenna
-Author: Ralf Schlatterbeck
-Author-email: rsc@runtux.com
-License: MIT License
-Description: Antenna Plotting Program
-        ========================
-        
-        :Author: Ralf Schlatterbeck <rsc@runtux.com>
-        
-        .. |--| unicode:: U+2013   .. en dash
-        .. |__| unicode:: U+2013   .. en dash without spaces
-            :trim:
-        .. |_| unicode:: U+00A0 .. Non-breaking space
-            :trim:
-        .. |-| unicode:: U+202F .. Thin non-breaking space
-            :trim:
-        
-        This is a program to plot antenna-related data resulting from an antenna
-        simulation. It can read the text output produced by nec2c_ and my
-        python mininec port pymininec_. Most notably it can plot antenna
-        far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
-        graphic that can be rotated and zoomed). It supports a local display
-        program (using matplotlib_) and a HTML output version that displays
-        everything using javascript (using plotly_). The program features a
-        ``--help`` option. If the program called with ``--help`` does not
-        display a ``-H`` or ``--export-html`` option, you most likely do not
-        have a recent version of plotly_ installed. In that case only the
-        matplotlib_ variant is available. For the plotly variant to work you
-        need both, a recent version of plotly_ as well as pandas_ installed.
-        
-        The program started out as a companion-program to my pymininec_
-        project and is now an independent program.
-        
-        The plot program can also display output files of nec2c_, not only
-        from pymininec_.
-        
-        Standalone Plotting with Matplotlib
-        -----------------------------------
-        
-        The default is to plot all available
-        graphics, including an interactive 3d view. In addition with the
-        ``--azimuth`` or ``--elevation`` options you can get an Azimuth
-        diagram::
-        
-            plot-antenna --azimuth test/12-el-1deg.pout
-        
-        .. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-azimuth.png
-            :align: center
-        
-        or an elevation diagram::
-        
-            plot-antenna --elevation test/12-el-1deg.pout
-        
-        .. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-elevation.png
-            :align: center
-        
-        respectively. Note that I used an output file with 1-degree resolution
-        in elevation and azimuth angles not with 5 degrees as in the example
-        above. The pattern look smoother but a 3D-view will be very slow due to
-        the large number of points. The plot program also has a ``--help``
-        option for further information. In particular the scaling of the antenna
-        plot can be selected using the ``--scaling-method`` option with an
-        additional keyword which can be one of ``linear``, ``linear_db``, and
-        ``linear_voltage`` in addition to the default of ``arrl`` scaling. You
-        may consult Cebik's [1]_ article for explanation of the different
-        diagrams. The ``linear_voltage`` option is not explained by Cebik, it is
-        in-between the ``linear`` and ``linear_db`` scaling options.
-        
-        The latest version accepts several plot parameters, ``--elevation``,
-        ``--azimuth``, ``--plot3d``, ``--plot-vswr``, and ``--geo`` which are
-        plotted into one diagram. The default is to plot the first four graphs.
-        With the ``--output`` option pictures can directly be saved without
-        displaying the graphics on the screen. Note that unfortunately the
-        geometry display with the ``--geo`` option does not perform very well
-        because matplotlib_ has poor support for panning and scaling in 3D
-        plots.
-        
-        The latest version has key-bindings for scrolling through the
-        frequencies of an antenna simulation. So if you have an output file with
-        a simulation of multiple frequencies (either with pymininec_ or
-        nec2c_) you can display diagrams for the next frequency by typing
-        ``+``, and to the previous frequency by typing ``-``. For newer versions
-        of matplotlib_ you can display a scrollbar for the frequencies with
-        the ``--with-slider`` option.
-        
-        Other keybindings switch the scaling for the antenna plots, ``a``
-        switches to ``arrl`` scaling, ``l`` switches to linear scaling, ``d``
-        switches to linear dB scaling, and ``v`` switches to linear voltage
-        scaling.
-        
-        Finally the ``w`` key toggles display of the 3d diagram from/to
-        wireframe display. Note that the wireframe display may not be supported
-        on all versions of matplotlib_ and/or graphics cards.
-        
-        Plotting for the Browser with Plotly
-        ------------------------------------
-        
-        All the plot supported for matplotlib_ are also supported with plotly_.
-        These are ``--elevation``, ``--azimuth``, ``--plot3d``, ``--plot-vswr``,
-        and ``--geo``. The plots can be either exported to a .html file using
-        the ``-H`` or ``--export-html`` option (with an additional filename to
-        export to) or injected into a running browser using the ``-S`` or
-        ``--show-in-browser`` option.
-        
-        Unlike for matplotlib_, each plot selected with an option is either
-        shown in a separate window in the browser or exported to a separate
-        file. If exporting to a file, additional output options can be selected
-        with the ``--html-export-option`` setting. The default is to export the
-        file with all javascript included (adds about 3MB to the file size).
-        With ``--html-export-option=directory`` the javascript is not included
-        and a ``plotly.min.js`` file is expected in the same directory as the
-        exported file. This file ships with the plotly_ distribution. When
-        exporting to a file, the plot name is appended to the file name given,
-        this allows export to several different plots in one program invocation.
-        
-        The scaling variants selected with the ``--scaling-method`` option
-        cannot currently be changed at runtime with the plotly_ plots. As with
-        matplotlib_, the default is ``arrl`` scaling.
-        
-        All plots are interactive. For the far-field pattern
-        plots (Azimuth, Elevation, 3D) frequencies can be selected in the legend
-        to the right of the plot. With mouse-over you can see the current angle
-        (Elevation or Azimuth with the 2D plots and both for the 3D plot) and
-        the gain at that point. For the 2D variants, more than one frequency can
-        be selected for plotting. This allows comparison of pattern between
-        different frequencies. For the 3D plot, the frequencies in the legend
-        act like radio-buttons, only one at a time can be selected.
-        
-        With the ``--geo`` option you get a display of the antenna geometry.
-        Unfortunately plotly_ seems to have limitations on the zoom depths, so
-        for large antennas it is not possible to see the plot in deep detail. As
-        of this writing not all geometry details are displayed. In particular 2D
-        patches in NEC, transmission lines in NEC, and visualization of loaded
-        segments (e.g. with a capacity) are not shown.
-        
-        .. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
-            In Antenna Modeling Notes [2], chapter 48, pages 366–379. Available
-            in Cebik's `Antenna modelling notes episode 48`_
-        .. [2] L. B. Cebik. Antenna Modeling Notes, volume 2. antenneX Online
-            Magazine, 2003. Available with antenna models from the `Cebik
-            collection`_.
-        
-        .. _`Cebik collection`:
-            http://on5au.be/Books/allmodnotes.zip
-        .. _`Antenna modelling notes episode 48`:
-            http://on5au.be/content/amod/amod48.html
-        .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
-        .. _pymininec: https://github.com/schlatterbeck/pymininec
-        .. _matplotlib: https://matplotlib.org/
-        .. _plotly: https://github.com/plotly/plotly.py
-        .. _pandas: https://pandas.pydata.org/
-        
-        Release Notes
-        -------------
-        
-        v1.6: More SWR plot changes
-        
-        - Make SWR-plot vertical line colors configurable
-        - Rename elevation-angle and azimuth-angle options to angle-elevation
-          and angle-azimuth so that we can again request an elevation/azimuth
-          plot with shortened options like --ele or --azi
-        - Sort options lexicographically on --help
-        
-        v1.5: Allow target SWR frequency in VSWR plot
-        
-        - Add command-line option --target-swr-frequency
-        - Draw user-specifed target frequency in red, best (minimum) swr in grey
-        
-        v1.4: Reset button and VSWR-Plot improvements
-        
-        - Add grid and minimum-SWR vertical line to VSWR plot
-        - Remove display of frequency in mouse-over (in polar plots and 3D plot)
-        - Make polar reset button reset more parameters
-        
-        v1.3: Add a reset button to plotly polar plots
-        
-        - The polar plots, when zoomed in, could only be reset to the unzoomed
-          view with a double-click. All other plots do have a reset button, add
-          one for the polar plots, too.
-        
-        v1.2: Allow specification of title (legend) font size in plotly version
-        
-        - For some application (e.g. when using the plotly graphics inside a
-          html iframe) the title (or we may want to call it legend) of the
-          graphics may collide with the graphics itself. We can now specify the
-          font size with ``--title-font-size``. This option currently works only
-          with plotly graphics.
-        
-        v1.1: Specification of azimuth / elevation angle
-        
-        - Now we can specify an azimuth angle for elevation plot and an
-          elevation angle for azimuth plots.
-        - Bug-fix in computation of maximum gain azimuth direction: If the
-          maximum gain in theta direction goes up or down, the azimuth angle
-          would be computed incorrectly because all gain values at that theta
-          angle are the same for all azimuth angles.
-        - Sort options: Since there are some options that only exist when some
-          packages are installed we sort options instead of trying to add them
-          in the correct order.
-        
-        v1.0: Initial Release
-        
-Platform: Any
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Other Audience
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Antenna Plotting Program
+========================
+
+:Author: Ralf Schlatterbeck <rsc@runtux.com>
+
+.. |--| unicode:: U+2013   .. en dash
+.. |__| unicode:: U+2013   .. en dash without spaces
+    :trim:
+.. |_| unicode:: U+00A0 .. Non-breaking space
+    :trim:
+.. |-| unicode:: U+202F .. Thin non-breaking space
+    :trim:
+
+This is a program to plot antenna-related data resulting from an antenna
+simulation. It can read the text output produced by nec2c_ and my
+python mininec port pymininec_. Most notably it can plot antenna
+far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
+graphic that can be rotated and zoomed). It supports a local display
+program (using matplotlib_) and a HTML output version that displays
+everything using javascript (using plotly_). The program features a
+``--help`` option. If the program called with ``--help`` does not
+display a ``-H`` or ``--export-html`` option, you most likely do not
+have a recent version of plotly_ installed. In that case only the
+matplotlib_ variant is available. For the plotly variant to work you
+need both, a recent version of plotly_ as well as pandas_ installed.
+
+The program started out as a companion-program to my pymininec_
+project and is now an independent program.
+
+The plot program can also display output files of nec2c_, not only
+from pymininec_.
+
+Standalone Plotting with Matplotlib
+-----------------------------------
+
+The default is to plot all available
+graphics, including an interactive 3d view. In addition with the
+``--azimuth`` or ``--elevation`` options you can get an Azimuth
+diagram::
+
+    plot-antenna --azimuth test/12-el-1deg.pout
+
+.. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-azimuth.png
+    :align: center
+
+or an elevation diagram::
+
+    plot-antenna --elevation test/12-el-1deg.pout
+
+.. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-elevation.png
+    :align: center
+
+respectively. Note that I used an output file with 1-degree resolution
+in elevation and azimuth angles not with 5 degrees as in the example
+above. The pattern look smoother but a 3D-view will be very slow due to
+the large number of points. The plot program also has a ``--help``
+option for further information. In particular the scaling of the antenna
+plot can be selected using the ``--scaling-method`` option with an
+additional keyword which can be one of ``linear``, ``linear_db``, and
+``linear_voltage`` in addition to the default of ``arrl`` scaling. You
+may consult Cebik's [1]_ article for explanation of the different
+diagrams. The ``linear_voltage`` option is not explained by Cebik, it is
+in-between the ``linear`` and ``linear_db`` scaling options.
+
+The latest version accepts several plot parameters, ``--elevation``,
+``--azimuth``, ``--plot3d``, ``--plot-vswr``, and ``--geo`` which are
+plotted into one diagram. The default is to plot the first four graphs.
+With the ``--output`` option pictures can directly be saved without
+displaying the graphics on the screen. Note that unfortunately the
+geometry display with the ``--geo`` option does not perform very well
+because matplotlib_ has poor support for panning and scaling in 3D
+plots.
+
+The latest version has key-bindings for scrolling through the
+frequencies of an antenna simulation. So if you have an output file with
+a simulation of multiple frequencies (either with pymininec_ or
+nec2c_) you can display diagrams for the next frequency by typing
+``+``, and to the previous frequency by typing ``-``. For newer versions
+of matplotlib_ you can display a scrollbar for the frequencies with
+the ``--with-slider`` option.
+
+Other keybindings switch the scaling for the antenna plots, ``a``
+switches to ``arrl`` scaling, ``l`` switches to linear scaling, ``d``
+switches to linear dB scaling, and ``v`` switches to linear voltage
+scaling.
+
+Finally the ``w`` key toggles display of the 3d diagram from/to
+wireframe display. Note that the wireframe display may not be supported
+on all versions of matplotlib_ and/or graphics cards.
+
+Plotting for the Browser with Plotly
+------------------------------------
+
+All the plot supported for matplotlib_ are also supported with plotly_.
+These are ``--elevation``, ``--azimuth``, ``--plot3d``, ``--plot-vswr``,
+and ``--geo``. The plots can be either exported to a .html file using
+the ``-H`` or ``--export-html`` option (with an additional filename to
+export to) or injected into a running browser using the ``-S`` or
+``--show-in-browser`` option.
+
+Unlike for matplotlib_, each plot selected with an option is either
+shown in a separate window in the browser or exported to a separate
+file. If exporting to a file, additional output options can be selected
+with the ``--html-export-option`` setting. The default is to export the
+file with all javascript included (adds about 3MB to the file size).
+With ``--html-export-option=directory`` the javascript is not included
+and a ``plotly.min.js`` file is expected in the same directory as the
+exported file. This file ships with the plotly_ distribution. When
+exporting to a file, the plot name is appended to the file name given,
+this allows export to several different plots in one program invocation.
+
+The scaling variants selected with the ``--scaling-method`` option
+cannot currently be changed at runtime with the plotly_ plots. As with
+matplotlib_, the default is ``arrl`` scaling.
+
+All plots are interactive. For the far-field pattern
+plots (Azimuth, Elevation, 3D) frequencies can be selected in the legend
+to the right of the plot. With mouse-over you can see the current angle
+(Elevation or Azimuth with the 2D plots and both for the 3D plot) and
+the gain at that point. For the 2D variants, more than one frequency can
+be selected for plotting. This allows comparison of pattern between
+different frequencies. For the 3D plot, the frequencies in the legend
+act like radio-buttons, only one at a time can be selected.
+
+With the ``--geo`` option you get a display of the antenna geometry.
+Unfortunately plotly_ seems to have limitations on the zoom depths, so
+for large antennas it is not possible to see the plot in deep detail. As
+of this writing not all geometry details are displayed. In particular 2D
+patches in NEC, transmission lines in NEC, and visualization of loaded
+segments (e.g. with a capacity) are not shown.
+
+.. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
+    In Antenna Modeling Notes [2], chapter 48, pages 366–379. Available
+    in Cebik's `Antenna modelling notes episode 48`_
+.. [2] L. B. Cebik. Antenna Modeling Notes, volume 2. antenneX Online
+    Magazine, 2003. Available with antenna models from the `Cebik
+    collection`_.
+
+.. _`Cebik collection`:
+    http://on5au.be/Books/allmodnotes.zip
+.. _`Antenna modelling notes episode 48`:
+    http://on5au.be/content/amod/amod48.html
+.. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
+.. _pymininec: https://github.com/schlatterbeck/pymininec
+.. _matplotlib: https://matplotlib.org/
+.. _plotly: https://github.com/plotly/plotly.py
+.. _pandas: https://pandas.pydata.org/
+
+Release Notes
+-------------
+
+v1.7: Add Smith charts, optionally show impedance and band in VSWR plots
+
+Many of the changes in this and several previous versions were suggested
+by Rob Banfield, DM1CM: Adding the bands and impedance to the VSWR plot
+are his idea as well as adding a Smith chart. Due to his attention to
+detail this release corrects a lot of rough edges of previous versions.
+Thanks Rob!
+
+- The aspect ratio in 3D plotly plots is now correct. It used to be a
+  little too wide in the X direction
+- Add Smith chart display
+- Options to add the impedance (either as real/imag or \|Z\|/phi (Z)) in
+  the VSWR plot
+- Option to show the ham radio bands in the VSWR plot
+- Show loads and excitation(s) in geo plot, add ground to geo plot
+- Margin of 3D plots in plotly are much wider now by default and can be
+  configured with an option
+- The style how the gain is displayed in the plotly 3D color bar can now
+  be configured to save space (either relative or absolute gain in dB or
+  dBi, the default is both)
+- When there is only one frequency in the 3D plot, remove the frequency
+  legend
+- Add LICENSE file and pyproject.toml for newer install mechanisms in
+  python
+- Add tests for plotly output
+- Use ppm images for the tests, the previously-used png images did
+  contain the matplotlib version and thus were different for each
+  version -- the ppm images do not have that problem, there are still
+  many differences with different matplotlib versions
+
+v1.6: More SWR plot changes
+
+- Make SWR-plot vertical line colors configurable
+- Rename elevation-angle and azimuth-angle options to angle-elevation
+  and angle-azimuth so that we can again request an elevation/azimuth
+  plot with shortened options like --ele or --azi
+- Sort options lexicographically on --help
+
+v1.5: Allow target SWR frequency in VSWR plot
+
+- Add command-line option --target-swr-frequency
+- Draw user-specifed target frequency in red, best (minimum) swr in grey
+
+v1.4: Reset button and VSWR-Plot improvements
+
+- Add grid and minimum-SWR vertical line to VSWR plot
+- Remove display of frequency in mouse-over (in polar plots and 3D plot)
+- Make polar reset button reset more parameters
+
+v1.3: Add a reset button to plotly polar plots
+
+- The polar plots, when zoomed in, could only be reset to the unzoomed
+  view with a double-click. All other plots do have a reset button, add
+  one for the polar plots, too.
+
+v1.2: Allow specification of title (legend) font size in plotly version
+
+- For some application (e.g. when using the plotly graphics inside a
+  html iframe) the title (or we may want to call it legend) of the
+  graphics may collide with the graphics itself. We can now specify the
+  font size with ``--title-font-size``. This option currently works only
+  with plotly graphics.
+
+v1.1: Specification of azimuth / elevation angle
+
+- Now we can specify an azimuth angle for elevation plot and an
+  elevation angle for azimuth plots.
+- Bug-fix in computation of maximum gain azimuth direction: If the
+  maximum gain in theta direction goes up or down, the azimuth angle
+  would be computed incorrectly because all gain values at that theta
+  angle are the same for all azimuth angles.
+- Sort options: Since there are some options that only exist when some
+  packages are installed we sort options instead of trying to add them
+  in the correct order.
+
+v1.0: Initial Release
```

### Comparing `plot-antenna-1.6/README.rst` & `plot-antenna-1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: plot-antenna
+Version: 1.7
+Summary: Antenna plotting program for plotting antenna simulation results
+Home-page: https://github.com/schlatterbeck/plot-antenna
+Author: Ralf Schlatterbeck
+Author-email: Ralf Schlatterbeck <rsc@runtux.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/schlatterbeck/plot-antenna
+Project-URL: Bug Tracker, https://github.com/schlatterbeck/plot-antenna/issues
+Platform: Any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Other Audience
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
 Antenna Plotting Program
 ========================
 
 :Author: Ralf Schlatterbeck <rsc@runtux.com>
 
 .. |--| unicode:: U+2013   .. en dash
 .. |__| unicode:: U+2013   .. en dash without spaces
@@ -145,14 +167,44 @@
 .. _matplotlib: https://matplotlib.org/
 .. _plotly: https://github.com/plotly/plotly.py
 .. _pandas: https://pandas.pydata.org/
 
 Release Notes
 -------------
 
+v1.7: Add Smith charts, optionally show impedance and band in VSWR plots
+
+Many of the changes in this and several previous versions were suggested
+by Rob Banfield, DM1CM: Adding the bands and impedance to the VSWR plot
+are his idea as well as adding a Smith chart. Due to his attention to
+detail this release corrects a lot of rough edges of previous versions.
+Thanks Rob!
+
+- The aspect ratio in 3D plotly plots is now correct. It used to be a
+  little too wide in the X direction
+- Add Smith chart display
+- Options to add the impedance (either as real/imag or \|Z\|/phi (Z)) in
+  the VSWR plot
+- Option to show the ham radio bands in the VSWR plot
+- Show loads and excitation(s) in geo plot, add ground to geo plot
+- Margin of 3D plots in plotly are much wider now by default and can be
+  configured with an option
+- The style how the gain is displayed in the plotly 3D color bar can now
+  be configured to save space (either relative or absolute gain in dB or
+  dBi, the default is both)
+- When there is only one frequency in the 3D plot, remove the frequency
+  legend
+- Add LICENSE file and pyproject.toml for newer install mechanisms in
+  python
+- Add tests for plotly output
+- Use ppm images for the tests, the previously-used png images did
+  contain the matplotlib version and thus were different for each
+  version -- the ppm images do not have that problem, there are still
+  many differences with different matplotlib versions
+
 v1.6: More SWR plot changes
 
 - Make SWR-plot vertical line colors configurable
 - Rename elevation-angle and azimuth-angle options to angle-elevation
   and angle-azimuth so that we can again request an elevation/azimuth
   plot with shortened options like --ele or --azi
 - Sort options lexicographically on --help
```

### Comparing `plot-antenna-1.6/plot_antenna/plot_antenna.py` & `plot-antenna-1.7/plot_antenna/plot_antenna.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 #!/usr/bin/python3
 
 import sys
 import os
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import numpy as np
+from html import escape
 from bisect import bisect
 from mpl_toolkits.mplot3d import Axes3D
 from argparse import ArgumentParser, HelpFormatter
-from matplotlib import cm, __version__ as matplotlib_version, rcParams
+from matplotlib import cm, __version__ as matplotlib_version, rcParams, ticker
 from matplotlib.widgets import Slider
+from matplotlib.patches import Rectangle
+from smithplot.smithaxes import SmithAxes
 try:
     import plotly.express as px
     import plotly.graph_objects as go
     from plotly.subplots import make_subplots
     import pandas         as pd
 except ImportError:
     px = None
 
 matplotlib_version_float = float ('.'.join (matplotlib_version.split ('.')[:2]))
 
+Omega = "\u2126"
+ohm = ' %s' % Omega
+
+def blend (color, alpha = 0x80, bg = '#FFFFFF'):
+    """ Blend a color with a background color, default white with a
+        given alpha channel, the input color is in #RRGGBB format
+    """
+    alpha = alpha / 255
+    color = np.array ([int (color [n:n+2], 16) for n in range (1, 6, 2)]) / 255
+    bg    = np.array ([int (bg    [n:n+2], 16) for n in range (1, 6, 2)]) / 255
+    rgb   = (((1 - alpha) * bg + alpha * color) * 255).astype (int)
+    return '#%02X%02X%02X' % tuple (rgb)
+# end def blend
+
 class Scaler:
 
     @property
     def tick_values (self):
         g = self.ticks
         return self.scale (0, g)
     # end def tick_values
@@ -145,14 +162,67 @@
         50.00
         """
         return v * -self.min_db + self.min_db
     # end def invscale
 
 # end class Linear_dB_Scaler
 
+class Plot_Range:
+    """ Sensible Y range so that all different Y coordinates can
+        share a grid.
+    """
+
+    def __init__ (self, y, min_y = None):
+        self.max = max (y)
+        self.min = min_y
+        if min_y is None:
+            self.min = min (y)
+        self.exp = int \
+            (np.log (max (abs (self.max), abs (self.min))) / np.log (10))
+        self.max /= 10 ** self.exp
+        self.min /= 10 ** self.exp
+        assert abs (self.max) < 10 and abs (self.min) < 10
+        # round mn to lower int
+        self.min = np.floor (self.min)
+        # round mx to higher int
+        self.max = np.ceil (self.max)
+        self.rng, self.tck = self.compute ()
+    # end def __init__
+
+    def compute (self):
+        for k in 1, 2, 4, 8, 10:
+            if self.max - self.min <= k:
+                rng = np.array ([self.min, self.min + k]) * 10 ** self.exp
+                tck = (k / 4) * 10 ** self.exp
+                return rng, tck
+        rng = np.array ([self.min, self.min + 12]) * 10 ** exp
+        tck = 3 * 10 ** exp
+        return rng, tck
+    # end def compute
+
+    def as_plotly (self):
+        return dict (range = self.rng, dtick = self.tck)
+    # end def as_plotly
+
+    def as_matplot (self):
+        r1, r2 = self.rng
+        t = self.tck
+        return dict (yticks = np.arange (r1, r2 + t, t), ylim = self.rng)
+    # end def as_matplot
+
+    def fmt (self, tail = '', precision = 1):
+        strf  = ticker.FormatStrFormatter
+        fmt = ('%%.%df' % precision) + tail
+        if self.tck == int (self.tck):
+            fmt = '%.0f' + tail
+        return strf (fmt)
+    # end def fmt
+
+# end class Plot_Range:
+
 class Gain_Data:
 
     def __init__ (self, parent, f):
         self.parent   = parent
         self.f        = f
         self.pattern  = {}
     # end def __init__
@@ -266,28 +336,58 @@
     if idx == 0:
         return idx
     if (abs (angles [idx] - dst_angle) < abs (angles [idx - 1] - dst_angle)):
         return idx
     return idx - 1
 # end def nearest_angle_idx
 
+class Loaded_Segment:
+    """ A segment either loaded with an impedance or an excitation
+    """
+
+    by_name = {}
+    nec_types = \
+	[ 'Series RLC, absolute'
+        , 'Parallel RLC, absolute'
+        , 'Series RLC, per m'
+        , 'Parallel RLC, per m'
+        , 'Impedance'
+        , 'Wire conductivity'
+	]
+
+    def __init__ (self, coord, name):
+        self.coord = coord
+        self.name  = name
+        if name not in self.by_name:
+            self.by_name [name] = []
+        self.by_name [name].append (self)
+    # end def __init__
+
+# end class Loaded_Segment
+
 class Gain_Plot:
     fig_x = 512
     fig_y = 384
-    plot_names   = ('azimuth', 'elevation', 'plot_vswr', 'plot3d', 'plot_geo')
+    plot_names   = \
+        ( 'azimuth', 'elevation'
+        , 'plot_vswr', 'plot3d', 'plot_geo', 'plot_smith'
+        )
     update_names = set (('azimuth', 'elevation', 'plot3d'))
     font_sans    = \
         "Helvetica, Nimbus Sans, Liberation Sans, Open Sans, arial, sans-serif"
-
+    # Default colors for swr plot
+    c_real = '#AE4141'
+    c_imag = '#FFB329'
 
     def __init__ (self, args):
         self.args        = args
         self.dpi         = args.dpi
         self.filename    = args.filename
         self.outfile     = args.output_file
+        self.save_format = getattr (args, 'save_format', None)
         self.f           = None
         self.with_slider = args.with_slider
         self.wireframe   = args.wireframe
         self.scalers     = dict \
             ( linear_db      = Linear_dB_Scaler (args.scaling_mindb)
             , linear_voltage = scale_linear_voltage
             , linear         = scale_linear
@@ -297,21 +397,26 @@
         self.cur_scaler = self.scaler
 
         # Discrete values for slider are available only in later
         # matplotlib versions
         if matplotlib_version_float < 3.5:
             self.with_slider = False
         # Default title from filename
-        self.title       = os.path.splitext \
-            (os.path.basename (args.filename)) [0]
+        self.title = os.path.splitext (os.path.basename (args.filename)) [0]
         # This might override title
         self.gdata = {}
         self.geo = []
+        self.seg_by_tag = {}
+        self.segments = []
+        self.has_ground = False
         # This populates gdata:
         self.read_file ()
+        # If there is a title option it wins:
+        if self.args.title:
+            self.title = self.args.title
         self.frequencies = []
         self.maxg = None
         theta_idx = {}
         phi_idx   = {}
         for f in sorted (self.gdata):
             gdata = self.gdata [f]
             gdata.compute ()
@@ -344,14 +449,15 @@
             self.theta_angle_idx = self.theta_maxidx
         if self.outfile or len (self.gdata) == 1 or not self.with_slider:
             self.with_slider = False
         # Borrow colormap from matplotlib to use in plotly
         self.colormap = []
         for cn in mcolors.TABLEAU_COLORS:
             self.colormap.append (mcolors.TABLEAU_COLORS [cn])
+        self.c_vswr = self.colormap [0]
     # end def __init__
 
     @property
     def plotly_polar_default (self):
         d = dict \
             ( layout = dict
                 ( showlegend = True
@@ -387,23 +493,60 @@
     @property
     def plotly_line_default (self):
         d = dict \
             ( layout = dict
                 ( showlegend = True
                 , colorway   = self.colormap
                 , xaxis = dict
-                    ( linecolor = "#B0B0B0"
-                    , gridcolor = "#F2F2F2"
+                    ( linecolor   = "#B0B0B0"
+                    , gridcolor   = "#B0B0B0"
+                    , domain      = [0, 0.9]
+                    #, ticksuffix  = ' MHz'
+                    , tickformat  = '.1f'
+                    , zeroline    = False
                     )
                 , yaxis = dict
-                    ( linecolor = "#B0B0B0"
-                    , gridcolor = "#F2F2F2"
+                    ( color       = self.c_vswr
+                    , linecolor   = self.c_vswr
+                    , showgrid    = True
+                    , gridcolor   = blend (self.c_vswr)
+                    , title       = {}
+		    , anchor      = "x"
+		    , side        = "left"
+                    , hoverformat = '.2f'
+                    , zeroline    = False
+                    )
+                , yaxis2 = dict
+                    ( color       = self.c_real
+                    , linecolor   = self.c_real
+                    , showgrid    = False
+                    , gridcolor   = blend (self.c_real)
+                    , title       = {}
+                    , overlaying  = "y"
+		    , side        = "right"
+		    , anchor      = "x2"
+                    , hoverformat = '.1f'
+                    , zeroline    = False
+                    )
+                , yaxis3 = dict
+                    ( color       = self.c_imag
+                    , linecolor   = self.c_imag
+                    , showgrid    = False
+                    , gridcolor   = blend (self.c_imag)
+                    , title       = {}
+                    , overlaying  = "y"
+		    , side        = "right"
+		    , position    = 0.96
+		    , anchor      = "free"
+                    , hoverformat = '.1f'
+                    , zeroline    = False
                     )
                 , paper_bgcolor = 'white'
                 , plot_bgcolor  = 'white'
+                , hovermode     = 'x unified'
                 )
             )
         return d
     # end def plotly_line_default
 
     @property
     def plotly_3d_default (self):
@@ -413,36 +556,62 @@
         # Ah: This applies only if we do not specify an explicit range
         d = dict \
             ( layout = dict
                 ( showlegend    = True
                 , colorway      = self.colormap
                 , paper_bgcolor = 'white'
                 , plot_bgcolor  = 'white'
+                , margin        = dict
+                    ( l = self.args.margin_3d
+                    , r = self.args.margin_3d
+                    , t = self.args.margin_3d
+                    , b = self.args.margin_3d
+                    )
                 , scene = dict
                     ( xaxis = dict
                         ( linecolor      = "#B0B0B0"
                         , gridcolor      = "#B0B0B0"
                         , showbackground = False
+                        , tickformat     = '.3f'
                         )
                     , yaxis = dict
                         ( linecolor      = "#B0B0B0"
                         , gridcolor      = "#B0B0B0"
                         , showbackground = False
+                        , tickformat     = '.3f'
                         )
                     , zaxis = dict
                         ( linecolor      = "#B0B0B0"
                         , gridcolor      = "#B0B0B0"
                         , showbackground = False
+                        , tickformat     = '.3f'
                         )
+                    , aspectratio = dict (x=1, y=1, z=1)
                     )
                 )
             )
         return d
     # end def plotly_3d_default
 
+    @property
+    def plotly_smith_default (self):
+        d = dict \
+            ( layout = dict
+                ( title = dict
+                    ( font = dict
+                        ( family = self.font_sans
+                        , color  = "#010101"
+                        , size   = 20
+                        )
+                    )
+                )
+            )
+        return d
+    # end def plotly_smith_default
+
     def all_gains (self):
         xyz = None
         for f in self.frequencies:
             g = self.gdata [f]
             _, _, X, Y, Z = g.plot3d_gains (self.scaler)
             if xyz is None:
                 xyz = np.array ([X, Y, Z]).T
@@ -474,33 +643,93 @@
                     continue
                 if  (   line.startswith ('No:       X         Y         Z')
                     and line.endswith ('I-     I    I+   No:')
                     ):
                     status = 'necgeo'
                     necidx = {}
                     continue
+                if line.startswith ('NO. OF SOURCES'):
+                    status = 'source'
+                    continue
+                if line.startswith ('NUMBER OF LOADS'):
+                    status = 'load'
+                    continue
+                if line.startswith ('ENVIRONMENT'):
+                    gp = int (line.split (':', 1) [-1])
+                    self.has_ground = gp < 0
+                if line.startswith ('DATA CARD No:'):
+                    ll = line.split ()
+                    if ll [4] == 'EX':
+                        typ, tag, n = (int (x) for x in ll [5:8])
+                        if typ in (0, 5):
+                            assert n >= 1
+                            name  = 'Excitation'
+                            if tag == 0:
+                                seg = self.segments [n - 1]
+                            else:
+                                seg = self.seg_by_tag [tag][n - 1]
+                            Loaded_Segment (seg, name)
+                    if ll [4] == 'LD':
+                        typ, tag, m, n = (int (x) for x in ll [5:9])
+                        name = Loaded_Segment.nec_types [typ]
+                        if tag == 0:
+                            segs = self.segments
+                        else:
+                            segs = self.seg_by_tag [tag]
+                        if m == 0:
+                            for s in segs:
+                                Loaded_Segment (s, name)
+                        else:
+                            if n == 0:
+                                n = m
+                            for i in range (n, m + 1):
+                                Loaded_Segment (segs [i], name)
+                    if ll [4] == 'GN':
+                        self.has_ground = True
                 if status != 'start' and not line:
                     status  = 'start'
                     continue
                 if status == 'geo':
                     x, y, z, r, e1, e2, n = line.split ()
+                    n = int (n)
+                    self.seg_by_tag [n] = np.array ([x, y, z])
                     self.geo [-1].append ([float (a) for a in (x, y, z)])
                     continue
+                if status == 'load':
+                    if line.startswith ('PULSE'):
+                        txt, l = line.split (':', 1)
+                        tag, r, x = l.split (',')
+                        tag = int (tag)
+                        name = txt.split (',', 1) [-1]
+                        if name == 'RESISTANCE,REACTANCE':
+                            name = 'Impedance'
+                        Loaded_Segment (self.seg_by_tag [tag], name)
+                if status == 'source':
+                    if line.startswith ('PULSE'):
+                        l = line.split (':')[1]
+                        tag, v, p = l.split (',')
+                        tag = int (tag)
+                        Loaded_Segment (self.seg_by_tag [tag], 'Excitation')
                 if status == 'wire':
                     l = line.split ()
                     wires [-1].append ([float (a) for a in l [:3]])
                     continue
                 if status == 'necgeo':
                     # Fixme: This should really be lambda-dependent
                     eps = 1e-3
                     started = False
                     ll = line.split ()
                     idx = int (ll [0])
                     x, y, z, l, alpha, beta = (float (a) for a in ll [1:7])
+                    tag = int (ll [-1])
+                    if tag not in self.seg_by_tag:
+                        self.seg_by_tag [tag] = []
                     mid = np.array ([x, y, z])
+                    self.seg_by_tag [tag].append (mid)
+                    self.segments.append (mid)
                     prev, cur, next = (int (a) for a in ll [8:11])
                     if prev == 0 or abs (prev) > idx:
                         self.geo.append ([])
                         started = True
                     elif abs (prev) != idx - 1:
                         self.geo.append ([])
                         a, b = necidx [abs (prev)]
@@ -624,22 +853,36 @@
                         % locals ()
                         )
                 else:
                     if name in ('azimuth', 'elevation', 'plot3d'):
                         self.plotly_lastfig  = False
                         self.plotly_firstfig = True
                         if name == 'plot3d':
-                            self.plotly_fig = make_subplots \
-                                ( rows=1, cols=2
-                                , specs=[ [ {'type': 'surface'}
-                                          , {'type': 'xy'}
-                                          ]
-                                        ]
-                                , column_widths = [0.8, 0.2]
-                                )
+                            if len (self.frequencies) > 1:
+                                w = 0.035
+                                if self.args.decibel_style == 'both':
+                                    w = 0.1
+                                self.legend_width = w
+                                self.plotly_fig = make_subplots \
+                                    ( rows=1, cols=2
+                                    , specs=[ [ {'type': 'surface'}
+                                              , {'type': 'xy'}
+                                              ]
+                                            ]
+                                    , column_widths = [1-w, w]
+                                    )
+                            else:
+                                self.legend_width = 0
+                                self.plotly_fig = make_subplots \
+                                    ( rows=1, cols=1
+                                    , specs=[ [ {'type': 'surface'}
+                                              ]
+                                            ]
+                                    , column_widths = [1]
+                                    )
                             self.plotly_fig.update (self.plotly_3d_default)
                         else:
                             self.plotly_fig = go.Figure \
                                 (** self.plotly_polar_default)
                         for n, f in enumerate (self.frequencies):
                             self.plotly_count = n
                             self.frequency = f
@@ -663,17 +906,31 @@
         for name in self.plot_names:
             if getattr (self.args, name):
                 p = dict (projection = 'polar')
                 if name == 'plot_vswr':
                     p = {}
                 elif name == 'plot3d' or name == 'plot_geo':
                     p = dict (projection = '3d')
+                elif name == 'plot_smith':
+                    p = dict \
+                        ( projection = 'smith'
+                        , grid_major_fancy  = True
+                        , grid_minor_enable = True
+                        , grid_minor_fancy  = True
+                        , axes_impedance = self.args.system_impedance
+                        , axes_normalize = True
+                        , axes_normalize_label = True
+                        , axes_labelpos = -1.5-1.1j
+                        )
                 d [name] = p
                 a [name] = dict (arg = count + 1)
                 count += 1
+        if len (d) > 4:
+            args       = [2, 3]
+            figsize    = [x * 2 / dpi, y * 3 / dpi]
         if len (d) > 2:
             args       = [2, 2]
             figsize    = [x * 2 / dpi, y * 2 / dpi]
         elif len (d) == 2:
             args       = [1, 2]
             figsize    = [x * 2 / dpi, y / dpi]
         else:
@@ -732,15 +989,18 @@
             kmap = dict (yscale = 'l', all_axes = 'a')
             for k in kmap:
                 try:
                     rcParams ['keymap.' + k].remove (kmap [k])
                 except KeyError:
                     pass
         if self.outfile:
-            fig.savefig (self.outfile)
+            d = {}
+            if self.save_format:
+                d.update (format = self.save_format)
+            fig.savefig (self.outfile, **d)
         else:
             plt.show ()
     # end def plot_matplotlib
 
     def azimuth (self, name):
         self.desc = self.data.azimuth_text (self.scaler)
         self.lbl_deg = self.data.phis_d [self.phi_angle_idx]
@@ -941,57 +1201,67 @@
                         }
                       );"""
 
     def plot3d_plotly (self, name):
         t, gains, X, Y, Z = self.data.plot3d_gains (self.scaler)
         xr, yr, zr = self.scene_ranges ()
         fig = self.plotly_fig
-        ticktext = ['%.2f dBi (%.2f dB)' % (u + self.maxg, u)
-                    for u in self.scaler.ticks
-                   ]
+        if self.args.decibel_style == 'both':
+            ticktext = ['%.2f dBi (%.2f dB)' % (u + self.maxg, u)
+                        for u in self.scaler.ticks
+                       ]
+        elif self.args.decibel_style == 'absolute':
+            ticktext = ['%.2f dBi' % (u + self.maxg) for u in self.scaler.ticks]
+        else:
+            ticktext = ['%.2f dB' % u for u in self.scaler.ticks]
         # Ensure that the uppermost (0dB) mark is printed
         # This may be slightly off when a pattern is very different for
         # different frequencies
         tickvals = self.scaler.tick_values
         tickvals [0] = gains.max ()
         lgroup  = 'l%d' % self.plotly_count
         visible = True if self.plotly_firstfig else 'legendonly'
         tpl = ('Gain: %{customdata[0]:.2f} dBi (%{customdata[1]:.2f} dB)<br>'
                'Azimuth: %{customdata[2]:.2f}° (X: 0°)<br>'
                'Elevation: %{customdata[3]:.2f}°<extra></extra>'
               )
 
+        colorbar_xpos = 1.02
+        if self.legend_width:
+            colorbar_xpos = 0.98 - self.legend_width
         fig.add_trace \
             ( go.Surface
                 ( x = X, y = Y, z = Z
                 , surfacecolor = gains
                 , colorscale   = 'rainbow'
                 , visible      = visible
                 , legendgroup  = lgroup
                 , name         = "f=%.3f MHz" % self.frequency
                 , colorbar = dict
                     ( tickvals = tickvals
                     , ticktext = ticktext
-                    , x = 0.75, y = 0.49
+                    , x = colorbar_xpos, y = 0.49
+                    , xpad = 0
                     )
                 , customdata    = t
                 , hovertemplate = tpl
                 )
             , row = 1, col = 1
             )
-        fig.add_trace \
-            ( go.Scatter
-                ( dict (x = [1.], y = [1.], line = dict (color = 'white'))
-                , legendgroup = lgroup
-                , visible     = visible
-                , showlegend  = True
-                , name        = "f=%.3f MHz" % self.frequency
+        if len (self.frequencies) > 1:
+            fig.add_trace \
+                ( go.Scatter
+                    ( dict (x = [1.], y = [1.], line = dict (color = 'white'))
+                    , legendgroup = lgroup
+                    , visible     = visible
+                    , showlegend  = True
+                    , name        = "f=%.3f MHz" % self.frequency
+                    )
+                , row = 1, col = 2
                 )
-            , row = 1, col = 2
-            )
         if self.plotly_lastfig:
             fig.layout.update \
                 ( legend = dict
                     ( itemclick       = 'toggle'
                     , itemdoubleclick = 'toggle'
                     )
                 , xaxis = dict
@@ -1006,132 +1276,354 @@
                     , zaxis = dict (range = zr, showticklabels = False)
                     )
                 )
             self.show_plotly (fig, name, script = self.plotly_3d_script)
     # end def plot3d_plotly
 
     def prepare_vswr (self):
-        z0 = self.impedance
-        X  = []
-        Y  = []
+        z0   = self.impedance
+        X    = []
+        Y    = []
+        Z    = []
+        imag = []
+        real = []
+        xabs = []
+        xphi = []
         for f in self.gdata:
             gd  = self.gdata [f]
             z   = gd.impedance
             rho = np.abs ((z - z0) / (z + z0))
+            imag.append (z.imag)
+            real.append (z.real)
+            xabs.append (np.abs   (z))
+            xphi.append (np.angle (z) * 180 / np.pi)
             X.append (f)
             Y.append ((1 + rho) / (1 - rho))
+            Z.append (z)
         min_idx = np.argmin (Y)
         self.min_x = X [min_idx]
         if self.args.target_swr_frequency:
             if not X [0] <= self.args.target_swr_frequency <= X [-1]:
                 print \
                     ( "Warning: SWR target frequency %.2f not in range, ignored"
                     % self.args.target_swr_frequency
                     , file = sys.stderr
                     )
                 self.args.target_swr_frequency = None
-        return X, Y
+        self.min_f = min (X)
+        self.max_f = max (X)
+        self.band  = {}
+        for n in self.args.band:
+            fmin, fmax = self.args.band [n]
+            in_band = self.min_f <= fmin <= self.max_f
+            in_band = in_band or self.min_f <= fmax <= self.max_f
+            in_band = in_band or fmin <= self.min_f and self.max_f <= fmax
+            if in_band:
+                self.band [n] = self.args.band [n]
+        return [np.array (v) for v in (X, Y, real, imag, xabs, xphi, Z)]
     # end def prepare_vswr
 
     def plot_vswr_matplotlib (self, name):
         ax = self.axes [name]
-        ax.set_xlabel ('Frequency')
-        ax.set_ylabel ('VSWR')
-        X, Y = self.prepare_vswr ()
-        ax.plot (X, Y)
-        ax.grid (color = '0.95')
+        ax.set_xlabel ('Frequency (MHz)')
+        ax.set_ylabel ('VSWR', color = self.c_vswr)
+        X, Y, real, imag, xabs, xphi, Z = self.prepare_vswr ()
+        strf  = ticker.FormatStrFormatter
+        min_y = min (Y)
+        max_y = max (Y)
+        ax.plot (X, Y, linewidth = 2)
+        ax.grid (color = blend (self.c_vswr), axis = 'y')
+        ax.grid (color = '#B0B0B0', axis = 'x')
+        ax.tick_params (axis = 'y', colors = self.c_vswr)
+        pr = Plot_Range (Y, 1)
+        max_y_r = pr.rng [1]
+        ax.set (**pr.as_matplot ())
+        ax.yaxis.set_major_formatter (pr.fmt ())
+        #ax.xaxis.set_major_formatter (strf ('%.1f MHz'))
         tg = self.args.target_swr_frequency
         if tg is not None:
             c = self.args.swr_target_color
             ax.axvline (x = tg, color = c, linestyle = 'dashed')
         c = self.args.swr_min_color
         if c and c.lower () != 'none':
             ax.axvline (x = self.min_x, color = c, linestyle = 'dashed')
+        if self.args.swr_show_impedance:
+            self.fig.subplots_adjust (right=0.75)
+            ax2 = ax.twinx ()
+            ax3 = ax.twinx ()
+            ax2.tick_params (axis = 'y', colors = self.c_real)
+            ax3.tick_params (axis = 'y', colors = self.c_imag)
+            ax3.spines.right.set_position (("axes", 1.2))
+            if self.args.swr_plot_impedance_angle:
+                ax2.set_ylabel ("|Z|", color = self.c_real)
+                ax2.plot (X, xabs, color = self.c_real, linewidth = 0.9)
+                pr = Plot_Range (xabs)
+                ax2.set (**pr.as_matplot ())
+                ax2.yaxis.set_major_formatter (pr.fmt (ohm))
+                ax3.set_ylabel ("phi (Z)", color = self.c_imag)
+                ax3.plot (X, xphi, color = self.c_imag, linewidth = 0.9)
+                yt = np.arange (-180, 180 + 30, 30)
+                ax3.set (ylim = (-180, 180), yticks = yt)
+                ax3.yaxis.set_major_formatter (strf ('%.0f°'))
+            else:
+                ax2.set_ylabel ("Z (real)", color = self.c_real)
+                ax2.plot (X, real, color = self.c_real, linewidth = 0.9)
+                pr = Plot_Range (real)
+                ax2.set (**pr.as_matplot ())
+                ax2.yaxis.set_major_formatter (pr.fmt (ohm))
+                ax3.set_ylabel ("Z (imag)", color = self.c_imag)
+                ax3.plot (X, imag, color = self.c_imag, linewidth = 0.9)
+                pr = Plot_Range (imag)
+                ax3.set (**pr.as_matplot ())
+                ax3.yaxis.set_major_formatter (pr.fmt (ohm))
+        if self.args.swr_show_bands:
+            y1, y2 = np.array (list (ax.get_ylim ()))
+            for b in self.band:
+                l, h = self.band [b]
+                ax.fill_between ([l, h], y1, y2, color = '#CCFFCC')
+                pos = ((l + h) / 2, 0.90 * max_y_r)
+                ax.annotate \
+                    ( '%s\nband' % b
+                    , xytext = pos
+                    , xy     = pos
+                    , ha     = 'center'
+                    )
     # end def plot_vswr_matplotlib
 
+    def add_plotly_df (self, yname, color = None, axisname = None, **kw):
+        """ Add yname in dataframe self.df to self.fig
+        """
+        d = dict (x = self.df ["Frequency"], y = self.df [yname], name = yname)
+        d.update (line = dict (width = 1.5))
+        d.update (kw)
+        if color:
+            if 'line' in d:
+                d ['line']['color'] = color
+            else:
+                d.update (line = dict (color = color))
+        if axisname:
+            d.update (yaxis = axisname)
+        self.fig.add_trace (go.Scatter (**d))
+    # end def add_plotly_df
+
     def plot_vswr_plotly (self, name):
-        X, Y = self.prepare_vswr ()
+        X, Y, real, imag, xabs, xphi, Z = self.prepare_vswr ()
         df = pd.DataFrame ()
         df ['Frequency'] = X
-        df ['VSWR'] = Y
-        fig = px.line (df, x="Frequency", y="VSWR")
-        fig.update (self.plotly_line_default)
+        df ['VSWR']      = Y
+        df ['Z (real)']  = real
+        df ['Z (imag)']  = imag
+        df ['|Z|']       = xabs
+        df ['phi (Z)']   = xphi
+        self.df = df
+        self.fig = fig = go.Figure ()
+        layout = self.plotly_line_default
+        lstyle = dict (color = self.c_vswr, width = 3.5)
+        self.add_plotly_df ("VSWR", line = lstyle)
+        y = layout ['layout']['yaxis']
+        y.update (**Plot_Range (Y, 1).as_plotly ())
+        layout ['layout']['yaxis']['title'].update  (text = "VSWR")
+        layout ['layout']['xaxis'].update \
+            (title = dict (text = 'Frequency (MHz)'))
+        if self.args.swr_show_impedance:
+            y2 = layout ['layout']['yaxis2']
+            y2 ['ticksuffix'] = ohm
+            y3 = layout ['layout']['yaxis3']
+            if self.args.swr_plot_impedance_angle:
+                self.add_plotly_df ("|Z|", self.c_real, "y2")
+                y2 ['title'].update (text = "|Z|")
+                self.add_plotly_df ("phi (Z)", self.c_imag, "y3")
+                y2.update (**Plot_Range (xabs).as_plotly ())
+                y3 ['title'].update (text = "phi (Z)")
+                y3.update (range = [-180, 180], dtick = 30)
+                y3 ['ticksuffix'] = '°'
+            else:
+                self.add_plotly_df ("Z (real)", self.c_real, "y2")
+                y2 ['title'].update (text = "Z (real)")
+                y2.update (**Plot_Range (real).as_plotly ())
+                self.add_plotly_df ("Z (imag)", self.c_imag, "y3")
+                y3 ['title'].update (text = "Z (imag)")
+                y3.update (**Plot_Range (imag).as_plotly ())
+                y3 ['ticksuffix'] = ohm
+        if self.args.swr_show_bands:
+            shapes = layout ['layout']['shapes'] = []
+            for b in self.band:
+                l, h = self.band [b]
+                d = dict \
+                    ( type       = 'rect'
+                    , yref       = 'paper'
+                    , x0         = max (l, self.min_f)
+                    , y0         = 0
+                    , x1         = min (h, self.max_f)
+                    , y1         = 1
+                    , fillcolor  = '#CCFFCC'
+                    , line_width = 0
+                    , layer      = 'below'
+                    )
+                fig.add_annotation \
+                    ( x         = (l + h) / 2
+                    , y         = 0.98
+                    , yref      = 'paper'
+                    , text      = '<b>%s<br>band</b>' % escape (b)
+                    , showarrow = False
+                    )
+                shapes.append (d)
+        fig.update (layout)
         tg = self.args.target_swr_frequency
         if tg is not None:
             c = self.args.swr_target_color
             fig.add_vline (x = tg, line_dash = "dash", line_color = c)
         c = self.args.swr_min_color
         if c and c.lower () != 'none':
             fig.add_vline (x = self.min_x, line_dash = "dash", line_color = c)
         self.show_plotly (fig, name)
     # end def plot_vswr_plotly
 
-    def scene_ranges (self, matrix = None):
+    def scene_ranges (self, matrix = None, add_ground = False):
         """ Create cubic bounding box to force equal aspect ratio
             If matrix is not given, we concatenate *all* gains.
         """
         if matrix is None:
             matrix = self.all_gains ()
         x, y, z = matrix
+        min_x = x.min ()
+        max_x = x.max ()
+        min_y = y.min ()
+        max_y = y.max ()
+        min_z = z.min ()
+        max_z = z.max ()
+        if add_ground and self.has_ground and min_z > 0:
+            min_z = 0
         max_range = np.array \
-            ( [ x.max () - x.min ()
-              , y.max () - y.min ()
-              , z.max () - z.min ()
-              ]
-            ).max() / 2.0
-        mid_x = (x.max () + x.min ()) / 2
-        mid_y = (y.max () + y.min ()) / 2
-        mid_z = (z.max () + z.min ()) / 2
+            ([ max_x - min_x, max_y - min_y, max_z - min_z ]).max() / 2.0
+        mid_x = (max_x + min_x) / 2
+        mid_y = (max_y + min_y) / 2
+        mid_z = (max_z + min_z) / 2
         xr = np.array ([mid_x - max_range, mid_x + max_range])
         yr = np.array ([mid_y - max_range, mid_y + max_range])
         zr = np.array ([mid_z - max_range, mid_z + max_range])
+        if add_ground and self.has_ground and min_z == 0:
+            zr = np.array ([min_z, min_z + 2 * max_range])
         return np.array ([xr, yr, zr])
     # end def scene_ranges
 
     def plot_geo_plotly (self, name):
-        xr, yr, zr = self.scene_ranges (np.concatenate (self.geo).T)
+        xr, yr, zr = self.scene_ranges (np.concatenate (self.geo).T, True)
         fig = px.line_3d ()
         fig.update (self.plotly_3d_default)
-        # We may want to draw everything in the same color and
-        # remove the individual scatter3d from the legend
-        # but then, maybe not
+        geo = []
         for n, g in enumerate (self.geo):
-            g = np.array (g)
-            d = dict (mode = 'lines', connectgaps = False)
-            d ['x'], d ['y'], d ['z'] = g.T
-            fig.add_scatter3d (**d)
+            if geo:
+                geo.append ([np.nan, np.nan, np.nan])
+            geo.extend (g)
+        geo = np.array (geo)
+        d = dict (mode = 'lines', connectgaps = False, name = 'Geometry')
+        d.update (marker = dict (color = self.colormap [0]))
+        d ['x'], d ['y'], d ['z'] = geo.T
+        fig.add_trace (go.Scatter3d (**d))
+        for i, name in enumerate (sorted (Loaded_Segment.by_name)):
+            segs = Loaded_Segment.by_name [name]
+            coord = []
+            for s in segs:
+                coord.append (s.coord)
+            coord = np.array (coord, dtype = float)
+            x, y, z = coord.T
+            marker = dict (color = self.colormap [i + 1], size = 3)
+            d = dict (marker = marker, name = name, mode = 'markers')
+            fig.add_trace (go.Scatter3d (x = x, y = y, z = z, **d))
         fig.layout.scene.update \
             ( dict
                 ( xaxis = dict (range = xr)
                 , yaxis = dict (range = yr)
                 , zaxis = dict (range = zr)
-                #, domain = dict (x = [0.0, 0.5], y = [0.0, 0.5]) ??
-                , camera = dict
-                    ( up     = dict (x = 0,    y = 0,    z = 1)
-                    , center = dict (x = 0,    y = 0,    z = 0)
-                    , eye    = dict (x = 0.01, y = 0.01, z = 1)
-                    )
                 )
             )
+        if self.has_ground:
+            x, y = np.meshgrid (xr, yr)
+            z = np.zeros (x.shape)
+            d = dict (showscale = False, colorscale = ['#6cbe6c'] * 2)
+            d.update (opacity = 0.9)
+            fig.add_trace (go.Surface (x = x, y = y, z = z, **d))
+        fig.layout.legend = dict (itemsizing = 'constant')
         self.show_plotly (fig, name)
     # end def plot_geo_plotly
 
     def plot_geo_matplotlib (self, name):
         ax = self.axes [name]
         # equal aspect ratio
-        xr, yr, zr = self.scene_ranges (np.concatenate (self.geo).T)
+        xr, yr, zr = self.scene_ranges (np.concatenate (self.geo).T, True)
         ax.set_xlim (*xr)
         ax.set_ylim (*yr)
         ax.set_zlim (*zr)
+        ax.set_xlabel ('X')
+        ax.set_ylabel ('Y')
+        ax.set_zlabel ('Z')
         for g in self.geo:
             g = np.array (g)
             x, y, z = g.T
-            ax.plot (x, y, z)
+            ax.plot (x, y, z, color = self.colormap [0])
+        for i, name in enumerate (sorted (Loaded_Segment.by_name)):
+            segs = Loaded_Segment.by_name [name]
+            coord = []
+            for s in segs:
+                coord.append (s.coord)
+            coord = np.array (coord, dtype = float)
+            x, y, z = coord.T
+            ax.scatter (x, y, z, color = self.colormap [i + 1], marker = 'o')
+        if self.has_ground:
+            x, y = np.meshgrid (xr, yr)
+            z = np.zeros (x.shape)
+            d = dict (color = '#6cbe6c', alpha = 0.9)
+            ax.plot_surface (x, y, z, **d)
     # end def plot_geo_matplotlib
 
+    def plot_smith_plotly (self, name):
+        X, Y, real, imag, xabs, xphi, Z = self.prepare_vswr ()
+        real_norm = real / self.args.system_impedance
+        imag_norm = imag / self.args.system_impedance
+        text = ['%.1f MHz' % x for x in X]
+        data = np.stack ([real, imag], axis=-1)
+        tpl = \
+            ( '%%{text}<br>'
+              'real: %%{real:.2f} (%%{customdata[0]:.1f} %s)<br>'
+              'imag: %%{imag:.2f} (%%{customdata[1]:.1f} %s)'
+              '<extra></extra>'
+            ) % (Omega, Omega)
+        self.fig = fig = go.Figure ()
+        smith = go.Scattersmith \
+            ( text          = text
+            , imag          = imag_norm
+            , real          = real_norm
+            , hovertemplate = tpl
+            , customdata    = data
+            )
+        fig.add_trace (smith)
+        fig.update (self.plotly_smith_default)
+        fmt = '$Z_0 = %.1f\,\Omega$'
+        if self.args.system_impedance == int (self.args.system_impedance):
+            fmt = '$Z_0 = %.0f\,\Omega$'
+        fig.add_annotation \
+            ( x         = 0.10
+            , y         = 0.15
+            , xref      = 'paper'
+            , yref      = 'paper'
+            , text      = fmt % self.args.system_impedance
+            , showarrow = False
+            )
+        fig.layout.title.text = 'Smith chart for %s' % self.title
+        self.show_plotly (fig, name)
+    # end def plot_smith_plotly
+
+    def plot_smith_matplotlib (self, name):
+        X, Y, real, imag, xabs, xphi, Z = self.prepare_vswr ()
+        ax = self.axes [name]
+        d  = dict (markevery = 1, datatype  = 'Z', markersize = 2)
+        ax.plot (Z, **d)
+    # end def plot_smith_matplotlib
+
     def show_plotly (self, fig, name, script = None):
         """ We can pass a config option into fig.show and fig.write_html,
             allowing scroll seems to be the default for 3d view.
             At some point we may want to set different config options
             for different plots.
             Note that the script is passed as post_script to the html.
             It is triggered after loading the figure.
@@ -1140,15 +1632,17 @@
         d = {}
         if self.args.html_export_option and self.args.export_html:
             d.update (include_plotlyjs = self.args.html_export_option)
         if not self.args.show_plotly_logo:
             d.update (config = config)
         if script is not None:
             d.update (post_script = script)
-        if self.args.export_html:
+        if self.args.output_file and self.save_format:
+            fig.write_image (self.args.output_file, format = 'png')
+        elif self.args.export_html:
             fn = self.args.export_html + '-' + name + '.html'
             fig.write_html (fn, **d)
         else:
             fig.show (**d)
     # end def show_plotly
 
     # For animation:
@@ -1239,15 +1733,36 @@
 
 class SortingArgumentParser (ArgumentParser):
     def __init__ (self, *args, **kw):
         super ().__init__ (*args, formatter_class = SortingHelpFormatter, **kw)
     # end def __init__
 # end class SortingArgumentParser
 
-def main (argv = sys.argv [1:]):
+ham_bands = dict \
+   (( ('70cm', (430.0,  440.0))
+    , ('2m',   (144.0,  146.0))
+    , ('6m',   ( 50.0,   52.0))
+    , ('10m',  ( 28.0,   29.7))
+    , ('12m',  ( 24.89,  24.99))
+    , ('15m',  ( 21.0,   21.45))
+    , ('17m',  ( 18.068, 18.168))
+    , ('20m',  ( 14.0,   14.35))
+    , ('30m',  ( 10.1,   10.15))
+    , ('40m',  (  7.0,    7.2))
+    , ('60m',  (  5.3513, 5.3665))
+    , ('80m',  (  3.5,    3.8))
+    , ('160m', (  1.81,   1.95))
+    , ('630m', (  0.472,  0.479))
+   ))
+
+def main (argv = sys.argv [1:], pic_io = None):
+    """ The pic_io argument is for testing:
+        We put the picture into that file-like object if the pic_io
+        is not None.
+    """
     cmd = SortingArgumentParser ()
     scaling = ['arrl', 'linear', 'linear_db', 'linear_voltage']
     cmd.add_argument \
         ( 'filename'
         , help    = 'File to parse and plot'
         )
     cmd.add_argument \
@@ -1257,14 +1772,22 @@
         )
     cmd.add_argument \
         ( '--angle-azimuth'
         , help    = 'Azimuth angle to use for elevation plot, default is '
                     'maximum gain angle'
         , type    = float
         )
+    deci_styles = ('absolute', 'relative', 'both')
+    cmd.add_argument \
+        ( '--decibel-style'
+        , help    = 'Decibel style for plotly 3D color bar,'
+                    ' one of %s, the default prints the relative value'
+                    ' in parentheses' % ', '.join (deci_styles)
+        , default = 'both'
+        )
     cmd.add_argument \
         ( '--dpi'
         , help    = 'Resolution for matplotlib, default = %(default)s'
         , type    = int
         , default = 80
         )
     cmd.add_argument \
@@ -1284,24 +1807,42 @@
             ( '--with-frequency-slider', '--with-slider'
             , dest    = 'with_slider'
             , help    = 'Turn on frequency slider, frequency can be stepped'
                         ' with +/- keys and slider is very slow.'
             , action  = 'store_true'
             )
     cmd.add_argument \
+        ( '--margin-3d'
+        , help    = 'Margin around 3D plot in pixel for plotly backend'
+        , type    = int
+        , default = 20
+        )
+    cmd.add_argument \
+        ( '--band'
+        , help    = 'Band to highlight in VSWR plot, default are ham'
+                    ' bands in Austria, Format: name:flow,fhi'
+        , default = []
+        , action  = 'append'
+        )
+    cmd.add_argument \
         ( '--plot-geo', '--geo'
         , help    = 'Plot Geometry'
         , action  = 'store_true'
         )
     cmd.add_argument \
+        ( '--plot-smith', '--smith'
+        , help    = 'Plot impedances in Smith chart'
+        , action  = 'store_true'
+        )
+    cmd.add_argument \
         ( '--output-file'
         , help    = 'Output file, default is interactive'
         )
     cmd.add_argument \
-        ( '--plot3d', '--3d', '--plot-3d'
+        ( '--plot3d', '--3d', '--plot-3d', '--3D'
         , help    = 'Do a 3D plot'
         , action  = 'store_true'
         )
     cmd.add_argument \
         ( '--scaling-method'
         , help    = 'Scaling method to use, default=%%(default)s, one of %s'
                   % (', '.join (scaling))
@@ -1338,22 +1879,42 @@
     cmd.add_argument \
         ( "--swr-target-color", "--vswr-target-color"
         , help    = "If the --target-swr-frequency option is given, draw "
                     "vertical line in this color"
         , default = 'grey'
         )
     cmd.add_argument \
+        ( "--swr-plot-impedance-angle"
+        , help    = "In SWR plot impedance as abs/angle, default is real/imag"
+        , action  = 'store_true'
+        )
+    cmd.add_argument \
+        ( "--swr-show-bands"
+        , help    = "Show (ham-radio) bands in SWR plot"
+        , action  = "store_true"
+        )
+    cmd.add_argument \
+        ( "--swr-show-impedance"
+        , help    = "Show impedance in SWR plot"
+        , action  = "store_true"
+        )
+    cmd.add_argument \
+        ( '--title'
+        , help    = 'Title for plot, overrides filename or '
+                    'information in parsed file'
+        )
+    cmd.add_argument \
         ( '--title-font-size'
         , help    = 'Title/legend font size in pt '
                     '(currently only used in plotly)'
         , type    = int
         )
     cmd.add_argument \
         ( '--wireframe'
-        , help    = 'Show 3d plot as a wireframe (not solid)'
+        , help    = 'Show 3D plot as a wireframe (not solid)'
         , action  = 'store_true'
         )
     if px is not None:
         cmd.add_argument \
             ( "-H", "--export-html"
             , help    = "Filename-prefix to export graphics as html, "
                         "type of graphics (azimuth, elevation, ..) is appended"
@@ -1375,21 +1936,47 @@
             )
         cmd.add_argument \
             ( "--show-plotly-logo"
             , help    = "Show plotly logo in menu"
             , action  = 'store_true'
             )
     args = cmd.parse_args (argv)
+    hb = dict (ham_bands)
+    for b in args.band:
+        try:
+            n, r = b.split (':')
+        except ValueError as err:
+            cmd.print_usage ()
+            exit ('Error in band: %s' % err)
+        n = n.strip ()
+        try:
+            l, h = (float (x) for x in r.split (','))
+        except ValueError as err:
+            cmd.print_usage ()
+            exit ('Error in band: %s' % err)
+        if h <= l:
+            if n in hb:
+                del hb [n]
+        else:
+            hb [n] = (l, h)
+    args.band = hb
+    if args.decibel_style not in deci_styles:
+        cmd.print_usage ()
+        exit ('Invalid decibel-style: "%s"' % args.decibel_style)
     if not hasattr (args, 'with_slider'):
         args.with_slider = False
-    gp   = Gain_Plot (args)
+    if pic_io is not None:
+        args.output_file = pic_io
+        args.save_format = 'png'
+    gp = Gain_Plot (args)
 
     # Default is all
     if  (   not args.azimuth and not args.elevation
         and not args.plot3d  and not args.plot_vswr and not args.plot_geo
+        and not args.plot_smith
         ):
         args.plot3d = args.elevation = args.azimuth = args.plot_vswr = True
     gp.plot ()
 # end def main
 
 if __name__ == '__main__':
     main ()
```

### Comparing `plot-antenna-1.6/plot_antenna.egg-info/PKG-INFO` & `plot-antenna-1.7/plot_antenna.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,215 +1,249 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.6
+Version: 1.7
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
-Author-email: rsc@runtux.com
+Author-email: Ralf Schlatterbeck <rsc@runtux.com>
 License: MIT License
-Description: Antenna Plotting Program
-        ========================
-        
-        :Author: Ralf Schlatterbeck <rsc@runtux.com>
-        
-        .. |--| unicode:: U+2013   .. en dash
-        .. |__| unicode:: U+2013   .. en dash without spaces
-            :trim:
-        .. |_| unicode:: U+00A0 .. Non-breaking space
-            :trim:
-        .. |-| unicode:: U+202F .. Thin non-breaking space
-            :trim:
-        
-        This is a program to plot antenna-related data resulting from an antenna
-        simulation. It can read the text output produced by nec2c_ and my
-        python mininec port pymininec_. Most notably it can plot antenna
-        far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
-        graphic that can be rotated and zoomed). It supports a local display
-        program (using matplotlib_) and a HTML output version that displays
-        everything using javascript (using plotly_). The program features a
-        ``--help`` option. If the program called with ``--help`` does not
-        display a ``-H`` or ``--export-html`` option, you most likely do not
-        have a recent version of plotly_ installed. In that case only the
-        matplotlib_ variant is available. For the plotly variant to work you
-        need both, a recent version of plotly_ as well as pandas_ installed.
-        
-        The program started out as a companion-program to my pymininec_
-        project and is now an independent program.
-        
-        The plot program can also display output files of nec2c_, not only
-        from pymininec_.
-        
-        Standalone Plotting with Matplotlib
-        -----------------------------------
-        
-        The default is to plot all available
-        graphics, including an interactive 3d view. In addition with the
-        ``--azimuth`` or ``--elevation`` options you can get an Azimuth
-        diagram::
-        
-            plot-antenna --azimuth test/12-el-1deg.pout
-        
-        .. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-azimuth.png
-            :align: center
-        
-        or an elevation diagram::
-        
-            plot-antenna --elevation test/12-el-1deg.pout
-        
-        .. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-elevation.png
-            :align: center
-        
-        respectively. Note that I used an output file with 1-degree resolution
-        in elevation and azimuth angles not with 5 degrees as in the example
-        above. The pattern look smoother but a 3D-view will be very slow due to
-        the large number of points. The plot program also has a ``--help``
-        option for further information. In particular the scaling of the antenna
-        plot can be selected using the ``--scaling-method`` option with an
-        additional keyword which can be one of ``linear``, ``linear_db``, and
-        ``linear_voltage`` in addition to the default of ``arrl`` scaling. You
-        may consult Cebik's [1]_ article for explanation of the different
-        diagrams. The ``linear_voltage`` option is not explained by Cebik, it is
-        in-between the ``linear`` and ``linear_db`` scaling options.
-        
-        The latest version accepts several plot parameters, ``--elevation``,
-        ``--azimuth``, ``--plot3d``, ``--plot-vswr``, and ``--geo`` which are
-        plotted into one diagram. The default is to plot the first four graphs.
-        With the ``--output`` option pictures can directly be saved without
-        displaying the graphics on the screen. Note that unfortunately the
-        geometry display with the ``--geo`` option does not perform very well
-        because matplotlib_ has poor support for panning and scaling in 3D
-        plots.
-        
-        The latest version has key-bindings for scrolling through the
-        frequencies of an antenna simulation. So if you have an output file with
-        a simulation of multiple frequencies (either with pymininec_ or
-        nec2c_) you can display diagrams for the next frequency by typing
-        ``+``, and to the previous frequency by typing ``-``. For newer versions
-        of matplotlib_ you can display a scrollbar for the frequencies with
-        the ``--with-slider`` option.
-        
-        Other keybindings switch the scaling for the antenna plots, ``a``
-        switches to ``arrl`` scaling, ``l`` switches to linear scaling, ``d``
-        switches to linear dB scaling, and ``v`` switches to linear voltage
-        scaling.
-        
-        Finally the ``w`` key toggles display of the 3d diagram from/to
-        wireframe display. Note that the wireframe display may not be supported
-        on all versions of matplotlib_ and/or graphics cards.
-        
-        Plotting for the Browser with Plotly
-        ------------------------------------
-        
-        All the plot supported for matplotlib_ are also supported with plotly_.
-        These are ``--elevation``, ``--azimuth``, ``--plot3d``, ``--plot-vswr``,
-        and ``--geo``. The plots can be either exported to a .html file using
-        the ``-H`` or ``--export-html`` option (with an additional filename to
-        export to) or injected into a running browser using the ``-S`` or
-        ``--show-in-browser`` option.
-        
-        Unlike for matplotlib_, each plot selected with an option is either
-        shown in a separate window in the browser or exported to a separate
-        file. If exporting to a file, additional output options can be selected
-        with the ``--html-export-option`` setting. The default is to export the
-        file with all javascript included (adds about 3MB to the file size).
-        With ``--html-export-option=directory`` the javascript is not included
-        and a ``plotly.min.js`` file is expected in the same directory as the
-        exported file. This file ships with the plotly_ distribution. When
-        exporting to a file, the plot name is appended to the file name given,
-        this allows export to several different plots in one program invocation.
-        
-        The scaling variants selected with the ``--scaling-method`` option
-        cannot currently be changed at runtime with the plotly_ plots. As with
-        matplotlib_, the default is ``arrl`` scaling.
-        
-        All plots are interactive. For the far-field pattern
-        plots (Azimuth, Elevation, 3D) frequencies can be selected in the legend
-        to the right of the plot. With mouse-over you can see the current angle
-        (Elevation or Azimuth with the 2D plots and both for the 3D plot) and
-        the gain at that point. For the 2D variants, more than one frequency can
-        be selected for plotting. This allows comparison of pattern between
-        different frequencies. For the 3D plot, the frequencies in the legend
-        act like radio-buttons, only one at a time can be selected.
-        
-        With the ``--geo`` option you get a display of the antenna geometry.
-        Unfortunately plotly_ seems to have limitations on the zoom depths, so
-        for large antennas it is not possible to see the plot in deep detail. As
-        of this writing not all geometry details are displayed. In particular 2D
-        patches in NEC, transmission lines in NEC, and visualization of loaded
-        segments (e.g. with a capacity) are not shown.
-        
-        .. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
-            In Antenna Modeling Notes [2], chapter 48, pages 366–379. Available
-            in Cebik's `Antenna modelling notes episode 48`_
-        .. [2] L. B. Cebik. Antenna Modeling Notes, volume 2. antenneX Online
-            Magazine, 2003. Available with antenna models from the `Cebik
-            collection`_.
-        
-        .. _`Cebik collection`:
-            http://on5au.be/Books/allmodnotes.zip
-        .. _`Antenna modelling notes episode 48`:
-            http://on5au.be/content/amod/amod48.html
-        .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
-        .. _pymininec: https://github.com/schlatterbeck/pymininec
-        .. _matplotlib: https://matplotlib.org/
-        .. _plotly: https://github.com/plotly/plotly.py
-        .. _pandas: https://pandas.pydata.org/
-        
-        Release Notes
-        -------------
-        
-        v1.6: More SWR plot changes
-        
-        - Make SWR-plot vertical line colors configurable
-        - Rename elevation-angle and azimuth-angle options to angle-elevation
-          and angle-azimuth so that we can again request an elevation/azimuth
-          plot with shortened options like --ele or --azi
-        - Sort options lexicographically on --help
-        
-        v1.5: Allow target SWR frequency in VSWR plot
-        
-        - Add command-line option --target-swr-frequency
-        - Draw user-specifed target frequency in red, best (minimum) swr in grey
-        
-        v1.4: Reset button and VSWR-Plot improvements
-        
-        - Add grid and minimum-SWR vertical line to VSWR plot
-        - Remove display of frequency in mouse-over (in polar plots and 3D plot)
-        - Make polar reset button reset more parameters
-        
-        v1.3: Add a reset button to plotly polar plots
-        
-        - The polar plots, when zoomed in, could only be reset to the unzoomed
-          view with a double-click. All other plots do have a reset button, add
-          one for the polar plots, too.
-        
-        v1.2: Allow specification of title (legend) font size in plotly version
-        
-        - For some application (e.g. when using the plotly graphics inside a
-          html iframe) the title (or we may want to call it legend) of the
-          graphics may collide with the graphics itself. We can now specify the
-          font size with ``--title-font-size``. This option currently works only
-          with plotly graphics.
-        
-        v1.1: Specification of azimuth / elevation angle
-        
-        - Now we can specify an azimuth angle for elevation plot and an
-          elevation angle for azimuth plots.
-        - Bug-fix in computation of maximum gain azimuth direction: If the
-          maximum gain in theta direction goes up or down, the azimuth angle
-          would be computed incorrectly because all gain values at that theta
-          angle are the same for all azimuth angles.
-        - Sort options: Since there are some options that only exist when some
-          packages are installed we sort options instead of trying to add them
-          in the correct order.
-        
-        v1.0: Initial Release
-        
+Project-URL: Homepage, https://github.com/schlatterbeck/plot-antenna
+Project-URL: Bug Tracker, https://github.com/schlatterbeck/plot-antenna/issues
 Platform: Any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
+Antenna Plotting Program
+========================
+
+:Author: Ralf Schlatterbeck <rsc@runtux.com>
+
+.. |--| unicode:: U+2013   .. en dash
+.. |__| unicode:: U+2013   .. en dash without spaces
+    :trim:
+.. |_| unicode:: U+00A0 .. Non-breaking space
+    :trim:
+.. |-| unicode:: U+202F .. Thin non-breaking space
+    :trim:
+
+This is a program to plot antenna-related data resulting from an antenna
+simulation. It can read the text output produced by nec2c_ and my
+python mininec port pymininec_. Most notably it can plot antenna
+far-field pattern in both 2D (Azimuth and Elevation) and 3D (as a 3D
+graphic that can be rotated and zoomed). It supports a local display
+program (using matplotlib_) and a HTML output version that displays
+everything using javascript (using plotly_). The program features a
+``--help`` option. If the program called with ``--help`` does not
+display a ``-H`` or ``--export-html`` option, you most likely do not
+have a recent version of plotly_ installed. In that case only the
+matplotlib_ variant is available. For the plotly variant to work you
+need both, a recent version of plotly_ as well as pandas_ installed.
+
+The program started out as a companion-program to my pymininec_
+project and is now an independent program.
+
+The plot program can also display output files of nec2c_, not only
+from pymininec_.
+
+Standalone Plotting with Matplotlib
+-----------------------------------
+
+The default is to plot all available
+graphics, including an interactive 3d view. In addition with the
+``--azimuth`` or ``--elevation`` options you can get an Azimuth
+diagram::
+
+    plot-antenna --azimuth test/12-el-1deg.pout
+
+.. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-azimuth.png
+    :align: center
+
+or an elevation diagram::
+
+    plot-antenna --elevation test/12-el-1deg.pout
+
+.. figure:: https://raw.githubusercontent.com/schlatterbeck/plot-antenna/master/test/12-el-elevation.png
+    :align: center
+
+respectively. Note that I used an output file with 1-degree resolution
+in elevation and azimuth angles not with 5 degrees as in the example
+above. The pattern look smoother but a 3D-view will be very slow due to
+the large number of points. The plot program also has a ``--help``
+option for further information. In particular the scaling of the antenna
+plot can be selected using the ``--scaling-method`` option with an
+additional keyword which can be one of ``linear``, ``linear_db``, and
+``linear_voltage`` in addition to the default of ``arrl`` scaling. You
+may consult Cebik's [1]_ article for explanation of the different
+diagrams. The ``linear_voltage`` option is not explained by Cebik, it is
+in-between the ``linear`` and ``linear_db`` scaling options.
+
+The latest version accepts several plot parameters, ``--elevation``,
+``--azimuth``, ``--plot3d``, ``--plot-vswr``, and ``--geo`` which are
+plotted into one diagram. The default is to plot the first four graphs.
+With the ``--output`` option pictures can directly be saved without
+displaying the graphics on the screen. Note that unfortunately the
+geometry display with the ``--geo`` option does not perform very well
+because matplotlib_ has poor support for panning and scaling in 3D
+plots.
+
+The latest version has key-bindings for scrolling through the
+frequencies of an antenna simulation. So if you have an output file with
+a simulation of multiple frequencies (either with pymininec_ or
+nec2c_) you can display diagrams for the next frequency by typing
+``+``, and to the previous frequency by typing ``-``. For newer versions
+of matplotlib_ you can display a scrollbar for the frequencies with
+the ``--with-slider`` option.
+
+Other keybindings switch the scaling for the antenna plots, ``a``
+switches to ``arrl`` scaling, ``l`` switches to linear scaling, ``d``
+switches to linear dB scaling, and ``v`` switches to linear voltage
+scaling.
+
+Finally the ``w`` key toggles display of the 3d diagram from/to
+wireframe display. Note that the wireframe display may not be supported
+on all versions of matplotlib_ and/or graphics cards.
+
+Plotting for the Browser with Plotly
+------------------------------------
+
+All the plot supported for matplotlib_ are also supported with plotly_.
+These are ``--elevation``, ``--azimuth``, ``--plot3d``, ``--plot-vswr``,
+and ``--geo``. The plots can be either exported to a .html file using
+the ``-H`` or ``--export-html`` option (with an additional filename to
+export to) or injected into a running browser using the ``-S`` or
+``--show-in-browser`` option.
+
+Unlike for matplotlib_, each plot selected with an option is either
+shown in a separate window in the browser or exported to a separate
+file. If exporting to a file, additional output options can be selected
+with the ``--html-export-option`` setting. The default is to export the
+file with all javascript included (adds about 3MB to the file size).
+With ``--html-export-option=directory`` the javascript is not included
+and a ``plotly.min.js`` file is expected in the same directory as the
+exported file. This file ships with the plotly_ distribution. When
+exporting to a file, the plot name is appended to the file name given,
+this allows export to several different plots in one program invocation.
+
+The scaling variants selected with the ``--scaling-method`` option
+cannot currently be changed at runtime with the plotly_ plots. As with
+matplotlib_, the default is ``arrl`` scaling.
+
+All plots are interactive. For the far-field pattern
+plots (Azimuth, Elevation, 3D) frequencies can be selected in the legend
+to the right of the plot. With mouse-over you can see the current angle
+(Elevation or Azimuth with the 2D plots and both for the 3D plot) and
+the gain at that point. For the 2D variants, more than one frequency can
+be selected for plotting. This allows comparison of pattern between
+different frequencies. For the 3D plot, the frequencies in the legend
+act like radio-buttons, only one at a time can be selected.
+
+With the ``--geo`` option you get a display of the antenna geometry.
+Unfortunately plotly_ seems to have limitations on the zoom depths, so
+for large antennas it is not possible to see the plot in deep detail. As
+of this writing not all geometry details are displayed. In particular 2D
+patches in NEC, transmission lines in NEC, and visualization of loaded
+segments (e.g. with a capacity) are not shown.
+
+.. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
+    In Antenna Modeling Notes [2], chapter 48, pages 366–379. Available
+    in Cebik's `Antenna modelling notes episode 48`_
+.. [2] L. B. Cebik. Antenna Modeling Notes, volume 2. antenneX Online
+    Magazine, 2003. Available with antenna models from the `Cebik
+    collection`_.
+
+.. _`Cebik collection`:
+    http://on5au.be/Books/allmodnotes.zip
+.. _`Antenna modelling notes episode 48`:
+    http://on5au.be/content/amod/amod48.html
+.. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
+.. _pymininec: https://github.com/schlatterbeck/pymininec
+.. _matplotlib: https://matplotlib.org/
+.. _plotly: https://github.com/plotly/plotly.py
+.. _pandas: https://pandas.pydata.org/
+
+Release Notes
+-------------
+
+v1.7: Add Smith charts, optionally show impedance and band in VSWR plots
+
+Many of the changes in this and several previous versions were suggested
+by Rob Banfield, DM1CM: Adding the bands and impedance to the VSWR plot
+are his idea as well as adding a Smith chart. Due to his attention to
+detail this release corrects a lot of rough edges of previous versions.
+Thanks Rob!
+
+- The aspect ratio in 3D plotly plots is now correct. It used to be a
+  little too wide in the X direction
+- Add Smith chart display
+- Options to add the impedance (either as real/imag or \|Z\|/phi (Z)) in
+  the VSWR plot
+- Option to show the ham radio bands in the VSWR plot
+- Show loads and excitation(s) in geo plot, add ground to geo plot
+- Margin of 3D plots in plotly are much wider now by default and can be
+  configured with an option
+- The style how the gain is displayed in the plotly 3D color bar can now
+  be configured to save space (either relative or absolute gain in dB or
+  dBi, the default is both)
+- When there is only one frequency in the 3D plot, remove the frequency
+  legend
+- Add LICENSE file and pyproject.toml for newer install mechanisms in
+  python
+- Add tests for plotly output
+- Use ppm images for the tests, the previously-used png images did
+  contain the matplotlib version and thus were different for each
+  version -- the ppm images do not have that problem, there are still
+  many differences with different matplotlib versions
+
+v1.6: More SWR plot changes
+
+- Make SWR-plot vertical line colors configurable
+- Rename elevation-angle and azimuth-angle options to angle-elevation
+  and angle-azimuth so that we can again request an elevation/azimuth
+  plot with shortened options like --ele or --azi
+- Sort options lexicographically on --help
+
+v1.5: Allow target SWR frequency in VSWR plot
+
+- Add command-line option --target-swr-frequency
+- Draw user-specifed target frequency in red, best (minimum) swr in grey
+
+v1.4: Reset button and VSWR-Plot improvements
+
+- Add grid and minimum-SWR vertical line to VSWR plot
+- Remove display of frequency in mouse-over (in polar plots and 3D plot)
+- Make polar reset button reset more parameters
+
+v1.3: Add a reset button to plotly polar plots
+
+- The polar plots, when zoomed in, could only be reset to the unzoomed
+  view with a double-click. All other plots do have a reset button, add
+  one for the polar plots, too.
+
+v1.2: Allow specification of title (legend) font size in plotly version
+
+- For some application (e.g. when using the plotly graphics inside a
+  html iframe) the title (or we may want to call it legend) of the
+  graphics may collide with the graphics itself. We can now specify the
+  font size with ``--title-font-size``. This option currently works only
+  with plotly graphics.
+
+v1.1: Specification of azimuth / elevation angle
+
+- Now we can specify an azimuth angle for elevation plot and an
+  elevation angle for azimuth plots.
+- Bug-fix in computation of maximum gain azimuth direction: If the
+  maximum gain in theta direction goes up or down, the azimuth angle
+  would be computed incorrectly because all gain values at that theta
+  angle are the same for all azimuth angles.
+- Sort options: Since there are some options that only exist when some
+  packages are installed we sort options instead of trying to add them
+  in the correct order.
+
+v1.0: Initial Release
```

### Comparing `plot-antenna-1.6/setup.py` & `plot-antenna-1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Copyright (C) 2022 Dr. Ralf Schlatterbeck Open Source Consulting.
+# Copyright (C) 2022-23 Dr. Ralf Schlatterbeck Open Source Consulting.
 # Reichergasse 131, A-3411 Weidling.
 # Web: http://www.runtux.com Email: office@runtux.com
 # All rights reserved
 # ****************************************************************************
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -40,15 +40,18 @@
     , description      =
         "Antenna plotting program for plotting antenna simulation results"
     , long_description = ''.join (description)
     , long_description_content_type='text/x-rst'
     , license          = license
     , author           = "Ralf Schlatterbeck"
     , author_email     = "rsc@runtux.com"
-    , install_requires = ['matplotlib', 'numpy']
+    , install_requires = \
+        [ 'matplotlib', 'numpy', 'pandas', 'plotly'
+        , 'pysmithplot@git+https://github.com/schlatterbeck/pySmithPlot.git'
+        ]
     , packages         = ['plot_antenna']
     , platforms        = 'Any'
     , url              = "https://github.com/schlatterbeck/plot-antenna"
     , python_requires  = rq
     , entry_points     = dict
         ( console_scripts =
             [ 'plot-antenna=plot_antenna.plot_antenna:main' ]
```

