# Comparing `tmp/cocoa-vanilla-0.3.0.tar.gz` & `tmp/cocoa-vanilla-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoa-vanilla-0.3.0.tar", last modified: Sat Mar  4 16:20:30 2023, max compression
+gzip compressed data, was "cocoa-vanilla-0.4.0.tar", last modified: Mon Jul 31 14:20:24 2023, max compression
```

## Comparing `cocoa-vanilla-0.3.0.tar` & `cocoa-vanilla-0.4.0.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.524304 cocoa-vanilla-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.492304 cocoa-vanilla-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.500304 cocoa-vanilla-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.500304 cocoa-vanilla-0.3.0/Data/
--rw-r--r--   0 runner    (1001) docker     (123)    19604 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Data/testIcon.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.496304 cocoa-vanilla-0.3.0/Demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.500304 cocoa-vanilla-0.3.0/Demos/SimpleApp/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/SimpleApp/ReadMe.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.492304 cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.500304 cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.500304 cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/designable.nib
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib.zip
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/SimpleApp/SimpleApp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/SimpleApp/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.504304 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.496304 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.496304 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.504304 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/TinyTextEditor.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Demos/TinyTextEditor/tinyTextEditorDocumentWindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.504304 cocoa-vanilla-0.3.0/Documentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.504304 cocoa-vanilla-0.3.0/Documentation/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.512304 cocoa-vanilla-0.3.0/Documentation/source/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ActionButton.png
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Box.png
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Button.png
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/CheckBox.png
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/CheckBoxListCell.png
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ColorWell.png
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ComboBox.png
--rw-r--r--   0 runner    (1001) docker     (123)   263854 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/DatePicker.png
--rw-r--r--   0 runner    (1001) docker     (123)    20931 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Drawer.png
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/EditText.png
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/FloatingWindow.png
--rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/GradientButton.png
--rw-r--r--   0 runner    (1001) docker     (123)   101511 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/GridView.png
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/HUDFloatingWindow.png
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/HelpButton.png
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/HorizontalLine.png
--rw-r--r--   0 runner    (1001) docker     (123)    86315 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/HorizontalStackView.png
--rw-r--r--   0 runner    (1001) docker     (123)    24650 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ImageButton.png
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ImageListCell.png
--rw-r--r--   0 runner    (1001) docker     (123)    26002 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ImageView.png
--rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/LevelIndicator.png
--rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/LevelIndicatorListCell.png
--rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/List.png
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ListMulticolumn.png
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/PopUpButton.png
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/PopUpButtonListCell.png
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Popover.png
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ProgressBar.png
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ProgressSpinner.png
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/RadioGroup.png
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/ScrollView.png
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SearchBox.png
--rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SecureEditText.png
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SegmentedButton.png
--rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SegmentedButtonListCell.png
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Sheet.png
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Slider.png
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SliderListCell.png
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SplitView.png
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/SquareButton.png
--rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Tabs.png
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/TextBox.png
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/TextEditor.png
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/VerticalLine.png
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/VerticalRadioGroup.png
--rw-r--r--   0 runner    (1001) docker     (123)   106358 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/VerticalStackView.png
--rw-r--r--   0 runner    (1001) docker     (123)    17150 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/_images/Window.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.512304 cocoa-vanilla-0.3.0/Documentation/source/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/concepts/positioning.rst
--rw-r--r--   0 runner    (1001) docker     (123)   140639 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.516304 cocoa-vanilla-0.3.0/Documentation/source/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ActionButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Box.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Button.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/CheckBox.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ColorWell.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ComboBox.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/DatePicker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Drawer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/EditText.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/FloatingWindow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/GradientButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/GridView.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Group.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/HelpButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/HorizontalLine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/HorizontalStackView.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ImageButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ImageView.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/LevelIndicator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/List.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/List2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/PopUpButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Popover.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ProgressBar.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ProgressSpinner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/RadioGroup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/ScrollView.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/SearchBox.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/SecureEditText.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/SegmentedButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Sheet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Slider.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/SplitView.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/SquareButton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Tabs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/TextBox.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/TextEditor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/VerticalLine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/VerticalStackView.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Documentation/source/objects/Window.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Install.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.496304 cocoa-vanilla-0.3.0/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.516304 cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-04 16:20:30.000000 cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-03-04 16:20:30.000000 cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 16:20:30.000000 cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-04 16:20:30.000000 cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-04 16:20:30.000000 cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.520304 cocoa-vanilla-0.3.0/Lib/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-04 16:20:30.000000 cocoa-vanilla-0.3.0/Lib/vanilla/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/dragAndDrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.520304 cocoa-vanilla-0.3.0/Lib/vanilla/externalFrameworks/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/externalFrameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/nsSubclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/py23.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.524304 cocoa-vanilla-0.3.0/Lib/vanilla/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:30.524304 cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/groupRows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testAll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testDialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testDragAndDrop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testGeometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testGridView.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testSplitview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testStackView.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/test/testWindowBindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaBrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaButton.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaCheckBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaColorWell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaComboBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaDatePicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaDrawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaEditText.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaGradientButton.py
--rw-r--r--   0 runner    (1001) docker     (123)    19371 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaGridView.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaImageView.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaLevelIndicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    66426 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaList.py
--rw-r--r--   0 runner    (1001) docker     (123)    49786 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaList2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaPathControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaPopUpButton.py
--rw-r--r--   0 runner    (1001) docker     (123)    14757 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaPopover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaProgressSpinner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaRadioGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaScrollView.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSearchBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSegmentedButton.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSlider.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25434 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSplitView.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaStackGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaStackView.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaStepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaTabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaTextBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaTextEditor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/Lib/vanilla/vanillaWindows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-04 16:20:30.524304 cocoa-vanilla-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/RELEASE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/ToDo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 16:20:30.524304 cocoa-vanilla-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-04 16:20:15.000000 cocoa-vanilla-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Data/
+-rw-r--r--   0 runner    (1001) docker     (123)    19604 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Data/testIcon.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/SimpleApp/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/SimpleApp/ReadMe.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/designable.nib
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/SimpleApp/SimpleApp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/SimpleApp/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/TinyTextEditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Demos/TinyTextEditor/tinyTextEditorDocumentWindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Documentation/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.357831 cocoa-vanilla-0.4.0/Documentation/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ActionButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Box.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Button.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/CheckBox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/CheckBoxListCell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ColorWell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ComboBox.png
+-rw-r--r--   0 runner    (1001) docker     (123)   263854 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/DatePicker.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20931 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Drawer.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/EditText.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/FloatingWindow.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/GradientButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)   101511 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/GridView.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/HUDFloatingWindow.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/HelpButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/HorizontalLine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86315 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/HorizontalStackView.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24650 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ImageButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ImageListCell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26002 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ImageView.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/LevelIndicator.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/LevelIndicatorListCell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/List.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ListMulticolumn.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/PopUpButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/PopUpButtonListCell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Popover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ProgressBar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ProgressSpinner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/RadioGroup.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/ScrollView.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SearchBox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SecureEditText.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SegmentedButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SegmentedButtonListCell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Sheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Slider.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SliderListCell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SplitView.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/SquareButton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Tabs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/TextBox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/TextEditor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/VerticalLine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/VerticalRadioGroup.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106358 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/VerticalStackView.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17150 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/_images/Window.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.357831 cocoa-vanilla-0.4.0/Documentation/source/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/concepts/positioning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   140639 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.361831 cocoa-vanilla-0.4.0/Documentation/source/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ActionButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Box.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Button.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/CheckBox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ColorWell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ComboBox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/DatePicker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Drawer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/EditText.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/FloatingWindow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/GradientButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/GridView.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Group.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/HelpButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/HorizontalLine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/HorizontalStackView.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ImageButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ImageView.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/LevelIndicator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/List.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/List2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/PopUpButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Popover.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ProgressBar.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ProgressSpinner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/RadioGroup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/ScrollView.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/SearchBox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/SecureEditText.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/SegmentedButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Sheet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Slider.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/SplitView.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/SquareButton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Tabs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/TextBox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/TextEditor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/VerticalLine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/VerticalStackView.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Documentation/source/objects/Window.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Install.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.349831 cocoa-vanilla-0.4.0/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.361831 cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-31 14:20:24.000000 cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-31 14:20:24.000000 cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:20:24.000000 cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 14:20:24.000000 cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:20:24.000000 cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/Lib/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 14:20:24.000000 cocoa-vanilla-0.4.0/Lib/vanilla/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/dragAndDrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/Lib/vanilla/externalFrameworks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/externalFrameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/nsSubclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/py23.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/Lib/vanilla/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/groupRows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testAll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testDialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testDragAndDrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testGeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testGridView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testSplitview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testStackView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/test/testWindowBindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaBrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaCheckBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaColorWell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaComboBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaDatePicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaDrawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaEditText.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaGradientButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19371 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaGridView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaImageView.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaLevelIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66242 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50356 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaList2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaPathControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaPopUpButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaPopover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaProgressSpinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaRadioGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaScrollView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSearchBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSegmentedButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSlider.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25336 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSplitView.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaStackGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaStackView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaStepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaTabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaTextBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaTextEditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51278 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/Lib/vanilla/vanillaWindows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/RELEASE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/ToDo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:20:24.365831 cocoa-vanilla-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-31 14:20:10.000000 cocoa-vanilla-0.4.0/setup.py
```

### Comparing `cocoa-vanilla-0.3.0/.github/workflows/publish.yml` & `cocoa-vanilla-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Data/testIcon.tif` & `cocoa-vanilla-0.4.0/Data/testIcon.tif`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/designable.nib` & `cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/designable.nib`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/keyedobjects.nib` & `cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib.zip` & `cocoa-vanilla-0.4.0/Demos/SimpleApp/Resources/English.lproj/MainMenu.nib.zip`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/SimpleApp/SimpleApp.py` & `cocoa-vanilla-0.4.0/Demos/SimpleApp/SimpleApp.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/info.nib` & `cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/keyedobjects.nib` & `cocoa-vanilla-0.4.0/Demos/TinyTextEditor/Resources/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Demos/TinyTextEditor/TinyTextEditor.py` & `cocoa-vanilla-0.4.0/Demos/TinyTextEditor/TinyTextEditor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from AppKit import NSDocument
 from PyObjCTools import AppHelper
 from tinyTextEditorDocumentWindow import TinyTextEditorDocumentWindow
 from io import open
+from objc import super
 
 
 class TinyTextEditorDocument(NSDocument):
-    
+
     def init(self):
-        self = super(TinyTextEditorDocument, self).init()
+        self = super().init()
         self.vanillaWindowController = TinyTextEditorDocumentWindow()
         self.vanillaWindowController.assignToDocument(self)
-        return self        
-    
+        return self
+
     def readFromFile_ofType_(self, path, tp):
         # refer to the NSDocument reference for information about this method
         f = open(path, 'r', encoding='utf-8')
         text = f.read()
         f.close()
         self.vanillaWindowController.setText(text)
         return True
-    
+
     def writeWithBackupToFile_ofType_saveOperation_(self, fileName, fileType, operation):
         # refer to the NSDocument reference for information about this method
         text = self.vanillaWindowController.getText()
         f = open(fileName, 'w', encoding='utf-8')
         f.write(text)
         f.close()
         return True
```

