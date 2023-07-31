# Comparing `tmp/reflex-0.2.3a8.tar.gz` & `tmp/reflex-0.2.3a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.3a8.tar", max compression
+gzip compressed data, was "reflex-0.2.3a9.tar", max compression
```

## Comparing `reflex-0.2.3a8.tar` & `reflex-0.2.3a9.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a8/LICENSE
--rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a8/README.md
--rw-r--r--   0        0        0     2001 2023-07-30 04:08:40.489186 reflex-0.2.3a8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a8/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-27 23:45:03.452394 reflex-0.2.3a8/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a8/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-27 23:45:03.453010 reflex-0.2.3a8/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a8/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a8/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a8/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a8/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a8/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a8/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a8/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a8/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a8/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a8/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a8/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a8/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a8/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a8/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a8/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10172 2023-07-27 23:45:03.453483 reflex-0.2.3a8/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1996 2023-07-27 23:45:03.454124 reflex-0.2.3a8/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a8/reflex/admin.py
--rw-r--r--   0        0        0    24864 2023-07-28 19:12:55.971292 reflex-0.2.3a8/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a8/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a8/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a8/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a8/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a8/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a8/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a8/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a8/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a8/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a8/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a8/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a8/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a8/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a8/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a8/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a8/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a8/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a8/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a8/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a8/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a8/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a8/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a8/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a8/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a8/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a8/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a8/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a8/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a8/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a8/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a8/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a8/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a8/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a8/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a8/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a8/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a8/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a8/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a8/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a8/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a8/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a8/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a8/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a8/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a8/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a8/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a8/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a8/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-29 23:01:33.748219 reflex-0.2.3a8/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a8/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a8/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a8/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a8/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a8/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a8/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a8/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a8/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a8/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a8/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a8/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a8/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a8/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a8/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a8/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a8/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a8/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a8/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a8/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a8/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a8/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a8/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a8/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a8/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a8/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a8/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a8/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a8/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a8/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a8/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a8/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a8/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a8/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a8/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a8/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a8/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a8/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a8/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a8/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a8/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2919 2023-07-29 01:05:18.595845 reflex-0.2.3a8/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a8/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a8/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a8/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a8/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a8/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a8/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a8/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a8/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a8/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a8/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a8/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a8/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a8/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a8/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a8/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5150 2023-07-27 23:45:03.454877 reflex-0.2.3a8/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a8/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a8/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      348 2023-07-27 23:45:03.455160 reflex-0.2.3a8/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a8/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     4679 2023-07-27 23:45:03.455385 reflex-0.2.3a8/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a8/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a8/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7564 2023-07-27 23:45:03.455544 reflex-0.2.3a8/reflex/config.py
--rw-r--r--   0        0        0    12451 2023-07-29 23:18:00.803629 reflex-0.2.3a8/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a8/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a8/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a8/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a8/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a8/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a8/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a8/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a8/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a8/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a8/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a8/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a8/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9598 2023-07-29 02:57:05.377850 reflex-0.2.3a8/reflex/model.py
--rw-r--r--   0        0        0     1832 2023-07-27 23:45:03.455818 reflex-0.2.3a8/reflex/page.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a8/reflex/py.typed
--rw-r--r--   0        0        0    10573 2023-07-30 02:48:40.517517 reflex-0.2.3a8/reflex/reflex.py
--rw-r--r--   0        0        0     3934 2023-07-27 23:45:03.456240 reflex-0.2.3a8/reflex/route.py
--rw-r--r--   0        0        0    32524 2023-07-29 03:11:02.108051 reflex-0.2.3a8/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a8/reflex/style.py
--rw-r--r--   0        0        0    15133 2023-07-30 02:59:25.316492 reflex-0.2.3a8/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a8/reflex/utils/__init__.py
--rw-r--r--   0        0        0     6212 2023-07-29 04:28:04.850394 reflex-0.2.3a8/reflex/utils/build.py
--rw-r--r--   0        0        0     3743 2023-07-30 03:08:01.692245 reflex-0.2.3a8/reflex/utils/console.py
--rw-r--r--   0        0        0     3795 2023-07-29 22:49:09.601795 reflex-0.2.3a8/reflex/utils/exec.py
--rw-r--r--   0        0        0    12342 2023-07-29 01:05:18.597732 reflex-0.2.3a8/reflex/utils/format.py
--rw-r--r--   0        0        0      590 2023-07-27 23:45:03.457502 reflex-0.2.3a8/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a8/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    16639 2023-07-30 02:54:45.030336 reflex-0.2.3a8/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     6387 2023-07-29 23:11:18.706469 reflex-0.2.3a8/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a8/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a8/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a8/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a8/reflex/vars.py
--rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a9/LICENSE
+-rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a9/README.md
+-rw-r--r--   0        0        0     2001 2023-07-31 02:51:35.668499 reflex-0.2.3a9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a9/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-27 23:45:03.452394 reflex-0.2.3a9/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a9/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-27 23:45:03.453010 reflex-0.2.3a9/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a9/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a9/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a9/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a9/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a9/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a9/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a9/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a9/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a9/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a9/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a9/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a9/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a9/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a9/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10172 2023-07-27 23:45:03.453483 reflex-0.2.3a9/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1996 2023-07-27 23:45:03.454124 reflex-0.2.3a9/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a9/reflex/admin.py
+-rw-r--r--   0        0        0    24864 2023-07-28 19:12:55.971292 reflex-0.2.3a9/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a9/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a9/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a9/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a9/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a9/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a9/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a9/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a9/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a9/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a9/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a9/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a9/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a9/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a9/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a9/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a9/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a9/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a9/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a9/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a9/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a9/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a9/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a9/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a9/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a9/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a9/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a9/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a9/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a9/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a9/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a9/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a9/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a9/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a9/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a9/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a9/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a9/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a9/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a9/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a9/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a9/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a9/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a9/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a9/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a9/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a9/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a9/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a9/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-31 00:05:16.998188 reflex-0.2.3a9/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a9/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a9/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a9/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a9/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a9/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a9/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a9/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a9/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a9/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a9/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a9/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a9/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a9/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a9/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a9/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a9/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a9/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a9/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a9/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a9/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a9/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a9/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a9/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a9/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a9/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a9/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a9/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a9/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a9/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a9/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a9/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a9/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a9/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a9/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a9/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a9/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a9/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a9/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a9/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a9/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2919 2023-07-29 01:05:18.595845 reflex-0.2.3a9/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a9/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a9/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a9/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a9/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a9/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a9/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a9/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a9/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a9/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a9/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a9/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a9/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a9/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a9/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a9/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5150 2023-07-27 23:45:03.454877 reflex-0.2.3a9/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a9/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a9/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-27 23:45:03.455160 reflex-0.2.3a9/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a9/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     4679 2023-07-27 23:45:03.455385 reflex-0.2.3a9/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a9/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a9/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7564 2023-07-27 23:45:03.455544 reflex-0.2.3a9/reflex/config.py
+-rw-r--r--   0        0        0    12431 2023-07-31 02:59:56.786376 reflex-0.2.3a9/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a9/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a9/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a9/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a9/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a9/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a9/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a9/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a9/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a9/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a9/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a9/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a9/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9598 2023-07-31 02:59:56.786564 reflex-0.2.3a9/reflex/model.py
+-rw-r--r--   0        0        0     1832 2023-07-27 23:45:03.455818 reflex-0.2.3a9/reflex/page.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a9/reflex/py.typed
+-rw-r--r--   0        0        0    10623 2023-07-31 02:59:56.786732 reflex-0.2.3a9/reflex/reflex.py
+-rw-r--r--   0        0        0     3934 2023-07-27 23:45:03.456240 reflex-0.2.3a9/reflex/route.py
+-rw-r--r--   0        0        0    32524 2023-07-29 03:11:02.108051 reflex-0.2.3a9/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a9/reflex/style.py
+-rw-r--r--   0        0        0    15133 2023-07-31 02:59:56.786903 reflex-0.2.3a9/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a9/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     6212 2023-07-31 02:59:56.787060 reflex-0.2.3a9/reflex/utils/build.py
+-rw-r--r--   0        0        0     3964 2023-07-31 02:59:56.787200 reflex-0.2.3a9/reflex/utils/console.py
+-rw-r--r--   0        0        0     3774 2023-07-31 02:59:56.787338 reflex-0.2.3a9/reflex/utils/exec.py
+-rw-r--r--   0        0        0    12342 2023-07-29 01:05:18.597732 reflex-0.2.3a9/reflex/utils/format.py
+-rw-r--r--   0        0        0      590 2023-07-27 23:45:03.457502 reflex-0.2.3a9/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a9/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    16616 2023-07-31 02:59:56.787507 reflex-0.2.3a9/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     6485 2023-07-31 02:59:56.787667 reflex-0.2.3a9/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a9/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a9/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a9/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a9/reflex/vars.py
+-rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a9/PKG-INFO
```

### Comparing `reflex-0.2.3a8/LICENSE` & `reflex-0.2.3a9/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/README.md` & `reflex-0.2.3a9/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/pyproject.toml` & `reflex-0.2.3a9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.3a8"
+version = "0.2.3a9"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.3a8/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.3a9/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/apps/default/default.py` & `reflex-0.2.3a9/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/assets/favicon.ico` & `reflex-0.2.3a9/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.3a9/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.3a9/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/web/bun.lockb` & `reflex-0.2.3a9/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/web/package.json` & `reflex-0.2.3a9/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/web/pages/_app.js` & `reflex-0.2.3a9/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.3a9/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/.templates/web/utils/state.js` & `reflex-0.2.3a9/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/__init__.py` & `reflex-0.2.3a9/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/app.py` & `reflex-0.2.3a9/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/base.py` & `reflex-0.2.3a9/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/compiler/compiler.py` & `reflex-0.2.3a9/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/compiler/templates.py` & `reflex-0.2.3a9/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/compiler/utils.py` & `reflex-0.2.3a9/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/__init__.py` & `reflex-0.2.3a9/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/base/bare.py` & `reflex-0.2.3a9/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/base/document.py` & `reflex-0.2.3a9/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/base/link.py` & `reflex-0.2.3a9/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/base/meta.py` & `reflex-0.2.3a9/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/base/script.py` & `reflex-0.2.3a9/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/component.py` & `reflex-0.2.3a9/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/code.py` & `reflex-0.2.3a9/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/datatable.py` & `reflex-0.2.3a9/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/divider.py` & `reflex-0.2.3a9/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/list.py` & `reflex-0.2.3a9/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/stat.py` & `reflex-0.2.3a9/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/table.py` & `reflex-0.2.3a9/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/datadisplay/tag.py` & `reflex-0.2.3a9/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/disclosure/accordion.py` & `reflex-0.2.3a9/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/disclosure/tabs.py` & `reflex-0.2.3a9/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/disclosure/transition.py` & `reflex-0.2.3a9/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/feedback/alert.py` & `reflex-0.2.3a9/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/feedback/circularprogress.py` & `reflex-0.2.3a9/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/feedback/progress.py` & `reflex-0.2.3a9/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/feedback/skeleton.py` & `reflex-0.2.3a9/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/feedback/spinner.py` & `reflex-0.2.3a9/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/__init__.py` & `reflex-0.2.3a9/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/button.py` & `reflex-0.2.3a9/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/checkbox.py` & `reflex-0.2.3a9/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.3a9/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.3a9/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/debounce.py` & `reflex-0.2.3a9/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/editable.py` & `reflex-0.2.3a9/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/form.py` & `reflex-0.2.3a9/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/iconbutton.py` & `reflex-0.2.3a9/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/input.py` & `reflex-0.2.3a9/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/multiselect.py` & `reflex-0.2.3a9/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/numberinput.py` & `reflex-0.2.3a9/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/pininput.py` & `reflex-0.2.3a9/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/radio.py` & `reflex-0.2.3a9/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/rangeslider.py` & `reflex-0.2.3a9/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/select.py` & `reflex-0.2.3a9/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/slider.py` & `reflex-0.2.3a9/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/switch.py` & `reflex-0.2.3a9/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/textarea.py` & `reflex-0.2.3a9/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/forms/upload.py` & `reflex-0.2.3a9/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/graphing/plotly.py` & `reflex-0.2.3a9/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/graphing/victory.py` & `reflex-0.2.3a9/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/__init__.py` & `reflex-0.2.3a9/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/box.py` & `reflex-0.2.3a9/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/card.py` & `reflex-0.2.3a9/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/cond.py` & `reflex-0.2.3a9/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/flex.py` & `reflex-0.2.3a9/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/foreach.py` & `reflex-0.2.3a9/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/grid.py` & `reflex-0.2.3a9/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/html.py` & `reflex-0.2.3a9/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/responsive.py` & `reflex-0.2.3a9/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/stack.py` & `reflex-0.2.3a9/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/layout/wrap.py` & `reflex-0.2.3a9/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/libs/react_player.py` & `reflex-0.2.3a9/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/media/avatar.py` & `reflex-0.2.3a9/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/media/icon.py` & `reflex-0.2.3a9/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/media/image.py` & `reflex-0.2.3a9/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.3a9/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/navigation/link.py` & `reflex-0.2.3a9/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.3a9/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/navigation/stepper.py` & `reflex-0.2.3a9/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/__init__.py` & `reflex-0.2.3a9/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/alertdialog.py` & `reflex-0.2.3a9/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/banner.py` & `reflex-0.2.3a9/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/drawer.py` & `reflex-0.2.3a9/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/menu.py` & `reflex-0.2.3a9/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/modal.py` & `reflex-0.2.3a9/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/popover.py` & `reflex-0.2.3a9/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/overlay/tooltip.py` & `reflex-0.2.3a9/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/tags/iter_tag.py` & `reflex-0.2.3a9/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/tags/tag.py` & `reflex-0.2.3a9/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/tags/tagless.py` & `reflex-0.2.3a9/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/typography/highlight.py` & `reflex-0.2.3a9/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/components/typography/markdown.py` & `reflex-0.2.3a9/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/config.py` & `reflex-0.2.3a9/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/constants.py` & `reflex-0.2.3a9/reflex/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,14 @@
     """The log levels."""
 
     DEBUG = "debug"
     INFO = "info"
     WARNING = "warning"
     ERROR = "error"
     CRITICAL = "critical"
