# Comparing `tmp/dfv-0.5.0.tar.gz` & `tmp/dfv-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfv-0.5.0.tar", max compression
+gzip compressed data, was "dfv-0.5.1.tar", max compression
```

## Comparing `dfv-0.5.0.tar` & `dfv-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    15042 2023-07-29 07:35:17.124824 dfv-0.5.0/dfv/__init__.py
--rw-r--r--   0        0        0    25324 2023-07-29 07:35:17.436828 dfv-0.5.0/dfv/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9764 2023-07-29 07:28:59.868353 dfv-0.5.0/dfv/__pycache__/test_element.cpython-311.pyc
--rw-r--r--   0        0        0     8642 2023-07-29 07:35:17.724831 dfv-0.5.0/dfv/__pycache__/test_form.cpython-311.pyc
--rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.5.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
--rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.5.0/dfv/static/dfv.js
--rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.5.0/dfv/templates/dfv/tests/TemplateResponse.html
--rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.5.0/dfv/templatetags/__init__.py
--rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.5.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.5.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
--rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.5.0/dfv/templatetags/dfv.py
--rw-r--r--   0        0        0     4027 2023-07-29 07:28:59.236346 dfv-0.5.0/dfv/test_element.py
--rw-r--r--   0        0        0     3338 2023-07-29 07:35:17.132824 dfv-0.5.0/dfv/test_form.py
--rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.5.0/dfv/test_params_to_args.py
--rw-r--r--   0        0        0     1421 2023-07-29 06:51:06.289661 dfv-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.5.0/setup.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    15349 2023-07-31 19:10:30.998195 dfv-0.5.1/dfv/__init__.py
+-rw-r--r--   0        0        0    25559 2023-07-31 19:10:42.642339 dfv-0.5.1/dfv/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10516 2023-07-31 19:12:13.755376 dfv-0.5.1/dfv/__pycache__/test_element.cpython-311.pyc
+-rw-r--r--   0        0        0     8642 2023-07-29 08:01:02.515193 dfv-0.5.1/dfv/__pycache__/test_form.cpython-311.pyc
+-rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.5.1/dfv/__pycache__/test_params_to_args.cpython-311.pyc
+-rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.5.1/dfv/static/dfv.js
+-rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.5.1/dfv/templates/dfv/tests/TemplateResponse.html
+-rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.5.1/dfv/templatetags/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.5.1/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.5.1/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
+-rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.5.1/dfv/templatetags/dfv.py
+-rw-r--r--   0        0        0     4360 2023-07-31 19:11:53.483153 dfv-0.5.1/dfv/test_element.py
+-rw-r--r--   0        0        0     3340 2023-07-29 08:01:00.971175 dfv-0.5.1/dfv/test_form.py
+-rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.5.1/dfv/test_params_to_args.py
+-rw-r--r--   0        0        0     1438 2023-07-31 19:08:19.608679 dfv-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.5.1/setup.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.5.1/PKG-INFO
```

### Comparing `dfv-0.5.0/dfv/__init__.py` & `dfv-0.5.1/dfv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,27 @@
     def __init__(
         self,
         response: HttpResponse,
         element_id: Optional[str],
         tag="div",
         hx_target="this",
         hx_swap="outerHTML",
+        classes: Optional[str] = None,
         no_element_wrap=False,
     ):
         if not no_element_wrap:
             attr_id = f"id='{element_id}'" if element_id is not None else ""
             attr_hx_target = f"hx-target='{hx_target}'" if hx_target else ""
             attr_hx_swap = f"hx-swap='{hx_swap}'" if hx_swap else ""
-            new_content = f"<{tag} {attr_id} {attr_hx_target} {attr_hx_swap}>{response_to_str(response)}</{tag}>"
+            attr_classes = f"class='{classes}'" if classes else ""
+            new_content = (
+                f"""<{tag} {attr_id} {attr_hx_target} {attr_hx_swap} {attr_classes}>"""
+                f"""{response_to_str(response)}"""
+                f"""</{tag}>"""
+            )
             response.content = bytes(new_content, "UTF-8")
 
         super().__init__(response)
 
     def __str__(self):
         return response_to_str(self)
 
@@ -62,38 +68,43 @@
 # noinspection PyShadowingNames
 def element(
     element_id: Optional[str] = None,
     *,
     tag="div",
     hx_target="this",
     hx_swap="outerHTML",
+    classes: Optional[str] = None,
     handle_args=True,
     login_required=False,
 ) -> Callable[[Callable[P, R]], Callable[P, R]]:
     def decorator(f: Callable[P, HttpResponse]) -> Callable[P, HttpResponse]:
         id = element_id if isinstance(element_id, str) else f.__name__
 
         if handle_args:
-            f = _handle_args()(f)
+            f = _inject_args()(f)
 
         if login_required:
             f = auth_decorators.login_required()(f)
 
         @functools.wraps(f)
         def inner(*args: P.args, **kwargs: P.kwargs) -> HttpResponse:
             response = f(*args, **kwargs)
-            response.streaming
             if not response["Content-Type"].startswith("text/html"):
                 return response
 
             if isinstance(response, ElementResponse):
                 return response
 
             return ElementResponse(
-                response, element_id=id, tag=tag, hx_target=hx_target, hx_swap=hx_swap
+                response,
+                element_id=id,
+                tag=tag,
+                hx_target=hx_target,
+                hx_swap=hx_swap,
+                classes=classes,
             )
 
         return inner
 
     return decorator
 
 
@@ -146,15 +157,15 @@
 
         return inner
 
     return decorator
 
 
 # alias, to allow parameters to be named handle_args
-_handle_args = inject_args
+_inject_args = inject_args
 
 
 @dataclasses.dataclass
 class InjectedParam:
     name: str = dataclasses.field(init=False)
     target_type: type = dataclasses.field(init=False)
```

### Comparing `dfv-0.5.0/dfv/__pycache__/__init__.cpython-311.pyc` & `dfv-0.5.1/dfv/__pycache__/__init__.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,56 +1,57 @@
 magic:    0xa70d0d0a
-moddate:  0x35c1c464 (Sat Jul 29 07:35:17 2023 UTC)
-files sz: 15042
+moddate:  0x2607c864 (Mon Jul 31 19:10:30 2023 UTC)
+files sz: 15349
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 11
+   stacksize : 12
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       016c035a03640064016c045a04640064016c055a05640064026c066d075a
       070100640064036c046d085a086d095a096d0a5a0a6d0b5a0b6d0c5a0c6d
       0d5a0d0100640064016c0e5a0f640064016c105a10640064046c116d125a
       120100640064056c136d145a150100640064066c166d175a176d185a186d
       195a196d1a5a1a0100640064076c1b6d1c5a1c0100640064086c1d6d1e5a
       1e6d1f5a1f01000200650c6409a6010000ab0100000000000000005a2002
       00650d640aa6010000ab0100000000000000005a210200650d640ba60100
       00ab0100000000000000005a2202004700640c8400640d65106a23000000
       0000000000a6030000ab0300000000000000005a24640e6518651c7a0700
-      00640f651f6604641084045a25090064456411641264136414641564169c
-      056417650b652619000000000000000000640f6509650965206521660219
-      000000000000000000670165096520652166021900000000000000000066
-      02190000000000000000006604641884075a2709006446640e6518641965
-      18640f65186606641a84055a2864156414641b9c02641c6529650a641d19
-      0000000000000000007a070000641e650b652965267a0700001900000000
+      00640f651f6604641084045a250900644664116412641364016414641564
+      169c066417650b6526190000000000000000006418650b65261900000000
       0000000000640f6509650965206521660219000000000000000000670165
       096520652166021900000000000000000066021900000000000000000066
-      06641f84065a2a652a5a2b65006a2c000000000000000002004700642084
-      006421a6020000ab020000000000000000a6000000ab0000000000000000
-      005a2d6422652d64236526642465026a2e00000000000000006606642584
-      045a2f090064476426653065026a2e000000000000000019000000000000
-      000000641c6529650a6427190000000000000000007a070000650a642819
-      0000000000000000007a070000641e650b652965267a0700001900000000
-      0000000000640f65316526652d6602190000000000000000006608642984
-      055a32642a6530650819000000000000000000640f65176604642b84045a
-      3365006a2c000000000000000002004700642c8400642d652da6030000ab
-      030000000000000000a6000000ab0000000000000000005a3465006a2c00
-      0000000000000002004700642e8400642f6534a6030000ab030000000000
-      000000a6000000ab0000000000000000005a3565006a2c00000000000000
-      00020047006430840064316534a6030000ab030000000000000000a60000
-      00ab0000000000000000005a366448640f65086602643284055a37644864
-      0f65086602643384055a38020065046a39000000000000000065086401a6
-      020000ab0200000000000000006414660264346522640f65226604643584
-      055a3a6436653065046a0800000000000000001900000000000000000064
-      37653b6604643884045a3c0200470064398400643a652da6030000ab0300
-      000000000000005a3d640f65086602643b84045a3e643c6531640f651a66
-      04643d84045a3f643e65176602643f84045a40643e65176602644084045a
-      41643e65176602644184045a42643e65176602644284045a43643e651766
-      02644384045a44643e65176602644484045a4564015300
+      06641984075a2709006447640e6518641a6518640f65186606641b84055a
+      2864156414641c9c02641d6529650a641e190000000000000000007a0700
+      00641f650b652965267a07000019000000000000000000640f6509650965
+      206521660219000000000000000000670165096520652166021900000000
+      00000000006602190000000000000000006606642084065a2a652a5a2b65
+      006a2c000000000000000002004700642184006422a6020000ab02000000
+      0000000000a6000000ab0000000000000000005a2d6423652d6424652664
+      2565026a2e00000000000000006606642684045a2f090064486427653065
+      026a2e000000000000000019000000000000000000641d6529650a642819
+      0000000000000000007a070000650a6429190000000000000000007a0700
+      00641f650b652965267a07000019000000000000000000640f6531652665
+      2d6602190000000000000000006608642a84055a32642b65306508190000
+      00000000000000640f65176604642c84045a3365006a2c00000000000000
+      0002004700642d8400642e652da6030000ab030000000000000000a60000
+      00ab0000000000000000005a3465006a2c00000000000000000200470064
+      2f840064306534a6030000ab030000000000000000a6000000ab00000000
+      00000000005a3565006a2c00000000000000000200470064318400643265
+      34a6030000ab030000000000000000a6000000ab0000000000000000005a
+      366449640f65086602643384055a376449640f65086602643484055a3802
+      0065046a39000000000000000065086401a6020000ab0200000000000000
+      006414660264356522640f65226604643684055a3a6437653065046a0800
+      00000000000000190000000000000000006438653b6604643984045a3c02
+      004700643a8400643b652da6030000ab0300000000000000005a3d640f65
+      086602643c84045a3e643d6531640f651a6604643e84045a3f643f651766
+      02644084045a40643f65176602644184045a41643f65176602644284045a
+      42643f65176602644384045a43643f65176602644484045a44643f651766
+      02644584045a4564015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (dataclasses)
                  8 STORE_NAME               0 (dataclasses)
    
@@ -184,384 +185,392 @@
                260 LOAD_CONST              13 ('ElementResponse')
                262 LOAD_NAME               16 (wrapt)
                264 LOAD_ATTR               35 (ObjectProxy)
                274 PRECALL                  3
                278 CALL                     3
                288 STORE_NAME              36 (ElementResponse)
    
-    55         290 LOAD_CONST              14 ('response')
+    61         290 LOAD_CONST              14 ('response')
                292 LOAD_NAME               24 (HttpResponse)
                294 LOAD_NAME               28 (TemplateResponse)
                296 BINARY_OP                7 (|)
                300 LOAD_CONST              15 ('return')
                302 LOAD_NAME               31 (SafeString)
                304 BUILD_TUPLE              4
-               306 LOAD_CONST              16 (<code object response_to_str, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 55>)
+               306 LOAD_CONST              16 (<code object response_to_str, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 61>)
                308 MAKE_FUNCTION            4 (annotations)
                310 STORE_NAME              37 (response_to_str)
    
-    64         312 NOP
+    70         312 NOP
    
-    63         314 LOAD_CONST              69 ((None,))
+    69         314 LOAD_CONST              70 ((None,))
    
-    66         316 LOAD_CONST              17 ('div')
+    72         316 LOAD_CONST              17 ('div')
    
-    67         318 LOAD_CONST              18 ('this')
+    73         318 LOAD_CONST              18 ('this')
    
-    68         320 LOAD_CONST              19 ('outerHTML')
+    74         320 LOAD_CONST              19 ('outerHTML')
    
-    69         322 LOAD_CONST              20 (True)
+    75         322 LOAD_CONST               1 (None)
    
-    70         324 LOAD_CONST              21 (False)
+    76         324 LOAD_CONST              20 (True)
    
-    63         326 LOAD_CONST              22 (('tag', 'hx_target', 'hx_swap', 'handle_args', 'login_required'))
-               328 BUILD_CONST_KEY_MAP      5
-               330 LOAD_CONST              23 ('element_id')
+    77         326 LOAD_CONST              21 (False)
    
-    64         332 LOAD_NAME               11 (Optional)
-               334 LOAD_NAME               38 (str)
-               336 BINARY_SUBSCR
+    69         328 LOAD_CONST              22 (('tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required'))
+               330 BUILD_CONST_KEY_MAP      6
+               332 LOAD_CONST              23 ('element_id')
    
-    63         346 LOAD_CONST              15 ('return')
+    70         334 LOAD_NAME               11 (Optional)
+               336 LOAD_NAME               38 (str)
+               338 BINARY_SUBSCR
    
-    71         348 LOAD_NAME                9 (Callable)
-               350 LOAD_NAME                9 (Callable)
-               352 LOAD_NAME               32 (P)
-               354 LOAD_NAME               33 (R)
-               356 BUILD_TUPLE              2
-               358 BINARY_SUBSCR
-               368 BUILD_LIST               1
-               370 LOAD_NAME                9 (Callable)
-               372 LOAD_NAME               32 (P)
-               374 LOAD_NAME               33 (R)
-               376 BUILD_TUPLE              2
-               378 BINARY_SUBSCR
-               388 BUILD_TUPLE              2
-               390 BINARY_SUBSCR
+    69         348 LOAD_CONST              24 ('classes')
    
-    63         400 BUILD_TUPLE              4
-               402 LOAD_CONST              24 (<code object element, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 63>)
-               404 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
-               406 STORE_NAME              39 (element)
+    75         350 LOAD_NAME               11 (Optional)
+               352 LOAD_NAME               38 (str)
+               354 BINARY_SUBSCR
    
-   101         408 NOP
+    69         364 LOAD_CONST              15 ('return')
    
-   100         410 LOAD_CONST              70 (('outerHTML',))
-               412 LOAD_CONST              14 ('response')
+    78         366 LOAD_NAME                9 (Callable)
+               368 LOAD_NAME                9 (Callable)
+               370 LOAD_NAME               32 (P)
+               372 LOAD_NAME               33 (R)
+               374 BUILD_TUPLE              2
+               376 BINARY_SUBSCR
+               386 BUILD_LIST               1
+               388 LOAD_NAME                9 (Callable)
+               390 LOAD_NAME               32 (P)
+               392 LOAD_NAME               33 (R)
+               394 BUILD_TUPLE              2
+               396 BINARY_SUBSCR
+               406 BUILD_TUPLE              2
+               408 BINARY_SUBSCR
    
-   101         414 LOAD_NAME               24 (HttpResponse)
+    69         418 BUILD_TUPLE              6
+               420 LOAD_CONST              25 (<code object element, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 69>)
+               422 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
+               424 STORE_NAME              39 (element)
    
-   100         416 LOAD_CONST              25 ('additional')
+   112         426 NOP
    
-   101         418 LOAD_NAME               24 (HttpResponse)
+   111         428 LOAD_CONST              71 (('outerHTML',))
+               430 LOAD_CONST              14 ('response')
    
-   100         420 LOAD_CONST              15 ('return')
+   112         432 LOAD_NAME               24 (HttpResponse)
    
-   102         422 LOAD_NAME               24 (HttpResponse)
+   111         434 LOAD_CONST              26 ('additional')
    
-   100         424 BUILD_TUPLE              6
-               426 LOAD_CONST              26 (<code object swap_oob, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 100>)
-               428 MAKE_FUNCTION            5 (defaults, annotations)
-               430 STORE_NAME              40 (swap_oob)
+   112         436 LOAD_NAME               24 (HttpResponse)
    
-   123         432 LOAD_CONST              21 (False)
+   111         438 LOAD_CONST              15 ('return')
    
-   124         434 LOAD_CONST              20 (True)
+   113         440 LOAD_NAME               24 (HttpResponse)
    
-   121         436 LOAD_CONST              27 (('auto_param', 'auto_form'))
-               438 BUILD_CONST_KEY_MAP      2
-               440 LOAD_CONST              28 ('auto_param')
+   111         442 BUILD_TUPLE              6
+               444 LOAD_CONST              27 (<code object swap_oob, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 111>)
+               446 MAKE_FUNCTION            5 (defaults, annotations)
+               448 STORE_NAME              40 (swap_oob)
    
-   123         442 LOAD_NAME               41 (bool)
-               444 LOAD_NAME               10 (Literal)
-               446 LOAD_CONST              29 (('get', 'post'))
-               448 BINARY_SUBSCR
-               458 BINARY_OP                7 (|)
+   134         450 LOAD_CONST              21 (False)
    
-   121         462 LOAD_CONST              30 ('auto_form')
+   135         452 LOAD_CONST              20 (True)
    
-   124         464 LOAD_NAME               11 (Optional)
-               466 LOAD_NAME               41 (bool)
-               468 LOAD_NAME               38 (str)
-               470 BINARY_OP                7 (|)
-               474 BINARY_SUBSCR
+   132         454 LOAD_CONST              28 (('auto_param', 'auto_form'))
+               456 BUILD_CONST_KEY_MAP      2
+               458 LOAD_CONST              29 ('auto_param')
    
-   121         484 LOAD_CONST              15 ('return')
+   134         460 LOAD_NAME               41 (bool)
+               462 LOAD_NAME               10 (Literal)
+               464 LOAD_CONST              30 (('get', 'post'))
+               466 BINARY_SUBSCR
+               476 BINARY_OP                7 (|)
    
-   125         486 LOAD_NAME                9 (Callable)
-               488 LOAD_NAME                9 (Callable)
-               490 LOAD_NAME               32 (P)
-               492 LOAD_NAME               33 (R)
-               494 BUILD_TUPLE              2
-               496 BINARY_SUBSCR
-               506 BUILD_LIST               1
-               508 LOAD_NAME                9 (Callable)
-               510 LOAD_NAME               32 (P)
-               512 LOAD_NAME               33 (R)
-               514 BUILD_TUPLE              2
-               516 BINARY_SUBSCR
-               526 BUILD_TUPLE              2
-               528 BINARY_SUBSCR
+   132         480 LOAD_CONST              31 ('auto_form')
    
-   121         538 BUILD_TUPLE              6
-               540 LOAD_CONST              31 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 121>)
-               542 MAKE_FUNCTION            6 (kwdefaults, annotations)
-               544 STORE_NAME              42 (inject_args)
+   135         482 LOAD_NAME               11 (Optional)
+               484 LOAD_NAME               41 (bool)
+               486 LOAD_NAME               38 (str)
+               488 BINARY_OP                7 (|)
+               492 BINARY_SUBSCR
    
-   153         546 LOAD_NAME               42 (inject_args)
-               548 STORE_NAME              43 (_handle_args)
+   132         502 LOAD_CONST              15 ('return')
    
-   156         550 LOAD_NAME                0 (dataclasses)
-               552 LOAD_ATTR               44 (dataclass)
+   136         504 LOAD_NAME                9 (Callable)
+               506 LOAD_NAME                9 (Callable)
+               508 LOAD_NAME               32 (P)
+               510 LOAD_NAME               33 (R)
+               512 BUILD_TUPLE              2
+               514 BINARY_SUBSCR
+               524 BUILD_LIST               1
+               526 LOAD_NAME                9 (Callable)
+               528 LOAD_NAME               32 (P)
+               530 LOAD_NAME               33 (R)
+               532 BUILD_TUPLE              2
+               534 BINARY_SUBSCR
+               544 BUILD_TUPLE              2
+               546 BINARY_SUBSCR
    
-   157         562 PUSH_NULL
-               564 LOAD_BUILD_CLASS
-               566 LOAD_CONST              32 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 156>)
-               568 MAKE_FUNCTION            0
-               570 LOAD_CONST              33 ('InjectedParam')
-               572 PRECALL                  2
-               576 CALL                     2
+   132         556 BUILD_TUPLE              6
+               558 LOAD_CONST              32 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 132>)
+               560 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               562 STORE_NAME              42 (inject_args)
    
-   156         586 PRECALL                  0
-               590 CALL                     0
+   164         564 LOAD_NAME               42 (inject_args)
+               566 STORE_NAME              43 (_inject_args)
    
