# Comparing `tmp/clientele-0.3.1.tar.gz` & `tmp/clientele-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.3.1.tar", max compression
+gzip compressed data, was "clientele-0.3.2.tar", max compression
```

## Comparing `clientele-0.3.1.tar` & `clientele-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.3.1/LICENSE
--rw-r--r--   0        0        0     1310 2023-07-25 03:26:20.606725 clientele-0.3.1/README.md
--rw-r--r--   0        0        0      898 2023-07-25 22:19:00.792847 clientele-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.3.1/src/__init__.py
--rw-r--r--   0        0        0     1896 2023-07-25 03:26:44.875798 clientele-0.3.1/src/cli.py
--rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.3.1/src/constants_template.py
--rw-r--r--   0        0        0     2055 2023-07-24 23:26:23.378037 clientele-0.3.1/src/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.3.1/src/generators/__init__.py
--rw-r--r--   0        0        0     7660 2023-07-25 22:22:46.450989 clientele-0.3.1/src/generators/clients.py
--rw-r--r--   0        0        0     2997 2023-07-25 21:56:31.511282 clientele-0.3.1/src/generators/http.py
--rw-r--r--   0        0        0     3577 2023-07-25 22:09:26.862604 clientele-0.3.1/src/generators/schemas.py
--rw-r--r--   0        0        0      190 2023-07-25 22:18:53.608786 clientele-0.3.1/src/settings.py
--rw-r--r--   0        0        0       61 2023-07-24 20:44:55.813864 clientele-0.3.1/src/template/MANIFEST
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.3.1/src/template/__init__.py
--rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.3.1/src/template/client.py
--rw-r--r--   0        0        0      974 2023-07-25 22:23:05.603189 clientele-0.3.1/src/template/http.py
--rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.3.1/src/template/schemas.py
--rw-r--r--   0        0        0     2107 2023-07-25 22:16:25.551674 clientele-0.3.1/src/utils.py
--rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.3.1/src/writer.py
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 clientele-0.3.1/setup.py
--rw-r--r--   0        0        0     2152 1970-01-01 00:00:00.000000 clientele-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1742 2023-07-30 22:05:13.221961 clientele-0.3.2/README.md
+-rw-r--r--   0        0        0      898 2023-07-30 21:43:47.060546 clientele-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.3.2/src/__init__.py
+-rw-r--r--   0        0        0     1896 2023-07-25 03:26:44.875798 clientele-0.3.2/src/cli.py
+-rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.3.2/src/constants_template.py
+-rw-r--r--   0        0        0     2055 2023-07-24 23:26:23.378037 clientele-0.3.2/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.3.2/src/generators/__init__.py
+-rw-r--r--   0        0        0     7681 2023-07-30 22:01:28.730710 clientele-0.3.2/src/generators/clients.py
+-rw-r--r--   0        0        0     2997 2023-07-25 21:56:31.511282 clientele-0.3.2/src/generators/http.py
+-rw-r--r--   0        0        0     3815 2023-07-30 22:01:28.702712 clientele-0.3.2/src/generators/schemas.py
+-rw-r--r--   0        0        0      190 2023-07-30 21:43:40.188450 clientele-0.3.2/src/settings.py
+-rw-r--r--   0        0        0       61 2023-07-24 20:44:55.813864 clientele-0.3.2/src/template/MANIFEST
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.3.2/src/template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.3.2/src/template/client.py
+-rw-r--r--   0        0        0      974 2023-07-25 22:23:05.603189 clientele-0.3.2/src/template/http.py
+-rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.3.2/src/template/schemas.py
+-rw-r--r--   0        0        0     2202 2023-07-30 21:39:17.797808 clientele-0.3.2/src/utils.py
+-rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.3.2/src/writer.py
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 clientele-0.3.2/PKG-INFO
```

### Comparing `clientele-0.3.1/LICENSE` & `clientele-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/README.md` & `clientele-0.3.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,109 @@
-00000000: 2320 e29a 9cef b88f 2043 6c69 656e 7465  # ...... Cliente
-00000010: 6c65 0a0a 2320 5479 7065 6420 4150 4920  le..# Typed API 
-00000020: 436c 6965 6e74 7320 6672 6f6d 204f 7065  Clients from Ope
-00000030: 6e41 5049 2073 6368 656d 6173 0a0a 215b  nAPI schemas..![
-00000040: 636c 6965 6e74 656c 655f 6c6f 676f 5d28  clientele_logo](
-00000050: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000060: 6f6d 2f62 6563 6b65 7474 2d73 6f66 7477  om/beckett-softw
-00000070: 6172 652f 636c 6965 6e74 656c 652f 626c  are/clientele/bl
-00000080: 6f62 2f6d 6169 6e2f 646f 6373 2f63 6c69  ob/main/docs/cli
-00000090: 656e 7465 6c65 2e6a 7065 673f 7261 773d  entele.jpeg?raw=
-000000a0: 7472 7565 290a 0a43 6c69 656e 7465 6c65  true)..Clientele
-000000b0: 206c 6574 7320 796f 7520 6765 6e65 7261   lets you genera
-000000c0: 7465 2066 756c 6c79 2d74 7970 6564 2c20  te fully-typed, 
-000000d0: 6675 6e63 7469 6f6e 616c 2c20 4150 4920  functional, API 
-000000e0: 436c 6965 6e74 7320 6672 6f6d 204f 7065  Clients from Ope
-000000f0: 6e41 5049 2073 6368 656d 6173 2e0a 0a49  nAPI schemas...I
-00000100: 7420 7573 6573 206d 6f64 6572 6e20 746f  t uses modern to
-00000110: 6f6c 7320 746f 2062 6520 626c 617a 696e  ols to be blazin
-00000120: 6720 6661 7374 2061 6e64 2074 7970 6520  g fast and type 
-00000130: 7361 6665 2e0a 0a50 6c75 7320 2d20 7468  safe...Plus - th
-00000140: 6572 6520 6973 206e 6f20 636f 6d70 6c65  ere is no comple
-00000150: 7820 626f 696c 6572 706c 6174 6520 616e  x boilerplate an
-00000160: 6420 7468 6520 6765 6e65 7261 7465 6420  d the generated 
-00000170: 636f 6465 2069 7320 7665 7279 2073 6d61  code is very sma
-00000180: 6c6c 2e0a 0a23 2320 4665 6174 7572 6573  ll...## Features
-00000190: 0a0a 2a20 4675 6c6c 7920 7479 7065 6420  ..* Fully typed 
-000001a0: 4150 4920 436c 6965 6e74 2075 7369 6e67  API Client using
-000001b0: 2050 7964 616e 7469 632e 0a2a 204d 696e   Pydantic..* Min
-000001c0: 696d 616c 6973 7420 616e 6420 6561 7379  imalist and easy
-000001d0: 2074 6f20 7573 6520 2d20 7468 6520 6765   to use - the ge
-000001e0: 6e65 7261 7465 6420 636f 6465 2069 7320  nerated code is 
-000001f0: 6465 7369 676e 6564 2066 6f72 2072 6561  designed for rea
-00000200: 6461 6269 6c69 7479 2e0a 2a20 4368 6f6f  dability..* Choo
-00000210: 7365 2065 6974 6865 7220 7379 6e63 206f  se either sync o
-00000220: 7220 6173 796e 6320 2d20 7765 2073 7570  r async - we sup
-00000230: 706f 7274 2062 6f74 682c 2061 6e64 2079  port both, and y
-00000240: 6f75 2063 616e 2073 7769 7463 6820 6265  ou can switch be
-00000250: 7477 6565 6e20 7468 656d 2065 6173 696c  tween them easil
-00000260: 792e 0a2a 2053 7570 706f 7274 7320 6175  y..* Supports au
-00000270: 7468 656e 7469 6361 7469 6f6e 2028 6375  thentication (cu
-00000280: 7265 6e74 6c79 206f 6e6c 7920 4854 5450  rently only HTTP
-00000290: 2042 6561 7265 7220 616e 6420 4854 5450   Bearer and HTTP
-000002a0: 2042 6173 6963 2061 7574 6829 2e0a 2a20   Basic auth)..* 
-000002b0: 5772 6974 7465 6e20 656e 7469 7265 6c79  Written entirely
-000002c0: 2069 6e20 5079 7468 6f6e 202d 206e 6f20   in Python - no 
-000002d0: 6e65 6564 2074 6f20 696e 7374 616c 6c20  need to install 
-000002e0: 6f74 6865 7220 6c61 6e67 7561 6765 7320  other languages 
-000002f0: 746f 2075 7365 204f 7065 6e41 5049 2e0a  to use OpenAPI..
-00000300: 2a20 5468 6520 636c 6965 6e74 2066 6f6f  * The client foo
-00000310: 7470 7269 6e74 2069 7320 6d69 6e69 6d61  tprint is minima
-00000320: 6c20 2d20 6974 206f 6e6c 7920 7265 7175  l - it only requ
-00000330: 6972 6573 2060 6874 7470 7860 2061 6e64  ires `httpx` and
-00000340: 2060 7079 6461 6e74 6963 602e 0a2a 2053   `pydantic`..* S
-00000350: 7570 706f 7274 7320 796f 7572 206f 776e  upports your own
-00000360: 2063 6f6e 6669 6775 7261 7469 6f6e 202d   configuration -
-00000370: 2077 6520 7072 6f76 6964 6520 616e 2065   we provide an e
-00000380: 6e74 7279 2070 6f69 6e74 2074 6861 7420  ntry point that 
-00000390: 7769 6c6c 206e 6576 6572 2062 6520 6f76  will never be ov
-000003a0: 6572 7772 6974 7465 6e2e 0a0a 5765 2772  erwritten...We'r
-000003b0: 6520 6275 696c 7420 6f6e 3a0a 0a2a 205b  e built on:..* [
-000003c0: 5079 6461 6e74 6963 2032 2e30 5d28 6874  Pydantic 2.0](ht
-000003d0: 7470 733a 2f2f 646f 6373 2e70 7964 616e  tps://docs.pydan
-000003e0: 7469 632e 6465 762f 6c61 7465 7374 2f29  tic.dev/latest/)
-000003f0: 0a2a 205b 6874 7470 785d 2868 7474 7073  .* [httpx](https
-00000400: 3a2f 2f77 7777 2e70 7974 686f 6e2d 6874  ://www.python-ht
-00000410: 7470 782e 6f72 672f 290a 2a20 5b6f 7065  tpx.org/).* [ope
-00000420: 6e61 7069 2d63 6f72 655d 2868 7474 7073  napi-core](https
-00000430: 3a2f 2f6f 7065 6e61 7069 2d63 6f72 652e  ://openapi-core.
-00000440: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000450: 6e2f 6c61 7465 7374 2f29 0a0a 2323 2049  n/latest/)..## I
-00000460: 6e73 7461 6c6c 0a0a 6060 6073 680a 706f  nstall..```sh.po
-00000470: 6574 7279 2061 6464 2063 6c69 656e 7465  etry add cliente
-00000480: 6c65 0a60 6060 0a0a 2323 2055 7361 6765  le.```..## Usage
-00000490: 0a0a 6060 6073 680a 636c 6965 6e74 656c  ..```sh.clientel
-000004a0: 6520 6765 6e65 7261 7465 202d 6620 7061  e generate -f pa
-000004b0: 7468 2f74 6f2f 6669 6c65 2e6a 736f 6e20  th/to/file.json 
-000004c0: 2d6f 206d 795f 636c 6965 6e74 2f20 2d2d  -o my_client/ --
-000004d0: 6173 796e 6369 6f20 740a 6060 600a 0a5b  asyncio t.```..[
-000004e0: 5265 6164 2074 6865 2064 6f63 735d 2868  Read the docs](h
-000004f0: 7474 7073 3a2f 2f62 6563 6b65 7474 2d73  ttps://beckett-s
-00000500: 6f66 7477 6172 652e 6769 7468 7562 2e69  oftware.github.i
-00000510: 6f2f 636c 6965 6e74 656c 652f 290a       o/clientele/).
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 2020 203c 6831 3ee2 9a9c efb8  ">.    <h1>.....
+00000020: 8f20 436c 6965 6e74 656c 653c 2f68 313e  . Clientele</h1>
+00000030: 0a20 2020 203c 656d 3e54 7970 6564 2041  .    <em>Typed A
+00000040: 5049 2043 6c69 656e 7473 2066 726f 6d20  PI Clients from 
+00000050: 4f70 656e 4150 4920 7363 6865 6d61 733c  OpenAPI schemas<
+00000060: 2f65 6d3e 0a20 2020 203c 696d 6720 7372  /em>.    <img sr
+00000070: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000080: 622e 636f 6d2f 6265 636b 6574 742d 736f  b.com/beckett-so
+00000090: 6674 7761 7265 2f63 6c69 656e 7465 6c65  ftware/clientele
+000000a0: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+000000b0: 636c 6965 6e74 656c 652e 6a70 6567 3f72  clientele.jpeg?r
+000000c0: 6177 3d74 7275 6522 3e0a 3c2f 703e 0a0a  aw=true">.</p>..
+000000d0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000000e0: 223e 0a3c 6120 6872 6566 3d22 6874 7470  ">.<a href="http
+000000f0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000100: 6a65 6374 2f63 6c69 656e 7465 6c65 2220  ject/clientele" 
+00000110: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000120: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000130: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000140: 6473 2e69 6f2f 7079 7069 2f76 2f63 6c69  ds.io/pypi/v/cli
+00000150: 656e 7465 6c65 3f63 6f6c 6f72 3d25 3233  entele?color=%23
+00000160: 3334 4430 3538 266c 6162 656c 3d70 7970  34D058&label=pyp
+00000170: 6925 3230 7061 636b 6167 6522 2061 6c74  i%20package" alt
+00000180: 3d22 5061 636b 6167 6520 7665 7273 696f  ="Package versio
+00000190: 6e22 3e0a 3c2f 613e 0a3c 6120 6872 6566  n">.</a>.<a href
+000001a0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+000001b0: 7267 2f70 726f 6a65 6374 2f63 6c69 656e  rg/project/clien
+000001c0: 7465 6c65 2220 7461 7267 6574 3d22 5f62  tele" target="_b
+000001d0: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
+000001e0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000001f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000200: 2f70 7976 6572 7369 6f6e 732f 636c 6965  /pyversions/clie
+00000210: 6e74 656c 652e 7376 673f 636f 6c6f 723d  ntele.svg?color=
+00000220: 2532 3333 3444 3035 3822 2061 6c74 3d22  %2334D058" alt="
+00000230: 5375 7070 6f72 7465 6420 5079 7468 6f6e  Supported Python
+00000240: 2076 6572 7369 6f6e 7322 3e0a 3c2f 613e   versions">.</a>
+00000250: 0a3c 2f70 3e0a 0a43 6c69 656e 7465 6c65  .</p>..Clientele
+00000260: 206c 6574 7320 796f 7520 6765 6e65 7261   lets you genera
+00000270: 7465 2066 756c 6c79 2d74 7970 6564 2c20  te fully-typed, 
+00000280: 6675 6e63 7469 6f6e 616c 2c20 4150 4920  functional, API 
+00000290: 436c 6965 6e74 7320 6672 6f6d 204f 7065  Clients from Ope
+000002a0: 6e41 5049 2073 6368 656d 6173 2e0a 0a49  nAPI schemas...I
+000002b0: 7420 7573 6573 206d 6f64 6572 6e20 746f  t uses modern to
+000002c0: 6f6c 7320 746f 2062 6520 626c 617a 696e  ols to be blazin
+000002d0: 6720 6661 7374 2061 6e64 2074 7970 6520  g fast and type 
+000002e0: 7361 6665 2e0a 0a50 6c75 7320 2d20 7468  safe...Plus - th
+000002f0: 6572 6520 6973 206e 6f20 636f 6d70 6c65  ere is no comple
+00000300: 7820 626f 696c 6572 706c 6174 6520 616e  x boilerplate an
+00000310: 6420 7468 6520 6765 6e65 7261 7465 6420  d the generated 
+00000320: 636f 6465 2069 7320 7665 7279 2073 6d61  code is very sma
+00000330: 6c6c 2e0a 0a23 2320 4665 6174 7572 6573  ll...## Features
+00000340: 0a0a 2a20 4675 6c6c 7920 7479 7065 6420  ..* Fully typed 
+00000350: 4150 4920 436c 6965 6e74 2075 7369 6e67  API Client using
+00000360: 2050 7964 616e 7469 632e 0a2a 204d 696e   Pydantic..* Min
+00000370: 696d 616c 6973 7420 616e 6420 6561 7379  imalist and easy
+00000380: 2074 6f20 7573 6520 2d20 7468 6520 6765   to use - the ge
+00000390: 6e65 7261 7465 6420 636f 6465 2069 7320  nerated code is 
+000003a0: 6465 7369 676e 6564 2066 6f72 2072 6561  designed for rea
+000003b0: 6461 6269 6c69 7479 2e0a 2a20 4368 6f6f  dability..* Choo
+000003c0: 7365 2065 6974 6865 7220 7379 6e63 206f  se either sync o
+000003d0: 7220 6173 796e 6320 2d20 7765 2073 7570  r async - we sup
+000003e0: 706f 7274 2062 6f74 682c 2061 6e64 2079  port both, and y
+000003f0: 6f75 2063 616e 2073 7769 7463 6820 6265  ou can switch be
+00000400: 7477 6565 6e20 7468 656d 2065 6173 696c  tween them easil
+00000410: 792e 0a2a 2053 7570 706f 7274 7320 6175  y..* Supports au
+00000420: 7468 656e 7469 6361 7469 6f6e 2028 6375  thentication (cu
+00000430: 7265 6e74 6c79 206f 6e6c 7920 4854 5450  rently only HTTP
+00000440: 2042 6561 7265 7220 616e 6420 4854 5450   Bearer and HTTP
+00000450: 2042 6173 6963 2061 7574 6829 2e0a 2a20   Basic auth)..* 
+00000460: 5772 6974 7465 6e20 656e 7469 7265 6c79  Written entirely
+00000470: 2069 6e20 5079 7468 6f6e 202d 206e 6f20   in Python - no 
+00000480: 6e65 6564 2074 6f20 696e 7374 616c 6c20  need to install 
+00000490: 6f74 6865 7220 6c61 6e67 7561 6765 7320  other languages 
+000004a0: 746f 2075 7365 204f 7065 6e41 5049 2e0a  to use OpenAPI..
+000004b0: 2a20 5468 6520 636c 6965 6e74 2066 6f6f  * The client foo
+000004c0: 7470 7269 6e74 2069 7320 6d69 6e69 6d61  tprint is minima
+000004d0: 6c20 2d20 6974 206f 6e6c 7920 7265 7175  l - it only requ
+000004e0: 6972 6573 2060 6874 7470 7860 2061 6e64  ires `httpx` and
+000004f0: 2060 7079 6461 6e74 6963 602e 0a2a 2053   `pydantic`..* S
+00000500: 7570 706f 7274 7320 796f 7572 206f 776e  upports your own
+00000510: 2063 6f6e 6669 6775 7261 7469 6f6e 202d   configuration -
+00000520: 2077 6520 7072 6f76 6964 6520 616e 2065   we provide an e
+00000530: 6e74 7279 2070 6f69 6e74 2074 6861 7420  ntry point that 
+00000540: 7769 6c6c 206e 6576 6572 2062 6520 6f76  will never be ov
+00000550: 6572 7772 6974 7465 6e2e 0a0a 5765 2772  erwritten...We'r
+00000560: 6520 6275 696c 7420 6f6e 3a0a 0a2a 205b  e built on:..* [
+00000570: 5079 6461 6e74 6963 2032 2e30 5d28 6874  Pydantic 2.0](ht
+00000580: 7470 733a 2f2f 646f 6373 2e70 7964 616e  tps://docs.pydan
+00000590: 7469 632e 6465 762f 6c61 7465 7374 2f29  tic.dev/latest/)
+000005a0: 0a2a 205b 6874 7470 785d 2868 7474 7073  .* [httpx](https
+000005b0: 3a2f 2f77 7777 2e70 7974 686f 6e2d 6874  ://www.python-ht
+000005c0: 7470 782e 6f72 672f 290a 2a20 5b6f 7065  tpx.org/).* [ope
+000005d0: 6e61 7069 2d63 6f72 655d 2868 7474 7073  napi-core](https
+000005e0: 3a2f 2f6f 7065 6e61 7069 2d63 6f72 652e  ://openapi-core.
+000005f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000600: 6e2f 6c61 7465 7374 2f29 0a0a 2323 2049  n/latest/)..## I
+00000610: 6e73 7461 6c6c 0a0a 6060 6073 680a 706f  nstall..```sh.po
+00000620: 6574 7279 2061 6464 2063 6c69 656e 7465  etry add cliente
+00000630: 6c65 0a60 6060 0a0a 2323 2055 7361 6765  le.```..## Usage
+00000640: 0a0a 6060 6073 680a 636c 6965 6e74 656c  ..```sh.clientel
+00000650: 6520 6765 6e65 7261 7465 202d 6620 7061  e generate -f pa
+00000660: 7468 2f74 6f2f 6669 6c65 2e6a 736f 6e20  th/to/file.json 
+00000670: 2d6f 206d 795f 636c 6965 6e74 2f20 2d2d  -o my_client/ --
+00000680: 6173 796e 6369 6f20 740a 6060 600a 0a5b  asyncio t.```..[
+00000690: 5265 6164 2074 6865 2064 6f63 735d 2868  Read the docs](h
+000006a0: 7474 7073 3a2f 2f62 6563 6b65 7474 2d73  ttps://beckett-s
+000006b0: 6f66 7477 6172 652e 6769 7468 7562 2e69  oftware.github.i
+000006c0: 6f2f 636c 6965 6e74 656c 652f 290a       o/clientele/).
```

### Comparing `clientele-0.3.1/pyproject.toml` & `clientele-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clientele"
-version = "0.3.1"
+version = "0.3.2"
 description = "Typed API Clients from OpenAPI schemas"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
 homepage = "https://beckett-software.github.io/clientele/"
