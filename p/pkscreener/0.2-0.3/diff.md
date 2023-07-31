# Comparing `tmp/pkscreener-0.2.tar.gz` & `tmp/pkscreener-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.2.tar", last modified: Sat Jul 29 00:06:24 2023, max compression
+gzip compressed data, was "pkscreener-0.3.tar", last modified: Mon Jul 31 10:23:54 2023, max compression
```

## Comparing `pkscreener-0.2.tar` & `pkscreener-0.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 00:06:24.946521 pkscreener-0.2/
--rw-rw-rw-   0        0        0     1086 2023-07-17 16:37:19.000000 pkscreener-0.2/LICENSE
--rw-rw-rw-   0        0        0     1091 2023-07-17 16:37:19.000000 pkscreener-0.2/LICENSE-Screenipy
--rw-rw-rw-   0        0        0    19969 2023-07-29 00:06:24.946521 pkscreener-0.2/PKG-INFO
--rw-rw-rw-   0        0        0    19092 2023-07-28 22:51:55.000000 pkscreener-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 00:06:24.869507 pkscreener-0.2/pkscreener/
--rw-rw-rw-   0        0        0     8732 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/Telegram.py
--rw-rw-rw-   0        0        0      421 2023-07-28 23:59:33.000000 pkscreener-0.2/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:06:24.943651 pkscreener-0.2/pkscreener/classes/
--rw-rw-rw-   0        0        0     1014 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Archiver.py
--rw-rw-rw-   0        0        0     3459 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    10043 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0      451 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0      391 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/ColorText.py
--rw-rw-rw-   0        0        0    11501 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9315 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11329 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     6311 2023-07-28 22:52:41.000000 pkscreener-0.2/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23029 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/ParallelProcessing.py
--rw-rw-rw-   0        0        0    11670 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0     4796 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/PortfolioTracker.py
--rw-rw-rw-   0        0        0    49315 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Screener.py
--rw-rw-rw-   0        0        0      947 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0      627 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/UserChoice.py
--rw-rw-rw-   0        0        0    30192 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0      421 2023-07-28 23:59:40.000000 pkscreener-0.2/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0    11228 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/log.py
--rw-rw-rw-   0        0        0     4038 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0    42838 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/globals.py
--rw-rw-rw-   0        0        0     7338 2023-07-28 22:51:55.000000 pkscreener-0.2/pkscreener/pkscreener.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:06:24.883505 pkscreener-0.2/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    19969 2023-07-29 00:06:22.000000 pkscreener-0.2/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2023-07-29 00:06:22.000000 pkscreener-0.2/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 00:06:22.000000 pkscreener-0.2/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-29 00:06:22.000000 pkscreener-0.2/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 23:10:34.000000 pkscreener-0.2/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      451 2023-07-29 00:06:22.000000 pkscreener-0.2/pkscreener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-29 00:06:22.000000 pkscreener-0.2/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-29 00:06:24.947544 pkscreener-0.2/setup.cfg
--rw-rw-rw-   0        0        0     2549 2023-07-29 00:06:15.000000 pkscreener-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:23:54.837229 pkscreener-0.3/
+-rw-rw-rw-   0        0        0     1086 2023-07-17 16:37:19.000000 pkscreener-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1091 2023-07-17 16:37:19.000000 pkscreener-0.3/LICENSE-Screenipy
+-rw-rw-rw-   0        0        0    20902 2023-07-31 10:23:54.846226 pkscreener-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    20025 2023-07-31 10:15:11.000000 pkscreener-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 10:23:54.781577 pkscreener-0.3/pkscreener/
+-rw-rw-rw-   0        0        0     8743 2023-07-31 09:45:36.000000 pkscreener-0.3/pkscreener/Telegram.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 09:23:44.000000 pkscreener-0.3/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:23:54.833222 pkscreener-0.3/pkscreener/classes/
+-rw-rw-rw-   0        0        0     1014 2023-07-31 09:47:22.000000 pkscreener-0.3/pkscreener/classes/Archiver.py
+-rw-rw-rw-   0        0        0     3470 2023-07-31 09:47:32.000000 pkscreener-0.3/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    10065 2023-07-31 09:47:41.000000 pkscreener-0.3/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0      473 2023-07-31 09:47:58.000000 pkscreener-0.3/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0      391 2023-07-28 22:51:55.000000 pkscreener-0.3/pkscreener/classes/ColorText.py
+-rw-rw-rw-   0        0        0    11523 2023-07-31 09:50:27.000000 pkscreener-0.3/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9348 2023-07-31 09:50:49.000000 pkscreener-0.3/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11362 2023-07-31 09:51:12.000000 pkscreener-0.3/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     6344 2023-07-31 09:56:15.000000 pkscreener-0.3/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23128 2023-07-31 09:52:16.000000 pkscreener-0.3/pkscreener/classes/ParallelProcessing.py
+-rw-rw-rw-   0        0        0    11692 2023-07-31 09:52:23.000000 pkscreener-0.3/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0     4796 2023-07-28 22:51:55.000000 pkscreener-0.3/pkscreener/classes/PortfolioTracker.py
+-rw-rw-rw-   0        0        0    49381 2023-07-31 09:52:43.000000 pkscreener-0.3/pkscreener/classes/Screener.py
+-rw-rw-rw-   0        0        0      947 2023-07-28 22:51:55.000000 pkscreener-0.3/pkscreener/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0      649 2023-07-31 09:52:53.000000 pkscreener-0.3/pkscreener/classes/UserChoice.py
+-rw-rw-rw-   0        0        0    30269 2023-07-31 09:53:20.000000 pkscreener-0.3/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0      421 2023-07-31 10:23:35.000000 pkscreener-0.3/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0    11228 2023-07-28 22:51:55.000000 pkscreener-0.3/pkscreener/classes/log.py
+-rw-rw-rw-   0        0        0     4038 2023-07-28 22:51:55.000000 pkscreener-0.3/pkscreener/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0    43003 2023-07-31 09:47:08.000000 pkscreener-0.3/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      228 2023-07-28 12:37:30.000000 pkscreener-0.3/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0     7470 2023-07-31 09:45:14.000000 pkscreener-0.3/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:23:54.791804 pkscreener-0.3/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    20902 2023-07-31 10:23:53.000000 pkscreener-0.3/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-07-31 10:23:53.000000 pkscreener-0.3/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:23:53.000000 pkscreener-0.3/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-31 10:23:53.000000 pkscreener-0.3/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 23:10:34.000000 pkscreener-0.3/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      592 2023-07-31 10:23:53.000000 pkscreener-0.3/pkscreener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 10:23:53.000000 pkscreener-0.3/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-31 10:23:54.848220 pkscreener-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2545 2023-07-31 10:02:20.000000 pkscreener-0.3/setup.py
```

### Comparing `pkscreener-0.2/LICENSE` & `pkscreener-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/LICENSE-Screenipy` & `pkscreener-0.3/LICENSE-Screenipy`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/PKG-INFO` & `pkscreener-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.2
+Version: 0.3
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.2.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.3.zip
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 
 
 # PKScreener
 
 [![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/pkjmesra/pkscreener/workflow-prod-scans_2.1.yml?logo=github)
-![github license](https://img.shields.io/pypi/l/gspread?logo=github)
+![github license](https://img.shields.io/pypi/l/gspread?logo=github) [![Downloads](https://static.pepy.tech/personalized-badge/pkscreener?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/pkscreener)
 ![latest download](https://img.shields.io/github/downloads-pre/pkjmesra/pkscreener/latest/total?logo=github)
 [![Documentation](https://readthedocs.org/projects/pkscreener/badge/?version=latest)](https://pkscreener.readthedocs.io/en/latest/?badge=latest) [![Docker Status](https://img.shields.io/docker/automated/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian)
 [![Docker Pulls](https://img.shields.io/docker/pulls/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian) [![3. Production Scan Tests On Dev](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml) [![4. After-Market Data Gen](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml) 
  [![PKScreener Test - New Features](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml/badge.svg?branch=new-features)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml) [![PKScreener Build - New Release](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml)
 [![Docker Build](https://github.com/pkjmesra/pkscreener/workflows/Docker%20Image%20CI/badge.svg)](https://github.com/pkjmesra/pkscreener/actions/workflows/docker-image.yml?query=workflow%3ADocker)
 
 ## What is PKScreener?
@@ -95,29 +95,34 @@
      5 > RSI screening                          6 > Reversal Signals
      7 > Stocks making Chart Patterns           8 > CCI outside of the given range
      9 > Volume gainers                         10 > Closing at least 2% up since last 3 days
     11 > Short term bullish stocks              12 > 15 Minute Price & Volume breakout
     13 > Bullish RSI & MACD Intraday            14 > NR4 Daily Today
 ```
 ## How to use on your own local Windows/Linux/Macbook laptop?
