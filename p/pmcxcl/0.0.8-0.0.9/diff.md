# Comparing `tmp/pmcxcl-0.0.8-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/pmcxcl-0.0.9-pp39-pypy39_pp73-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 871555 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  1817600 b- defN 23-Jul-30 19:08 _pmcxcl.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-30 19:05 pmcxcl/__init__.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-30 19:05 pmcxcl/bench.py
--rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      535 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/RECORD
-7 files, 1830878 bytes uncompressed, 870621 bytes compressed:  52.4%
+Zip file size: 526648 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx   903664 b- defN 23-Jul-31 03:22 _pmcxcl.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx     1584 b- defN 23-Jul-31 03:21 pmcxcl/__init__.py
+-rw-r--r--  2.0 unx     1691 b- defN 23-Jul-31 03:21 pmcxcl/bench.py
+-rw-r--r--  2.0 unx     8344 b- defN 23-Jul-31 03:22 pmcxcl-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-31 03:22 pmcxcl-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-31 03:22 pmcxcl-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 23-Jul-31 03:22 pmcxcl-0.0.9.dist-info/RECORD
+7 files, 915944 bytes uncompressed, 525722 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: _pmcxcl.pypy39-pp73-win_amd64.pyd
+Filename: _pmcxcl.pypy39-pp73-darwin.so
 Comment: 
 
 Filename: pmcxcl/__init__.py
 Comment: 
 
 Filename: pmcxcl/bench.py
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/METADATA
+Filename: pmcxcl-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/WHEEL
+Filename: pmcxcl-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/top_level.txt
+Filename: pmcxcl-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/RECORD
+Filename: pmcxcl-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmcxcl/__init__.py

 * *Ordering differences only*

```diff
@@ -1,42 +1,42 @@
-# Copyright (c) 2022-2023 Matin Raayai Ardakani <raayaiardakani.m at northeastern.edu>. All rights reserved.
-# Copyright (c) 2022-2023 Qianqian Fang <q.fang at neu.edu>. All rights reserved.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""PMCXCL - Python bindings for Monte Carlo eXtreme photon transport simulator
-
-Example usage:
-
-# To list available GPUs
-import pmcxcl
-pmcxcl.gpuinfo()
-
-# To run a simulation
-res = pmcxcl.run(nphoton=1000000, vol=np.ones([60, 60, 60], dtype='uint8'),
-               tstart=0, tend=5e-9, tstep=5e-9, srcpos=[30,30,0],
-               srcdir=[0,0,1], prop=np.array([[0, 0, 1, 1], [0.005, 1, 0.01, 1.37]]))
-"""
-
-try:
-    from _pmcxcl import gpuinfo, run
-except ImportError:  # pragma: no cover
-    print("the pmcxcl binary extension (_pmcxcl) is not compiled! please compile first")
-
-# from .utils import detweight, cwdref
-# from .files import loadmc2, loadmch, load, save
-from .bench import bench
-
-__version__ = "0.0.8"
-
-__all__ = ("gpuinfo", "run", "bench")
+# Copyright (c) 2022-2023 Matin Raayai Ardakani <raayaiardakani.m at northeastern.edu>. All rights reserved.
+# Copyright (c) 2022-2023 Qianqian Fang <q.fang at neu.edu>. All rights reserved.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""PMCXCL - Python bindings for Monte Carlo eXtreme photon transport simulator
+
+Example usage:
+
+# To list available GPUs
+import pmcxcl
+pmcxcl.gpuinfo()
+
+# To run a simulation
+res = pmcxcl.run(nphoton=1000000, vol=np.ones([60, 60, 60], dtype='uint8'),
+               tstart=0, tend=5e-9, tstep=5e-9, srcpos=[30,30,0],
+               srcdir=[0,0,1], prop=np.array([[0, 0, 1, 1], [0.005, 1, 0.01, 1.37]]))
+"""
+
+try:
+    from _pmcxcl import gpuinfo, run
+except ImportError:  # pragma: no cover
+    print("the pmcxcl binary extension (_pmcxcl) is not compiled! please compile first")
+
+# from .utils import detweight, cwdref
+# from .files import loadmc2, loadmch, load, save
+from .bench import bench
+
+__version__ = "0.0.8"
+
+__all__ = ("gpuinfo", "run", "bench")
```