```

### Comparing `clientele-0.3.1/src/cli.py` & `clientele-0.3.2/src/cli.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/src/constants_template.py` & `clientele-0.3.2/src/constants_template.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/src/generator.py` & `clientele-0.3.2/src/generator.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/src/generators/clients.py` & `clientele-0.3.2/src/generators/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,23 +157,25 @@
 
     def generate_post_content(self, operation: Dict, path: str) -> None:
         response_types = self.generate_response_types(operation["responses"])
         func_name = get_func_name(operation, path)
         if not operation.get("requestBody"):
             input_class_name = "None"
         else:
-            input_class_name = self.generate_input_types(operation.get("requestBody", {}))
+            input_class_name = self.generate_input_types(
+                operation.get("requestBody", {})
+            )
         function_arguments = self.generate_function_args(
             operation.get("parameters", [])
         )
         FUNCTION_ARGS = f"""
 {function_arguments['return_string']}{function_arguments['return_string'] and ", "}data: {input_class_name}"""
         CONTENT = f"""
 {self.asyncio and "async " or ""}def {func_name}({FUNCTION_ARGS}) -> {response_types}:
-    response = {self.asyncio and "await " or ""}http.post(f"{path}", data=data and data.model_dump())
+    response = {self.asyncio and "await " or ""}http.post(f"{path}", data=data.model_dump())
     return http.handle_response({func_name}, response)
     """
         self.results["post_methods"] += 1
         write_to_client(content=CONTENT, output_dir=self.output_dir)
 
     def write_path_to_client(self, path: Dict) -> None:
         url, operations = path
