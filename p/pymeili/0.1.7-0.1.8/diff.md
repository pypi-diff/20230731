# Comparing `tmp/pymeili-0.1.7.tar.gz` & `tmp/pymeili-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.1.7.tar", last modified: Thu Jul 27 15:38:59 2023, max compression
+gzip compressed data, was "pymeili-0.1.8.tar", last modified: Mon Jul 31 00:47:09 2023, max compression
```

## Comparing `pymeili-0.1.7.tar` & `pymeili-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.843371 pymeili-0.1.7/
--rw-rw-rw-   0        0        0      433 2023-07-27 13:09:18.000000 pymeili-0.1.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.7/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1627 2023-07-27 15:38:59.843371 pymeili-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-07-27 13:10:18.000000 pymeili-0.1.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.813415 pymeili-0.1.7/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.841376 pymeili-0.1.7/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.7/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.7/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.7/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      785 2023-07-27 13:08:56.000000 pymeili-0.1.7/pymeili/__init__.py
--rw-rw-rw-   0        0        0    60827 2023-07-27 15:38:43.000000 pymeili-0.1.7/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.828442 pymeili-0.1.7/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1627 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 15:38:59.843371 pymeili-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-07-27 13:09:50.000000 pymeili-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:47:09.993783 pymeili-0.1.8/
+-rw-rw-rw-   0        0        0      501 2023-07-31 00:47:02.000000 pymeili-0.1.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.8/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1695 2023-07-31 00:47:09.992786 pymeili-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-07-27 13:10:18.000000 pymeili-0.1.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 00:47:09.978824 pymeili-0.1.8/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-31 00:47:09.991788 pymeili-0.1.8/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.8/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.8/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.8/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      785 2023-07-31 00:46:21.000000 pymeili-0.1.8/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    63530 2023-07-31 00:45:09.000000 pymeili-0.1.8/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:47:09.988796 pymeili-0.1.8/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1695 2023-07-31 00:47:09.000000 pymeili-0.1.8/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-31 00:47:09.000000 pymeili-0.1.8/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 00:47:09.000000 pymeili-0.1.8/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 00:47:09.000000 pymeili-0.1.8/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 00:47:09.993783 pymeili-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-31 00:46:20.000000 pymeili-0.1.8/setup.py
```

### Comparing `pymeili-0.1.7/LISCENCE.txt` & `pymeili-0.1.8/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.7/PKG-INFO` & `pymeili-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.7
+Version: 0.1.8
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -50,7 +50,10 @@
 - Add Basic Basemap Function, fix some problems
 
 0.1.6 (27/07/2023)
 - Fix Some Problems, add common raise function
 
 0.1.7 (27/07/2023)
 - Fix Some Minor Problems
+
+0.1.8 (31/07/2023)
+- Fix Some Minor Problems, add new cmap '35'
```

### Comparing `pymeili-0.1.7/README.txt` & `pymeili-0.1.8/README.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.7/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.8/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.7/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.8/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.7/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.8/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.7/pymeili/__init__.py` & `pymeili-0.1.8/pymeili/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     fill_between, fill_betweenx,
     pause, normalize, adjust, addaxes, slider, set_xydata,
     figsize, show, clf, close, figure, savefig,
     imread, imshow, imsave,
     
 )
 
-__version__: str = '0.1.7'
+__version__: str = '0.1.8'
```

### Comparing `pymeili-0.1.7/pymeili/beautifyplot.py` & `pymeili-0.1.8/pymeili/beautifyplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 
 
 # METHOD I
 # 獲取當前檔案位址
 currentfilepath = __file__
 
 # 刪去__file__中最後面自"\"開始的字串(刪除檔名)
-motherpath = currentfilepath[:-len(currentfilepath.split('\\')[-1])]
+motherpath = currentfilepath[:-len(currentfilepath.split('/')[-1])]
+
+# /work/home/L.Yen-Ting-Chou/pymeili/FONT/Futura Extra Black font.ttf
+
 try:
-    fontpath = Path(mpl.get_data_path(), motherpath+"\\futura medium bt.ttf")
-    fontpath_bold = Path(mpl.get_data_path(), motherpath+"\Futura Heavy font.ttf")
-    fontpath_black = Path(mpl.get_data_path(), motherpath+"\Futura Extra Black font.ttf")
+    fontpath = Path(mpl.get_data_path(), motherpath+"FONT/futura medium bt.ttf")
+    fontpath_bold = Path(mpl.get_data_path(), motherpath+"FONT/Futura Heavy font.ttf")
+    fontpath_black = Path(mpl.get_data_path(), motherpath+"FONT/Futura Extra Black font.ttf")
 except: # 未安裝字體
     try:
         # 退而求其次，使用預設字體
         fontpath = 'C:\Windows\Fonts\Arial.ttf'
         fontpath_bold = 'C:\Windows\Fonts\Arial Bold.ttf'
         fontpath_black = 'C:\Windows\Fonts\Arial Black.ttf'
         print(bcolors.WARNING+'Please install Futura fonts in the same directory as this file.\ninstall font-packages: https://dwl.freefontsfamily.com/download/futura/;\n Moving the font file to installed module folder(e.g."C:>Users>Username>AppData>Local>Programs>Python>Python311>Lib>site-packages>pymeili").\n Currently using system default font: Arial'+bcolors.ENDC)
