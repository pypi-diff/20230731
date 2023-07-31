# Comparing `tmp/systembridgefrontend-3.8.0.dev9.tar.gz` & `tmp/systembridgefrontend-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgefrontend-3.8.0.dev9.tar", last modified: Tue Jul 18 14:37:54 2023, max compression
+gzip compressed data, was "systembridgefrontend-3.8.1.tar", last modified: Mon Jul 31 14:20:24 2023, max compression
```

## Comparing `systembridgefrontend-3.8.0.dev9.tar` & `systembridgefrontend-3.8.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.535525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 14:37:53.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.535525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.535525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.535525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.543525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    60819 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/134-be8afb194db80d1f.js
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js
--rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js
--rw-r--r--   0 runner    (1001) docker     (123)   116154 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js
--rw-r--r--   0 runner    (1001) docker     (123)    69763 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/498-c0ac8cca5a5197e4.js
--rw-r--r--   0 runner    (1001) docker     (123)    54369 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/514-17895623628db944.js
--rw-r--r--   0 runner    (1001) docker     (123)    69853 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js
--rw-r--r--   0 runner    (1001) docker     (123)    56876 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/713-76d25fee0de05077.js
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js
--rw-r--r--   0 runner    (1001) docker     (123)    23306 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/731-b6cafe94e88ed8c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    58300 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   140978 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js
--rw-r--r--   0 runner    (1001) docker     (123)    98361 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/main-2ecf43899f8683c2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.543525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    51899 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.543525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.543525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.543525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
--rw-r--r--   0 runner    (1001) docker     (123)    91381 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.543525 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/sSLrbmPkLTT_gNozLHC0I/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/bridges/openon.html
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/bridges/setup.html
--rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/data.html
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/notification.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.547526 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/player/audio.html
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/player/video.html
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-18 14:37:19.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-18 14:37:18.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:54.535525 systembridgefrontend-3.8.0.dev9/systembridgefrontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-18 14:37:54.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-18 14:37:54.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:37:54.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 14:37:54.000000 systembridgefrontend-3.8.0.dev9/systembridgefrontend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-31 14:19:47.000000 systembridgefrontend-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 14:19:47.000000 systembridgefrontend-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.750465 systembridgefrontend-3.8.1/systembridgefrontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-31 14:19:47.000000 systembridgefrontend-3.8.1/systembridgefrontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-31 14:19:47.000000 systembridgefrontend-3.8.1/systembridgefrontend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.750465 systembridgefrontend-3.8.1/systembridgefrontend/out/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.750465 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.750465 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.750465 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/E7eXuapuFPIf8l3VFcw-l/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.754466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    60769 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/134-1ec0772e58be8d0c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js
+-rw-r--r--   0 runner    (1001) docker     (123)   116154 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69763 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/498-4e8ce630a90e85c2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    54363 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/514-87c66909ad150ba9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69853 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56872 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/713-b2b4846010d39d53.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24483 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/731-8a6748b651b08a0a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58286 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/75fc9c18-6f0090aa3d354e90.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   140978 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js
+-rw-r--r--   0 runner    (1001) docker     (123)    98803 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/main-92011a1a7f336a6f.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.754466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    51875 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/_app-08072decd7c39068.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91381 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-31 14:19:49.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/bridges/openon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/bridges/setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/notification.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.758466 systembridgefrontend-3.8.1/systembridgefrontend/out/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/player/audio.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/player/video.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-31 14:19:50.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/app/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-31 14:19:48.000000 systembridgefrontend-3.8.1/systembridgefrontend/out/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:24.750465 systembridgefrontend-3.8.1/systembridgefrontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 14:20:24.000000 systembridgefrontend-3.8.1/systembridgefrontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-31 14:20:24.000000 systembridgefrontend-3.8.1/systembridgefrontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:20:24.000000 systembridgefrontend-3.8.1/systembridgefrontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 14:20:24.000000 systembridgefrontend-3.8.1/systembridgefrontend.egg-info/top_level.txt
```

### Comparing `systembridgefrontend-3.8.0.dev9/pyproject.toml` & `systembridgefrontend-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/setup.py` & `systembridgefrontend-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/404.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/404.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/134-be8afb194db80d1f.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/134-1ec0772e58be8d0c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2488,24 +2488,24 @@
                     let n = {};
                     return r.forEach(e => {
                         let t = c(e.props);
                         n[t] = e.style
                     }), n
                 },
                 h = (e, t, r, n) => {
-                    var o, i;
+                    var o;
                     let {
-                        ownerState: a = {}
-                    } = e, l = [], s = null == r ? void 0 : null == (o = r.components) ? void 0 : null == (i = o[n]) ? void 0 : i.variants;
-                    return s && s.forEach(r => {
+                        ownerState: i = {}
+                    } = e, a = [], l = null == r || null == (o = r.components) || null == (o = o[n]) ? void 0 : o.variants;
+                    return l && l.forEach(r => {
                         let n = !0;
                         Object.keys(r.props).forEach(t => {
-                            a[t] !== r.props[t] && e[t] !== r.props[t] && (n = !1)
-                        }), n && l.push(t[c(r.props)])
-                    }), l
+                            i[t] !== r.props[t] && e[t] !== r.props[t] && (n = !1)
+                        }), n && a.push(t[c(r.props)])
+                    }), a
                 };
 
             function v(e) {
                 return "ownerState" !== e && "theme" !== e && "sx" !== e && "as" !== e
             }
             let g = (0, a.Z)();
 