-    QUIET = "quiet"
 
     def __le__(self, other: LogLevel) -> bool:
         """Compare log levels.
 
         Args:
             other: The other log level.
```

### Comparing `reflex-0.2.3a8/reflex/el/constants/html.py` & `reflex-0.2.3a9/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/el/constants/react.py` & `reflex-0.2.3a9/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/el/constants/reflex.py` & `reflex-0.2.3a9/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/el/element.py` & `reflex-0.2.3a9/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/el/elements/__init__.py` & `reflex-0.2.3a9/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/el/precompile.py` & `reflex-0.2.3a9/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/event.py` & `reflex-0.2.3a9/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.3a9/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/middleware/middleware.py` & `reflex-0.2.3a9/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/model.py` & `reflex-0.2.3a9/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/page.py` & `reflex-0.2.3a9/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/reflex.py` & `reflex-0.2.3a9/reflex/reflex.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 ):
     """Reflex CLI to create, run, and deploy apps."""
     pass
 
 
 @cli.command()
 def init(
-    name: str = typer.Option(None, help="Name of the app to be initialized."),
+    name: str = typer.Option(
+        None, metavar="APP_NAME", help="The name of the app to be initialized."
+    ),
     template: constants.Template = typer.Option(
-        constants.Template.DEFAULT, help="Template to use for the app."
+        constants.Template.DEFAULT, help="The template to initialize the app with."
     ),
     loglevel: constants.LogLevel = typer.Option(
         constants.LogLevel.INFO, help="The log level to use."
     ),
 ):
     """Initialize a new Reflex app in the current directory."""
     # Set the log level.
@@ -103,17 +105,14 @@
         constants.LogLevel.INFO, help="The log level to use."
     ),
 ):
     """Run the app in the current directory."""
     # Set the log level.
     console.set_log_level(loglevel)
 
-    # Check that the app is initialized.
-    prerequisites.check_initialized(frontend=frontend)
-
     # Set ports as os env variables to take precedence over config and
     # .env variables(if override_os_envs flag in config is set to False).
     build.set_os_env(
         frontend_port=frontend_port,
         backend_port=backend_port,
         backend_host=backend_host,
     )
@@ -125,14 +124,17 @@
     backend_host = config.backend_host if backend_host is None else backend_host
 
     # If no --frontend-only and no --backend-only, then turn on frontend and backend both
     if not frontend and not backend:
         frontend = True
         backend = True
 
+    # Check that the app is initialized.
+    prerequisites.check_initialized(frontend=frontend)
+
     # If something is running on the ports, ask the user if they want to kill or change it.
     if frontend and processes.is_process_on_port(frontend_port):
         frontend_port = processes.change_or_terminate_port(frontend_port, "frontend")
 
     if backend and processes.is_process_on_port(backend_port):
         backend_port = processes.change_or_terminate_port(backend_port, "backend")
```

### Comparing `reflex-0.2.3a8/reflex/route.py` & `reflex-0.2.3a9/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/state.py` & `reflex-0.2.3a9/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/style.py` & `reflex-0.2.3a9/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/testing.py` & `reflex-0.2.3a9/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/utils/build.py` & `reflex-0.2.3a9/reflex/utils/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     ]
 
     # Start the subprocess with the progress bar.
     process = new_process(
         [prerequisites.get_package_manager(), "run", command],
         cwd=constants.WEB_DIR,
     )
-    show_progress(process, "Creating Production Build", checkpoints)
+    show_progress("Creating Production Build", process, checkpoints)
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
```

### Comparing `reflex-0.2.3a8/reflex/utils/console.py` & `reflex-0.2.3a9/reflex/utils/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,15 @@
 def rule(title: str, **kwargs):
     """Prints a horizontal rule with a title.
 
     Args:
         title: The title of the rule.
         kwargs: Keyword arguments to pass to the print function.
     """
-    if LOG_LEVEL <= LogLevel.INFO:
-        _console.rule(title, **kwargs)
+    _console.rule(title, **kwargs)
 
 
 def warn(msg: str, **kwargs):
     """Print a warning message.
 
     Args:
         msg: The warning message.