```

### Comparing `clientele-0.3.1/src/generators/http.py` & `clientele-0.3.2/src/generators/http.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/src/generators/schemas.py` & `clientele-0.3.2/src/generators/schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 from openapi_core import Spec
 from rich.console import Console
 
 from src.utils import class_name_titled, clean_prop, get_type
 from src.writer import write_to_schemas
 
@@ -33,23 +33,25 @@
         for arg, arg_details in properties.items():
             content = (
                 content
                 + f"""    {clean_prop(arg.upper())} = {get_type(arg_details)}\n"""
             )
         return content
 
-    def generate_class_properties(self, properties: Dict) -> str:
+    def generate_class_properties(
+        self, properties: Dict, required: Optional[List] = None
+    ) -> str:
         """
         Generate a string list of the properties for this pydantic class.
         """
         content = ""
         for arg, arg_details in properties.items():
             arg_type = get_type(arg_details)
             # TODO support this
-            is_optional = False
+            is_optional = required and arg not in required
             content = (
                 content
                 + f"""    {clean_prop(arg)}: {is_optional and f"typing.Optional[{arg_type}]" or arg_type}\n"""
             )
         return content
 
     def generate_input_class(self, schema: Dict) -> None:
@@ -62,20 +64,21 @@
                     )
                 elif title := input_schema["schema"].get("title", False):
                     class_name = class_name_titled(title)
                 else:
                     # No idea, using the encoding?
                     class_name = class_name_titled(encoding)
                 properties = self.generate_class_properties(
-                    input_schema["schema"].get("properties", {})
+                    properties=input_schema["schema"].get("properties", {}),
+                    required=input_schema["schema"].get("required", None),
                 )
                 out_content = f"""
 class {class_name}(BaseModel):
 {properties if properties else "    pass"}
-    """
+"""
             write_to_schemas(
                 out_content,
                 output_dir=self.output_dir,
             )
 
     def generate_schema_classes(self) -> None:
         """