### Comparing `cocoa-vanilla-0.3.0/Demos/TinyTextEditor/setup.py` & `cocoa-vanilla-0.4.0/Demos/TinyTextEditor/setup.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/Makefile` & `cocoa-vanilla-0.4.0/Documentation/Makefile`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ActionButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ActionButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Box.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Box.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Button.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Button.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/CheckBox.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/CheckBox.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/CheckBoxListCell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/CheckBoxListCell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ColorWell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ColorWell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ComboBox.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ComboBox.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/DatePicker.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/DatePicker.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Drawer.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Drawer.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/EditText.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/EditText.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/FloatingWindow.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/FloatingWindow.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/GradientButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/GradientButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/GridView.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/GridView.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Group.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Group.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/HUDFloatingWindow.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/HUDFloatingWindow.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/HelpButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/HelpButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/HorizontalLine.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/HorizontalLine.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/HorizontalStackView.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/HorizontalStackView.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ImageButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ImageButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ImageListCell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ImageListCell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ImageView.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ImageView.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/LevelIndicator.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/LevelIndicator.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/LevelIndicatorListCell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/LevelIndicatorListCell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/List.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/List.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ListMulticolumn.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ListMulticolumn.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/PopUpButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/PopUpButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/PopUpButtonListCell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/PopUpButtonListCell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Popover.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Popover.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ProgressBar.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ProgressBar.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ProgressSpinner.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ProgressSpinner.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/RadioGroup.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/RadioGroup.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/ScrollView.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/ScrollView.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SearchBox.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SearchBox.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SecureEditText.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SecureEditText.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SegmentedButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SegmentedButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SegmentedButtonListCell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SegmentedButtonListCell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Sheet.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Sheet.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Slider.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Slider.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SliderListCell.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SliderListCell.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SplitView.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SplitView.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/SquareButton.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/SquareButton.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Tabs.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Tabs.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/TextBox.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/TextBox.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/TextEditor.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/TextEditor.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/VerticalLine.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/VerticalLine.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/VerticalRadioGroup.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/VerticalRadioGroup.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/VerticalStackView.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/VerticalStackView.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/_images/Window.png` & `cocoa-vanilla-0.4.0/Documentation/source/_images/Window.png`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/concepts/positioning.rst` & `cocoa-vanilla-0.4.0/Documentation/source/concepts/positioning.rst`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/conf.py` & `cocoa-vanilla-0.4.0/Documentation/source/conf.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/index.rst` & `cocoa-vanilla-0.4.0/Documentation/source/index.rst`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/objects/FloatingWindow.rst` & `cocoa-vanilla-0.4.0/Documentation/source/objects/FloatingWindow.rst`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Documentation/source/objects/Window.rst` & `cocoa-vanilla-0.4.0/Documentation/source/objects/Window.rst`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/PKG-INFO` & `cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoa-vanilla
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Pythonic wrapper around Cocoa.
 Home-page: https://github.com/robotools/vanilla
 Author: Tal Leming
 Author-email: tal@typesupply.com
 Maintainer: Just van Rossum, Frederik Berlaen
 Maintainer-email: justvanrossum@gmail.com
 License: MIT
