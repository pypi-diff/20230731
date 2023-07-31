# Comparing `tmp/harmonai-tools-0.0.4.tar.gz` & `tmp/harmonai-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonai-tools-0.0.4.tar", last modified: Wed Jul 26 16:18:13 2023, max compression
+gzip compressed data, was "harmonai-tools-0.0.5.tar", last modified: Fri Jul 28 19:52:58 2023, max compression
```

## Comparing `harmonai-tools-0.0.4.tar` & `harmonai-tools-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.4/README.md
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/__init__.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools/data/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/data/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.4/harmonai_tools/data/dataset.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/data/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/inference/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/inference/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3162 2023-07-22 08:03:32.000000 harmonai-tools-0.0.4/harmonai_tools/inference/generation.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5146 2023-07-22 08:03:42.000000 harmonai-tools-0.0.4/harmonai_tools/inference/sampling.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      798 2023-07-25 21:08:25.000000 harmonai-tools-0.0.4/harmonai_tools/inference/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/interface/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.4/harmonai_tools/interface/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     7186 2023-07-26 16:13:56.000000 harmonai-tools-0.0.4/harmonai_tools/interface/gradio.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/models/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/models/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15321 2023-07-24 20:06:26.000000 harmonai-tools-0.0.4/harmonai_tools/models/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.4/harmonai_tools/models/blocks.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.4/harmonai_tools/models/bottleneck.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12143 2023-07-18 19:21:16.000000 harmonai-tools-0.0.4/harmonai_tools/models/conditioners.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18798 2023-07-23 21:05:39.000000 harmonai-tools-0.0.4/harmonai_tools/models/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.4/harmonai_tools/models/discriminators.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4148 2023-07-21 07:18:52.000000 harmonai-tools-0.0.4/harmonai_tools/models/factory.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.4/harmonai_tools/models/pretransforms.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.4/harmonai_tools/models/wavelets.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/harmonai_tools/training/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.4/harmonai_tools/training/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11972 2023-07-24 20:17:16.000000 harmonai-tools-0.0.4/harmonai_tools/training/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    27359 2023-07-21 05:02:50.000000 harmonai-tools-0.0.4/harmonai_tools/training/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5184 2023-07-21 03:28:12.000000 harmonai-tools-0.0.4/harmonai_tools/training/factory.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1075 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      424 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-26 16:18:12.000000 harmonai-tools-0.0.4/harmonai_tools.egg-info/top_level.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.4/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-26 16:18:13.000000 harmonai-tools-0.0.4/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1103 2023-07-26 16:16:21.000000 harmonai-tools-0.0.4/setup.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/LICENSE
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.5/README.md
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/harmonai_tools/__init__.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools/data/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/harmonai_tools/data/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.5/harmonai_tools/data/dataset.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/harmonai_tools/data/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools/inference/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/harmonai_tools/inference/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3162 2023-07-22 08:03:32.000000 harmonai-tools-0.0.5/harmonai_tools/inference/generation.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5442 2023-07-28 18:03:27.000000 harmonai-tools-0.0.5/harmonai_tools/inference/sampling.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      798 2023-07-25 21:08:25.000000 harmonai-tools-0.0.5/harmonai_tools/inference/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools/interface/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.5/harmonai_tools/interface/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     8325 2023-07-27 19:08:57.000000 harmonai-tools-0.0.5/harmonai_tools/interface/gradio.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools/models/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/harmonai_tools/models/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15321 2023-07-24 20:06:26.000000 harmonai-tools-0.0.5/harmonai_tools/models/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.5/harmonai_tools/models/blocks.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.5/harmonai_tools/models/bottleneck.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12143 2023-07-18 19:21:16.000000 harmonai-tools-0.0.5/harmonai_tools/models/conditioners.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18798 2023-07-23 21:05:39.000000 harmonai-tools-0.0.5/harmonai_tools/models/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.5/harmonai_tools/models/discriminators.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4262 2023-07-28 19:25:25.000000 harmonai-tools-0.0.5/harmonai_tools/models/factory.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.5/harmonai_tools/models/pretransforms.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.5/harmonai_tools/models/wavelets.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools/training/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.5/harmonai_tools/training/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11971 2023-07-28 05:44:14.000000 harmonai-tools-0.0.5/harmonai_tools/training/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    27359 2023-07-21 05:02:50.000000 harmonai-tools-0.0.5/harmonai_tools/training/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5184 2023-07-21 03:28:12.000000 harmonai-tools-0.0.5/harmonai_tools/training/factory.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools.egg-info/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-28 19:52:57.000000 harmonai-tools-0.0.5/harmonai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1075 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-28 19:52:57.000000 harmonai-tools-0.0.5/harmonai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      590 2023-07-28 19:52:57.000000 harmonai-tools-0.0.5/harmonai_tools.egg-info/requires.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/harmonai_tools.egg-info/top_level.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.5/pyproject.toml
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-28 19:52:58.000000 harmonai-tools-0.0.5/setup.cfg
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1258 2023-07-28 19:50:35.000000 harmonai-tools-0.0.5/setup.py
```

### Comparing `harmonai-tools-0.0.4/LICENSE` & `harmonai-tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/data/dataset.py` & `harmonai-tools-0.0.5/harmonai_tools/data/dataset.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/data/utils.py` & `harmonai-tools-0.0.5/harmonai_tools/data/utils.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/inference/generation.py` & `harmonai-tools-0.0.5/harmonai_tools/inference/generation.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/inference/sampling.py` & `harmonai-tools-0.0.5/harmonai_tools/inference/sampling.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,53 +54,53 @@
                 x += torch.randn_like(x) * ddim_sigma
 
     # If we are on the last timestep, output the denoised image
     return pred
 
 
 
