# Comparing `tmp/demeuk-3.9.7.tar.gz` & `tmp/demeuk-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demeuk-3.9.7.tar", last modified: Thu Feb 17 11:46:06 2022, max compression
+gzip compressed data, was "demeuk-4.0.1.tar", last modified: Mon Jul 31 09:30:27 2023, max compression
```

## Comparing `demeuk-3.9.7.tar` & `demeuk-4.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:46:06.901337 demeuk-3.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-17 11:45:48.000000 demeuk-3.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-02-17 11:46:06.901337 demeuk-3.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-02-17 11:45:48.000000 demeuk-3.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:46:06.901337 demeuk-3.9.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)    42836 2022-02-17 11:45:48.000000 demeuk-3.9.7/bin/demeuk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:46:06.901337 demeuk-3.9.7/demeuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-17 11:46:06.901337 demeuk-3.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-02-17 11:45:48.000000 demeuk-3.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:30:27.708792 demeuk-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 09:30:02.000000 demeuk-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-31 09:30:27.708792 demeuk-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-31 09:30:02.000000 demeuk-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:30:27.704792 demeuk-4.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51479 2023-07-31 09:30:02.000000 demeuk-4.0.1/bin/demeuk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:30:27.708792 demeuk-4.0.1/demeuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-31 09:30:27.000000 demeuk-4.0.1/demeuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-31 09:30:27.000000 demeuk-4.0.1/demeuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:30:27.000000 demeuk-4.0.1/demeuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 09:30:27.000000 demeuk-4.0.1/demeuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:30:27.000000 demeuk-4.0.1/demeuk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:30:27.708792 demeuk-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 09:30:02.000000 demeuk-4.0.1/setup.py
```

### Comparing `demeuk-3.9.7/LICENSE` & `demeuk-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `demeuk-3.9.7/PKG-INFO` & `demeuk-4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: demeuk
-Version: 3.9.7
+Version: 4.0.1
 Summary: CLI tool to remove invalid chars from a corpus.
 Home-page: https://github.com/NetherlandsForensicInstitute/demeuk
 Author: Netherlands Forensic Institute
 Author-email: holmesnl@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -56,14 +54,14 @@
 
 Now you can run bin/demeuk.py:
 
 Examples:
 ```
     demeuk -i inputfile.tmp -o outputfile.dict -l droppedfile.txt
     demeuk -i inputfile -o outputfile -j 24 -l logfile.log