@@ -160,14 +163,33 @@
                     return LinearSegmentedColormap.from_list('mycmap', ['#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
                 if index == '-24':
                     return LinearSegmentedColormap.from_list('mycmap', ['#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
                 if index == '-23':
                     return LinearSegmentedColormap.from_list('mycmap', ['#F1C9B4','#F2CABF','#EEEEEE'])
                 if index == '-22':
                     return LinearSegmentedColormap.from_list('mycmap', ['#F2CABF','#EEEEEE'])
+                
+                if index == '35':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
+                if index == '34':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
+                if index == '33':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#D5EDD5','#AB503B'])
+                if index == '32':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#47A7DE','#E08A16'])
+                
+                if index == '-35': # reversed 1
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#D5EDD5','#47A7DE','#454FB4'])
+                if index == '-34': # reversed 1 but 4 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#47A7DE','#454FB4'])
+                if index == '-33': # reversed 1 but 3 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#D5EDD5','#454FB4'])
+                if index == '-32': # reversed 1 but 2 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#E08A16','#47A7DE'])
+                
             
             
             elif theme == 'dark_background':
                 if index == '15':
                     return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
                 if index == '14':
                     return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
@@ -210,14 +232,32 @@
                     return LinearSegmentedColormap.from_list('mycmap', ['#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
                 if index == '-24':
                     return LinearSegmentedColormap.from_list('mycmap', ['#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
                 if index == '-23':
                     return LinearSegmentedColormap.from_list('mycmap', ['#F1C9B4','#F2CABF','#EEEEEE'])
                 if index == '-22':
                     return LinearSegmentedColormap.from_list('mycmap', ['#F2CABF','#EEEEEE'])
+                
+                if index == '35':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
+                if index == '34':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
+                if index == '33':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#D5EDD5','#AB503B'])
+                if index == '32':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#47A7DE','#E08A16'])
+                
+                if index == '-35': # reversed 1
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#D5EDD5','#47A7DE','#454FB4'])
+                if index == '-34': # reversed 1 but 4 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#47A7DE','#454FB4'])
+                if index == '-33': # reversed 1 but 3 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#D5EDD5','#454FB4'])
+                if index == '-32': # reversed 1 but 2 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#E08A16','#47A7DE'])
         except: # NameError: name 'theme' is not defined
             raise Exception(bcolors.WARNING+'Please run initplot() first.'+bcolors.ENDC)
     else: 
         return index
 
 # LABEL設定
 '''
@@ -324,15 +364,15 @@
     if clabel == True:
         CL = CS.clabel(fontsize=8, colors=colorlist(color), inline=True)
     plt.contourf(x, y, z, cmap=cmaplist(cmap), vmin=vmin, vmax=vmax, levels=levels, **kwargs)
 
 
 
 # colorbar顯示
-def colorbar(ticks='auto',label=' ', orientation='vertical',shrink=0.95, aspect=20, fraction=0.046, pad=0.04, labelfontsize=16, font=fontpath, color='fg', extebd='neither',**kwargs):
+def colorbar(ticks='auto',label=' ', orientation='vertical',shrink=0.95, aspect=20, fraction=0.046, pad=0.04, labelfontsize=16, font=fontpath, color='fg', extend='neither',**kwargs):
     if orientation == 'v' or 'V':
         orientation = 'vertical'
     elif orientation == 'h' or 'H':
         orientation = 'horizontal'
     if ticks == 'auto':
         import numpy as np
         ticks = []
@@ -811,24 +851,24 @@
         self.basemap.drawmeridians(meridians, fontsize=fontsize, color=colorlist(color), linewidth=linewidth, **kwargs)
 
 
 
 
 
     # 繪製海岸線
-    def drawcoastlines(self, linewidth=3, color='fg', **kwargs):
+    def drawcoastlines(self, linewidth=2, color='fg', **kwargs):
         self.basemap.drawcoastlines(linewidth=linewidth, color=colorlist(color), **kwargs)
     # 繪製國家
-    def drawcountries(self, linewidth=2, color='fg', **kwargs):
+    def drawcountries(self, linewidth=1, color='fg', **kwargs):
         self.basemap.drawcountries(linewidth=linewidth, color=colorlist(color), **kwargs)
     # 繪製州界
-    def drawstates(self, linewidth=1, color='fg', **kwargs):
+    def drawstates(self, linewidth=0.5, color='fg', **kwargs):
         self.basemap.drawstates(linewidth=linewidth, color=colorlist(color), **kwargs)
     # 繪製河流
-    def drawrivers(self, linewidth=1, color='bg', **kwargs):
+    def drawrivers(self, linewidth=0.3, color='bg', **kwargs):
         self.basemap.drawrivers(linewidth=linewidth, color=colorlist(color), **kwargs)
     # 繪製海陸mask
     def drawlsmask(self, land_color='rfg', ocean_color='bg', lakes=True, resolution='l', grid=5, **kwargs):
         self.basemap.drawlsmask(land_color=colorlist(land_color), ocean_color=colorlist(ocean_color), lakes=lakes, resolution=resolution, grid=grid, **kwargs)
     # 繪製陰影浮雕
     def shadedrelief(self, alpha=1, **kwargs):
         self.basemap.shadedrelief(alpha=alpha, **kwargs)
@@ -886,14 +926,15 @@
         if roundedge == False:
             LG.get_frame().set_boxstyle('Round', pad=0.2, rounding_size=-0.01)
         LG.get_frame().set_linewidth(edgewidth)
     # 繪製文字
     def text(self, x, y, text, color='fg', font=fontpath, fontsize=20, **kwargs):
         self.basemap.text(x, y, text, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize), **kwargs)
 
+
     
 
 
 # subplot系列
 class initsubplots():
     def __init__(self, nrows=1, ncols=1, figsize=(8,10), style='default', background=True, **kwargs):
         self.row = 0 # 標示子圖的目標列
@@ -1122,7 +1163,11 @@
 
 
 
 
     
 
 
+
+    
+
+
```

### Comparing `pymeili-0.1.7/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.8/pymeili.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.7
+Version: 0.1.8
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -50,7 +50,10 @@
 - Add Basic Basemap Function, fix some problems
 
 0.1.6 (27/07/2023)
 - Fix Some Problems, add common raise function
 
 0.1.7 (27/07/2023)
 - Fix Some Minor Problems
+
+0.1.8 (31/07/2023)
+- Fix Some Minor Problems, add new cmap '35'
```

### Comparing `pymeili-0.1.7/setup.py` & `pymeili-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.1.7',
+    version='0.1.8',
     description='a module to beautify your python plot.',
     long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

