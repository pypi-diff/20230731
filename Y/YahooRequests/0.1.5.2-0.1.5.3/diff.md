# Comparing `tmp/YahooRequests-0.1.5.2.tar.gz` & `tmp/YahooRequests-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YahooRequests-0.1.5.2.tar", last modified: Fri Jul 21 11:57:31 2023, max compression
+gzip compressed data, was "YahooRequests-0.1.5.3.tar", last modified: Mon Jul 31 13:40:28 2023, max compression
```

## Comparing `YahooRequests-0.1.5.2.tar` & `YahooRequests-0.1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 11:57:31.144018 YahooRequests-0.1.5.2/
--rw-rw-rw-   0        0        0     1092 2023-07-19 12:31:31.000000 YahooRequests-0.1.5.2/LICENSE
--rw-rw-rw-   0        0        0     1092 2023-07-19 12:31:19.000000 YahooRequests-0.1.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1656 2023-07-21 11:57:31.145020 YahooRequests-0.1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-07-19 22:16:56.000000 YahooRequests-0.1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 11:57:31.122048 YahooRequests-0.1.5.2/YahooRequests.egg-info/
--rw-rw-rw-   0        0        0     1656 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      492 2023-07-21 11:57:31.152050 YahooRequests-0.1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-07-21 11:56:28.000000 YahooRequests-0.1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:57:31.141019 YahooRequests-0.1.5.2/yahoorequests/
--rw-rw-rw-   0        0        0       73 2023-07-20 21:20:43.000000 YahooRequests-0.1.5.2/yahoorequests/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-07-19 13:18:08.000000 YahooRequests-0.1.5.2/yahoorequests/yahoorequests.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 13:40:28.088552 YahooRequests-0.1.5.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.3/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1612 2023-07-31 13:40:28.088552 YahooRequests-0.1.5.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      716 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 13:40:28.088552 YahooRequests-0.1.5.3/YahooRequests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.3/YahooRequests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.3/YahooRequests/yahoorequests.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 13:40:28.088552 YahooRequests-0.1.5.3/YahooRequests.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1612 2023-07-31 13:40:28.000000 YahooRequests-0.1.5.3/YahooRequests.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2023-07-31 13:40:28.000000 YahooRequests-0.1.5.3/YahooRequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 13:40:28.000000 YahooRequests-0.1.5.3/YahooRequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       57 2023-07-31 13:40:28.000000 YahooRequests-0.1.5.3/YahooRequests.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-31 13:40:28.000000 YahooRequests-0.1.5.3/YahooRequests.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-07-31 13:40:28.000000 YahooRequests-0.1.5.3/YahooRequests.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-07-31 13:40:28.088552 YahooRequests-0.1.5.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1235 2023-07-31 13:39:54.000000 YahooRequests-0.1.5.3/setup.py
```

### Comparing `YahooRequests-0.1.5.2/LICENSE` & `YahooRequests-0.1.5.3/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 TheodorGajhede
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 TheodorGajhede
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `YahooRequests-0.1.5.2/LICENSE.txt` & `YahooRequests-0.1.5.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 TheodorGajhede
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 TheodorGajhede
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `YahooRequests-0.1.5.2/PKG-INFO` & `YahooRequests-0.1.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1
-Name: YahooRequests
-Version: 0.1.5.2
-Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
-Home-page: https://github.com/TheodorGajhede/YahooRequests
-Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/0.1.5.tar.gz
-Author: Theodor Gajhede
-Author-email: theodorgajhede@gmail.com
-License: MIT
-Keywords: Stocks,Ticker,Yahoo
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-
-# Yahoo Requests
-
-## By Theodor Gajhede from the northeren part of Denmark
-
-### This is a small library for getting prices and fullnames of companies using Yahoo
-
-### How to use
-
-    from YahooRequests import YahooRequests as yr    
-    # Now you can just print this value or assign it as a variable
-    yr.price("googl")
-    # The same goes for name
-    yr.name("googl")
-
-### YahooRequests.price(ticker)
-
-    It is very simple you are only required to input a ticker  and it will return the live price
-    the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
-
-### YahooRequests.convert(ticker)
-
-    The same goes for convert, the returned value will be the full company name
+Metadata-Version: 2.1
+Name: YahooRequests
+Version: 0.1.5.3
+Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
+Home-page: https://github.com/TheodorGajhede/YahooRequests
+Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/FIXED.tar.gz
+Author: Theodor Gajhede
+Author-email: theodorgajhede@gmail.com
+License: MIT
+Keywords: Stocks,Ticker,Yahoo
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
+
+# Yahoo Requests
+
+## By Theodor Gajhede from the northeren part of Denmark
+
+### This is a small library for getting prices and fullnames of companies using Yahoo
+
+### How to use
+
+    from YahooRequests import YahooRequests as yr    
+    # Now you can just print this value or assign it as a variable
+    yr.price("googl")
+    # The same goes for name
+    yr.name("googl")
+
+### YahooRequests.price(ticker)
+
+    It is very simple you are only required to input a ticker  and it will return the live price
+    the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
+
+### YahooRequests.convert(ticker)
+
+    The same goes for convert, the returned value will be the full company name
```

### Comparing `YahooRequests-0.1.5.2/README.md` & `YahooRequests-0.1.5.3/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Yahoo Requests
-
-## By Theodor Gajhede from the northeren part of Denmark
-
-### This is a small library for getting prices and fullnames of companies using Yahoo
-
-### How to use
-
-    from YahooRequests import YahooRequests as yr    
-    # Now you can just print this value or assign it as a variable
-    yr.price("googl")
-    # The same goes for name
-    yr.name("googl")
-
-### YahooRequests.price(ticker)
-
-    It is very simple you are only required to input a ticker  and it will return the live price
-    the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
-
-### YahooRequests.convert(ticker)
-
-    The same goes for convert, the returned value will be the full company name
+# Yahoo Requests
+
+## By Theodor Gajhede from the northeren part of Denmark
+
+### This is a small library for getting prices and fullnames of companies using Yahoo
+
+### How to use
+
+    from YahooRequests import YahooRequests as yr    
+    # Now you can just print this value or assign it as a variable
+    yr.price("googl")
+    # The same goes for name
+    yr.name("googl")
+
+### YahooRequests.price(ticker)
+
+    It is very simple you are only required to input a ticker  and it will return the live price
+    the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
+
+### YahooRequests.convert(ticker)
+
+    The same goes for convert, the returned value will be the full company name
```

### Comparing `YahooRequests-0.1.5.2/YahooRequests.egg-info/PKG-INFO` & `YahooRequests-0.1.5.3/YahooRequests.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1
-Name: YahooRequests
-Version: 0.1.5.2
-Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
-Home-page: https://github.com/TheodorGajhede/YahooRequests
-Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/0.1.5.tar.gz
-Author: Theodor Gajhede
-Author-email: theodorgajhede@gmail.com
-License: MIT
-Keywords: Stocks,Ticker,Yahoo
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-
-# Yahoo Requests
-
-## By Theodor Gajhede from the northeren part of Denmark
-
-### This is a small library for getting prices and fullnames of companies using Yahoo
-
-### How to use
-
-    from YahooRequests import YahooRequests as yr    
-    # Now you can just print this value or assign it as a variable
-    yr.price("googl")
-    # The same goes for name
-    yr.name("googl")
-
-### YahooRequests.price(ticker)
-
-    It is very simple you are only required to input a ticker  and it will return the live price
-    the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
-
-### YahooRequests.convert(ticker)
-
-    The same goes for convert, the returned value will be the full company name
+Metadata-Version: 2.1
+Name: YahooRequests
+Version: 0.1.5.3
+Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
+Home-page: https://github.com/TheodorGajhede/YahooRequests
+Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/FIXED.tar.gz
+Author: Theodor Gajhede
+Author-email: theodorgajhede@gmail.com
+License: MIT
+Keywords: Stocks,Ticker,Yahoo
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
+
+# Yahoo Requests
+
+## By Theodor Gajhede from the northeren part of Denmark
+
+### This is a small library for getting prices and fullnames of companies using Yahoo
+
+### How to use
+
+    from YahooRequests import YahooRequests as yr    
+    # Now you can just print this value or assign it as a variable
+    yr.price("googl")
+    # The same goes for name
+    yr.name("googl")
+
+### YahooRequests.price(ticker)
+
+    It is very simple you are only required to input a ticker  and it will return the live price
+    the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
+
+### YahooRequests.convert(ticker)
+
+    The same goes for convert, the returned value will be the full company name
```

### Comparing `YahooRequests-0.1.5.2/setup.py` & `YahooRequests-0.1.5.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from distutils.core import setup
-setup(
-    name='YahooRequests',
-    packages=['yahoorequests'],
-    version='0.1.5.2',
-    chmod=0o644,
-    license='MIT',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    description='A simple Python library for getting stock prices and company names from Yahoo Finance.',
-    author='Theodor Gajhede',
-    author_email='theodorgajhede@gmail.com',
-    url='https://github.com/TheodorGajhede/YahooRequests',
-    download_url='https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/0.1.5.tar.gz',
-    keywords=['Stocks', 'Ticker', 'Yahoo'],
-    install_requires=[
-          'requests'
-          ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',      # Define that your audience are developers
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',   # Again, pick a license
-        'Programming Language :: Python :: 3',      # Specify which pyhton versions that you want to support
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.8',
-            ],
-)
+from distutils.core import setup
+setup(
+    name='YahooRequests',
+    packages=['YahooRequests'],
+    version='0.1.5.3',
+    license='MIT',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    description='A simple Python library for getting stock prices and company names from Yahoo Finance.',
+    author='Theodor Gajhede',
+    author_email='theodorgajhede@gmail.com',
+    url='https://github.com/TheodorGajhede/YahooRequests',
+    download_url='https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/FIXED.tar.gz',
+    keywords=['Stocks', 'Ticker', 'Yahoo'],
+    install_requires=[
+          'requests'
+          ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',      # Define that your audience are developers
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',   # Again, pick a license
+        'Programming Language :: Python :: 3',      # Specify which pyhton versions that you want to support
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.8',
+            ],
+)
```

### Comparing `YahooRequests-0.1.5.2/yahoorequests/yahoorequests.py` & `YahooRequests-0.1.5.3/YahooRequests/yahoorequests.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import requests
-
-'''If you are one day trying to use this code and it does not work
-    it is up to god and you to fix it, becuase OC doesn't know what he is doing
-            - OC'''
-
-
-class ConvertError(Exception):
-    "Ticker could not be converted to companmy name please contact the creater"
-    pass
-
-
-class YahooRequests():
-    global url
-    global headers
-
-    # Define url for requesting data
-    url = 'https://query1.finance.yahoo.com/v7/finance/options/{}'
-
-    # Yahoo's api was shut down in 2017 so making a headers is required to look like a browser
-    headers = {
-        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)\
-        AppleWebKit/537.36 (KHTML, like Gecko)\
-        Chrome/108.0.0.0 Safari/537.36'
-        }
-
-    @staticmethod
-    def price(*ticker: str) -> int:
-        # Request url formatted as if the ticker is a str including headers for baiting as if a browser
-        response = requests.get(url.format(*ticker), headers=headers)
-        if response.status_code == 200:
-            # Unpack the data as a json type
-            data = response.json()
-            # return only the needed data
-            return data["optionChain"]["result"][0]["quote"]["regularMarketPrice"]
-        else:
-            # raise the custom convert error if the url could not be reached
-            # or any other error is raised when requesting
-            raise ConvertError
-
-    @staticmethod
-    def name(*ticker: str) -> str:
-        # Request url formatted as if the ticker is a str including headers for baiting as if a browser
-        response = requests.get(url.format(*ticker), headers=headers)
-        if response.status_code == 200:
-            # Unpack the data as a json type
-            data = response.json()
-            # return only the needed data
-            return data["optionChain"]["result"][0]["quote"]["shortName"]
-        else:
-            # raise the custom ConvertError
-            raise ConvertError()
-
-
-def main():
-    yahoo_requests = YahooRequests()
-    print(yahoo_requests.price("AAPL"))
-    print(yahoo_requests.name("AAPL"))
-
-
-if __name__ == "__main__":
-    main()
+import requests
+
+'''If you are one day trying to use this code and it does not work
+    it is up to god and you to fix it, becuase OC doesn't know what he is doing
+            - OC'''
+
+
+class ConvertError(Exception):
+    "Ticker could not be converted to companmy name please contact the creater"
+    pass
+
+
+class YahooRequests():
+    global url
+    global headers
+
+    # Define url for requesting data
+    url = 'https://query1.finance.yahoo.com/v7/finance/options/{}'
+
+    # Yahoo's api was shut down in 2017 so making a headers is required to look like a browser
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)\
+        AppleWebKit/537.36 (KHTML, like Gecko)\
+        Chrome/108.0.0.0 Safari/537.36'
+        }
+
+    @staticmethod
+    def price(*ticker: str) -> int:
+        # Request url formatted as if the ticker is a str including headers for baiting as if a browser
+        response = requests.get(url.format(*ticker), headers=headers)
+        if response.status_code == 200:
+            # Unpack the data as a json type
+            data = response.json()
+            # return only the needed data
+            return data["optionChain"]["result"][0]["quote"]["regularMarketPrice"]
+        else:
+            # raise the custom convert error if the url could not be reached
+            # or any other error is raised when requesting
+            raise ConvertError
+
+    @staticmethod
+    def name(*ticker: str) -> str:
+        # Request url formatted as if the ticker is a str including headers for baiting as if a browser
+        response = requests.get(url.format(*ticker), headers=headers)
+        if response.status_code == 200:
+            # Unpack the data as a json type
+            data = response.json()
+            # return only the needed data
+            return data["optionChain"]["result"][0]["quote"]["shortName"]
+        else:
+            # raise the custom ConvertError
+            raise ConvertError()
+
+
+def main():
+    yahoo_requests = YahooRequests()
+    print(yahoo_requests.price("AAPL"))
+    print(yahoo_requests.name("AAPL"))
+
+
+if __name__ == "__main__":
+    main()
```