+    demeuk -i inputfile.tmp -o outputfile.dict -l droppedfile.txt --leak
+    demeuk -i inputfile -o outputfile -j 24 -l logfile.log --leak-full
     demeuk -i inputdir/*.txt -o outputfile.dict -l logfile.log
 ```
 
 ## Docs
 The docs are available at: <http://demeuk.rtfd.io/>
-
-
```

### Comparing `demeuk-3.9.7/README.md` & `demeuk-4.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -37,12 +37,14 @@
 
 Now you can run bin/demeuk.py:
 
 Examples:
 ```
     demeuk -i inputfile.tmp -o outputfile.dict -l droppedfile.txt
     demeuk -i inputfile -o outputfile -j 24 -l logfile.log
+    demeuk -i inputfile.tmp -o outputfile.dict -l droppedfile.txt --leak
+    demeuk -i inputfile -o outputfile -j 24 -l logfile.log --leak-full
     demeuk -i inputdir/*.txt -o outputfile.dict -l logfile.log
 ```
 
 ## Docs
 The docs are available at: <http://demeuk.rtfd.io/>
```

### Comparing `demeuk-3.9.7/bin/demeuk.py` & `demeuk-4.0.1/bin/demeuk.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,20 +19,21 @@
         -i --input <path to file>       Specify the input file to be cleaned, or provide a glob pattern
         -o --output <path to file>      Specify the output file name.
         -l --log <path to file>         Optional, specify where the log file needs to be writen to
         -j --threads <threads>          Optional, demeuk doesn't use threads by default. Specify amount of threads to
                                         spawn. Specify the string 'all' to make demeuk auto detect the amount of threads
                                         to start based on the CPU's.
                                         Note: threading will cost some setup time. Only speeds up for larger files.
-        --input-encoding <encoding>     Forces demeuk to decode the input using this encoding.
+        --input-encoding <encoding>     Forces demeuk to decode the input using this encoding (default: en_US.UTF-8).
         --output-encoding <encoding>    Forces demeuk to encoding the output using this encoding (default: en_US.UTF-8).
         -v --verbose                    When set, the logfile will not only contain lines which caused an error, but
                                         also line which were modified.
         --progress                      Prints out the progress of the demeuk process.
         -n --limit <int>                Limit the number of lines per thread.
+        -s --skip <int>                 Skip <int> amount of lines per thread.
         --punctuation <punctuation>     Use to set the punctuation that is use by options. Defaults to:
                                         ! "#$%&'()*+,-./:;<=>?@[\]^_`{|}~
         --version                       Prints the version of demeuk.
 
     Separating Options:
         -c --cut                        Specify if demeuk should split (default splits on ':'). Returns everything
                                         after the delimiter.
@@ -45,34 +46,44 @@
                                         specified using ','. If the ',' is required for cutting, escape it with a
                                         backslash. Only one delimiter can be used per line.
 
     Check modules (check if a line matches a specific condition):
         --check-min-length <length>     Requires that entries have a minimal requirement of <length> unicode chars
         --check-max-length <length>     Requires that entries have a maximal requirement of <length> unicode chars
         --check-case                    Drop lines where the uppercase line is not equal to the lowercase line
-        --no-check-controlchar          Disable the dropping of lines containing control chars.
+        --check-controlchar             Drop lines containing control chars.
         --check-email                   Drop lines containing e-mail addresses.
-        --check-hash                    Drop lines containing hashes.
+        --check-hash                    Drop lines which are hashes.
+        --check-mac-address             Drop lines which are MAC-addresses.
+        --check-uuid                    Drop lines which are UUID.
         --check-non-ascii               If a line contain a non ascii char e.g. ü or ç (or everything outside ascii
                                         range) the line is dropped.
         --check-replacement-character   Drop lines containing replacement characters '�'.
+        --check-starting-with <string>  Drop lines starting with string, can be multiple strings. Specify multiple
+                                        with as comma-seperated list.
+        --check-ending-with <string>    Drop lines ending with string, can be multiple strings. Specify multiple
+                                        with as comma-seperated list.
+        --check-empty-line              Drop lines that are empty or only contain whitespace characters
+        --check-regex <string>          Drop lines that do not match the regex. Regex is a comma seperated list of
+                                        regexes. Example: [a-z]{1,8},[0-9]{1,8}
 
     Modify modules (modify a line in place):
         --hex                           Replace lines like: $HEX[41424344] with ABCD.
         --html                          Replace lines like: &#351;ifreyok with şifreyok.
         --html-named                    Replace lines like: &#alpha; Those structures are more like passwords, so
                                         be careful to enable this option.
+        --title-case                    Replace line like 'this test string' to 'This Test String'
         --umlaut                        Replace lines like ko"ffie with an o with an umlaut.
-        --no-mojibake                   disable fixing mojibakes, useful if you know the encoding.
-        --no-encode                     disable guessing of encoding, this force to use the --input-encoding.
-        --no-tab                        disable replacing tab char with ':'
-        --no-newline                    disable removing newline characters (\r\n) from end and beginning.
+        --mojibake                      Fixes mojibakes, which means lines like SmˆrgÂs will be fixed to Smörgås.
+        --encode                        Enables guessing of encoding, based on chardet and custom implementation.
+        --tab                           Enables replacing tab char with ':', sometimes leaks contain both ':' and '\t'.
+        --newline                       Enables removing newline characters (\r\n) from end and beginning of lines.
         --non-ascii                     Replace non ascii char with their replacement letters. For example ü
                                         becomes u, ç becomes c.
-        --no-trim                       disable removing newlines representations from end and beginning. Newline
+        --trim                          Enables removing newlines representations from end and beginning. Newline
                                         representations detected are '\\n', '\\r', '\n', '\r', '<br>', and '<br />'.
 
     Add modules (Modify a line, but keep the original as well):
         --add-lower                     If a line contains a capital letter this will add the lower case variant
         --add-latin-ligatures           If a line contains a single ligatures of a latin letter (such as ij), the line
                                         is correct but the original line contain the ligatures is also added to output.
         --add-split                     split on known chars like - and . and add those to the final dictionary.
@@ -84,14 +95,23 @@
     Remove modules (remove specific parts of a line):
         --remove-strip-punctuation      Remove starting and trailing punctuation
         --remove-punctuation            Remove all punctuation in a line
         --remove-email                  Enable email filter, this will catch strings like
                                         1238661:test@example.com:password
     Macro modules:
         -g --googlengram                When set, demeuk will strip universal pos tags: like _NOUN_ or _ADJ
+        --leak                          When set, demeuk will run the following modules:
+                                            mojibake, encode, newline, check-controlchar
+                                        This is recommended when working with leaks and was the default bevarior in
+                                        demeuk version 3.11.0 and below.
+        --leak-full                     When set, demeuk will run the following modules:
+                                            mojibake, encode, newline, check-controlchar,
+                                            hex, html, html-named,
+                                            check-hash, check-mac-address, check-uuid, check-email,
+                                            check-replacement-character, check-empty-line
 """
 
 from binascii import hexlify, unhexlify
 from glob import glob
 from hashlib import md5
 from html import unescape
 from inspect import cleandoc
@@ -114,21 +134,23 @@
 from ftfy.fixes import fix_latin_ligatures
 from nltk import str2tuple
 from nltk.tokenize import WhitespaceTokenizer
 from tqdm import tqdm
 from unidecode import unidecode
 
 
-version = '3.9.7'
+version = '4.0.1'
 
 # Search from start to finish for the string $HEX[], with block of a-f0-9 with even number
 # of hex chars. The first match group is repeated.
 HEX_REGEX = re_compile(r"^\$(?:HEX|hex)\[((?:[0-9a-fA-F]{2})+)\]$")
 EMAIL_REGEX = '.{1,64}@([a-zA-Z0-9_-]{1,63}\\.){1,3}[a-zA-Z]{2,6}'
 HASH_HEX_REGEX = '^[a-fA-F0-9]+$'
+MAC_REGEX = '^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$'
+UUID_REGEX = '^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$'
 
 # Officiale bcrypt hashes hae a bit more fixed size, but saw some weird once:
 # $2a$10$demo as example
 HASH_BCRYPT_REGEX = '^\\$2[ayb]\\$[0-9]{1,}\\$[\\w\\.\\/]{4,}$'
 # Crypt hashes can look a lot like passwords. We do two options here
 # $1[$optional salt, max 16]$string of a-zA-Z0-9./ length 7 min till end of line
 # $1$a-zA-Z0-9./ min length 12 to make sure we hit somthing like: a-zA-Z0-9./
@@ -178,14 +200,15 @@
 
 
 def clean_googlengram(line):
     """Removes speechtags from line specific to the googlengram module
 
     Param:
         line (unicode)
+
     Returns:
         line (unicode)
     """
     return_line = line.split("\t")[0]  # Get the ngram, remove year, counter, etc
     clean = []
     words = WhitespaceTokenizer().tokenize(return_line)
     for word in words:
@@ -209,28 +232,30 @@
 
 
 def remove_email(line):
     """Removes e-mail addresses from a line.
 
     Params:
         line (unicode)
+
     Returns:
         line (unicode)
     """
     if '@' in line:
         if search(f'{EMAIL_REGEX}(:|;)', line):
             return True, sub(f'{EMAIL_REGEX}(:|;)', '', line)
     return False, line
 
 
 def add_lower(line):
     """Returns if the upper case string is different from the lower case line
 
     Param:
         line (unicode)
+
     Returns:
         False if they are the same
         Lowered string if they are not
     """
     line_lower = line.lower()
     if line != line_lower:
         return line_lower
@@ -239,14 +264,15 @@
 
 
 def add_latin_ligatures(line):
     """Returns the line cleaned of latin ligatures if there are any.
 
     Param:
         line (unicode)
+
     Returns:
         False if there are not any latin ligatures
         Corrected line
     """
     cleaned_line = fix_latin_ligatures(line)
     if line != cleaned_line:
         return cleaned_line
@@ -255,14 +281,15 @@
 
 
 def add_without_punctuation(line, punctuation):
     """Returns the line cleaned of punctuation.
 
     Param:
         line (unicode)
+
     Returns:
         False if there are not any punctuation
         Corrected line
     """
     cleaned_line = line.translate(str.maketrans('', '', punctuation))
 
     if line != cleaned_line:
@@ -272,14 +299,15 @@
 
 
 def clean_add_umlaut(line):
     """Returns the line cleaned of incorrect umlauting
 
     Param:
         line (unicode)
+
     Returns:
         Corrected line
     """
     cleaned_line = line
 
     umlaut_dict = {
         'a"': 'ä',
@@ -304,14 +332,15 @@
 
 def remove_punctuation(line, punctuation):
     """Returns the line without punctuation
 
     Param:
         line (unicode)
         punctuation (unicode)
+
     Returns:
         line without start and end punctuation
     """
     return_line = line.translate(str.maketrans('', '', punctuation))
     if return_line != line:
         return True, return_line
     else:
@@ -319,14 +348,15 @@
 
 
 def remove_strip_punctuation(line, punctuation):
     """Returns the line without start and end punctuation
 
     Param:
         line (unicode)
+
     Returns:
         line without start and end punctuation
     """
     return_line = line.strip(punctuation)
     if return_line != line:
         return True, return_line
     else:
@@ -334,14 +364,15 @@
 
 
 def add_split(line, punctuation=(' ', '-', r'\.')):
     """Split the line on the punctuation and return elements longer then 1 char.
 
     Param:
         line (unicode)
+
     Returns:
         split line
     """
     for p in punctuation:
         if p in line:
             return [i for i in re_split('|'.join(punctuation), line) if len(i) > 1]
     return False
@@ -349,14 +380,15 @@
 
 def check_case(line, ignored_chars=(' ', "'", '-')):
     """Checks if an uppercase line is equal to a lowercase line.
 
     Param:
         line (unicode)
         ignored_chars list(string)
+
     Returns:
         true if uppercase line is equal to uppercase line
     """
     for c in line:
         c = str(c)
         if c.lower() == c.upper():
             if c in ignored_chars:
@@ -369,15 +401,16 @@
 def check_length(line, min=0, max=0):
     """Does a length check on the line
 
     Params:
         line (unicode)
         min (int)
         max (int)
-    Returns
+
+    Returns:
         true if length is ok
     """
     status = True
     if min and status:
         status = len(line) >= min
     if max and status:
         status = len(line) < max
@@ -386,46 +419,64 @@
 
 def check_hash(line):
     """Check if a line contains a hash
 
     Params:
         line (unicode)
 
-    Returns true if line does not contain hash
+    Returns:
+        true if line does not contain hash
     """
     if search(HASH_HEX_REGEX, line):
         if len(line) in [32, 40, 64]:
             return False
     if len(line) > 0:
         if line[0] == '$':
             for hash_regex in HASH_REGEX_LIST:
                 if search(hash_regex, line):
                     return False
     return True
 
 
+def check_mac_address(line):
+    """Check if a line contains a MAC-address
+
+    Params:
+        line (unicode)
+
+    Returns:
+        true if line does not contain a MAC-address
+    """
+    if search(MAC_REGEX, line):
+        return False
+
+    return True
+
+
 def check_email(line):
     """Check if lines contain e-mail addresses with a simple regex
 
     Params:
         line (unicode)
-    Returns
+
+    Returns:
         true is line does not contain email
     """
     if search(EMAIL_REGEX, line):
         return False
     else:
         return True
 
 
 def check_non_ascii(line):
     """Checks if a line contains a non ascii chars
 
     Params:
         line (unicode)
+
     Returns:
         true if line does not contain non ascii chars
     """
     try:
         line.encode('ascii')
         return True
     except UnicodeEncodeError:
@@ -433,31 +484,99 @@
 
 
 def check_character(line, character):
     """Checks if a line contains a specific character
 
     Params:
         line (unicode)
+
     Returns:
         true if line does contain the specific character
 
     """
     if character in line:
         return True
     else:
         return False
 
 
+def check_starting_with(line, strings):
+    """Checks if a line start with a specific strings
+
+    Params:
+        line (unicode)
+        strings[str]
+
+    Returns:
+        true if line does start with one of the strings
+
+    """
+    for string in strings:
+        if line.startswith(string):
+            return True
+    return False
+
+
+def check_uuid(line):
+    """Check if a line contains a UUID
+
+    Params:
+        line (unicode)
+
+    Returns:
+        true if line does not contain a UUID
+    """
+    if search(UUID_REGEX, line):
+        return False
+
+    return True
+
+
+def check_ending_with(line, strings):
+    """Checks if a line ends with specific strings
+
+    Params:
+        line (unicode)
+        strings[str]
+
+    Returns:
+        true if line does end with one of the strings
+
+    """
+    for string in strings:
+        if line.endswith(string):
+            return True
+    return False
+
+
+def check_empty_line(line):
+    """Checks if a line is empty or only contains whitespace chars
+
+    Params:
+        line (unicode)
+
+    Returns:
+        true of line is empty or only contains whitespace chars
+    """
+    if line == '':
+        return True
+    elif line.isspace():
+        return True
+    return False
+
+
 def clean_cut(line, delimiters, fields):
     """Finds the first delimiter and returns the remaining string either after
     or before the delimiter.
+
     Params:
         line (unicode)
         delimiters list(unicode)
         fields (unicode)
+
     Returns:
         line (unicode)
     """
     for delimiter in delimiters:
         if delimiter in line:
             if '-' in fields:
                 start = fields.split('-')[0]
@@ -475,30 +594,49 @@
 
 
 def clean_non_ascii(line):
     """Replace non ascii chars with there ascii representation.
 
     Params:
         line (Unicode)
+
     Returns:
         line (Unicode)
     """
     cleaned_line = unidecode(line)
     if line != cleaned_line:
         return True, cleaned_line
     else:
         return False, line
 
 
+def clean_title_case(line):
+    """Replace words to title word (uppercasing first letter)
+
+    Params:
+        line (Unicode)
+
+    Returns:
+        line (Unicode)
+
+    """
+    cleaned_line = line.title()
+    if line != cleaned_line:
+        return True, cleaned_line
+    else:
+        return False, line
+
+
 def clean_trim(line):
     """Delete leading and trailing character sequences representing a newline
     from beginning end end of line.
 
     Params:
         line (Unicode)
+
     Returns:
         line (Unicode)
     """
     cleaned_line = line
     # Ensure removal of duplicated blocks
     while True:
         has_match = False
@@ -521,14 +659,15 @@
 
 
 def clean_tab(line):
     """Replace tab character with ':' greedy
 
     Params:
         line (bytes)
+
     Returns:
         line (bytes)
     """
     if b'\x09' in line:
         line = sub(b'\x09+', b'\x3a', line)
         return True, line
     else:
@@ -536,29 +675,31 @@
 
 
 def clean_hex(line):
     """Converts strings like '$HEX[]' to proper binary
 
     Params:
         line (bytes)
-    Returns
+
+    Returns:
         line (bytes)
     """
     match = HEX_REGEX.search(line)
     if match:
         return True, unhexlify(match.group(1))
     else:
         return False, line
 
 
 def clean_html(line):
     """Detects html encode chars and decodes them
 
     Params:
         line (Unicode)
+
     Returns:
         line (Unicode)
     """
     return_line = HTML_ENTITY_RE.sub(_unescape_fixup, line)
     if return_line != line:
         return True, return_line
     else:
@@ -566,14 +707,15 @@
 
 
 def clean_html_named(line):
     """Detects named html encode chars and decodes them
 
     Params:
         line (Unicode)
+
     Returns:
         line (Unicode)
     """
     return_line = HTML_ENTITY_RE.sub(_unescape_fixup_named, line)
     if return_line != line:
         return True, return_line
     else:
@@ -581,14 +723,15 @@
 
 
 def clean_newline(line):
     """Delete newline characters at start and end of line
 
     Params:
         line (Unicode)
+
     Returns:
         line (Unicode)
     """
     return_line = line.strip('\r\n')
     if return_line != line:
         return True, return_line
     else:
@@ -596,14 +739,15 @@
 
 
 def check_controlchar(line):
     """Detects control chars, returns True when detected
 
     Params:
         line (Unicode)
+
     Returns:
         Status, String
     """
     for c in line:
         # https://en.wikipedia.org/wiki/Unicode_character_property#General_Category
         # Characters (they have meaning):
         # Cc -> Control Char (End of stream)
@@ -613,20 +757,40 @@
         # Co -> Private use
         # Cs -> Surrogate
         if category(c) in ['Cc', 'Cf', 'Cn', 'Co', 'Cs']:
             return True, c
     return False, None
 
 
+def check_regex(line, regex):
+    """Checks if a line matches a list of regexes
+
+    Params:
+        line (unicode)
+        regex (list)
+
+    Returns:
+        true if all regexes match
+        false if line does not match regex
+    """
+    for regex in regex:
+        if search(regex, line):
+            continue
+        else:
+            return False
+    return True
+
+
 def try_encoding(line, encoding):
     """Tries to decode a line using supplied encoding
 
     Params:
         line (Byte): byte variable that will be decoded
         encoding (string): the encoding to be tried
+
     Returns:
         False if decoding failed
         String if decoding worked
     """
     try:
         # Try to decode the line
         line_decoded = line.decode(encoding)
@@ -646,14 +810,15 @@
 def clean_mojibake(line):
     """Detects mojibake and tries to correct it.
     Mojibake are string that are decoded incorrectly and then encoded incorrectly.
     This results in strings like: Ãºnico which should be único.
 
     Param:
         line (str)
+
     Returns:
         Cleaned string
     """
     return_line = fix_encoding(line)
     if return_line != line:
         return True, return_line
     else:
@@ -661,14 +826,15 @@
 
 
 def clean_encode(line, input_encoding):
     """Detects and tries encoding
 
     Params:
         line (bytes)
+
     Returns:
         Decoded UTF-8 string
     """
     # Try either a user set of encodings or the default encoding set.
     # When using multiple encoding is it beter to have multibyte encodings before
     # Single byte encodings. Also it is beter to not include iso encoding by default.
     # https://en.wikipedia.org/wiki/Character_encoding#Common_character_encodings
@@ -733,15 +899,14 @@
         if config['verbose']:
             log.append(f'----BEGIN---- {hexlify(line)}{linesep}')
         # Replace tab chars as ':' greedy
         if config.get('tab') and not stop:
             status, line = clean_tab(line)
             if status and config['verbose']:
                 log.append(f'Clean_tab; replaced tab characters; {line}{linesep}')
-
         # Converting enoding to UTF-8
         if config.get('encode') and not stop:
             status, line_decoded = clean_encode(line, config.get('input_encoding'))
             if status is False:
                 log.append(f'Clean_encode; decoding error with {line_decoded}; {line}{linesep}')
                 stop = True
             elif status is True and config['verbose']:
@@ -827,14 +992,20 @@
 
         # Replace non-ascii
         if config.get('non-ascii') and not stop:
             status, line_decoded = clean_non_ascii(line_decoded)
             if status and config['verbose']:
                 log.append(f'Clean_non_ascii; non-ascii replaced; {line_decoded}{linesep}')
 
+        # Replace first letter of a word to a uppercase letter
+        if config.get('title-case') and not stop:
+            status, line_decoded = clean_title_case(line_decoded)
+            if status and config['verbose']:
+                log.append(f'Clean_title_case; non-ascii replaced; {line_decoded}{linesep}')
+
         # Should we remove emails?
         if config.get('remove-email') and not stop:
             status, line_decoded = remove_email(line_decoded)
             if status and config['verbose']:
                 log.append(f'Remove_email; email found; {line_decoded}{linesep}')
 
         if config.get('googlengram') and not stop:
@@ -859,24 +1030,57 @@
                 stop = True
 
         if config.get('check-hash') and not stop:
             if not check_hash(line_decoded):
                 log.append(f'Check_hash; dropped line because found a hash; {line_decoded}{linesep}')
                 stop = True
 
+        if config.get('check-mac-address') and not stop:
+            if not check_mac_address(line_decoded):
+                log.append(f'Check_mac_address; dropped line because found a MAC address; {line_decoded}{linesep}')
+                stop = True
+
         if config.get('check-non-ascii') and not stop:
             if not check_non_ascii(line_decoded):
                 log.append(f'Check_non_ascii; dropped line because non ascii char found; {line_decoded}{linesep}')
                 stop = True
 
         if config.get('check-replacement-character') and not stop:
             if check_character(line_decoded, '�'):
                 log.append(f'Check_replacement_character; dropped line because "�" found; {line_decoded}{linesep}')
                 stop = True
 
+        if config.get('check-regex') and not stop:
+            if not check_regex(line_decoded, config.get('check-regex')):
+                log.append(f'Check_regex; dropped line because it does not match the regex; {line_decoded}{linesep}')
+                stop = True
+
+        if config.get('check-starting-with') and not stop:
+            to_check = config.get("check-starting-with")
+            if check_starting_with(line_decoded, to_check):
+                log.append(f'Check_starting_with; dropped line because {to_check} found; {line_decoded}{linesep}')
+                stop = True
+
+        if config.get('check-uuid') and not stop:
+            if not check_uuid(line_decoded):
+                log.append(f'Check_uuid; dropped line because found a uuid; {line_decoded}{linesep}')
+                stop = True
+
+        if config.get('check-ending-with') and not stop:
+            to_check = config.get("check-ending-with")
+            if check_ending_with(line_decoded, to_check):
+                log.append(f'Check_ending_with; dropped line because {to_check} found; {line_decoded}{linesep}')
+                stop = True
+
+        if config.get('check-empty-line') and not stop:
+            if check_empty_line(line_decoded):
+                log_line = "Check_empty_line; dropped line because is empty or only contains whitespace;"
+                log.append(f'{log_line} {line_decoded}{linesep}')
+                stop = True
+
         if config.get('remove-punctuation') and not stop:
             status, line_decoded = remove_punctuation(line_decoded, config.get('punctuation'))
             if status and config['verbose']:
                 log.append(f'Remove_punctuation; stripped punctuation; {line_decoded}{linesep}')
 
         if config.get('remove-strip-punctuation') and not stop:
             status, line_decoded = remove_strip_punctuation(line_decoded, config.get('punctuation'))
@@ -954,14 +1158,16 @@
     # based on: https://www.blopig.com/blog/2016/08/processing-large-files-using-python/
     for filename in tqdm(glob(fname, recursive=True), desc='Chunkify', mininterval=0.1, unit='files',
                          disable=not config.get('progress')):
         if not path.isfile(filename):
             continue
         fileend = path.getsize(filename)
         with open(filename, 'br') as f:
+            for x in range(0, config.get('skip')):
+                f.readline()
             chunkend = f.tell()
             while True:
                 chunkstart = chunkend
                 f.seek(size, 1)
                 f.readline()
                 chunkend = f.tell()
                 yield chunkstart, chunkend - chunkstart, filename
@@ -1001,37 +1207,45 @@
         'input_encoding': ['UTF-8'],
         'cut': False,
         'delimiter': ':',
         'cut-fields': '2-',
         'verbose': False,
         'progress': False,
         'limit': False,
+        'skip': False,
 
         # Modify
-        'encode': True,
-        'mojibake': True,
-        'tab': True,
-        'trim': True,
-        'newline': True,
+        'encode': False,
+        'mojibake': False,
+        'tab': False,
+        'trim': False,
+        'newline': False,
         'hex': False,
         'html': False,
         'html-named': False,
         'umlaut': False,
         'non-ascii': False,
+        'title_case': False,
 
         # Check
         'length': False,
         'check-min-length': 0,
         'check-max-length': 0,
-        'check-controlchar': True,
+        'check-controlchar': False,
         'check-case': False,
         'check-email': False,
         'check-hash': False,
+        'check-mac-address': False,
         'check-non-ascii': False,
         'check-replacement-character': False,
+        'check-starting-with': False,
+        'check-uuid': False,
+        'check-ending-with': False,
+        'check-empty-line': False,
+        'check-regex': False,
 
         # Add
         'add-lower': False,
         'add-latin-ligatures': False,
         'add-split': False,
         'add-umlaut': False,
         'add-without-punctuation': False,
@@ -1048,14 +1262,17 @@
 
     if arguments.get('--progress'):
         config['progress'] = True
 
     if arguments.get('--limit'):
         config['limit'] = int(arguments.get('--limit'))
 
+    if arguments.get('--skip'):
+        config['skip'] = int(arguments.get('--skip'))
+
     if arguments.get('--input-encoding'):
         config['input_encoding'] = arguments.get('--input-encoding').split(',')
 
     if arguments.get('--output-encoding'):
         setlocale(LC_ALL, arguments.get('--output-encoding'))
     else:
         setlocale(LC_ALL, 'en_US.UTF-8')
@@ -1093,14 +1310,32 @@
 
     if arguments.get('--umlaut'):
         config['umlaut'] = True
 
     if arguments.get('--non-ascii'):
         config['non-ascii'] = True
 
+    if arguments.get('--title-case'):
+        config['title-case'] = True
+
+    if arguments.get('--mojibake'):
+        config['mojibake'] = True
+
+    if arguments.get('--encode'):
+        config['encode'] = True
+
+    if arguments.get('--tab'):
+        config['tab'] = True
+
+    if arguments.get('--newline'):
+        config['newline'] = True
+
+    if arguments.get('--trim'):
+        config['trim'] = True
+
     # Check modules
     if arguments.get('--check-min-length'):
         config['check-length'] = True
         config['check-min-length'] = int(arguments.get('--check-min-length'))
 
     if arguments.get('--check-max-length'):
         config['check-length'] = True
@@ -1111,20 +1346,47 @@
 
     if arguments.get('--check-email'):
         config['check-email'] = True
 
     if arguments.get('--check-hash'):
         config['check-hash'] = True
 
+    if arguments.get('--check-mac-address'):
+        config['check-mac-address'] = True
+
     if arguments.get('--check-non-ascii'):
         config['check-non-ascii'] = True
 
     if arguments.get('--check-replacement-character'):
         config['check-replacement-character'] = True
 
+    if arguments.get('--check-starting-with'):
+        if ',' in arguments.get('--check-starting-with'):
+            config['check-starting-with'] = arguments.get('--check-starting-with').split(',')
+        else:
+            config['check-starting-with'] = [arguments.get('--check-starting-with')]
+
+    if arguments.get('--check-uuid'):
+        config['check-uuid'] = True
+
+    if arguments.get('--check-ending-with'):
+        if ',' in arguments.get('--check-ending-with'):
+            config['check-ending-with'] = arguments.get('--check-ending-with').split(',')
+        else:
+            config['check-ending-with'] = [arguments.get('--check-ending-with')]
+
+    if arguments.get('--check-empty-line'):
+        config['check-empty-line'] = True
+
+    if arguments.get('--check-controlchar'):
+        config['check-controlchar'] = True
+
+    if arguments.get('--check-regex'):
+        config['check-regex'] = arguments.get('--check-regex').split(',')
+
     # Add modules
     if arguments.get('--add-lower'):
         config['add-lower'] = True
 
     if arguments.get('--add-latin-ligatures'):
         config['add-latin-ligatures'] = True
 
@@ -1143,44 +1405,52 @@
 
     if arguments.get('--remove-email'):
         config['remove-email'] = True
 
     if arguments.get('--remove-punctuation'):
         config['remove-punctuation'] = True
 
-    # Negative modules
-    # Test if there are any disable functions, they must always overrule any other option.
-    if arguments.get('--no-mojibake'):
-        config['mojibake'] = False
-
-    if arguments.get('--no-encode'):
-        config['encode'] = False
-
-    if arguments.get('--no-check-controlchar'):
-        config['check-controlchar'] = False
-
-    if arguments.get('--no-tab'):
-        config['tab'] = False
-
-    if arguments.get('--no-newline'):
-        config['newline'] = False
-
-    if arguments.get('--no-trim'):
-        config['trim'] = False
-
     # Some meta-modules, those overwrite settings
     if arguments.get('--googlengram'):
         config['cut'] = False
         config['remove-email'] = False
         config['encode'] = True
         config['mojibake'] = False
         config['check-controlchar'] = False
         config['tab'] = False
         config['googlengram'] = True
 
+    # Meta-module for leak files. Set the following defaults:
+    # mojibake, encode, newline, check-controlchar
+    if arguments.get('--leak'):
+        config['mojibake'] = True
+        config['encode'] = True
+        config['newline'] = True
+        config['check-controlchar'] = True
+
+    # Meta-module for leak fils, but more modules. Set the following defaults:
+    # --mojibake, --encode, --newline, --check-controlchar,
+    # --hex, --html, --html-named,
+    # --check-hash, --check-mac-address, --check-uuid, --check-email,
+    # --check-replacement-character, --check-empty-line
+    if arguments.get('--leak-full'):
+        config['mojibake'] = False
+        config['encode'] = True
+        config['newline'] = True
+        config['check-controlchar'] = True
+        config['hex'] = True
+        config['html'] = True
+        config['html-named'] = True
+        config['check-hash'] = True
+        config['check-mac-address'] = True
+        config['check-uuid'] = True
+        config['check-email'] = True
+        config['check-replacement-character'] = True
+        config['check-empty-line'] = True
+
     print(f'Main: running demeuk - {version}')
     if path.isdir('demeuk_tmp'):
         rmtree('demeuk_tmp')
     mkdir('demeuk_tmp')
 
     pool = Pool(a_threads)
     jobs = []
```

### Comparing `demeuk-3.9.7/demeuk.egg-info/PKG-INFO` & `demeuk-4.0.1/demeuk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: demeuk
-Version: 3.9.7
+Version: 4.0.1
 Summary: CLI tool to remove invalid chars from a corpus.
 Home-page: https://github.com/NetherlandsForensicInstitute/demeuk
 Author: Netherlands Forensic Institute
 Author-email: holmesnl@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -56,14 +54,14 @@
 
 Now you can run bin/demeuk.py:
 
 Examples:
 ```
     demeuk -i inputfile.tmp -o outputfile.dict -l droppedfile.txt
     demeuk -i inputfile -o outputfile -j 24 -l logfile.log
+    demeuk -i inputfile.tmp -o outputfile.dict -l droppedfile.txt --leak
+    demeuk -i inputfile -o outputfile -j 24 -l logfile.log --leak-full
     demeuk -i inputdir/*.txt -o outputfile.dict -l logfile.log
 ```
 
 ## Docs
 The docs are available at: <http://demeuk.rtfd.io/>
-
-
```

### Comparing `demeuk-3.9.7/setup.py` & `demeuk-4.0.1/setup.py`

 * *Files identical despite different names*