```

### Comparing `cocoa-vanilla-0.3.0/Lib/cocoa_vanilla.egg-info/SOURCES.txt` & `cocoa-vanilla-0.4.0/Lib/cocoa_vanilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/__init__.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/__init__.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/dialogs.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from objc import selector
 from objc import python_method
+from objc import super
 from Foundation import NSObject
 from AppKit import NSAlert, NSSavePanel, NSOpenPanel, NSAlertStyleCritical, NSAlertStyleInformational, NSAlertStyleWarning, NSAlertFirstButtonReturn, NSAlertSecondButtonReturn, NSAlertThirdButtonReturn, NSOKButton, NSURL, NSImage
 
 
 __all__ = ["message", "askYesNoCancel", "askYesNo", "getFile", "getFolder", "getFileOrFolder", "putFile"]
 
 
@@ -39,15 +40,15 @@
     def windowWillClose_(self, notification):
         self.autorelease()
 
 
 class BaseMessageDialog(BasePanel):
 
     def initWithWindow_resultCallback_(cls, parentWindow=None, resultCallback=None):
-        self = super(BaseMessageDialog, cls).initWithWindow_resultCallback_(parentWindow, resultCallback)
+        self = super().initWithWindow_resultCallback_(parentWindow, resultCallback)
         self.messageText = ""
         self.informativeText = ""
         self.alertStyle = NSAlertStyleInformational
         self.buttonTitlesValues = []
         self.accessoryView = None
         self.icon = None
         self.showsHelpCallback = None
@@ -135,15 +136,15 @@
             if self._cancelCallback is not None:
                 self._cancelCallback()
 
 
 class PutFilePanel(BasePutGetPanel):
 
     def initWithWindow_resultCallback_cancelCallback_(self, parentWindow=None, resultCallback=None, cancelCallback=None):
-        self = super(PutFilePanel, self).initWithWindow_resultCallback_cancelCallback_(parentWindow, resultCallback, cancelCallback)
+        self = super().initWithWindow_resultCallback_cancelCallback_(parentWindow, resultCallback, cancelCallback)
         self.messageText = None
         self.title = None
         self.fileTypes = None
         self.directory = None
         self.fileName = None
         self.canCreateDirectories = True
         self.accessoryView = None
@@ -182,15 +183,15 @@
             if self._cancelCallback is not None:
                 self._cancelCallback()
 
 
 class GetFileOrFolderPanel(BasePutGetPanel):
 
     def initWithWindow_resultCallback_cancelCallback_(self, parentWindow=None, resultCallback=None, cancelCallback=None):
-        self = super(GetFileOrFolderPanel, self).initWithWindow_resultCallback_cancelCallback_(parentWindow, resultCallback, cancelCallback)
+        self = super().initWithWindow_resultCallback_cancelCallback_(parentWindow, resultCallback, cancelCallback)
         self.messageText = None
         self.title = None
         self.directory = None
         self.fileName = None
         self.fileTypes = None
         self.allowsMultipleSelection = False
         self.canChooseDirectories = True
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/dragAndDrop.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/dragAndDrop.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/nsSubclasses.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/nsSubclasses.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/py23.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/py23.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/cells.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/cells.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/groupRows.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/groupRows.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/list2/selection.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/list2/selection.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testAll.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testAll.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testDialogs.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testDialogs.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testDragAndDrop.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testDragAndDrop.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testGeometry.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testGeometry.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testGridView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testGridView.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testSplitview.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testSplitview.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testStackView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testStackView.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testTools.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testTools.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/test/testWindowBindings.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/test/testWindowBindings.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaBase.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import platform
+from objc import super
 
 from Foundation import NSObject
 from AppKit import NSFont, NSRegularControlSize, NSSmallControlSize, NSMiniControlSize, \
     NSViewMinXMargin, NSViewMaxXMargin, NSViewMaxYMargin, NSViewMinYMargin, \
     NSViewWidthSizable, NSViewHeightSizable, \
     NSLayoutConstraint, NSLayoutFormatAlignAllLeft, \
     NSLayoutAttributeLeft, NSLayoutAttributeRight, NSLayoutAttributeTop, NSLayoutAttributeBottom, NSLayoutAttributeLeading, NSLayoutAttributeTrailing, \
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaBox.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaBox.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import objc
+from objc import super
 from AppKit import NSBox, NSColor, NSFont, NSSmallControlSize, NSNoTitle, NSLineBorder, NSBoxSeparator, NSBoxCustom
 from vanilla.vanillaBase import VanillaBaseObject, _breakCycles, osVersionCurrent, osVersion10_10
 
 
 class Box(VanillaBaseObject):
 
     """
@@ -38,21 +38,23 @@
     allFrameAdjustments = {
         # Box does not have sizeStyle, but the
         # adjustment is differeent based on the
         # presence of a title.
         "Box-Titled": (-3, -4, 6, 4),
         "Box-None": (-3, -4, 6, 6)
     }
+    _ignoreFrameAdjustments = False
 
     nsBoxClass = NSBox
 
     def __init__(self, posSize, title=None,
             fillColor=None, borderColor=None, borderWidth=None,
             cornerRadius=None, margins=None
         ):
+        self._ignoreFrameAdjustments = set((fillColor, borderColor, borderWidth, cornerRadius)) != set((None,))
         self._setupView(self.nsBoxClass, posSize)
         if title:
             self._nsObject.setTitle_(title)
             if osVersionCurrent < osVersion10_10:
                 self._nsObject.titleCell().setTextColor_(NSColor.blackColor())
             font = NSFont.systemFontOfSize_(NSFont.systemFontSizeForControlSize_(NSSmallControlSize))
             self._nsObject.setTitleFont_(font)
@@ -74,30 +76,32 @@
         Return the `NSBox`_ that this object wraps.
 
         .. _NSBox: https://developer.apple.com/documentation/appkit/nsbox?language=objc
         """
         return self._nsObject
 
     def _adjustPosSize(self, frame):
+        if self._ignoreFrameAdjustments:
+            self.frameAdjustments = (0, 0, 0, 0)
         # skip subclasses
-        if self.__class__.__name__ == "Box":
+        elif self.__class__.__name__ == "Box":
             pos = self._nsObject.titlePosition()
             if pos != NSNoTitle:
                 title = "Titled"
             else:
                 title = "None"
             boxType = "Box-" + title
             self.frameAdjustments = self.allFrameAdjustments[boxType]
-        return super(Box, self)._adjustPosSize(frame)
+        return super()._adjustPosSize(frame)
 
     def _getContentView(self):
         return self._nsObject.contentView()
 
     def _breakCycles(self):
-        super(Box, self)._breakCycles()
+        super()._breakCycles()
         view = self._nsObject.contentView()
         if view is not None:
             _breakCycles(view)
 
     def setTitle(self, title):
         """
         Set the title of the box.
@@ -188,15 +192,15 @@
     | **Standard Dimensions** |
     +===+=====================+
     | H | 1                   |
     +---+---------------------+
     """
 
     def __init__(self, posSize):