-   157         600 STORE_NAME              45 (InjectedParam)
+   167         568 LOAD_NAME                0 (dataclasses)
+               570 LOAD_ATTR               44 (dataclass)
    
-   173         602 LOAD_CONST              34 ('ip')
-               604 LOAD_NAME               45 (InjectedParam)
-               606 LOAD_CONST              35 ('name')
-               608 LOAD_NAME               38 (str)
-               610 LOAD_CONST              36 ('parameter')
-               612 LOAD_NAME                2 (inspect)
-               614 LOAD_ATTR               46 (Parameter)
-               624 BUILD_TUPLE              6
-               626 LOAD_CONST              37 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 173>)
-               628 MAKE_FUNCTION            4 (annotations)
-               630 STORE_NAME              47 (_setup_injected_param)
+   168         580 PUSH_NULL
+               582 LOAD_BUILD_CLASS
+               584 LOAD_CONST              33 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 167>)
+               586 MAKE_FUNCTION            0
+               588 LOAD_CONST              34 ('InjectedParam')
+               590 PRECALL                  2
+               594 CALL                     2
    
-   193         632 NOP
+   167         604 PRECALL                  0
+               608 CALL                     0
    
-   190         634 LOAD_CONST              71 ((True,))
-               636 LOAD_CONST              38 ('parameters')
+   168         618 STORE_NAME              45 (InjectedParam)
    
-   191         638 LOAD_NAME               48 (list)
-               640 LOAD_NAME                2 (inspect)
-               642 LOAD_ATTR               46 (Parameter)
-               652 BINARY_SUBSCR
+   184         620 LOAD_CONST              35 ('ip')
+               622 LOAD_NAME               45 (InjectedParam)
+               624 LOAD_CONST              36 ('name')
+               626 LOAD_NAME               38 (str)
+               628 LOAD_CONST              37 ('parameter')
+               630 LOAD_NAME                2 (inspect)
+               632 LOAD_ATTR               46 (Parameter)
+               642 BUILD_TUPLE              6
+               644 LOAD_CONST              38 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 184>)
+               646 MAKE_FUNCTION            4 (annotations)
+               648 STORE_NAME              47 (_setup_injected_param)
    
-   190         662 LOAD_CONST              28 ('auto_param')
+   204         650 NOP
    
-   192         664 LOAD_NAME               41 (bool)
-               666 LOAD_NAME               10 (Literal)
-               668 LOAD_CONST              39 ('get')
+   201         652 LOAD_CONST              72 ((True,))
+               654 LOAD_CONST              39 ('parameters')
+   
+   202         656 LOAD_NAME               48 (list)
+               658 LOAD_NAME                2 (inspect)
+               660 LOAD_ATTR               46 (Parameter)
                670 BINARY_SUBSCR
-               680 BINARY_OP                7 (|)
+   
+   201         680 LOAD_CONST              29 ('auto_param')
+   
+   203         682 LOAD_NAME               41 (bool)
                684 LOAD_NAME               10 (Literal)
-               686 LOAD_CONST              40 ('post')
+               686 LOAD_CONST              40 ('get')
                688 BINARY_SUBSCR
                698 BINARY_OP                7 (|)
-   
-   190         702 LOAD_CONST              30 ('auto_form')
-   
-   193         704 LOAD_NAME               11 (Optional)
-               706 LOAD_NAME               41 (bool)
-               708 LOAD_NAME               38 (str)
-               710 BINARY_OP                7 (|)
-               714 BINARY_SUBSCR
-   
-   190         724 LOAD_CONST              15 ('return')
-   
-   194         726 LOAD_NAME               49 (dict)
-               728 LOAD_NAME               38 (str)
-               730 LOAD_NAME               45 (InjectedParam)
-               732 BUILD_TUPLE              2
-               734 BINARY_SUBSCR
-   
-   190         744 BUILD_TUPLE              8
-               746 LOAD_CONST              41 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 190>)
-               748 MAKE_FUNCTION            5 (defaults, annotations)
-               750 STORE_NAME              50 (_extract_injected_params)
-   
-   243         752 LOAD_CONST              42 ('args')
-               754 LOAD_NAME               48 (list)
-               756 LOAD_NAME                8 (Any)
-               758 BINARY_SUBSCR
-               768 LOAD_CONST              15 ('return')
-               770 LOAD_NAME               23 (HttpRequest)
-               772 BUILD_TUPLE              4
-               774 LOAD_CONST              43 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 243>)
-               776 MAKE_FUNCTION            4 (annotations)
-               778 STORE_NAME              51 (_get_request_from_args)
-   
-   252         780 LOAD_NAME                0 (dataclasses)
-               782 LOAD_ATTR               44 (dataclass)
-   
-   253         792 PUSH_NULL
-               794 LOAD_BUILD_CLASS
-               796 LOAD_CONST              44 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 252>)
-               798 MAKE_FUNCTION            0
-               800 LOAD_CONST              45 ('InjectedParamQuery')
-               802 LOAD_NAME               45 (InjectedParam)
-               804 PRECALL                  3
-               808 CALL                     3
-   
-   252         818 PRECALL                  0
-               822 CALL                     0
-   
-   253         832 STORE_NAME              52 (InjectedParamQuery)
-   
-   300         834 LOAD_NAME                0 (dataclasses)
-               836 LOAD_ATTR               44 (dataclass)
-   
-   301         846 PUSH_NULL
-               848 LOAD_BUILD_CLASS
-               850 LOAD_CONST              46 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 300>)
-               852 MAKE_FUNCTION            0
-               854 LOAD_CONST              47 ('InjectedParamQueryGet')
-               856 LOAD_NAME               52 (InjectedParamQuery)
-               858 PRECALL                  3
-               862 CALL                     3
-   
-   300         872 PRECALL                  0
-               876 CALL                     0
-   
-   301         886 STORE_NAME              53 (InjectedParamQueryGet)
-   
-   313         888 LOAD_NAME                0 (dataclasses)
-               890 LOAD_ATTR               44 (dataclass)
-   
-   314         900 PUSH_NULL
-               902 LOAD_BUILD_CLASS
-               904 LOAD_CONST              48 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 313>)
-               906 MAKE_FUNCTION            0
-               908 LOAD_CONST              49 ('InjectedParamQueryPost')
-               910 LOAD_NAME               52 (InjectedParamQuery)
-               912 PRECALL                  3
-               916 CALL                     3
-   
-   313         926 PRECALL                  0
-               930 CALL                     0
-   
-   314         940 STORE_NAME              54 (InjectedParamQueryPost)
-   
-   326         942 LOAD_CONST              72 ((None, True))
-               944 LOAD_CONST              15 ('return')
-               946 LOAD_NAME                8 (Any)
-               948 BUILD_TUPLE              2
-               950 LOAD_CONST              50 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 326>)
-               952 MAKE_FUNCTION            5 (defaults, annotations)
-               954 STORE_NAME              55 (param_get)
-   
-   330         956 LOAD_CONST              72 ((None, True))
-               958 LOAD_CONST              15 ('return')
-               960 LOAD_NAME                8 (Any)
-               962 BUILD_TUPLE              2
-               964 LOAD_CONST              51 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 330>)
-               966 MAKE_FUNCTION            5 (defaults, annotations)
-               968 STORE_NAME              56 (param_post)
-   
-   334         970 PUSH_NULL
-               972 LOAD_NAME                4 (typing)
-               974 LOAD_ATTR               57 (cast)
-               984 LOAD_NAME                8 (Any)
-               986 LOAD_CONST               1 (None)
-               988 PRECALL                  2
-               992 CALL                     2
-              1002 LOAD_CONST              20 (True)
-              1004 BUILD_TUPLE              2
-              1006 LOAD_CONST              52 ('default')
-              1008 LOAD_NAME               34 (T)
-              1010 LOAD_CONST              15 ('return')
-              1012 LOAD_NAME               34 (T)
-              1014 BUILD_TUPLE              4
-              1016 LOAD_CONST              53 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 334>)
-              1018 MAKE_FUNCTION            5 (defaults, annotations)
-              1020 STORE_NAME              58 (param)
-   
-   338        1022 LOAD_CONST              54 ('values')
-              1024 LOAD_NAME               48 (list)
-              1026 LOAD_NAME                4 (typing)
-              1028 LOAD_ATTR                8 (Any)
-              1038 BINARY_SUBSCR
-              1048 LOAD_CONST              55 ('target_type')
-              1050 LOAD_NAME               59 (type)
-              1052 BUILD_TUPLE              4
-              1054 LOAD_CONST              56 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 338>)
-              1056 MAKE_FUNCTION            4 (annotations)
-              1058 STORE_NAME              60 (_convert_value_to_type)
-   
-   373        1060 PUSH_NULL
-              1062 LOAD_BUILD_CLASS
-              1064 LOAD_CONST              57 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 373>)
-              1066 MAKE_FUNCTION            0
-              1068 LOAD_CONST              58 ('InjectedParamForm')
-              1070 LOAD_NAME               45 (InjectedParam)
-              1072 PRECALL                  3
-              1076 CALL                     3
-              1086 STORE_NAME              61 (InjectedParamForm)
-   
-   419        1088 LOAD_CONST              15 ('return')
-              1090 LOAD_NAME                8 (Any)
-              1092 BUILD_TUPLE              2
-              1094 LOAD_CONST              59 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 419>)
-              1096 MAKE_FUNCTION            4 (annotations)
-              1098 STORE_NAME              62 (handle_form)
-   
-   428        1100 LOAD_CONST              60 ('querydict')
-              1102 LOAD_NAME               49 (dict)
-              1104 LOAD_CONST              15 ('return')
-              1106 LOAD_NAME               26 (QueryDict)
-              1108 BUILD_TUPLE              4
-              1110 LOAD_CONST              61 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 428>)
-              1112 MAKE_FUNCTION            4 (annotations)
-              1114 STORE_NAME              63 (querydict_key_removed)
-   
-   435        1116 LOAD_CONST              62 ('request')
-              1118 LOAD_NAME               23 (HttpRequest)
-              1120 BUILD_TUPLE              2
-              1122 LOAD_CONST              63 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 435>)
-              1124 MAKE_FUNCTION            4 (annotations)
-              1126 STORE_NAME              64 (is_head)
-   
-   439        1128 LOAD_CONST              62 ('request')
-              1130 LOAD_NAME               23 (HttpRequest)
-              1132 BUILD_TUPLE              2
-              1134 LOAD_CONST              64 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 439>)
-              1136 MAKE_FUNCTION            4 (annotations)
-              1138 STORE_NAME              65 (is_get)
-   
-   443        1140 LOAD_CONST              62 ('request')
-              1142 LOAD_NAME               23 (HttpRequest)
-              1144 BUILD_TUPLE              2
-              1146 LOAD_CONST              65 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 443>)
-              1148 MAKE_FUNCTION            4 (annotations)
-              1150 STORE_NAME              66 (is_post)
-   
-   447        1152 LOAD_CONST              62 ('request')
-              1154 LOAD_NAME               23 (HttpRequest)
-              1156 BUILD_TUPLE              2
-              1158 LOAD_CONST              66 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 447>)
-              1160 MAKE_FUNCTION            4 (annotations)
-              1162 STORE_NAME              67 (is_put)
-   
-   451        1164 LOAD_CONST              62 ('request')
-              1166 LOAD_NAME               23 (HttpRequest)
-              1168 BUILD_TUPLE              2
-              1170 LOAD_CONST              67 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 451>)
-              1172 MAKE_FUNCTION            4 (annotations)
-              1174 STORE_NAME              68 (is_patch)
-   
-   455        1176 LOAD_CONST              62 ('request')
-              1178 LOAD_NAME               23 (HttpRequest)
-              1180 BUILD_TUPLE              2
-              1182 LOAD_CONST              68 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 455>)
-              1184 MAKE_FUNCTION            4 (annotations)
-              1186 STORE_NAME              69 (is_delete)
-              1188 LOAD_CONST               1 (None)
-              1190 RETURN_VALUE
+               702 LOAD_NAME               10 (Literal)
+               704 LOAD_CONST              41 ('post')
+               706 BINARY_SUBSCR
+               716 BINARY_OP                7 (|)
+   
+   201         720 LOAD_CONST              31 ('auto_form')
+   
+   204         722 LOAD_NAME               11 (Optional)
+               724 LOAD_NAME               41 (bool)
+               726 LOAD_NAME               38 (str)
+               728 BINARY_OP                7 (|)
+               732 BINARY_SUBSCR
+   
+   201         742 LOAD_CONST              15 ('return')
+   
+   205         744 LOAD_NAME               49 (dict)
+               746 LOAD_NAME               38 (str)
+               748 LOAD_NAME               45 (InjectedParam)
+               750 BUILD_TUPLE              2
+               752 BINARY_SUBSCR
+   
+   201         762 BUILD_TUPLE              8
+               764 LOAD_CONST              42 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 201>)
+               766 MAKE_FUNCTION            5 (defaults, annotations)
+               768 STORE_NAME              50 (_extract_injected_params)
+   
+   254         770 LOAD_CONST              43 ('args')
+               772 LOAD_NAME               48 (list)
+               774 LOAD_NAME                8 (Any)
+               776 BINARY_SUBSCR
+               786 LOAD_CONST              15 ('return')
+               788 LOAD_NAME               23 (HttpRequest)
+               790 BUILD_TUPLE              4
+               792 LOAD_CONST              44 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 254>)
+               794 MAKE_FUNCTION            4 (annotations)
+               796 STORE_NAME              51 (_get_request_from_args)
+   
+   263         798 LOAD_NAME                0 (dataclasses)
+               800 LOAD_ATTR               44 (dataclass)
+   
+   264         810 PUSH_NULL
+               812 LOAD_BUILD_CLASS
+               814 LOAD_CONST              45 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 263>)
+               816 MAKE_FUNCTION            0
+               818 LOAD_CONST              46 ('InjectedParamQuery')
+               820 LOAD_NAME               45 (InjectedParam)
+               822 PRECALL                  3
+               826 CALL                     3
+   
+   263         836 PRECALL                  0
+               840 CALL                     0
+   
+   264         850 STORE_NAME              52 (InjectedParamQuery)
+   
+   311         852 LOAD_NAME                0 (dataclasses)
+               854 LOAD_ATTR               44 (dataclass)
+   
+   312         864 PUSH_NULL
+               866 LOAD_BUILD_CLASS
+               868 LOAD_CONST              47 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 311>)
+               870 MAKE_FUNCTION            0
+               872 LOAD_CONST              48 ('InjectedParamQueryGet')
+               874 LOAD_NAME               52 (InjectedParamQuery)
+               876 PRECALL                  3
+               880 CALL                     3
+   
+   311         890 PRECALL                  0
+               894 CALL                     0
+   
+   312         904 STORE_NAME              53 (InjectedParamQueryGet)
+   
+   324         906 LOAD_NAME                0 (dataclasses)
+               908 LOAD_ATTR               44 (dataclass)
+   
+   325         918 PUSH_NULL
+               920 LOAD_BUILD_CLASS
+               922 LOAD_CONST              49 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 324>)
+               924 MAKE_FUNCTION            0
+               926 LOAD_CONST              50 ('InjectedParamQueryPost')
+               928 LOAD_NAME               52 (InjectedParamQuery)
+               930 PRECALL                  3
+               934 CALL                     3
+   
+   324         944 PRECALL                  0
+               948 CALL                     0
+   
+   325         958 STORE_NAME              54 (InjectedParamQueryPost)
+   
+   337         960 LOAD_CONST              73 ((None, True))
+               962 LOAD_CONST              15 ('return')
+               964 LOAD_NAME                8 (Any)
+               966 BUILD_TUPLE              2
+               968 LOAD_CONST              51 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 337>)
+               970 MAKE_FUNCTION            5 (defaults, annotations)
+               972 STORE_NAME              55 (param_get)
+   
+   341         974 LOAD_CONST              73 ((None, True))
+               976 LOAD_CONST              15 ('return')
+               978 LOAD_NAME                8 (Any)
+               980 BUILD_TUPLE              2
+               982 LOAD_CONST              52 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 341>)
+               984 MAKE_FUNCTION            5 (defaults, annotations)
+               986 STORE_NAME              56 (param_post)
+   
+   345         988 PUSH_NULL
+               990 LOAD_NAME                4 (typing)
+               992 LOAD_ATTR               57 (cast)
+              1002 LOAD_NAME                8 (Any)
+              1004 LOAD_CONST               1 (None)
+              1006 PRECALL                  2
+              1010 CALL                     2
+              1020 LOAD_CONST              20 (True)
+              1022 BUILD_TUPLE              2
+              1024 LOAD_CONST              53 ('default')
+              1026 LOAD_NAME               34 (T)
+              1028 LOAD_CONST              15 ('return')
+              1030 LOAD_NAME               34 (T)
+              1032 BUILD_TUPLE              4
+              1034 LOAD_CONST              54 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 345>)
+              1036 MAKE_FUNCTION            5 (defaults, annotations)
+              1038 STORE_NAME              58 (param)
+   
+   349        1040 LOAD_CONST              55 ('values')
+              1042 LOAD_NAME               48 (list)
+              1044 LOAD_NAME                4 (typing)
+              1046 LOAD_ATTR                8 (Any)
+              1056 BINARY_SUBSCR
+              1066 LOAD_CONST              56 ('target_type')
+              1068 LOAD_NAME               59 (type)
+              1070 BUILD_TUPLE              4
+              1072 LOAD_CONST              57 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 349>)
+              1074 MAKE_FUNCTION            4 (annotations)
+              1076 STORE_NAME              60 (_convert_value_to_type)
+   
+   384        1078 PUSH_NULL
+              1080 LOAD_BUILD_CLASS
+              1082 LOAD_CONST              58 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 384>)
+              1084 MAKE_FUNCTION            0
+              1086 LOAD_CONST              59 ('InjectedParamForm')
+              1088 LOAD_NAME               45 (InjectedParam)
+              1090 PRECALL                  3
+              1094 CALL                     3
+              1104 STORE_NAME              61 (InjectedParamForm)
+   
+   430        1106 LOAD_CONST              15 ('return')
+              1108 LOAD_NAME                8 (Any)
+              1110 BUILD_TUPLE              2
+              1112 LOAD_CONST              60 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 430>)
+              1114 MAKE_FUNCTION            4 (annotations)
+              1116 STORE_NAME              62 (handle_form)
+   
+   439        1118 LOAD_CONST              61 ('querydict')
+              1120 LOAD_NAME               49 (dict)
+              1122 LOAD_CONST              15 ('return')
+              1124 LOAD_NAME               26 (QueryDict)
+              1126 BUILD_TUPLE              4
+              1128 LOAD_CONST              62 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 439>)
+              1130 MAKE_FUNCTION            4 (annotations)
+              1132 STORE_NAME              63 (querydict_key_removed)
+   
+   446        1134 LOAD_CONST              63 ('request')
+              1136 LOAD_NAME               23 (HttpRequest)
+              1138 BUILD_TUPLE              2
+              1140 LOAD_CONST              64 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 446>)
+              1142 MAKE_FUNCTION            4 (annotations)
+              1144 STORE_NAME              64 (is_head)
+   
+   450        1146 LOAD_CONST              63 ('request')
+              1148 LOAD_NAME               23 (HttpRequest)
+              1150 BUILD_TUPLE              2
+              1152 LOAD_CONST              65 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 450>)
+              1154 MAKE_FUNCTION            4 (annotations)
+              1156 STORE_NAME              65 (is_get)
+   
+   454        1158 LOAD_CONST              63 ('request')
+              1160 LOAD_NAME               23 (HttpRequest)
+              1162 BUILD_TUPLE              2
+              1164 LOAD_CONST              66 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 454>)
+              1166 MAKE_FUNCTION            4 (annotations)
+              1168 STORE_NAME              66 (is_post)
+   
+   458        1170 LOAD_CONST              63 ('request')
+              1172 LOAD_NAME               23 (HttpRequest)
+              1174 BUILD_TUPLE              2
+              1176 LOAD_CONST              67 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 458>)
+              1178 MAKE_FUNCTION            4 (annotations)
+              1180 STORE_NAME              67 (is_put)
+   
+   462        1182 LOAD_CONST              63 ('request')
+              1184 LOAD_NAME               23 (HttpRequest)
+              1186 BUILD_TUPLE              2
+              1188 LOAD_CONST              68 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 462>)
+              1190 MAKE_FUNCTION            4 (annotations)
+              1192 STORE_NAME              68 (is_patch)
+   
+   466        1194 LOAD_CONST              63 ('request')
+              1196 LOAD_NAME               23 (HttpRequest)
+              1198 BUILD_TUPLE              2
+              1200 LOAD_CONST              69 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 466>)
+              1202 MAKE_FUNCTION            4 (annotations)
+              1204 STORE_NAME              69 (is_delete)
+              1206 LOAD_CONST               1 (None)
+              1208 RETURN_VALUE
    consts
       0
       None
       ('NoneType',)
       ('Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar')
       ('forms',)
       ('decorators',)
