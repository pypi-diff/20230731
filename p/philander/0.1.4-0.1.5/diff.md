# Comparing `tmp/philander-0.1.4.tar.gz` & `tmp/philander-0.1.5.tar.gz`

## Comparing `philander-0.1.4.tar` & `philander-0.1.5.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 philander-0.1.4/.buildpath
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 philander-0.1.4/.project
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.4/.pydevproject
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 philander-0.1.4/.externalToolBuilders/Build Dist.launch
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 philander-0.1.4/.externalToolBuilders/Sphinx API Doc.launch
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 philander-0.1.4/.externalToolBuilders/Sphinx Doc Build.launch
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 philander-0.1.4/.settings/org.eclipse.core.resources.prefs
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 philander-0.1.4/.settings/org.eclipse.ltk.core.refactoring.prefs
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/conf.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/modules.rst
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/philander.fastgait.rst
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/philander.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.buildinfo
--rw-r--r--   0        0        0   281201 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/genindex.html
--rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/gpio.html
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/index.html
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/interruptable.html
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/module.html
--rw-r--r--   0        0        0   456817 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/modules.html
--rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/objects.inv
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/philander.fastgait.html
--rw-r--r--   0        0        0  1347132 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/philander.html
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/py-modindex.html
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/search.html
--rw-r--r--   0        0        0   362586 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/searchindex.js
--rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/systypes.html
--rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/test.html
--rw-r--r--   0        0        0  1893358 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/environment.pickle
--rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/gpio.doctree
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/index.doctree
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/interruptable.doctree
--rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/module.doctree
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/modules.doctree
--rw-r--r--   0        0        0  3591284 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/philander.doctree
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/philander.fastgait.doctree
--rw-r--r--   0        0        0    50137 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/systypes.doctree
--rw-r--r--   0        0        0    76214 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/test.doctree
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/doc/api/index.doctree
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/doc/api/modules.doctree
--rw-r--r--   0        0        0   138640 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/.doctrees/doc/api/philander.doctree
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/dictionary.html
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/index.html
--rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/sensor.html
--rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/systypes.html
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/Configurable.html
--rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/Device.html
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/EventHandler.html
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/FuelGauge.html
--rw-r--r--   0        0        0    61389 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/Sensor.html
--rw-r--r--   0        0        0   115813 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/Serial_Bus.html
--rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/Watchdog.html
--rw-r--r--   0        0        0    23313 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/accelerometer.html
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/battery.html
--rw-r--r--   0        0        0   260186 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/bma456.html
--rw-r--r--   0        0        0   123528 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/bma456_reg.html
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/button.html
--rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/charger.html
--rw-r--r--   0        0        0    27732 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/dictionary.html
--rw-r--r--   0        0        0    28007 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/gasgauge.html
--rw-r--r--   0        0        0    81838 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/gpio.html
--rw-r--r--   0        0        0    60743 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/htu21d.html
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/hygrometer.html
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/imath.html
--rw-r--r--   0        0        0    30184 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/interruptable.html
--rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/led.html
--rw-r--r--   0        0        0   186098 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/max77960.html
--rw-r--r--   0        0        0   118450 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/max77960_reg.html
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/module.html
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/primitives.html
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/sbsimBMA456.html
--rw-r--r--   0        0        0   181688 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/serialbus.html
--rw-r--r--   0        0        0    48037 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/simBMA456.html
--rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/simbus.html
--rw-r--r--   0        0        0    50492 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/simdev.html
--rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/systypes.html
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/thermometer.html
--rw-r--r--   0        0        0    19853 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/vibrasense.html
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/vibrasense2.html
--rw-r--r--   0        0        0    19228 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/voltmeter.html
--rw-r--r--   0        0        0    70844 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_modules/philander/fastgait/actorunit.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/gpio.rst.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/interruptable.rst.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/module.rst.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/philander.fastgait.rst.txt
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/philander.rst.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/systypes.rst.txt
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_sources/test.rst.txt
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/alabaster.css
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/doctools.js
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/plus.png
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 philander-0.1.4/doc/api/html/_static/underscore.js
--rw-r--r--   0        0        0   276792 2020-02-02 00:00:00.000000 philander-0.1.4/doc/uml/philander.aird
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 philander-0.1.4/doc/uml/philander.ecore
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 philander-0.1.4/philander/__init__.py
--rw-r--r--   0        0        0   116874 2020-02-02 00:00:00.000000 philander-0.1.4/philander/_bma456_feature.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 philander-0.1.4/philander/accelerometer.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 philander-0.1.4/philander/battery.py
--rw-r--r--   0        0        0    82563 2020-02-02 00:00:00.000000 philander-0.1.4/philander/bma456.py
--rw-r--r--   0        0        0    53191 2020-02-02 00:00:00.000000 philander-0.1.4/philander/bma456_reg.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 philander-0.1.4/philander/button.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 philander-0.1.4/philander/charger.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 philander-0.1.4/philander/configurable.py
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 philander-0.1.4/philander/dictionary.py
--rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 philander-0.1.4/philander/gasgauge.py
--rw-r--r--   0        0        0    23026 2020-02-02 00:00:00.000000 philander-0.1.4/philander/gpio.py
--rw-r--r--   0        0        0    16476 2020-02-02 00:00:00.000000 philander-0.1.4/philander/htu21d.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 philander-0.1.4/philander/hygrometer.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 philander-0.1.4/philander/imath.py
--rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 philander-0.1.4/philander/interruptable.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 philander-0.1.4/philander/led.py
--rw-r--r--   0        0        0    51566 2020-02-02 00:00:00.000000 philander-0.1.4/philander/max77960.py
--rw-r--r--   0        0        0    39765 2020-02-02 00:00:00.000000 philander-0.1.4/philander/max77960_reg.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 philander-0.1.4/philander/module.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 philander-0.1.4/philander/primitives.py
--rw-r--r--   0        0        0    26759 2020-02-02 00:00:00.000000 philander-0.1.4/philander/sensor.py
--rw-r--r--   0        0        0    59754 2020-02-02 00:00:00.000000 philander-0.1.4/philander/serialbus.py
--rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 philander-0.1.4/philander/simBMA456.py
--rw-r--r--   0        0        0    18518 2020-02-02 00:00:00.000000 philander-0.1.4/philander/simdev.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 philander-0.1.4/philander/systypes.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 philander-0.1.4/philander/thermometer.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 philander-0.1.4/philander/vibrasense.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 philander-0.1.4/philander/vibrasense2.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 philander-0.1.4/philander/voltmeter.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 philander-0.1.4/philander/watchdog.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 philander-0.1.4/philander/fastgait/__init__.py
--rw-r--r--   0        0        0    20466 2020-02-02 00:00:00.000000 philander-0.1.4/philander/fastgait/actorunit.py
--rw-r--r--   0        0        0    21356 2020-02-02 00:00:00.000000 philander-0.1.4/philander/fastgait/sysman.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 philander-0.1.4/test/utgpio.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 philander-0.1.4/test/utimath.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 philander-0.1.4/test/utserialbus.py
--rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 philander-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 philander-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1.4/readme.md
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 philander-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 philander-0.1.5/.buildpath
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 philander-0.1.5/.project
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.5/.pydevproject
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 philander-0.1.5/.externalToolBuilders/Build Dist.launch
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 philander-0.1.5/.externalToolBuilders/Sphinx API Doc.launch
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 philander-0.1.5/.externalToolBuilders/Sphinx Doc Build.launch
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 philander-0.1.5/.settings/org.eclipse.core.resources.prefs
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 philander-0.1.5/.settings/org.eclipse.ltk.core.refactoring.prefs
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/conf.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/modules.rst
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/philander.fastgait.rst
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/philander.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.buildinfo
+-rw-r--r--   0        0        0   281201 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/genindex.html
+-rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/gpio.html
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/index.html
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/interruptable.html
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/module.html
+-rw-r--r--   0        0        0   456817 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/modules.html
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/objects.inv
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/philander.fastgait.html
+-rw-r--r--   0        0        0  1347132 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/philander.html
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/py-modindex.html
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/search.html
+-rw-r--r--   0        0        0   362586 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/searchindex.js
+-rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/systypes.html
+-rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/test.html
+-rw-r--r--   0        0        0  1893129 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/gpio.doctree
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/index.doctree
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/interruptable.doctree
+-rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/module.doctree
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/modules.doctree
+-rw-r--r--   0        0        0  3591284 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/philander.doctree
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/philander.fastgait.doctree
+-rw-r--r--   0        0        0    50137 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/systypes.doctree
+-rw-r--r--   0        0        0    76214 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/test.doctree
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/doc/api/index.doctree
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/doc/api/modules.doctree
+-rw-r--r--   0        0        0   138640 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/.doctrees/doc/api/philander.doctree
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/dictionary.html
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/index.html
+-rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/sensor.html
+-rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/systypes.html
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/Configurable.html
+-rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/Device.html
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/EventHandler.html
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/FuelGauge.html
+-rw-r--r--   0        0        0    61389 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/Sensor.html
+-rw-r--r--   0        0        0   115813 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/Serial_Bus.html
+-rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/Watchdog.html
+-rw-r--r--   0        0        0    23313 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/accelerometer.html
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/battery.html
+-rw-r--r--   0        0        0   260186 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/bma456.html
+-rw-r--r--   0        0        0   123528 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/bma456_reg.html
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/button.html
+-rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/charger.html
+-rw-r--r--   0        0        0    27732 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/dictionary.html
+-rw-r--r--   0        0        0    28007 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/gasgauge.html
+-rw-r--r--   0        0        0    80958 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/gpio.html
+-rw-r--r--   0        0        0    60743 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/htu21d.html
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/hygrometer.html
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/imath.html
+-rw-r--r--   0        0        0    30184 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/interruptable.html
+-rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/led.html
+-rw-r--r--   0        0        0   186098 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/max77960.html
+-rw-r--r--   0        0        0   118450 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/max77960_reg.html
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/module.html
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/primitives.html
+-rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/sbsimBMA456.html
+-rw-r--r--   0        0        0   181688 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/serialbus.html
+-rw-r--r--   0        0        0    48037 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/simBMA456.html
+-rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/simbus.html
+-rw-r--r--   0        0        0    50492 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/simdev.html
+-rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/systypes.html
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/thermometer.html
+-rw-r--r--   0        0        0    19853 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/vibrasense.html
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/vibrasense2.html
+-rw-r--r--   0        0        0    19228 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/voltmeter.html
+-rw-r--r--   0        0        0    70844 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_modules/philander/fastgait/actorunit.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/gpio.rst.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/interruptable.rst.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/module.rst.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/philander.fastgait.rst.txt
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/philander.rst.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/systypes.rst.txt
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_sources/test.rst.txt
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/doctools.js
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 philander-0.1.5/doc/api/html/_static/underscore.js
+-rw-r--r--   0        0        0   276792 2020-02-02 00:00:00.000000 philander-0.1.5/doc/uml/philander.aird
+-rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 philander-0.1.5/doc/uml/philander.ecore
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 philander-0.1.5/philander/__init__.py
+-rw-r--r--   0        0        0   116874 2020-02-02 00:00:00.000000 philander-0.1.5/philander/_bma456_feature.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 philander-0.1.5/philander/accelerometer.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 philander-0.1.5/philander/battery.py
+-rw-r--r--   0        0        0    82563 2020-02-02 00:00:00.000000 philander-0.1.5/philander/bma456.py
+-rw-r--r--   0        0        0    53191 2020-02-02 00:00:00.000000 philander-0.1.5/philander/bma456_reg.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 philander-0.1.5/philander/button.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 philander-0.1.5/philander/charger.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 philander-0.1.5/philander/configurable.py
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 philander-0.1.5/philander/dictionary.py
+-rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 philander-0.1.5/philander/gasgauge.py
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 philander-0.1.5/philander/gpio.py
+-rw-r--r--   0        0        0    16476 2020-02-02 00:00:00.000000 philander-0.1.5/philander/htu21d.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 philander-0.1.5/philander/hygrometer.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 philander-0.1.5/philander/imath.py
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 philander-0.1.5/philander/interruptable.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 philander-0.1.5/philander/led.py
+-rw-r--r--   0        0        0    51566 2020-02-02 00:00:00.000000 philander-0.1.5/philander/max77960.py
+-rw-r--r--   0        0        0    39765 2020-02-02 00:00:00.000000 philander-0.1.5/philander/max77960_reg.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 philander-0.1.5/philander/module.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 philander-0.1.5/philander/primitives.py
+-rw-r--r--   0        0        0    26759 2020-02-02 00:00:00.000000 philander-0.1.5/philander/sensor.py
+-rw-r--r--   0        0        0    59754 2020-02-02 00:00:00.000000 philander-0.1.5/philander/serialbus.py
+-rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 philander-0.1.5/philander/simBMA456.py
+-rw-r--r--   0        0        0    18518 2020-02-02 00:00:00.000000 philander-0.1.5/philander/simdev.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 philander-0.1.5/philander/systypes.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 philander-0.1.5/philander/thermometer.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 philander-0.1.5/philander/vibrasense.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 philander-0.1.5/philander/vibrasense2.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 philander-0.1.5/philander/voltmeter.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 philander-0.1.5/philander/watchdog.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 philander-0.1.5/philander/fastgait/__init__.py
+-rw-r--r--   0        0        0    20466 2020-02-02 00:00:00.000000 philander-0.1.5/philander/fastgait/actorunit.py
+-rw-r--r--   0        0        0    21356 2020-02-02 00:00:00.000000 philander-0.1.5/philander/fastgait/sysman.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 philander-0.1.5/test/utgpio.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 philander-0.1.5/test/utimath.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 philander-0.1.5/test/utserialbus.py
+-rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 philander-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 philander-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1.5/readme.md
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 philander-0.1.5/PKG-INFO
```

### Comparing `philander-0.1.4/.project` & `philander-0.1.5/.project`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/.pydevproject` & `philander-0.1.5/.pydevproject`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/.externalToolBuilders/Build Dist.launch` & `philander-0.1.5/.externalToolBuilders/Build Dist.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/.externalToolBuilders/Sphinx API Doc.launch` & `philander-0.1.5/.externalToolBuilders/Sphinx API Doc.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/.externalToolBuilders/Sphinx Doc Build.launch` & `philander-0.1.5/.externalToolBuilders/Sphinx Doc Build.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/conf.py` & `philander-0.1.5/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/philander.fastgait.rst` & `philander-0.1.5/doc/api/philander.fastgait.rst`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/philander.rst` & `philander-0.1.5/doc/api/philander.rst`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/genindex.html` & `philander-0.1.5/doc/api/html/genindex.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/gpio.html` & `philander-0.1.5/doc/api/html/gpio.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/index.html` & `philander-0.1.5/doc/api/html/index.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/interruptable.html` & `philander-0.1.5/doc/api/html/interruptable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/module.html` & `philander-0.1.5/doc/api/html/module.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/modules.html` & `philander-0.1.5/doc/api/html/modules.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/objects.inv` & `philander-0.1.5/doc/api/html/objects.inv`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/philander.fastgait.html` & `philander-0.1.5/doc/api/html/philander.fastgait.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/philander.html` & `philander-0.1.5/doc/api/html/philander.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/py-modindex.html` & `philander-0.1.5/doc/api/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/search.html` & `philander-0.1.5/doc/api/html/search.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/searchindex.js` & `philander-0.1.5/doc/api/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/systypes.html` & `philander-0.1.5/doc/api/html/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/test.html` & `philander-0.1.5/doc/api/html/test.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/gpio.doctree` & `philander-0.1.5/doc/api/html/.doctrees/gpio.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/index.doctree` & `philander-0.1.5/doc/api/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/interruptable.doctree` & `philander-0.1.5/doc/api/html/.doctrees/interruptable.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/module.doctree` & `philander-0.1.5/doc/api/html/.doctrees/module.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/modules.doctree` & `philander-0.1.5/doc/api/html/.doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/philander.doctree` & `philander-0.1.5/doc/api/html/.doctrees/philander.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/philander.fastgait.doctree` & `philander-0.1.5/doc/api/html/.doctrees/philander.fastgait.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/systypes.doctree` & `philander-0.1.5/doc/api/html/.doctrees/systypes.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/test.doctree` & `philander-0.1.5/doc/api/html/.doctrees/test.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/doc/api/index.doctree` & `philander-0.1.5/doc/api/html/.doctrees/doc/api/index.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/doc/api/modules.doctree` & `philander-0.1.5/doc/api/html/.doctrees/doc/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/.doctrees/doc/api/philander.doctree` & `philander-0.1.5/doc/api/html/.doctrees/doc/api/philander.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/dictionary.html` & `philander-0.1.5/doc/api/html/_modules/dictionary.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/index.html` & `philander-0.1.5/doc/api/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/sensor.html` & `philander-0.1.5/doc/api/html/_modules/sensor.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/systypes.html` & `philander-0.1.5/doc/api/html/_modules/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/Configurable.html` & `philander-0.1.5/doc/api/html/_modules/philander/Configurable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/Device.html` & `philander-0.1.5/doc/api/html/_modules/philander/Device.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/EventHandler.html` & `philander-0.1.5/doc/api/html/_modules/philander/EventHandler.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/FuelGauge.html` & `philander-0.1.5/doc/api/html/_modules/philander/FuelGauge.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/Sensor.html` & `philander-0.1.5/doc/api/html/_modules/philander/Sensor.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/Serial_Bus.html` & `philander-0.1.5/doc/api/html/_modules/philander/Serial_Bus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/Watchdog.html` & `philander-0.1.5/doc/api/html/_modules/philander/Watchdog.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/accelerometer.html` & `philander-0.1.5/doc/api/html/_modules/philander/accelerometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/battery.html` & `philander-0.1.5/doc/api/html/_modules/philander/battery.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/bma456.html` & `philander-0.1.5/doc/api/html/_modules/philander/bma456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/bma456_reg.html` & `philander-0.1.5/doc/api/html/_modules/philander/bma456_reg.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/button.html` & `philander-0.1.5/doc/api/html/_modules/philander/button.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/charger.html` & `philander-0.1.5/doc/api/html/_modules/philander/charger.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/dictionary.html` & `philander-0.1.5/doc/api/html/_modules/philander/dictionary.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/gasgauge.html` & `philander-0.1.5/doc/api/html/_modules/philander/gasgauge.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/gpio.html` & `philander-0.1.5/doc/api/html/_modules/philander/gpio.html`

 * *Files 0% similar despite different names*