-        super(HorizontalLine, self).__init__(posSize)
+        super().__init__(posSize)
 
 
 class VerticalLine(_Line):
 
     """
     A vertical line.
 
@@ -222,8 +226,8 @@
     | **Standard Dimensions** |
     +===+=====================+
     | V | 1                   |
     +---+---------------------+
     """
 
     def __init__(self, posSize):
-        super(VerticalLine, self).__init__(posSize)
+        super().__init__(posSize)
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaBrowser.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaBrowser.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaButton.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaButton.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self._setSizeStyle(sizeStyle)
         self._nsObject.setTitle_(title)
         if self.nsBezelStyle is not None:
             self._nsObject.setBezelStyle_(self.nsBezelStyle)
         self._nsObject.setButtonType_(self.nsButtonType)
 
     def _testForDeprecatedAttributes(self):
-        super(Button, self)._testForDeprecatedAttributes()
+        super()._testForDeprecatedAttributes()
         from warnings import warn
         if hasattr(self, "_nsBezelStyle"):
             warn(DeprecationWarning("The _nsBezelStyle attribute is deprecated. Use the nsBezelStyle attribute."))
             self.nsBezelStyle = self._nsBezelStyle
         if hasattr(self, "_nsButtonType"):
             warn(DeprecationWarning("The _nsButtonType attribute is deprecated. Use the nsButtonType attribute."))
             self.nsButtonType = self._nsButtonType
@@ -205,15 +205,15 @@
     +-----------+
     """
 
     nsBezelStyle = NSShadowlessSquareBezelStyle
     frameAdjustments = None
 
     def __init__(self, posSize, title, callback=None, sizeStyle="regular"):
-        super(SquareButton, self).__init__(posSize=posSize, title=title, callback=callback, sizeStyle=sizeStyle)
+        super().__init__(posSize=posSize, title=title, callback=callback, sizeStyle=sizeStyle)
 
 
 _imagePositionMap = {
         "left": NSImageLeft,
         "right": NSImageRight,
         "top": NSImageAbove,
         "bottom": NSImageBelow,
@@ -292,15 +292,15 @@
     """
 
     frameAdjustments = None
 
     def __init__(self, posSize,
                 imagePath=None, imageNamed=None, imageObject=None,
                 title=None, bordered=True, imagePosition="top", callback=None, sizeStyle="regular"):
-        super(ImageButton,  self).__init__(posSize, title=title, callback=callback, sizeStyle=sizeStyle)
+        super().__init__(posSize, title=title, callback=callback, sizeStyle=sizeStyle)
         image = None
         if imagePath is not None:
             image = NSImage.alloc().initWithContentsOfFile_(imagePath)
         elif imageNamed is not None:
             image = NSImage.imageNamed_(imageNamed)
         elif imageObject is not None:
             image = imageObject
@@ -390,15 +390,15 @@
         # XXX perhaps this should choke if more than one arg is present.
         # callback, page and anchor are all mutually exclusive.
         self._page = page
         self._anchor = anchor
         if callback is None:
             if page is not None or anchor is not None:
                 callback = self._helpBookCallback
-        super(HelpButton, self).__init__(posSize, title="", callback=callback)
+        super().__init__(posSize, title="", callback=callback)
 
     def _helpBookCallback(self, sender):
         from Carbon import AH
         bundle = NSBundle.mainBundle()
         if bundle is None:
             return
         info = bundle.infoDictionary()
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaCheckBox.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaCheckBox.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     frameAdjustments = {
         "mini": (-4, -4, 6, 8),
         "small": (-3, -2, 5, 4),
         "regular": (-2, -2, 4, 4),
     }
 
     def __init__(self, posSize, title, callback=None, value=False, sizeStyle="regular"):
-        super(_CheckBoxStandardBuild, self).__init__(posSize, title, callback=callback, sizeStyle=sizeStyle)
+        super().__init__(posSize, title, callback=callback, sizeStyle=sizeStyle)
         self.set(value)
 
     def set(self, value):
         """
         Set the state of the check box.
 
         **value** A boolean representing the state of the check box.
@@ -129,15 +129,15 @@
 
 class _CheckBoxManualBuildTextButton(Button):
 
     nsBezelStyle = NSShadowlessSquareBezelStyle
     frameAdjustments = None
 
     def __init__(self, posSize, title, callback, sizeStyle):
-        super(_CheckBoxManualBuildTextButton, self).__init__(posSize, title=title, callback=callback)
+        super().__init__(posSize, title=title, callback=callback)
         self._nsObject.setBordered_(False)
         self._setSizeStyle(sizeStyle)
         self._nsObject.setAlignment_(NSTextAlignmentLeft)
         self._nsObject.cell().setHighlightsBy_(NSNoCellMask)
 
 
 class _CheckBoxManualBuild(VanillaBaseObject):
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaColorWell.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaColorWell.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             self._nsObject.setColor_(color)
         colorPanel = NSColorPanel.sharedColorPanel()
         colorPanel.setShowsAlpha_(True)
         if osVersionCurrent >= osVersion13_0:
             # https://developer.apple.com/documentation/appkit/nscolorwell/3955203-colorwellstyle?language=objc
             nsColorWellStyle = colorWellStyleMap.get(colorWellStyle)
             if nsColorWellStyle is not None:
-                colorPanel.setColorWellStyle_(nsColorWellStyle)
+                self._nsObject.setColorWellStyle_(nsColorWellStyle)
 
     def getNSColorWell(self):
         """
         Return the `NSColorWell`_ that this object wraps.
 
         .. _NSColorWell: https://developer.apple.com/documentation/appkit/nscolorwell?language=objc
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaComboBox.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaComboBox.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,19 +111,19 @@
         self._setSizeStyle(sizeStyle)
         self._nsObject.addItemsWithObjectValues_(items)
         self._nsObject.setCompletes_(completes)
         if formatter is not None:
             self._nsObject.setFormatter_(formatter)
 
     def _breakCycles(self):
-        super(ComboBox, self)._breakCycles()
+        super()._breakCycles()
         self._delegate = None
 
     def _setCallback(self, callback):
-        super(ComboBox, self)._setCallback(callback)
+        super()._setCallback(callback)
         if callback is not None:
             self._delegate = VanillaComboBoxDelegate.alloc().init()
             self._delegate._continuous = self._continuous
             self._nsObject.setDelegate_(self._delegate)
 
     def getNSComboBox(self):
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaDatePicker.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaDatePicker.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaDrawer.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaDrawer.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         """
         return self._nsObject
 
     def _getContentView(self):
         return self._nsObject.contentView()
 
     def _breakCycles(self):
-        super(Drawer, self)._breakCycles()
+        super()._breakCycles()
         view = self._getContentView()
         if view is not None:
             _breakCycles(view)
 
     def open(self):
         """
         Open the drawer.
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaEditText.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaEditText.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         self._nsObject.setEditable_(not readOnly)
         self._nsObject.setSelectable_(True)
         self._nsObject.setFormatter_(formatter)
         if placeholder:
             self._nsObject.cell().setPlaceholderString_(placeholder)
 
     def _testForDeprecatedAttributes(self):