@@ -570,21 +579,21 @@
       ('mark_safe', 'SafeString')
       'P'
       'R'
       'T'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 6
+         stacksize : 8
          flags     : 0
          code
             0x8700970065005a0164005a02650364016504660264028404a6000000ab
-            0000000000000000005a050900090009000900640b640765046408650665
-            07190000000000000000006604880066016409840d5a08640a84005a0988
-            0078015a0a5300
+            0000000000000000005a0509000900090009000900640d64086504640965
+            06650719000000000000000000640a650665071900000000000000000066
+            0688006601640b840d5a08640c84005a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
           28           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ElementResponse')
                       10 STORE_NAME               2 (__qualname__)
@@ -606,39 +615,47 @@
          
           38          42 NOP
          
           39          44 NOP
          
           40          46 NOP
          
-          33          48 LOAD_CONST              11 (('div', 'this', 'outerHTML', False))
-                      50 LOAD_CONST               7 ('response')
+          41          48 NOP
+         
+          33          50 LOAD_CONST              13 (('div', 'this', 'outerHTML', None, False))
+                      52 LOAD_CONST               8 ('response')
+         
+          35          54 LOAD_NAME                4 (HttpResponse)
+         
+          33          56 LOAD_CONST               9 ('element_id')
+         
+          36          58 LOAD_NAME                6 (Optional)
+                      60 LOAD_NAME                7 (str)
+                      62 BINARY_SUBSCR
+         
+          33          72 LOAD_CONST              10 ('classes')
          
-          35          52 LOAD_NAME                4 (HttpResponse)
+          40          74 LOAD_NAME                6 (Optional)
+                      76 LOAD_NAME                7 (str)
+                      78 BINARY_SUBSCR
          
-          33          54 LOAD_CONST               8 ('element_id')
+          33          88 BUILD_TUPLE              6
+                      90 LOAD_CLOSURE             0 (__class__)
+                      92 BUILD_TUPLE              1
+                      94 LOAD_CONST              11 (<code object __init__, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 33>)
+                      96 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                      98 STORE_NAME               8 (__init__)
          
-          36          56 LOAD_NAME                6 (Optional)
-                      58 LOAD_NAME                7 (str)
-                      60 BINARY_SUBSCR
-         
-          33          70 BUILD_TUPLE              4
-                      72 LOAD_CLOSURE             0 (__class__)
-                      74 BUILD_TUPLE              1
-                      76 LOAD_CONST               9 (<code object __init__, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 33>)
-                      78 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                      80 STORE_NAME               8 (__init__)
-         
-          51          82 LOAD_CONST              10 (<code object __str__, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 51>)
-                      84 MAKE_FUNCTION            0
-                      86 STORE_NAME               9 (__str__)
-                      88 LOAD_CLOSURE             0 (__class__)
-                      90 COPY                     1
-                      92 STORE_NAME              10 (__classcell__)
-                      94 RETURN_VALUE
+          57         100 LOAD_CONST              12 (<code object __str__, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 57>)
+                     102 MAKE_FUNCTION            0
+                     104 STORE_NAME               9 (__str__)
+                     106 LOAD_CLOSURE             0 (__class__)
+                     108 COPY                     1
+                     110 STORE_NAME              10 (__classcell__)
+                     112 RETURN_VALUE
          consts
             'ElementResponse'
             'return'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 5
@@ -670,169 +687,194 @@
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'empty'
                firstlineno 29
                lnotab 0x0202
             'div'
             'this'
             'outerHTML'
+            None
             False
             'response'
             'element_id'
+            'classes'
             code
-               argcount  : 7
-               nlocals   : 11
-               stacksize : 13
+               argcount  : 8
+               nlocals   : 13
+               stacksize : 15
                flags     : 3
                code
-                  0x950197007c0673557c02810664017c029b0064029d036e0164037d077c
-                  04720664047c049b0064029d036e0164037d087c05720664057c059b0064
-                  029d036e0164037d0964067c039b0064077c079b0064077c089b0064077c
-                  099b0064087401000000000000000000007c01a6010000ab010000000000
-                  0000009b0064097c039b0064089d0d7d0a7403000000000000000000007c
-                  0a640aa6020000ab0200000000000000007c015f02000000000000000074
-                  0700000000000000000000a6000000ab000000000000000000a004000000
-                  00000000000000000000000000000000007c01a6010000ab010000000000
-                  000000010064005300
+                  0x950197007c0773627c02810664017c029b0064029d036e0164037d087c
+                  04720664047c049b0064029d036e0164037d097c05720664057c059b0064
+                  029d036e0164037d0a7c06720664067c069b0064029d036e0164037d0b64
+                  077c039b0064087c089b0064087c099b0064087c0a9b0064087c0b9b0064
+                  097401000000000000000000007c01a6010000ab0100000000000000009b
+                  00640a7c039b0064099d0f7d0c7403000000000000000000007c0c640ba6
+                  020000ab0200000000000000007c015f0200000000000000007407000000
+                  00000000000000a6000000ab000000000000000000a00400000000000000
+                  000000000000000000000000007c01a6010000ab01000000000000000001
+                  0064005300
                              0 COPY_FREE_VARS           1
                
                 33           2 RESUME                   0
                
-                42           4 LOAD_FAST                6 (no_element_wrap)
-                             6 POP_JUMP_FORWARD_IF_TRUE    85 (to 178)
+                43           4 LOAD_FAST                7 (no_element_wrap)
+                             6 POP_JUMP_FORWARD_IF_TRUE    98 (to 204)
                
-                43           8 LOAD_FAST                2 (element_id)
+                44           8 LOAD_FAST                2 (element_id)
                             10 POP_JUMP_FORWARD_IF_NONE     6 (to 24)
                             12 LOAD_CONST               1 ("id='")
                             14 LOAD_FAST                2 (element_id)
                             16 FORMAT_VALUE             0
                             18 LOAD_CONST               2 ("'")
                             20 BUILD_STRING             3
                             22 JUMP_FORWARD             1 (to 26)
                        >>   24 LOAD_CONST               3 ('')
-                       >>   26 STORE_FAST               7 (attr_id)
+                       >>   26 STORE_FAST               8 (attr_id)
                
-                44          28 LOAD_FAST                4 (hx_target)
+                45          28 LOAD_FAST                4 (hx_target)
                             30 POP_JUMP_FORWARD_IF_FALSE     6 (to 44)
                             32 LOAD_CONST               4 ("hx-target='")
                             34 LOAD_FAST                4 (hx_target)
                             36 FORMAT_VALUE             0
                             38 LOAD_CONST               2 ("'")
                             40 BUILD_STRING             3
                             42 JUMP_FORWARD             1 (to 46)
                        >>   44 LOAD_CONST               3 ('')
-                       >>   46 STORE_FAST               8 (attr_hx_target)
+                       >>   46 STORE_FAST               9 (attr_hx_target)
                
-                45          48 LOAD_FAST                5 (hx_swap)
+                46          48 LOAD_FAST                5 (hx_swap)
                             50 POP_JUMP_FORWARD_IF_FALSE     6 (to 64)
                             52 LOAD_CONST               5 ("hx-swap='")
                             54 LOAD_FAST                5 (hx_swap)
                             56 FORMAT_VALUE             0
                             58 LOAD_CONST               2 ("'")
                             60 BUILD_STRING             3
                             62 JUMP_FORWARD             1 (to 66)
                        >>   64 LOAD_CONST               3 ('')
-                       >>   66 STORE_FAST               9 (attr_hx_swap)
+                       >>   66 STORE_FAST              10 (attr_hx_swap)
                
-                46          68 LOAD_CONST               6 ('<')
-                            70 LOAD_FAST                3 (tag)
-                            72 FORMAT_VALUE             0
-                            74 LOAD_CONST               7 (' ')
-                            76 LOAD_FAST                7 (attr_id)
-                            78 FORMAT_VALUE             0
-                            80 LOAD_CONST               7 (' ')
-                            82 LOAD_FAST                8 (attr_hx_target)
-                            84 FORMAT_VALUE             0
-                            86 LOAD_CONST               7 (' ')
-                            88 LOAD_FAST                9 (attr_hx_swap)
-                            90 FORMAT_VALUE             0
-                            92 LOAD_CONST               8 ('>')
-                            94 LOAD_GLOBAL              1 (NULL + response_to_str)
-                           106 LOAD_FAST                1 (response)
-                           108 PRECALL                  1
-                           112 CALL                     1
-                           122 FORMAT_VALUE             0
-                           124 LOAD_CONST               9 ('</')
-                           126 LOAD_FAST                3 (tag)
-                           128 FORMAT_VALUE             0
-                           130 LOAD_CONST               8 ('>')
-                           132 BUILD_STRING            13
-                           134 STORE_FAST              10 (new_content)
-               
-                47         136 LOAD_GLOBAL              3 (NULL + bytes)
-                           148 LOAD_FAST               10 (new_content)
-                           150 LOAD_CONST              10 ('UTF-8')
-                           152 PRECALL                  2
-                           156 CALL                     2
-                           166 LOAD_FAST                1 (response)
-                           168 STORE_ATTR               2 (content)
-               
-                49     >>  178 LOAD_GLOBAL              7 (NULL + super)
-                           190 PRECALL                  0
-                           194 CALL                     0
-                           204 LOAD_METHOD              4 (__init__)
-                           226 LOAD_FAST                1 (response)
-                           228 PRECALL                  1
-                           232 CALL                     1
-                           242 POP_TOP
-                           244 LOAD_CONST               0 (None)
-                           246 RETURN_VALUE
+                47          68 LOAD_FAST                6 (classes)
+                            70 POP_JUMP_FORWARD_IF_FALSE     6 (to 84)
+                            72 LOAD_CONST               6 ("class='")
+                            74 LOAD_FAST                6 (classes)
+                            76 FORMAT_VALUE             0
+                            78 LOAD_CONST               2 ("'")
+                            80 BUILD_STRING             3
+                            82 JUMP_FORWARD             1 (to 86)
+                       >>   84 LOAD_CONST               3 ('')
+                       >>   86 STORE_FAST              11 (attr_classes)
+               
+                49          88 LOAD_CONST               7 ('<')
+                            90 LOAD_FAST                3 (tag)
+                            92 FORMAT_VALUE             0
+                            94 LOAD_CONST               8 (' ')
+                            96 LOAD_FAST                8 (attr_id)
+                            98 FORMAT_VALUE             0
+                           100 LOAD_CONST               8 (' ')
+                           102 LOAD_FAST                9 (attr_hx_target)
+                           104 FORMAT_VALUE             0
+                           106 LOAD_CONST               8 (' ')
+                           108 LOAD_FAST               10 (attr_hx_swap)
+                           110 FORMAT_VALUE             0
+                           112 LOAD_CONST               8 (' ')
+                           114 LOAD_FAST               11 (attr_classes)
+                           116 FORMAT_VALUE             0
+                           118 LOAD_CONST               9 ('>')
+               
+                50         120 LOAD_GLOBAL              1 (NULL + response_to_str)
+                           132 LOAD_FAST                1 (response)
+                           134 PRECALL                  1
+                           138 CALL                     1
+               
+                49         148 FORMAT_VALUE             0
+                           150 LOAD_CONST              10 ('</')
+               
+                51         152 LOAD_FAST                3 (tag)
+               
+                49         154 FORMAT_VALUE             0
+                           156 LOAD_CONST               9 ('>')
+                           158 BUILD_STRING            15
+               
+                48         160 STORE_FAST              12 (new_content)
+               
+                53         162 LOAD_GLOBAL              3 (NULL + bytes)
+                           174 LOAD_FAST               12 (new_content)
+                           176 LOAD_CONST              11 ('UTF-8')
+                           178 PRECALL                  2
+                           182 CALL                     2
+                           192 LOAD_FAST                1 (response)
+                           194 STORE_ATTR               2 (content)
+               
+                55     >>  204 LOAD_GLOBAL              7 (NULL + super)
+                           216 PRECALL                  0
+                           220 CALL                     0
+                           230 LOAD_METHOD              4 (__init__)
+                           252 LOAD_FAST                1 (response)
+                           254 PRECALL                  1
+                           258 CALL                     1
+                           268 POP_TOP
+                           270 LOAD_CONST               0 (None)
+                           272 RETURN_VALUE
                consts
                   None
                   "id='"
                   "'"
                   ''
                   "hx-target='"
                   "hx-swap='"
+                  "class='"
                   '<'
                   ' '
                   '>'
                   '</'
                   'UTF-8'
                names      ('response_to_str', 'bytes', 'content', 'super', '__init__')
-               varnames   ('self', 'response', 'element_id', 'tag', 'hx_target', 'hx_swap', 'no_element_wrap', 'attr_id', 'attr_hx_target', 'attr_hx_swap', 'new_content')
+               varnames   ('self', 'response', 'element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'no_element_wrap', 'attr_id', 'attr_hx_target', 'attr_hx_swap', 'attr_classes', 'new_content')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '__init__'
                firstlineno 33
-               lnotab 0x0409040114011401140144012a02
+               lnotab 0x040a0401140114011401140220011cff040202fe06ff02052a02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-                51           0 RESUME                   0
+                57           0 RESUME                   0
                
-                52           2 LOAD_GLOBAL              1 (NULL + response_to_str)
+                58           2 LOAD_GLOBAL              1 (NULL + response_to_str)
                             14 LOAD_FAST                0 (self)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('response_to_str',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '__str__'
-               firstlineno 51
+               firstlineno 57
                lnotab 0x0201
-            ('div', 'this', 'outerHTML', False)
+            ('div', 'this', 'outerHTML', None, False)
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'HttpResponse', 'empty', 'Optional', 'str', '__init__', '__str__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'ElementResponse'
          firstlineno 28
-         lnotab 0x0c0102010aff0e01020702010201020102f9040202fe02030efd0c12
+         lnotab
+            0x0c0102010aff0e010207020102010201020102f8040202fe02030efd02
+            070ef90c18
       'ElementResponse'
       'response'
       'return'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
@@ -840,30 +882,30 @@
          code
             0x97007401000000000000000000007c00740200000000000000000000a6
             020000ab02000000000000000072147c00a0020000000000000000000000
             000000000000000000a6000000ab0000000000000000007d007407000000
             000000000000007409000000000000000000007c006a0500000000000000
             006401a6020000ab020000000000000000a6010000ab0100000000000000
             005300
-          55           0 RESUME                   0
+          61           0 RESUME                   0
          
-          56           2 LOAD_GLOBAL              1 (NULL + isinstance)
+          62           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (response)
                       16 LOAD_GLOBAL              2 (TemplateResponse)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_FALSE    20 (to 84)
          
-          57          44 LOAD_FAST                0 (response)
+          63          44 LOAD_FAST                0 (response)
                       46 LOAD_METHOD              2 (render)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 STORE_FAST               0 (response)
          
-          59     >>   84 LOAD_GLOBAL              7 (NULL + mark_safe)
+          65     >>   84 LOAD_GLOBAL              7 (NULL + mark_safe)
                       96 LOAD_GLOBAL              9 (NULL + str)
                      108 LOAD_FAST                0 (response)
                      110 LOAD_ATTR                5 (content)
                      120 LOAD_CONST               1 ('utf-8')
                      122 PRECALL                  2
                      126 CALL                     2
                      136 PRECALL                  1
@@ -874,261 +916,267 @@
             'utf-8'
          names      ('isinstance', 'TemplateResponse', 'render', 'mark_safe', 'str', 'content')
          varnames   ('response',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'response_to_str'
-         firstlineno 55
+         firstlineno 61
          lnotab 0x02012a012802
       'div'
       'this'
       'outerHTML'
       True
       False
-      ('tag', 'hx_target', 'hx_swap', 'handle_args', 'login_required')
+      ('tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required')
       'element_id'
+      'classes'
       code
          argcount  : 1
-         nlocals   : 7
-         stacksize : 7
+         nlocals   : 8
+         stacksize : 8
          flags     : 3
          code
-            0x8700870187028703870487059700640174000000000000000000000074
-            020000000000000000000074040000000000000000000066021900000000
-            000000000064027400000000000000000000007402000000000000000000
-            007404000000000000000000006602190000000000000000006604880088
-            04880388028805880166066403840c7d067c065300
+            0x8700870187028703870487058706970064017400000000000000000000
+            007402000000000000000000007404000000000000000000006602190000
+            000000000000006402740000000000000000000000740200000000000000
+            000000740400000000000000000000660219000000000000000000660488
+            0488008805880388028806880166076403840c7d077c075300
                        0 MAKE_CELL                0 (element_id)
                        2 MAKE_CELL                1 (tag)
                        4 MAKE_CELL                2 (hx_target)
                        6 MAKE_CELL                3 (hx_swap)
-                       8 MAKE_CELL                4 (handle_args)
-                      10 MAKE_CELL                5 (login_required)
-         
-          63          12 RESUME                   0
-         
-          72          14 LOAD_CONST               1 ('f')
-                      16 LOAD_GLOBAL              0 (Callable)
-                      28 LOAD_GLOBAL              2 (P)
-                      40 LOAD_GLOBAL              4 (HttpResponse)
-                      52 BUILD_TUPLE              2
-                      54 BINARY_SUBSCR
-                      64 LOAD_CONST               2 ('return')
-                      66 LOAD_GLOBAL              0 (Callable)
-                      78 LOAD_GLOBAL              2 (P)
-                      90 LOAD_GLOBAL              4 (HttpResponse)
-                     102 BUILD_TUPLE              2
-                     104 BINARY_SUBSCR
-                     114 BUILD_TUPLE              4
-                     116 LOAD_CLOSURE             0 (element_id)
-                     118 LOAD_CLOSURE             4 (handle_args)
-                     120 LOAD_CLOSURE             3 (hx_swap)
-                     122 LOAD_CLOSURE             2 (hx_target)
-                     124 LOAD_CLOSURE             5 (login_required)
-                     126 LOAD_CLOSURE             1 (tag)
-                     128 BUILD_TUPLE              6
-                     130 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 72>)
-                     132 MAKE_FUNCTION           12 (annotations, closure)
-                     134 STORE_FAST               6 (decorator)
+                       8 MAKE_CELL                4 (classes)
+                      10 MAKE_CELL                5 (handle_args)
+                      12 MAKE_CELL                6 (login_required)
+         
+          69          14 RESUME                   0
+         
+          79          16 LOAD_CONST               1 ('f')
+                      18 LOAD_GLOBAL              0 (Callable)
+                      30 LOAD_GLOBAL              2 (P)
+                      42 LOAD_GLOBAL              4 (HttpResponse)
+                      54 BUILD_TUPLE              2
+                      56 BINARY_SUBSCR
+                      66 LOAD_CONST               2 ('return')
+                      68 LOAD_GLOBAL              0 (Callable)
+                      80 LOAD_GLOBAL              2 (P)
+                      92 LOAD_GLOBAL              4 (HttpResponse)
+                     104 BUILD_TUPLE              2
+                     106 BINARY_SUBSCR
+                     116 BUILD_TUPLE              4
+                     118 LOAD_CLOSURE             4 (classes)
+                     120 LOAD_CLOSURE             0 (element_id)
+                     122 LOAD_CLOSURE             5 (handle_args)
+                     124 LOAD_CLOSURE             3 (hx_swap)
+                     126 LOAD_CLOSURE             2 (hx_target)
+                     128 LOAD_CLOSURE             6 (login_required)
+                     130 LOAD_CLOSURE             1 (tag)
+                     132 BUILD_TUPLE              7
+                     134 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 79>)
+                     136 MAKE_FUNCTION           12 (annotations, closure)
+                     138 STORE_FAST               7 (decorator)
          
-          97         136 LOAD_FAST                6 (decorator)
-                     138 RETURN_VALUE
+         108         140 LOAD_FAST                7 (decorator)
+                     142 RETURN_VALUE
          consts
             None
             'f'
             'return'
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 7
+               stacksize : 8
                flags     : 19
                code
-                  0x9506870087029700740100000000000000000000890374020000000000
-                  0000000000a6020000ab020000000000000000720289036e0689006a0200
-                  000000000000008a02890472170200740700000000000000000000a60000
+                  0x9507870087029700740100000000000000000000890474020000000000
+                  0000000000a6020000ab020000000000000000720289046e0689006a0200
+                  000000000000008a02890572170200740700000000000000000000a60000
                   00ab0000000000000000008900a6010000ab0100000000000000008a0089
-                  07721c02007409000000000000000000006a050000000000000000a60000
+                  08721c02007409000000000000000000006a050000000000000000a60000
                   00ab0000000000000000008900a6010000ab0100000000000000008a0074
                   0d000000000000000000006a0700000000000000008900a6010000ab0100
                   0000000000000064017410000000000000000000006a0900000000000000
                   0064027410000000000000000000006a0a00000000000000006403741600
-                  00000000000000000066068800880588068802880866056404840ca60000
-                  00ab0000000000000000007d017c015300
-                             0 COPY_FREE_VARS           6
+                  000000000000000000660688038800880688078802880966066404840ca6
+                  000000ab0000000000000000007d017c015300
+                             0 COPY_FREE_VARS           7
                              2 MAKE_CELL                0 (f)
                              4 MAKE_CELL                2 (id)
                
-                72           6 RESUME                   0
+                79           6 RESUME                   0
                
-                73           8 LOAD_GLOBAL              1 (NULL + isinstance)
-                            20 LOAD_DEREF               3 (element_id)
+                80           8 LOAD_GLOBAL              1 (NULL + isinstance)
+                            20 LOAD_DEREF               4 (element_id)
                             22 LOAD_GLOBAL              2 (str)
                             34 PRECALL                  2
                             38 CALL                     2
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
-                            50 LOAD_DEREF               3 (element_id)
+                            50 LOAD_DEREF               4 (element_id)
                             52 JUMP_FORWARD             6 (to 66)
                        >>   54 LOAD_DEREF               0 (f)
                             56 LOAD_ATTR                2 (__name__)
                        >>   66 STORE_DEREF              2 (id)
                
-                75          68 LOAD_DEREF               4 (handle_args)
+                82          68 LOAD_DEREF               5 (handle_args)
                             70 POP_JUMP_FORWARD_IF_FALSE    23 (to 118)
                
-                76          72 PUSH_NULL
-                            74 LOAD_GLOBAL              7 (NULL + _handle_args)
+                83          72 PUSH_NULL
+                            74 LOAD_GLOBAL              7 (NULL + _inject_args)
                             86 PRECALL                  0
                             90 CALL                     0
                            100 LOAD_DEREF               0 (f)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 STORE_DEREF              0 (f)
                
-                78     >>  118 LOAD_DEREF               7 (login_required)
+                85     >>  118 LOAD_DEREF               8 (login_required)
                            120 POP_JUMP_FORWARD_IF_FALSE    28 (to 178)
                
-                79         122 PUSH_NULL
+                86         122 PUSH_NULL
                            124 LOAD_GLOBAL              9 (NULL + auth_decorators)
                            136 LOAD_ATTR                5 (login_required)
                            146 PRECALL                  0
                            150 CALL                     0
                            160 LOAD_DEREF               0 (f)
                            162 PRECALL                  1
                            166 CALL                     1
                            176 STORE_DEREF              0 (f)
                
-                81     >>  178 LOAD_GLOBAL             13 (NULL + functools)
+                88     >>  178 LOAD_GLOBAL             13 (NULL + functools)
                            190 LOAD_ATTR                7 (wraps)
                            200 LOAD_DEREF               0 (f)
                            202 PRECALL                  1
                            206 CALL                     1
                
-                82         216 LOAD_CONST               1 ('args')
+                89         216 LOAD_CONST               1 ('args')
                            218 LOAD_GLOBAL             16 (P)
                            230 LOAD_ATTR                9 (args)
                            240 LOAD_CONST               2 ('kwargs')
                            242 LOAD_GLOBAL             16 (P)
                            254 LOAD_ATTR               10 (kwargs)
                            264 LOAD_CONST               3 ('return')
                            266 LOAD_GLOBAL             22 (HttpResponse)
                            278 BUILD_TUPLE              6
-                           280 LOAD_CLOSURE             0 (f)
-                           282 LOAD_CLOSURE             5 (hx_swap)
-                           284 LOAD_CLOSURE             6 (hx_target)
-                           286 LOAD_CLOSURE             2 (id)
-                           288 LOAD_CLOSURE             8 (tag)
-                           290 BUILD_TUPLE              5
-                           292 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 81>)
-                           294 MAKE_FUNCTION           12 (annotations, closure)
+                           280 LOAD_CLOSURE             3 (classes)
+                           282 LOAD_CLOSURE             0 (f)
+                           284 LOAD_CLOSURE             6 (hx_swap)
+                           286 LOAD_CLOSURE             7 (hx_target)
+                           288 LOAD_CLOSURE             2 (id)
+                           290 LOAD_CLOSURE             9 (tag)
+                           292 BUILD_TUPLE              6
+                           294 LOAD_CONST               4 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 88>)
+                           296 MAKE_FUNCTION           12 (annotations, closure)
                