+# Installing the latest version from PyPi.
+* Go ahead and install using `pip install pkscreener`
+* This should install all of the major dependencies, except maybe, TA-Lib. 
+* This app can still run without TA-Lib, but if you need to install TA-Lib for technical indicators (which otherwise is used from `pandas_ta` in the absence of TA-Lib), you can do this: Head to `.github/dependencies/` under this repo. Download the respective TA-Lib file/whl file and install either from the .whl file or from source. Check out any of the workflow files for steps to install TA-Lib.
+* Now launch your favorite command line CLI and issue `pkscreener`. This will launch the pkscreener executable.
 
 # Using docker, running within docker container
 * Download and install docker desktop: https://docs.docker.com/get-docker/
 * After installation, launch/run docker desktop and if it asks, login using your docker credentials.
 * Launch any command line and type `docker pull pkjmesra/pkscreener-debian:latest`. Then type `docker run pkjmesra/pkscreener-debian:latest python3 pkscreener -a Y -o X:12:10 -e` ow whatever -o options you'd like executed.
 * Pass whatever option you'd like to pass in `-o`. Look at the menu options above. For, example, `12` is `Scanners.`. `10` `Closing at least 2% up since last 3 days` etc. Wait while it runs and produces the output for you.
 
 # Building from source repo
 * Install python 3.9 for your OS/CPU. Download the installer from https://www.python.org/downloads/release/python-3913/#Files
 * Just clone the repo with `git clone https://github.com/pkjmesra/PKScreener.git`
 * `cd PKScreener`
 * `pip install -r requirements.txt` .
 * (Optional) If you would like to have technical indicators evaluated using TA-Lib, go ahead and install TA-Lib as well.
 * `cd pkscreener`
-* Finally, from within the `pkscreener` directory, run `python pkscreener.py`. You are all set.
+* Finally, from within the `pkscreener` directory, run `python pkscreenercli.py`. You are all set.
 
 # Running the executables
 * Download the suitable file according to your OS.
 * Linux & Mac users should make sure that the `pkscreener.bin or pkscreener.run` is having `execute` permission.
 * **Run** the file. Following window will appear after a brief delay.
 
 