```diff
@@ -312,33 +312,33 @@
 <span class="sd">        a good choice. After usage of this instance is finished, the</span>
 <span class="sd">        application should call :meth:`close`.</span>
 <span class="sd">        </span>
 <span class="sd">        :param dict(str, object) paramDict: Configuration parameters as obtained from :meth:`Params_init`, possibly.</span>
 <span class="sd">        :return: An error code indicating either success or the reason of failure.</span>
 <span class="sd">        :rtype: ErrorCode</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
+        <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
         <span class="c1"># Retrieve defaults</span>
         <span class="n">defaults</span> <span class="o">=</span> <span class="p">{}</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">Params_init</span><span class="p">(</span><span class="n">defaults</span><span class="p">)</span>
         <span class="n">handler</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="c1"># Scan parameters</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_designator</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.pinDesignator&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_designator</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-            <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errInvalidParameter</span>
+            <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errInvalidParameter</span>
         <span class="n">numScheme</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.pinNumbering&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.pinNumbering&quot;</span><span class="p">])</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_direction</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.direction&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.direction&quot;</span><span class="p">])</span>
         <span class="n">level</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.level&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.level&quot;</span><span class="p">])</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_direction</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">DIRECTION_IN</span><span class="p">:</span>
             <span class="n">pull</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.pull&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.pull&quot;</span><span class="p">])</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_trigger</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.trigger&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.trigger&quot;</span><span class="p">])</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_bounce</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.bounce&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.bounce&quot;</span><span class="p">])</span>
             <span class="n">feedback</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.feedback&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.feedback&quot;</span><span class="p">])</span>
             <span class="n">handler</span> <span class="o">=</span> <span class="n">paramDict</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;gpio.handler&quot;</span><span class="p">,</span> <span class="n">defaults</span><span class="p">[</span><span class="s2">&quot;gpio.handler&quot;</span><span class="p">])</span>
-        <span class="k">if</span> <span class="n">ret</span> <span class="o">==</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span><span class="p">:</span>
+        <span class="k">if</span> <span class="n">ret</span> <span class="o">==</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_RPIGPIO</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="o">.</span><span class="n">setmode</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dictNumScheme</span><span class="p">[</span><span class="n">numScheme</span><span class="p">])</span>
                 <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_direction</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">DIRECTION_OUT</span><span class="p">:</span>
                     <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="o">.</span><span class="n">setup</span><span class="p">(</span>
                         <span class="bp">self</span><span class="o">.</span><span class="n">_designator</span><span class="p">,</span>
                         <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="o">.</span><span class="n">OUT</span><span class="p">,</span>
                         <span class="n">initial</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dictLevel</span><span class="p">[</span><span class="n">level</span><span class="p">],</span>
@@ -388,20 +388,20 @@
                         <span class="bp">self</span><span class="o">.</span><span class="n">pin</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="p">(</span>
                             <span class="s2">&quot;/dev/gpiochip0&quot;</span><span class="p">,</span>
                             <span class="bp">self</span><span class="o">.</span><span class="n">_designator</span><span class="p">,</span>
                             <span class="bp">self</span><span class="o">.</span><span class="n">_dictDirection</span><span class="p">[</span><span class="n">GPIO</span><span class="o">.</span><span class="n">DIRECTION_IN</span><span class="p">],</span>
                             <span class="n">bias</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dictPull</span><span class="p">[</span><span class="n">pull</span><span class="p">],</span>
                         <span class="p">)</span>
                 <span class="k">else</span><span class="p">:</span>
-                    <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotSupported</span>
+                    <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotSupported</span>
             <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_SIM</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_level</span> <span class="o">=</span> <span class="n">level</span>
             <span class="k">else</span><span class="p">:</span>
-                <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
-        <span class="k">if</span> <span class="n">ret</span> <span class="o">==</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span><span class="p">:</span>
+                <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
+        <span class="k">if</span> <span class="n">ret</span> <span class="o">==</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">handler</span><span class="p">:</span>
                 <span class="n">ret</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">registerInterruptHandler</span><span class="p">(</span>
                     <span class="n">GPIO</span><span class="o">.</span><span class="n">EVENT_DEFAULT</span><span class="p">,</span> <span class="n">feedback</span><span class="p">,</span> <span class="n">handler</span>
                 <span class="p">)</span>
         <span class="k">return</span> <span class="n">ret</span></div>
 
 <div class="viewcode-block" id="GPIO.close"><a class="viewcode-back" href="../../philander.html#philander.gpio.GPIO.close">[docs]</a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
@@ -422,15 +422,15 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_PERIPHERY</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_stopWorker</span><span class="p">()</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_SIM</span><span class="p">:</span>
             <span class="k">pass</span>
         <span class="k">else</span><span class="p">:</span>
-            <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
+            <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">pin</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">return</span> <span class="n">ret</span></div>
 
 <div class="viewcode-block" id="GPIO.setRunLevel"><a class="viewcode-back" href="../../philander.html#philander.gpio.GPIO.setRunLevel">[docs]</a>    <span class="k">def</span> <span class="nf">setRunLevel</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">level</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Select the power-saving operation mode.</span>
 
 <span class="sd">        Switches the instance to one of the power-saving modes or</span>
@@ -438,30 +438,30 @@
 <span class="sd">        modes can greatly reduce the system&#39;s total power consumption.</span>
 <span class="sd">        </span>
 <span class="sd">        :param RunLevel level: The level to switch to.</span>
 <span class="sd">        :return: An error code indicating either success or the reason of failure.</span>
 <span class="sd">        :rtype: ErrorCode</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">del</span> <span class="n">level</span>
-        <span class="k">return</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span></div>
+        <span class="k">return</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span></div>
 
 <div class="viewcode-block" id="GPIO.enableInterrupt"><a class="viewcode-back" href="../../philander.html#philander.gpio.GPIO.enableInterrupt">[docs]</a>    <span class="k">def</span> <span class="nf">enableInterrupt</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Enables the gpio interrupt for that pin.</span>
 
 <span class="sd">        If the pin is configured for input, enables the interrupt for</span>
 <span class="sd">        that pin. Depending on the trigger configured during :meth:`open`,</span>
 <span class="sd">        an event will be fired the next time when the condition is</span>
 <span class="sd">        satisfied.</span>
 <span class="sd">        </span>
 <span class="sd">        :return: An error code indicating either success or the reason of failure.</span>
 <span class="sd">        :rtype: ErrorCode</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
+        <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_fIntEnabled</span><span class="p">:</span>
-            <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
+            <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_RPIGPIO</span><span class="p">:</span>
                 <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_bounce</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
                     <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="o">.</span><span class="n">add_event_detect</span><span class="p">(</span>
                         <span class="bp">self</span><span class="o">.</span><span class="n">_designator</span><span class="p">,</span>
                         <span class="bp">self</span><span class="o">.</span><span class="n">_dictTrigger</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_trigger</span><span class="p">],</span>
                         <span class="n">callback</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_callback</span><span class="p">,</span>
@@ -482,28 +482,28 @@
             <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_PERIPHERY</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">edge</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dictTrigger</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_trigger</span><span class="p">]</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_stopWorker</span><span class="p">()</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_worker</span> <span class="o">=</span> <span class="n">Thread</span><span class="p">(</span><span class="n">target</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_workerLoop</span><span class="p">,</span> <span class="n">name</span><span class="o">=</span><span class="s2">&quot;GPIO worker&quot;</span><span class="p">)</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_worker</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_fIntEnabled</span> <span class="o">=</span> <span class="kc">True</span>
             <span class="k">else</span><span class="p">:</span>
-                <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
+                <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
         <span class="k">return</span> <span class="n">ret</span></div>
 
 <div class="viewcode-block" id="GPIO.disableInterrupt"><a class="viewcode-back" href="../../philander.html#philander.gpio.GPIO.disableInterrupt">[docs]</a>    <span class="k">def</span> <span class="nf">disableInterrupt</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Disables the gpio interrupt for that pin.</span>
 
 <span class="sd">        Immediately disables the interrupt for that pin. It will not</span>
 <span class="sd">        _fire an event anymore, unless :meth:`enableInterrupt` is called</span>
 <span class="sd">        anew.</span>
 <span class="sd">        </span>
 <span class="sd">        :return: An error code indicating either success or the reason of failure.</span>
 <span class="sd">        :rtype: ErrorCode</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
+        <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_fIntEnabled</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_RPIGPIO</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="o">.</span><span class="n">remove_event_detect</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_designator</span><span class="p">)</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_fIntEnabled</span> <span class="o">=</span> <span class="kc">False</span>
             <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_GPIOZERO</span><span class="p">:</span>
                 <span class="kn">from</span> <span class="nn">gpiozero</span> <span class="kn">import</span> <span class="n">CallbackSetToNone</span>
 
@@ -513,17 +513,17 @@
                     <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">when_deactivated</span> <span class="o">=</span> <span class="kc">None</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_fIntEnabled</span> <span class="o">=</span> <span class="kc">False</span>
             <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_PERIPHERY</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_stopWorker</span><span class="p">()</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">edge</span> <span class="o">=</span> <span class="s2">&quot;none&quot;</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_fIntEnabled</span> <span class="o">=</span> <span class="kc">False</span>
             <span class="k">else</span><span class="p">:</span>
-                <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
+                <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
         <span class="k">else</span><span class="p">:</span>
-            <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
+            <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
         <span class="k">return</span> <span class="n">ret</span></div>
 
 <div class="viewcode-block" id="GPIO.get"><a class="viewcode-back" href="../../philander.html#philander.gpio.GPIO.get">[docs]</a>    <span class="k">def</span> <span class="nf">get</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Retrieve the pin level.</span>
 
 <span class="sd">        Gives the pin level, independent of whether the pin direction</span>
 <span class="sd">        is set to input or output.</span>
@@ -555,28 +555,28 @@
 <span class="sd">        Outputs the given level at this pin. Does not work, if this pin</span>
 <span class="sd">        is set to input direction.</span>
 <span class="sd">        </span>
 <span class="sd">        :param int newLevel: The new level to set this pin to. Must be one of GPIO.LEVEL_[HIGH | LOW].</span>
 <span class="sd">        :return: An error code indicating either success or the reason of failure.</span>
 <span class="sd">        :rtype: ErrorCode</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
+        <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errOk</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_RPIGPIO</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_factory</span><span class="o">.</span><span class="n">output</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_designator</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dictLevel</span><span class="p">[</span><span class="n">newLevel</span><span class="p">])</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_GPIOZERO</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dictLevel</span><span class="p">[</span><span class="n">newLevel</span><span class="p">]</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_PERIPHERY</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">pin</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dictLevel</span><span class="p">[</span><span class="n">newLevel</span><span class="p">])</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">_implpak</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">_IMPLPAK_SIM</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">newLevel</span> <span class="o">==</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">LEVEL_HIGH</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_level</span> <span class="o">=</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">LEVEL_HIGH</span>
             <span class="k">else</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_level</span> <span class="o">=</span> <span class="n">GPIO</span><span class="o">.</span><span class="n">LEVEL_LOW</span>
         <span class="k">else</span><span class="p">:</span>
-            <span class="n">ret</span> <span class="o">=</span> <span class="n">systypes</span><span class="o">.</span><span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
+            <span class="n">ret</span> <span class="o">=</span> <span class="n">ErrorCode</span><span class="o">.</span><span class="n">errNotImplemented</span>
 
         <span class="k">return</span> <span class="n">ret</span></div></div>
 </pre></div>
 
           </div>
           
         </div>
```