-                81         296 PRECALL                  0
-                           300 CALL                     0
+                88         298 PRECALL                  0
+                           302 CALL                     0
                
-                82         310 STORE_FAST               1 (inner)
+                89         312 STORE_FAST               1 (inner)
                
-                95         312 LOAD_FAST                1 (inner)
-                           314 RETURN_VALUE
+               106         314 LOAD_FAST                1 (inner)
+                           316 RETURN_VALUE
                consts
                   None
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
                      nlocals   : 3
-                     stacksize : 7
+                     stacksize : 8
                      flags     : 31
                      code
-                        0x95059700020089037c0069007c01a4018e017d027c026a000000000000
-                        00000001007c02640119000000000000000000a001000000000000000000
-                        00000000000000000000006402a6010000ab01000000000000000073027c
-                        0253007405000000000000000000007c02740600000000000000000000a6
-                        020000ab02000000000000000072027c0253007407000000000000000000
-                        007c028906890789058904ac03a6050000ab0500000000000000005300
-                                   0 COPY_FREE_VARS           5
+                        0x95069700020089047c0069007c01a4018e017d027c0264011900000000
+                        0000000000a00000000000000000000000000000000000000000006402a6
+                        010000ab01000000000000000073027c0253007403000000000000000000
+                        007c02740400000000000000000000a6020000ab02000000000000000072
+                        027c0253007405000000000000000000007c0289078908890689058903ac
+                        03a6060000ab0600000000000000005300
+                                   0 COPY_FREE_VARS           6
                      
-                      81           2 RESUME                   0
+                      88           2 RESUME                   0
                      
-                      83           4 PUSH_NULL
-                                   6 LOAD_DEREF               3 (f)
+                      90           4 PUSH_NULL
+                                   6 LOAD_DEREF               4 (f)
                                    8 LOAD_FAST                0 (args)
                                   10 BUILD_MAP                0
                                   12 LOAD_FAST                1 (kwargs)
                                   14 DICT_MERGE               1
                                   16 CALL_FUNCTION_EX         1
                                   18 STORE_FAST               2 (response)
                      
-                      84          20 LOAD_FAST                2 (response)
-                                  22 LOAD_ATTR                0 (streaming)
-                                  32 POP_TOP
+                      91          20 LOAD_FAST                2 (response)
+                                  22 LOAD_CONST               1 ('Content-Type')
+                                  24 BINARY_SUBSCR
+                                  34 LOAD_METHOD              0 (startswith)
+                                  56 LOAD_CONST               2 ('text/html')
+                                  58 PRECALL                  1
+                                  62 CALL                     1
+                                  72 POP_JUMP_FORWARD_IF_TRUE     2 (to 78)
                      
-                      85          34 LOAD_FAST                2 (response)
-                                  36 LOAD_CONST               1 ('Content-Type')
-                                  38 BINARY_SUBSCR
-                                  48 LOAD_METHOD              1 (startswith)
-                                  70 LOAD_CONST               2 ('text/html')
-                                  72 PRECALL                  1
-                                  76 CALL                     1
-                                  86 POP_JUMP_FORWARD_IF_TRUE     2 (to 92)
-                     
-                      86          88 LOAD_FAST                2 (response)
-                                  90 RETURN_VALUE
-                     
-                      88     >>   92 LOAD_GLOBAL              5 (NULL + isinstance)
-                                 104 LOAD_FAST                2 (response)
-                                 106 LOAD_GLOBAL              6 (ElementResponse)
-                                 118 PRECALL                  2
-                                 122 CALL                     2
-                                 132 POP_JUMP_FORWARD_IF_FALSE     2 (to 138)
-                     
-                      89         134 LOAD_FAST                2 (response)
-                                 136 RETURN_VALUE
-                     
-                      91     >>  138 LOAD_GLOBAL              7 (NULL + ElementResponse)
-                     
-                      92         150 LOAD_FAST                2 (response)
-                                 152 LOAD_DEREF               6 (id)
-                                 154 LOAD_DEREF               7 (tag)
-                                 156 LOAD_DEREF               5 (hx_target)
-                                 158 LOAD_DEREF               4 (hx_swap)
-                     
-                      91         160 KW_NAMES                 3
-                                 162 PRECALL                  5
-                                 166 CALL                     5
-                                 176 RETURN_VALUE
+                      92          74 LOAD_FAST                2 (response)
+                                  76 RETURN_VALUE
+                     
+                      94     >>   78 LOAD_GLOBAL              3 (NULL + isinstance)
+                                  90 LOAD_FAST                2 (response)
+                                  92 LOAD_GLOBAL              4 (ElementResponse)
+                                 104 PRECALL                  2
+                                 108 CALL                     2
+                                 118 POP_JUMP_FORWARD_IF_FALSE     2 (to 124)
+                     
+                      95         120 LOAD_FAST                2 (response)
+                                 122 RETURN_VALUE
+                     
+                      97     >>  124 LOAD_GLOBAL              5 (NULL + ElementResponse)
+                     
+                      98         136 LOAD_FAST                2 (response)
+                     
+                      99         138 LOAD_DEREF               7 (id)
+                     
+                     100         140 LOAD_DEREF               8 (tag)
+                     
+                     101         142 LOAD_DEREF               6 (hx_target)
+                     
+                     102         144 LOAD_DEREF               5 (hx_swap)
+                     
+                     103         146 LOAD_DEREF               3 (classes)
+                     
+                      97         148 KW_NAMES                 3
+                                 150 PRECALL                  6
+                                 154 CALL                     6
+                                 164 RETURN_VALUE
                      consts
                         None
                         'Content-Type'
                         'text/html'
-                        ('element_id', 'tag', 'hx_target', 'hx_swap')
-                     names      ('streaming', 'startswith', 'isinstance', 'ElementResponse')
+                        ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes')
+                     names      ('startswith', 'isinstance', 'ElementResponse')
                      varnames   ('args', 'kwargs', 'response')
-                     freevars   ('f', 'hx_swap', 'hx_target', 'id', 'tag')
+                     freevars   ('classes', 'f', 'hx_swap', 'hx_target', 'id', 'tag')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 81
-                     lnotab 0x040210010e01360104022a0104020c010aff
-               names      ('isinstance', 'str', '__name__', '_handle_args', 'auth_decorators', 'login_required', 'functools', 'wraps', 'P', 'args', 'kwargs', 'HttpResponse')
+                     firstlineno 88
+                     lnotab 0x04021001360104022a0104020c010201020102010201020102fa
+               names      ('isinstance', 'str', '__name__', '_inject_args', 'auth_decorators', 'login_required', 'functools', 'wraps', 'P', 'args', 'kwargs', 'HttpResponse')
                varnames   ('f', 'inner')
-               freevars   ('element_id', 'handle_args', 'hx_swap', 'hx_target', 'login_required', 'tag')
+               freevars   ('classes', 'element_id', 'handle_args', 'hx_swap', 'hx_target', 'login_required', 'tag')
                cellvars   ('f', 'id')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 72
-               lnotab 0x08013c0204012e0204013802260150ff0e01020d
+               firstlineno 79
+               lnotab 0x08013c0204012e0204013802260152ff0e010211
          names      ('Callable', 'P', 'HttpResponse')
-         varnames   ('element_id', 'tag', 'hx_target', 'hx_swap', 'handle_args', 'login_required', 'decorator')
+         varnames   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required', 'decorator')
          freevars   ()
-         cellvars   ('element_id', 'tag', 'hx_target', 'hx_swap', 'handle_args', 'login_required')
+         cellvars   ('element_id', 'tag', 'hx_target', 'hx_swap', 'classes', 'handle_args', 'login_required')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'element'
-         firstlineno 63
-         lnotab 0x0e097a19
+         firstlineno 69
+         lnotab 0x100a7c1d
       'additional'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1140,91 +1188,91 @@
             0000000000000000000000000000006401a6010000ab0100000000000000
             007d057c05800f740f000000000000000000006402a6010000ab01000000
             000000000082017c029b0064037c059b009d037c046a0500000000000000
             0064043c0000007c0078016a080000000000000000740400000000000000
             0000006a030000000000000000a009000000000000000000000000000000
             00000000007c04a6010000ab0100000000000000007a0d000063025f0800
             000000000000007c005300
-         100           0 RESUME                   0
+         111           0 RESUME                   0
          
-         103           2 LOAD_GLOBAL              1 (NULL + response_to_str)
+         114           2 LOAD_GLOBAL              1 (NULL + response_to_str)
                       14 LOAD_FAST                1 (additional)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_METHOD              1 (strip)
                       52 PRECALL                  0
                       56 CALL                     0
                       66 STORE_FAST               3 (oob_content)
          
-         104          68 LOAD_GLOBAL              4 (lxml)
+         115          68 LOAD_GLOBAL              4 (lxml)
                       80 LOAD_ATTR                3 (html)
                       90 LOAD_METHOD              4 (fromstring)
                      112 LOAD_FAST                3 (oob_content)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 STORE_FAST               4 (parsed)
          
-         105         130 LOAD_FAST                4 (parsed)
+         116         130 LOAD_FAST                4 (parsed)
                      132 LOAD_ATTR                5 (attrib)
                      142 LOAD_METHOD              6 (get)
                      164 LOAD_CONST               1 ('id')
                      166 PRECALL                  1
                      170 CALL                     1
                      180 STORE_FAST               5 (id)
          
-         106         182 LOAD_FAST                5 (id)
+         117         182 LOAD_FAST                5 (id)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 216)
          
-         107         186 LOAD_GLOBAL             15 (NULL + Exception)
+         118         186 LOAD_GLOBAL             15 (NULL + Exception)
          
-         108         198 LOAD_CONST               2 ('The additional response does not contain exactly one element with an id attribute.')
+         119         198 LOAD_CONST               2 ('The additional response does not contain exactly one element with an id attribute.')
          
-         107         200 PRECALL                  1
+         118         200 PRECALL                  1
                      204 CALL                     1
                      214 RAISE_VARARGS            1
          
-         111     >>  216 LOAD_FAST                2 (hx_swap_oob_method)
+         122     >>  216 LOAD_FAST                2 (hx_swap_oob_method)
                      218 FORMAT_VALUE             0
                      220 LOAD_CONST               3 (':#')
                      222 LOAD_FAST                5 (id)
                      224 FORMAT_VALUE             0
                      226 BUILD_STRING             3
                      228 LOAD_FAST                4 (parsed)
                      230 LOAD_ATTR                5 (attrib)
                      240 LOAD_CONST               4 ('hx-swap-oob')
                      242 STORE_SUBSCR
          
-         112         246 LOAD_FAST                0 (response)
+         123         246 LOAD_FAST                0 (response)
                      248 COPY                     1
                      250 LOAD_ATTR                8 (content)
                      260 LOAD_GLOBAL              4 (lxml)
                      272 LOAD_ATTR                3 (html)
                      282 LOAD_METHOD              9 (tostring)
                      304 LOAD_FAST                4 (parsed)
                      306 PRECALL                  1
                      310 CALL                     1
                      320 BINARY_OP               13 (+=)
                      324 SWAP                     2
                      326 STORE_ATTR               8 (content)
          
-         113         336 LOAD_FAST                0 (response)
+         124         336 LOAD_FAST                0 (response)
                      338 RETURN_VALUE
          consts
             None
             'id'
             'The additional response does not contain exactly one element with an id attribute.'
             ':#'
             'hx-swap-oob'
          names      ('response_to_str', 'strip', 'lxml', 'html', 'fromstring', 'attrib', 'get', 'Exception', 'content', 'tostring')
          varnames   ('response', 'additional', 'hx_swap_oob_method', 'oob_content', 'parsed', 'id')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'swap_oob'
-         firstlineno 100
+         firstlineno 111
          lnotab 0x020342013e01340104010c0102ff10041e015a01
       ('auto_param', 'auto_form')
       'auto_param'
       ('get', 'post')
       'auto_form'
       code
          argcount  : 0
@@ -1236,17 +1284,17 @@
             000000740400000000000000000000660219000000000000000000640274
             000000000000000000000074020000000000000000000074040000000000
             000000000066021900000000000000000066048801880066026403840c7d
             027c025300
                        0 MAKE_CELL                0 (auto_param)
                        2 MAKE_CELL                1 (auto_form)
          
-         121           4 RESUME                   0
+         132           4 RESUME                   0
          
-         126           6 LOAD_CONST               1 ('fn')
+         137           6 LOAD_CONST               1 ('fn')
                        8 LOAD_GLOBAL              0 (Callable)
                       20 LOAD_GLOBAL              2 (P)
                       32 LOAD_GLOBAL              4 (R)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('return')
                       58 LOAD_GLOBAL              0 (Callable)
@@ -1254,19 +1302,19 @@
                       82 LOAD_GLOBAL              4 (R)
                       94 BUILD_TUPLE              2
                       96 BINARY_SUBSCR
                      106 BUILD_TUPLE              4
                      108 LOAD_CLOSURE             1 (auto_form)
                      110 LOAD_CLOSURE             0 (auto_param)
                      112 BUILD_TUPLE              2
-                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 126>)
+                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 137>)
                      116 MAKE_FUNCTION           12 (annotations, closure)
                      118 STORE_FAST               2 (decorator)
          
-         149         120 LOAD_FAST                2 (decorator)
+         160         120 LOAD_FAST                2 (decorator)
                      122 RETURN_VALUE
          consts
             None
             'fn'
             'return'
             code
                argcount  : 1
@@ -1286,86 +1334,86 @@
                   1600000000000000000000660688038800880466036405840ca6000000ab
                   0000000000000000007d027c025300
                              0 COPY_FREE_VARS           2
                              2 MAKE_CELL                0 (fn)
                              4 MAKE_CELL                3 (arg_names)
                              6 MAKE_CELL                4 (injected_params)
                
-               126           8 RESUME                   0
+               137           8 RESUME                   0
                
-               127          10 LOAD_GLOBAL              1 (NULL + list)
+               138          10 LOAD_GLOBAL              1 (NULL + list)
                
-               128          22 LOAD_GLOBAL              3 (NULL + inspect)
+               139          22 LOAD_GLOBAL              3 (NULL + inspect)
                             34 LOAD_ATTR                2 (signature)
                             44 LOAD_DEREF               0 (fn)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 LOAD_ATTR                3 (parameters)
                             70 LOAD_METHOD              4 (values)
                             92 PRECALL                  0
                             96 CALL                     0
                
-               127         106 PRECALL                  1
+               138         106 PRECALL                  1
                            110 CALL                     1
                            120 STORE_FAST               1 (parameters)
                
-               130         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
+               141         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
                            134 LOAD_FAST                1 (parameters)
                            136 LOAD_DEREF               6 (auto_param)
                            138 LOAD_DEREF               5 (auto_form)
                            140 PRECALL                  3
                            144 CALL                     3
                            154 STORE_DEREF              4 (injected_params)
                
-               131         156 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 131>)
+               142         156 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 142>)
                            158 MAKE_FUNCTION            0
                            160 LOAD_FAST                1 (parameters)
                            162 GET_ITER
                            164 PRECALL                  0
                            168 CALL                     0
                            178 STORE_DEREF              3 (arg_names)
                
-               133         180 LOAD_GLOBAL             13 (NULL + functools)
+               144         180 LOAD_GLOBAL             13 (NULL + functools)
                            192 LOAD_ATTR                7 (wraps)
                            202 LOAD_DEREF               0 (fn)
                            204 PRECALL                  1
                            208 CALL                     1
                
-               134         218 LOAD_CONST               2 ('args')
+               145         218 LOAD_CONST               2 ('args')
                            220 LOAD_GLOBAL             16 (P)
                            232 LOAD_ATTR                9 (args)
                            242 LOAD_CONST               3 ('kwargs')
                            244 LOAD_GLOBAL             16 (P)
                            256 LOAD_ATTR               10 (kwargs)
                            266 LOAD_CONST               4 ('return')
                            268 LOAD_GLOBAL             22 (R)
                            280 BUILD_TUPLE              6
                            282 LOAD_CLOSURE             3 (arg_names)
                            284 LOAD_CLOSURE             0 (fn)
                            286 LOAD_CLOSURE             4 (injected_params)
                            288 BUILD_TUPLE              3
-                           290 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 133>)
+                           290 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 144>)
                            292 MAKE_FUNCTION           12 (annotations, closure)
                
-               133         294 PRECALL                  0
+               144         294 PRECALL                  0
                            298 CALL                     0
                
-               134         308 STORE_FAST               2 (inner)
+               145         308 STORE_FAST               2 (inner)
                
-               147         310 LOAD_FAST                2 (inner)
+               158         310 LOAD_FAST                2 (inner)
                            312 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     131           0 RESUME                   0