-def sample_k(model_fn, noise, steps=100, sampler_type="dpmpp-2m-sde", sigma_min=0.5, sigma_max=50, rho=1.0, device="cuda", **extra_args):
+def sample_k(model_fn, noise, steps=100, sampler_type="dpmpp-2m-sde", sigma_min=0.5, sigma_max=50, rho=1.0, device="cuda", callback=None, **extra_args):
 
     denoiser = K.external.VDenoiser(model_fn)
     sigmas = K.sampling.get_sigmas_polyexponential(steps, sigma_min, sigma_max, rho, device=device)
 
     noise = noise * sigmas[0]
 
     with torch.cuda.amp.autocast():
         if sampler_type == "k-heun":
-            return K.sampling.sample_heun(denoiser, noise, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_heun(denoiser, noise, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-lms":
-            return K.sampling.sample_lms(denoiser, noise, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_lms(denoiser, noise, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpmpp-2s-ancestral":
-            return K.sampling.sample_dpmpp_2s_ancestral(denoiser, noise, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpmpp_2s_ancestral(denoiser, noise, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpm-2":
-            return K.sampling.sample_dpm_2(denoiser, noise, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpm_2(denoiser, noise, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpm-fast":
-            return K.sampling.sample_dpm_fast(denoiser, noise, sigma_min, sigma_max, steps, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpm_fast(denoiser, noise, sigma_min, sigma_max, steps, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpm-adaptive":
-            return K.sampling.sample_dpm_adaptive(denoiser, noise, sigma_min, sigma_max, rtol=0.01, atol=0.01, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpm_adaptive(denoiser, noise, sigma_min, sigma_max, rtol=0.01, atol=0.01, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "dpmpp-2m-sde":
-            return K.sampling.sample_dpmpp_2m_sde(denoiser, noise, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpmpp_2m_sde(denoiser, noise, sigmas, disable=False, callback=callback, extra_args=extra_args)
         
 
-def variation_k(model_fn, init_audio, init_noise_level=0.1, steps=100, sampler_type="dpmpp-2m-sde", sigma_max=80, sigma_min=0.5, rho=1.0, device="cuda", **extra_args):
+def variation_k(model_fn, init_audio, init_noise_level=0.1, steps=100, sampler_type="dpmpp-2m-sde", sigma_max=80, sigma_min=0.5, rho=1.0, device="cuda", callback=None, **extra_args):
 
     denoiser = K.external.VDenoiser(model_fn)
     sigmas = K.sampling.get_sigmas_polyexponential(steps, sigma_min, init_noise_level, rho, device=device)
 
     init_audio = init_audio + torch.randn_like(init_audio) * init_noise_level
 
     with torch.cuda.amp.autocast():
         if sampler_type == "k-heun":
-            return K.sampling.sample_heun(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_heun(denoiser, init_audio, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-lms":
-            return K.sampling.sample_lms(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_lms(denoiser, init_audio, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpmpp-2s-ancestral":
-            return K.sampling.sample_dpmpp_2s_ancestral(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpmpp_2s_ancestral(denoiser, init_audio, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpm-2":
-            return K.sampling.sample_dpm_2(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpm_2(denoiser, init_audio, sigmas, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpm-fast":
-            return K.sampling.sample_dpm_fast(denoiser, init_audio, sigma_min, init_noise_level, steps, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpm_fast(denoiser, init_audio, sigma_min, init_noise_level, steps, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "k-dpm-adaptive":
-            return K.sampling.sample_dpm_adaptive(denoiser, init_audio, sigma_min, init_noise_level, rtol=0.01, atol=0.01, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpm_adaptive(denoiser, init_audio, sigma_min, init_noise_level, rtol=0.01, atol=0.01, disable=False, callback=callback, extra_args=extra_args)
         elif sampler_type == "dpmpp-2m-sde":
-            return K.sampling.sample_dpmpp_2m_sde(denoiser, init_audio, sigmas, disable=False, extra_args=extra_args)
+            return K.sampling.sample_dpmpp_2m_sde(denoiser, init_audio, sigmas, disable=False, callback=callback, extra_args=extra_args)
```

### Comparing `harmonai-tools-0.0.4/harmonai_tools/inference/utils.py` & `harmonai-tools-0.0.5/harmonai_tools/inference/utils.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/interface/gradio.py` & `harmonai-tools-0.0.5/harmonai_tools/interface/gradio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 import gradio as gr
 import json 
 import torch
 import torchaudio
 
+from aeiou.viz import audio_spectrogram_image
+
 from torch.nn import functional as F
 
 from einops import rearrange
 
 from ..inference.generation import generate_diffusion_cond
 from ..models.factory import create_model_from_config
 from ..inference.utils import prepare_audio
@@ -42,15 +44,21 @@
         sampler_type="dpmpp-2m-sde",
         sigma_min=0.5,
         sigma_max=50,
         use_init=False,
         init_audio=None,
         init_noise_level=1.0,
         batch_size=1,
+        preview_every=None
         ):
+
+    global preview_images
+
+    preview_images = []
+
     # Return fake stereo audio
 
     conditioning = [{"prompt": prompt, "seconds_start": seconds_start, "seconds_total": seconds_total}] * batch_size
 
     #Get the device from the model
     device = next(model.parameters()).device
 
@@ -63,14 +71,33 @@
         in_sr, init_audio = init_audio
 
         # Turn into torch tensor, converting from int16 to float32
         init_audio = torch.from_numpy(init_audio).float().div(32767).transpose(0, 1)
 
         init_audio = (in_sr, init_audio)
 
+    def progress_callback(callback_info):
+        global preview_images
+        denoised = callback_info["denoised"]
+        current_step = callback_info["i"]
+        sigma = callback_info["sigma"]
+
+        if (current_step - 1) % preview_every == 0:
+
+            if model.pretransform is not None:
+                denoised = model.pretransform.decode(denoised)
+
+            denoised = rearrange(denoised, "b d n -> d (b n)")
+
+            denoised = denoised.clamp(-1, 1).mul(32767).to(torch.int16).cpu()
+
+            audio_spectrogram = audio_spectrogram_image(denoised, sample_rate=sample_rate)
+
+            preview_images.append((audio_spectrogram, f"Step {current_step} sigma={sigma:.3f})"))
+
     audio = generate_diffusion_cond(
         model, 
         conditioning=conditioning,
         steps=steps,
         cfg_scale=cfg_scale,
         batch_size=batch_size,
         sample_size=sample_size,
@@ -78,23 +105,26 @@
         seed=seed,
         device=device,
         sampler_type=sampler_type,
         sigma_min=sigma_min,
         sigma_max=sigma_max,
         init_audio=init_audio,
         init_noise_level=init_noise_level,
+        callback = progress_callback if preview_every is not None else None
     )
 
     audio = rearrange(audio, "b d n -> d (b n)")
 
     audio = audio.clamp(-1, 1).mul(32767).to(torch.int16).cpu()
 
     torchaudio.save("output.wav", audio, sample_rate)
 
-    return "output.wav" 
+    audio_spectrogram = audio_spectrogram_image(audio, sample_rate=sample_rate)
+
+    return ("output.wav", [audio_spectrogram, *preview_images])
 
 def create_sampling_ui():
     with gr.Row():
         prompt = gr.Textbox(show_label=False, placeholder="Prompt", scale=6)
         generate_button = gr.Button("Generate", variant='primary', scale=1)
     
     with gr.Row(equal_height=False):
@@ -115,42 +145,48 @@
             
                 # Seed
                 seed_textbox = gr.Textbox(label="Seed (set to -1 for random seed)", value="-1")
 
             # Sampler params
                 with gr.Row():
                     sampler_type_dropdown = gr.Dropdown(["dpmpp-2m-sde", "k-heun", "k-lms", "k-dpmpp-2s-ancestral", "k-dpm-2", "k-dpm-fast"], label="Sampler type", value="dpmpp-2m-sde")
-                    sigma_min_slider = gr.Slider(minimum=0.0, maximum=2.0, step=0.01, value=0.95, label="Sigma min")
-                    sigma_max_slider = gr.Slider(minimum=0.0, maximum=200.0, step=0.1, value=77, label="Sigma max")
+                    sigma_min_slider = gr.Slider(minimum=0.0, maximum=2.0, step=0.01, value=0.03, label="Sigma min")
+                    sigma_max_slider = gr.Slider(minimum=0.0, maximum=200.0, step=0.1, value=80, label="Sigma max")
 
             with gr.Accordion("Init audio", open=False):
                 init_audio_checkbox = gr.Checkbox(label="Use init audio")
                 init_audio_input = gr.Audio(label="Init audio")
                 init_noise_level_slider = gr.Slider(minimum=0.0, maximum=100.0, step=0.01, value=0.1, label="Init noise level")
 
         with gr.Column():
-            audio_output = gr.Audio(label="Output audio", scale=6, interactive=False)
-            # audio_spectrogram_output = gr.Image(label="Output spectrogram", scale=6, interactive=False)
+            audio_output = gr.Audio(label="Output audio", interactive=False)
+            audio_spectrogram_output = gr.Gallery(label="Output spectrogram", show_label=False)
             send_to_init_button = gr.Button("Send to init audio", scale=1)
             send_to_init_button.click(fn=lambda audio: audio, inputs=[audio_output], outputs=[init_audio_input])
     
-    generate_button.click(fn=generate, inputs=[
-        prompt, 
-        seconds_start_slider, 
-        seconds_total_slider, 
-        cfg_scale_slider, 
-        steps_slider, 
-        seed_textbox, 
-        sampler_type_dropdown, 
-        sigma_min_slider, 
-        sigma_max_slider,
-        init_audio_checkbox,
-        init_audio_input,
-        init_noise_level_slider,
-        ], outputs=audio_output, api_name="generate")
+    generate_button.click(fn=generate, 
+        inputs=[
+            prompt, 
+            seconds_start_slider, 
+            seconds_total_slider, 
+            cfg_scale_slider, 
+            steps_slider, 
+            seed_textbox, 
+            sampler_type_dropdown, 
+            sigma_min_slider, 
+            sigma_max_slider,
+            init_audio_checkbox,
+            init_audio_input,
+            init_noise_level_slider,
+        ], 
+        outputs=[
+            audio_output, 
+            audio_spectrogram_output
+        ], 
+        api_name="generate")
 
 
 def create_txt2audio_ui():
     with gr.Blocks() as ui:
         with gr.Tab("Generation"):
             create_sampling_ui()
```

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/autoencoders.py` & `harmonai-tools-0.0.5/harmonai_tools/models/autoencoders.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/blocks.py` & `harmonai-tools-0.0.5/harmonai_tools/models/blocks.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/bottleneck.py` & `harmonai-tools-0.0.5/harmonai_tools/models/bottleneck.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/conditioners.py` & `harmonai-tools-0.0.5/harmonai_tools/models/conditioners.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/diffusion.py` & `harmonai-tools-0.0.5/harmonai_tools/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/discriminators.py` & `harmonai-tools-0.0.5/harmonai_tools/models/discriminators.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/factory.py` & `harmonai-tools-0.0.5/harmonai_tools/models/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,9 +100,12 @@
     elif bottleneck_type == 'dac_rvq_vae':
         from .bottleneck import DACRVQVAEBottleneck
 
         return DACRVQVAEBottleneck(**bottleneck_config["config"])
     elif bottleneck_type == 'memcodes':
         from .bottleneck import MemcodesBottleneck
         return MemcodesBottleneck(**bottleneck_config["config"])
+    elif bottleneck_type == 'l2_norm':
+        from .bottleneck import L2Bottleneck
+        return L2Bottleneck()
     else:
         raise NotImplementedError(f'Unknown bottleneck type: {bottleneck_type}')
```

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/pretransforms.py` & `harmonai-tools-0.0.5/harmonai_tools/models/pretransforms.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/models/wavelets.py` & `harmonai-tools-0.0.5/harmonai_tools/models/wavelets.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/training/autoencoders.py` & `harmonai-tools-0.0.5/harmonai_tools/training/autoencoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(
             self, 
             autoencoder: AudioAutoencoder,
             lr: float = 1e-4,
             warmup_steps: int = 150000,
             sample_rate=48000,
             loss_config: dict = None,
-            use_ema: bool = False,
+            use_ema: bool = True,
             ema_copy = None
     ):
         super().__init__()
 
         self.automatic_optimization = False
 
         self.autoencoder = autoencoder
```

### Comparing `harmonai-tools-0.0.4/harmonai_tools/training/diffusion.py` & `harmonai-tools-0.0.5/harmonai_tools/training/diffusion.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools/training/factory.py` & `harmonai-tools-0.0.5/harmonai_tools/training/factory.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.4/harmonai_tools.egg-info/SOURCES.txt` & `harmonai-tools-0.0.5/harmonai_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