@@ -150,7 +149,20 @@
         A new progress bar.
     """
     return Progress(
         *Progress.get_default_columns()[:-1],
         MofNCompleteColumn(),
         TimeElapsedColumn(),
     )
+
+
+def status(*args, **kwargs):
+    """Create a status with a spinner.
+
+    Args:
+        *args: Args to pass to the status.
+        **kwargs: Kwargs to pass to the status.
+
+    Returns:
+        A new status.
+    """
+    return _console.status(*args, **kwargs)
```

### Comparing `reflex-0.2.3a8/reflex/utils/exec.py` & `reflex-0.2.3a9/reflex/utils/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Everything regarding execution of the built app."""
 
 from __future__ import annotations
 
 import os
-import platform
 from pathlib import Path
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites, processes
 from reflex.utils.processes import new_process
 from reflex.utils.watch import AssetFolderWatch
@@ -36,15 +35,15 @@
         cwd=constants.WEB_DIR,
     )
 
     if process.stdout:
         for line in process.stdout:
             if "ready started server on" in line:
                 url = line.split("url: ")[-1].strip()
-                console.info(f"App running at: [bold green]{url}")
+                console.print(f"App running at: [bold green]{url}")
             else:
                 console.debug(line)
 
 
 def run_frontend(
     root: Path,
     port: str,
@@ -135,15 +134,15 @@
             *constants.RUN_BACKEND_PROD_WINDOWS,
             "--host",
             host,
             "--port",
             str(port),
             f"{app_name}:{constants.APP_VAR}",
         ]