+                     142           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (p)
                                   10 LOAD_FAST                1 (p)
                                   12 LOAD_ATTR                0 (name)
                                   22 LIST_APPEND              2
@@ -1374,15 +1422,15 @@
                      consts
                      names      ('name',)
                      varnames   ('.0', 'p')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<listcomp>'
-                     firstlineno 131
+                     firstlineno 142
                      lnotab 0x
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
                      nlocals   : 6
@@ -1400,90 +1448,90 @@
                         020000ab020000000000000000a6010000ab0100000000000000007c017c
                         0319000000000000000000a6020000ab0200000000000000007d057c0581
                         1c740b000000000000000000006a06000000000000000074100000000000
                         00000000007c05a6020000ab0200000000000000006302010053008c8602
                         0089077c0069007c01a4018e015300
                                    0 COPY_FREE_VARS           3
                      
-                     133           2 RESUME                   0
+                     144           2 RESUME                   0
                      
-                     135           4 LOAD_DEREF               6 (arg_names)
+                     146           4 LOAD_DEREF               6 (arg_names)
                                    6 LOAD_CONST               0 (None)
                                    8 LOAD_GLOBAL              1 (NULL + len)
                                   20 LOAD_FAST                0 (args)
                                   22 PRECALL                  1
                                   26 CALL                     1
                                   36 BUILD_SLICE              2
                                   38 BINARY_SUBSCR
                                   48 STORE_FAST               2 (supplied_args)
                      
-                     136          50 LOAD_DEREF               8 (injected_params)
+                     147          50 LOAD_DEREF               8 (injected_params)
                                   52 LOAD_METHOD              1 (items)
                                   74 PRECALL                  0
                                   78 CALL                     0
                                   88 GET_ITER
                              >>   90 FOR_ITER               133 (to 358)
                                   92 UNPACK_SEQUENCE          2
                                   96 STORE_FAST               3 (name)
                                   98 STORE_FAST               4 (ip)
                      
-                     137         100 LOAD_FAST                3 (name)
+                     148         100 LOAD_FAST                3 (name)
                                  102 LOAD_FAST                1 (kwargs)
                                  104 CONTAINS_OP              1
                                  106 POP_JUMP_FORWARD_IF_FALSE   124 (to 356)
                                  108 LOAD_FAST                3 (name)
                                  110 LOAD_FAST                2 (supplied_args)
                                  112 CONTAINS_OP              1
                                  114 POP_JUMP_FORWARD_IF_FALSE   120 (to 356)
                      
-                     138         116 LOAD_FAST                4 (ip)
+                     149         116 LOAD_FAST                4 (ip)
                                  118 LOAD_METHOD              2 (get_value)
                                  140 LOAD_FAST                0 (args)
                                  142 LOAD_FAST                1 (kwargs)
                                  144 PRECALL                  2
                                  148 CALL                     2
                                  158 LOAD_FAST                1 (kwargs)
                                  160 LOAD_FAST                3 (name)
                                  162 STORE_SUBSCR
                      
-                     139         166 LOAD_FAST                4 (ip)
+                     150         166 LOAD_FAST                4 (ip)
                                  168 LOAD_METHOD              3 (replace_response)
                      
-                     140         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
+                     151         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
                                  202 LOAD_GLOBAL             11 (NULL + typing)
                                  214 LOAD_ATTR                6 (cast)
                                  224 LOAD_GLOBAL             14 (Any)
                                  236 LOAD_FAST                0 (args)
                                  238 PRECALL                  2
                                  242 CALL                     2
                                  252 PRECALL                  1
                                  256 CALL                     1
                                  266 LOAD_FAST                1 (kwargs)
                                  268 LOAD_FAST                3 (name)
                                  270 BINARY_SUBSCR
                      
-                     139         280 PRECALL                  2
+                     150         280 PRECALL                  2
                                  284 CALL                     2
                                  294 STORE_FAST               5 (replace_response)
                      
-                     142         296 LOAD_FAST                5 (replace_response)
+                     153         296 LOAD_FAST                5 (replace_response)
                                  298 POP_JUMP_FORWARD_IF_NONE    28 (to 356)
                      
-                     143         300 LOAD_GLOBAL             11 (NULL + typing)
+                     154         300 LOAD_GLOBAL             11 (NULL + typing)
                                  312 LOAD_ATTR                6 (cast)
                                  322 LOAD_GLOBAL             16 (R)
                                  334 LOAD_FAST                5 (replace_response)
                                  336 PRECALL                  2
                                  340 CALL                     2
                                  350 SWAP                     2
                                  352 POP_TOP
                                  354 RETURN_VALUE
                              >>  356 JUMP_BACKWARD          134 (to 90)
                      
-                     145     >>  358 PUSH_NULL
+                     156     >>  358 PUSH_NULL
                                  360 LOAD_DEREF               7 (fn)
                                  362 LOAD_FAST                0 (args)
                                  364 BUILD_MAP                0
                                  366 LOAD_FAST                1 (kwargs)
                                  368 DICT_MERGE               1
                                  370 CALL_FUNCTION_EX         1
                                  372 RETURN_VALUE
@@ -1491,112 +1539,112 @@
                         None
                      names      ('len', 'items', 'get_value', 'replace_response', '_get_request_from_args', 'typing', 'cast', 'Any', 'R')
                      varnames   ('args', 'kwargs', 'supplied_args', 'name', 'ip', 'replace_response')
                      freevars   ('arg_names', 'fn', 'injected_params')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 133
+                     firstlineno 144
                      lnotab 0x04022e0132011001320118015aff100304013a02
                names      ('list', 'inspect', 'signature', 'parameters', 'values', '_extract_injected_params', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
                varnames   ('fn', 'parameters', 'inner')
                freevars   ('auto_form', 'auto_param')
                cellvars   ('fn', 'arg_names', 'injected_params')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 126
+               firstlineno 137
                lnotab 0x0a010c0154ff10032201180226014cff0e01020d
          names      ('Callable', 'P', 'R')
          varnames   ('auto_param', 'auto_form', 'decorator')
          freevars   ()
          cellvars   ('auto_param', 'auto_form')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'inject_args'
-         firstlineno 121
+         firstlineno 132
          lnotab 0x06057217
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a025500020065036a0400000000000000006401ac
             02a6010000ab0100000000000000005a056506650764033c000000020065
             036a0400000000000000006401ac02a6010000ab0100000000000000005a
             086509650764043c000000640584005a0a6406650b6407650c6506650b66
             02190000000000000000006408650b6606640984045a0d640a650e640b65
             0b6408650f6510190000000000000000006606640c84045a11640d5300
-         156           0 RESUME                   0
+         167           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParam')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         158          12 PUSH_NULL
+         169          12 PUSH_NULL
                       14 LOAD_NAME                3 (dataclasses)
                       16 LOAD_ATTR                4 (field)
                       26 LOAD_CONST               1 (False)
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (name)
                       46 LOAD_NAME                6 (str)
                       48 LOAD_NAME                7 (__annotations__)
                       50 LOAD_CONST               3 ('name')
                       52 STORE_SUBSCR
          
-         159          56 PUSH_NULL
+         170          56 PUSH_NULL
                       58 LOAD_NAME                3 (dataclasses)
                       60 LOAD_ATTR                4 (field)
                       70 LOAD_CONST               1 (False)
                       72 KW_NAMES                 2
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME               8 (target_type)
                       90 LOAD_NAME                9 (type)
                       92 LOAD_NAME                7 (__annotations__)
                       94 LOAD_CONST               4 ('target_type')
                       96 STORE_SUBSCR
          
-         161         100 LOAD_CONST               5 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 161>)
+         172         100 LOAD_CONST               5 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 172>)
                      102 MAKE_FUNCTION            0
                      104 STORE_NAME              10 (check)
          
-         164         106 LOAD_CONST               6 ('args')
+         175         106 LOAD_CONST               6 ('args')
                      108 LOAD_NAME               11 (Any)
                      110 LOAD_CONST               7 ('kwargs')
                      112 LOAD_NAME               12 (dict)
                      114 LOAD_NAME                6 (str)
                      116 LOAD_NAME               11 (Any)
                      118 BUILD_TUPLE              2
                      120 BINARY_SUBSCR
                      130 LOAD_CONST               8 ('return')
                      132 LOAD_NAME               11 (Any)
                      134 BUILD_TUPLE              6
-                     136 LOAD_CONST               9 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 164>)
+                     136 LOAD_CONST               9 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 175>)
                      138 MAKE_FUNCTION            4 (annotations)
                      140 STORE_NAME              13 (get_value)
          
-         167         142 LOAD_CONST              10 ('request')
+         178         142 LOAD_CONST              10 ('request')
          
-         168         144 LOAD_NAME               14 (HttpRequest)
+         179         144 LOAD_NAME               14 (HttpRequest)
          
-         167         146 LOAD_CONST              11 ('value')
+         178         146 LOAD_CONST              11 ('value')
          
-         168         148 LOAD_NAME               11 (Any)
+         179         148 LOAD_NAME               11 (Any)
          
-         167         150 LOAD_CONST               8 ('return')
+         178         150 LOAD_CONST               8 ('return')
          
-         169         152 LOAD_NAME               15 (Optional)
+         180         152 LOAD_NAME               15 (Optional)
                      154 LOAD_NAME               16 (HttpResponse)
                      156 BINARY_SUBSCR
          
-         167         166 BUILD_TUPLE              6
-                     168 LOAD_CONST              12 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 167>)
+         178         166 BUILD_TUPLE              6
+                     168 LOAD_CONST              12 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 178>)
                      170 MAKE_FUNCTION            4 (annotations)
                      172 STORE_NAME              17 (replace_response)
                      174 LOAD_CONST              13 (None)
                      176 RETURN_VALUE
          consts
             'InjectedParam'
             False
@@ -1605,81 +1653,81 @@
             'target_type'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               161           0 RESUME                   0
+               172           0 RESUME                   0
                
-               162           2 LOAD_CONST               0 (None)
+               173           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 161
+               firstlineno 172
                lnotab 0x0201
             'args'
             'kwargs'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               164           0 RESUME                   0
+               175           0 RESUME                   0
                
-               165           2 LOAD_CONST               0 (None)
+               176           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 164
+               firstlineno 175
                lnotab 0x0201
             'request'
             'value'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               167           0 RESUME                   0
+               178           0 RESUME                   0
                
-               170           2 LOAD_CONST               0 (None)
+               181           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'request', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 167
+               firstlineno 178
                lnotab 0x0203
             None
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'name', 'str', '__annotations__', 'target_type', 'type', 'check', 'Any', 'dict', 'get_value', 'HttpRequest', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParam'
-         firstlineno 156
+         firstlineno 167
          lnotab 0x0c022c012c0206032403020102ff020102ff02020efe
       'InjectedParam'
       'ip'
       'name'
       'parameter'
       code
          argcount  : 3
@@ -1697,100 +1745,100 @@
             000000000000006e45740f000000000000000000007c026a050000000000
             000000741400000000000000000000a6020000ab02000000000000000072
             257c026a0500000000000000006a05000000000000000081197413000000
             000000000000007c026a0500000000000000006a050000000000000000a6
             010000ab0100000000000000006e067416000000000000000000007c005f
             0c00000000000000007c00a00d0000000000000000000000000000000000
             000000a6000000ab00000000000000000001007c005300
-         173           0 RESUME                   0
+         184           0 RESUME                   0
          
-         174           2 LOAD_FAST                1 (name)
+         185           2 LOAD_FAST                1 (name)
                        4 LOAD_FAST                0 (ip)
                        6 STORE_ATTR               0 (name)
          
-         177          16 LOAD_FAST                2 (parameter)
+         188          16 LOAD_FAST                2 (parameter)
                       18 LOAD_ATTR                1 (annotation)
                       28 LOAD_GLOBAL              4 (inspect)
                       40 LOAD_ATTR                3 (Signature)
                       50 LOAD_ATTR                4 (empty)
                       60 IS_OP                    1
                       62 POP_JUMP_FORWARD_IF_FALSE     7 (to 78)
          
-         176          64 LOAD_FAST                2 (parameter)
+         187          64 LOAD_FAST                2 (parameter)
                       66 LOAD_ATTR                1 (annotation)
                       76 JUMP_FORWARD           139 (to 356)
          
-         179     >>   78 LOAD_FAST                2 (parameter)
+         190     >>   78 LOAD_FAST                2 (parameter)
                       80 LOAD_ATTR                5 (default)
                       90 LOAD_GLOBAL              4 (inspect)
                      102 LOAD_ATTR                6 (Parameter)
                      112 LOAD_ATTR                4 (empty)
                      122 IS_OP                    1
                      124 POP_JUMP_FORWARD_IF_FALSE    46 (to 218)
          
-         180         126 LOAD_GLOBAL             15 (NULL + isinstance)
+         191         126 LOAD_GLOBAL             15 (NULL + isinstance)
                      138 LOAD_FAST                2 (parameter)
                      140 LOAD_ATTR                5 (default)
                      150 LOAD_GLOBAL             16 (InjectedParam)
                      162 PRECALL                  2
                      166 CALL                     2
          
-         179         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
+         190         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
          
-         178         178 LOAD_GLOBAL             19 (NULL + type)
+         189         178 LOAD_GLOBAL             19 (NULL + type)
                      190 LOAD_FAST                2 (parameter)
                      192 LOAD_ATTR                5 (default)
                      202 PRECALL                  1
                      206 CALL                     1
                      216 JUMP_FORWARD            69 (to 356)
          
-         182     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
+         193     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
                      230 LOAD_FAST                2 (parameter)
                      232 LOAD_ATTR                5 (default)
                      242 LOAD_GLOBAL             20 (InjectedParamQuery)
                      254 PRECALL                  2
                      258 CALL                     2
          
-         181         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
+         192         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
          
-         183         270 LOAD_FAST                2 (parameter)
+         194         270 LOAD_FAST                2 (parameter)
                      272 LOAD_ATTR                5 (default)
                      282 LOAD_ATTR                5 (default)
                      292 POP_JUMP_FORWARD_IF_NONE    25 (to 344)
          
-         181         294 LOAD_GLOBAL             19 (NULL + type)
+         192         294 LOAD_GLOBAL             19 (NULL + type)
                      306 LOAD_FAST                2 (parameter)
                      308 LOAD_ATTR                5 (default)
                      318 LOAD_ATTR                5 (default)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 JUMP_FORWARD             6 (to 356)
          
-         184     >>  344 LOAD_GLOBAL             22 (str)
+         195     >>  344 LOAD_GLOBAL             22 (str)
          
-         175     >>  356 LOAD_FAST                0 (ip)
+         186     >>  356 LOAD_FAST                0 (ip)
                      358 STORE_ATTR              12 (target_type)
          
-         186         368 LOAD_FAST                0 (ip)
+         197         368 LOAD_FAST                0 (ip)
                      370 LOAD_METHOD             13 (check)
                      392 PRECALL                  0
                      396 CALL                     0
                      406 POP_TOP
          
-         187         408 LOAD_FAST                0 (ip)
+         198         408 LOAD_FAST                0 (ip)
                      410 RETURN_VALUE
          consts
             None
          names      ('name', 'annotation', 'inspect', 'Signature', 'empty', 'default', 'Parameter', 'isinstance', 'InjectedParam', 'type', 'InjectedParamQuery', 'str', 'target_type', 'check')
          varnames   ('ip', 'name', 'parameter')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_setup_injected_param'
-         firstlineno 173
+         firstlineno 184
          lnotab
             0x02010e0330ff0e03300132ff02ff280432ff020218fe32030cf70c0b28
             01
       'parameters'
       'get'
       'post'
       code
@@ -1822,202 +1870,202 @@
             00000000007421000000000000000000007c07ac06a6010000ab01000000
             00000000007c056a0400000000000000007c05a6030000ab030000000000
             0000007c037c056a0400000000000000003c00000090018c457c0164086b
             0200000000722c7407000000000000000000007423000000000000000000
             007c07ac06a6010000ab0100000000000000007c056a0400000000000000
             007c05a6030000ab0300000000000000007c037c056a0400000000000000
             003c00000090018c797c035300
-         190           0 RESUME                   0
+         201           0 RESUME                   0
          
-         198           2 BUILD_MAP                0
+         209           2 BUILD_MAP                0
                        4 STORE_FAST               3 (result)
          
-         201           6 LOAD_FAST                0 (parameters)
+         212           6 LOAD_FAST                0 (parameters)
                        8 LOAD_CONST               1 (1)
                       10 LOAD_CONST               2 (None)
                       12 BUILD_SLICE              2
                       14 BINARY_SUBSCR
                       24 STORE_FAST               0 (parameters)
          
-         203          26 LOAD_CONST               3 (False)
+         214          26 LOAD_CONST               3 (False)
                       28 STORE_FAST               4 (found_form_arg)
          
-         204          30 LOAD_FAST                0 (parameters)
+         215          30 LOAD_FAST                0 (parameters)
                       32 GET_ITER
                  >>   34 EXTENDED_ARG             1
                       36 FOR_ITER               375 (to 788)
                       38 STORE_FAST               5 (arg)
          
-         205          40 LOAD_GLOBAL              1 (NULL + isinstance)
+         216          40 LOAD_GLOBAL              1 (NULL + isinstance)
                       52 LOAD_FAST                5 (arg)
                       54 LOAD_ATTR                1 (default)
                       64 LOAD_GLOBAL              4 (InjectedParam)
                       76 PRECALL                  2
                       80 CALL                     2
                       90 POP_JUMP_FORWARD_IF_FALSE    38 (to 168)
          
-         206          92 LOAD_FAST                5 (arg)
+         217          92 LOAD_FAST                5 (arg)
                       94 LOAD_ATTR                1 (default)
                      104 STORE_FAST               6 (ip)
          
-         207         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         218         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
                      118 LOAD_FAST                6 (ip)
                      120 LOAD_FAST                5 (arg)
                      122 LOAD_ATTR                4 (name)
                      132 LOAD_FAST                5 (arg)
                      134 PRECALL                  3
                      138 CALL                     3
                      148 LOAD_FAST                3 (result)
                      150 LOAD_FAST                6 (ip)
                      152 LOAD_ATTR                4 (name)
                      162 STORE_SUBSCR
                      166 JUMP_BACKWARD           67 (to 34)
          
-         212     >>  168 LOAD_FAST                5 (arg)
+         223     >>  168 LOAD_FAST                5 (arg)
                      170 LOAD_ATTR                1 (default)
                      180 LOAD_GLOBAL             10 (inspect)
                      192 LOAD_ATTR                6 (Parameter)
                      202 LOAD_ATTR                7 (empty)
                      212 COMPARE_OP               3 (!=)
                      218 POP_JUMP_FORWARD_IF_FALSE     7 (to 234)
                      220 LOAD_FAST                5 (arg)
                      222 LOAD_ATTR                1 (default)
                      232 JUMP_FORWARD             1 (to 236)
                  >>  234 LOAD_CONST               2 (None)
          
-         211     >>  236 STORE_FAST               7 (default_value)
+         222     >>  236 STORE_FAST               7 (default_value)
          
-         216         238 LOAD_FAST                2 (auto_form)
+         227         238 LOAD_FAST                2 (auto_form)
          
-         215         240 POP_JUMP_FORWARD_IF_FALSE   119 (to 480)
+         226         240 POP_JUMP_FORWARD_IF_FALSE   119 (to 480)
          
-         217         242 LOAD_GLOBAL              1 (NULL + isinstance)
+         228         242 LOAD_GLOBAL              1 (NULL + isinstance)
                      254 LOAD_FAST                5 (arg)
                      256 LOAD_ATTR                8 (annotation)
                      266 LOAD_GLOBAL             18 (type)
                      278 PRECALL                  2
                      282 CALL                     2
          
-         215         292 POP_JUMP_FORWARD_IF_FALSE    93 (to 480)
+         226         292 POP_JUMP_FORWARD_IF_FALSE    93 (to 480)
          
-         218         294 LOAD_GLOBAL             21 (NULL + issubclass)
+         229         294 LOAD_GLOBAL             21 (NULL + issubclass)
                      306 LOAD_FAST                5 (arg)
                      308 LOAD_ATTR                8 (annotation)
                      318 LOAD_GLOBAL             22 (forms)
                      330 LOAD_ATTR               12 (BaseForm)
                      340 PRECALL                  2
                      344 CALL                     2
          
-         215         354 POP_JUMP_FORWARD_IF_FALSE    62 (to 480)
+         226         354 POP_JUMP_FORWARD_IF_FALSE    62 (to 480)
          
-         220         356 LOAD_FAST                4 (found_form_arg)
+         231         356 LOAD_FAST                4 (found_form_arg)
                      358 POP_JUMP_FORWARD_IF_FALSE    15 (to 390)
          
-         221         360 LOAD_GLOBAL             27 (NULL + Exception)
+         232         360 LOAD_GLOBAL             27 (NULL + Exception)
          