-        super(EditText, self)._testForDeprecatedAttributes()
+        super()._testForDeprecatedAttributes()
         from warnings import warn
         if hasattr(self, "_textFieldClass"):
             warn(DeprecationWarning("The _textFieldClass attribute is deprecated. Use the nsTextFieldClass attribute."))
             self.nsTextFieldClass = self._textFieldClass
 
     def getNSTextField(self):
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaGradientButton.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaGradientButton.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaGridView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaGridView.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaGroup.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,25 +120,25 @@
             self._visualEffectGroup.getNSVisualEffectView().setBlendingMode_(blendingMode)
         if dropSettings is not None:
             self.setDropSettings(dropSettings)
 
     def __setattr__(self, attr, value):
         # __init__
         if not hasattr(self, "_visualEffectGroup") or attr == "_visualEffectGroup":
-            super(Group, self).__setattr__(attr, value)
+            super().__setattr__(attr, value)
         # adding a vanilla subview: add to the visual effect view
         elif hasattr(self, "_visualEffectGroup") and isinstance(value, VanillaBaseObject) and hasattr(value, "_posSize"):
             setattr(self._visualEffectGroup, attr, value)
         # fallback: add to the main view
         else:
-            super(Group, self).__setattr__(attr, value)
+            super().__setattr__(attr, value)
 
     def __delattr__(self, attr):
         if hasattr(self, attr):
-            super(Group, self).__delattr__(attr)
+            super().__delattr__(attr)
         elif hasattr(self, "_visualEffectView"):
             delattr(self._visualEffectView, attr)
 
     def getNSView(self):
         """
         Return the `NSView`_ that this object wraps.
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaImageView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaImageView.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaLevelIndicator.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaLevelIndicator.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaList.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaList.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 import time
 from Foundation import NSObject, NSArray, NSMutableArray, NSDictionary, NSMutableDictionary, NSMutableIndexSet, NSString, NSAttributedString, NSKeyValueObservingOptionNew, NSKeyValueObservingOptionOld, NSNotFound
 from AppKit import NSApp, NSTableView, NSTableColumn, NSArrayController, NSScrollView, NSSwitchButton, NSButtonCell, NSSliderCell, NSPopUpButtonCell, NSImageCell, NSSegmentedCell, NSFont, NSImage, NSReturnTextMovement, NSTabTextMovement, NSBacktabTextMovement, NSIllegalTextMovement, NSNotification, NSDragOperationNone, NSTableViewDropOn, NSDragOperationCopy, NSBezelBorder, NSFocusRingTypeNone, NSTableViewSolidVerticalGridLineMask, NSTableViewSolidHorizontalGridLineMask, NSTableViewUniformColumnAutoresizingStyle, NSTableColumnNoResizing, NSTableColumnUserResizingMask, NSTableColumnAutoresizingMask, NSCreatesSortDescriptorBindingOption, NSBackspaceCharacter, NSDeleteFunctionKey, NSDeleteCharacter, NSUpArrowFunctionKey, NSDownArrowFunctionKey, NSLeftArrowFunctionKey, NSRightArrowFunctionKey, NSPageUpFunctionKey, NSPageDownFunctionKey, NSSmallControlSize, NSMiniControlSize, NSSegmentSwitchTrackingSelectOne, NSMenuItem, NSMenu
 from objc import python_method, pyobjc_unicode
+from objc import super
 
 from vanilla.nsSubclasses import getNSSubclass
 from vanilla.vanillaBase import VanillaBaseObject, VanillaError, VanillaCallbackWrapper
 
 
 class VanillaTableViewSubclass(NSTableView):
 
     def keyDown_(self, event):
         didSomething = self.vanillaWrapper()._keyDown(event)
         if not didSomething:
-            super(VanillaTableViewSubclass, self).keyDown_(event)
+            super().keyDown_(event)
 
     def textDidEndEditing_(self, notification):
         info = notification.userInfo()
         if info["NSTextMovement"] in [NSReturnTextMovement, NSTabTextMovement, NSBacktabTextMovement]:
             # This is ugly, but just about the only way to do it.
             # NSTableView is determined to select and edit something else,
             # even the text field that it just finished editing, unless we
             # mislead it about what key was pressed to end editing.
             info = dict(info)  # make a copy
             info["NSTextMovement"] = NSIllegalTextMovement
             newNotification = NSNotification.notificationWithName_object_userInfo_(
                     notification.name(),
                     notification.object(),
                     info)
-            super(VanillaTableViewSubclass, self).textDidEndEditing_(newNotification)
+            super().textDidEndEditing_(newNotification)
             self.window().makeFirstResponder_(self)
         else:
-            super(VanillaTableViewSubclass, self).textDidEndEditing_(notification)
+            super().textDidEndEditing_(notification)
 
     def menuForEvent_(self, event):
         wrapper = self.vanillaWrapper()
         return wrapper._menuForEvent(event)
 
 
 class _VanillaTableViewSubclass(VanillaTableViewSubclass):
 
     def init(self):
         from warnings import warn
         warn(DeprecationWarning("_VanillaTableViewSubclass is deprecated. Use VanillaTableViewSubclass"))
-        return super(_VanillaTableViewSubclass, self).init()
+        return super().init()
 
 
 class VanillaArrayControllerObserver(NSObject):
 
     def observeValueForKeyPath_ofObject_change_context_(self, keyPath, obj, change, context):
         if hasattr(self, "_targetMethod") and self._targetMethod is not None:
             self._targetMethod()
 
 
 class _VanillaArrayControllerObserver(VanillaArrayControllerObserver):
 
     def init(self):
         from warnings import warn
         warn(DeprecationWarning("_VanillaArrayControllerObserver is deprecated. Use VanillaArrayControllerObserver"))
-        return super(_VanillaArrayControllerObserver, self).init()
+        return super().init()
 
 
 class VanillaArrayController(NSArrayController):
 
     def tableView_writeRowsWithIndexes_toPasteboard_(self,
         tableView, indexes, pboard):
         vanillaWrapper = tableView.vanillaWrapper()
@@ -187,15 +188,15 @@
 
 
 class _VanillaArrayController(VanillaArrayController):
 
     def init(self):
         from warnings import warn
         warn(DeprecationWarning("_VanillaArrayController is deprecated. Use VanillaArrayController"))
-        return super(_VanillaArrayController, self).init()
+        return super().init()
 
 
 def VanillaMenuBuilder(sender, items, menu, resetCallbackWrapper=True):
     """
     Build a menu from a given set of items
     Each items must be a dict with the following keys:
 
@@ -620,15 +621,15 @@
                 continue
             local = settings.get("operation", NSDragOperationCopy)
         self._tableView.setDraggingSourceOperationMask_forLocal_(local, True)
         # set the drag data
         self._dragSettings = dragSettings
 
     def _testForDeprecatedAttributes(self):
-        super(List, self)._testForDeprecatedAttributes()
+        super()._testForDeprecatedAttributes()
         from warnings import warn
         if hasattr(self, "_scrollViewClass"):
             warn(DeprecationWarning("The _scrollViewClass attribute is deprecated. Use the nsScrollViewClass attribute."))
             self.nsScrollViewClass = self._scrollViewClass
         if hasattr(self, "_tableViewClass"):
             warn(DeprecationWarning("The _tableViewClass attribute is deprecated. Use the nsTableViewClass attribute."))
             self.nsTableViewClass = self._tableViewClass