@@ -142,18 +147,18 @@
 You can now use the *Backtests* menu to backtest any of the selected strategies.
 ![backtest](https://raw.githubusercontent.com/pkjmesra/PKScreener/main/screenshots/backtest.png)
 
 * Once done, you can also view the output html file saved at the same location from where you launched the app.
 
 ## Scanning as a scheduled job once or at regular intervals
 * Running it once with pre-defined inputs
-You can also run it as a one time job in any scheduler with pre-defined options. For example `./pkscreener.py -a Y -o X:12:10 -e` (or `pkscreener.exe -a Y -o X:12:10 -e` if you're executing with the exe) will run the scanner for all Nifty stocks and find all stocks matching CCI filter, save the results in xlsx file and exit. `./pkscreener.py -a Y -o X:12:9:2.5 -e` will run the scanner (menu option `X`) for all Nifty stocks (menu option `12`) to find volume gainers (menu option `9`) with at least the volume multiplier of 2.5 (input variable `2.5`), save the results in xlsx file and exit (menu option `-e`). Passing in the `-p` option for example `pkscreener.py -a Y -p -o X:12:6:1 -e` will also silence all command line prints/outputs and just run silently for the given options, save results and exit. Try and see all options with `./pkscreener.py -h`.
+You can also run it as a one time job in any scheduler with pre-defined options. For example `./pkscreenercli.py -a Y -o X:12:10 -e` (or `pkscreener.exe -a Y -o X:12:10 -e` if you're executing with the exe) will run the scanner for all Nifty stocks and find all stocks matching CCI filter, save the results in xlsx file and exit. `./pkscreenercli.py -a Y -o X:12:9:2.5 -e` will run the scanner (menu option `X`) for all Nifty stocks (menu option `12`) to find volume gainers (menu option `9`) with at least the volume multiplier of 2.5 (input variable `2.5`), save the results in xlsx file and exit (menu option `-e`). Passing in the `-p` option for example `pkscreenercli.py -a Y -p -o X:12:6:1 -e` will also silence all command line prints/outputs and just run silently for the given options, save results and exit. Try and see all options with `./pkscreenercli.py -h`.
 
 * Running it at regular intervals
-If you want to runn it at regular intervals, you can just pass the interval in `-c` command line option. For example, `./pkscreener.py -a Y -o X:12:6:1 -c 180` will run it every `180` seconds with console outputs also being printed. If you'd just like it to run as a cron job without console outputs, you may also pass the `-p` parameter. For example, `./pkscreener.py -a Y -p -o X:12:6:1 -c 180`
+If you want to runn it at regular intervals, you can just pass the interval in `-c` command line option. For example, `./pkscreenercli.py -a Y -o X:12:6:1 -c 180` will run it every `180` seconds with console outputs also being printed. If you'd just like it to run as a cron job without console outputs, you may also pass the `-p` parameter. For example, `./pkscreenercli.py -a Y -p -o X:12:6:1 -c 180`
 
 ## Understanding the Result Table:
 
 The Result table contains a lot of different parameters which can be pretty overwhelming to the new users, so here's the description and significance of each parameter.
 
 | Sr | Parameter | Description | Example |
 |:---:|:---:|:---|:---|
@@ -194,15 +199,15 @@
 CHAT_ID=Your_Channel_Id_Here_Without_A_Hyphen_or_Minus_Sign
 TOKEN=Your_Bot_Token_Here
 chat_idADMIN=Your_Own_ID_Here
 ```
 3. From now on, you will begin to receive your own alerts on your telegram channel.
 
 ## Troubleshooting and Logs:
-If you are having issues running the program, you can just launch a command line interface (On windows> Start > Run > cmd) and then launch PKScreener with a command line option of `-l`. For example, `python pkscreener.py -l`. This will show you the path where the program will save all the log outputs from this run. Copy that path and go ahead and run the application. Altenatively, you can just go ahead and modify the `logsEnabled` value to `y`, save & close it and then run `python pkscreener.py`.
+If you are having issues running the program, you can just launch a command line interface (On windows> Start > Run > cmd) and then launch PKScreener with a command line option of `-l`. For example, `python pkscreenercli.py -l`. This will show you the path where the program will save all the log outputs from this run. Copy that path and go ahead and run the application. Altenatively, you can just go ahead and modify the `logsEnabled` value to `y`, save & close it and then run `python pkscreenercli.py`.
 
 After you have finished the run, go to that copied path, zip the contents of the file `pkscreener-logs.txt` and create an issue at https://github.com/pkjmesra/PKScreener/issues. Please do not forget to attach the log files in the issue.
 
 ## Contributing:
 * Please feel free to Suggest improvements bugs by creating an issue.
 * Please follow the [Guidelines for Contributing](https://github.com/pkjmesra/PKScreener/blob/main/CONTRIBUTING.md) while making a Pull Request.
```

### Comparing `pkscreener-0.2/README.md` & `pkscreener-0.3/pkscreener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,36 @@
+Metadata-Version: 2.1
+Name: pkscreener
+Version: 0.3
+Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
+Home-page: https://github.com/pkjmesra/pkscreener
+Author: pkjmesra
+Author-email: pkjmesra@gmail.com
+License: OSI Approved (MIT)
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.3.zip
+Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE-Screenipy
+
 
 # PKScreener
 
 [![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/pkjmesra/pkscreener/workflow-prod-scans_2.1.yml?logo=github)
-![github license](https://img.shields.io/pypi/l/gspread?logo=github)
+![github license](https://img.shields.io/pypi/l/gspread?logo=github) [![Downloads](https://static.pepy.tech/personalized-badge/pkscreener?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/pkscreener)
 ![latest download](https://img.shields.io/github/downloads-pre/pkjmesra/pkscreener/latest/total?logo=github)
 [![Documentation](https://readthedocs.org/projects/pkscreener/badge/?version=latest)](https://pkscreener.readthedocs.io/en/latest/?badge=latest) [![Docker Status](https://img.shields.io/docker/automated/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian)
 [![Docker Pulls](https://img.shields.io/docker/pulls/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian) [![3. Production Scan Tests On Dev](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml) [![4. After-Market Data Gen](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml) 
  [![PKScreener Test - New Features](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml/badge.svg?branch=new-features)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml) [![PKScreener Build - New Release](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml)
 [![Docker Build](https://github.com/pkjmesra/pkscreener/workflows/Docker%20Image%20CI/badge.svg)](https://github.com/pkjmesra/pkscreener/actions/workflows/docker-image.yml?query=workflow%3ADocker)
 
 ## What is PKScreener?
@@ -73,29 +95,34 @@
      5 > RSI screening                          6 > Reversal Signals
      7 > Stocks making Chart Patterns           8 > CCI outside of the given range
      9 > Volume gainers                         10 > Closing at least 2% up since last 3 days
     11 > Short term bullish stocks              12 > 15 Minute Price & Volume breakout
     13 > Bullish RSI & MACD Intraday            14 > NR4 Daily Today
 ```
 ## How to use on your own local Windows/Linux/Macbook laptop?
+# Installing the latest version from PyPi.
+* Go ahead and install using `pip install pkscreener`
+* This should install all of the major dependencies, except maybe, TA-Lib. 
+* This app can still run without TA-Lib, but if you need to install TA-Lib for technical indicators (which otherwise is used from `pandas_ta` in the absence of TA-Lib), you can do this: Head to `.github/dependencies/` under this repo. Download the respective TA-Lib file/whl file and install either from the .whl file or from source. Check out any of the workflow files for steps to install TA-Lib.
+* Now launch your favorite command line CLI and issue `pkscreener`. This will launch the pkscreener executable.
 
 # Using docker, running within docker container
 * Download and install docker desktop: https://docs.docker.com/get-docker/
 * After installation, launch/run docker desktop and if it asks, login using your docker credentials.
 * Launch any command line and type `docker pull pkjmesra/pkscreener-debian:latest`. Then type `docker run pkjmesra/pkscreener-debian:latest python3 pkscreener -a Y -o X:12:10 -e` ow whatever -o options you'd like executed.
 * Pass whatever option you'd like to pass in `-o`. Look at the menu options above. For, example, `12` is `Scanners.`. `10` `Closing at least 2% up since last 3 days` etc. Wait while it runs and produces the output for you.
 
 # Building from source repo
 * Install python 3.9 for your OS/CPU. Download the installer from https://www.python.org/downloads/release/python-3913/#Files
 * Just clone the repo with `git clone https://github.com/pkjmesra/PKScreener.git`
 * `cd PKScreener`
 * `pip install -r requirements.txt` .
 * (Optional) If you would like to have technical indicators evaluated using TA-Lib, go ahead and install TA-Lib as well.
 * `cd pkscreener`
-* Finally, from within the `pkscreener` directory, run `python pkscreener.py`. You are all set.
+* Finally, from within the `pkscreener` directory, run `python pkscreenercli.py`. You are all set.
 
 # Running the executables
 * Download the suitable file according to your OS.
 * Linux & Mac users should make sure that the `pkscreener.bin or pkscreener.run` is having `execute` permission.
 * **Run** the file. Following window will appear after a brief delay.
 
 
@@ -120,18 +147,18 @@
 You can now use the *Backtests* menu to backtest any of the selected strategies.
 ![backtest](https://raw.githubusercontent.com/pkjmesra/PKScreener/main/screenshots/backtest.png)
 
 * Once done, you can also view the output html file saved at the same location from where you launched the app.
 
 ## Scanning as a scheduled job once or at regular intervals
 * Running it once with pre-defined inputs
-You can also run it as a one time job in any scheduler with pre-defined options. For example `./pkscreener.py -a Y -o X:12:10 -e` (or `pkscreener.exe -a Y -o X:12:10 -e` if you're executing with the exe) will run the scanner for all Nifty stocks and find all stocks matching CCI filter, save the results in xlsx file and exit. `./pkscreener.py -a Y -o X:12:9:2.5 -e` will run the scanner (menu option `X`) for all Nifty stocks (menu option `12`) to find volume gainers (menu option `9`) with at least the volume multiplier of 2.5 (input variable `2.5`), save the results in xlsx file and exit (menu option `-e`). Passing in the `-p` option for example `pkscreener.py -a Y -p -o X:12:6:1 -e` will also silence all command line prints/outputs and just run silently for the given options, save results and exit. Try and see all options with `./pkscreener.py -h`.
+You can also run it as a one time job in any scheduler with pre-defined options. For example `./pkscreenercli.py -a Y -o X:12:10 -e` (or `pkscreener.exe -a Y -o X:12:10 -e` if you're executing with the exe) will run the scanner for all Nifty stocks and find all stocks matching CCI filter, save the results in xlsx file and exit. `./pkscreenercli.py -a Y -o X:12:9:2.5 -e` will run the scanner (menu option `X`) for all Nifty stocks (menu option `12`) to find volume gainers (menu option `9`) with at least the volume multiplier of 2.5 (input variable `2.5`), save the results in xlsx file and exit (menu option `-e`). Passing in the `-p` option for example `pkscreenercli.py -a Y -p -o X:12:6:1 -e` will also silence all command line prints/outputs and just run silently for the given options, save results and exit. Try and see all options with `./pkscreenercli.py -h`.
 
 * Running it at regular intervals
-If you want to runn it at regular intervals, you can just pass the interval in `-c` command line option. For example, `./pkscreener.py -a Y -o X:12:6:1 -c 180` will run it every `180` seconds with console outputs also being printed. If you'd just like it to run as a cron job without console outputs, you may also pass the `-p` parameter. For example, `./pkscreener.py -a Y -p -o X:12:6:1 -c 180`
+If you want to runn it at regular intervals, you can just pass the interval in `-c` command line option. For example, `./pkscreenercli.py -a Y -o X:12:6:1 -c 180` will run it every `180` seconds with console outputs also being printed. If you'd just like it to run as a cron job without console outputs, you may also pass the `-p` parameter. For example, `./pkscreenercli.py -a Y -p -o X:12:6:1 -c 180`
 
 ## Understanding the Result Table:
 
 The Result table contains a lot of different parameters which can be pretty overwhelming to the new users, so here's the description and significance of each parameter.
 
 | Sr | Parameter | Description | Example |
 |:---:|:---:|:---|:---|
@@ -172,20 +199,22 @@
 CHAT_ID=Your_Channel_Id_Here_Without_A_Hyphen_or_Minus_Sign
 TOKEN=Your_Bot_Token_Here
 chat_idADMIN=Your_Own_ID_Here
 ```
 3. From now on, you will begin to receive your own alerts on your telegram channel.
 
 ## Troubleshooting and Logs:
-If you are having issues running the program, you can just launch a command line interface (On windows> Start > Run > cmd) and then launch PKScreener with a command line option of `-l`. For example, `python pkscreener.py -l`. This will show you the path where the program will save all the log outputs from this run. Copy that path and go ahead and run the application. Altenatively, you can just go ahead and modify the `logsEnabled` value to `y`, save & close it and then run `python pkscreener.py`.
+If you are having issues running the program, you can just launch a command line interface (On windows> Start > Run > cmd) and then launch PKScreener with a command line option of `-l`. For example, `python pkscreenercli.py -l`. This will show you the path where the program will save all the log outputs from this run. Copy that path and go ahead and run the application. Altenatively, you can just go ahead and modify the `logsEnabled` value to `y`, save & close it and then run `python pkscreenercli.py`.
 
 After you have finished the run, go to that copied path, zip the contents of the file `pkscreener-logs.txt` and create an issue at https://github.com/pkjmesra/PKScreener/issues. Please do not forget to attach the log files in the issue.
 
 ## Contributing:
 * Please feel free to Suggest improvements bugs by creating an issue.
 * Please follow the [Guidelines for Contributing](https://github.com/pkjmesra/PKScreener/blob/main/CONTRIBUTING.md) while making a Pull Request.
 
 ## Disclaimer:
 * DO NOT use the results provided by the software 'solely' to make your trading decisions.
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * A lot of this work is based on the work of https://github.com/pranjal-joshi/Screeni-py. A big thank you!
+
+
```

### Comparing `pkscreener-0.2/pkscreener/Telegram.py` & `pkscreener-0.3/pkscreener/Telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from dotenv import dotenv_values
 
 import requests
 import pandas as pd
 from datetime import datetime
 
 from telegram.constants import ParseMode
-from classes.log import default_logger
+from pkscreener.classes.log import default_logger
 
 TOKEN = "00000000xxxxxxx"
 # URL_TELE = f"https://api.telegram.org/bot{TOKEN}/getUpdates"
 #**DOCU**
 # 5.2 Configure chatID and tokes in Telegram
 # Once the token has been obtained, the chatId of the users and the administrator must be obtained.
 # The users only receive purchase and startup alerts, while the administrator receives the alerts of the users as well as possible problems.
```

### Comparing `pkscreener-0.2/pkscreener/classes/Archiver.py` & `pkscreener-0.3/pkscreener/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/pkscreener/classes/Backtest.py` & `pkscreener-0.3/pkscreener/classes/Backtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from classes.ColorText import colorText
+from pkscreener.classes.ColorText import colorText
 
 def backtest(stock, data, screenedDict=None, periods=30,sampleDays=365, backTestedData = None):
     if stock == '' or data is None:
         print(f'No data/stock{(stock)} received for backtesting!')
         return
     if screenedDict is None or len(screenedDict) == 0:
         print(f'{(stock)}No backtesting strategy or screened dictionary received!')
```

### Comparing `pkscreener-0.2/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.3/pkscreener/classes/CandlePatterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
  *  Project             :   Screenipy
  *  Author              :   Pranjal Joshi
  *  Created             :   11/04/2021
  *  Description         :   Class for analyzing candle-stick patterns
 '''
 
 import pandas as pd
-from classes.Pktalib import pktalib
-from classes.ColorText import colorText
+from pkscreener.classes.Pktalib import pktalib
+from pkscreener.classes.ColorText import colorText
 
 class CandlePatterns:
 
     reversalPatternsBullish = ['Morning Star', 'Morning Doji Star', '3 Inside Up', 'Hammer', '3 White Soldiers', 'Bullish Engulfing', 'Dragonfly Doji', 'Supply Drought', 'Demand Rise']
     reversalPatternsBearish = ['Evening Star', 'Evening Doji Star', '3 Inside Down', 'Inverted Hammer', 'Hanging Man', '3 Black Crows', 'Bearish Engulfing', 'Shooting Star', 'Gravestone Doji']
 
     def __init__(self):
```

### Comparing `pkscreener-0.2/pkscreener/classes/ConfigManager.py` & `pkscreener-0.3/pkscreener/classes/ConfigManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import sys
 import os
 import string
 import glob
 import configparser
 from datetime import date
-from classes.ColorText import colorText
-from classes.log import default_logger
+from pkscreener.classes.ColorText import colorText
+from pkscreener.classes.log import default_logger
 
 parser = configparser.ConfigParser(strict=False)
 
 # Default attributes for Downloading Cache from Git repo
 default_period = '400d'
 default_duration = '1d'
```

### Comparing `pkscreener-0.2/pkscreener/classes/Fetcher.py` & `pkscreener-0.3/pkscreener/classes/Fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import csv
 import requests
 import random
 import os
 import yfinance as yf
 import pandas as pd
 from nsetools import Nse
-from classes.ColorText import colorText
-from classes.SuppressOutput import SuppressOutput
-from classes.log import default_logger
+from pkscreener.classes.ColorText import colorText
+from pkscreener.classes.SuppressOutput import SuppressOutput
+from pkscreener.classes.log import default_logger
 
 nse = Nse()
 
 # Exception class if yfinance stock delisted
 
 
 class StockDataEmptyException(Exception):
```

### Comparing `pkscreener-0.2/pkscreener/classes/MenuOptions.py` & `pkscreener-0.3/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
-from classes.ColorText import colorText
-import classes.ConfigManager as ConfigManager
-from classes.log import default_logger
+from pkscreener.classes.ColorText import colorText
+import pkscreener.classes.ConfigManager as ConfigManager
+from pkscreener.classes.log import default_logger
 
 configManager = ConfigManager.tools()
 
 level0MenuDict = {'X': 'Scanners', 
                   'S': 'Strategies',
                   'B': 'Backtests',
                   'T': '~',
```

### Comparing `pkscreener-0.2/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.3/pkscreener/classes/OtaUpdater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 '''
  *  Project             :   Screenipy
  *  Author              :   Pranjal Joshi
  *  Created             :   21/04/2021
  *  Description         :   Class for handling OTA updates
 '''
 
-from classes.ColorText import colorText
+from pkscreener.classes.ColorText import colorText
 import requests
 import os
 import platform
 import sys
 import subprocess
 import requests
-from classes import VERSION
-from classes.log import default_logger
+from pkscreener.classes import VERSION
+from pkscreener.classes.log import default_logger
 
 class OTAUpdater:
 
     developmentVersion = 'd'
 
     # Download and replace exe through other process for Windows
     def updateForWindows(url):
```

### Comparing `pkscreener-0.2/pkscreener/classes/ParallelProcessing.py` & `pkscreener-0.3/pkscreener/classes/ParallelProcessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 import numpy as np
 import sys
 import os
 import pytz
 import logging
 from queue import Empty
 from datetime import datetime
-from classes import Imports
-import classes.Fetcher as Fetcher
-import classes.Screener as Screener
-import classes.Utility as Utility
-from classes.CandlePatterns import CandlePatterns
-from classes.ColorText import colorText
-from classes.SuppressOutput import SuppressOutput
-from classes.log import default_logger, tracelog
-import classes.Archiver as Archiver
+from pkscreener.classes import Imports
+import pkscreener.classes.Fetcher as Fetcher
+import pkscreener.classes.Screener as Screener
+import pkscreener.classes.Utility as Utility
+from pkscreener.classes.CandlePatterns import CandlePatterns
+from pkscreener.classes.ColorText import colorText
+from pkscreener.classes.SuppressOutput import SuppressOutput
+from pkscreener.classes.log import default_logger, tracelog
+import pkscreener.classes.Archiver as Archiver
 
 # https://github.com/pyinstaller/pyinstaller/wiki/Recipe-Multiprocessing
 # Module multiprocessing is organized differently in Python 3.4+
 try:
     # Python 3.4+
     if sys.platform.startswith('win'):
         import multiprocessing.popen_spawn_win32 as forking
```

### Comparing `pkscreener-0.2/pkscreener/classes/Pktalib.py` & `pkscreener-0.3/pkscreener/classes/Pktalib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from classes import Imports
-from classes.log import default_logger
+from pkscreener.classes import Imports
+from pkscreener.classes.log import default_logger
 
 if Imports['talib']:
     import talib
 else:
     try:
         import pandas_ta as talib
     except Exception as e:
```

### Comparing `pkscreener-0.2/pkscreener/classes/PortfolioTracker.py` & `pkscreener-0.3/pkscreener/classes/PortfolioTracker.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/pkscreener/classes/Screener.py` & `pkscreener-0.3/pkscreener/classes/Screener.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 '''
 
 import sys
 import math
 import numpy as np
 import pandas as pd
 import joblib
-import classes.Utility as Utility
-from classes.Pktalib import pktalib
-from classes import Imports
-from classes.log import default_logger, tracelog
+import pkscreener.classes.Utility as Utility
+from pkscreener.classes.Pktalib import pktalib
+from pkscreener.classes import Imports
+from pkscreener.classes.log import default_logger, tracelog
 # from sklearn.preprocessing import StandardScaler
 if Imports['scipy']:
     from scipy.signal import argrelextrema
     from scipy.stats import linregress
-from classes.ColorText import colorText
-from classes.SuppressOutput import SuppressOutput
+from pkscreener.classes.ColorText import colorText
+from pkscreener.classes.SuppressOutput import SuppressOutput
 
 # Exception for only downloading stock data and not screening
 class DownloadDataOnly(Exception):
     pass
 
 # Exception for stocks which are not newly listed when screening only for Newly Listed
 class NotNewlyListed(Exception):
```

### Comparing `pkscreener-0.2/pkscreener/classes/SuppressOutput.py` & `pkscreener-0.3/pkscreener/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/pkscreener/classes/UserChoice.py` & `pkscreener-0.3/pkscreener/classes/UserChoice.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
-from classes.MenuOptions import menu, menus
-from classes.ColorText import colorText
+from pkscreener.classes.MenuOptions import menu, menus
+from pkscreener.classes.ColorText import colorText
 
 # This Class manages user menu choices
 class choices:
     level0MenuChoice = None
     level1MenuChoice = None
     level2MenuChoice = None
     level3MenuChoice = None
```

### Comparing `pkscreener-0.2/pkscreener/classes/Utility.py` & `pkscreener-0.3/pkscreener/classes/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 import platform
 import datetime
 import pytz
 import pickle
 import requests
 import time
 import joblib
-from classes import Imports
-from classes.log import default_logger
+from pkscreener.classes import Imports
+from pkscreener.classes.log import default_logger
 
 if Imports['keras']:
     import keras
 import warnings
 from PIL import Image, ImageDraw, ImageFont, ImageColor
 import pandas as pd
 from alive_progress import alive_bar
 from tabulate import tabulate
 from time import sleep
-from classes.ColorText import colorText
-from classes import VERSION
-from classes.Changelog import changelog
-import classes.ConfigManager as ConfigManager
-from classes.MenuOptions import menus, menu, MenuRenderStyle
+from pkscreener.classes.ColorText import colorText
+from pkscreener.classes import VERSION
+from pkscreener.classes.Changelog import changelog
+import pkscreener.classes.ConfigManager as ConfigManager
+from pkscreener.classes.MenuOptions import menus, menu, MenuRenderStyle
 
 artText = '''
     $$$$$$      $$   $$      $$$$$                                                        
     $$    $$    $$  $$      $$   $$                         $$$$       $$$$                  $$$$         
     $$    $$    $$$$$        $$$       $$$$$     $$ $$     $$  $$     $$  $$     $$$$$      $$  $$     $$ $$ 
     $$$$$$      $$  $$         $$$     $$        $$$ $     $$$$$$     $$$$$$     $$  $$     $$$$$$     $$$ $ 
     $$          $$   $$     $$   $$    $$        $$        $$         $$         $$  $$     $$         $$
```

### Comparing `pkscreener-0.2/pkscreener/classes/log.py` & `pkscreener-0.3/pkscreener/classes/log.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/pkscreener/classes/multiprocessing_logging.py` & `pkscreener-0.3/pkscreener/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.2/pkscreener/globals.py` & `pkscreener-0.3/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 import sys
 import logging
 # import dataframe_image as dfi
 # import df2img
 
-import classes.Fetcher as Fetcher
-import classes.ConfigManager as ConfigManager
-from classes.OtaUpdater import OTAUpdater
-from classes import VERSION
-from classes.log import default_logger, tracelog
-import classes.Screener as Screener
-import classes.Utility as Utility
-from classes.ColorText import colorText
-from classes.CandlePatterns import CandlePatterns
-from classes.MenuOptions import menu, menus, level0MenuDict, level1_X_MenuDict, level2_X_MenuDict, level3_X_Reversal_MenuDict, level3_X_ChartPattern_MenuDict
-from classes.ParallelProcessing import StockConsumer
-from classes.Utility import level3ReversalMenuDict, level3ChartPatternMenuDict
+import pkscreener.classes.Fetcher as Fetcher
+import pkscreener.classes.ConfigManager as ConfigManager
+from pkscreener.classes.OtaUpdater import OTAUpdater
+from pkscreener.classes import VERSION
+from pkscreener.classes.log import default_logger, tracelog
+import pkscreener.classes.Screener as Screener
+import pkscreener.classes.Utility as Utility
+from pkscreener.classes.ColorText import colorText
+from pkscreener.classes.CandlePatterns import CandlePatterns
+from pkscreener.classes.MenuOptions import menu, menus, level0MenuDict, level1_X_MenuDict, level2_X_MenuDict, level3_X_Reversal_MenuDict, level3_X_ChartPattern_MenuDict
+from pkscreener.classes.ParallelProcessing import StockConsumer
+from pkscreener.classes.Utility import level3ReversalMenuDict, level3ChartPatternMenuDict
 # import classes.Archiver as Archiver
 
 from alive_progress import alive_bar
 import urllib
 import numpy as np
 import pandas as pd
 from datetime import datetime
-import classes.PortfolioTracker as tracker
-from classes.Backtest import backtest
+import pkscreener.classes.PortfolioTracker as tracker
+from pkscreener.classes.Backtest import backtest
 from time import sleep
 from tabulate import tabulate
-from Telegram import send_message, send_photo, send_document, is_token_telegram_configured
+from pkscreener.Telegram import send_message, send_photo, send_document, is_token_telegram_configured
 import multiprocessing
 multiprocessing.freeze_support()
 
 # Try Fixing bug with this symbol
 TEST_STKCODE = "SBIN"
 
 # Constants
```

### Comparing `pkscreener-0.2/pkscreener/pkscreener.py` & `pkscreener-0.3/pkscreener/pkscreenercli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Keep module imports prior to classes
 import os
 import sys
 import multiprocessing
 import argparse
 import builtins
 import tempfile
+sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 
 def decorator(func):
     def new_func(*args,**kwargs):
         return
         # if printenabled:
         #     func("print:",*args,**kwargs)
         #     func("input:",*args,**kwargs)
@@ -22,18 +23,18 @@
 def disableSysOut(input=True):
     builtins.print = decorator(builtins.print)  # all files
     if input:
         builtins.input = decorator(builtins.input)  # all files
     sys.stdout = open(os.devnull, 'w')
     sys.__stdout__ = open(os.devnull, 'w')
 
-import classes.log as log
-from classes.log import default_logger
-from classes.ColorText import colorText
-import classes.ConfigManager as ConfigManager
+from pkscreener.classes import log as log
+from pkscreener.classes.log import default_logger
+from pkscreener.classes.ColorText import colorText
+import pkscreener.classes.ConfigManager as ConfigManager
 from time import sleep
 import multiprocessing
 multiprocessing.freeze_support()
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
 # Argument Parsing for test purpose
@@ -71,16 +72,16 @@
         multiprocessing.set_start_method('fork')
     configManager.getConfig(ConfigManager.parser)
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild:
             input(f'Press any key to continue...')
-    from globals import main
-    import classes.Utility as Utility
+    from pkscreener.globals import main
+    import pkscreener.classes.Utility as Utility
     
     configManager.default_logger = default_logger()
     Utility.tools.clearScreen()
 
     if args.prodbuild:
         disableSysOut()
```

### Comparing `pkscreener-0.2/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,14 @@
-Metadata-Version: 2.1
-Name: pkscreener
-Version: 0.2
-Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
-Home-page: https://github.com/pkjmesra/pkscreener
-Author: pkjmesra
-Author-email: pkjmesra@gmail.com
-License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.2.zip
-Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE-Screenipy
-
 
 # PKScreener
 
 [![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.01/pkscreener.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/pkjmesra/pkscreener/workflow-prod-scans_2.1.yml?logo=github)
-![github license](https://img.shields.io/pypi/l/gspread?logo=github)
+![github license](https://img.shields.io/pypi/l/gspread?logo=github) [![Downloads](https://static.pepy.tech/personalized-badge/pkscreener?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/pkscreener)
 ![latest download](https://img.shields.io/github/downloads-pre/pkjmesra/pkscreener/latest/total?logo=github)
 [![Documentation](https://readthedocs.org/projects/pkscreener/badge/?version=latest)](https://pkscreener.readthedocs.io/en/latest/?badge=latest) [![Docker Status](https://img.shields.io/docker/automated/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian)
 [![Docker Pulls](https://img.shields.io/docker/pulls/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian) [![3. Production Scan Tests On Dev](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml) [![4. After-Market Data Gen](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml) 
  [![PKScreener Test - New Features](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml/badge.svg?branch=new-features)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml) [![PKScreener Build - New Release](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml)
 [![Docker Build](https://github.com/pkjmesra/pkscreener/workflows/Docker%20Image%20CI/badge.svg)](https://github.com/pkjmesra/pkscreener/actions/workflows/docker-image.yml?query=workflow%3ADocker)
 
 ## What is PKScreener?
@@ -95,29 +73,34 @@
      5 > RSI screening                          6 > Reversal Signals
      7 > Stocks making Chart Patterns           8 > CCI outside of the given range
      9 > Volume gainers                         10 > Closing at least 2% up since last 3 days
     11 > Short term bullish stocks              12 > 15 Minute Price & Volume breakout
     13 > Bullish RSI & MACD Intraday            14 > NR4 Daily Today
 ```
 ## How to use on your own local Windows/Linux/Macbook laptop?
+# Installing the latest version from PyPi.
+* Go ahead and install using `pip install pkscreener`
+* This should install all of the major dependencies, except maybe, TA-Lib. 
+* This app can still run without TA-Lib, but if you need to install TA-Lib for technical indicators (which otherwise is used from `pandas_ta` in the absence of TA-Lib), you can do this: Head to `.github/dependencies/` under this repo. Download the respective TA-Lib file/whl file and install either from the .whl file or from source. Check out any of the workflow files for steps to install TA-Lib.
+* Now launch your favorite command line CLI and issue `pkscreener`. This will launch the pkscreener executable.
 
 # Using docker, running within docker container
 * Download and install docker desktop: https://docs.docker.com/get-docker/
 * After installation, launch/run docker desktop and if it asks, login using your docker credentials.
 * Launch any command line and type `docker pull pkjmesra/pkscreener-debian:latest`. Then type `docker run pkjmesra/pkscreener-debian:latest python3 pkscreener -a Y -o X:12:10 -e` ow whatever -o options you'd like executed.
 * Pass whatever option you'd like to pass in `-o`. Look at the menu options above. For, example, `12` is `Scanners.`. `10` `Closing at least 2% up since last 3 days` etc. Wait while it runs and produces the output for you.
 
 # Building from source repo
 * Install python 3.9 for your OS/CPU. Download the installer from https://www.python.org/downloads/release/python-3913/#Files
 * Just clone the repo with `git clone https://github.com/pkjmesra/PKScreener.git`
 * `cd PKScreener`
 * `pip install -r requirements.txt` .
 * (Optional) If you would like to have technical indicators evaluated using TA-Lib, go ahead and install TA-Lib as well.
 * `cd pkscreener`
-* Finally, from within the `pkscreener` directory, run `python pkscreener.py`. You are all set.
+* Finally, from within the `pkscreener` directory, run `python pkscreenercli.py`. You are all set.
 
 # Running the executables
 * Download the suitable file according to your OS.
 * Linux & Mac users should make sure that the `pkscreener.bin or pkscreener.run` is having `execute` permission.
 * **Run** the file. Following window will appear after a brief delay.
 
 
@@ -142,18 +125,18 @@
 You can now use the *Backtests* menu to backtest any of the selected strategies.
 ![backtest](https://raw.githubusercontent.com/pkjmesra/PKScreener/main/screenshots/backtest.png)
 
 * Once done, you can also view the output html file saved at the same location from where you launched the app.
 
 ## Scanning as a scheduled job once or at regular intervals
 * Running it once with pre-defined inputs
-You can also run it as a one time job in any scheduler with pre-defined options. For example `./pkscreener.py -a Y -o X:12:10 -e` (or `pkscreener.exe -a Y -o X:12:10 -e` if you're executing with the exe) will run the scanner for all Nifty stocks and find all stocks matching CCI filter, save the results in xlsx file and exit. `./pkscreener.py -a Y -o X:12:9:2.5 -e` will run the scanner (menu option `X`) for all Nifty stocks (menu option `12`) to find volume gainers (menu option `9`) with at least the volume multiplier of 2.5 (input variable `2.5`), save the results in xlsx file and exit (menu option `-e`). Passing in the `-p` option for example `pkscreener.py -a Y -p -o X:12:6:1 -e` will also silence all command line prints/outputs and just run silently for the given options, save results and exit. Try and see all options with `./pkscreener.py -h`.
+You can also run it as a one time job in any scheduler with pre-defined options. For example `./pkscreenercli.py -a Y -o X:12:10 -e` (or `pkscreener.exe -a Y -o X:12:10 -e` if you're executing with the exe) will run the scanner for all Nifty stocks and find all stocks matching CCI filter, save the results in xlsx file and exit. `./pkscreenercli.py -a Y -o X:12:9:2.5 -e` will run the scanner (menu option `X`) for all Nifty stocks (menu option `12`) to find volume gainers (menu option `9`) with at least the volume multiplier of 2.5 (input variable `2.5`), save the results in xlsx file and exit (menu option `-e`). Passing in the `-p` option for example `pkscreenercli.py -a Y -p -o X:12:6:1 -e` will also silence all command line prints/outputs and just run silently for the given options, save results and exit. Try and see all options with `./pkscreenercli.py -h`.
 
 * Running it at regular intervals
-If you want to runn it at regular intervals, you can just pass the interval in `-c` command line option. For example, `./pkscreener.py -a Y -o X:12:6:1 -c 180` will run it every `180` seconds with console outputs also being printed. If you'd just like it to run as a cron job without console outputs, you may also pass the `-p` parameter. For example, `./pkscreener.py -a Y -p -o X:12:6:1 -c 180`
+If you want to runn it at regular intervals, you can just pass the interval in `-c` command line option. For example, `./pkscreenercli.py -a Y -o X:12:6:1 -c 180` will run it every `180` seconds with console outputs also being printed. If you'd just like it to run as a cron job without console outputs, you may also pass the `-p` parameter. For example, `./pkscreenercli.py -a Y -p -o X:12:6:1 -c 180`
 
 ## Understanding the Result Table:
 
 The Result table contains a lot of different parameters which can be pretty overwhelming to the new users, so here's the description and significance of each parameter.
 
 | Sr | Parameter | Description | Example |
 |:---:|:---:|:---|:---|
@@ -194,22 +177,20 @@
 CHAT_ID=Your_Channel_Id_Here_Without_A_Hyphen_or_Minus_Sign
 TOKEN=Your_Bot_Token_Here
 chat_idADMIN=Your_Own_ID_Here
 ```
 3. From now on, you will begin to receive your own alerts on your telegram channel.
 
 ## Troubleshooting and Logs:
-If you are having issues running the program, you can just launch a command line interface (On windows> Start > Run > cmd) and then launch PKScreener with a command line option of `-l`. For example, `python pkscreener.py -l`. This will show you the path where the program will save all the log outputs from this run. Copy that path and go ahead and run the application. Altenatively, you can just go ahead and modify the `logsEnabled` value to `y`, save & close it and then run `python pkscreener.py`.
+If you are having issues running the program, you can just launch a command line interface (On windows> Start > Run > cmd) and then launch PKScreener with a command line option of `-l`. For example, `python pkscreenercli.py -l`. This will show you the path where the program will save all the log outputs from this run. Copy that path and go ahead and run the application. Altenatively, you can just go ahead and modify the `logsEnabled` value to `y`, save & close it and then run `python pkscreenercli.py`.
 
 After you have finished the run, go to that copied path, zip the contents of the file `pkscreener-logs.txt` and create an issue at https://github.com/pkjmesra/PKScreener/issues. Please do not forget to attach the log files in the issue.
 
 ## Contributing:
 * Please feel free to Suggest improvements bugs by creating an issue.
 * Please follow the [Guidelines for Contributing](https://github.com/pkjmesra/PKScreener/blob/main/CONTRIBUTING.md) while making a Pull Request.
 
 ## Disclaimer:
 * DO NOT use the results provided by the software 'solely' to make your trading decisions.
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * A lot of this work is based on the work of https://github.com/pranjal-joshi/Screeni-py. A big thank you!
-
-
```

### Comparing `pkscreener-0.2/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.3/pkscreener.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 LICENSE-Screenipy
 README.md
 setup.cfg
 setup.py
 pkscreener/Telegram.py
 pkscreener/__init__.py
 pkscreener/globals.py
-pkscreener/pkscreener.py
+pkscreener/pkscreener.ini
+pkscreener/pkscreenercli.py
 pkscreener.egg-info/PKG-INFO
 pkscreener.egg-info/SOURCES.txt
 pkscreener.egg-info/dependency_links.txt
 pkscreener.egg-info/entry_points.txt
 pkscreener.egg-info/not-zip-safe
 pkscreener.egg-info/requires.txt
 pkscreener.egg-info/top_level.txt
```

### Comparing `pkscreener-0.2/setup.py` & `pkscreener-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from distutils.core import setup
 from pkscreener.classes import VERSION
 
 __USERNAME__ = 'pkjmesra'
 
 with open('README.md', 'r') as fh:
 	long_description = fh.read()
-with open('requirements-alpine.txt', 'r') as fh:
+with open('requirements.txt', 'r') as fh:
 	install_requires = fh.read().splitlines()
 
 SYS_MAJOR_VERSION = str(sys.version_info.major)
 SYS_VERSION = SYS_MAJOR_VERSION + '.' +str(sys.version_info.minor)
 
 WHEEL_NAME = 'pkscreener-'+VERSION+'-py'+SYS_MAJOR_VERSION+'-none-any.whl'
 TAR_FILE = 'pkscreener-'+VERSION+'.tar.gz'
@@ -51,15 +51,15 @@
 	author = __USERNAME__,
 	author_email = __USERNAME__+'@gmail.com',
 	license = 'OSI Approved (MIT)',
 	url = 'https://github.com/'+__USERNAME__+'/pkscreener', # use the URL to the github repo
 	zip_safe=False,
 	entry_points='''
 	[console_scripts]
-	pkscreener=pkscreener.pkscreener:pkscreenercli
+	pkscreener=pkscreener.pkscreenercli:pkscreenercli
 	''',
 	download_url = 'https://github.com/'+__USERNAME__+'/pkscreener/archive/v' + VERSION + '.zip',
 	classifiers=[
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: Microsoft :: Windows",
 	"Operating System :: MacOS",
 	"Operating System :: POSIX :: Linux",
```