-         222         372 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
+         233         372 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
          
-         221         374 PRECALL                  1
+         232         374 PRECALL                  1
                      378 CALL                     1
                      388 RAISE_VARARGS            1
          
-         224     >>  390 LOAD_CONST               5 (True)
+         235     >>  390 LOAD_CONST               5 (True)
                      392 STORE_FAST               4 (found_form_arg)
          
-         225         394 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         236         394 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
                      406 LOAD_GLOBAL             29 (NULL + handle_form)
                      418 PRECALL                  0
                      422 CALL                     0
                      432 LOAD_FAST                5 (arg)
                      434 LOAD_ATTR                4 (name)
                      444 LOAD_FAST                5 (arg)
                      446 PRECALL                  3
                      450 CALL                     3
                      460 LOAD_FAST                3 (result)
                      462 LOAD_FAST                5 (arg)
                      464 LOAD_ATTR                4 (name)
                      474 STORE_SUBSCR
                      478 JUMP_BACKWARD          223 (to 34)
          
-         227     >>  480 LOAD_FAST                1 (auto_param)
+         238     >>  480 LOAD_FAST                1 (auto_param)
                      482 LOAD_CONST               5 (True)
                      484 IS_OP                    0
                      486 POP_JUMP_FORWARD_IF_FALSE    46 (to 580)
          
-         228         488 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         239         488 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         229         500 LOAD_GLOBAL             31 (NULL + InjectedParamQuery)
+         240         500 LOAD_GLOBAL             31 (NULL + InjectedParamQuery)
                      512 LOAD_FAST                7 (default_value)
                      514 KW_NAMES                 6
                      516 PRECALL                  1
                      520 CALL                     1
                      530 LOAD_FAST                5 (arg)
                      532 LOAD_ATTR                4 (name)
                      542 LOAD_FAST                5 (arg)
          
-         228         544 PRECALL                  3
+         239         544 PRECALL                  3
                      548 CALL                     3
                      558 LOAD_FAST                3 (result)
                      560 LOAD_FAST                5 (arg)
                      562 LOAD_ATTR                4 (name)
                      572 STORE_SUBSCR
                      576 EXTENDED_ARG             1
                      578 JUMP_BACKWARD          273 (to 34)
          
-         231     >>  580 LOAD_FAST                1 (auto_param)
+         242     >>  580 LOAD_FAST                1 (auto_param)
                      582 LOAD_CONST               7 ('get')
                      584 COMPARE_OP               2 (==)
                      590 POP_JUMP_FORWARD_IF_FALSE    46 (to 684)
          
-         232         592 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         243         592 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         233         604 LOAD_GLOBAL             33 (NULL + InjectedParamQueryGet)
+         244         604 LOAD_GLOBAL             33 (NULL + InjectedParamQueryGet)
                      616 LOAD_FAST                7 (default_value)
                      618 KW_NAMES                 6
                      620 PRECALL                  1
                      624 CALL                     1
                      634 LOAD_FAST                5 (arg)
                      636 LOAD_ATTR                4 (name)
                      646 LOAD_FAST                5 (arg)
          
-         232         648 PRECALL                  3
+         243         648 PRECALL                  3
                      652 CALL                     3
                      662 LOAD_FAST                3 (result)
                      664 LOAD_FAST                5 (arg)
                      666 LOAD_ATTR                4 (name)
                      676 STORE_SUBSCR
                      680 EXTENDED_ARG             1
                      682 JUMP_BACKWARD          325 (to 34)
          
-         235     >>  684 LOAD_FAST                1 (auto_param)
+         246     >>  684 LOAD_FAST                1 (auto_param)
                      686 LOAD_CONST               8 ('post')
                      688 COMPARE_OP               2 (==)
                      694 POP_JUMP_FORWARD_IF_FALSE    44 (to 784)
          
-         236         696 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         247         696 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         237         708 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
+         248         708 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
                      720 LOAD_FAST                7 (default_value)
                      722 KW_NAMES                 6
                      724 PRECALL                  1
                      728 CALL                     1
                      738 LOAD_FAST                5 (arg)
                      740 LOAD_ATTR                4 (name)
                      750 LOAD_FAST                5 (arg)
          
-         236         752 PRECALL                  3
+         247         752 PRECALL                  3
                      756 CALL                     3
                      766 LOAD_FAST                3 (result)
                      768 LOAD_FAST                5 (arg)
                      770 LOAD_ATTR                4 (name)
                      780 STORE_SUBSCR
                  >>  784 EXTENDED_ARG             1
                      786 JUMP_BACKWARD          377 (to 34)
          
-         240     >>  788 LOAD_FAST                3 (result)
+         251     >>  788 LOAD_FAST                3 (result)
                      790 RETURN_VALUE
          consts
             '\n    Extracts all injected parameters from the given list of function arguments.\n    '
             1
             None
             False
             'You can only have one Form argument in a view function.'
@@ -2027,42 +2075,42 @@
             'post'
          names      ('isinstance', 'default', 'InjectedParam', '_setup_injected_param', 'name', 'inspect', 'Parameter', 'empty', 'annotation', 'type', 'issubclass', 'forms', 'BaseForm', 'Exception', 'handle_form', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost')
          varnames   ('parameters', 'auto_param', 'auto_form', 'result', 'found_form_arg', 'arg', 'ip', 'default_value')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_extract_injected_params'
-         firstlineno 190
+         firstlineno 201
          lnotab
             0x02080403140204010a0134010e013e0544ff020502ff020232fe02033c
             fd020504010c0102ff10030401560208010c012cff24030c010c012cff24
             030c010c012cff2404
       'args'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006401190000000000000000005300
-         243           0 RESUME                   0
+         254           0 RESUME                   0
          
-         244           2 LOAD_FAST                0 (args)
+         255           2 LOAD_FAST                0 (args)
                        4 LOAD_CONST               1 (0)
                        6 BINARY_SUBSCR
                       16 RETURN_VALUE
          consts
             None
             0
          names      ()
          varnames   ('args',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_get_request_from_args'
-         firstlineno 243
+         firstlineno 254
          lnotab 0x0201
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
@@ -2070,90 +2118,90 @@
             02a6010000ab0100000000000000005a0565066507190000000000000000
             00650864033c000000020065036a0400000000000000006401ac02a60100
             00ab0100000000000000005a09650a650864043c000000020065036a0400
             000000000000006405ac02a6010000ab0100000000000000005a0b650c65
             0864063c000000640784005a0d6408650e6602640984045a0f6408650e66
             02640a84045a10640b650a640c65116507650a6602190000000000000000
             006604640d84045a1264015300
-         252           0 RESUME                   0
+         263           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQuery')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         254          12 PUSH_NULL
+         265          12 PUSH_NULL
                       14 LOAD_NAME                3 (dataclasses)
                       16 LOAD_ATTR                4 (field)
                       26 LOAD_CONST               1 (None)
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (query_param_name)
                       46 LOAD_NAME                6 (Optional)
                       48 LOAD_NAME                7 (str)
                       50 BINARY_SUBSCR
                       60 LOAD_NAME                8 (__annotations__)
                       62 LOAD_CONST               3 ('query_param_name')
                       64 STORE_SUBSCR
          
-         255          68 PUSH_NULL
+         266          68 PUSH_NULL
                       70 LOAD_NAME                3 (dataclasses)
                       72 LOAD_ATTR                4 (field)
                       82 LOAD_CONST               1 (None)
                       84 KW_NAMES                 2
                       86 PRECALL                  1
                       90 CALL                     1
                      100 STORE_NAME               9 (default)
                      102 LOAD_NAME               10 (Any)
                      104 LOAD_NAME                8 (__annotations__)
                      106 LOAD_CONST               4 ('default')
                      108 STORE_SUBSCR
          
-         256         112 PUSH_NULL
+         267         112 PUSH_NULL
                      114 LOAD_NAME                3 (dataclasses)
                      116 LOAD_ATTR                4 (field)
                      126 LOAD_CONST               5 (True)
                      128 KW_NAMES                 2
                      130 PRECALL                  1
                      134 CALL                     1
                      144 STORE_NAME              11 (consume)
                      146 LOAD_NAME               12 (bool)
                      148 LOAD_NAME                8 (__annotations__)
                      150 LOAD_CONST               6 ('consume')
                      152 STORE_SUBSCR
          
-         258         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 258>)
+         269         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 269>)
                      158 MAKE_FUNCTION            0
                      160 STORE_NAME              13 (check)
          
-         262         162 LOAD_CONST               8 ('request')
+         273         162 LOAD_CONST               8 ('request')
                      164 LOAD_NAME               14 (HttpRequest)
                      166 BUILD_TUPLE              2
-                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 262>)
+                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 273>)
                      170 MAKE_FUNCTION            4 (annotations)
                      172 STORE_NAME              15 (_create_lookup_dict)
          
-         269         174 LOAD_CONST               8 ('request')
+         280         174 LOAD_CONST               8 ('request')
                      176 LOAD_NAME               14 (HttpRequest)
                      178 BUILD_TUPLE              2
-                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 269>)
+                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 280>)
                      182 MAKE_FUNCTION            4 (annotations)
                      184 STORE_NAME              16 (_consume_param)
          
-         279         186 LOAD_CONST              11 ('args')
+         290         186 LOAD_CONST              11 ('args')
                      188 LOAD_NAME               10 (Any)
                      190 LOAD_CONST              12 ('kwargs')
                      192 LOAD_NAME               17 (dict)
                      194 LOAD_NAME                7 (str)
                      196 LOAD_NAME               10 (Any)
                      198 BUILD_TUPLE              2
                      200 BINARY_SUBSCR
                      210 BUILD_TUPLE              4
-                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 279>)
+                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 290>)
                      214 MAKE_FUNCTION            4 (annotations)
                      216 STORE_NAME              18 (get_value)
                      218 LOAD_CONST               1 (None)
                      220 RETURN_VALUE
          consts
             'InjectedParamQuery'
             None
@@ -2166,38 +2214,38 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000800e7c006a0100000000000000007c
                   005f0000000000000000006400530064005300
-               258           0 RESUME                   0
+               269           0 RESUME                   0
                
-               259           2 LOAD_FAST                0 (self)
+               270           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 44)
                
-               260          16 LOAD_FAST                0 (self)
+               271          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (name)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               0 (query_param_name)
                             40 LOAD_CONST               0 (None)
                             42 RETURN_VALUE
                
-               259     >>   44 LOAD_CONST               0 (None)
+               270     >>   44 LOAD_CONST               0 (None)
                             46 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 258
+               firstlineno 269
                lnotab 0x02010e011cff
             'request'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -2208,55 +2256,55 @@
                   00000000007d027401000000000000000000006a01000000000000000074
                   04000000000000000000007c016a040000000000000000a6020000ab0200
                   000000000000008a05880566016402840889054400a6000000ab00000000
                   00000000007d037c037c027a0700005300
                              0 MAKE_CELL                4 (getqd)
                              2 MAKE_CELL                5 (postqd)
                
-               262           4 RESUME                   0
+               273           4 RESUME                   0
                
-               263           6 LOAD_GLOBAL              1 (NULL + typing)
+               274           6 LOAD_GLOBAL              1 (NULL + typing)
                             18 LOAD_ATTR                1 (cast)
                             28 LOAD_GLOBAL              4 (QueryDict)
                             40 LOAD_FAST                1 (request)
                             42 LOAD_ATTR                3 (GET)
                             52 PRECALL                  2
                             56 CALL                     2
                             66 STORE_DEREF              4 (getqd)
                
-               264          68 LOAD_CLOSURE             4 (getqd)
+               275          68 LOAD_CLOSURE             4 (getqd)
                             70 BUILD_TUPLE              1
-                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 264>)
+                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 275>)
                             74 MAKE_FUNCTION            8 (closure)
                             76 LOAD_DEREF               4 (getqd)
                             78 GET_ITER
                             80 PRECALL                  0
                             84 CALL                     0
                             94 STORE_FAST               2 (getd)
                
-               265          96 LOAD_GLOBAL              1 (NULL + typing)
+               276          96 LOAD_GLOBAL              1 (NULL + typing)
                            108 LOAD_ATTR                1 (cast)
                            118 LOAD_GLOBAL              4 (QueryDict)
                            130 LOAD_FAST                1 (request)
                            132 LOAD_ATTR                4 (POST)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_DEREF              5 (postqd)
                
-               266         158 LOAD_CLOSURE             5 (postqd)
+               277         158 LOAD_CLOSURE             5 (postqd)
                            160 BUILD_TUPLE              1
-                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 266>)
+                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 277>)
                            164 MAKE_FUNCTION            8 (closure)
                            166 LOAD_DEREF               5 (postqd)
                            168 GET_ITER
                            170 PRECALL                  0
                            174 CALL                     0
                            184 STORE_FAST               3 (postd)
                
-               267         186 LOAD_FAST                3 (postd)
+               278         186 LOAD_FAST                3 (postd)
                            188 LOAD_FAST                2 (getd)
                            190 BINARY_OP                7 (|)
                            194 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
@@ -2265,15 +2313,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     264           2 RESUME                   0
+                     275           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (getqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2286,28 +2334,28 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('getqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 264
+                     firstlineno 275
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     266           2 RESUME                   0
+                     277           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (postqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2320,23 +2368,23 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('postqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 266
+                     firstlineno 277
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET', 'POST')
                varnames   ('self', 'request', 'getd', 'postd')
                freevars   ()
                cellvars   ('getqd', 'postqd')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 262
+               firstlineno 273
                lnotab 0x06013e011c013e011c01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -2346,79 +2394,79 @@
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f010000000000000000640053007c006a0000
                   000000000000007c016a0600000000000000007600723974050000000000
                   00000000007407000000000000000000006a040000000000000000740a00
                   0000000000000000007c016a060000000000000000a6020000ab02000000
                   00000000007c006a000000000000000000a6020000ab0200000000000000
                   007c015f0600000000000000006400530064005300
-               269           0 RESUME                   0
+               280           0 RESUME                   0
                
-               270           2 LOAD_FAST                0 (self)
+               281           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               271          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               282          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               272          42 LOAD_GLOBAL              7 (NULL + typing)
+               283          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               271         114 PRECALL                  2
+               282         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               274     >>  144 LOAD_FAST                0 (self)
+               285     >>  144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                0 (query_param_name)
                            156 LOAD_FAST                1 (request)
                            158 LOAD_ATTR                6 (POST)
                            168 CONTAINS_OP              0
                            170 POP_JUMP_FORWARD_IF_FALSE    57 (to 286)
                
-               275         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               286         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               276         184 LOAD_GLOBAL              7 (NULL + typing)
+               287         184 LOAD_GLOBAL              7 (NULL + typing)
                            196 LOAD_ATTR                4 (cast)
                            206 LOAD_GLOBAL             10 (Any)
                            218 LOAD_FAST                1 (request)
                            220 LOAD_ATTR                6 (POST)
                            230 PRECALL                  2
                            234 CALL                     2
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR                0 (query_param_name)
                
-               275         256 PRECALL                  2
+               286         256 PRECALL                  2
                            260 CALL                     2
                            270 LOAD_FAST                1 (request)
                            272 STORE_ATTR               6 (POST)
                            282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                
-               274     >>  286 LOAD_CONST               0 (None)
+               285     >>  286 LOAD_CONST               0 (None)
                            288 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 269
+               firstlineno 280
                lnotab 0x02011c010c0148ff1e031c010c0148ff1eff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -2433,87 +2481,87 @@
                   0000000000000000007c006a070000000000000000a6020000ab02000000
                   000000000072026400530074110000000000000000000064017c006a0300
                   000000000000009b0064029d03a6010000ab01000000000000000082017c
                   006a09000000000000000072157c00a00a00000000000000000000000000
                   000000000000007c03a6010000ab01000000000000000001007417000000
                   000000000000007c057c006a070000000000000000a6020000ab02000000
                   00000000005300
-               279           0 RESUME                   0
+               290           0 RESUME                   0
                
-               280           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               291           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               281          32 LOAD_FAST                0 (self)
+               292          32 LOAD_FAST                0 (self)
                             34 LOAD_METHOD              1 (_create_lookup_dict)
                             56 LOAD_FAST                3 (request)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               4 (lookup_dict)
                
-               282          74 LOAD_FAST                4 (lookup_dict)
+               293          74 LOAD_FAST                4 (lookup_dict)
                             76 LOAD_METHOD              2 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (query_param_name)
                            110 LOAD_CONST               0 (None)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               5 (values)
                
-               284         128 LOAD_FAST                5 (values)
+               295         128 LOAD_FAST                5 (values)
                            130 POP_JUMP_FORWARD_IF_NOT_NONE    68 (to 268)
                
-               285         132 LOAD_FAST                0 (self)
+               296         132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                4 (default)
                            144 POP_JUMP_FORWARD_IF_NONE     9 (to 164)
                
-               286         146 LOAD_FAST                0 (self)
+               297         146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                4 (default)
                            158 BUILD_LIST               1
                            160 STORE_FAST               5 (values)
                            162 JUMP_FORWARD            52 (to 268)
                
-               287     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
+               298     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
                            176 LOAD_GLOBAL             12 (NoneType)
                            188 LOAD_FAST                0 (self)
                            190 LOAD_ATTR                7 (target_type)
                            200 PRECALL                  2
                            204 CALL                     2
                            214 POP_JUMP_FORWARD_IF_FALSE     2 (to 220)
                
-               288         216 LOAD_CONST               0 (None)
+               299         216 LOAD_CONST               0 (None)
                            218 RETURN_VALUE
                
-               290     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
+               301     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
                
-               291         232 LOAD_CONST               1 ("No value found for request parameter '")
+               302         232 LOAD_CONST               1 ("No value found for request parameter '")
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (query_param_name)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               2 ("'")
                            250 BUILD_STRING             3
                
-               290         252 PRECALL                  1
+               301         252 PRECALL                  1
                            256 CALL                     1
                            266 RAISE_VARARGS            1
                
-               294     >>  268 LOAD_FAST                0 (self)
+               305     >>  268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                9 (consume)
                            280 POP_JUMP_FORWARD_IF_FALSE    21 (to 324)
                
-               295         282 LOAD_FAST                0 (self)
+               306         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD             10 (_consume_param)
                            306 LOAD_FAST                3 (request)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               297     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
+               308     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
                            336 LOAD_FAST                5 (values)
                            338 LOAD_FAST                0 (self)
                            340 LOAD_ATTR                7 (target_type)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 RETURN_VALUE
                consts
@@ -2522,50 +2570,50 @@
                   "'"
                names      ('_get_request_from_args', '_create_lookup_dict', 'get', 'query_param_name', 'default', 'issubclass', 'NoneType', 'target_type', 'Exception', 'consume', '_consume_param', '_convert_value_to_type')
                varnames   ('self', 'args', 'kwargs', 'request', 'lookup_dict', 'values')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 279
+               firstlineno 290
                lnotab 0x02011e012a01360204010e011201340104020c0114ff10040e012a02
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'query_param_name', 'Optional', 'str', '__annotations__', 'default', 'Any', 'consume', 'bool', 'check', 'HttpRequest', '_create_lookup_dict', '_consume_param', 'dict', 'get_value')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQuery'
-         firstlineno 252
+         firstlineno 263
          lnotab 0x0c0238012c012c0206040c070c0a
       'InjectedParamQuery'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640165036602640284045a0464016503660264
             0384045a0564045300
-         300           0 RESUME                   0
+         311           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryGet')
                        8 STORE_NAME               2 (__qualname__)
          
-         302          10 LOAD_CONST               1 ('request')
+         313          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 302>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 313>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         306          22 LOAD_CONST               1 ('request')
+         317          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 306>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 317>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryGet'
             'request'
@@ -2577,28 +2625,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               302           2 RESUME                   0
+               313           2 RESUME                   0
                
-               303           4 LOAD_GLOBAL              1 (NULL + typing)
+               314           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (GET)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               304          66 LOAD_CLOSURE             2 (qd)
+               315          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 304>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 315>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -2610,15 +2658,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     304           2 RESUME                   0
+                     315           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2631,110 +2679,110 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 304
+                     firstlineno 315
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 302
+               firstlineno 313
                lnotab 0x04013e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000760072
                   397405000000000000000000007407000000000000000000006a04000000
                   0000000000740a000000000000000000007c016a010000000000000000a6
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f0100000000000000006400530064005300
-               306           0 RESUME                   0
+               317           0 RESUME                   0
                
-               307           2 LOAD_FAST                0 (self)
+               318           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               308          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               319          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               309          42 LOAD_GLOBAL              7 (NULL + typing)
+               320          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               308         114 PRECALL                  2
+               319         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               307     >>  144 LOAD_CONST               0 (None)
+               318     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 306
+               firstlineno 317
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryGet'
-         firstlineno 300
+         firstlineno 311
          lnotab 0x0a020c04
       'InjectedParamQueryGet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640165036602640284045a0464016503660264
             0384045a0564045300
-         313           0 RESUME                   0
+         324           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryPost')
                        8 STORE_NAME               2 (__qualname__)
          
-         315          10 LOAD_CONST               1 ('request')
+         326          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 315>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 326>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         319          22 LOAD_CONST               1 ('request')
+         330          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 319>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 330>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryPost'
             'request'
@@ -2746,28 +2794,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               315           2 RESUME                   0
+               326           2 RESUME                   0
                
-               316           4 LOAD_GLOBAL              1 (NULL + typing)
+               327           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (POST)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               317          66 LOAD_CLOSURE             2 (qd)
+               328          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 317>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 328>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -2779,15 +2827,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     317           2 RESUME                   0
+                     328           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -2800,96 +2848,96 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 317
+                     firstlineno 328
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 315
+               firstlineno 326
                lnotab 0x04013e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000760072
                   397405000000000000000000007407000000000000000000006a04000000
                   0000000000740a000000000000000000007c016a010000000000000000a6
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f0100000000000000006400530064005300
-               319           0 RESUME                   0
+               330           0 RESUME                   0
                
-               320           2 LOAD_FAST                0 (self)
+               331           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (POST)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               321          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               332          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               322          42 LOAD_GLOBAL              7 (NULL + typing)
+               333          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (POST)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               321         114 PRECALL                  2
+               332         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (POST)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               320     >>  144 LOAD_CONST               0 (None)
+               331     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'POST', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 319
+               firstlineno 330
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryPost'
-         firstlineno 313
+         firstlineno 324
          lnotab 0x0a020c04
       'InjectedParamQueryPost'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         326           0 RESUME                   0
+         337           0 RESUME                   0
          
-         327           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
+         338           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -2897,27 +2945,27 @@
             ('default', 'consume')
          names      ('InjectedParamQueryGet',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_get'
-         firstlineno 326
+         firstlineno 337
          lnotab 0x0201
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         330           0 RESUME                   0
+         341           0 RESUME                   0
          
-         331           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
+         342           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -2925,29 +2973,29 @@
             ('default', 'consume')
          names      ('InjectedParamQueryPost',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_post'
-         firstlineno 330
+         firstlineno 341
          lnotab 0x0201
       'default'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007404000000
             000000000000007407000000000000000000007c007c01ac01a6020000ab
             020000000000000000a6020000ab0200000000000000005300
-         334           0 RESUME                   0
+         345           0 RESUME                   0
          
-         335           2 LOAD_GLOBAL              1 (NULL + typing)
+         346           2 LOAD_GLOBAL              1 (NULL + typing)
                       14 LOAD_ATTR                1 (cast)
                       24 LOAD_GLOBAL              4 (T)
                       36 LOAD_GLOBAL              7 (NULL + InjectedParamQuery)
                       48 LOAD_FAST                0 (default)
                       50 LOAD_FAST                1 (consume)
                       52 KW_NAMES                 1
                       54 PRECALL                  2
@@ -2960,15 +3008,15 @@
             ('default', 'consume')
          names      ('typing', 'cast', 'T', 'InjectedParamQuery')
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param'
-         firstlineno 334
+         firstlineno 345
          lnotab 0x0201
       'values'
       'target_type'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 6
@@ -2994,148 +3042,148 @@
             00720264056e0164065300740b0000000000000000000074140000000000
             00000000006a0b00000000000000007c01a6020000ab0200000000000000
             0072147415000000000000000000006a0b00000000000000007c02a60100
             00ab010000000000000000530074190000000000000000000064077c019b
             0064087c029b009d04a6010000ab0100000000000000008201
                        0 MAKE_CELL                3 (list_type)
          
-         338           2 RESUME                   0
+         349           2 RESUME                   0
          
-         340           4 LOAD_GLOBAL              1 (NULL + typing)
+         351           4 LOAD_GLOBAL              1 (NULL + typing)
                       16 LOAD_ATTR                1 (get_origin)
                       26 LOAD_FAST                1 (target_type)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 LOAD_GLOBAL              4 (list)
                       54 COMPARE_OP               2 (==)
                       60 POP_JUMP_FORWARD_IF_FALSE    40 (to 142)
          
-         341          62 LOAD_GLOBAL              1 (NULL + typing)
+         352          62 LOAD_GLOBAL              1 (NULL + typing)
                       74 LOAD_ATTR                3 (get_args)
                       84 LOAD_FAST                1 (target_type)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_CONST               1 (0)
                      102 BINARY_SUBSCR
                      112 STORE_DEREF              3 (list_type)
          
-         342         114 LOAD_CLOSURE             3 (list_type)
+         353         114 LOAD_CLOSURE             3 (list_type)
                      116 BUILD_TUPLE              1
-                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 342>)
+                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 353>)
                      120 MAKE_FUNCTION            8 (closure)
                      122 LOAD_FAST                0 (values)
                      124 GET_ITER
                      126 PRECALL                  0
                      130 CALL                     0
                      140 RETURN_VALUE
          
-         344     >>  142 LOAD_FAST                1 (target_type)
+         355     >>  142 LOAD_FAST                1 (target_type)
                      144 LOAD_GLOBAL              4 (list)
                      156 COMPARE_OP               2 (==)
                      162 POP_JUMP_FORWARD_IF_FALSE    12 (to 188)
          
-         345         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 345>)
+         356         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 356>)
                      166 MAKE_FUNCTION            0
                      168 LOAD_FAST                0 (values)
                      170 GET_ITER
                      172 PRECALL                  0
                      176 CALL                     0
                      186 RETURN_VALUE
          
-         348     >>  188 LOAD_FAST                0 (values)
+         359     >>  188 LOAD_FAST                0 (values)
                      190 LOAD_CONST               1 (0)
                      192 BINARY_SUBSCR
                      202 STORE_FAST               2 (value)
          
-         350         204 LOAD_FAST                2 (value)
+         361         204 LOAD_FAST                2 (value)
                      206 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 210)
          