#### html2text {}

```diff
@@ -307,38 +307,38 @@
 
         :param dict(str, object) paramDict: Configuration parameters as
 obtained from :meth:`Params_init`, possibly.
         :return: An error code indicating either success or the reason of
 failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         # Retrieve defaults
         defaults = {}
         self.Params_init(defaults)
         handler = None
         # Scan parameters
         self._designator = paramDict.get("gpio.pinDesignator", None)
         if self._designator is None:
-            ret = systypes.ErrorCode.errInvalidParameter
+            ret = ErrorCode.errInvalidParameter
         numScheme = paramDict.get("gpio.pinNumbering", defaults
 ["gpio.pinNumbering"])
         self._direction = paramDict.get("gpio.direction", defaults
 ["gpio.direction"])
         level = paramDict.get("gpio.level", defaults["gpio.level"])
         if self._direction == GPIO.DIRECTION_IN:
             pull = paramDict.get("gpio.pull", defaults["gpio.pull"])
             self._trigger = paramDict.get("gpio.trigger", defaults
 ["gpio.trigger"])
             self._bounce = paramDict.get("gpio.bounce", defaults
 ["gpio.bounce"])
             feedback = paramDict.get("gpio.feedback", defaults
 ["gpio.feedback"])
             handler = paramDict.get("gpio.handler", defaults["gpio.handler"])
-        if ret == systypes.ErrorCode.errOk:
+        if ret == ErrorCode.errOk:
             if self._implpak == GPIO._IMPLPAK_RPIGPIO:
                 self._factory.setmode(self._dictNumScheme[numScheme])
                 if self._direction == GPIO.DIRECTION_OUT:
                     self._factory.setup(
                         self._designator,
                         self._factory.OUT,
                         initial=self._dictLevel[level],
@@ -389,20 +389,20 @@
                         self.pin = self._factory(
                             "/dev/gpiochip0",
                             self._designator,
                             self._dictDirection[GPIO.DIRECTION_IN],
                             bias=self._dictPull[pull],
                         )
                 else:
-                    ret = systypes.ErrorCode.errNotSupported
+                    ret = ErrorCode.errNotSupported
             elif self._implpak == GPIO._IMPLPAK_SIM:
                 self._level = level
             else:
-                ret = systypes.ErrorCode.errNotImplemented
-        if ret == systypes.ErrorCode.errOk:
+                ret = ErrorCode.errNotImplemented
+        if ret == ErrorCode.errOk:
             if handler:
                 ret = self.registerInterruptHandler(
                     GPIO.EVENT_DEFAULT, feedback, handler
                 )
         return ret
 
 
@@ -425,15 +425,15 @@
             self.pin.close()
         elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
             self._stopWorker()
             self.pin.close()
         elif self._implpak == GPIO._IMPLPAK_SIM:
             pass
         else:
-            ret = systypes.ErrorCode.errNotImplemented
+            ret = ErrorCode.errNotImplemented
         self.pin = None
         return ret
 
 
 [docs]    def setRunLevel(self, level):
         """Select the power-saving operation mode.
 
@@ -443,32 +443,32 @@
 
         :param RunLevel level: The level to switch to.
         :return: An error code indicating either success or the reason of
 failure.
         :rtype: ErrorCode
         """
         del level
-        return systypes.ErrorCode.errNotImplemented
+        return ErrorCode.errNotImplemented
 
 
 [docs]    def enableInterrupt(self):
         """Enables the gpio interrupt for that pin.
 
         If the pin is configured for input, enables the interrupt for
         that pin. Depending on the trigger configured during :meth:`open`,
         an event will be fired the next time when the condition is
         satisfied.
 
         :return: An error code indicating either success or the reason of
 failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         if self._fIntEnabled:
-            ret = systypes.ErrorCode.errOk
+            ret = ErrorCode.errOk
         else:
             if self._implpak == GPIO._IMPLPAK_RPIGPIO:
                 if self._bounce > 0:
                     self._factory.add_event_detect(
                         self._designator,
                         self._dictTrigger[self._trigger],
                         callback=self._callback,
@@ -490,30 +490,30 @@
                 self.pin.edge = self._dictTrigger[self._trigger]
                 self._stopWorker()
                 self._worker = Thread(target=self._workerLoop, name="GPIO
 worker")
                 self._worker.start()
                 self._fIntEnabled = True
             else:
-                ret = systypes.ErrorCode.errNotImplemented
+                ret = ErrorCode.errNotImplemented
         return ret
 
 
 [docs]    def disableInterrupt(self):
         """Disables the gpio interrupt for that pin.
 
         Immediately disables the interrupt for that pin. It will not
         _fire an event anymore, unless :meth:`enableInterrupt` is called
         anew.
 
         :return: An error code indicating either success or the reason of
 failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         if self._fIntEnabled:
             if self._implpak == GPIO._IMPLPAK_RPIGPIO:
                 self._factory.remove_event_detect(self._designator)
                 self._fIntEnabled = False
             elif self._implpak == GPIO._IMPLPAK_GPIOZERO:
                 from gpiozero import CallbackSetToNone
 
@@ -523,17 +523,17 @@
                     self.pin.when_deactivated = None
                 self._fIntEnabled = False
             elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
                 self._stopWorker()
                 self.pin.edge = "none"
                 self._fIntEnabled = False
             else:
-                ret = systypes.ErrorCode.errNotImplemented
+                ret = ErrorCode.errNotImplemented
         else:
-            ret = systypes.ErrorCode.errOk
+            ret = ErrorCode.errOk
         return ret
 
 
 [docs]    def get(self):
         """Retrieve the pin level.
 
         Gives the pin level, independent of whether the pin direction
@@ -570,28 +570,28 @@
 
         :param int newLevel: The new level to set this pin to. Must be one of
 GPIO.LEVEL_[HIGH | LOW].
         :return: An error code indicating either success or the reason of
 failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         if self._implpak == GPIO._IMPLPAK_RPIGPIO:
             self._factory.output(self._designator, self._dictLevel[newLevel])
         elif self._implpak == GPIO._IMPLPAK_GPIOZERO:
             self.pin.value = self._dictLevel[newLevel]
         elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
             self.pin.write(self._dictLevel[newLevel])
         elif self._implpak == GPIO._IMPLPAK_SIM:
             if newLevel == GPIO.LEVEL_HIGH:
                 self._level = GPIO.LEVEL_HIGH
             else:
                 self._level = GPIO.LEVEL_LOW
         else:
-            ret = systypes.ErrorCode.errNotImplemented
+            ret = ErrorCode.errNotImplemented
 
         return ret
 ****** philander ******
 **** Navigation ****
 Contents:
     * philander
 **** Related Topics ****
```

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/htu21d.html` & `philander-0.1.5/doc/api/html/_modules/philander/htu21d.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/hygrometer.html` & `philander-0.1.5/doc/api/html/_modules/philander/hygrometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/imath.html` & `philander-0.1.5/doc/api/html/_modules/philander/imath.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/interruptable.html` & `philander-0.1.5/doc/api/html/_modules/philander/interruptable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/led.html` & `philander-0.1.5/doc/api/html/_modules/philander/led.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/max77960.html` & `philander-0.1.5/doc/api/html/_modules/philander/max77960.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/max77960_reg.html` & `philander-0.1.5/doc/api/html/_modules/philander/max77960_reg.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/module.html` & `philander-0.1.5/doc/api/html/_modules/philander/module.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/primitives.html` & `philander-0.1.5/doc/api/html/_modules/philander/primitives.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/sbsimBMA456.html` & `philander-0.1.5/doc/api/html/_modules/philander/sbsimBMA456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/serialbus.html` & `philander-0.1.5/doc/api/html/_modules/philander/serialbus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/simBMA456.html` & `philander-0.1.5/doc/api/html/_modules/philander/simBMA456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/simbus.html` & `philander-0.1.5/doc/api/html/_modules/philander/simbus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/simdev.html` & `philander-0.1.5/doc/api/html/_modules/philander/simdev.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/systypes.html` & `philander-0.1.5/doc/api/html/_modules/philander/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/thermometer.html` & `philander-0.1.5/doc/api/html/_modules/philander/thermometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/vibrasense.html` & `philander-0.1.5/doc/api/html/_modules/philander/vibrasense.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/vibrasense2.html` & `philander-0.1.5/doc/api/html/_modules/philander/vibrasense2.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/voltmeter.html` & `philander-0.1.5/doc/api/html/_modules/philander/voltmeter.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_modules/philander/fastgait/actorunit.html` & `philander-0.1.5/doc/api/html/_modules/philander/fastgait/actorunit.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_sources/philander.fastgait.rst.txt` & `philander-0.1.5/doc/api/html/_sources/philander.fastgait.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_sources/philander.rst.txt` & `philander-0.1.5/doc/api/html/_sources/philander.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_sources/test.rst.txt` & `philander-0.1.5/doc/api/html/_sources/test.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js` & `philander-0.1.5/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/alabaster.css` & `philander-0.1.5/doc/api/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/basic.css` & `philander-0.1.5/doc/api/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/doctools.js` & `philander-0.1.5/doc/api/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/jquery-3.6.0.js` & `philander-0.1.5/doc/api/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/jquery.js` & `philander-0.1.5/doc/api/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/language_data.js` & `philander-0.1.5/doc/api/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/pygments.css` & `philander-0.1.5/doc/api/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/searchtools.js` & `philander-0.1.5/doc/api/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/sphinx_highlight.js` & `philander-0.1.5/doc/api/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/underscore-1.13.1.js` & `philander-0.1.5/doc/api/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/api/html/_static/underscore.js` & `philander-0.1.5/doc/api/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/uml/philander.aird` & `philander-0.1.5/doc/uml/philander.aird`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/doc/uml/philander.ecore` & `philander-0.1.5/doc/uml/philander.ecore`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/__init__.py` & `philander-0.1.5/philander/__init__.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/_bma456_feature.py` & `philander-0.1.5/philander/_bma456_feature.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/accelerometer.py` & `philander-0.1.5/philander/accelerometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/battery.py` & `philander-0.1.5/philander/battery.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/bma456.py` & `philander-0.1.5/philander/bma456.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/bma456_reg.py` & `philander-0.1.5/philander/bma456_reg.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/button.py` & `philander-0.1.5/philander/button.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/charger.py` & `philander-0.1.5/philander/charger.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/configurable.py` & `philander-0.1.5/philander/configurable.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/dictionary.py` & `philander-0.1.5/philander/dictionary.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/gasgauge.py` & `philander-0.1.5/philander/gasgauge.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/gpio.py` & `philander-0.1.5/philander/gpio.py`

 * *Files 4% similar despite different names*

```diff
@@ -277,33 +277,33 @@
         a good choice. After usage of this instance is finished, the
         application should call :meth:`close`.
         
         :param dict(str, object) paramDict: Configuration parameters as obtained from :meth:`Params_init`, possibly.
         :return: An error code indicating either success or the reason of failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         # Retrieve defaults
         defaults = {}
         self.Params_init(defaults)
         handler = None
         # Scan parameters
         self._designator = paramDict.get("gpio.pinDesignator", None)
         if self._designator is None:
-            ret = systypes.ErrorCode.errInvalidParameter
+            ret = ErrorCode.errInvalidParameter
         numScheme = paramDict.get("gpio.pinNumbering", defaults["gpio.pinNumbering"])
         self._direction = paramDict.get("gpio.direction", defaults["gpio.direction"])
         level = paramDict.get("gpio.level", defaults["gpio.level"])
         if self._direction == GPIO.DIRECTION_IN:
             pull = paramDict.get("gpio.pull", defaults["gpio.pull"])
             self._trigger = paramDict.get("gpio.trigger", defaults["gpio.trigger"])
             self._bounce = paramDict.get("gpio.bounce", defaults["gpio.bounce"])
             feedback = paramDict.get("gpio.feedback", defaults["gpio.feedback"])
             handler = paramDict.get("gpio.handler", defaults["gpio.handler"])
-        if ret == systypes.ErrorCode.errOk:
+        if ret == ErrorCode.errOk:
             if self._implpak == GPIO._IMPLPAK_RPIGPIO:
                 self._factory.setmode(self._dictNumScheme[numScheme])
                 if self._direction == GPIO.DIRECTION_OUT:
                     self._factory.setup(
                         self._designator,
                         self._factory.OUT,
                         initial=self._dictLevel[level],
@@ -353,20 +353,20 @@
                         self.pin = self._factory(
                             "/dev/gpiochip0",
                             self._designator,
                             self._dictDirection[GPIO.DIRECTION_IN],
                             bias=self._dictPull[pull],
                         )
                 else:
-                    ret = systypes.ErrorCode.errNotSupported
+                    ret = ErrorCode.errNotSupported
             elif self._implpak == GPIO._IMPLPAK_SIM:
                 self._level = level
             else:
-                ret = systypes.ErrorCode.errNotImplemented
-        if ret == systypes.ErrorCode.errOk:
+                ret = ErrorCode.errNotImplemented
+        if ret == ErrorCode.errOk:
             if handler:
                 ret = self.registerInterruptHandler(
                     GPIO.EVENT_DEFAULT, feedback, handler
                 )
         return ret
 
     def close(self):
@@ -387,15 +387,15 @@
             self.pin.close()
         elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
             self._stopWorker()
             self.pin.close()
         elif self._implpak == GPIO._IMPLPAK_SIM:
             pass
         else:
-            ret = systypes.ErrorCode.errNotImplemented
+            ret = ErrorCode.errNotImplemented
         self.pin = None
         return ret
 
     def setRunLevel(self, level):
         """Select the power-saving operation mode.
 
         Switches the instance to one of the power-saving modes or
@@ -403,30 +403,30 @@
         modes can greatly reduce the system's total power consumption.
         
         :param RunLevel level: The level to switch to.
         :return: An error code indicating either success or the reason of failure.
         :rtype: ErrorCode
         """
         del level
-        return systypes.ErrorCode.errNotImplemented
+        return ErrorCode.errNotImplemented
 
     def enableInterrupt(self):
         """Enables the gpio interrupt for that pin.
 
         If the pin is configured for input, enables the interrupt for
         that pin. Depending on the trigger configured during :meth:`open`,
         an event will be fired the next time when the condition is
         satisfied.
         
         :return: An error code indicating either success or the reason of failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         if self._fIntEnabled:
-            ret = systypes.ErrorCode.errOk
+            ret = ErrorCode.errOk
         else:
             if self._implpak == GPIO._IMPLPAK_RPIGPIO:
                 if self._bounce > 0:
                     self._factory.add_event_detect(
                         self._designator,
                         self._dictTrigger[self._trigger],
                         callback=self._callback,
@@ -447,28 +447,28 @@
             elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
                 self.pin.edge = self._dictTrigger[self._trigger]
                 self._stopWorker()
                 self._worker = Thread(target=self._workerLoop, name="GPIO worker")
                 self._worker.start()
                 self._fIntEnabled = True
             else:
-                ret = systypes.ErrorCode.errNotImplemented
+                ret = ErrorCode.errNotImplemented
         return ret
 
     def disableInterrupt(self):
         """Disables the gpio interrupt for that pin.
 
         Immediately disables the interrupt for that pin. It will not
         _fire an event anymore, unless :meth:`enableInterrupt` is called
         anew.
         
         :return: An error code indicating either success or the reason of failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         if self._fIntEnabled:
             if self._implpak == GPIO._IMPLPAK_RPIGPIO:
                 self._factory.remove_event_detect(self._designator)
                 self._fIntEnabled = False
             elif self._implpak == GPIO._IMPLPAK_GPIOZERO:
                 from gpiozero import CallbackSetToNone
 
@@ -478,17 +478,17 @@
                     self.pin.when_deactivated = None
                 self._fIntEnabled = False
             elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
                 self._stopWorker()
                 self.pin.edge = "none"
                 self._fIntEnabled = False
             else:
-                ret = systypes.ErrorCode.errNotImplemented
+                ret = ErrorCode.errNotImplemented
         else:
-            ret = systypes.ErrorCode.errOk
+            ret = ErrorCode.errOk
         return ret
 
     def get(self):
         """Retrieve the pin level.
 
         Gives the pin level, independent of whether the pin direction
         is set to input or output.
@@ -520,23 +520,23 @@
         Outputs the given level at this pin. Does not work, if this pin
         is set to input direction.
         
         :param int newLevel: The new level to set this pin to. Must be one of GPIO.LEVEL_[HIGH | LOW].
         :return: An error code indicating either success or the reason of failure.
         :rtype: ErrorCode
         """
-        ret = systypes.ErrorCode.errOk
+        ret = ErrorCode.errOk
         if self._implpak == GPIO._IMPLPAK_RPIGPIO:
             self._factory.output(self._designator, self._dictLevel[newLevel])
         elif self._implpak == GPIO._IMPLPAK_GPIOZERO:
             self.pin.value = self._dictLevel[newLevel]
         elif self._implpak == GPIO._IMPLPAK_PERIPHERY:
             self.pin.write(self._dictLevel[newLevel])
         elif self._implpak == GPIO._IMPLPAK_SIM:
             if newLevel == GPIO.LEVEL_HIGH:
                 self._level = GPIO.LEVEL_HIGH
             else:
                 self._level = GPIO.LEVEL_LOW
         else:
-            ret = systypes.ErrorCode.errNotImplemented
+            ret = ErrorCode.errNotImplemented
 
         return ret
```

### Comparing `philander-0.1.4/philander/htu21d.py` & `philander-0.1.5/philander/htu21d.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/hygrometer.py` & `philander-0.1.5/philander/hygrometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/imath.py` & `philander-0.1.5/philander/imath.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/interruptable.py` & `philander-0.1.5/philander/interruptable.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/led.py` & `philander-0.1.5/philander/led.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/max77960.py` & `philander-0.1.5/philander/max77960.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/max77960_reg.py` & `philander-0.1.5/philander/max77960_reg.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/module.py` & `philander-0.1.5/philander/module.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/primitives.py` & `philander-0.1.5/philander/primitives.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/sensor.py` & `philander-0.1.5/philander/sensor.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/serialbus.py` & `philander-0.1.5/philander/serialbus.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/simBMA456.py` & `philander-0.1.5/philander/simBMA456.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/simdev.py` & `philander-0.1.5/philander/simdev.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/systypes.py` & `philander-0.1.5/philander/systypes.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/thermometer.py` & `philander-0.1.5/philander/thermometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/vibrasense.py` & `philander-0.1.5/philander/vibrasense.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/vibrasense2.py` & `philander-0.1.5/philander/vibrasense2.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/voltmeter.py` & `philander-0.1.5/philander/voltmeter.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/watchdog.py` & `philander-0.1.5/philander/watchdog.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/fastgait/__init__.py` & `philander-0.1.5/philander/fastgait/__init__.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/fastgait/actorunit.py` & `philander-0.1.5/philander/fastgait/actorunit.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/philander/fastgait/sysman.py` & `philander-0.1.5/philander/fastgait/sysman.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/test/utgpio.py` & `philander-0.1.5/test/utgpio.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/test/utimath.py` & `philander-0.1.5/test/utimath.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/test/utserialbus.py` & `philander-0.1.5/test/utserialbus.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/LICENSE.txt` & `philander-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.4/pyproject.toml` & `philander-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "philander"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Oliver Maye", email="maye@ihp-microelectronics.com" },
 ]
 description = "Sensor and other parts driver collection"
 readme = "readme.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `philander-0.1.4/PKG-INFO` & `philander-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philander
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sensor and other parts driver collection
 Project-URL: Homepage, https://www.ihp-microelectronics.com/
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Oliver Maye <maye@ihp-microelectronics.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
```