@@ -653,15 +654,15 @@
 
         .. _NSTableView: https://developer.apple.com/documentation/appkit/nstableview?language=objc
         """
         return self._tableView
 
     def _breakCycles(self):
         self._menuItemCallbackWrappers = None
-        super(List, self)._breakCycles()
+        super()._breakCycles()
         if hasattr(self, "_editCallback") and self._editObserver is not None:
             for column in self._tableView.tableColumns():
                 if not column.isEditable():
                     continue
                 keyPath = "arrangedObjects.%s" % column.identifier()
                 self._arrayController.removeObserver_forKeyPath_(self._editObserver, keyPath)
             self._editObserver._targetMethod = None
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaList2.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaList2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import operator
 import weakref
 import types
 import objc
 from objc import python_method
+from objc import super
 import AppKit
 from vanilla.nsSubclasses import getNSSubclass
 from vanilla.vanillaBase import VanillaBaseObject, VanillaCallbackWrapper, osVersionCurrent, osVersion10_16
 from vanilla.vanillaScrollView import ScrollView
 from vanilla.dragAndDrop import DropTargetProtocolMixIn, dropOperationMap, makePasteboardItem
 
 simpleDataTypes = (
@@ -925,26 +926,41 @@
 # -----
 # Cells
 # -----
 
 from vanilla.vanillaGroup import Group
 from vanilla.vanillaEditText import EditText
 
+truncationMap = dict(
+    clipping=AppKit.NSLineBreakByClipping,
+    head=AppKit.NSLineBreakByTruncatingHead,
+    tail=AppKit.NSLineBreakByTruncatingTail,
+    middle=AppKit.NSLineBreakByTruncatingMiddle
+)
+
 class EditTextList2Cell(Group):
 
     """
     An object that displays text in a List2 column.
 
     **verticalAlignment** The vertical alignment of the text
     within the row. Options:
 
     - `"top"`
     - `"center"`
     - `"bottom"`
 
+    **truncationMode** How text should be truncated. Options:
+
+    - `"clipping"`
+    - `"head"`
+    - `"tail"`
+    - `"middle"`
+    - A specific `NSLineBreakMode`.
+
     .. note::
        This class should only be used in the *columnDescriptions*
        *cellClass* argument during the construction of a List.
        This is never constructed directly.
     """
 
     # Implementation Note:
@@ -962,14 +978,15 @@
     # so it has to be built and we may as well skip the
     # expense of NSTableCellView and go straight to NSView.
     # Sigh.
 
     def __init__(self,
             verticalAlignment="center",
             editable=False,
+            truncationMode="tail",
             callback=None
         ):
         self._externalCallback = callback
         super().__init__("auto")
         self.editText = EditText(
             "auto",
             readOnly=not editable,
@@ -999,14 +1016,16 @@
                 view2=self,
                 attribute2="height"
             )
             rules.append(heightRule)
         self.addAutoPosSizeRules(rules)
         textField.setDrawsBackground_(False)
         textField.setBezeled_(False)
+        lineBreakMode = truncationMap.get(truncationMode, truncationMode)
+        textField.setLineBreakMode_(lineBreakMode)
 
     def getNSTextField(self):
         return self.editText.getNSTextField()
 
     def _internalCallback(self, sender):
         if self._externalCallback is not None:
             self._externalCallback(self)
@@ -1358,14 +1377,14 @@
             majorTickMarkCount=majorTickMarkCount,
             # sizeStyle="small",
             callback=callback
         )
         self.enable(editable)
         cell = self._nsObject.cell()
         if imagePath is not None:
-            image = NSImage.alloc().initWithContentsOfFile_(imagePath)
+            image = AppKit.NSImage.alloc().initWithContentsOfFile_(imagePath)
         elif imageNamed is not None:
-            image = NSImage.imageNamed_(imageNamed)
+            image = AppKit.NSImage.imageNamed_(imageNamed)
         elif imageObject is not None:
             image = imageObject
         if imageObject is not None:
-            cell.setImage_(image)
+            cell.setImage_(image)
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaPathControl.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaPathControl.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaPopUpButton.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaPopUpButton.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,22 +204,22 @@
 
     **bordered** Boolean representing if the button should be bordered.
 
     .. _NSMenuItem: https://developer.apple.com/documentation/appkit/nsmenuitem?language=objc
     """
 
     def __init__(self, posSize, items, sizeStyle="regular", bordered=True):
-        super(ActionButton, self).__init__(posSize, items, sizeStyle=sizeStyle)
+        super().__init__(posSize, items, sizeStyle=sizeStyle)
         self._nsObject.setPullsDown_(True)
         self._nsObject.setBezelStyle_(NSTexturedRoundedBezelStyle)
         self._nsObject.setBordered_(bordered)
 
     def _breakCycles(self):
         self._menuItemCallbackWrappers = None
-        super(ActionButton, self)._breakCycles()
+        super()._breakCycles()
 
     def getFirstItem(self):
         actionImage = NSImage.imageNamed_(NSImageNameActionTemplate).copy()
         sizeStyle = _reverseSizeStyleMap[self._nsObject.cell().controlSize()]
         if sizeStyle == "small":
             actionImage.setSize_((10, 10))
         elif sizeStyle == "mini":
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaPopover.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaPopover.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         self._bindings = {}
         self._autoLayoutViews = {}
 
     def __del__(self):
         self._breakCycles()
 
     def _breakCycles(self):
-        super(Popover, self)._breakCycles()
+        super()._breakCycles()
         view = self._getContentView()
         if view is not None:
             _breakCycles(view)
         self._contentViewController = None
         self._popover = None
         self._parentView = None
         self._delegate = None
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaProgressBar.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaProgressBar.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaProgressSpinner.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaProgressSpinner.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaRadioGroup.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaRadioGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     )
 
     def _init(self, cls, posSize, titles, callback=None, sizeStyle="regular"):
         spacing = self._spacing[sizeStyle]
         self._buttonHeight = self._heights[sizeStyle]
         self._callback = callback
         self._sizeStyle = sizeStyle
-        super(cls, self).__init__(posSize, spacing=spacing, alignment="leading")
+        super().__init__(posSize, spacing=spacing, alignment="leading")
         self._buildButtons(titles, sizeStyle)
 
     def _buildButtons(self, titles, sizeStyle):
         self._buttons = []
         for title in titles:
             button = RadioButton("auto", title, callback=self._buttonCallback, sizeStyle=sizeStyle)
             self._buttons.append(button)
@@ -197,15 +197,15 @@
     A single radio button.
     """
 
     nsBezelStyle = None
     nsButtonType = NSRadioButtonType
 
     def __init__(self, posSize, title, value=False, callback=None, sizeStyle="regular"):
-        super(RadioButton, self).__init__(posSize, title, callback=callback, sizeStyle=sizeStyle)
+        super().__init__(posSize, title, callback=callback, sizeStyle=sizeStyle)
         self.set(value)
 
     def set(self, value):
         """
         Set the state of the radio button.
 
         **value** A boolean representing the state of the radio button.
@@ -312,15 +312,15 @@
         for title, cell in zip(titles, matrix.cells()):
             cell.setButtonType_(NSRadioButton)
             cell.setTitle_(title)
             cell.setControlSize_(cellSizeStyle)
             cell.setFont_(font)
 
     def _testForDeprecatedAttributes(self):