-         351         208 JUMP_FORWARD           201 (to 612)
+         362         208 JUMP_FORWARD           201 (to 612)
          
-         352     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
+         363     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
                      222 LOAD_FAST                2 (value)
                      224 LOAD_FAST                1 (target_type)
                      226 PRECALL                  2
                      230 CALL                     2
                      240 POP_JUMP_FORWARD_IF_FALSE     2 (to 246)
          
-         353         242 LOAD_FAST                2 (value)
+         364         242 LOAD_FAST                2 (value)
                      244 RETURN_VALUE
          
-         354     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
+         365     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
                      258 LOAD_GLOBAL             12 (str)
                      270 LOAD_FAST                1 (target_type)
                      272 PRECALL                  2
                      276 CALL                     2
                      286 POP_JUMP_FORWARD_IF_FALSE    15 (to 318)
          
-         355         288 LOAD_GLOBAL             13 (NULL + str)
+         366         288 LOAD_GLOBAL             13 (NULL + str)
                      300 LOAD_FAST                2 (value)
                      302 PRECALL                  1
                      306 CALL                     1
                      316 RETURN_VALUE
          
-         356     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
+         367     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
                      330 LOAD_GLOBAL             14 (int)
                      342 LOAD_FAST                1 (target_type)
                      344 PRECALL                  2
                      348 CALL                     2
                      358 POP_JUMP_FORWARD_IF_FALSE    15 (to 390)
          
-         357         360 LOAD_GLOBAL             15 (NULL + int)
+         368         360 LOAD_GLOBAL             15 (NULL + int)
                      372 LOAD_FAST                2 (value)
                      374 PRECALL                  1
                      378 CALL                     1
                      388 RETURN_VALUE
          
-         358     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
+         369     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
                      402 LOAD_GLOBAL             16 (float)
                      414 LOAD_FAST                1 (target_type)
                      416 PRECALL                  2
                      420 CALL                     2
                      430 POP_JUMP_FORWARD_IF_FALSE    15 (to 462)
          
-         359         432 LOAD_GLOBAL             17 (NULL + float)
+         370         432 LOAD_GLOBAL             17 (NULL + float)
                      444 LOAD_FAST                2 (value)
                      446 PRECALL                  1
                      450 CALL                     1
                      460 RETURN_VALUE
          
-         360     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
+         371     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
                      474 LOAD_GLOBAL             18 (bool)
                      486 LOAD_FAST                1 (target_type)
                      488 PRECALL                  2
                      492 CALL                     2
                      502 POP_JUMP_FORWARD_IF_FALSE     8 (to 520)
          
-         361         504 LOAD_FAST                2 (value)
+         372         504 LOAD_FAST                2 (value)
                      506 LOAD_CONST               4 ((False, '', 'false', 'False'))
                      508 CONTAINS_OP              0
                      510 POP_JUMP_FORWARD_IF_FALSE     2 (to 516)
                      512 LOAD_CONST               5 (False)
                      514 JUMP_FORWARD             1 (to 518)
                  >>  516 LOAD_CONST               6 (True)
                  >>  518 RETURN_VALUE
          
-         362     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
+         373     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
                      532 LOAD_GLOBAL             20 (uuid)
                      544 LOAD_ATTR               11 (UUID)
                      554 LOAD_FAST                1 (target_type)
                      556 PRECALL                  2
                      560 CALL                     2
                      570 POP_JUMP_FORWARD_IF_FALSE    20 (to 612)
          
-         363         572 LOAD_GLOBAL             21 (NULL + uuid)
+         374         572 LOAD_GLOBAL             21 (NULL + uuid)
                      584 LOAD_ATTR               11 (UUID)
                      594 LOAD_FAST                2 (value)
                      596 PRECALL                  1
                      600 CALL                     1
                      610 RETURN_VALUE
          
-         365     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
+         376     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
                      624 LOAD_CONST               7 ('Unsupported type: ')
                      626 LOAD_FAST                1 (target_type)
                      628 FORMAT_VALUE             0
                      630 LOAD_CONST               8 (' for value: ')
                      632 LOAD_FAST                2 (value)
                      634 FORMAT_VALUE             0
                      636 BUILD_STRING             4
@@ -3151,15 +3199,15 @@
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d137d017401000000000000000000007c01670189
                   02a6020000ab02000000000000000091028c145300
                              0 COPY_FREE_VARS           1
                
-               342           2 RESUME                   0
+               353           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                19 (to 48)
                             10 STORE_FAST               1 (v)
                             12 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             24 LOAD_FAST                1 (v)
                             26 BUILD_LIST               1
@@ -3172,25 +3220,25 @@
                consts
                names      ('_convert_value_to_type',)
                varnames   ('.0', 'v')
                freevars   ('list_type',)
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 342
+               firstlineno 353
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d187d017401000000000000000000007c016701740200
                   000000000000000000a6020000ab02000000000000000091028c195300
-               345           0 RESUME                   0
+               356           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                24 (to 56)
                              8 STORE_FAST               1 (v)
                             10 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             22 LOAD_FAST                1 (v)
                             24 BUILD_LIST               1
@@ -3203,81 +3251,81 @@
                consts
                names      ('_convert_value_to_type', 'str')
                varnames   ('.0', 'v')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 345
+               firstlineno 356
                lnotab 0x
             (False, '', 'false', 'False')
             False
             True
             'Unsupported type: '
             ' for value: '
          names      ('typing', 'get_origin', 'list', 'get_args', 'isinstance', 'issubclass', 'str', 'int', 'float', 'bool', 'uuid', 'UUID', 'ValueError')
          varnames   ('values', 'target_type', 'value')
          freevars   ()
          cellvars   ('list_type',)
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_convert_value_to_type'
-         firstlineno 338
+         firstlineno 349
          lnotab
             0x04023a0134011c0216011803100204010201200104012a011e012a011e
             012a011e012a01100134012802
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02640184005a0364026504640365056506650466
             02190000000000000000006604640484045a0764056508640665096a0a00
             000000000000006407650b650c190000000000000000006606640884045a
             0d64095300
-         373           0 RESUME                   0
+         384           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamForm')
                        8 STORE_NAME               2 (__qualname__)
          
-         374          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 374>)
+         385          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 385>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (check)
          
-         380          16 LOAD_CONST               2 ('args')
+         391          16 LOAD_CONST               2 ('args')
                       18 LOAD_NAME                4 (Any)
                       20 LOAD_CONST               3 ('kwargs')
                       22 LOAD_NAME                5 (dict)
                       24 LOAD_NAME                6 (str)
                       26 LOAD_NAME                4 (Any)
                       28 BUILD_TUPLE              2
                       30 BINARY_SUBSCR
                       40 BUILD_TUPLE              4
-                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 380>)
+                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 391>)
                       44 MAKE_FUNCTION            4 (annotations)
                       46 STORE_NAME               7 (get_value)
          
-         392          48 LOAD_CONST               5 ('request')
+         403          48 LOAD_CONST               5 ('request')
          
-         393          50 LOAD_NAME                8 (HttpRequest)
+         404          50 LOAD_NAME                8 (HttpRequest)
          
-         392          52 LOAD_CONST               6 ('value')
+         403          52 LOAD_CONST               6 ('value')
          
-         393          54 LOAD_NAME                9 (forms)
+         404          54 LOAD_NAME                9 (forms)
                       56 LOAD_ATTR               10 (Form)
          
-         392          66 LOAD_CONST               7 ('return')
+         403          66 LOAD_CONST               7 ('return')
          
-         394          68 LOAD_NAME               11 (Optional)
+         405          68 LOAD_NAME               11 (Optional)
                       70 LOAD_NAME               12 (HttpResponse)
                       72 BINARY_SUBSCR
          
-         392          82 BUILD_TUPLE              6
-                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 392>)
+         403          82 BUILD_TUPLE              6
+                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 403>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              13 (replace_response)
                       90 LOAD_CONST               9 (None)
                       92 RETURN_VALUE
          consts
             'InjectedParamForm'
             code
@@ -3286,49 +3334,49 @@
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000740400
                   0000000000000000006a030000000000000000a6020000ab020000000000
                   000000731774090000000000000000000064017c006a0100000000000000
                   009b009d02a6010000ab010000000000000000820164005300
-               374           0 RESUME                   0
+               385           0 RESUME                   0
                
-               375           2 LOAD_GLOBAL              1 (NULL + issubclass)
+               386           2 LOAD_GLOBAL              1 (NULL + issubclass)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (target_type)
                             26 LOAD_GLOBAL              4 (forms)
                             38 LOAD_ATTR                3 (BaseForm)
                             48 PRECALL                  2
                             52 CALL                     2
                             62 POP_JUMP_FORWARD_IF_TRUE    23 (to 110)
                
-               376          64 LOAD_GLOBAL              9 (NULL + Exception)
+               387          64 LOAD_GLOBAL              9 (NULL + Exception)
                
-               377          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
+               388          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                1 (target_type)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             2
                
-               376          94 PRECALL                  1
+               387          94 PRECALL                  1
                             98 CALL                     1
                            108 RAISE_VARARGS            1
                
-               375     >>  110 LOAD_CONST               0 (None)
+               386     >>  110 LOAD_CONST               0 (None)
                            112 RETURN_VALUE
                consts
                   None
                   'argument type for handle_form() must be a subclass of django.forms.BaseForm, got '
                names      ('issubclass', 'target_type', 'forms', 'BaseForm', 'Exception')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 374
+               firstlineno 385
                lnotab 0x02013e010c0112ff10ff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -3345,99 +3393,99 @@
                   0000000000000000007d057c05a00a000000000000000000000000000000
                   00000000007417000000000000000000006a0c00000000000000007c036a
                   0d0000000000000000a6010000ab010000000000000000a6010000ab0100
                   0000000000000001007c00a0020000000000000000000000000000000000
                   0000007c05ac03a6010000ab0100000000000000007d046e147c00a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007d047c045300
-               380           0 RESUME                   0
+               391           0 RESUME                   0
                
-               381           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               392           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               382          32 LOAD_GLOBAL              3 (NULL + is_post)
+               393          32 LOAD_GLOBAL              3 (NULL + is_post)
                             44 LOAD_FAST                3 (request)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 POP_JUMP_FORWARD_IF_FALSE    34 (to 130)
                
-               383          62 LOAD_FAST                0 (self)
+               394          62 LOAD_FAST                0 (self)
                             64 LOAD_METHOD              2 (target_type)
                             86 LOAD_FAST                3 (request)
                             88 LOAD_ATTR                3 (POST)
                             98 LOAD_FAST                3 (request)
                            100 LOAD_ATTR                4 (FILES)
                            110 KW_NAMES                 1
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               4 (form)
                            128 JUMP_FORWARD           147 (to 424)
                
-               384     >>  130 LOAD_FAST                3 (request)
+               395     >>  130 LOAD_FAST                3 (request)
                            132 LOAD_ATTR                5 (content_type)
                            142 LOAD_CONST               2 ('application/json')
                            144 COMPARE_OP               2 (==)
                            150 POP_JUMP_FORWARD_IF_FALSE   116 (to 384)
                
-               385         152 LOAD_GLOBAL             13 (NULL + typing)
+               396         152 LOAD_GLOBAL             13 (NULL + typing)
                            164 LOAD_ATTR                7 (cast)
                            174 LOAD_GLOBAL             16 (QueryDict)
                            186 LOAD_FAST                3 (request)
                            188 LOAD_ATTR                3 (POST)
                            198 PRECALL                  2
                            202 CALL                     2
                            212 LOAD_METHOD              9 (copy)
                            234 PRECALL                  0
                            238 CALL                     0
                            248 STORE_FAST               5 (new_post_dict)
                
-               386         250 LOAD_FAST                5 (new_post_dict)
+               397         250 LOAD_FAST                5 (new_post_dict)
                            252 LOAD_METHOD             10 (update)
                            274 LOAD_GLOBAL             23 (NULL + json)
                            286 LOAD_ATTR               12 (loads)
                            296 LOAD_FAST                3 (request)
                            298 LOAD_ATTR               13 (body)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 PRECALL                  1
                            326 CALL                     1
                            336 POP_TOP
                
-               387         338 LOAD_FAST                0 (self)
+               398         338 LOAD_FAST                0 (self)
                            340 LOAD_METHOD              2 (target_type)
                            362 LOAD_FAST                5 (new_post_dict)
                            364 KW_NAMES                 3
                            366 PRECALL                  1
                            370 CALL                     1
                            380 STORE_FAST               4 (form)
                            382 JUMP_FORWARD            20 (to 424)
                
-               389     >>  384 LOAD_FAST                0 (self)
+               400     >>  384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD              2 (target_type)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 STORE_FAST               4 (form)
                
-               390     >>  424 LOAD_FAST                4 (form)
+               401     >>  424 LOAD_FAST                4 (form)
                            426 RETURN_VALUE
                consts
                   None
                   ('data', 'files')
                   'application/json'
                   ('data',)
                names      ('_get_request_from_args', 'is_post', 'target_type', 'POST', 'FILES', 'content_type', 'typing', 'cast', 'QueryDict', 'copy', 'update', 'json', 'loads', 'body')
                varnames   ('self', 'args', 'kwargs', 'request', 'form', 'new_post_dict')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 380
+               firstlineno 391
                lnotab 0x02011e011e0144011601620158012e022801
             'request'
             'value'
             'return'
             code
                argcount  : 3
                nlocals   : 7
@@ -3456,362 +3504,362 @@
                   0000000000a6010000ab0100000000000000007c066a0b00000000000000
                   0064049c037c047c056a0a00000000000000003c0000008c557419000000
                   000000000000007c037c047413000000000000000000007c02a00d000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00a6010000ab0100000000000000007c02a0040000000000000000000000
                   000000000000000000a6000000ab00000000000000000064059c04a60100
                   00ab010000000000000000530064005300
-               392           0 RESUME                   0
+               403           0 RESUME                   0
                
-               395           2 LOAD_GLOBAL              1 (NULL + is_patch)
+               406           2 LOAD_GLOBAL              1 (NULL + is_patch)
                             14 LOAD_FAST                1 (request)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 POP_JUMP_FORWARD_IF_FALSE   215 (to 462)
                             32 LOAD_FAST                1 (request)
                             34 LOAD_ATTR                1 (content_type)
                             44 LOAD_CONST               1 ('application/json')
                             46 COMPARE_OP               2 (==)
                             52 POP_JUMP_FORWARD_IF_FALSE   204 (to 462)
                
-               396          54 LOAD_FAST                1 (request)
+               407          54 LOAD_FAST                1 (request)
                             56 LOAD_ATTR                2 (headers)
                             66 LOAD_METHOD              3 (get)
                             88 LOAD_CONST               2 ('X-DFV-Validate-Field')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 STORE_FAST               3 (validate_field)
                
-               397         106 LOAD_FAST                2 (value)
+               408         106 LOAD_FAST                2 (value)
                            108 LOAD_METHOD              4 (is_valid)
                            130 PRECALL                  0
                            134 CALL                     0
                            144 POP_TOP
                
-               398         146 BUILD_MAP                0
+               409         146 BUILD_MAP                0
                            148 STORE_FAST               4 (fields)
                