## pmcxcl/bench.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-# Copyright (c) 2022-2023 Matin Raayai Ardakani <raayaiardakani.m at northeastern.edu>. All rights reserved.
-# Copyright (c) 2022-2023 Qianqian Fang <q.fang at neu.edu>. All rights reserved.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""Built-in benchmark configurations"""
-
-import numpy as np
-import copy
-
-bench = {}
-bench["cube60"] = {
-    "nphoton": 1000000,
-    "vol": np.ones([60, 60, 60], dtype="uint8"),
-    "tstart": 0,
-    "tend": 5e-9,
-    "tstep": 5e-9,
-    "srcpos": [29, 29, 0],
-    "srcdir": [0, 0, 1],
-    "prop": [[0, 0, 1, 1], [0.005, 1, 0.01, 1.37], [0.002, 5, 0.9, 1]],
-    "isreflect": 0,
-    "seed": 1648335518,
-    "session": "cube60",
-    "detpos": [[29, 19, 0, 1], [29, 39, 0, 1], [19, 29, 0, 1], [39, 29, 0, 1]],
-    "issrcfrom0": 1,
-}
-
-bench["cube60b"] = copy.deepcopy(bench["cube60"])
-bench["cube60b"]["isreflect"] = 1
-
-bench["cube60planar"] = copy.deepcopy(bench["cube60b"])
-bench["cube60planar"]["srctype"] = "planar"
-bench["cube60planar"]["srcpos"] = [10, 10, -10]
-bench["cube60planar"]["srcparam1"] = [40, 0, 0, 0]
-bench["cube60planar"]["srcparam2"] = [0, 40, 0, 0]
+# Copyright (c) 2022-2023 Matin Raayai Ardakani <raayaiardakani.m at northeastern.edu>. All rights reserved.
+# Copyright (c) 2022-2023 Qianqian Fang <q.fang at neu.edu>. All rights reserved.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""Built-in benchmark configurations"""
+
+import numpy as np
+import copy
+
+bench = {}
+bench["cube60"] = {
+    "nphoton": 1000000,
+    "vol": np.ones([60, 60, 60], dtype="uint8"),
+    "tstart": 0,
+    "tend": 5e-9,
+    "tstep": 5e-9,
+    "srcpos": [29, 29, 0],
+    "srcdir": [0, 0, 1],
+    "prop": [[0, 0, 1, 1], [0.005, 1, 0.01, 1.37], [0.002, 5, 0.9, 1]],
+    "isreflect": 0,
+    "seed": 1648335518,
+    "session": "cube60",
+    "detpos": [[29, 19, 0, 1], [29, 39, 0, 1], [19, 29, 0, 1], [39, 29, 0, 1]],
+    "issrcfrom0": 1,
+}
+
+bench["cube60b"] = copy.deepcopy(bench["cube60"])
+bench["cube60b"]["isreflect"] = 1
+
+bench["cube60planar"] = copy.deepcopy(bench["cube60b"])
+bench["cube60planar"]["srctype"] = "planar"
+bench["cube60planar"]["srcpos"] = [10, 10, -10]
+bench["cube60planar"]["srcparam1"] = [40, 0, 0, 0]
+bench["cube60planar"]["srcparam2"] = [0, 40, 0, 0]
```

## Comparing `pmcxcl-0.0.8.dist-info/METADATA` & `pmcxcl-0.0.9.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,156 @@
-Metadata-Version: 2.1
-Name: pmcxcl
-Version: 0.0.8
-Summary: Python bindings for Monte Carlo eXtreme photon transport simulator
-Home-page: https://github.com/fangq/mcxcl
-Author: Matin Raayai Ardakani, Qianqian Fang
-Author-email: raayaiardakani.m@northeastern.edu, q.fang@neu.edu
-Maintainer: Qianqian Fang
-License: GPLv3+
-Download-URL: http://mcx.space
-Keywords: Monte Carlo simulation,Biophotonics,Ray-tracing,Rendering,GPU,Modeling,Biomedical Optics,Tissue Optics,Simulator,Optics
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Environment :: GPU
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires: numpy
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-![](http://mcx.space/img/mcx18_banner.png)
-
-# PMCX-CL - Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
-
-- Copyright: (C) Matin Raayai Ardakani (2022-2023) <raayaiardakani.m at northeastern.edu> 
-and Qianqian Fang (2019-2023) <q.fang at neu.edu>
-- License: GNU Public License V3 or later
-- Version: 0.0.8
-- URL: https://pypi.org/project/pmcxcl/
-- Github: https://github.com/fangq/mcxcl
-
-![Linux Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_linux_manywheel.yml/badge.svg)\
-![MacOS Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_macos_wheel.yml/badge.svg)\
-![Windows Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_windows_wheel.yml/badge.svg)\
-![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
-
-This module provides a Python binding for Monte Carlo eXtreme for OpenCL (MCXCL).
-For other binaries, including the standalone executable and the MATLAB bindings,
-see [our website](https://mcx.space).
-
-Monte Carlo eXtreme (MCX) is a fast photon transport simulation software for 3D 
-heterogeneous turbid media. By taking advantage of the massively parallel 
-threads and extremely low memory latency in a modern graphics processing unit 
-(GPU), MCX is capable of performing Monte Carlo (MC) photon simulations at a 
-blazing speed, typically hundreds to a thousand times faster than a single-threaded
-CPU-based MC implementation.
-
-## How to Install
-
-* PIP: ```pip install pmcxcl```
-
-## Runtime Dependencies
-* **CPU or GPU**: An OpenCL-capable CPU or GPU; most modern CPUs or GPUs support OpenCL -
-an industrial-standard heterogeneous computing library and specification (https://www.khronos.org/opencl/)
-* **OpenCL CPU or GPU runtime/driver**: Both NVIDIA and AMD GPU graphics drivers should contain
-out-of-box OpenCL runtimes or drivers; for Intel GPUs, one should install additional OpenCL runtime
-support from https://github.com/intel/compute-runtime or install the `intel-opencl-icd` package
-if the OS provides (such as Ubuntu 22.04); one can also install an open-source OpenCL runtime
-[POCL](http://portablecl.org/), using package manager such as `sudo apt-get install pocl-opencl-icd`. However,
-POCL's support is largely limited to CPUs. You **do not need** to install CUDA SDK to use pmcxcl.
-* **Python**: Python 3.6 and newer is required. **Python 2 is not supported**.
-* **numpy**: Used to pass/receive volumetric information to/from pmcxcl. To install, use either conda or pip 
-package managers: `pip install numpy` or `conda install numpy`
-* (optional) **jdata**: Only needed to read/write JNIfTI output files. To install, use pip: `pip install jdata` 
-on all operating systems; For Debian-based Linux distributions, you can also install to the system interpreter 
-using apt-get: `sudo apt-get install python3-jdata`. See https://pypi.org/project/jdata/ for more details. 
-* (optional) **bjdata**: Only needed to read/write BJData/UBJSON files. To install, run `pip install bjdata` 
-on all operating systems; For Debian-based Linux distributions, you can also install to the system interpreter 
-using apt-get: `sudo apt-get install python3-bjdata`. See https://pypi.org/project/bjdata/ for more details. 
-* (optional) **matplotlib**: For plotting the results. To install, run either `pip install matplotlib` or
-`conda install matplotlib`
-
-## Build Instructions
-
-### Build Dependencies
-* **Operating System**: pmcxcl and mcxcl can be compiled on most OSes, including Windows, Linux and MacOS.
-* **OpenCL library**: compiling mcxcl or pmcxcl requires to link with `libOpenCL.so` on Linux, or `libOpenCL.dylib`
-on MacOS or `OpenCL.dll` on Windows. These libraries should have been installed by either graphics driver or
-OpenCL runtimes.
-* **Python Interpreter**: Python 3.6 or above. The ```pip``` Python package manager and the ```wheel``` package (available
-  via ```pip```) are not required but recommended.
-* **C/C++ Compiler**: pmcxcl can be compiled using a wide variety of C compilers, including
-  * GNU GCC for Linux, MacOS (intalled via MacPorts or brew), and Windows (installed via msys2, mingw64 or cygwin64)
-  * Microsoft Visual Studio C/C++ Compiler for Windows.
-  * Apple Clang for macOS, available via Xcode.
-
-  Refer to each OS's online documentations for more in-depth information on how to install these compilers.
-  MacOS provides built-in OpenCL library support.
-* **OpenMP**: The installed C/C++ Compiler should have support for [OpenMP](https://www.openmp.org/). 
-  GCC and Microsoft Visual Studio compiler support OpenMP out of the box. Apple Clang, however, requires manual 
-  installation of OpenMP libraries for Apple Clang. The easiest way to do this is via the [Brew](https://brew.sh/) package
-  manager, preferably after selecting the correct Xcode version:
-  ```zsh
-    brew install libomp
-    brew link --force libomp
-  ```
-* **CMake**: CMake version 3.15 and later is required. Refer to the [CMake website](https://cmake.org/download/) for more information on how to download.
-  CMake is also widely available on package managers across all operating systems.
-* **Zlib Compression Development Headers**: On Linux, this is generally available via the built-in package manager. For 
-  example, on Debian-based distributions like Ubuntu it is available via ```apt``` under the name ```zlib1g-dev```. On
-  macOS, brew provides it under the name ```zlib```. No packaged versions of Zlib are available for windows, therefore it must be
-  downloaded manually and added to the CMake environment variables in your working Powershell session:
-  ```powershell
-    curl.exe --retry 3 -kL https://cytranet.dl.sourceforge.net/project/gnuwin32/zlib/1.2.3/zlib-1.2.3-lib.zip --output zlib.zip
-    Expand-Archive .\zlib.zip -DestinationPath zlib\
-    $env:CMAKE_INCLUDE_PATH=$PWD\zlib\include
-    $env:CMAKE_LIBRARY_PATH=$PWD\zlib\lib
-  ```
-
-### Build Steps
-1. Ensure that ```cmake```, ```python``` and the C/C++ compiler are all located over your ```PATH```.
-This can be queried via ```echo $env:PATH``` on Windows or ```echo $PATH``` on Linux. If not, locate them and add their folder to the ```PATH```.
-
-2. Clone the repository and switch to the ```pmcxcl/``` folder:
-    ```bash
-        git clone --recursive https://github.com/fangq/mcx.git
-        cd mcx/pmcxcl
-    ```
-3. Run ```pip wheel .``` inside the `pmcxcl` folder to locally build the Python wheel without installing it
-4. One can also run ```python setup.py install``` or ```pip install .``` to build and directly install the compiled package
-
-
-## How to use
-
-The PMCXCL module is easy to use. You can use the `pmcxcl.gpuinfo()` function to first verify
-if you have NVIDIA/CUDA compatible GPUs installed; if there are NVIDIA GPUs detected,
-you can then call the `run()` function to launch a photon simulation.
-
-A simulation can be defined conveniently in two approaches - a one-liner and a two-liner:
-
-* For the one-liner, one simply pass on each MCX simulation setting as positional
-argument. The supported setting names are compatible to nearly all the input fields
-for the MATLAB version of MCX/MCXCL - [MCXLAB](https://github.com/fangq/mcx/blob/master/mcxlab/mcxlab.m))
-
-```python3
-import pmcxcl
-import numpy as np
-import matplotlib.pyplot as plt
-
-res = pmcxcl.run(nphoton=1000000, vol=np.ones([60, 60, 60], dtype='uint8'), tstart=0, tend=5e-9, 
-               tstep=5e-9, srcpos=[30,30,0], srcdir=[0,0,1], prop=np.array([[0, 0, 1, 1], [0.005, 1, 0.01, 1.37]]))
-res['flux'].shape
-
-plt.imshow(np.log10(res['flux'][30,:, :]))
-plt.show()
-```
-
-* Alternatively, one can also define a Python dict object containing each setting
-as a key, and pass on the dict object to `pmcxcl.run()`
-
-```python3
-import pmcxcl
-import numpy as np
-cfg = {'nphoton': 1000000, 'vol':np.ones([60,60,60],dtype='uint8'), 'tstart':0, 'tend':5e-9, 'tstep':5e-9,
-       'srcpos': [30,30,0], 'srcdir':[0,0,1], 'prop':[[0,0,1,1],[0.005,1,0.01,1.37]]}
-res = pmcxcl.run(cfg)
-```
-
-
+Metadata-Version: 2.1
+Name: pmcxcl
+Version: 0.0.9
+Summary: Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
+Home-page: https://github.com/fangq/mcxcl
+Author: Matin Raayai Ardakani, Qianqian Fang
+Author-email: raayaiardakani.m@northeastern.edu, q.fang@neu.edu
+Maintainer: Qianqian Fang
+License: GPLv3+
+Download-URL: http://mcx.space
+Keywords: Monte Carlo simulation,Biophotonics,Ray-tracing,Rendering,GPU,Modeling,Biomedical Optics,Tissue Optics,Simulator,Optics,OpenCL
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Environment :: GPU
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires: numpy
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+![](http://mcx.space/img/mcx18_banner.png)
+
+# PMCX-CL - Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
+
+- Copyright: (C) Matin Raayai Ardakani (2022-2023) <raayaiardakani.m at northeastern.edu> 
+and Qianqian Fang (2019-2023) <q.fang at neu.edu>
+- License: GNU Public License V3 or later
+- Version: 0.0.9
+- URL: https://pypi.org/project/pmcxcl/
+- Github: https://github.com/fangq/mcxcl
+
+![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
+![Linux Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_linux_manywheel.yml/badge.svg)\
+![MacOS Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_macos_wheel.yml/badge.svg)\
+![Windows Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_windows_wheel.yml/badge.svg)\
+
+This module provides a Python binding for Monte Carlo eXtreme for OpenCL (MCXCL).
+For other binaries, including the standalone executable and the MATLAB bindings,
+see [our website](https://mcx.space).
+
+Monte Carlo eXtreme (MCX) is a fast photon transport simulation software for 3D 
+heterogeneous turbid media. By taking advantage of the massively parallel 
+threads and extremely low memory latency in a modern graphics processing unit 
+(GPU), MCX is capable of performing Monte Carlo (MC) photon simulations at a 
+blazing speed, typically hundreds to a thousand times faster than a single-threaded
+CPU-based MC implementation.
+
+## How to Install
+
+* PIP: ```pip install pmcxcl```
+
+## Runtime Dependencies
+* **CPU or GPU**: An OpenCL-capable CPU or GPU; most modern CPUs or GPUs support OpenCL -
+an industrial-standard heterogeneous computing library and specification (https://www.khronos.org/opencl/)
+* **OpenCL CPU or GPU runtime/driver**: Both NVIDIA and AMD GPU graphics drivers should contain
+out-of-box OpenCL runtimes or drivers; for Intel GPUs, one should install additional OpenCL runtime
+support from https://github.com/intel/compute-runtime or install the `intel-opencl-icd` package
+if the OS provides (such as Ubuntu 22.04); one can also install an open-source OpenCL runtime
+[POCL](http://portablecl.org/), using package manager such as `sudo apt-get install pocl-opencl-icd`. However,
+POCL's support is largely limited to CPUs. You **do not need** to install CUDA SDK to use pmcxcl.
+* **Python**: Python 3.6 and newer is required. **Python 2 is not supported**.
+* **numpy**: Used to pass/receive volumetric information to/from pmcxcl. To install, use either conda or pip 
+package managers: `pip install numpy` or `conda install numpy`
+* (optional) **jdata**: Only needed to read/write JNIfTI output files. To install, use pip: `pip install jdata` 
+on all operating systems; For Debian-based Linux distributions, you can also install to the system interpreter 
+using apt-get: `sudo apt-get install python3-jdata`. See https://pypi.org/project/jdata/ for more details. 
+* (optional) **bjdata**: Only needed to read/write BJData/UBJSON files. To install, run `pip install bjdata` 
+on all operating systems; For Debian-based Linux distributions, you can also install to the system interpreter 
+using apt-get: `sudo apt-get install python3-bjdata`. See https://pypi.org/project/bjdata/ for more details. 
+* (optional) **matplotlib**: For plotting the results. To install, run either `pip install matplotlib` or
+`conda install matplotlib`
+
+## Build Instructions
+
+### Build Dependencies
+* **Operating System**: pmcxcl and mcxcl can be compiled on most OSes, including Windows, Linux and MacOS.
+* **OpenCL library**: compiling mcxcl or pmcxcl requires to link with `libOpenCL.so` on Linux, or `libOpenCL.dylib`
+on MacOS or `OpenCL.dll` on Windows. These libraries should have been installed by either graphics driver or
+OpenCL runtimes.
+* **Python Interpreter**: Python 3.6 or above. The ```pip``` Python package manager and the ```wheel``` package (available
+  via ```pip```) are not required but recommended.
+* **C/C++ Compiler**: pmcxcl can be compiled using a wide variety of C compilers, including
+  * GNU GCC for Linux, MacOS (intalled via MacPorts or brew), and Windows (installed via msys2, mingw64 or cygwin64)
+  * Microsoft Visual Studio C/C++ Compiler for Windows.
+  * Apple Clang for macOS, available via Xcode.
+
+  Refer to each OS's online documentations for more in-depth information on how to install these compilers.
+  MacOS provides built-in OpenCL library support.
+* **OpenMP**: The installed C/C++ Compiler should have support for [OpenMP](https://www.openmp.org/). 
+  GCC and Microsoft Visual Studio compiler support OpenMP out of the box. Apple Clang, however, requires manual 
+  installation of OpenMP libraries for Apple Clang. The easiest way to do this is via the [Brew](https://brew.sh/) package
+  manager, preferably after selecting the correct Xcode version:
+  ```zsh
+    brew install libomp
+    brew link --force libomp
+  ```
+* **CMake**: CMake version 3.15 and later is required. Refer to the [CMake website](https://cmake.org/download/) for more information on how to download.
+  CMake is also widely available on package managers across all operating systems.
+
+### Build Steps
+1. Ensure that ```cmake```, ```python``` and the C/C++ compiler are all located over your ```PATH```.
+This can be queried via ```echo $env:PATH``` on Windows or ```echo $PATH``` on Linux. If not, locate them and add their folder to the ```PATH```.
+
+2. Clone the repository and switch to the ```pmcxcl/``` folder:
+    ```bash
+        git clone --recursive https://github.com/fangq/mcx.git
+        cd mcx/pmcxcl
+    ```
+3. Run ```pip wheel .``` inside the `pmcxcl` folder to locally build the Python wheel without installing it
+4. One can also run ```python setup.py install``` or ```pip install .``` to build and directly install the compiled package
+
+
+## How to use
+
+The PMCXCL module is easy to use. You can use the `pmcxcl.gpuinfo()` function to first verify
+if you have NVIDIA/CUDA compatible GPUs installed; if there are NVIDIA GPUs detected,
+you can then call the `run()` function to launch a photon simulation.
+
+A simulation can be defined conveniently in two approaches - a one-liner and a two-liner:
+
+* For the one-liner, one simply pass on each MCX simulation setting as positional
+argument. The supported setting names are compatible to nearly all the input fields
+for the MATLAB version of MCX/MCXCL - [MCXLAB](https://github.com/fangq/mcx/blob/master/mcxlab/mcxlab.m))
+
+```python3
+import pmcxcl
+import numpy as np
+import matplotlib.pyplot as plt
+
+res = pmcxcl.run(nphoton=1000000, vol=np.ones([60, 60, 60], dtype='uint8'), tstart=0, tend=5e-9, 
+               tstep=5e-9, srcpos=[30,30,0], srcdir=[0,0,1], prop=np.array([[0, 0, 1, 1], [0.005, 1, 0.01, 1.37]]))
+res['flux'].shape
+
+plt.imshow(np.log10(res['flux'][30,:, :]))
+plt.show()
+```
+
+* Alternatively, one can also define a Python dict object containing each setting
+as a key, and pass on the dict object to `pmcxcl.run()`
+
+```python3
+import pmcxcl
+import numpy as np
+cfg = {'nphoton': 1000000, 'vol':np.ones([60,60,60],dtype='uint8'), 'tstart':0, 'tend':5e-9, 'tstep':5e-9,
+       'srcpos': [30,30,0], 'srcdir':[0,0,1], 'prop':[[0,0,1,1],[0.005,1,0.01,1.37]]}
+res = pmcxcl.run(cfg)
+```
+
+
```