@@ -2605,15 +2605,15 @@
             let l = ["sx"],
                 s = e => {
                     var t, r;
                     let n = {
                             systemProps: {},
                             otherProps: {}
                         },
-                        o = null != (t = null == e ? void 0 : null == (r = e.theme) ? void 0 : r.unstable_sxConfig) ? t : a.Z;
+                        o = null != (t = null == e || null == (r = e.theme) ? void 0 : r.unstable_sxConfig) ? t : a.Z;
                     return Object.keys(e).forEach(t => {
                         o[t] ? n.systemProps[t] = e[t] : n.otherProps[t] = e[t]
                     }), n
                 };
 
             function u(e) {
                 let t;
@@ -2749,23 +2749,17 @@
             "use strict";
             var n = r(7294);
             let o = "undefined" != typeof window ? n.useLayoutEffect : n.useEffect;
             t.Z = o
         },
         9948: function(e, t, r) {
             "use strict";
-            r.d(t, {
-                Z: function() {
-                    return i
-                }
-            });
             var n = r(7294),
                 o = r(3546);
-
-            function i(e) {
+            t.Z = function(e) {
                 let t = n.useRef(e);
                 return (0, o.Z)(() => {
                     t.current = e
                 }), n.useCallback((...e) => (0, t.current)(...e), [])
             }
         },
         3703: function(e, t, r) {
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/498-c0ac8cca5a5197e4.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/498-4e8ce630a90e85c2.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -11,21 +11,21 @@
                 i = o(7462),
                 n = o(7294),
                 a = o(3680),
                 l = o(4780),
                 s = o(917),
                 c = o(8216),
                 u = o(1657),
-                d = o(948),
-                f = o(1588),
+                f = o(948),
+                d = o(1588),
                 m = o(4867);
 
             function v(r) {
                 return (0, m.Z)("MuiCircularProgress", r)
-            }(0, f.Z)("MuiCircularProgress", ["root", "determinate", "indeterminate", "colorPrimary", "colorSecondary", "svg", "circle", "circleDeterminate", "circleIndeterminate", "circleDisableShrink"]);
+            }(0, d.Z)("MuiCircularProgress", ["root", "determinate", "indeterminate", "colorPrimary", "colorSecondary", "svg", "circle", "circleDeterminate", "circleIndeterminate", "circleDisableShrink"]);
             var h = o(5893);
             let p = ["className", "color", "disableShrink", "size", "style", "thickness", "value", "variant"],
                 S = r => r,
                 Z, y, g, b, x = (0, s.F4)(Z || (Z = S`
   0% {
     transform: rotate(0deg);
   }
@@ -59,15 +59,15 @@
                     } = r, n = {
                         root: ["root", o, `color${(0,c.Z)(t)}`],
                         svg: ["svg"],
                         circle: ["circle", `circle${(0,c.Z)(o)}`, i && "circleDisableShrink"]
                     };
                     return (0, l.Z)(n, v, e)
                 },
-                z = (0, d.ZP)("span", {
+                z = (0, f.ZP)("span", {
                     name: "MuiCircularProgress",
                     slot: "Root",
                     overridesResolver: (r, e) => {
                         let {
                             ownerState: o
                         } = r;
                         return [e.root, e[o.variant], e[`color${(0,c.Z)(o.color)}`]]
@@ -82,22 +82,22 @@
                 }, "inherit" !== r.color && {
                     color: (e.vars || e).palette[r.color].main
                 }), ({
                     ownerState: r
                 }) => "indeterminate" === r.variant && (0, s.iv)(g || (g = S`
       animation: ${0} 1.4s linear infinite;
     `), x)),
-                C = (0, d.ZP)("svg", {
+                C = (0, f.ZP)("svg", {
                     name: "MuiCircularProgress",
                     slot: "Svg",
                     overridesResolver: (r, e) => e.svg
                 })({
                     display: "block"
                 }),
-                M = (0, d.ZP)("circle", {
+                M = (0, f.ZP)("circle", {
                     name: "MuiCircularProgress",
                     slot: "Circle",
                     overridesResolver: (r, e) => {
                         let {
                             ownerState: o
                         } = r;
                         return [e.circle, e[`circle${(0,c.Z)(o.variant)}`], o.disableShrink && e.circleDisableShrink]
@@ -123,59 +123,59 @@
                             name: "MuiCircularProgress"
                         }),
                         {
                             className: n,
                             color: l = "primary",
                             disableShrink: s = !1,
                             size: c = 40,
-                            style: d,
-                            thickness: f = 3.6,
+                            style: f,
+                            thickness: d = 3.6,
                             value: m = 0,
                             variant: v = "indeterminate"
                         } = o,
                         S = (0, t.Z)(o, p),
                         Z = (0, i.Z)({}, o, {
                             color: l,
                             disableShrink: s,
                             size: c,
-                            thickness: f,
+                            thickness: d,
                             value: m,
                             variant: v
                         }),
                         y = w(Z),
                         g = {},
                         b = {},
                         x = {};
                     if ("determinate" === v) {
-                        let r = 2 * Math.PI * ((44 - f) / 2);
+                        let r = 2 * Math.PI * ((44 - d) / 2);
                         g.strokeDasharray = r.toFixed(3), x["aria-valuenow"] = Math.round(m), g.strokeDashoffset = `${((100-m)/100*r).toFixed(3)}px`, b.transform = "rotate(-90deg)"
                     }
                     return (0, h.jsx)(z, (0, i.Z)({
                         className: (0, a.Z)(y.root, n),
                         style: (0, i.Z)({
                             width: c,
                             height: c
-                        }, b, d),
+                        }, b, f),
                         ownerState: Z,
                         ref: e,
                         role: "progressbar"
                     }, x, S, {
                         children: (0, h.jsx)(C, {
                             className: y.svg,
                             ownerState: Z,
                             viewBox: "22 22 44 44",
                             children: (0, h.jsx)(M, {
                                 className: y.circle,
                                 style: g,
                                 ownerState: Z,
                                 cx: 44,
                                 cy: 44,
-                                r: (44 - f) / 2,
+                                r: (44 - d) / 2,
                                 fill: "none",
-                                strokeWidth: f
+                                strokeWidth: d
                             })
                         })
                     }))
                 });
             var R = P
         },
         8169: function(r, e, o) {
@@ -188,20 +188,20 @@
                 i = o(7294),
                 n = o(3366),
                 a = o(3680),
                 l = o(4780),
                 s = o(8216),
                 c = o(1657),
                 u = o(948),
-                d = o(1588),
-                f = o(4867);
+                f = o(1588),
+                d = o(4867);
 
             function m(r) {
-                return (0, f.Z)("MuiSvgIcon", r)
-            }(0, d.Z)("MuiSvgIcon", ["root", "colorPrimary", "colorSecondary", "colorAction", "colorError", "colorDisabled", "fontSizeInherit", "fontSizeSmall", "fontSizeMedium", "fontSizeLarge"]);
+                return (0, d.Z)("MuiSvgIcon", r)
+            }(0, f.Z)("MuiSvgIcon", ["root", "colorPrimary", "colorSecondary", "colorAction", "colorError", "colorDisabled", "fontSizeInherit", "fontSizeSmall", "fontSizeMedium", "fontSizeLarge"]);
             var v = o(5893);
             let h = ["children", "className", "color", "component", "fontSize", "htmlColor", "inheritViewBox", "titleAccess", "viewBox"],
                 p = r => {
                     let {
                         color: e,
                         fontSize: o,
                         classes: t
@@ -219,70 +219,70 @@
                         } = r;
                         return [e.root, "inherit" !== o.color && e[`color${(0,s.Z)(o.color)}`], e[`fontSize${(0,s.Z)(o.fontSize)}`]]
                     }
                 })(({
                     theme: r,
                     ownerState: e
                 }) => {
-                    var o, t, i, n, a, l, s, c, u, d, f, m, v, h, p, S, Z;
+                    var o, t, i, n, a, l, s, c, u, f, d, m, v;
                     return {
                         userSelect: "none",
                         width: "1em",
                         height: "1em",
                         display: "inline-block",
                         fill: e.hasSvgAsChild ? void 0 : "currentColor",
                         flexShrink: 0,
-                        transition: null == (o = r.transitions) ? void 0 : null == (t = o.create) ? void 0 : t.call(o, "fill", {
-                            duration: null == (i = r.transitions) ? void 0 : null == (n = i.duration) ? void 0 : n.shorter
+                        transition: null == (o = r.transitions) || null == (t = o.create) ? void 0 : t.call(o, "fill", {
+                            duration: null == (i = r.transitions) || null == (i = i.duration) ? void 0 : i.shorter
                         }),
                         fontSize: ({
                             inherit: "inherit",
-                            small: (null == (a = r.typography) ? void 0 : null == (l = a.pxToRem) ? void 0 : l.call(a, 20)) || "1.25rem",
-                            medium: (null == (s = r.typography) ? void 0 : null == (c = s.pxToRem) ? void 0 : c.call(s, 24)) || "1.5rem",
-                            large: (null == (u = r.typography) ? void 0 : null == (d = u.pxToRem) ? void 0 : d.call(u, 35)) || "2.1875rem"
+                            small: (null == (n = r.typography) || null == (a = n.pxToRem) ? void 0 : a.call(n, 20)) || "1.25rem",
+                            medium: (null == (l = r.typography) || null == (s = l.pxToRem) ? void 0 : s.call(l, 24)) || "1.5rem",
+                            large: (null == (c = r.typography) || null == (u = c.pxToRem) ? void 0 : u.call(c, 35)) || "2.1875rem"
                         })[e.fontSize],
-                        color: null != (f = null == (m = (r.vars || r).palette) ? void 0 : null == (v = m[e.color]) ? void 0 : v.main) ? f : ({
-                            action: null == (h = (r.vars || r).palette) ? void 0 : null == (p = h.action) ? void 0 : p.active,
-                            disabled: null == (S = (r.vars || r).palette) ? void 0 : null == (Z = S.action) ? void 0 : Z.disabled,
+                        color: null != (f = null == (d = (r.vars || r).palette) || null == (d = d[e.color]) ? void 0 : d.main) ? f : ({
+                            action: null == (m = (r.vars || r).palette) || null == (m = m.action) ? void 0 : m.active,
+                            disabled: null == (v = (r.vars || r).palette) || null == (v = v.action) ? void 0 : v.disabled,
                             inherit: void 0
                         })[e.color]
                     }
                 }),
                 Z = i.forwardRef(function(r, e) {
                     let o = (0, c.Z)({
                             props: r,
                             name: "MuiSvgIcon"
                         }),
                         {
                             children: l,
                             className: s,
                             color: u = "inherit",
-                            component: d = "svg",
-                            fontSize: f = "medium",
+                            component: f = "svg",
+                            fontSize: d = "medium",
                             htmlColor: m,
                             inheritViewBox: Z = !1,
                             titleAccess: y,
                             viewBox: g = "0 0 24 24"
                         } = o,
                         b = (0, n.Z)(o, h),
                         x = i.isValidElement(l) && "svg" === l.type,
                         k = (0, t.Z)({}, o, {
                             color: u,
-                            component: d,
-                            fontSize: f,
+                            component: f,
+                            fontSize: d,
                             instanceFontSize: r.fontSize,
                             inheritViewBox: Z,
                             viewBox: g,
                             hasSvgAsChild: x
                         }),
                         w = {};
                     Z || (w.viewBox = g);
                     let z = p(k);
                     return (0, v.jsxs)(S, (0, t.Z)({
-                        as: d,
+                        as: f,
                         className: (0, a.Z)(z.root, s),
                         focusable: "false",
                         color: m,
                         "aria-hidden": !y || void 0,
                         role: y ? "img" : void 0,
                         ref: e
                     }, w, b, x && l.props, {
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/514-17895623628db944.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/514-87c66909ad150ba9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -84,15 +84,15 @@
             function O({
                 sliderRef: e,
                 activeIndex: t,
                 setActive: r
             }) {
                 var n, o, a;
                 let i = (0, f.Z)(e.current);
-                null != (n = e.current) && n.contains(i.activeElement) && Number(null == i ? void 0 : null == (o = i.activeElement) ? void 0 : o.getAttribute("data-index")) === t || null == (a = e.current) || a.querySelector(`[type="range"][data-index="${t}"]`).focus(), r && r(t)
+                null != (n = e.current) && n.contains(i.activeElement) && Number(null == i || null == (o = i.activeElement) ? void 0 : o.getAttribute("data-index")) === t || null == (a = e.current) || a.querySelector(`[type="range"][data-index="${t}"]`).focus(), r && r(t)
             }
 
             function S(e, t) {
                 return "number" == typeof e && "number" == typeof t ? e === t : "object" == typeof e && "object" == typeof t && function(e, t, r = (e, t) => e === t) {
                     return e.length === t.length && e.every((e, n) => r(e, t[n]))
                 }(e, t)
             }
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/713-76d25fee0de05077.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/713-b2b4846010d39d53.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1447,15 +1447,14 @@
                         justifyContent: "center",
                         height: 32,
                         color: (e.vars || e).palette.text.primary,
                         backgroundColor: (e.vars || e).palette.action.selected,
                         borderRadius: 16,
                         whiteSpace: "nowrap",
                         transition: e.transitions.create(["background-color", "box-shadow"]),
-                        cursor: "default",
                         outline: 0,
                         textDecoration: "none",
                         border: 0,
                         padding: 0,
                         verticalAlign: "middle",
                         boxSizing: "border-box",
                         [`&.${e8.disabled}`]: {
@@ -2256,15 +2255,15 @@
                                     let a = ee.current;
                                     if ("listbox" !== ee.current.getAttribute("role") && (a = ee.current.parentElement.querySelector('[role="listbox"]')), !a) return;
                                     if (-1 === t) {
                                         a.scrollTop = 0;
                                         return
                                     }
                                     let i = ee.current.querySelector(`[data-option-index="${t}"]`);
-                                    if (i && (i.classList.add(`${o}-focused`), "keyboard" === r && i.classList.add(`${o}-focusVisible`), a.scrollHeight > a.clientHeight && "mouse" !== r)) {
+                                    if (i && (i.classList.add(`${o}-focused`), "keyboard" === r && i.classList.add(`${o}-focusVisible`), a.scrollHeight > a.clientHeight && "mouse" !== r && "touch" !== r)) {
                                         let e = a.clientHeight + a.scrollTop,
                                             t = i.offsetTop + i.offsetHeight;
                                         t > e ? a.scrollTop = t - a.clientHeight : i.offsetTop - i.offsetHeight * (L ? 1.3 : 0) < a.scrollTop && (a.scrollTop = i.offsetTop - i.offsetHeight * (L ? 1.3 : 0))
                                     }
                                 }),
                                 eC = (0, b.Z)(({
                                     event: e,
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/731-b6cafe94e88ed8c7.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/731-8a6748b651b08a0a.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -102,20 +102,20 @@
                         b = (0, r.Z)({}, f, l, d, u);
                     return p.length > 0 && (b.className = p), Object.keys(h).length > 0 && (b.style = h), {
                         props: b,
                         internalRef: f.ref
                     }
                 }((0, r.Z)({}, b, {
                     externalSlotProps: m
-                })), Z = (0, n.Z)(y, null == m ? void 0 : m.ref, null == (t = e.additionalProps) ? void 0 : t.ref), g = (l = (0, r.Z)({}, v, {
-                    ref: Z
+                })), g = (0, n.Z)(y, null == m ? void 0 : m.ref, null == (t = e.additionalProps) ? void 0 : t.ref), Z = (l = (0, r.Z)({}, v, {
+                    ref: g
                 }), void 0 === d || (0, i.Z)(d) ? l : (0, r.Z)({}, l, {
                     ownerState: (0, r.Z)({}, l.ownerState, p)
                 }));
-                return g
+                return Z
             }
         },
         4267: function(e, t, l) {
             "use strict";
             l.d(t, {
                 Z: function() {
                     return y
@@ -214,15 +214,15 @@
                         disabled: u
                     } = e, d = {
                         root: ["root", n && i && "labelIcon", `textColor${(0,c.Z)(l)}`, r && "fullWidth", o && "wrapped", s && "selected", u && "disabled"],
                         iconWrapper: ["iconWrapper"]
                     };
                     return (0, a.Z)(d, h, t)
                 },
-                Z = (0, d.ZP)(s.Z, {
+                g = (0, d.ZP)(s.Z, {
                     name: "MuiTab",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [t.root, l.label && l.icon && t.labelIcon, t[`textColor${(0,c.Z)(l.textColor)}`], l.fullWidth && t.fullWidth, l.wrapped && t.wrapped]
@@ -286,29 +286,29 @@
                     flexShrink: 1,
                     flexGrow: 1,
                     flexBasis: 0,
                     maxWidth: "none"
                 }, t.wrapped && {
                     fontSize: e.typography.pxToRem(12)
                 })),
-                g = n.forwardRef(function(e, t) {
+                Z = n.forwardRef(function(e, t) {
                     let l = (0, u.Z)({
                             props: e,
                             name: "MuiTab"
                         }),
                         {
                             className: a,
                             disabled: s = !1,
                             disableFocusRipple: c = !1,
                             fullWidth: d,
                             icon: f,
                             iconPosition: p = "top",
                             indicator: h,
                             label: b,
-                            onChange: g,
+                            onChange: Z,
                             onClick: x,
                             onFocus: w,
                             selected: S,
                             selectionFollowsFocus: C,
                             textColor: _ = "inherit",
                             value: B,
                             wrapped: P = !1
@@ -325,45 +325,45 @@
                             textColor: _,
                             wrapped: P
                         }),
                         R = y(M),
                         T = f && b && n.isValidElement(f) ? n.cloneElement(f, {
                             className: (0, i.Z)(R.iconWrapper, f.props.className)
                         }) : f;
-                    return (0, m.jsxs)(Z, (0, o.Z)({
+                    return (0, m.jsxs)(g, (0, o.Z)({
                         focusRipple: !c,
                         className: (0, i.Z)(R.root, a),
                         ref: t,
                         role: "tab",
                         "aria-selected": S,
                         disabled: s,
                         onClick: e => {
-                            !S && g && g(e, B), x && x(e)
+                            !S && Z && Z(e, B), x && x(e)
                         },
                         onFocus: e => {
-                            C && !S && g && g(e, B), w && w(e)
+                            C && !S && Z && Z(e, B), w && w(e)
                         },
                         ownerState: M,
                         tabIndex: S ? 0 : -1
                     }, E, {
                         children: ["top" === p || "start" === p ? (0, m.jsxs)(n.Fragment, {
                             children: [T, b]
                         }) : (0, m.jsxs)(n.Fragment, {
                             children: [b, T]
                         }), h]
                     }))
                 });
-            var x = g
+            var x = Z
         },
         1703: function(e, t, l) {
             "use strict";
             let r;
             l.d(t, {
                 Z: function() {
-                    return K
+                    return q
                 }
             });
             var o = l(3366),
                 n = l(7462),
                 i = l(7294);
             l(9864);
             var a = l(3680),
@@ -377,152 +377,138 @@
             function h() {
                 if (r) return r;
                 let e = document.createElement("div"),
                     t = document.createElement("div");
                 return t.style.width = "10px", t.style.height = "1px", e.appendChild(t), e.dir = "rtl", e.style.fontSize = "14px", e.style.width = "4px", e.style.height = "1px", e.style.position = "absolute", e.style.top = "-1000px", e.style.overflow = "scroll", document.body.appendChild(e), r = "reverse", e.scrollLeft > 0 ? r = "default" : (e.scrollLeft = 1, 0 === e.scrollLeft && (r = "negative")), document.body.removeChild(e), r
             }
 
-            function b(e, t) {
-                let l = e.scrollLeft;
-                if ("rtl" !== t) return l;
-                let r = h();
-                switch (r) {
-                    case "negative":
-                        return e.scrollWidth - e.clientWidth + l;
-                    case "reverse":
-                        return e.scrollWidth - e.clientWidth - l;
-                    default:
-                        return l
-                }
-            }
-
-            function m(e) {
+            function b(e) {
                 return (1 + Math.sin(Math.PI * e - Math.PI / 2)) / 2
             }
-            var v = l(8974),
-                y = l(5340),
-                Z = l(5893);
+            var m = l(8974),
+                v = l(5340),
+                y = l(5893);
             let g = ["onChange"],
-                x = {
+                Z = {
                     width: 99,
                     height: 99,
                     position: "absolute",
                     top: -9999,
                     overflow: "scroll"
                 };
-            var w = l(8169),
-                S = (0, w.Z)((0, Z.jsx)("path", {
+            var x = l(8169),
+                w = (0, x.Z)((0, y.jsx)("path", {
                     d: "M15.41 16.09l-4.58-4.59 4.58-4.59L14 5.5l-6 6 6 6z"
                 }), "KeyboardArrowLeft"),
-                C = (0, w.Z)((0, Z.jsx)("path", {
+                S = (0, x.Z)((0, y.jsx)("path", {
                     d: "M8.59 16.34l4.58-4.59-4.58-4.59L10 5.75l6 6-6 6z"
                 }), "KeyboardArrowRight"),
-                _ = l(2022),
-                B = l(1588),
-                P = l(4867);
+                C = l(2022),
+                _ = l(1588),
+                B = l(4867);
 
-            function E(e) {
-                return (0, P.Z)("MuiTabScrollButton", e)
+            function P(e) {
+                return (0, B.Z)("MuiTabScrollButton", e)
             }
-            let M = (0, B.Z)("MuiTabScrollButton", ["root", "vertical", "horizontal", "disabled"]),
-                R = ["className", "slots", "slotProps", "direction", "orientation", "disabled"],
-                T = e => {
+            let E = (0, _.Z)("MuiTabScrollButton", ["root", "vertical", "horizontal", "disabled"]),
+                M = ["className", "slots", "slotProps", "direction", "orientation", "disabled"],
+                R = e => {
                     let {
                         classes: t,
                         orientation: l,
                         disabled: r
                     } = e;
                     return (0, s.Z)({
                         root: ["root", l, r && "disabled"]
-                    }, E, t)
+                    }, P, t)
                 },
-                k = (0, u.ZP)(_.Z, {
+                T = (0, u.ZP)(C.Z, {
                     name: "MuiTabScrollButton",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [t.root, l.orientation && t[l.orientation]]
                     }
                 })(({
                     ownerState: e
                 }) => (0, n.Z)({
                     width: 40,
                     flexShrink: 0,
                     opacity: .8,
-                    [`&.${M.disabled}`]: {
+                    [`&.${E.disabled}`]: {
                         opacity: 0
                     }
                 }, "vertical" === e.orientation && {
                     width: "100%",
                     height: 40,
                     "& svg": {
                         transform: `rotate(${e.isRtl?-90:90}deg)`
                     }
                 })),
-                N = i.forwardRef(function(e, t) {
+                k = i.forwardRef(function(e, t) {
                     var l, r;
                     let i = (0, d.Z)({
                             props: e,
                             name: "MuiTabScrollButton"
                         }),
                         {
                             className: s,
                             slots: u = {},
                             slotProps: p = {},
                             direction: h
                         } = i,
-                        b = (0, o.Z)(i, R),
+                        b = (0, o.Z)(i, M),
                         m = (0, f.Z)(),
                         v = "rtl" === m.direction,
-                        y = (0, n.Z)({
+                        g = (0, n.Z)({
                             isRtl: v
                         }, i),
-                        g = T(y),
-                        x = null != (l = u.StartScrollButtonIcon) ? l : S,
-                        w = null != (r = u.EndScrollButtonIcon) ? r : C,
+                        Z = R(g),
+                        x = null != (l = u.StartScrollButtonIcon) ? l : w,
+                        C = null != (r = u.EndScrollButtonIcon) ? r : S,
                         _ = (0, c.Z)({
                             elementType: x,
                             externalSlotProps: p.startScrollButtonIcon,
                             additionalProps: {
                                 fontSize: "small"
                             },
-                            ownerState: y
+                            ownerState: g
                         }),
                         B = (0, c.Z)({
-                            elementType: w,
+                            elementType: C,
                             externalSlotProps: p.endScrollButtonIcon,
                             additionalProps: {
                                 fontSize: "small"
                             },
-                            ownerState: y
+                            ownerState: g
                         });
-                    return (0, Z.jsx)(k, (0, n.Z)({
+                    return (0, y.jsx)(T, (0, n.Z)({
                         component: "div",
-                        className: (0, a.Z)(g.root, s),
+                        className: (0, a.Z)(Z.root, s),
                         ref: t,
                         role: null,
-                        ownerState: y,
+                        ownerState: g,
                         tabIndex: null
                     }, b, {
-                        children: "left" === h ? (0, Z.jsx)(x, (0, n.Z)({}, _)) : (0, Z.jsx)(w, (0, n.Z)({}, B))
+                        children: "left" === h ? (0, y.jsx)(x, (0, n.Z)({}, _)) : (0, y.jsx)(C, (0, n.Z)({}, B))
                     }))
                 });
-            var j = l(2068);
+            var N = l(2068);
 
-            function W(e) {
-                return (0, P.Z)("MuiTabs", e)
+            function j(e) {
+                return (0, B.Z)("MuiTabs", e)
             }
-            let I = (0, B.Z)("MuiTabs", ["root", "vertical", "flexContainer", "flexContainerVertical", "centered", "scroller", "fixed", "scrollableX", "scrollableY", "hideScrollbar", "scrollButtons", "scrollButtonsHideMobile", "indicator"]);
-            var L = l(8038);
+            let I = (0, _.Z)("MuiTabs", ["root", "vertical", "flexContainer", "flexContainerVertical", "centered", "scroller", "fixed", "scrollableX", "scrollableY", "hideScrollbar", "scrollButtons", "scrollButtonsHideMobile", "indicator"]);
+            var W = l(8038);
             let A = ["aria-label", "aria-labelledby", "action", "centered", "children", "className", "component", "allowScrollButtonsMobile", "indicatorColor", "onChange", "orientation", "ScrollButtonComponent", "scrollButtons", "selectionFollowsFocus", "slots", "slotProps", "TabIndicatorProps", "TabScrollButtonProps", "textColor", "value", "variant", "visibleScrollbar"],
-                z = (e, t) => e === t ? e.firstChild : t && t.nextElementSibling ? t.nextElementSibling : e.firstChild,
+                L = (e, t) => e === t ? e.firstChild : t && t.nextElementSibling ? t.nextElementSibling : e.firstChild,
                 O = (e, t) => e === t ? e.lastChild : t && t.previousElementSibling ? t.previousElementSibling : e.lastChild,
-                D = (e, t, l) => {
+                z = (e, t, l) => {
                     let r = !1,
                         o = l(e, t);
                     for (; o;) {
                         if (o === e.firstChild) {
                             if (r) return;
                             r = !0
                         }
@@ -530,15 +516,15 @@
                         if (!o.hasAttribute("tabindex") || t) o = l(e, o);
                         else {
                             o.focus();
                             return
                         }
                     }
                 },
-                H = e => {
+                D = e => {
                     let {
                         vertical: t,
                         fixed: l,
                         hideScrollbar: r,
                         scrollableX: o,
                         scrollableY: n,
                         centered: i,
@@ -549,17 +535,17 @@
                         root: ["root", t && "vertical"],
                         scroller: ["scroller", l && "fixed", r && "hideScrollbar", o && "scrollableX", n && "scrollableY"],
                         flexContainer: ["flexContainer", t && "flexContainerVertical", i && "centered"],
                         indicator: ["indicator"],
                         scrollButtons: ["scrollButtons", a && "scrollButtonsHideMobile"],
                         scrollableX: [o && "scrollableX"],
                         hideScrollbar: [r && "hideScrollbar"]
-                    }, W, c)
+                    }, j, c)
                 },
-                F = (0, u.ZP)("div", {
+                H = (0, u.ZP)("div", {
                     name: "MuiTabs",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [{
@@ -581,15 +567,15 @@
                 }, e.scrollButtonsHideMobile && {
                     [`& .${I.scrollButtons}`]: {
                         [t.breakpoints.down("sm")]: {
                             display: "none"
                         }
                     }
                 })),
-                $ = (0, u.ZP)("div", {
+                F = (0, u.ZP)("div", {
                     name: "MuiTabs",
                     slot: "Scroller",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [t.scroller, l.fixed && t.fixed, l.hideScrollbar && t.hideScrollbar, l.scrollableX && t.scrollableX, l.scrollableY && t.scrollableY]
@@ -612,15 +598,15 @@
                 }, e.scrollableX && {
                     overflowX: "auto",
                     overflowY: "hidden"
                 }, e.scrollableY && {
                     overflowY: "auto",
                     overflowX: "hidden"
                 })),
-                X = (0, u.ZP)("div", {
+                $ = (0, u.ZP)("div", {
                     name: "MuiTabs",
                     slot: "FlexContainer",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [t.flexContainer, l.vertical && t.flexContainerVertical, l.centered && t.centered]
@@ -630,15 +616,15 @@
                 }) => (0, n.Z)({
                     display: "flex"
                 }, e.vertical && {
                     flexDirection: "column"
                 }, e.centered && {
                     justifyContent: "center"
                 })),
-                V = (0, u.ZP)("span", {
+                X = (0, u.ZP)("span", {
                     name: "MuiTabs",
                     slot: "Indicator",
                     overridesResolver: (e, t) => t.indicator
                 })(({
                     ownerState: e,
                     theme: t
                 }) => (0, n.Z)({
@@ -652,184 +638,195 @@
                 }, "secondary" === e.indicatorColor && {
                     backgroundColor: (t.vars || t).palette.secondary.main
                 }, e.vertical && {
                     height: "100%",
                     width: 2,
                     right: 0
                 })),
-                Y = (0, u.ZP)(function(e) {
+                V = (0, u.ZP)(function(e) {
                     let {
                         onChange: t
                     } = e, l = (0, o.Z)(e, g), r = i.useRef(), a = i.useRef(null), s = () => {
                         r.current = a.current.offsetHeight - a.current.clientHeight
                     };
-                    return (0, v.Z)(() => {
+                    return (0, m.Z)(() => {
                         let e = (0, p.Z)(() => {
                                 let e = r.current;
                                 s(), e !== r.current && t(r.current)
                             }),
-                            l = (0, y.Z)(a.current);
+                            l = (0, v.Z)(a.current);
                         return l.addEventListener("resize", e), () => {
                             e.clear(), l.removeEventListener("resize", e)
                         }
                     }, [t]), i.useEffect(() => {
                         s(), t(r.current)
-                    }, [t]), (0, Z.jsx)("div", (0, n.Z)({
-                        style: x,
+                    }, [t]), (0, y.jsx)("div", (0, n.Z)({
+                        style: Z,
                         ref: a
                     }, l))
                 }, {
                     name: "MuiTabs",
                     slot: "ScrollbarSize"
                 })({
                     overflowX: "auto",
                     overflowY: "hidden",
                     scrollbarWidth: "none",
                     "&::-webkit-scrollbar": {
                         display: "none"
                     }
                 }),
-                G = {},
-                q = i.forwardRef(function(e, t) {
+                Y = {},
+                G = i.forwardRef(function(e, t) {
                     let l = (0, d.Z)({
                             props: e,
                             name: "MuiTabs"
                         }),
                         r = (0, f.Z)(),
                         s = "rtl" === r.direction,
                         {
                             "aria-label": u,
-                            "aria-labelledby": v,
+                            "aria-labelledby": m,
                             action: g,
-                            centered: x = !1,
-                            children: w,
-                            className: S,
-                            component: C = "div",
-                            allowScrollButtonsMobile: _ = !1,
-                            indicatorColor: B = "primary",
-                            onChange: P,
-                            orientation: E = "horizontal",
-                            ScrollButtonComponent: M = N,
-                            scrollButtons: R = "auto",
-                            selectionFollowsFocus: T,
-                            slots: k = {},
-                            slotProps: W = {},
+                            centered: Z = !1,
+                            children: x,
+                            className: w,
+                            component: S = "div",
+                            allowScrollButtonsMobile: C = !1,
+                            indicatorColor: _ = "primary",
+                            onChange: B,
+                            orientation: P = "horizontal",
+                            ScrollButtonComponent: E = k,
+                            scrollButtons: M = "auto",
+                            selectionFollowsFocus: R,
+                            slots: T = {},
+                            slotProps: j = {},
                             TabIndicatorProps: I = {},
-                            TabScrollButtonProps: q = {},
-                            textColor: K = "primary",
-                            value: U,
-                            variant: J = "standard",
-                            visibleScrollbar: Q = !1
+                            TabScrollButtonProps: G = {},
+                            textColor: q = "primary",
+                            value: K,
+                            variant: U = "standard",
+                            visibleScrollbar: J = !1
                         } = l,
-                        ee = (0, o.Z)(l, A),
-                        et = "scrollable" === J,
-                        el = "vertical" === E,
-                        er = el ? "scrollTop" : "scrollLeft",
-                        eo = el ? "top" : "left",
-                        en = el ? "bottom" : "right",
-                        ei = el ? "clientHeight" : "clientWidth",
-                        ea = el ? "height" : "width",
-                        es = (0, n.Z)({}, l, {
-                            component: C,
-                            allowScrollButtonsMobile: _,
-                            indicatorColor: B,
-                            orientation: E,
-                            vertical: el,
-                            scrollButtons: R,
-                            textColor: K,
-                            variant: J,
-                            visibleScrollbar: Q,
-                            fixed: !et,
-                            hideScrollbar: et && !Q,
-                            scrollableX: et && !el,
-                            scrollableY: et && el,
-                            centered: x && !et,
-                            scrollButtonsHideMobile: !_
+                        Q = (0, o.Z)(l, A),
+                        ee = "scrollable" === U,
+                        et = "vertical" === P,
+                        el = et ? "scrollTop" : "scrollLeft",
+                        er = et ? "top" : "left",
+                        eo = et ? "bottom" : "right",
+                        en = et ? "clientHeight" : "clientWidth",
+                        ei = et ? "height" : "width",
+                        ea = (0, n.Z)({}, l, {
+                            component: S,
+                            allowScrollButtonsMobile: C,
+                            indicatorColor: _,
+                            orientation: P,
+                            vertical: et,
+                            scrollButtons: M,
+                            textColor: q,
+                            variant: U,
+                            visibleScrollbar: J,
+                            fixed: !ee,
+                            hideScrollbar: ee && !J,
+                            scrollableX: ee && !et,
+                            scrollableY: ee && et,
+                            centered: Z && !ee,
+                            scrollButtonsHideMobile: !C
                         }),
-                        ec = H(es),
-                        eu = (0, c.Z)({
-                            elementType: k.StartScrollButtonIcon,
-                            externalSlotProps: W.startScrollButtonIcon,
-                            ownerState: es
+                        es = D(ea),
+                        ec = (0, c.Z)({
+                            elementType: T.StartScrollButtonIcon,
+                            externalSlotProps: j.startScrollButtonIcon,
+                            ownerState: ea
                         }),
-                        ed = (0, c.Z)({
-                            elementType: k.EndScrollButtonIcon,
-                            externalSlotProps: W.endScrollButtonIcon,
-                            ownerState: es
-                        }),
-                        [ef, ep] = i.useState(!1),
-                        [eh, eb] = i.useState(G),
-                        [em, ev] = i.useState({
-                            start: !1,
-                            end: !1
+                        eu = (0, c.Z)({
+                            elementType: T.EndScrollButtonIcon,
+                            externalSlotProps: j.endScrollButtonIcon,
+                            ownerState: ea
                         }),
-                        [ey, eZ] = i.useState({
+                        [ed, ef] = i.useState(!1),
+                        [ep, eh] = i.useState(Y),
+                        [eb, em] = i.useState(!1),
+                        [ev, ey] = i.useState(!1),
+                        [eg, eZ] = i.useState(!1),
+                        [ex, ew] = i.useState({
                             overflow: "hidden",
                             scrollbarWidth: 0
                         }),
-                        eg = new Map,
-                        ex = i.useRef(null),
-                        ew = i.useRef(null),
-                        eS = () => {
+                        eS = new Map,
+                        eC = i.useRef(null),
+                        e_ = i.useRef(null),
+                        eB = () => {
                             let e, t;
-                            let l = ex.current;
+                            let l = eC.current;
                             if (l) {
                                 let t = l.getBoundingClientRect();
                                 e = {
                                     clientWidth: l.clientWidth,
                                     scrollLeft: l.scrollLeft,
                                     scrollTop: l.scrollTop,
-                                    scrollLeftNormalized: b(l, r.direction),
+                                    scrollLeftNormalized: function(e, t) {
+                                        let l = e.scrollLeft;
+                                        if ("rtl" !== t) return l;
+                                        let r = h();
+                                        switch (r) {
+                                            case "negative":
+                                                return e.scrollWidth - e.clientWidth + l;
+                                            case "reverse":
+                                                return e.scrollWidth - e.clientWidth - l;
+                                            default:
+                                                return l
+                                        }
+                                    }(l, r.direction),
                                     scrollWidth: l.scrollWidth,
                                     top: t.top,
                                     bottom: t.bottom,
                                     left: t.left,
                                     right: t.right
                                 }
                             }
-                            if (l && !1 !== U) {
-                                let e = ew.current.children;
+                            if (l && !1 !== K) {
+                                let e = e_.current.children;
                                 if (e.length > 0) {
-                                    let l = e[eg.get(U)];
+                                    let l = e[eS.get(K)];
                                     t = l ? l.getBoundingClientRect() : null
                                 }
                             }
                             return {
                                 tabsMeta: e,
                                 tabMeta: t
                             }
                         },
-                        eC = (0, j.Z)(() => {
+                        eP = (0, N.Z)(() => {
                             let e;
                             let {
                                 tabsMeta: t,
                                 tabMeta: l
-                            } = eS(), r = 0;
-                            if (el) e = "top", l && t && (r = l.top - t.top + t.scrollTop);
+                            } = eB(), r = 0;
+                            if (et) e = "top", l && t && (r = l.top - t.top + t.scrollTop);
                             else if (e = s ? "right" : "left", l && t) {
                                 let o = s ? t.scrollLeftNormalized + t.clientWidth - t.scrollWidth : t.scrollLeft;
                                 r = (s ? -1 : 1) * (l[e] - t[e] + o)
                             }
                             let o = {
                                 [e]: r,
-                                [ea]: l ? l[ea] : 0
+                                [ei]: l ? l[ei] : 0
                             };
-                            if (isNaN(eh[e]) || isNaN(eh[ea])) eb(o);
+                            if (isNaN(ep[e]) || isNaN(ep[ei])) eh(o);
                             else {
-                                let t = Math.abs(eh[e] - o[e]),
-                                    l = Math.abs(eh[ea] - o[ea]);
-                                (t >= 1 || l >= 1) && eb(o)
+                                let t = Math.abs(ep[e] - o[e]),
+                                    l = Math.abs(ep[ei] - o[ei]);
+                                (t >= 1 || l >= 1) && eh(o)
                             }
                         }),
-                        e_ = (e, {
+                        eE = (e, {
                             animation: t = !0
                         } = {}) => {
                             t ? function(e, t, l, r = {}, o = () => {}) {
                                 let {
-                                    ease: n = m,
+                                    ease: n = b,
                                     duration: i = 300
                                 } = r, a = null, s = t[e], c = !1, u = r => {
                                     if (c) {
                                         o(Error("Animation cancelled"));
                                         return
                                     }
                                     null === a && (a = r);
@@ -841,223 +838,219 @@
                                         return
                                     }
                                     requestAnimationFrame(u)
                                 };
                                 return s === l ? o(Error("Element already at target position")) : requestAnimationFrame(u), () => {
                                     c = !0
                                 }
-                            }(er, ex.current, e, {
+                            }(el, eC.current, e, {
                                 duration: r.transitions.duration.standard
-                            }) : ex.current[er] = e
+                            }) : eC.current[el] = e
                         },
-                        eB = e => {
-                            let t = ex.current[er];
-                            el ? t += e : (t += e * (s ? -1 : 1), t *= s && "reverse" === h() ? -1 : 1), e_(t)
+                        eM = e => {
+                            let t = eC.current[el];
+                            et ? t += e : (t += e * (s ? -1 : 1), t *= s && "reverse" === h() ? -1 : 1), eE(t)
                         },
-                        eP = () => {
-                            let e = ex.current[ei],
+                        eR = () => {
+                            let e = eC.current[en],
                                 t = 0,
-                                l = Array.from(ew.current.children);
+                                l = Array.from(e_.current.children);
                             for (let r = 0; r < l.length; r += 1) {
                                 let o = l[r];
-                                if (t + o[ei] > e) {
+                                if (t + o[en] > e) {
                                     0 === r && (t = e);
                                     break
                                 }
-                                t += o[ei]
+                                t += o[en]
                             }
                             return t
                         },
-                        eE = () => {
-                            eB(-1 * eP())
+                        eT = () => {
+                            eM(-1 * eR())
                         },
-                        eM = () => {
-                            eB(eP())
+                        ek = () => {
+                            eM(eR())
                         },
-                        eR = i.useCallback(e => {
-                            eZ({
+                        eN = i.useCallback(e => {
+                            ew({
                                 overflow: null,
                                 scrollbarWidth: e
                             })
                         }, []),
-                        eT = (0, j.Z)(e => {
+                        ej = (0, N.Z)(e => {
                             let {
                                 tabsMeta: t,
                                 tabMeta: l
-                            } = eS();
+                            } = eB();
                             if (l && t) {
-                                if (l[eo] < t[eo]) {
-                                    let r = t[er] + (l[eo] - t[eo]);
-                                    e_(r, {
+                                if (l[er] < t[er]) {
+                                    let r = t[el] + (l[er] - t[er]);
+                                    eE(r, {
                                         animation: e
                                     })
-                                } else if (l[en] > t[en]) {
-                                    let r = t[er] + (l[en] - t[en]);
-                                    e_(r, {
+                                } else if (l[eo] > t[eo]) {
+                                    let r = t[el] + (l[eo] - t[eo]);
+                                    eE(r, {
                                         animation: e
                                     })
                                 }
                             }
                         }),
-                        ek = (0, j.Z)(() => {
-                            if (et && !1 !== R) {
-                                let e, t;
-                                let {
-                                    scrollTop: l,
-                                    scrollHeight: o,
-                                    clientHeight: n,
-                                    scrollWidth: i,
-                                    clientWidth: a
-                                } = ex.current;
-                                if (el) e = l > 1, t = l < o - n - 1;
-                                else {
-                                    let l = b(ex.current, r.direction);
-                                    e = s ? l < i - a - 1 : l > 1, t = s ? l > 1 : l < i - a - 1
-                                }(e !== em.start || t !== em.end) && ev({
-                                    start: e,
-                                    end: t
-                                })
-                            }
+                        eI = (0, N.Z)(() => {
+                            ee && !1 !== M && eZ(!eg)
                         });
                     i.useEffect(() => {
                         let e;
                         let t = (0, p.Z)(() => {
-                                ex.current && (eC(), ek())
+                                eC.current && eP()
                             }),
-                            l = (0, y.Z)(ex.current);
-                        return l.addEventListener("resize", t), "undefined" != typeof ResizeObserver && (e = new ResizeObserver(t), Array.from(ew.current.children).forEach(t => {
+                            l = (0, v.Z)(eC.current);
+                        return l.addEventListener("resize", t), "undefined" != typeof ResizeObserver && (e = new ResizeObserver(t), Array.from(e_.current.children).forEach(t => {
                             e.observe(t)
                         })), () => {
                             t.clear(), l.removeEventListener("resize", t), e && e.disconnect()
                         }
-                    }, [eC, ek]);
-                    let eN = i.useMemo(() => (0, p.Z)(() => {
-                        ek()
-                    }), [ek]);
-                    i.useEffect(() => () => {
-                        eN.clear()
-                    }, [eN]), i.useEffect(() => {
-                        ep(!0)
+                    }, [eP]), i.useEffect(() => {
+                        let e = Array.from(e_.current.children),
+                            t = e.length;
+                        if ("undefined" != typeof IntersectionObserver && t > 0 && ee && !1 !== M) {
+                            let l = e[0],
+                                r = e[t - 1],
+                                o = {
+                                    root: eC.current,
+                                    threshold: .99
+                                },
+                                n = new IntersectionObserver(e => {
+                                    em(!e[0].isIntersecting)
+                                }, o);
+                            n.observe(l);
+                            let i = new IntersectionObserver(e => {
+                                ey(!e[0].isIntersecting)
+                            }, o);
+                            return i.observe(r), () => {
+                                n.disconnect(), i.disconnect()
+                            }
+                        }
+                    }, [ee, M, eg, null == x ? void 0 : x.length]), i.useEffect(() => {
+                        ef(!0)
                     }, []), i.useEffect(() => {
-                        eC(), ek()
+                        eP()
                     }), i.useEffect(() => {
-                        eT(G !== eh)
-                    }, [eT, eh]), i.useImperativeHandle(g, () => ({
-                        updateIndicator: eC,
-                        updateScrollButtons: ek
-                    }), [eC, ek]);
-                    let ej = (0, Z.jsx)(V, (0, n.Z)({}, I, {
-                            className: (0, a.Z)(ec.indicator, I.className),
-                            ownerState: es,
-                            style: (0, n.Z)({}, eh, I.style)
+                        ej(Y !== ep)
+                    }, [ej, ep]), i.useImperativeHandle(g, () => ({
+                        updateIndicator: eP,
+                        updateScrollButtons: eI
+                    }), [eP, eI]);
+                    let eW = (0, y.jsx)(X, (0, n.Z)({}, I, {
+                            className: (0, a.Z)(es.indicator, I.className),
+                            ownerState: ea,
+                            style: (0, n.Z)({}, ep, I.style)
                         })),
-                        eW = 0,
-                        eI = i.Children.map(w, e => {
+                        eA = 0,
+                        eL = i.Children.map(x, e => {
                             if (!i.isValidElement(e)) return null;
-                            let t = void 0 === e.props.value ? eW : e.props.value;
-                            eg.set(t, eW);
-                            let l = t === U;
-                            return eW += 1, i.cloneElement(e, (0, n.Z)({
-                                fullWidth: "fullWidth" === J,
-                                indicator: l && !ef && ej,
+                            let t = void 0 === e.props.value ? eA : e.props.value;
+                            eS.set(t, eA);
+                            let l = t === K;
+                            return eA += 1, i.cloneElement(e, (0, n.Z)({
+                                fullWidth: "fullWidth" === U,
+                                indicator: l && !ed && eW,
                                 selected: l,
-                                selectionFollowsFocus: T,
-                                onChange: P,
-                                textColor: K,
+                                selectionFollowsFocus: R,
+                                onChange: B,
+                                textColor: q,
                                 value: t
-                            }, 1 !== eW || !1 !== U || e.props.tabIndex ? {} : {
+                            }, 1 !== eA || !1 !== K || e.props.tabIndex ? {} : {
                                 tabIndex: 0
                             }))
                         }),
-                        eL = (() => {
+                        eO = (() => {
                             let e = {};
-                            e.scrollbarSizeListener = et ? (0, Z.jsx)(Y, {
-                                onChange: eR,
-                                className: (0, a.Z)(ec.scrollableX, ec.hideScrollbar)
+                            e.scrollbarSizeListener = ee ? (0, y.jsx)(V, {
+                                onChange: eN,
+                                className: (0, a.Z)(es.scrollableX, es.hideScrollbar)
                             }) : null;
-                            let t = em.start || em.end,
-                                l = et && ("auto" === R && t || !0 === R);
-                            return e.scrollButtonStart = l ? (0, Z.jsx)(M, (0, n.Z)({
+                            let t = ee && ("auto" === M && (eb || ev) || !0 === M);
+                            return e.scrollButtonStart = t ? (0, y.jsx)(E, (0, n.Z)({
                                 slots: {
-                                    StartScrollButtonIcon: k.StartScrollButtonIcon
+                                    StartScrollButtonIcon: T.StartScrollButtonIcon
                                 },
                                 slotProps: {
-                                    startScrollButtonIcon: eu
+                                    startScrollButtonIcon: ec
                                 },
-                                orientation: E,
+                                orientation: P,
                                 direction: s ? "right" : "left",
-                                onClick: eE,
-                                disabled: !em.start
-                            }, q, {
-                                className: (0, a.Z)(ec.scrollButtons, q.className)
-                            })) : null, e.scrollButtonEnd = l ? (0, Z.jsx)(M, (0, n.Z)({
+                                onClick: eT,
+                                disabled: !eb
+                            }, G, {
+                                className: (0, a.Z)(es.scrollButtons, G.className)
+                            })) : null, e.scrollButtonEnd = t ? (0, y.jsx)(E, (0, n.Z)({
                                 slots: {
-                                    EndScrollButtonIcon: k.EndScrollButtonIcon
+                                    EndScrollButtonIcon: T.EndScrollButtonIcon
                                 },
                                 slotProps: {
-                                    endScrollButtonIcon: ed
+                                    endScrollButtonIcon: eu
                                 },
-                                orientation: E,
+                                orientation: P,
                                 direction: s ? "left" : "right",
-                                onClick: eM,
-                                disabled: !em.end
-                            }, q, {
-                                className: (0, a.Z)(ec.scrollButtons, q.className)
+                                onClick: ek,
+                                disabled: !ev
+                            }, G, {
+                                className: (0, a.Z)(es.scrollButtons, G.className)
                             })) : null, e
                         })();
-                    return (0, Z.jsxs)(F, (0, n.Z)({
-                        className: (0, a.Z)(ec.root, S),
-                        ownerState: es,
+                    return (0, y.jsxs)(H, (0, n.Z)({
+                        className: (0, a.Z)(es.root, w),
+                        ownerState: ea,
                         ref: t,
-                        as: C
-                    }, ee, {
-                        children: [eL.scrollButtonStart, eL.scrollbarSizeListener, (0, Z.jsxs)($, {
-                            className: ec.scroller,
-                            ownerState: es,
+                        as: S
+                    }, Q, {
+                        children: [eO.scrollButtonStart, eO.scrollbarSizeListener, (0, y.jsxs)(F, {
+                            className: es.scroller,
+                            ownerState: ea,
                             style: {
-                                overflow: ey.overflow,
-                                [el ? `margin${s?"Left":"Right"}` : "marginBottom"]: Q ? void 0 : -ey.scrollbarWidth
+                                overflow: ex.overflow,
+                                [et ? `margin${s?"Left":"Right"}` : "marginBottom"]: J ? void 0 : -ex.scrollbarWidth
                             },
-                            ref: ex,
-                            onScroll: eN,
-                            children: [(0, Z.jsx)(X, {
+                            ref: eC,
+                            children: [(0, y.jsx)($, {
                                 "aria-label": u,
-                                "aria-labelledby": v,
-                                "aria-orientation": "vertical" === E ? "vertical" : null,
-                                className: ec.flexContainer,
-                                ownerState: es,
+                                "aria-labelledby": m,
+                                "aria-orientation": "vertical" === P ? "vertical" : null,
+                                className: es.flexContainer,
+                                ownerState: ea,
                                 onKeyDown: e => {
-                                    let t = ew.current,
-                                        l = (0, L.Z)(t).activeElement,
+                                    let t = e_.current,
+                                        l = (0, W.Z)(t).activeElement,
                                         r = l.getAttribute("role");
                                     if ("tab" !== r) return;
-                                    let o = "horizontal" === E ? "ArrowLeft" : "ArrowUp",
-                                        n = "horizontal" === E ? "ArrowRight" : "ArrowDown";
-                                    switch ("horizontal" === E && s && (o = "ArrowRight", n = "ArrowLeft"), e.key) {
+                                    let o = "horizontal" === P ? "ArrowLeft" : "ArrowUp",
+                                        n = "horizontal" === P ? "ArrowRight" : "ArrowDown";
+                                    switch ("horizontal" === P && s && (o = "ArrowRight", n = "ArrowLeft"), e.key) {
                                         case o:
-                                            e.preventDefault(), D(t, l, O);
+                                            e.preventDefault(), z(t, l, O);
                                             break;
                                         case n:
-                                            e.preventDefault(), D(t, l, z);
+                                            e.preventDefault(), z(t, l, L);
                                             break;
                                         case "Home":
-                                            e.preventDefault(), D(t, null, z);
+                                            e.preventDefault(), z(t, null, L);
                                             break;
                                         case "End":
-                                            e.preventDefault(), D(t, null, O)
+                                            e.preventDefault(), z(t, null, O)
                                     }
                                 },
-                                ref: ew,
+                                ref: e_,
                                 role: "tablist",
-                                children: eI
-                            }), ef && ej]
-                        }), eL.scrollButtonEnd]
+                                children: eL
+                            }), ed && eW]
+                        }), eO.scrollButtonEnd]
                     }))
                 });
-            var K = q
+            var q = G
         },
         2690: function(e, t, l) {
             "use strict";
 
             function r(e) {
                 return e && e.ownerDocument || document
             }
@@ -1141,14 +1134,34 @@
             });
             let r = l(8754),
                 o = r._(l(7294)),
                 n = o.default.createContext(null)
         },
         8976: function(e, t, l) {
             "use strict";
+            /**
+            @copyright (c) 2017-present James Kyle <me@thejameskyle.com>
+             MIT License
+             Permission is hereby granted, free of charge, to any person obtaining
+            a copy of this software and associated documentation files (the
+            "Software"), to deal in the Software without restriction, including
+            without limitation the rights to use, copy, modify, merge, publish,
+            distribute, sublicense, and/or sell copies of the Software, and to
+            permit persons to whom the Software is furnished to do so, subject to
+            the following conditions:
+             The above copyright notice and this permission notice shall be
+            included in all copies or substantial portions of the Software.
+             THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+            EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+            MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+            NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+            LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+            OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+            WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE
+            */
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), Object.defineProperty(t, "default", {
                 enumerable: !0,
                 get: function() {
                     return p
                 }
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/75fc9c18-6f0090aa3d354e90.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1618,117 +1618,116 @@
                         l = nd(this._days),
                         h = nd(this._months),
                         d = this.asSeconds();
                     return d ? (e = I(u / 60), t = I(e / 60), u %= 60, e %= 60, n = I(h / 12), h %= 12, s = u ? u.toFixed(3).replace(/\.?0+$/, "") : "", i = d < 0 ? "-" : "", r = nc(this._months) !== nc(d) ? "-" : "", a = nc(this._days) !== nc(d) ? "-" : "", o = nc(this._milliseconds) !== nc(d) ? "-" : "", i + "P" + (n ? r + n + "Y" : "") + (h ? r + h + "M" : "") + (l ? a + l + "D" : "") + (t || e || u ? "T" : "") + (t ? o + t + "H" : "") + (e ? o + e + "M" : "") + (u ? o + s + "S" : "")) : "P0D"
                 }
                 var nm = tl.prototype;
                 return nm.isValid = function() {
-                        return this._isValid
-                    }, nm.abs = function() {
-                        var e = this._data;
-                        return this._milliseconds = tB(this._milliseconds), this._days = tB(this._days), this._months = tB(this._months), e.milliseconds = tB(e.milliseconds), e.seconds = tB(e.seconds), e.minutes = tB(e.minutes), e.hours = tB(e.hours), e.months = tB(e.months), e.years = tB(e.years), this
-                    }, nm.add = function(e, t) {
-                        return tJ(this, e, t, 1)
-                    }, nm.subtract = function(e, t) {
-                        return tJ(this, e, t, -1)
-                    }, nm.as = function(e) {
-                        if (!this.isValid()) return NaN;
-                        var t, n, s = this._milliseconds;
-                        if ("month" === (e = V(e)) || "quarter" === e || "year" === e) switch (t = this._days + s / 864e5, n = this._months + tX(t), e) {
-                            case "month":
-                                return n;
-                            case "quarter":
-                                return n / 3;
-                            case "year":
-                                return n / 12
-                        } else switch (t = this._days + Math.round(tK(this._months)), e) {
-                            case "week":
-                                return t / 7 + s / 6048e5;
-                            case "day":
-                                return t + s / 864e5;
-                            case "hour":
-                                return 24 * t + s / 36e5;
-                            case "minute":
-                                return 1440 * t + s / 6e4;
-                            case "second":
-                                return 86400 * t + s / 1e3;
-                            case "millisecond":
-                                return Math.floor(864e5 * t) + s;
-                            default:
-                                throw Error("Unknown unit " + e)
-                        }
-                    }, nm.asMilliseconds = t1, nm.asSeconds = t2, nm.asMinutes = t4, nm.asHours = t6, nm.asDays = t3, nm.asWeeks = t5, nm.asMonths = t7, nm.asQuarters = t9, nm.asYears = t8, nm.valueOf = function() {
-                        return this.isValid() ? this._milliseconds + 864e5 * this._days + this._months % 12 * 2592e6 + 31536e6 * j(this._months / 12) : NaN
-                    }, nm._bubble = function() {
-                        var e, t, n, s, i, r = this._milliseconds,
-                            a = this._days,
-                            o = this._months,
-                            u = this._data;
-                        return r >= 0 && a >= 0 && o >= 0 || r <= 0 && a <= 0 && o <= 0 || (r += 864e5 * tQ(tK(o) + a), a = 0, o = 0), u.milliseconds = r % 1e3, e = I(r / 1e3), u.seconds = e % 60, t = I(e / 60), u.minutes = t % 60, n = I(t / 60), u.hours = n % 24, a += I(n / 24), o += i = I(tX(a)), a -= tQ(tK(i)), s = I(o / 12), o %= 12, u.days = a, u.months = o, u.years = s, this
-                    }, nm.clone = function() {
-                        return tv(this)
-                    }, nm.get = function(e) {
-                        return e = V(e), this.isValid() ? this[e + "s"]() : NaN
-                    }, nm.milliseconds = nt, nm.seconds = nn, nm.minutes = ns, nm.hours = ni, nm.days = nr, nm.weeks = function() {
-                        return I(this.days() / 7)
-                    }, nm.months = na, nm.years = no, nm.humanize = function(e, t) {
-                        if (!this.isValid()) return this.localeData().invalidDate();
-                        var n, s, i, r, a, o, u, l, h, d, c, f, m, _ = !1,
-                            y = nl;
-                        return "object" == typeof e && (t = e, e = !1), "boolean" == typeof e && (_ = e), "object" == typeof t && (y = Object.assign({}, nl, t), null != t.s && null == t.ss && (y.ss = t.s - 1)), f = this.localeData(), n = !_, s = y, r = nu((i = tv(this).abs()).as("s")), a = nu(i.as("m")), o = nu(i.as("h")), u = nu(i.as("d")), l = nu(i.as("M")), h = nu(i.as("w")), d = nu(i.as("y")), c = r <= s.ss && ["s", r] || r < s.s && ["ss", r] || a <= 1 && ["m"] || a < s.m && ["mm", a] || o <= 1 && ["h"] || o < s.h && ["hh", o] || u <= 1 && ["d"] || u < s.d && ["dd", u], null != s.w && (c = c || h <= 1 && ["w"] || h < s.w && ["ww", h]), (c = c || l <= 1 && ["M"] || l < s.M && ["MM", l] || d <= 1 && ["y"] || ["yy", d])[2] = n, c[3] = +this > 0, c[4] = f, m = nh.apply(null, c), _ && (m = f.pastFuture(+this, m)), f.postformat(m)
-                    }, nm.toISOString = nf, nm.toString = nf, nm.toJSON = nf, nm.locale = tT, nm.localeData = tP, nm.toIsoString = D("toIsoString() is deprecated. Please use toISOString() instead (notice the capitals)", nf), nm.lang = tN, C("X", 0, 0, "unix"), C("x", 0, 0, "valueOf"), em("x", eh), em("X", /[+-]?\d+(\.\d{1,3})?/), eg("X", function(e, t, n) {
-                        n._d = new Date(1e3 * parseFloat(e))
-                    }), eg("x", function(e, t, n) {
-                        n._d = new Date(j(e))
-                    }), //! moment.js
-                    t.version = "2.29.4", q = ti, t.fn = tI, t.min = function() {
-                        var e = [].slice.call(arguments, 0);
-                        return to("isBefore", e)
-                    }, t.max = function() {
-                        var e = [].slice.call(arguments, 0);
-                        return to("isAfter", e)
-                    }, t.now = function() {
-                        return Date.now ? Date.now() : +new Date
-                    }, t.utc = d, t.unix = function(e) {
-                        return ti(1e3 * e)
-                    }, t.months = function(e, t) {
-                        return t$(e, t, "months")
-                    }, t.isDate = u, t.locale = eB, t.invalid = m, t.duration = tv, t.isMoment = k, t.weekdays = function(e, t, n) {
-                        return tq(e, t, n, "weekdays")
-                    }, t.parseZone = function() {
-                        return ti.apply(null, arguments).parseZone()
-                    }, t.localeData = eQ, t.isDuration = th, t.monthsShort = function(e, t) {
-                        return t$(e, t, "monthsShort")
-                    }, t.weekdaysMin = function(e, t, n) {
-                        return tq(e, t, n, "weekdaysMin")
-                    }, t.defineLocale = eJ, t.updateLocale = function(e, t) {
-                        if (null != t) {
-                            var n, s, i = ej;
-                            null != eZ[e] && null != eZ[e].parentLocale ? eZ[e].set(b(eZ[e]._config, t)) : (null != (s = eq(e)) && (i = s._config), t = b(i, t), null == s && (t.abbr = e), (n = new x(t)).parentLocale = eZ[e], eZ[e] = n), eB(e)
-                        } else null != eZ[e] && (null != eZ[e].parentLocale ? (eZ[e] = eZ[e].parentLocale, e === eB() && eB(e)) : null != eZ[e] && delete eZ[e]);
-                        return eZ[e]
-                    }, t.locales = function() {
-                        return J(eZ)
-                    }, t.weekdaysShort = function(e, t, n) {
-                        return tq(e, t, n, "weekdaysShort")
-                    }, t.normalizeUnits = V, t.relativeTimeRounding = function(e) {
-                        return void 0 === e ? nu : "function" == typeof e && (nu = e, !0)
-                    }, t.relativeTimeThreshold = function(e, t) {
-                        return void 0 !== nl[e] && (void 0 === t ? nl[e] : (nl[e] = t, "s" === e && (nl.ss = t - 1), !0))
-                    }, t.calendarFormat = function(e, t) {
-                        var n = e.diff(t, "days", !0);
-                        return n < -6 ? "sameElse" : n < -1 ? "lastWeek" : n < 0 ? "lastDay" : n < 1 ? "sameDay" : n < 2 ? "nextDay" : n < 7 ? "nextWeek" : "sameElse"
-                    }, t.prototype = tI, t.HTML5_FMT = {
-                        DATETIME_LOCAL: "YYYY-MM-DDTHH:mm",
-                        DATETIME_LOCAL_SECONDS: "YYYY-MM-DDTHH:mm:ss",
-                        DATETIME_LOCAL_MS: "YYYY-MM-DDTHH:mm:ss.SSS",
-                        DATE: "YYYY-MM-DD",
-                        TIME: "HH:mm",
-                        TIME_SECONDS: "HH:mm:ss",
-                        TIME_MS: "HH:mm:ss.SSS",
-                        WEEK: "GGGG-[W]WW",
-                        MONTH: "YYYY-MM"
-                    }, t
+                    return this._isValid
+                }, nm.abs = function() {
+                    var e = this._data;
+                    return this._milliseconds = tB(this._milliseconds), this._days = tB(this._days), this._months = tB(this._months), e.milliseconds = tB(e.milliseconds), e.seconds = tB(e.seconds), e.minutes = tB(e.minutes), e.hours = tB(e.hours), e.months = tB(e.months), e.years = tB(e.years), this
+                }, nm.add = function(e, t) {
+                    return tJ(this, e, t, 1)
+                }, nm.subtract = function(e, t) {
+                    return tJ(this, e, t, -1)
+                }, nm.as = function(e) {
+                    if (!this.isValid()) return NaN;
+                    var t, n, s = this._milliseconds;
+                    if ("month" === (e = V(e)) || "quarter" === e || "year" === e) switch (t = this._days + s / 864e5, n = this._months + tX(t), e) {
+                        case "month":
+                            return n;
+                        case "quarter":
+                            return n / 3;
+                        case "year":
+                            return n / 12
+                    } else switch (t = this._days + Math.round(tK(this._months)), e) {
+                        case "week":
+                            return t / 7 + s / 6048e5;
+                        case "day":
+                            return t + s / 864e5;
+                        case "hour":
+                            return 24 * t + s / 36e5;
+                        case "minute":
+                            return 1440 * t + s / 6e4;
+                        case "second":
+                            return 86400 * t + s / 1e3;
+                        case "millisecond":
+                            return Math.floor(864e5 * t) + s;
+                        default:
+                            throw Error("Unknown unit " + e)
+                    }
+                }, nm.asMilliseconds = t1, nm.asSeconds = t2, nm.asMinutes = t4, nm.asHours = t6, nm.asDays = t3, nm.asWeeks = t5, nm.asMonths = t7, nm.asQuarters = t9, nm.asYears = t8, nm.valueOf = function() {
+                    return this.isValid() ? this._milliseconds + 864e5 * this._days + this._months % 12 * 2592e6 + 31536e6 * j(this._months / 12) : NaN
+                }, nm._bubble = function() {
+                    var e, t, n, s, i, r = this._milliseconds,
+                        a = this._days,
+                        o = this._months,
+                        u = this._data;
+                    return r >= 0 && a >= 0 && o >= 0 || r <= 0 && a <= 0 && o <= 0 || (r += 864e5 * tQ(tK(o) + a), a = 0, o = 0), u.milliseconds = r % 1e3, e = I(r / 1e3), u.seconds = e % 60, t = I(e / 60), u.minutes = t % 60, n = I(t / 60), u.hours = n % 24, a += I(n / 24), o += i = I(tX(a)), a -= tQ(tK(i)), s = I(o / 12), o %= 12, u.days = a, u.months = o, u.years = s, this
+                }, nm.clone = function() {
+                    return tv(this)
+                }, nm.get = function(e) {
+                    return e = V(e), this.isValid() ? this[e + "s"]() : NaN
+                }, nm.milliseconds = nt, nm.seconds = nn, nm.minutes = ns, nm.hours = ni, nm.days = nr, nm.weeks = function() {
+                    return I(this.days() / 7)
+                }, nm.months = na, nm.years = no, nm.humanize = function(e, t) {
+                    if (!this.isValid()) return this.localeData().invalidDate();
+                    var n, s, i, r, a, o, u, l, h, d, c, f, m, _ = !1,
+                        y = nl;
+                    return "object" == typeof e && (t = e, e = !1), "boolean" == typeof e && (_ = e), "object" == typeof t && (y = Object.assign({}, nl, t), null != t.s && null == t.ss && (y.ss = t.s - 1)), f = this.localeData(), n = !_, s = y, r = nu((i = tv(this).abs()).as("s")), a = nu(i.as("m")), o = nu(i.as("h")), u = nu(i.as("d")), l = nu(i.as("M")), h = nu(i.as("w")), d = nu(i.as("y")), c = r <= s.ss && ["s", r] || r < s.s && ["ss", r] || a <= 1 && ["m"] || a < s.m && ["mm", a] || o <= 1 && ["h"] || o < s.h && ["hh", o] || u <= 1 && ["d"] || u < s.d && ["dd", u], null != s.w && (c = c || h <= 1 && ["w"] || h < s.w && ["ww", h]), (c = c || l <= 1 && ["M"] || l < s.M && ["MM", l] || d <= 1 && ["y"] || ["yy", d])[2] = n, c[3] = +this > 0, c[4] = f, m = nh.apply(null, c), _ && (m = f.pastFuture(+this, m)), f.postformat(m)
+                }, nm.toISOString = nf, nm.toString = nf, nm.toJSON = nf, nm.locale = tT, nm.localeData = tP, nm.toIsoString = D("toIsoString() is deprecated. Please use toISOString() instead (notice the capitals)", nf), nm.lang = tN, C("X", 0, 0, "unix"), C("x", 0, 0, "valueOf"), em("x", eh), em("X", /[+-]?\d+(\.\d{1,3})?/), eg("X", function(e, t, n) {
+                    n._d = new Date(1e3 * parseFloat(e))
+                }), eg("x", function(e, t, n) {
+                    n._d = new Date(j(e))
+                }), t.version = "2.29.4", q = ti, t.fn = tI, t.min = function() {
+                    var e = [].slice.call(arguments, 0);
+                    return to("isBefore", e)
+                }, t.max = function() {
+                    var e = [].slice.call(arguments, 0);
+                    return to("isAfter", e)
+                }, t.now = function() {
+                    return Date.now ? Date.now() : +new Date
+                }, t.utc = d, t.unix = function(e) {
+                    return ti(1e3 * e)
+                }, t.months = function(e, t) {
+                    return t$(e, t, "months")
+                }, t.isDate = u, t.locale = eB, t.invalid = m, t.duration = tv, t.isMoment = k, t.weekdays = function(e, t, n) {
+                    return tq(e, t, n, "weekdays")
+                }, t.parseZone = function() {
+                    return ti.apply(null, arguments).parseZone()
+                }, t.localeData = eQ, t.isDuration = th, t.monthsShort = function(e, t) {
+                    return t$(e, t, "monthsShort")
+                }, t.weekdaysMin = function(e, t, n) {
+                    return tq(e, t, n, "weekdaysMin")
+                }, t.defineLocale = eJ, t.updateLocale = function(e, t) {
+                    if (null != t) {
+                        var n, s, i = ej;
+                        null != eZ[e] && null != eZ[e].parentLocale ? eZ[e].set(b(eZ[e]._config, t)) : (null != (s = eq(e)) && (i = s._config), t = b(i, t), null == s && (t.abbr = e), (n = new x(t)).parentLocale = eZ[e], eZ[e] = n), eB(e)
+                    } else null != eZ[e] && (null != eZ[e].parentLocale ? (eZ[e] = eZ[e].parentLocale, e === eB() && eB(e)) : null != eZ[e] && delete eZ[e]);
+                    return eZ[e]
+                }, t.locales = function() {
+                    return J(eZ)
+                }, t.weekdaysShort = function(e, t, n) {
+                    return tq(e, t, n, "weekdaysShort")
+                }, t.normalizeUnits = V, t.relativeTimeRounding = function(e) {
+                    return void 0 === e ? nu : "function" == typeof e && (nu = e, !0)
+                }, t.relativeTimeThreshold = function(e, t) {
+                    return void 0 !== nl[e] && (void 0 === t ? nl[e] : (nl[e] = t, "s" === e && (nl.ss = t - 1), !0))
+                }, t.calendarFormat = function(e, t) {
+                    var n = e.diff(t, "days", !0);
+                    return n < -6 ? "sameElse" : n < -1 ? "lastWeek" : n < 0 ? "lastDay" : n < 1 ? "sameDay" : n < 2 ? "nextDay" : n < 7 ? "nextWeek" : "sameElse"
+                }, t.prototype = tI, t.HTML5_FMT = {
+                    DATETIME_LOCAL: "YYYY-MM-DDTHH:mm",
+                    DATETIME_LOCAL_SECONDS: "YYYY-MM-DDTHH:mm:ss",
+                    DATETIME_LOCAL_MS: "YYYY-MM-DDTHH:mm:ss.SSS",
+                    DATE: "YYYY-MM-DD",
+                    TIME: "HH:mm",
+                    TIME_SECONDS: "HH:mm:ss",
+                    TIME_MS: "HH:mm:ss.SSS",
+                    WEEK: "GGGG-[W]WW",
+                    MONTH: "YYYY-MM"
+                }, t
             }()
         }
     }
 ]);
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/main-2ecf43899f8683c2.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/main-92011a1a7f336a6f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -246,18 +246,18 @@
             r(37);
             let y = g._(r(7294)),
                 _ = g._(r(745)),
                 b = r(9958),
                 v = g._(r(6595)),
                 P = r(9955),
                 w = r(3105),
-                S = r(3162),
-                j = r(3908),
-                O = r(7905),
-                E = r(9064),
+                j = r(3162),
+                S = r(3908),
+                E = r(7905),
+                O = r(9064),
                 R = r(3232),
                 x = g._(r(9623)),
                 C = g._(r(9030)),
                 M = g._(r(5108)),
                 A = r(2827),
                 L = r(6885),
                 I = r(676),
@@ -271,25 +271,25 @@
                 F = e => t => e(t) + "",
                 W = r.u;
             r.u = F(W);
             let q = r.k;
             r.k = F(q);
             let z = r.miniCssF;
             r.miniCssF = F(z);
-            let G = "13.4.10",
+            let G = "13.4.12",
                 V = (0, v.default)(),
                 X = e => [].slice.call(e),
                 $ = !1;
             self.__next_require__ = r;
             class Y extends y.default.Component {
                 componentDidCatch(e, t) {
                     this.props.fn(e, t)
                 }
                 componentDidMount() {
-                    this.scrollToHash(), n.isSsr && (a.isFallback || a.nextExport && ((0, S.isDynamicRoute)(n.pathname) || location.search || $) || a.props && a.props.__N_SSG && (location.search || $)) && n.replace(n.pathname + "?" + String((0, j.assign)((0, j.urlQueryToSearchParams)(n.query), new URLSearchParams(location.search))), o, {
+                    this.scrollToHash(), n.isSsr && (a.isFallback || a.nextExport && ((0, j.isDynamicRoute)(n.pathname) || location.search || $) || a.props && a.props.__N_SSG && (location.search || $)) && n.replace(n.pathname + "?" + String((0, S.assign)((0, S.urlQueryToSearchParams)(n.query), new URLSearchParams(location.search))), o, {
                         _h: 1,
                         shallow: !a.isFallback && !$
                     }).catch(e => {
                         if (!e.cancelled) throw e
                     })
                 }
                 componentDidUpdate() {
@@ -306,18 +306,18 @@
                 render() {
                     return this.props.children
                 }
             }
             async function K(e) {
                 void 0 === e && (e = {}), a = JSON.parse(document.getElementById("__NEXT_DATA__").textContent), window.__NEXT_DATA__ = a, p = a.defaultLocale;
                 let t = a.assetPrefix || "";
-                if (r.p = "" + t + "/_next/", (0, O.setConfig)({
+                if (r.p = "" + t + "/_next/", (0, E.setConfig)({
                         serverRuntimeConfig: {},
                         publicRuntimeConfig: a.runtimeConfig || {}
-                    }), o = (0, E.getURL)(), (0, k.hasBasePath)(o) && (o = (0, N.removeBasePath)(o)), a.scriptLoader) {
+                    }), o = (0, O.getURL)(), (0, k.hasBasePath)(o) && (o = (0, N.removeBasePath)(o)), a.scriptLoader) {
                     let {
                         initScriptLoader: e
                     } = r(5442);
                     e(a.scriptLoader)
                 }
                 i = new C.default(a.buildId, t);
                 let s = e => {
@@ -405,15 +405,15 @@
                             err: l,
                             pathname: a.page,
                             query: a.query,
                             asPath: o,
                             AppTree: c
                         }
                     };
-                    return Promise.resolve((null == (i = e.props) ? void 0 : i.err) ? e.props : (0, E.loadGetInitialProps)(t, f)).then(t => eu({
+                    return Promise.resolve((null == (i = e.props) ? void 0 : i.err) ? e.props : (0, O.loadGetInitialProps)(t, f)).then(t => eu({
                         ...e,
                         err: l,
                         Component: u,
                         styleSheets: s,
                         props: t
                     }))
                 })
@@ -429,19 +429,19 @@
                 en = !0;
 
             function ea() {
                 ["beforeRender", "afterHydrate", "afterRender", "routeChange"].forEach(e => performance.clearMarks(e))
             }
 
             function eo() {
-                E.ST && (performance.mark("afterHydrate"), performance.measure("Next.js-before-hydration", "navigationStart", "beforeRender"), performance.measure("Next.js-hydration", "beforeRender", "afterHydrate"), d && performance.getEntriesByName("Next.js-hydration").forEach(d), ea())
+                O.ST && (performance.mark("afterHydrate"), performance.measure("Next.js-before-hydration", "navigationStart", "beforeRender"), performance.measure("Next.js-hydration", "beforeRender", "afterHydrate"), d && performance.getEntriesByName("Next.js-hydration").forEach(d), ea())
             }
 
             function ei() {
-                if (!E.ST) return;
+                if (!O.ST) return;
                 performance.mark("afterRender");
                 let e = performance.getEntriesByName("routeChange", "mark");
                 e.length && (performance.measure("Next.js-route-change-to-render", e[0].name, "beforeRender"), performance.measure("Next.js-render", "beforeRender", "afterRender"), d && (performance.getEntriesByName("Next.js-render").forEach(d), performance.getEntriesByName("Next.js-route-change-to-render").forEach(d)), ea(), ["Next.js-route-change-to-render", "Next.js-render"].forEach(e => performance.clearMeasures(e)))
             }
 
             function el(e) {
                 let {
@@ -526,15 +526,15 @@
                             })
                         }
                     }
                 }), y.default.createElement(Q, null, J(r, f), y.default.createElement(R.Portal, {
                     type: "next-route-announcer"
                 }, y.default.createElement(A.RouteAnnouncer, null))));
                 return ! function(e, t) {
-                    E.ST && performance.mark("beforeRender");
+                    O.ST && performance.mark("beforeRender");
                     let r = t(en ? eo : ei);
                     if (er) {
                         let e = y.default.startTransition;
                         e(() => {
                             er.render(r)
                         })
                     } else er = _.default.hydrateRoot(e, r, {
@@ -1249,154 +1249,176 @@
                 function(e, t) {
                     for (var r in t) Object.defineProperty(e, r, {
                         enumerable: !0,
                         get: t[r]
                     })
                 }(t, {
                     handleClientScriptLoad: function() {
-                        return p
+                        return m
                     },
                     initScriptLoader: function() {
-                        return m
+                        return g
                     },
                     default: function() {
-                        return y
+                        return _
                     }
                 });
             let n = r(8754),
                 a = r(1757),
                 o = n._(r(3935)),
                 i = a._(r(7294)),
                 l = r(9958),
                 u = r(9623),
                 s = r(29),
                 c = new Map,
                 f = new Set,
-                d = ["onLoad", "onReady", "dangerouslySetInnerHTML", "children", "onError", "strategy"],
+                d = ["onLoad", "onReady", "dangerouslySetInnerHTML", "children", "onError", "strategy", "stylesheets"],
                 h = e => {
+                    if (o.default.preinit) {
+                        e.forEach(e => {
+                            o.default.preinit(e, {
+                                as: "style"
+                            })
+                        });
+                        return
+                    } {
+                        let t = document.head;
+                        e.forEach(e => {
+                            let r = document.createElement("link");
+                            r.type = "text/css", r.rel = "stylesheet", r.href = e, t.appendChild(r)
+                        })
+                    }
+                },
+                p = e => {
                     let {
                         src: t,
                         id: r,
                         onLoad: n = () => {},
                         onReady: a = null,
                         dangerouslySetInnerHTML: o,
                         children: i = "",
                         strategy: l = "afterInteractive",
-                        onError: s
-                    } = e, h = r || t;
-                    if (h && f.has(h)) return;
+                        onError: s,
+                        stylesheets: p
+                    } = e, m = r || t;
+                    if (m && f.has(m)) return;
                     if (c.has(t)) {
-                        f.add(h), c.get(t).then(n, s);
+                        f.add(m), c.get(t).then(n, s);
                         return
                     }
-                    let p = () => {
-                            a && a(), f.add(h)
+                    let g = () => {
+                            a && a(), f.add(m)
                         },
-                        m = document.createElement("script"),
-                        g = new Promise((e, t) => {
-                            m.addEventListener("load", function(t) {
-                                e(), n && n.call(this, t), p()
-                            }), m.addEventListener("error", function(e) {
+                        y = document.createElement("script"),
+                        _ = new Promise((e, t) => {
+                            y.addEventListener("load", function(t) {
+                                e(), n && n.call(this, t), g()
+                            }), y.addEventListener("error", function(e) {
                                 t(e)
                             })
                         }).catch(function(e) {
                             s && s(e)
                         });
-                    for (let [r, n] of(o ? (m.innerHTML = o.__html || "", p()) : i ? (m.textContent = "string" == typeof i ? i : Array.isArray(i) ? i.join("") : "", p()) : t && (m.src = t, c.set(t, g)), Object.entries(e))) {
+                    for (let [r, n] of(o ? (y.innerHTML = o.__html || "", g()) : i ? (y.textContent = "string" == typeof i ? i : Array.isArray(i) ? i.join("") : "", g()) : t && (y.src = t, c.set(t, _)), Object.entries(e))) {
                         if (void 0 === n || d.includes(r)) continue;
                         let e = u.DOMAttributeNames[r] || r.toLowerCase();
-                        m.setAttribute(e, n)
+                        y.setAttribute(e, n)
                     }
-                    "worker" === l && m.setAttribute("type", "text/partytown"), m.setAttribute("data-nscript", l), document.body.appendChild(m)
+                    "worker" === l && y.setAttribute("type", "text/partytown"), y.setAttribute("data-nscript", l), p && h(p), document.body.appendChild(y)
                 };
 
-            function p(e) {
+            function m(e) {
                 let {
                     strategy: t = "afterInteractive"
                 } = e;
                 "lazyOnload" === t ? window.addEventListener("load", () => {
-                    (0, s.requestIdleCallback)(() => h(e))
-                }) : h(e)
+                    (0, s.requestIdleCallback)(() => p(e))
+                }) : p(e)
             }
 
-            function m(e) {
-                e.forEach(p),
+            function g(e) {
+                e.forEach(m),
                     function() {
                         let e = [...document.querySelectorAll('[data-nscript="beforeInteractive"]'), ...document.querySelectorAll('[data-nscript="beforePageRender"]')];
                         e.forEach(e => {
                             let t = e.id || e.getAttribute("src");
                             f.add(t)
                         })
                     }()
             }
 
-            function g(e) {
+            function y(e) {
                 let {
                     id: t,
                     src: r = "",
                     onLoad: n = () => {},
                     onReady: a = null,
                     strategy: u = "afterInteractive",
                     onError: c,
-                    ...d
+                    stylesheets: d,
+                    ...h
                 } = e, {
-                    updateScripts: p,
-                    scripts: m,
-                    getIsSsr: g,
-                    appDir: y,
-                    nonce: _
-                } = (0, i.useContext)(l.HeadManagerContext), b = (0, i.useRef)(!1);
+                    updateScripts: m,
+                    scripts: g,
+                    getIsSsr: y,
+                    appDir: _,
+                    nonce: b
+                } = (0, i.useContext)(l.HeadManagerContext), v = (0, i.useRef)(!1);
                 (0, i.useEffect)(() => {
                     let e = t || r;
-                    b.current || (a && e && f.has(e) && a(), b.current = !0)
+                    v.current || (a && e && f.has(e) && a(), v.current = !0)
                 }, [a, t, r]);
-                let v = (0, i.useRef)(!1);
+                let P = (0, i.useRef)(!1);
                 if ((0, i.useEffect)(() => {
-                        !v.current && ("afterInteractive" === u ? h(e) : "lazyOnload" === u && ("complete" === document.readyState ? (0, s.requestIdleCallback)(() => h(e)) : window.addEventListener("load", () => {
-                            (0, s.requestIdleCallback)(() => h(e))
-                        })), v.current = !0)
-                    }, [e, u]), ("beforeInteractive" === u || "worker" === u) && (p ? (m[u] = (m[u] || []).concat([{
+                        !P.current && ("afterInteractive" === u ? p(e) : "lazyOnload" === u && ("complete" === document.readyState ? (0, s.requestIdleCallback)(() => p(e)) : window.addEventListener("load", () => {
+                            (0, s.requestIdleCallback)(() => p(e))
+                        })), P.current = !0)
+                    }, [e, u]), ("beforeInteractive" === u || "worker" === u) && (m ? (g[u] = (g[u] || []).concat([{
                         id: t,
                         src: r,
                         onLoad: n,
                         onReady: a,
                         onError: c,
-                        ...d
-                    }]), p(m)) : g && g() ? f.add(t || r) : g && !g() && h(e)), y) {
-                    if ("beforeInteractive" === u) return r ? (o.default.preload(r, d.integrity ? {
+                        ...h
+                    }]), m(g)) : y && y() ? f.add(t || r) : y && !y() && p(e)), _) {
+                    if (d && d.forEach(e => {
+                            o.default.preinit(e, {
+                                as: "style"
+                            })
+                        }), "beforeInteractive" === u) return r ? (o.default.preload(r, h.integrity ? {
                         as: "script",
-                        integrity: d.integrity
+                        integrity: h.integrity
                     } : {
                         as: "script"
                     }), i.default.createElement("script", {
-                        nonce: _,
+                        nonce: b,
                         dangerouslySetInnerHTML: {
                             __html: "(self.__next_s=self.__next_s||[]).push(" + JSON.stringify([r]) + ")"
                         }
-                    })) : (d.dangerouslySetInnerHTML && (d.children = d.dangerouslySetInnerHTML.__html, delete d.dangerouslySetInnerHTML), i.default.createElement("script", {
-                        nonce: _,
+                    })) : (h.dangerouslySetInnerHTML && (h.children = h.dangerouslySetInnerHTML.__html, delete h.dangerouslySetInnerHTML), i.default.createElement("script", {
+                        nonce: b,
                         dangerouslySetInnerHTML: {
                             __html: "(self.__next_s=self.__next_s||[]).push(" + JSON.stringify([0, {
-                                ...d
+                                ...h
                             }]) + ")"
                         }
                     }));
-                    "afterInteractive" === u && r && o.default.preload(r, d.integrity ? {
+                    "afterInteractive" === u && r && o.default.preload(r, h.integrity ? {
                         as: "script",
-                        integrity: d.integrity
+                        integrity: h.integrity
                     } : {
                         as: "script"
                     })
                 }
                 return null
             }
-            Object.defineProperty(g, "__nextScript", {
+            Object.defineProperty(y, "__nextScript", {
                 value: !0
             });
-            let y = g;
+            let _ = y;
             ("function" == typeof t.default || "object" == typeof t.default && null !== t.default) && void 0 === t.default.__esModule && (Object.defineProperty(t.default, "__esModule", {
                 value: !0
             }), Object.assign(t.default, t), e.exports = t.default)
         },
         466: function(e, t) {
             "use strict";
             let r;
@@ -2100,19 +2122,29 @@
                     },
                     forward() {
                         e.forward()
                     },
                     refresh() {
                         e.reload()
                     },
-                    push(t) {
-                        e.push(t)
+                    push(t, r) {
+                        let {
+                            scroll: n
+                        } = void 0 === r ? {} : r;
+                        e.push(t, void 0, {
+                            scroll: n
+                        })
                     },
-                    replace(t) {
-                        e.replace(t)
+                    replace(t, r) {
+                        let {
+                            scroll: n
+                        } = void 0 === r ? {} : r;
+                        e.replace(t, void 0, {
+                            scroll: n
+                        })
                     },
                     prefetch(t) {
                         e.prefetch(t)
                     }
                 }
             }
 
@@ -2187,18 +2219,18 @@
                 y = r(1410);
             r(2249);
             let _ = r(4046),
                 b = r(370),
                 v = r(2080),
                 P = r(9577),
                 w = r(4266),
-                S = r(2140),
-                j = r(9423),
-                O = r(6373),
-                E = r(9473),
+                j = r(2140),
+                S = r(9423),
+                E = r(6373),
+                O = r(9473),
                 R = r(6385),
                 x = r(3353),
                 C = r(293),
                 M = r(5821),
                 A = r(4532),
                 L = r(5036),
                 I = r(3105);
@@ -2209,15 +2241,15 @@
                 })
             }
             async function N(e) {
                 let t = await Promise.resolve(e.router.pageLoader.getMiddleware());
                 if (!t) return !1;
                 let {
                     pathname: r
-                } = (0, _.parsePath)(e.asPath), n = (0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, a = (0, w.addBasePath)((0, b.addLocale)(n, e.locale));
+                } = (0, _.parsePath)(e.asPath), n = (0, j.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, a = (0, w.addBasePath)((0, b.addLocale)(n, e.locale));
                 return t.some(e => new RegExp(e.regexp).test(a))
             }
 
             function k(e) {
                 let t = (0, d.getLocationOrigin)();
                 return e.startsWith(t) ? e.substring(t.length) : e
             }
@@ -2255,25 +2287,25 @@
                             },
                             a = t.headers.get("x-nextjs-rewrite"),
                             l = a || t.headers.get("x-nextjs-matched-path"),
                             u = t.headers.get("x-matched-path");
                         if (!u || l || u.includes("__next_data_catchall") || u.includes("/_error") || u.includes("/404") || (l = u), l) {
                             if (l.startsWith("/")) {
                                 let t = (0, p.parseRelativeUrl)(l),
-                                    u = (0, O.getNextPathnameInfo)(t.pathname, {
+                                    u = (0, E.getNextPathnameInfo)(t.pathname, {
                                         nextConfig: n,
                                         parseData: !0
                                     }),
                                     s = (0, o.removeTrailingSlash)(u.pathname);
                                 return Promise.all([r.router.pageLoader.getPageList(), (0, i.getClientBuildManifest)()]).then(o => {
                                     let [i, {
                                         __rewrites: l
                                     }] = o, f = (0, b.addLocale)(u.pathname, u.locale);
                                     if ((0, h.isDynamicRoute)(f) || !a && i.includes((0, c.normalizeLocalePath)((0, P.removeBasePath)(f), r.router.locales).pathname)) {
-                                        let r = (0, O.getNextPathnameInfo)((0, p.parseRelativeUrl)(e).pathname, {
+                                        let r = (0, E.getNextPathnameInfo)((0, p.parseRelativeUrl)(e).pathname, {
                                             nextConfig: n,
                                             parseData: !0
                                         });
                                         f = (0, w.addBasePath)(r.pathname), t.pathname = f
                                     }
                                     if (!i.includes(s)) {
                                         let e = B(s, i);
@@ -2288,16 +2320,16 @@
                                         type: "rewrite",
                                         parsedAs: t,
                                         resolvedHref: d
                                     }
                                 })
                             }
                             let t = (0, _.parsePath)(e),
-                                u = (0, E.formatNextPathnameInfo)({
-                                    ...(0, O.getNextPathnameInfo)(t.pathname, {
+                                u = (0, O.formatNextPathnameInfo)({
+                                    ...(0, E.getNextPathnameInfo)(t.pathname, {
                                         nextConfig: n,
                                         parseData: !0
                                     }),
                                     defaultLocale: r.router.defaultLocale,
                                     buildId: ""
                                 });
                             return Promise.resolve({
@@ -2305,16 +2337,16 @@
                                 destination: "" + u + t.query + t.hash
                             })
                         }
                         let s = t.headers.get("x-nextjs-redirect");
                         if (s) {
                             if (s.startsWith("/")) {
                                 let e = (0, _.parsePath)(s),
-                                    t = (0, E.formatNextPathnameInfo)({
-                                        ...(0, O.getNextPathnameInfo)(e.pathname, {
+                                    t = (0, O.formatNextPathnameInfo)({
+                                        ...(0, E.getNextPathnameInfo)(e.pathname, {
                                             nextConfig: n,
                                             parseData: !0
                                         }),
                                         defaultLocale: r.router.defaultLocale,
                                         buildId: ""
                                     });
                                 return Promise.resolve({
@@ -2506,15 +2538,15 @@
                                     }
                                 }
                             }
                     }
                     return !1
                 }
                 async change(e, t, r, n, a) {
-                    var s, c, f, j, O, E, C, A, I;
+                    var s, c, f, S, E, O, C, A, I;
                     let k, H;
                     if (!(0, x.isLocalURL)(t)) return z({
                         url: t,
                         router: this
                     }), !1;
                     let F = 1 === n._h;
                     F || n.shallow || await this._bfl(r, void 0, n.locale);
@@ -2530,16 +2562,16 @@
                     d.ST && performance.mark("routeChange");
                     let {
                         shallow: Y = !1,
                         scroll: K = !0
                     } = n, J = {
                         shallow: Y
                     };
-                    this._inFlightRoute && this.clc && (X || V.events.emit("routeChangeError", T(), this._inFlightRoute, J), this.clc(), this.clc = null), r = (0, w.addBasePath)((0, b.addLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, n.locale, this.defaultLocale));
-                    let Q = (0, v.removeLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, q.locale);
+                    this._inFlightRoute && this.clc && (X || V.events.emit("routeChangeError", T(), this._inFlightRoute, J), this.clc(), this.clc = null), r = (0, w.addBasePath)((0, b.addLocale)((0, j.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, n.locale, this.defaultLocale));
+                    let Q = (0, v.removeLocale)((0, j.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, q.locale);
                     this._inFlightRoute = r;
                     let Z = $ !== q.locale;
                     if (!F && this.onlyAHashChange(Q) && !Z) {
                         q.asPath = Q, V.events.emit("hashChangeStart", r, J), this.changeState(e, t, r, {
                             ...n,
                             scroll: !1
                         }), K && this.scrollToHash(Q);
@@ -2617,21 +2649,21 @@
                             hasMiddleware: el,
                             unstable_skipClientCache: n.unstable_skipClientCache,
                             isQueryUpdating: F && !this.isFallback,
                             isMiddlewareRewrite: ei
                         });
                         if (F || n.shallow || await this._bfl(r, "resolvedAs" in o ? o.resolvedAs : void 0, q.locale), "route" in o && el) {
                             ea = et = o.route || ea, J.shallow || (er = Object.assign({}, o.query || {}, er));
-                            let e = (0, S.hasBasePath)(ee.pathname) ? (0, P.removeBasePath)(ee.pathname) : ee.pathname;
+                            let e = (0, j.hasBasePath)(ee.pathname) ? (0, P.removeBasePath)(ee.pathname) : ee.pathname;
                             if (eu && et !== e && Object.keys(eu).forEach(e => {
                                     eu && er[e] === eu[e] && delete er[e]
                                 }), (0, h.isDynamicRoute)(et)) {
                                 let e = !J.shallow && o.resolvedAs ? o.resolvedAs : (0, w.addBasePath)((0, b.addLocale)(new URL(r, location.href).pathname, q.locale), !0),
                                     t = e;
-                                (0, S.hasBasePath)(t) && (t = (0, P.removeBasePath)(t));
+                                (0, j.hasBasePath)(t) && (t = (0, P.removeBasePath)(t));
                                 let n = (0, g.getRouteRegex)(et),
                                     a = (0, m.getRouteMatcher)(n)(new URL(t, location.href).pathname);
                                 a && Object.assign(er, a)
                             }
                         }
                         if ("type" in o) {
                             if ("redirect-internal" === o.type) return this.change(e, o.newUrl, o.newAs, n);
@@ -2683,17 +2715,17 @@
                                         },
                                         locale: q.locale,
                                         isPreview: q.isPreview,
                                         isNotFound: !0
                                     }), "type" in o) throw Error("Unexpected middleware effect on /404")
                             }
                         }
-                        F && "/_error" === this.pathname && (null == (c = self.__NEXT_DATA__.props) ? void 0 : null == (f = c.pageProps) ? void 0 : f.statusCode) === 500 && (null == (j = o.props) ? void 0 : j.pageProps) && (o.props.pageProps.statusCode = 500);
-                        let s = n.shallow && q.route === (null != (O = o.route) ? O : ea),
-                            d = null != (E = n.scroll) ? E : !F && !s,
+                        F && "/_error" === this.pathname && (null == (c = self.__NEXT_DATA__.props) ? void 0 : null == (f = c.pageProps) ? void 0 : f.statusCode) === 500 && (null == (S = o.props) ? void 0 : S.pageProps) && (o.props.pageProps.statusCode = 500);
+                        let s = n.shallow && q.route === (null != (E = o.route) ? E : ea),
+                            d = null != (O = n.scroll) ? O : !F && !s,
                             y = null != a ? a : d ? {
                                 x: 0,
                                 y: 0
                             } : null,
                             _ = {
                                 ...q,
                                 route: ea,
@@ -2796,24 +2828,24 @@
                         isPreview: d,
                         unstable_skipClientCache: h,
                         isQueryUpdating: p,
                         isMiddlewareRewrite: m,
                         isNotFound: g
                     } = e, _ = t;
                     try {
-                        var b, v, w, S;
+                        var b, v, w, j;
                         let e = G({
                                 route: _,
                                 router: this
                             }),
                             t = this.components[_];
                         if (l.shallow && t && this.route === _) return t;
                         f && (t = void 0);
                         let u = !t || "initial" in t ? void 0 : t,
-                            O = {
+                            E = {
                                 dataHref: this.pageLoader.getDataHref({
                                     href: (0, y.formatWithValidation)({
                                         pathname: r,
                                         query: n
                                     }),
                                     skipInterpolation: !0,
                                     asPath: g ? "/404" : i,
@@ -2824,60 +2856,60 @@
                                 parseJSON: !0,
                                 inflightCache: p ? this.sbc : this.sdc,
                                 persistCache: !d,
                                 isPrefetch: !1,
                                 unstable_skipClientCache: h,
                                 isBackground: p
                             },
-                            E = p && !m ? null : await H({
-                                fetchData: () => W(O),
+                            O = p && !m ? null : await H({
+                                fetchData: () => W(E),
                                 asPath: g ? "/404" : i,
                                 locale: s,
                                 router: this
                             }).catch(e => {
                                 if (p) return null;
                                 throw e
                             });
-                        if (E && ("/_error" === r || "/404" === r) && (E.effect = void 0), p && (E ? E.json = self.__NEXT_DATA__.props : E = {
+                        if (O && ("/_error" === r || "/404" === r) && (O.effect = void 0), p && (O ? O.json = self.__NEXT_DATA__.props : O = {
                                 json: self.__NEXT_DATA__.props
-                            }), e(), (null == E ? void 0 : null == (b = E.effect) ? void 0 : b.type) === "redirect-internal" || (null == E ? void 0 : null == (v = E.effect) ? void 0 : v.type) === "redirect-external") return E.effect;
-                        if ((null == E ? void 0 : null == (w = E.effect) ? void 0 : w.type) === "rewrite") {
-                            let e = (0, o.removeTrailingSlash)(E.effect.resolvedHref),
+                            }), e(), (null == O ? void 0 : null == (b = O.effect) ? void 0 : b.type) === "redirect-internal" || (null == O ? void 0 : null == (v = O.effect) ? void 0 : v.type) === "redirect-external") return O.effect;
+                        if ((null == O ? void 0 : null == (w = O.effect) ? void 0 : w.type) === "rewrite") {
+                            let e = (0, o.removeTrailingSlash)(O.effect.resolvedHref),
                                 a = await this.pageLoader.getPageList();
-                            if ((!p || a.includes(e)) && (_ = e, r = E.effect.resolvedHref, n = {
+                            if ((!p || a.includes(e)) && (_ = e, r = O.effect.resolvedHref, n = {
                                     ...n,
-                                    ...E.effect.parsedAs.query
-                                }, i = (0, P.removeBasePath)((0, c.normalizeLocalePath)(E.effect.parsedAs.pathname, this.locales).pathname), t = this.components[_], l.shallow && t && this.route === _ && !f)) return {
+                                    ...O.effect.parsedAs.query
+                                }, i = (0, P.removeBasePath)((0, c.normalizeLocalePath)(O.effect.parsedAs.pathname, this.locales).pathname), t = this.components[_], l.shallow && t && this.route === _ && !f)) return {
                                 ...t,
                                 route: _
                             }
                         }
-                        if ((0, j.isAPIRoute)(_)) return z({
+                        if ((0, S.isAPIRoute)(_)) return z({
                             url: a,
                             router: this
                         }), new Promise(() => {});
                         let R = u || await this.fetchComponent(_).then(e => ({
                                 Component: e.page,
                                 styleSheets: e.styleSheets,
                                 __N_SSG: e.mod.__N_SSG,
                                 __N_SSP: e.mod.__N_SSP
                             })),
-                            x = null == E ? void 0 : null == (S = E.response) ? void 0 : S.headers.get("x-middleware-skip"),
+                            x = null == O ? void 0 : null == (j = O.response) ? void 0 : j.headers.get("x-middleware-skip"),
                             C = R.__N_SSG || R.__N_SSP;
-                        x && (null == E ? void 0 : E.dataHref) && delete this.sdc[E.dataHref];
+                        x && (null == O ? void 0 : O.dataHref) && delete this.sdc[O.dataHref];
                         let {
                             props: M,
                             cacheKey: A
                         } = await this._getData(async () => {
                             if (C) {
-                                if ((null == E ? void 0 : E.json) && !x) return {
-                                    cacheKey: E.cacheKey,
-                                    props: E.json
+                                if ((null == O ? void 0 : O.json) && !x) return {
+                                    cacheKey: O.cacheKey,
+                                    props: O.json
                                 };
-                                let e = (null == E ? void 0 : E.dataHref) ? E.dataHref : this.pageLoader.getDataHref({
+                                let e = (null == O ? void 0 : O.dataHref) ? O.dataHref : this.pageLoader.getDataHref({
                                         href: (0, y.formatWithValidation)({
                                             pathname: r,
                                             query: n
                                         }),
                                         asPath: i,
                                         locale: s
                                     }),
@@ -2903,15 +2935,15 @@
                                     asPath: a,
                                     locale: s,
                                     locales: this.locales,
                                     defaultLocale: this.defaultLocale
                                 })
                             }
                         });
-                        return R.__N_SSP && O.dataHref && A && delete this.sdc[A], this.isPreview || !R.__N_SSG || p || W(Object.assign({}, O, {
+                        return R.__N_SSP && E.dataHref && A && delete this.sdc[A], this.isPreview || !R.__N_SSG || p || W(Object.assign({}, E, {
                             isBackground: !0,
                             persistCache: !1,
                             inflightCache: this.sbc
                         })).catch(() => {}), M.pageProps = Object.assign({}, M.pageProps), R.props = M, R.route = _, R.query = n, R.resolvedAs = i, this.components[_] = R, R
                     } catch (e) {
                         return this.handleRouteInfoError((0, u.getProperError)(e), r, n, a, l)
                     }
@@ -2925,26 +2957,30 @@
                 onlyAHashChange(e) {
                     if (!this.asPath) return !1;
                     let [t, r] = this.asPath.split("#"), [n, a] = e.split("#");
                     return !!a && t === n && r === a || t === n && r !== a
                 }
                 scrollToHash(e) {
                     let [, t = ""] = e.split("#");
-                    if ("" === t || "top" === t) {
-                        (0, I.handleSmoothScroll)(() => window.scrollTo(0, 0));
-                        return
-                    }
-                    let r = decodeURIComponent(t),
-                        n = document.getElementById(r);
-                    if (n) {
-                        (0, I.handleSmoothScroll)(() => n.scrollIntoView());
-                        return
-                    }
-                    let a = document.getElementsByName(r)[0];
-                    a && (0, I.handleSmoothScroll)(() => a.scrollIntoView())
+                    (0, I.handleSmoothScroll)(() => {
+                        if ("" === t || "top" === t) {
+                            window.scrollTo(0, 0);
+                            return
+                        }
+                        let e = decodeURIComponent(t),
+                            r = document.getElementById(e);
+                        if (r) {
+                            r.scrollIntoView();
+                            return
+                        }
+                        let n = document.getElementsByName(e)[0];
+                        n && n.scrollIntoView()
+                    }, {
+                        onlyHashChange: this.onlyAHashChange(e)
+                    })
                 }
                 urlIsNew(e) {
                     return this.asPath !== e
                 }
                 async prefetch(e, t, r) {
                     if (void 0 === t && (t = e), void 0 === r && (r = {}), (0, C.isBot)(window.navigator.userAgent)) return;
                     let n = (0, p.parseRelativeUrl)(e),
@@ -3130,16 +3166,16 @@
                         } = (0, p.parseRelativeUrl)(a);
                         (!this.isSsr || o !== (0, w.addBasePath)(this.asPath) || u !== (0, w.addBasePath)(this.pathname)) && (!this._bps || this._bps(n)) && this.change("replaceState", a, o, Object.assign({}, i, {
                             shallow: i.shallow && this._shallow,
                             locale: i.locale || this.defaultLocale,
                             _h: 0
                         }), t)
                     };
-                    let S = (0, o.removeTrailingSlash)(e);
-                    this.components = {}, "/_error" !== e && (this.components[S] = {
+                    let j = (0, o.removeTrailingSlash)(e);
+                    this.components = {}, "/_error" !== e && (this.components[j] = {
                         Component: s,
                         initial: !0,
                         props: a,
                         err: c,
                         __N_SSG: a && a.__N_SSG,
                         __N_SSP: a && a.__N_SSP
                     }), this.components["/_app"] = {
@@ -3160,20 +3196,20 @@
                             numBits: 0,
                             numHashes: null,
                             bitArray: []
                         };
                         (null == t ? void 0 : t.numHashes) && (this._bfl_s = new e(t.numItems, t.errorRate), this._bfl_s.import(t)), (null == n ? void 0 : n.numHashes) && (this._bfl_d = new e(n.numItems, n.errorRate), this._bfl_d.import(n))
                     }
                     this.events = V.events, this.pageLoader = i;
-                    let j = (0, h.isDynamicRoute)(e) && self.__NEXT_DATA__.autoExport;
-                    if (this.basePath = "", this.sub = f, this.clc = null, this._wrapApp = u, this.isSsr = !0, this.isLocaleDomain = !1, this.isReady = !!(self.__NEXT_DATA__.gssp || self.__NEXT_DATA__.gip || self.__NEXT_DATA__.appGip && !self.__NEXT_DATA__.gsp || !j && !self.location.search), this.state = {
-                            route: S,
+                    let S = (0, h.isDynamicRoute)(e) && self.__NEXT_DATA__.autoExport;
+                    if (this.basePath = "", this.sub = f, this.clc = null, this._wrapApp = u, this.isSsr = !0, this.isLocaleDomain = !1, this.isReady = !!(self.__NEXT_DATA__.gssp || self.__NEXT_DATA__.gip || self.__NEXT_DATA__.appGip && !self.__NEXT_DATA__.gsp || !S && !self.location.search), this.state = {
+                            route: j,
                             pathname: e,
                             query: t,
-                            asPath: j ? e : n,
+                            asPath: S ? e : n,
                             isPreview: !!P,
                             locale: void 0,
                             isFallback: m
                         }, this._initialMatchesMiddlewarePromise = Promise.resolve(!1), !n.startsWith("//")) {
                         let r = {
                                 locale: g
                             },
@@ -3427,15 +3463,18 @@
                 return f
             }
         },
         3105: function(e, t) {
             "use strict";
 
             function r(e, t) {
-                void 0 === t && (t = {});
+                if (void 0 === t && (t = {}), t.onlyHashChange) {
+                    e();
+                    return
+                }
                 let r = document.documentElement,
                     n = r.style.scrollBehavior;
                 r.style.scrollBehavior = "auto", t.dontForceLayout || r.getClientRects(), e(), r.style.scrollBehavior = n
             }
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), Object.defineProperty(t, "handleSmoothScroll", {
@@ -4275,15 +4314,15 @@
                 get: function() {
                     return r
                 }
             });
             let r = e => {}
         },
         8018: function(e) {
-            var t, r, n, a, o, i, l, u, s, c, f, d, h, p, m, g, y, _, b, v, P, w, S, j, O, E, R, x, C, M, A, L, I, T, N, k, D, B, H, U, F, W, q, z, G, V;
+            var t, r, n, a, o, i, l, u, s, c, f, d, h, p, m, g, y, _, b, v, P, w, j, S, E, O, R, x, C, M, A, L, I, T, N, k, D, B, H, U, F, W, q, z, G, V;
             (t = {}).d = function(e, r) {
                 for (var n in r) t.o(r, n) && !t.o(e, n) && Object.defineProperty(e, n, {
                     enumerable: !0,
                     get: r[n]
                 })
             }, t.o = function(e, t) {
                 return Object.prototype.hasOwnProperty.call(e, t)
@@ -4291,15 +4330,15 @@
                 "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
                     value: "Module"
                 }), Object.defineProperty(e, "__esModule", {
                     value: !0
                 })
             }, void 0 !== t && (t.ab = "//"), r = {}, t.r(r), t.d(r, {
                 getCLS: function() {
-                    return S
+                    return j
                 },
                 getFCP: function() {
                     return v
                 },
                 getFID: function() {
                     return M
                 },
@@ -4309,15 +4348,15 @@
                 getLCP: function() {
                     return z
                 },
                 getTTFB: function() {
                     return V
                 },
                 onCLS: function() {
-                    return S
+                    return j
                 },
                 onFCP: function() {
                     return v
                 },
                 onFID: function() {
                     return M
                 },
@@ -4405,15 +4444,15 @@
                 (l || u) && (r = m(e, o, n, t.reportAllChanges), l && i([l]), s(function(a) {
                     r = m(e, o = d("FCP"), n, t.reportAllChanges), requestAnimationFrame(function() {
                         requestAnimationFrame(function() {
                             o.value = performance.now() - a.timeStamp, r(!0)
                         })
                     })
                 }))
-            }, P = !1, w = -1, S = function(e, t) {
+            }, P = !1, w = -1, j = function(e, t) {
                 t = t || {};
                 var r = [.1, .25];
                 P || (v(function(e) {
                     w = e.value
                 }), P = !0);
                 var n, a = function(t) {
                         w > -1 && e(t)
@@ -4432,21 +4471,21 @@
                     },
                     c = h("layout-shift", u);
                 c && (n = m(a, o, r, t.reportAllChanges), p(function() {
                     u(c.takeRecords()), n(!0)
                 }), s(function() {
                     i = 0, w = -1, n = m(a, o = d("CLS", 0), r, t.reportAllChanges)
                 }))
-            }, j = {
+            }, S = {
                 passive: !0,
                 capture: !0
-            }, O = new Date, E = function(e, t) {
+            }, E = new Date, O = function(e, t) {
                 n || (n = t, a = e, o = new Date, C(removeEventListener), R())
             }, R = function() {
-                if (a >= 0 && a < o - O) {
+                if (a >= 0 && a < o - E) {
                     var e = {
                         entryType: "first-input",
                         name: n.type,
                         target: n.target,
                         cancelable: n.cancelable,
                         startTime: n.timeStamp,
                         processingStart: n.timeStamp + a
@@ -4455,24 +4494,24 @@
                         t(e)
                     }), i = []
                 }
             }, x = function(e) {
                 if (e.cancelable) {
                     var t, r, n, a = (e.timeStamp > 1e12 ? new Date : performance.now()) - e.timeStamp;
                     "pointerdown" == e.type ? (t = function() {
-                        E(a, e), n()
+                        O(a, e), n()
                     }, r = function() {
                         n()
                     }, n = function() {
-                        removeEventListener("pointerup", t, j), removeEventListener("pointercancel", r, j)
-                    }, addEventListener("pointerup", t, j), addEventListener("pointercancel", r, j)) : E(a, e)
+                        removeEventListener("pointerup", t, S), removeEventListener("pointercancel", r, S)
+                    }, addEventListener("pointerup", t, S), addEventListener("pointercancel", r, S)) : O(a, e)
                 }
             }, C = function(e) {
                 ["mousedown", "keydown", "touchstart", "pointerdown"].forEach(function(t) {
-                    return e(t, x, j)
+                    return e(t, x, S)
                 })
             }, M = function(e, t) {
                 t = t || {};
                 var r, o = [100, 300],
                     l = b(),
                     u = d("FID"),
                     c = function(e) {
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/_app-08072decd7c39068.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2050,18 +2050,18 @@
             }
             a(_, M, R);
             let B = (0, o.ZP)({
                     prop: "width",
                     transform: I
                 }),
                 z = e => void 0 !== e.maxWidth && null !== e.maxWidth ? (0, s.k9)(e, e.maxWidth, t => {
-                    var r, n, o;
-                    let i = (null == (r = e.theme) ? void 0 : null == (n = r.breakpoints) ? void 0 : null == (o = n.values) ? void 0 : o[t]) || s.VO[t];
+                    var r;
+                    let n = (null == (r = e.theme) || null == (r = r.breakpoints) || null == (r = r.values) ? void 0 : r[t]) || s.VO[t];
                     return {
-                        maxWidth: i || I(t)
+                        maxWidth: n || I(t)
                     }
                 }) : null;
             z.filterProps = ["maxWidth"];
             let F = (0, o.ZP)({
                     prop: "minWidth",
                     transform: I
                 }),
@@ -2903,40 +2903,40 @@
                 }, e.typography.body1, {
                     backgroundColor: (e.vars || e).palette.background.default,
                     "@media print": {
                         backgroundColor: (e.vars || e).palette.common.white
                     }
                 }),
                 A = (e, t = !1) => {
-                    var r, n;
-                    let o = {};
+                    var r;
+                    let n = {};
                     t && e.colorSchemes && Object.entries(e.colorSchemes).forEach(([t, r]) => {
-                        var n;
-                        o[e.getColorSchemeSelector(t).replace(/\s*&/, "")] = {
-                            colorScheme: null == (n = r.palette) ? void 0 : n.mode
+                        var o;
+                        n[e.getColorSchemeSelector(t).replace(/\s*&/, "")] = {
+                            colorScheme: null == (o = r.palette) ? void 0 : o.mode
                         }
                     });
-                    let i = (0, l.Z)({
+                    let o = (0, l.Z)({
                             html: S(e, t),
                             "*, *::before, *::after": {
                                 boxSizing: "inherit"
                             },
                             "strong, b": {
                                 fontWeight: e.typography.fontWeightBold
                             },
                             body: (0, l.Z)({
                                 margin: 0
                             }, O(e), {
                                 "&::backdrop": {
                                     backgroundColor: (e.vars || e).palette.background.default
                                 }
                             })
-                        }, o),
-                        a = null == (r = e.components) ? void 0 : null == (n = r.MuiCssBaseline) ? void 0 : n.styleOverrides;
-                    return a && (i = [i, a]), i
+                        }, n),
+                        i = null == (r = e.components) || null == (r = r.MuiCssBaseline) ? void 0 : r.styleOverrides;
+                    return i && (o = [o, i]), o
                 };
             var C = function(e) {
                     let t = (0, $.Z)({
                             props: e,
                             name: "MuiCssBaseline"
                         }),
                         {
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js` & `systembridgefrontend-3.8.1/systembridgefrontend/out/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
-self.__BUILD_MANIFEST = function(s, a, c, e, t, p, i, n, d, f, b, u) {
+self.__BUILD_MANIFEST = function(s, a, c, e, t, p, i, n, d, f, u, b) {
     return {
         __rewrites: {
             beforeFiles: [],
             afterFiles: [],
             fallback: []
         },
         "/": [s, a, "static/chunks/pages/index-f934b9a030f633a0.js"],
         "/_error": ["static/chunks/pages/_error-54de1933a164a1ff.js"],
         "/app/bridges/openon": [s, a, c, e, t, p, n, "static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js"],
         "/app/bridges/setup": [s, a, c, e, t, p, d, "static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js"],
-        "/app/data": [s, a, e, i, "static/chunks/731-b6cafe94e88ed8c7.js", "static/chunks/pages/app/data-59d72c465167efc4.js"],
+        "/app/data": [s, a, e, i, "static/chunks/731-8a6748b651b08a0a.js", "static/chunks/pages/app/data-59d72c465167efc4.js"],
         "/app/notification": [s, a, p, "static/chunks/pages/app/notification-416e0ab0e8597db3.js"],
-        "/app/player/audio": [s, f, a, c, i, b, u, "static/chunks/pages/app/player/audio-3826169d9ca46804.js"],
-        "/app/player/video": [s, f, a, c, i, b, u, "static/chunks/pages/app/player/video-9c7e9646d273d6aa.js"],
+        "/app/player/audio": [s, f, a, c, i, u, b, "static/chunks/pages/app/player/audio-3826169d9ca46804.js"],
+        "/app/player/video": [s, f, a, c, i, u, b, "static/chunks/pages/app/player/video-9c7e9646d273d6aa.js"],
         "/app/settings": [s, "static/chunks/29107295-809b6f0b05884bf7.js", a, c, e, t, n, d, "static/chunks/826-25c5c840b401fbf5.js", "static/chunks/pages/app/settings-c2e844bc6170d7a5.js"],
         sortedPages: ["/", "/_app", "/_error", "/app/bridges/openon", "/app/bridges/setup", "/app/data", "/app/notification", "/app/player/audio", "/app/player/video", "/app/settings"]
     }
-}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-be8afb194db80d1f.js", "static/chunks/728-4d1eeb7a2f426351.js", "static/chunks/498-c0ac8cca5a5197e4.js", "static/chunks/699-a015e8646ccfaf97.js", "static/chunks/154-454aae7a1f6cc481.js", "static/chunks/361-70173883768cacf6.js", "static/chunks/713-76d25fee0de05077.js", "static/chunks/767-21712ed9071ee20e.js", "static/chunks/75fc9c18-c0cb841eaf75495d.js", "static/chunks/514-17895623628db944.js", "static/chunks/142-6fa2d4be01c7dab9.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
+}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-1ec0772e58be8d0c.js", "static/chunks/728-4d1eeb7a2f426351.js", "static/chunks/498-4e8ce630a90e85c2.js", "static/chunks/699-a015e8646ccfaf97.js", "static/chunks/154-454aae7a1f6cc481.js", "static/chunks/361-70173883768cacf6.js", "static/chunks/713-b2b4846010d39d53.js", "static/chunks/767-21712ed9071ee20e.js", "static/chunks/75fc9c18-6f0090aa3d354e90.js", "static/chunks/514-87c66909ad150ba9.js", "static/chunks/142-6fa2d4be01c7dab9.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/bridges/openon.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/bridges/openon.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/713-76d25fee0de05077.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-4e8ce630a90e85c2.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/713-b2b4846010d39d53.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/bridges/setup.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/bridges/setup.html`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/767-21712ed9071ee20e.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-4e8ce630a90e85c2.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/767-21712ed9071ee20e.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/data.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/data.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/731-b6cafe94e88ed8c7.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-59d72c465167efc4.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Media</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-9" aria-controls="scrollable-auto-tabpanel-9">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/498-4e8ce630a90e85c2.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/731-8a6748b651b08a0a.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-59d72c465167efc4.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Media</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-9" aria-controls="scrollable-auto-tabpanel-9">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/notification.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/notification.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/player/audio.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/player/audio.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-17895623628db944.js" defer=""></script><script src="/_next/static/chunks/142-6fa2d4be01c7dab9.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-6f0090aa3d354e90.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-87c66909ad150ba9.js" defer=""></script><script src="/_next/static/chunks/142-6fa2d4be01c7dab9.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/player/video.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/player/video.html`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-17895623628db944.js" defer=""></script><script src="/_next/static/chunks/142-6fa2d4be01c7dab9.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-6f0090aa3d354e90.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-87c66909ad150ba9.js" defer=""></script><script src="/_next/static/chunks/142-6fa2d4be01c7dab9.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/app/settings.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/app/settings.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-809b6f0b05884bf7.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/713-76d25fee0de05077.js" defer=""></script><script src="/_next/static/chunks/767-21712ed9071ee20e.js" defer=""></script><script src="/_next/static/chunks/826-25c5c840b401fbf5.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-809b6f0b05884bf7.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-4e8ce630a90e85c2.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/713-b2b4846010d39d53.js" defer=""></script><script src="/_next/static/chunks/767-21712ed9071ee20e.js" defer=""></script><script src="/_next/static/chunks/826-25c5c840b401fbf5.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/favicon.svg` & `systembridgefrontend-3.8.1/systembridgefrontend/out/favicon.svg`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend/out/index.html` & `systembridgefrontend-3.8.1/systembridgefrontend/out/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js" defer=""></script><script src="/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"sSLrbmPkLTT_gNozLHC0I","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-92011a1a7f336a6f.js" defer=""></script><script src="/_next/static/chunks/pages/_app-08072decd7c39068.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-1ec0772e58be8d0c.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js" defer=""></script><script src="/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"E7eXuapuFPIf8l3VFcw-l","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.8.0.dev9/systembridgefrontend.egg-info/SOURCES.txt` & `systembridgefrontend-3.8.1/systembridgefrontend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 systembridgefrontend.egg-info/PKG-INFO
 systembridgefrontend.egg-info/SOURCES.txt
 systembridgefrontend.egg-info/dependency_links.txt
 systembridgefrontend.egg-info/top_level.txt
 systembridgefrontend/out/404.html
 systembridgefrontend/out/favicon.svg
 systembridgefrontend/out/index.html
-systembridgefrontend/out/_next/static/chunks/134-be8afb194db80d1f.js
+systembridgefrontend/out/_next/static/E7eXuapuFPIf8l3VFcw-l/_buildManifest.js
+systembridgefrontend/out/_next/static/E7eXuapuFPIf8l3VFcw-l/_ssgManifest.js
+systembridgefrontend/out/_next/static/chunks/134-1ec0772e58be8d0c.js
 systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js
 systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js
 systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js
 systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
 systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
-systembridgefrontend/out/_next/static/chunks/498-c0ac8cca5a5197e4.js
-systembridgefrontend/out/_next/static/chunks/514-17895623628db944.js
+systembridgefrontend/out/_next/static/chunks/498-4e8ce630a90e85c2.js
+systembridgefrontend/out/_next/static/chunks/514-87c66909ad150ba9.js
 systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js
-systembridgefrontend/out/_next/static/chunks/713-76d25fee0de05077.js
+systembridgefrontend/out/_next/static/chunks/713-b2b4846010d39d53.js
 systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js
-systembridgefrontend/out/_next/static/chunks/731-b6cafe94e88ed8c7.js
-systembridgefrontend/out/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js
+systembridgefrontend/out/_next/static/chunks/731-8a6748b651b08a0a.js
+systembridgefrontend/out/_next/static/chunks/75fc9c18-6f0090aa3d354e90.js
 systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js
 systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js
 systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
 systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js
-systembridgefrontend/out/_next/static/chunks/main-2ecf43899f8683c2.js
+systembridgefrontend/out/_next/static/chunks/main-92011a1a7f336a6f.js
 systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
@@ -38,15 +40,15 @@
 systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
 systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js
-systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js
+systembridgefrontend/out/_next/static/chunks/pages/_app-08072decd7c39068.js
 systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
 systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
 systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js
 systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js
 systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js
 systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js
 systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js
@@ -63,16 +65,14 @@
 systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
 systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
 systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
 systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
 systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
 systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
 systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
-systembridgefrontend/out/_next/static/sSLrbmPkLTT_gNozLHC0I/_buildManifest.js
-systembridgefrontend/out/_next/static/sSLrbmPkLTT_gNozLHC0I/_ssgManifest.js
 systembridgefrontend/out/app/data.html
 systembridgefrontend/out/app/notification.html
 systembridgefrontend/out/app/settings.html
 systembridgefrontend/out/app/bridges/openon.html
 systembridgefrontend/out/app/bridges/setup.html
 systembridgefrontend/out/app/player/audio.html
 systembridgefrontend/out/app/player/video.html
```