-               399         150 LOAD_FAST                2 (value)
+               410         150 LOAD_FAST                2 (value)
                            152 GET_ITER
                        >>  154 FOR_ITER                84 (to 324)
                            156 STORE_FAST               5 (bound_field)
                
-               400         158 LOAD_FAST                5 (bound_field)
+               411         158 LOAD_FAST                5 (bound_field)
                            160 LOAD_ATTR                5 (field)
                            170 LOAD_ATTR                6 (widget)
                            180 STORE_FAST               6 (widget)
                
-               402         182 LOAD_GLOBAL             15 (NULL + len)
+               413         182 LOAD_GLOBAL             15 (NULL + len)
                            194 LOAD_FAST                5 (bound_field)
                            196 LOAD_ATTR                8 (errors)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 LOAD_CONST               3 (0)
                            222 COMPARE_OP               2 (==)
                
-               403         228 LOAD_GLOBAL             19 (NULL + str)
+               414         228 LOAD_GLOBAL             19 (NULL + str)
                            240 LOAD_FAST                2 (value)
                            242 LOAD_FAST                5 (bound_field)
                            244 LOAD_ATTR               10 (name)
                            254 BINARY_SUBSCR
                            264 LOAD_ATTR                8 (errors)
                            274 PRECALL                  1
                            278 CALL                     1
                
-               404         288 LOAD_FAST                6 (widget)
+               415         288 LOAD_FAST                6 (widget)
                            290 LOAD_ATTR               11 (attrs)
                
-               401         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
+               412         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
                            302 BUILD_CONST_KEY_MAP      3
                            304 LOAD_FAST                4 (fields)
                            306 LOAD_FAST                5 (bound_field)
                            308 LOAD_ATTR               10 (name)
                            318 STORE_SUBSCR
                            322 JUMP_BACKWARD           85 (to 154)
                
-               407     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
+               418     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
                
-               409         336 LOAD_FAST                3 (validate_field)
+               420         336 LOAD_FAST                3 (validate_field)
                
-               410         338 LOAD_FAST                4 (fields)
+               421         338 LOAD_FAST                4 (fields)
                
-               411         340 LOAD_GLOBAL             19 (NULL + str)
+               422         340 LOAD_GLOBAL             19 (NULL + str)
                            352 LOAD_FAST                2 (value)
                            354 LOAD_METHOD             13 (non_field_errors)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 PRECALL                  1
                            394 CALL                     1
                
-               412         404 LOAD_FAST                2 (value)
+               423         404 LOAD_FAST                2 (value)
                            406 LOAD_METHOD              4 (is_valid)
                            428 PRECALL                  0
                            432 CALL                     0
                
-               408         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
+               419         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
                            444 BUILD_CONST_KEY_MAP      4
                
-               407         446 PRECALL                  1
+               418         446 PRECALL                  1
                            450 CALL                     1
                            460 RETURN_VALUE
                
-               416     >>  462 LOAD_CONST               0 (None)
+               427     >>  462 LOAD_CONST               0 (None)
                            464 RETURN_VALUE
                consts
                   None
                   'application/json'
                   'X-DFV-Validate-Field'
                   0
                   ('valid', 'errors', 'attrs')
                   ('name', 'fields', 'non_field_errors', 'form_valid')
                names      ('is_patch', 'content_type', 'headers', 'get', 'is_valid', 'field', 'widget', 'len', 'errors', 'str', 'name', 'attrs', 'JsonResponse', 'non_field_errors')
                varnames   ('self', 'request', 'value', 'validate_field', 'fields', 'bound_field', 'widget')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 392
+               firstlineno 403
                lnotab
                   0x02033401340128010401080118022e013c010cfd18060c020201020140
                   0126fc04ff1009
             None
          names      ('__name__', '__module__', '__qualname__', 'check', 'Any', 'dict', 'str', 'get_value', 'HttpRequest', 'forms', 'Form', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamForm'
-         firstlineno 373
+         firstlineno 384
          lnotab 0x0a010606200c020102ff02010cff02020efe
       'InjectedParamForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000053
             00
-         419           0 RESUME                   0
+         430           0 RESUME                   0
          
-         420           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
+         431           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 RETURN_VALUE
          consts
             None
          names      ('InjectedParamForm',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'handle_form'
-         firstlineno 419
+         firstlineno 430
          lnotab 0x0201
       'querydict'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401ac02a6010000ab010000000000
             0000007d027c02a00100000000000000000000000000000000000000007c
             00a6010000ab01000000000000000001007c027c013d007c025300
-         428           0 RESUME                   0
+         439           0 RESUME                   0
          
-         429           2 LOAD_GLOBAL              1 (NULL + QueryDict)
+         440           2 LOAD_GLOBAL              1 (NULL + QueryDict)
                       14 LOAD_CONST               1 (True)
                       16 KW_NAMES                 2
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               2 (temp)
          
-         430          34 LOAD_FAST                2 (temp)
+         441          34 LOAD_FAST                2 (temp)
                       36 LOAD_METHOD              1 (update)
                       58 LOAD_FAST                0 (querydict)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_TOP
          
-         431          76 LOAD_FAST                2 (temp)
+         442          76 LOAD_FAST                2 (temp)
                       78 LOAD_FAST                1 (key)
                       80 DELETE_SUBSCR
          
-         432          82 LOAD_FAST                2 (temp)
+         443          82 LOAD_FAST                2 (temp)
                       84 RETURN_VALUE
          consts
             None
             True
             ('mutable',)
          names      ('QueryDict', 'update')
          varnames   ('querydict', 'key', 'temp')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'querydict_key_removed'
-         firstlineno 428
+         firstlineno 439
          lnotab 0x020120012a010601
       'request'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         435           0 RESUME                   0
+         446           0 RESUME                   0
          
-         436           2 LOAD_FAST                0 (request)
+         447           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('HEAD')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'HEAD'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_head'
-         firstlineno 435
+         firstlineno 446
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         439           0 RESUME                   0
+         450           0 RESUME                   0
          
-         440           2 LOAD_FAST                0 (request)
+         451           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('GET')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'GET'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_get'
-         firstlineno 439
+         firstlineno 450
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         443           0 RESUME                   0
+         454           0 RESUME                   0
          
-         444           2 LOAD_FAST                0 (request)
+         455           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('POST')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'POST'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_post'
-         firstlineno 443
+         firstlineno 454
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         447           0 RESUME                   0
+         458           0 RESUME                   0
          
-         448           2 LOAD_FAST                0 (request)
+         459           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('PUT')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'PUT'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_put'
-         firstlineno 447
+         firstlineno 458
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         451           0 RESUME                   0
+         462           0 RESUME                   0
          
-         452           2 LOAD_FAST                0 (request)
+         463           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('PATCH')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'PATCH'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_patch'
-         firstlineno 451
+         firstlineno 462
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006a00000000000000000064016b02000000005300
-         455           0 RESUME                   0
+         466           0 RESUME                   0
          
-         456           2 LOAD_FAST                0 (request)
+         467           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('DELETE')
                       16 COMPARE_OP               2 (==)
                       22 RETURN_VALUE
          consts
             None
             'DELETE'
          names      ('method',)
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_delete'
-         firstlineno 455
+         firstlineno 466
          lnotab 0x0201
       (None,)
       ('outerHTML',)
       (True,)
       (None, True)
-   names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'element', 'swap_oob', 'bool', 'inject_args', '_handle_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'list', 'dict', '_extract_injected_params', '_get_request_from_args', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete')
+   names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'element', 'swap_oob', 'bool', 'inject_args', '_inject_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'list', 'dict', '_extract_injected_params', '_get_request_from_args', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c012002080108010c010c0118
-      010c011002160116011608261b160902ff0203020102010201020102f906
-      010eff020834f8082602ff040102ff020102ff020202fe0817020102fd06
-      0214fe020314fd020434fc082004030c0118ff0e0102101e1402fd040118
-      ff020226fe020314fd020412fc08351c090c011aff0e01022f0c011aff0e
-      01020c0c011aff0e01020c0e040e04340426231c2e0c0910070c040c040c
-      040c040c04
+      010c0110021601160116082621160902ff02030201020102010201020102
+      f806010eff02060efa020934f7082b02ff040102ff020102ff020202fe08
+      17020102fd060214fe020314fd020434fc082004030c0118ff0e0102101e
+      1402fd040118ff020226fe020314fd020412fc08351c090c011aff0e0102
+      2f0c011aff0e01020c0c011aff0e01020c0e040e04340426231c2e0c0910
+      070c040c040c040c040c04
```

### Comparing `dfv-0.5.0/dfv/__pycache__/test_element.cpython-311.pyc` & `dfv-0.5.1/dfv/__pycache__/test_element.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xbbbfc464 (Sat Jul 29 07:28:59 2023 UTC)
-files sz: 4027
+moddate:  0x7907c864 (Mon Jul 31 19:11:53 2023 UTC)
+files sz: 4360
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a02640064026c035a
@@ -86,31 +86,31 @@
       ('element', 'ElementResponse', 'response_to_str', 'swap_oob')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
-            0x970065005a0164005a0255006503650464013c000000640f640484045a
+            0x970065005a0164005a0255006503650464013c0000006410640484045a
             05640565066602640684045a07640784005a08640884005a09640984005a
             0a640a84005a0b640b84005a0c640c84005a0d640d84005a0e640e84005a
-            0f64035300
+            0f640f84005a1064035300
           12           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ElementDecoratorTestCase')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
           13          12 LOAD_NAME                3 (RequestFactory)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('factory')
                       18 STORE_SUBSCR
          
-          15          22 LOAD_CONST              15 (('return', None))
+          15          22 LOAD_CONST              16 (('return', None))
                       24 LOAD_CONST               4 (<code object setUp, file "/home/roman/prjs/python/dfv/dfv/test_element.py", line 15>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               5 (setUp)
          
           18          30 LOAD_CONST               5 ('response')
                       32 LOAD_NAME                6 (HttpResponse)
                       34 BUILD_TUPLE              2
@@ -145,16 +145,20 @@
           90          78 LOAD_CONST              13 (<code object test_element_return_element_response, file "/home/roman/prjs/python/dfv/dfv/test_element.py", line 90>)
                       80 MAKE_FUNCTION            0
                       82 STORE_NAME              14 (test_element_return_element_response)
          
           99          84 LOAD_CONST              14 (<code object test_element_return_template_http_response, file "/home/roman/prjs/python/dfv/dfv/test_element.py", line 99>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              15 (test_element_return_template_http_response)
-                      90 LOAD_CONST               3 (None)
-                      92 RETURN_VALUE
+         
+         114          90 LOAD_CONST              15 (<code object test_classes, file "/home/roman/prjs/python/dfv/dfv/test_element.py", line 114>)
+                      92 MAKE_FUNCTION            0
+                      94 STORE_NAME              16 (test_classes)
+                      96 LOAD_CONST               3 (None)
+                      98 RETURN_VALUE
          consts
             'ElementDecoratorTestCase'
             'factory'
             'return'
             None
             code
                argcount  : 1
@@ -1212,23 +1216,130 @@
                varnames   ('self', 'viewfn', 'result', 'parsed')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/test_element.py'
                name       'test_element_return_template_http_response'
                firstlineno 99
                lnotab 0x020126021a0104ff0e0102054601200158014201
+            code
+               argcount  : 1
+               nlocals   : 4
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007401000000000000000000006401ac02a6010000ab010000000000
+                  00000064038400a6000000ab0000000000000000007d0102007c017c006a
+                  010000000000000000a00200000000000000000000000000000000000000
+                  006404a6010000ab010000000000000000a6010000ab0100000000000000
+                  007d027406000000000000000000006a040000000000000000a005000000
+                  0000000000000000000000000000000000740d000000000000000000007c
+                  02a6010000ab010000000000000000a6010000ab0100000000000000007d
+                  037c00a00700000000000000000000000000000000000000007c036a0800
+                  000000000000006405190000000000000000006401a6020000ab02000000
+                  0000000000010064005300
+               114           0 RESUME                   0
+               
+               115           2 LOAD_GLOBAL              1 (NULL + element)
+                            14 LOAD_CONST               1 ('foo bar')
+                            16 KW_NAMES                 2
+                            18 PRECALL                  1
+                            22 CALL                     1
+               
+               116          32 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_element.py", line 115>)
+                            34 MAKE_FUNCTION            0
+               
+               115          36 PRECALL                  0
+                            40 CALL                     0
+               
+               116          50 STORE_FAST               1 (viewfn)
+               
+               119          52 PUSH_NULL
+                            54 LOAD_FAST                1 (viewfn)
+                            56 LOAD_FAST                0 (self)
+                            58 LOAD_ATTR                1 (factory)
+                            68 LOAD_METHOD              2 (get)
+                            90 LOAD_CONST               4 ('/')
+                            92 PRECALL                  1
+                            96 CALL                     1
+                           106 PRECALL                  1
+                           110 CALL                     1
+                           120 STORE_FAST               2 (response)
+               
+               120         122 LOAD_GLOBAL              6 (lxml)
+                           134 LOAD_ATTR                4 (html)
+                           144 LOAD_METHOD              5 (fromstring)
+                           166 LOAD_GLOBAL             13 (NULL + response_to_str)
+                           178 LOAD_FAST                2 (response)
+                           180 PRECALL                  1
+                           184 CALL                     1
+                           194 PRECALL                  1
+                           198 CALL                     1
+                           208 STORE_FAST               3 (parsed)
+               
+               121         210 LOAD_FAST                0 (self)
+                           212 LOAD_METHOD              7 (assertEqual)
+                           234 LOAD_FAST                3 (parsed)
+                           236 LOAD_ATTR                8 (attrib)
+                           246 LOAD_CONST               5 ('class')
+                           248 BINARY_SUBSCR
+                           258 LOAD_CONST               1 ('foo bar')
+                           260 PRECALL                  2
+                           264 CALL                     2
+                           274 POP_TOP
+                           276 LOAD_CONST               0 (None)
+                           278 RETURN_VALUE
+               consts
+                  None
+                  'foo bar'
+                  ('classes',)
+                  code
+                     argcount  : 1
+                     nlocals   : 1
+                     stacksize : 3
+                     flags     : 19
+                     code
+                        0x97007401000000000000000000006401a6010000ab0100000000000000
+                        005300
+                     115           0 RESUME                   0
+                     
+                     117           2 LOAD_GLOBAL              1 (NULL + HttpResponse)
+                                  14 LOAD_CONST               1 ('body')
+                                  16 PRECALL                  1
+                                  20 CALL                     1
+                                  30 RETURN_VALUE
+                     consts
+                        None
+                        'body'
+                     names      ('HttpResponse',)
+                     varnames   ('_request',)
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/home/roman/prjs/python/dfv/dfv/test_element.py'
+                     name       'viewfn'
+                     firstlineno 115
+                     lnotab 0x0202
+                  '/'
+                  'class'
+               names      ('element', 'factory', 'get', 'lxml', 'html', 'fromstring', 'response_to_str', 'assertEqual', 'attrib')
+               varnames   ('self', 'viewfn', 'response', 'parsed')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/roman/prjs/python/dfv/dfv/test_element.py'
+               name       'test_classes'
+               firstlineno 114
+               lnotab 0x02011e0104ff0e01020346015801
             ('return', None)
-         names      ('__name__', '__module__', '__qualname__', 'RequestFactory', '__annotations__', 'setUp', 'HttpResponse', '_assert_default_values', 'test_without_braces', 'test_config', 'test_append_swap_oob', 'test_append_swap_oob_exception_if_additional_has_more_than_one_root_element', 'test_swap_oob_exception_if_additional_has_no_id', 'test_element_return_another_element', 'test_element_return_element_response', 'test_element_return_template_http_response')
+         names      ('__name__', '__module__', '__qualname__', 'RequestFactory', '__annotations__', 'setUp', 'HttpResponse', '_assert_default_values', 'test_without_braces', 'test_config', 'test_append_swap_oob', 'test_append_swap_oob_exception_if_additional_has_more_than_one_root_element', 'test_swap_oob_exception_if_additional_has_no_id', 'test_element_return_another_element', 'test_element_return_element_response', 'test_element_return_template_http_response', 'test_classes')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/test_element.py'
          name       'ElementDecoratorTestCase'
          firstlineno 12
-         lnotab 0x0c010a0208030c070608060c0609060b060b060e0609
+         lnotab 0x0c010a0208030c070608060c0609060b060b060e0609060f
       'ElementDecoratorTestCase'
    names      ('unittest', 'TestCase', 'django', 'lxml.html', 'lxml', 'django.http', 'HttpResponse', 'django.template.response', 'TemplateResponse', 'django.test', 'RequestFactory', 'dfv', 'element', 'ElementResponse', 'response_to_str', 'swap_oob', 'ElementDecoratorTestCase')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/roman/prjs/python/dfv/dfv/test_element.py'
    name       '<module>'
```

### Comparing `dfv-0.5.0/dfv/__pycache__/test_form.cpython-311.pyc` & `dfv-0.5.1/dfv/__pycache__/test_form.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x35c1c464 (Sat Jul 29 07:35:17 2023 UTC)
-files sz: 3338
+moddate:  0x3cc7c464 (Sat Jul 29 08:01:00 2023 UTC)
+files sz: 3340
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
```

### Comparing `dfv-0.5.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc` & `dfv-0.5.1/dfv/__pycache__/test_params_to_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.5.0/dfv/static/dfv.js` & `dfv-0.5.1/dfv/static/dfv.js`

 * *Files identical despite different names*

### Comparing `dfv-0.5.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc` & `dfv-0.5.1/dfv/templatetags/__pycache__/dfv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.5.0/dfv/test_element.py` & `dfv-0.5.1/dfv/test_element.py`

 * *Files 9% similar despite different names*

```diff
@@ -106,7 +106,16 @@
             )
 
         result = viewfn(self.factory.get("/"))
         print("result", result)
         parsed: lxml.html.HtmlElement = lxml.html.fromstring(response_to_str(result))
         self.assertEqual(parsed.attrib["id"], "viewfn")
         self.assertEqual(parsed.text.strip(), "123")
+
+    def test_classes(self):
+        @element(classes="foo bar")
+        def viewfn(_request):
+            return HttpResponse("body")
+
+        response = viewfn(self.factory.get("/"))
+        parsed: lxml.html.HtmlElement = lxml.html.fromstring(response_to_str(response))
+        self.assertEqual(parsed.attrib["class"], "foo bar")
```

### Comparing `dfv-0.5.0/dfv/test_form.py` & `dfv-0.5.1/dfv/test_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,27 +27,27 @@
         def test():
             @inject_args()
             def viewfn(_request, form=handle_form()):
                 return HttpResponse(form)
 
         self.assertRaisesRegex(
             Exception,
-            "argument type for handle_form\(\) must be a subclass of django.forms.BaseForm",
+            r"argument type for handle_form\(\) must be a subclass of django.forms.BaseForm",
             test,
         )
 
     def test_error_wrong_form_type(self):
         def test():
             @inject_args()
             def viewfn(_request, _form: str = handle_form()):
                 return HttpResponse("")
 
         self.assertRaisesRegex(
             Exception,
-            "argument type for handle_form\(\) must be a subclass of django.forms.BaseForm",
+            r"argument type for handle_form\(\) must be a subclass of django.forms.BaseForm",
             test,
         )
 
     def test_form_explicit(self):
         @inject_args()
         def viewfn(_request, form: TestForm = handle_form()):
             self.assertEqual(type(form), TestForm)
```

### Comparing `dfv-0.5.0/dfv/test_params_to_args.py` & `dfv-0.5.1/dfv/test_params_to_args.py`

 * *Files identical despite different names*

### Comparing `dfv-0.5.0/pyproject.toml` & `dfv-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfv"
-version = "0.5.0"
+version = "0.5.1"
 description = "Django Function Views"
 authors = ["Roman Roelofsen <romanroe@gmail.com>"]
 include = ["dfv"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 django = "^4.1.7"
@@ -21,14 +21,15 @@
 django-extensions = "^3.1.5"
 black = {extras = ["d"], version = "^23.1.0"}
 django-click = "^2.3.0"
 ruff = "^0.0.280"
 mypy = "1.4.1"
 coverage = "^7.2.1"
 psycopg = "^3.1.9"
+tblib = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line_length = 88
```

### Comparing `dfv-0.5.0/setup.py` & `dfv-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'django>=4.1.7,<5.0.0',
  'lxml>=4.9.2,<5.0.0',
  'typeguard',
  'wrapt>=1.15.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'dfv',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Django Function Views',
     'long_description': 'None',
     'author': 'Roman Roelofsen',
     'author_email': 'romanroe@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dfv-0.5.0/PKG-INFO` & `dfv-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfv
-Version: 0.5.0
+Version: 0.5.1
 Summary: Django Function Views
 Author: Roman Roelofsen
 Author-email: romanroe@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