@@ -87,15 +90,16 @@
             if schema.get("enum"):
                 enum = True
                 properties = self.generate_enum_properties(
                     {v: {"type": f'"{v}"'} for v in schema["enum"]}
                 )
             else:
                 properties = self.generate_class_properties(
-                    schema.get("properties", {})
+                    properties=schema.get("properties", {}),
+                    required=schema.get("required", None),
                 )
             self.schemas[schema_key] = properties
             content = f"""
 class {schema_key}({"Enum" if enum else "BaseModel"}):
 {properties if properties else "    pass"}
     """
             write_to_schemas(
```

### Comparing `clientele-0.3.1/src/template/http.py` & `clientele-0.3.2/src/template/http.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/src/utils.py` & `clientele-0.3.2/src/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,21 +39,26 @@
     reserved_words = ["from"]
     if input_str in reserved_words:
         input_str = input_str + "_"
     return input_str
 
 
 def _split_upper(s):
-    return "_".join(re.findall(".[^A-Z]*", s))
+    res = re.findall(".[^A-Z]*", s)
+    if len(res) > 1:
+        return "_".join(res)
+    return res[0]
 
 
 def _snake_case(s):
     for badchar in ["/", "-", "."]:
         s = s.replace(badchar, "_")
     s = _split_upper(s)
+    if s[0] == "_":
+        s = s[1:]
     return s.lower()
 
 
 def get_func_name(operation: Dict, path: str) -> str:
     if operation.get("operationId"):
         return _snake_case(operation["operationId"].split("__")[0])
     return _snake_case(path)
```

### Comparing `clientele-0.3.1/src/writer.py` & `clientele-0.3.2/src/writer.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.1/PKG-INFO` & `clientele-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636c 6965  : 2.1.Name: clie
 00000020: 6e74 656c 650a 5665 7273 696f 6e3a 2030  ntele.Version: 0
-00000030: 2e33 2e31 0a53 756d 6d61 7279 3a20 5479  .3.1.Summary: Ty
+00000030: 2e33 2e32 0a53 756d 6d61 7279 3a20 5479  .3.2.Summary: Ty
 00000040: 7065 6420 4150 4920 436c 6965 6e74 7320  ped API Clients 
 00000050: 6672 6f6d 204f 7065 6e41 5049 2073 6368  from OpenAPI sch
 00000060: 656d 6173 0a48 6f6d 652d 7061 6765 3a20  emas.Home-page: 
 00000070: 6874 7470 733a 2f2f 6265 636b 6574 742d  https://beckett-
 00000080: 736f 6674 7761 7265 2e67 6974 6875 622e  software.github.
 00000090: 696f 2f63 6c69 656e 7465 6c65 2f0a 4c69  io/clientele/.Li
 000000a0: 6365 6e73 653a 204d 4954 0a41 7574 686f  cense: MIT.Autho
@@ -46,90 +46,117 @@
 000002d0: 6973 743a 2072 6963 6820 283e 3d31 332e  ist: rich (>=13.
 000002e0: 342e 322c 3c31 342e 302e 3029 0a52 6571  4.2,<14.0.0).Req
 000002f0: 7569 7265 732d 4469 7374 3a20 7479 7065  uires-Dist: type
 00000300: 732d 7079 7961 6d6c 2028 3e3d 362e 302e  s-pyyaml (>=6.0.
 00000310: 3132 2e31 312c 3c37 2e30 2e30 2e30 290a  12.11,<7.0.0.0).
 00000320: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000330: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-00000340: 6172 6b64 6f77 6e0a 0a23 20e2 9a9c efb8  arkdown..# .....
-00000350: 8f20 436c 6965 6e74 656c 650a 0a23 2054  . Clientele..# T
-00000360: 7970 6564 2041 5049 2043 6c69 656e 7473  yped API Clients
-00000370: 2066 726f 6d20 4f70 656e 4150 4920 7363   from OpenAPI sc
-00000380: 6865 6d61 730a 0a21 5b63 6c69 656e 7465  hemas..![cliente
-00000390: 6c65 5f6c 6f67 6f5d 2868 7474 7073 3a2f  le_logo](https:/
-000003a0: 2f67 6974 6875 622e 636f 6d2f 6265 636b  /github.com/beck
-000003b0: 6574 742d 736f 6674 7761 7265 2f63 6c69  ett-software/cli
-000003c0: 656e 7465 6c65 2f62 6c6f 622f 6d61 696e  entele/blob/main
-000003d0: 2f64 6f63 732f 636c 6965 6e74 656c 652e  /docs/clientele.
-000003e0: 6a70 6567 3f72 6177 3d74 7275 6529 0a0a  jpeg?raw=true)..
-000003f0: 436c 6965 6e74 656c 6520 6c65 7473 2079  Clientele lets y
-00000400: 6f75 2067 656e 6572 6174 6520 6675 6c6c  ou generate full
-00000410: 792d 7479 7065 642c 2066 756e 6374 696f  y-typed, functio
-00000420: 6e61 6c2c 2041 5049 2043 6c69 656e 7473  nal, API Clients
-00000430: 2066 726f 6d20 4f70 656e 4150 4920 7363   from OpenAPI sc
-00000440: 6865 6d61 732e 0a0a 4974 2075 7365 7320  hemas...It uses 
-00000450: 6d6f 6465 726e 2074 6f6f 6c73 2074 6f20  modern tools to 
-00000460: 6265 2062 6c61 7a69 6e67 2066 6173 7420  be blazing fast 
-00000470: 616e 6420 7479 7065 2073 6166 652e 0a0a  and type safe...
-00000480: 506c 7573 202d 2074 6865 7265 2069 7320  Plus - there is 
-00000490: 6e6f 2063 6f6d 706c 6578 2062 6f69 6c65  no complex boile
-000004a0: 7270 6c61 7465 2061 6e64 2074 6865 2067  rplate and the g
-000004b0: 656e 6572 6174 6564 2063 6f64 6520 6973  enerated code is
-000004c0: 2076 6572 7920 736d 616c 6c2e 0a0a 2323   very small...##
-000004d0: 2046 6561 7475 7265 730a 0a2a 2046 756c   Features..* Ful
-000004e0: 6c79 2074 7970 6564 2041 5049 2043 6c69  ly typed API Cli
-000004f0: 656e 7420 7573 696e 6720 5079 6461 6e74  ent using Pydant
-00000500: 6963 2e0a 2a20 4d69 6e69 6d61 6c69 7374  ic..* Minimalist
-00000510: 2061 6e64 2065 6173 7920 746f 2075 7365   and easy to use
-00000520: 202d 2074 6865 2067 656e 6572 6174 6564   - the generated
-00000530: 2063 6f64 6520 6973 2064 6573 6967 6e65   code is designe
-00000540: 6420 666f 7220 7265 6164 6162 696c 6974  d for readabilit
-00000550: 792e 0a2a 2043 686f 6f73 6520 6569 7468  y..* Choose eith
-00000560: 6572 2073 796e 6320 6f72 2061 7379 6e63  er sync or async
-00000570: 202d 2077 6520 7375 7070 6f72 7420 626f   - we support bo
-00000580: 7468 2c20 616e 6420 796f 7520 6361 6e20  th, and you can 
-00000590: 7377 6974 6368 2062 6574 7765 656e 2074  switch between t
-000005a0: 6865 6d20 6561 7369 6c79 2e0a 2a20 5375  hem easily..* Su
-000005b0: 7070 6f72 7473 2061 7574 6865 6e74 6963  pports authentic
-000005c0: 6174 696f 6e20 2863 7572 656e 746c 7920  ation (curently 
-000005d0: 6f6e 6c79 2048 5454 5020 4265 6172 6572  only HTTP Bearer
-000005e0: 2061 6e64 2048 5454 5020 4261 7369 6320   and HTTP Basic 
-000005f0: 6175 7468 292e 0a2a 2057 7269 7474 656e  auth)..* Written
-00000600: 2065 6e74 6972 656c 7920 696e 2050 7974   entirely in Pyt
-00000610: 686f 6e20 2d20 6e6f 206e 6565 6420 746f  hon - no need to
-00000620: 2069 6e73 7461 6c6c 206f 7468 6572 206c   install other l
-00000630: 616e 6775 6167 6573 2074 6f20 7573 6520  anguages to use 
-00000640: 4f70 656e 4150 492e 0a2a 2054 6865 2063  OpenAPI..* The c
-00000650: 6c69 656e 7420 666f 6f74 7072 696e 7420  lient footprint 
-00000660: 6973 206d 696e 696d 616c 202d 2069 7420  is minimal - it 
-00000670: 6f6e 6c79 2072 6571 7569 7265 7320 6068  only requires `h
-00000680: 7474 7078 6020 616e 6420 6070 7964 616e  ttpx` and `pydan
-00000690: 7469 6360 2e0a 2a20 5375 7070 6f72 7473  tic`..* Supports
-000006a0: 2079 6f75 7220 6f77 6e20 636f 6e66 6967   your own config
-000006b0: 7572 6174 696f 6e20 2d20 7765 2070 726f  uration - we pro
-000006c0: 7669 6465 2061 6e20 656e 7472 7920 706f  vide an entry po
-000006d0: 696e 7420 7468 6174 2077 696c 6c20 6e65  int that will ne
-000006e0: 7665 7220 6265 206f 7665 7277 7269 7474  ver be overwritt
-000006f0: 656e 2e0a 0a57 6527 7265 2062 7569 6c74  en...We're built
-00000700: 206f 6e3a 0a0a 2a20 5b50 7964 616e 7469   on:..* [Pydanti
-00000710: 6320 322e 305d 2868 7474 7073 3a2f 2f64  c 2.0](https://d
-00000720: 6f63 732e 7079 6461 6e74 6963 2e64 6576  ocs.pydantic.dev
-00000730: 2f6c 6174 6573 742f 290a 2a20 5b68 7474  /latest/).* [htt
-00000740: 7078 5d28 6874 7470 733a 2f2f 7777 772e  px](https://www.
-00000750: 7079 7468 6f6e 2d68 7474 7078 2e6f 7267  python-httpx.org
-00000760: 2f29 0a2a 205b 6f70 656e 6170 692d 636f  /).* [openapi-co
-00000770: 7265 5d28 6874 7470 733a 2f2f 6f70 656e  re](https://open
-00000780: 6170 692d 636f 7265 2e72 6561 6474 6865  api-core.readthe
-00000790: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-000007a0: 742f 290a 0a23 2320 496e 7374 616c 6c0a  t/)..## Install.
-000007b0: 0a60 6060 7368 0a70 6f65 7472 7920 6164  .```sh.poetry ad
-000007c0: 6420 636c 6965 6e74 656c 650a 6060 600a  d clientele.```.
-000007d0: 0a23 2320 5573 6167 650a 0a60 6060 7368  .## Usage..```sh
-000007e0: 0a63 6c69 656e 7465 6c65 2067 656e 6572  .clientele gener
-000007f0: 6174 6520 2d66 2070 6174 682f 746f 2f66  ate -f path/to/f
-00000800: 696c 652e 6a73 6f6e 202d 6f20 6d79 5f63  ile.json -o my_c
-00000810: 6c69 656e 742f 202d 2d61 7379 6e63 696f  lient/ --asyncio
-00000820: 2074 0a60 6060 0a0a 5b52 6561 6420 7468   t.```..[Read th
-00000830: 6520 646f 6373 5d28 6874 7470 733a 2f2f  e docs](https://
-00000840: 6265 636b 6574 742d 736f 6674 7761 7265  beckett-software
-00000850: 2e67 6974 6875 622e 696f 2f63 6c69 656e  .github.io/clien
-00000860: 7465 6c65 2f29 0a0a                      tele/)..
+00000340: 6172 6b64 6f77 6e0a 0a3c 7020 616c 6967  arkdown..<p alig
+00000350: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000360: 3c68 313e e29a 9cef b88f 2043 6c69 656e  <h1>...... Clien
+00000370: 7465 6c65 3c2f 6831 3e0a 2020 2020 3c65  tele</h1>.    <e
+00000380: 6d3e 5479 7065 6420 4150 4920 436c 6965  m>Typed API Clie
+00000390: 6e74 7320 6672 6f6d 204f 7065 6e41 5049  nts from OpenAPI
+000003a0: 2073 6368 656d 6173 3c2f 656d 3e0a 2020   schemas</em>.  
+000003b0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000003c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+000003d0: 6563 6b65 7474 2d73 6f66 7477 6172 652f  eckett-software/
+000003e0: 636c 6965 6e74 656c 652f 626c 6f62 2f6d  clientele/blob/m
+000003f0: 6169 6e2f 646f 6373 2f63 6c69 656e 7465  ain/docs/cliente
+00000400: 6c65 2e6a 7065 673f 7261 773d 7472 7565  le.jpeg?raw=true
+00000410: 223e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  ">.</p>..<p alig
+00000420: 6e3d 2263 656e 7465 7222 3e0a 3c61 2068  n="center">.<a h
+00000430: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000440: 692e 6f72 672f 7072 6f6a 6563 742f 636c  i.org/project/cl
+00000450: 6965 6e74 656c 6522 2074 6172 6765 743d  ientele" target=
+00000460: 225f 626c 616e 6b22 3e0a 2020 2020 3c69  "_blank">.    <i
+00000470: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000480: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000490: 7970 692f 762f 636c 6965 6e74 656c 653f  ypi/v/clientele?
+000004a0: 636f 6c6f 723d 2532 3333 3444 3035 3826  color=%2334D058&
+000004b0: 6c61 6265 6c3d 7079 7069 2532 3070 6163  label=pypi%20pac
+000004c0: 6b61 6765 2220 616c 743d 2250 6163 6b61  kage" alt="Packa
+000004d0: 6765 2076 6572 7369 6f6e 223e 0a3c 2f61  ge version">.</a
+000004e0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+000004f0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000500: 6563 742f 636c 6965 6e74 656c 6522 2074  ect/clientele" t
+00000510: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
+00000520: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000530: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000540: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000550: 696f 6e73 2f63 6c69 656e 7465 6c65 2e73  ions/clientele.s
+00000560: 7667 3f63 6f6c 6f72 3d25 3233 3334 4430  vg?color=%2334D0
+00000570: 3538 2220 616c 743d 2253 7570 706f 7274  58" alt="Support
+00000580: 6564 2050 7974 686f 6e20 7665 7273 696f  ed Python versio
+00000590: 6e73 223e 0a3c 2f61 3e0a 3c2f 703e 0a0a  ns">.</a>.</p>..
+000005a0: 436c 6965 6e74 656c 6520 6c65 7473 2079  Clientele lets y
+000005b0: 6f75 2067 656e 6572 6174 6520 6675 6c6c  ou generate full
+000005c0: 792d 7479 7065 642c 2066 756e 6374 696f  y-typed, functio
+000005d0: 6e61 6c2c 2041 5049 2043 6c69 656e 7473  nal, API Clients
+000005e0: 2066 726f 6d20 4f70 656e 4150 4920 7363   from OpenAPI sc
+000005f0: 6865 6d61 732e 0a0a 4974 2075 7365 7320  hemas...It uses 
+00000600: 6d6f 6465 726e 2074 6f6f 6c73 2074 6f20  modern tools to 
+00000610: 6265 2062 6c61 7a69 6e67 2066 6173 7420  be blazing fast 
+00000620: 616e 6420 7479 7065 2073 6166 652e 0a0a  and type safe...
+00000630: 506c 7573 202d 2074 6865 7265 2069 7320  Plus - there is 
+00000640: 6e6f 2063 6f6d 706c 6578 2062 6f69 6c65  no complex boile
+00000650: 7270 6c61 7465 2061 6e64 2074 6865 2067  rplate and the g
+00000660: 656e 6572 6174 6564 2063 6f64 6520 6973  enerated code is
+00000670: 2076 6572 7920 736d 616c 6c2e 0a0a 2323   very small...##
+00000680: 2046 6561 7475 7265 730a 0a2a 2046 756c   Features..* Ful
+00000690: 6c79 2074 7970 6564 2041 5049 2043 6c69  ly typed API Cli
+000006a0: 656e 7420 7573 696e 6720 5079 6461 6e74  ent using Pydant
+000006b0: 6963 2e0a 2a20 4d69 6e69 6d61 6c69 7374  ic..* Minimalist
+000006c0: 2061 6e64 2065 6173 7920 746f 2075 7365   and easy to use
+000006d0: 202d 2074 6865 2067 656e 6572 6174 6564   - the generated
+000006e0: 2063 6f64 6520 6973 2064 6573 6967 6e65   code is designe
+000006f0: 6420 666f 7220 7265 6164 6162 696c 6974  d for readabilit
+00000700: 792e 0a2a 2043 686f 6f73 6520 6569 7468  y..* Choose eith
+00000710: 6572 2073 796e 6320 6f72 2061 7379 6e63  er sync or async
+00000720: 202d 2077 6520 7375 7070 6f72 7420 626f   - we support bo
+00000730: 7468 2c20 616e 6420 796f 7520 6361 6e20  th, and you can 
+00000740: 7377 6974 6368 2062 6574 7765 656e 2074  switch between t
+00000750: 6865 6d20 6561 7369 6c79 2e0a 2a20 5375  hem easily..* Su
+00000760: 7070 6f72 7473 2061 7574 6865 6e74 6963  pports authentic
+00000770: 6174 696f 6e20 2863 7572 656e 746c 7920  ation (curently 
+00000780: 6f6e 6c79 2048 5454 5020 4265 6172 6572  only HTTP Bearer
+00000790: 2061 6e64 2048 5454 5020 4261 7369 6320   and HTTP Basic 
+000007a0: 6175 7468 292e 0a2a 2057 7269 7474 656e  auth)..* Written
+000007b0: 2065 6e74 6972 656c 7920 696e 2050 7974   entirely in Pyt
+000007c0: 686f 6e20 2d20 6e6f 206e 6565 6420 746f  hon - no need to
+000007d0: 2069 6e73 7461 6c6c 206f 7468 6572 206c   install other l
+000007e0: 616e 6775 6167 6573 2074 6f20 7573 6520  anguages to use 
+000007f0: 4f70 656e 4150 492e 0a2a 2054 6865 2063  OpenAPI..* The c
+00000800: 6c69 656e 7420 666f 6f74 7072 696e 7420  lient footprint 
+00000810: 6973 206d 696e 696d 616c 202d 2069 7420  is minimal - it 
+00000820: 6f6e 6c79 2072 6571 7569 7265 7320 6068  only requires `h
+00000830: 7474 7078 6020 616e 6420 6070 7964 616e  ttpx` and `pydan
+00000840: 7469 6360 2e0a 2a20 5375 7070 6f72 7473  tic`..* Supports
+00000850: 2079 6f75 7220 6f77 6e20 636f 6e66 6967   your own config
+00000860: 7572 6174 696f 6e20 2d20 7765 2070 726f  uration - we pro
+00000870: 7669 6465 2061 6e20 656e 7472 7920 706f  vide an entry po
+00000880: 696e 7420 7468 6174 2077 696c 6c20 6e65  int that will ne
+00000890: 7665 7220 6265 206f 7665 7277 7269 7474  ver be overwritt
+000008a0: 656e 2e0a 0a57 6527 7265 2062 7569 6c74  en...We're built
+000008b0: 206f 6e3a 0a0a 2a20 5b50 7964 616e 7469   on:..* [Pydanti
+000008c0: 6320 322e 305d 2868 7474 7073 3a2f 2f64  c 2.0](https://d
+000008d0: 6f63 732e 7079 6461 6e74 6963 2e64 6576  ocs.pydantic.dev
+000008e0: 2f6c 6174 6573 742f 290a 2a20 5b68 7474  /latest/).* [htt
+000008f0: 7078 5d28 6874 7470 733a 2f2f 7777 772e  px](https://www.
+00000900: 7079 7468 6f6e 2d68 7474 7078 2e6f 7267  python-httpx.org
+00000910: 2f29 0a2a 205b 6f70 656e 6170 692d 636f  /).* [openapi-co
+00000920: 7265 5d28 6874 7470 733a 2f2f 6f70 656e  re](https://open
+00000930: 6170 692d 636f 7265 2e72 6561 6474 6865  api-core.readthe
+00000940: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000950: 742f 290a 0a23 2320 496e 7374 616c 6c0a  t/)..## Install.
+00000960: 0a60 6060 7368 0a70 6f65 7472 7920 6164  .```sh.poetry ad
+00000970: 6420 636c 6965 6e74 656c 650a 6060 600a  d clientele.```.
+00000980: 0a23 2320 5573 6167 650a 0a60 6060 7368  .## Usage..```sh
+00000990: 0a63 6c69 656e 7465 6c65 2067 656e 6572  .clientele gener
+000009a0: 6174 6520 2d66 2070 6174 682f 746f 2f66  ate -f path/to/f
+000009b0: 696c 652e 6a73 6f6e 202d 6f20 6d79 5f63  ile.json -o my_c
+000009c0: 6c69 656e 742f 202d 2d61 7379 6e63 696f  lient/ --asyncio
+000009d0: 2074 0a60 6060 0a0a 5b52 6561 6420 7468   t.```..[Read th
+000009e0: 6520 646f 6373 5d28 6874 7470 733a 2f2f  e docs](https://
+000009f0: 6265 636b 6574 742d 736f 6674 7761 7265  beckett-software
+00000a00: 2e67 6974 6875 622e 696f 2f63 6c69 656e  .github.io/clien
+00000a10: 7465 6c65 2f29 0a0a                      tele/)..
```