-        super(RadioGroup, self)._testForDeprecatedAttributes()
+        super()._testForDeprecatedAttributes()
         from warnings import warn
         if hasattr(self, "_cellClass"):
             warn(DeprecationWarning("The _cellClass attribute is deprecated. Use the nsCellClass attribute."))
             self.nsCellClass = self._cellClass
 
     def getNSMatrix(self):
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaScrollView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaScrollView.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._nsObject.setAutohidesScrollers_(autohidesScrollers)
         self._nsObject.setBorderType_(NSBezelBorder)
         if backgroundColor:
             self._nsObject.setBackgroundColor_(backgroundColor)
         self._nsObject.setDrawsBackground_(drawsBackground)
 
     def _testForDeprecatedAttributes(self):
-        super(ScrollView, self)._testForDeprecatedAttributes()
+        super()._testForDeprecatedAttributes()
         from warnings import warn
         if hasattr(self, "_scrollViewClass"):
             warn(DeprecationWarning("The _scrollViewClass attribute is deprecated. Use the nsScrollViewClass attribute."))
             self.nsScrollViewClass = self._scrollViewClass
 
     def getNSScrollView(self):
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSearchBox.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSearchBox.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSegmentedButton.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSegmentedButton.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSlider.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSlider.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 if tickPos == NSTickMarkBelow:
                     tickPos = "Below"
                 elif tickPos == NSTickMarkAbove:
                     tickPos = "Above"
         sliderType = prefix + "Slider-" + tickPos
         self.frameAdjustments = self.allFrameAdjustments[sliderType]
         # now let the super class do the work
-        return super(Slider, self)._adjustPosSize(frame)
+        return super()._adjustPosSize(frame)
 
     def get(self):
         """
         Get the value of the slider.
         """
         return self._nsObject.floatValue()
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaSplitView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaSplitView.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from warnings import warn
 from Foundation import NSObject
 from AppKit import NSSplitView, NSSplitViewDividerStylePaneSplitter, NSSplitViewDividerStyleThin, NSSplitViewDividerStyleThick, NSViewWidthSizable, NSViewHeightSizable
 from objc import python_method