-        if platform.system() == "Windows"
+        if prerequisites.IS_WINDOWS
         else [
             *constants.RUN_BACKEND_PROD,
             "--bind",
             f"{host}:{port}",
             "--threads",
             str(num_workers),
             f"{app_name}:{constants.APP_VAR}()",
```

### Comparing `reflex-0.2.3a8/reflex/utils/format.py` & `reflex-0.2.3a9/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/utils/imports.py` & `reflex-0.2.3a9/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/utils/path_ops.py` & `reflex-0.2.3a9/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/utils/prerequisites.py` & `reflex-0.2.3a9/reflex/utils/prerequisites.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from alembic.util.exc import CommandError
 from packaging import version
 from redis import Redis
 
 from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import console, path_ops
-from reflex.utils.processes import new_process, show_logs
+from reflex.utils.processes import new_process, show_logs, show_status
 
 IS_WINDOWS = platform.system() == "Windows"
 
 
 def check_node_version() -> bool:
     """Check the version of Node.js.
 
@@ -86,15 +86,15 @@
 
     Returns:
         The path to the package manager.
     """
     get_config()
 
     # On Windows, we use npm instead of bun.
-    if platform.system() == "Windows":
+    if IS_WINDOWS:
         return get_windows_package_manager()
 
     # On other platforms, we use bun.
     return constants.BUN_PATH
 
 
 def get_package_manager() -> str:
@@ -102,15 +102,15 @@
       currently on unix systems, npm is used for running the app only.
 
     Returns:
         The path to the package manager.
     """
     get_config()
 
-    if platform.system() == "Windows":
+    if IS_WINDOWS:
         return get_windows_package_manager()
     return constants.NPM_PATH
 
 
 def get_app() -> ModuleType:
     """Get the app module based on the default config.
 
@@ -293,18 +293,15 @@
 
     # Save the script to a temporary file.
     script = tempfile.NamedTemporaryFile()
     with open(script.name, "w") as f:
         f.write(response.text)
 
     # Run the script.
-    env = {
-        **os.environ,
-        **env,
-    }
+    env = {**os.environ, **env}
     process = new_process(["bash", f.name, *args], env=env)
     show_logs(f"Installing {url}", process)
 
 
 def install_node():
     """Install nvm and nodejs for use by Reflex.
        Independent of any existing system installations.
@@ -366,27 +363,27 @@
     )
 
 
 def install_frontend_packages():
     """Installs the base and custom frontend packages."""
     # Install the base packages.
     process = new_process(
-        [get_install_package_manager(), "install"],
+        [get_install_package_manager(), "install", "--loglevel", "silly"],
         cwd=constants.WEB_DIR,
     )
-    show_logs("Installing base frontend packages", process)
+    show_status("Installing base frontend packages", process)
 
     # Install the app packages.
     packages = get_config().frontend_packages
     if len(packages) > 0:
         process = new_process(
             [get_install_package_manager(), "add", *packages],
             cwd=constants.WEB_DIR,
         )
-        show_logs("Installing custom frontend packages", process)
+        show_status("Installing custom frontend packages", process)
 
 
 def check_initialized(frontend: bool = True):
     """Check that the app is initialized.
 
     Args:
         frontend: Whether to check if the frontend is initialized.
```

### Comparing `reflex-0.2.3a8/reflex/utils/processes.py` & `reflex-0.2.3a9/reflex/utils/processes.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from __future__ import annotations
 
 import contextlib
 import os
 import signal
 import subprocess
 import sys
-from typing import Callable, List, Optional
+from typing import List, Optional
 from urllib.parse import urlparse
 
 import psutil
-import typer
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites
 
 
 def kill(pid):
@@ -132,93 +131,106 @@
         run: Whether to run the process to completion.
         show_logs: Whether to show the logs of the process.
         **kwargs: Kwargs to override default wrap values to pass to subprocess.Popen as arguments.
 
     Returns:
         Execute a child program in a new process.
     """
+    # Add the node bin path to the PATH environment variable.
     env = {
         **os.environ,
         "PATH": os.pathsep.join([constants.NODE_BIN_PATH, os.environ["PATH"]]),
     }
     kwargs = {
         "env": env,
         "stderr": None if show_logs else subprocess.STDOUT,
         "stdout": None if show_logs else subprocess.PIPE,
         "universal_newlines": True,
         "encoding": "UTF-8",
         **kwargs,
     }
-    console.debug(f"Running command: {args} with kwargs: {kwargs}")
+    console.debug(f"Running command: {args}")
     fn = subprocess.run if run else subprocess.Popen
     return fn(args, **kwargs)
 
 
-def show_progress(process: subprocess.Popen, message: str, checkpoints: List[str]):
-    """Show a progress bar for a process.
+def stream_logs(
+    message: str,
+    process: subprocess.Popen,
+):
+    """Stream the logs for a process.
 
     Args:
-        process: The process.
         message: The message to display.
-        checkpoints: The checkpoints to advance the progress bar.
-    """
-    # Create a progress object
-    progress = console.progress()
-    task = progress.add_task(f"{message}: ", total=len(checkpoints))
+        process: The process.
 
-    # Iterate over the process output.
-    try:
-        with progress, process:
-            if process.stdout is None:
-                return
-            for line in process.stdout:
-                console.debug(line, end="")
-
-                # Check for special strings and update the progress bar.
-                for special_string in checkpoints:
-                    if special_string in line:
-                        if special_string == checkpoints[-1]:
-                            progress.update(task, completed=len(checkpoints))
-                        else:
-                            progress.update(task, advance=1)
-                        break
+    Yields:
+        The lines of the process output.
+    """
+    with process:
+        console.debug(message)
+        if process.stdout is None:
+            return
+        for line in process.stdout:
+            console.debug(line, end="")
+            yield line
 
-    except Exception as e:
-        console.error(f"Error during {message} {e}")
+    if process.returncode != 0:
+        console.error(f"Error during {message}")
         console.error(
             "Run in with [bold]--loglevel debug[/bold] to see the full error."
         )
-        typer.Exit(1)
+        os._exit(1)
 
 
 def show_logs(
-    message: str, process: subprocess.Popen, logger: Callable = console.debug
+    message: str,
+    process: subprocess.Popen,
 ):
     """Show the logs for a process.
 
     Args:
         message: The message to display.
         process: The process.
-        logger: The log function to use.
     """
-    # TODO: refactor this function with show_progress
-    # Iterate over the process output.
-    try:
-        with process:
-            if process.stdout is None:
-                return
-            for line in process.stdout:
-                logger(line, end="")
+    for _ in stream_logs(message, process):
+        pass
 
-    except Exception as e:
-        console.error(f"Error during {message} {e}")
-        console.error(
-            "Run in with [bold]--loglevel debug[/bold] to see the full error."
-        )
-        typer.Exit(1)
+
+def show_status(message: str, process: subprocess.Popen):
+    """Show the status of a process.
+
+    Args:
+        message: The initial message to display.
+        process: The process.
+    """
+    with console.status(message) as status:
+        for line in stream_logs(message, process):
+            status.update(f"{message}: {line}")
+
+
+def show_progress(message: str, process: subprocess.Popen, checkpoints: List[str]):
+    """Show a progress bar for a process.
+
+    Args:
+        message: The message to display.
+        process: The process.
+        checkpoints: The checkpoints to advance the progress bar.
+    """
+    # Iterate over the process output.
+    with console.progress() as progress:
+        task = progress.add_task(f"{message}: ", total=len(checkpoints))
+        for line in stream_logs(message, process):
+            # Check for special strings and update the progress bar.
+            for special_string in checkpoints:
+                if special_string in line:
+                    progress.update(task, advance=1)
+                    if special_string == checkpoints[-1]:
+                        progress.update(task, completed=len(checkpoints))
+                    break
 
 
 def catch_keyboard_interrupt(signal, frame):
     """Display a custom message with the current time when exiting an app.
 
     Args:
         signal: The keyboard interrupt signal.
```

### Comparing `reflex-0.2.3a8/reflex/utils/telemetry.py` & `reflex-0.2.3a9/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/utils/types.py` & `reflex-0.2.3a9/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/utils/watch.py` & `reflex-0.2.3a9/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/reflex/vars.py` & `reflex-0.2.3a9/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a8/PKG-INFO` & `reflex-0.2.3a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.3a8
+Version: 0.2.3a9
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