+from objc import super
 
 import vanilla
 from vanilla.vanillaBase import VanillaBaseObject, _breakCycles
 
 
 _dividerStyleMap = {
     "splitter": NSSplitViewDividerStylePaneSplitter,
@@ -25,36 +26,36 @@
         if delegate is not None:
             self.delegate().splitViewInitialSizing_(self)
 
     # Divider
 
     def dividerColor(self):
         if self._dividerColor is None:
-            return super(VanillaSplitViewSubclass, self).dividerColor()
+            return super().dividerColor()
         return self._dividerColor
 
     def setDividerColor_(self, color):
         self._dividerColor = color
         self.setNeedsDisplay_(True)
 
     def dividerThickness(self):
         if self._dividerThickness is None:
-            return super(VanillaSplitViewSubclass, self).dividerThickness()
+            return super().dividerThickness()
         return self._dividerThickness
 
     def setDividerThickness_(self, value):
         self._dividerThickness = value
 
     def setDividerDrawingFunction_(self, function):
         self._dividerDrawingFunction = function
         self.setNeedsDisplay_(True)
 
     def drawDividerInRect_(self, rect):
         if self._dividerDrawingFunction is None:
-            super(VanillaSplitViewSubclass, self).drawDividerInRect_(rect)
+            super().drawDividerInRect_(rect)
         else:
             self._dividerDrawingFunction(splitView=self.vanillaWrapper(), rect=rect)
 
     # Pane Visibility
 
     def getStateForPane_(self, identifier):
         wrapper = self.vanillaWrapper()
@@ -487,15 +488,15 @@
         for view in list(splitView.subviews()):
             view.removeFromSuperview()
             _breakCycles(view)
         self._nsObject.setDelegate_(None)
         self._delegate = None
         self._paneDescriptions = None
         self._identifierToPane = None
-        super(SplitView, self)._breakCycles()
+        super()._breakCycles()
 
     def _setupPanes(self):
         self._identifierToPane = {}
         splitView = self.getNSSplitView()
         splitViewFrame = splitView.frame()
         mask = NSViewWidthSizable | NSViewHeightSizable
         for index, paneDescription in enumerate(self._paneDescriptions):
@@ -592,8 +593,8 @@
 def _dummySplitViewDrawingFunction(splitView, rect):
     return
 
 
 class SplitView2(SplitView):
     def __init__(self, *args, **kwargs):
         warn(DeprecationWarning("SplitView2 has been deprecated, use SplitView instead."))
-        super(SplitView2, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaStackGroup.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaStackGroup.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaStackView.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaStackView.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,20 +149,23 @@
         stackView.insertView_atIndex_inGravity_(view, index, gravity)
         if isinstance(view, VanillaBaseObject):
             view = view._nsObject
         stackView = self.getNSStackView()
         # size shortcuts
         # - when "fill" if used in the direction of the main axis,
         #   it means "use a flexible space"
+        # - when "fit" is used, let AppKit figure out the width.
+        #   (note: this previously used view.fittingSize()
+        #   to get an absolute size, but it was unreliable.)
         if width == "fit":
-            width = view.fittingSize()[0]
+            width = None
         elif width == "fill" and self._orientation == NSUserInterfaceLayoutOrientationHorizontal:
             width = None
         if height == "fit":
-            height = view.fittingSize()[1]
+            height = None
         elif height == "fill" and self._orientation == NSUserInterfaceLayoutOrientationVertical:
             height = None
         # hugging and compression
         widthHuggingPriority = AppKit.NSLayoutPriorityRequired
         widthCompressionPriority = AppKit.NSLayoutPriorityRequired
         if width is None:
             intrinsicWidth = view.intrinsicContentSize()[0]
@@ -233,19 +236,23 @@
             else:
                 _setAnchorConstraint(
                     view.widthAnchor(),
                     width
                 )
         if height is not None:
             if height == "fill":
-                view.topAnchor().constraintEqualToAnchor_(
-                    stackView.topAnchor()
+                _setAnchorConstraint(
+                    anchor=view.topAnchor(),
+                    otherAnchor=stackView.topAnchor(),
+                    constant=topInset
                 )
-                view.bottomAnchor().constraintEqualToAnchor_(
-                    stackView.bottomAnchor()
+                _setAnchorConstraint(
+                    anchor=view.bottomAnchor(),
+                    otherAnchor=stackView.bottomAnchor(),
+                    constant=-bottomInset
                 )
             else:
                 _setAnchorConstraint(
                     view.heightAnchor(),
                     height
                 )
         # spacing
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaStepper.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaStepper.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaTabs.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaTabs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from Foundation import NSObject
+from objc import super
+
 from AppKit import NSViewController,\
     NSTabViewController, NSTabView, NSTabViewItem,\
     NSTabPositionTop,\
     NSTabPositionNone,\
     NSNoTabsNoBorder,\
     NSViewControllerTransitionNone,\
     NSViewControllerTransitionCrossfade,\
@@ -10,15 +12,15 @@
     NSViewControllerTransitionSlideDown,\
     NSViewControllerTransitionSlideLeft,\
     NSViewControllerTransitionSlideRight,\
     NSViewControllerTransitionSlideForward,\
     NSViewControllerTransitionSlideBackward,\
     NSFont
 from vanilla.vanillaBase import VanillaBaseObject, _breakCycles, _sizeStyleMap, VanillaCallbackWrapper, \
-    _reverseSizeStyleMap
+    _reverseSizeStyleMap, _recursiveSetFrame
 from vanilla.nsSubclasses import getNSSubclass
 
 
 class VanillaTabView(NSTabView):
 
     def viewDidMoveToWindow(self):
         if self.window() is not None:
@@ -191,29 +193,35 @@
         """
         Return the `NSTabView`_ that this object wraps.
 
         .. _NSTabView: https://developer.apple.com/documentation/appkit/nstabview?language=objc
         """
         return self._nsObject
 
+    _didPositionViews = False
+
     def _positionViews(self):
+        if self._didPositionViews:
+            return
         contentRect = self.getNSTabView().contentRect()
         # only do after the first because
         # adjusting the first gives it
         # incorrect positioning
         for item in self._tabItems[1:]:
             item._setFrame(contentRect)
+            _recursiveSetFrame(item._nsObject)
+        self._didPositionViews = True
 
     def _adjustPosSize(self, frame):
         if self._nsObject.tabViewType() == NSNoTabsNoBorder:
             return frame
         sizeStyle = _reverseSizeStyleMap[self._nsObject.controlSize()]
         tabsType = "Tabs-" + sizeStyle
         self.frameAdjustments = self.allFrameAdjustments[tabsType]
-        return super(Tabs, self)._adjustPosSize(frame)
+        return super()._adjustPosSize(frame)
 
     def _setCallback(self, callback):
         if callback is not None:
             self._target = VanillaCallbackWrapper(callback)
             delegate = self._nsObject.delegate()
             delegate._target = self._target
 
@@ -223,15 +231,15 @@
         font = NSFont.systemFontOfSize_(NSFont.systemFontSizeForControlSize_(value))
         self._nsObject.setFont_(font)
 
     def __getitem__(self, index):
         return self._tabItems[index]
 
     def _breakCycles(self):
-        super(Tabs, self)._breakCycles()
+        super()._breakCycles()
         for item in self._tabItems:
             item._breakCycles()
 
     def get(self):
         """
         Get the index of the selected tab.
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaTextBox.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaTextBox.py`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaTextEditor.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaTextEditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self._textView.setEditable_(not readOnly)
         self._nsObject.setDocumentView_(self._textView)
         # do the base object init methods
         self._setCallback(callback)
         self._setAutosizingFromPosSize(posSize)
 
     def _testForDeprecatedAttributes(self):
-        super(TextEditor, self)._testForDeprecatedAttributes()
+        super()._testForDeprecatedAttributes()
         from warnings import warn
         if hasattr(self, "_textViewClass"):
             warn(DeprecationWarning("The _textViewClass attribute is deprecated. Use the nsTextViewClass attribute."))
             self.nsTextViewClass = self._textViewClass
 
     def getNSScrollView(self):
         """
```

### Comparing `cocoa-vanilla-0.3.0/Lib/vanilla/vanillaWindows.py` & `cocoa-vanilla-0.4.0/Lib/vanilla/vanillaWindows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from Foundation import NSObject
 from AppKit import NSApp, NSWindow, NSPanel, NSScreen, NSWindowController, NSToolbar, NSToolbarItem, NSImage, NSNormalWindowLevel, NSFloatingWindowLevel, NSClosableWindowMask, NSMiniaturizableWindowMask, NSResizableWindowMask, NSTexturedBackgroundWindowMask, NSUnifiedTitleAndToolbarWindowMask, NSHUDWindowMask, NSUtilityWindowMask, NSTitledWindowMask, NSBorderlessWindowMask, NSBackingStoreBuffered, NSToolbarFlexibleSpaceItemIdentifier, NSToolbarSpaceItemIdentifier, NSToolbarSeparatorItemIdentifier, NSToolbarCustomizeToolbarItemIdentifier, NSToolbarPrintItemIdentifier, NSToolbarShowFontsItemIdentifier, NSToolbarShowColorsItemIdentifier, NSToolbarDisplayModeDefault, NSToolbarDisplayModeIconAndLabel, NSToolbarDisplayModeIconOnly, NSToolbarDisplayModeLabelOnly, NSToolbarSizeModeDefault, NSToolbarSizeModeRegular, NSToolbarSizeModeSmall
 from objc import python_method
+from objc import super
 
 from vanilla.vanillaBase import _breakCycles, _calcFrame, _setAttr, _delAttr, _addAutoLayoutRules, _flipFrame, \
         VanillaCallbackWrapper, VanillaError, VanillaWarning, VanillaBaseControl, \
         osVersionCurrent, osVersion10_7, osVersion10_10, osVersion10_16
 
 # PyObjC may not have these constants wrapped,
 # so test and fallback if needed.
@@ -1015,15 +1016,15 @@
     nsWindowStyleMask = NSTitledWindowMask | NSUtilityWindowMask
     nsWindowClass = NSPanel
     nsWindowLevel = NSFloatingWindowLevel
 
     def __init__(self, posSize, title="", minSize=None, maxSize=None,
             textured=False, autosaveName=None, closable=True,
             initiallyVisible=True, screen=None):
-        super(FloatingWindow, self).__init__(posSize, title, minSize, maxSize,
+        super().__init__(posSize, title, minSize, maxSize,
                 textured, autosaveName, closable, initiallyVisible=initiallyVisible, screen=screen)
         self._window.setBecomesKeyOnlyIfNeeded_(True)
 
     def show(self):
         """
         Show the window if it is hidden.
         """
@@ -1138,15 +1139,15 @@
 
     def __init__(self, posSize, parentWindow, minSize=None, maxSize=None,
             autosaveName=None):
         if isinstance(parentWindow, Window):
             parentWindow = parentWindow._window
         self.parentWindow = parentWindow
         textured = bool(parentWindow.styleMask() & NSTexturedBackgroundWindowMask)
-        super(Sheet, self).__init__(posSize, "", minSize, maxSize, textured,
+        super().__init__(posSize, "", minSize, maxSize, textured,
                 autosaveName=autosaveName)
 
     def open(self):
         """
         Open the window.
         """
         parentWindow = self.parentWindow
```

### Comparing `cocoa-vanilla-0.3.0/License.txt` & `cocoa-vanilla-0.4.0/License.txt`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/PKG-INFO` & `cocoa-vanilla-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoa-vanilla
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Pythonic wrapper around Cocoa.
 Home-page: https://github.com/robotools/vanilla
 Author: Tal Leming
 Author-email: tal@typesupply.com
 Maintainer: Just van Rossum, Frederik Berlaen
 Maintainer-email: justvanrossum@gmail.com
 License: MIT
```

### Comparing `cocoa-vanilla-0.3.0/ToDo.txt` & `cocoa-vanilla-0.4.0/ToDo.txt`

 * *Files identical despite different names*

### Comparing `cocoa-vanilla-0.3.0/setup.py` & `cocoa-vanilla-0.4.0/setup.py`

 * *Files identical despite different names*

