# Comparing `tmp/pellipop-0.2.0.tar.gz` & `tmp/pellipop-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pellipop-0.2.0.tar", last modified: Fri Jul  7 08:39:15 2023, max compression
+gzip compressed data, was "pellipop-0.3.0.tar", last modified: Mon Jul 31 13:21:25 2023, max compression
```

## Comparing `pellipop-0.2.0.tar` & `pellipop-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.252168 pellipop-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.248167 pellipop-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.248167 pellipop-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 08:39:04.000000 pellipop-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-07 08:39:04.000000 pellipop-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 08:39:15.252168 pellipop-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 08:39:04.000000 pellipop-0.2.0/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 08:39:04.000000 pellipop-0.2.0/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.248167 pellipop-0.2.0/pellipop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:04.000000 pellipop-0.2.0/pellipop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-07 08:39:04.000000 pellipop-0.2.0/pellipop/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.252168 pellipop-0.2.0/pellipop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 08:39:04.000000 pellipop-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:39:15.252168 pellipop-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-07 08:39:04.000000 pellipop-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:21:25.735240 pellipop-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:21:25.731239 pellipop-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:21:25.731239 pellipop-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 13:21:15.000000 pellipop-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-31 13:21:15.000000 pellipop-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-31 13:21:25.735240 pellipop-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-31 13:21:15.000000 pellipop-0.3.0/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-31 13:21:15.000000 pellipop-0.3.0/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:21:25.731239 pellipop-0.3.0/pellipop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:21:15.000000 pellipop-0.3.0/pellipop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-31 13:21:15.000000 pellipop-0.3.0/pellipop/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:21:25.735240 pellipop-0.3.0/pellipop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-31 13:21:25.000000 pellipop-0.3.0/pellipop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-31 13:21:25.000000 pellipop-0.3.0/pellipop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:21:25.000000 pellipop-0.3.0/pellipop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 13:21:25.000000 pellipop-0.3.0/pellipop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 13:21:25.000000 pellipop-0.3.0/pellipop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 13:21:25.000000 pellipop-0.3.0/pellipop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 13:21:15.000000 pellipop-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:21:25.735240 pellipop-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-31 13:21:15.000000 pellipop-0.3.0/setup.py
```

### Comparing `pellipop-0.2.0/.github/workflows/python-publish.yml` & `pellipop-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pellipop-0.2.0/.gitignore` & `pellipop-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pellipop-0.2.0/PKG-INFO` & `pellipop-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pellipop
-Version: 0.2.0
+Version: 0.3.0
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Pellipop
 
 ## Installation
```

### Comparing `pellipop-0.2.0/Readme.md` & `pellipop-0.3.0/Readme.md`

 * *Files identical despite different names*

### Comparing `pellipop-0.2.0/description.md` & `pellipop-0.3.0/description.md`

 * *Files identical despite different names*

### Comparing `pellipop-0.2.0/pellipop/main.py` & `pellipop-0.3.0/pellipop/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,21 @@
 def save_frame_range_sec(video_path, duree, step_sec, output_folder):
     cap = cv2.VideoCapture(video_path)
 
     if not cap.isOpened():
         print(f"impossible de lire {video_path}")
         return
         
-    digit = len(str(int(cap.get(cv2.CAP_PROP_FRAME_COUNT))))
     fps = cap.get(cv2.CAP_PROP_FPS)
     fps_inv = 1 / fps
 
     sec = 0
 
     with tqdm(total=round(duree / step_sec), desc=f"Etat d'avancement de : {video_path}") as bar:
-        while True:
+        while sec <= duree:
             n = round(fps * sec)
             cap.set(cv2.CAP_PROP_POS_FRAMES, n)
             ret, frame = cap.read()
             file_name = os.path.join(output_folder, format_time(n, fps_inv))
             if ret:
                 if not cv2.imwrite(file_name, frame):
                     print("error saving image")
@@ -68,21 +67,20 @@
     #Affichage des informations à l'utilisateur-trice
     print("\n*** Liste des vidéos à découper : ***\n")
     print(fichiers)
     print("\nVous souhaitez découpez " + str(len(fichiers)) + " vidéos. Chaque vidéo va être découpée en images fixes séparées les unes des autres de " + str(intervalle_de_temps) + " secondes.\n")
 
     #Programme de découpe
     for fichier in tqdm(fichiers, desc="Nombre de vidéos traitées"):
-        input_file = os.path.join(input_folder, fichier)
-        duree = int(VideoFileClip(input_file).duration) #calcul la durée de la vidéo pour la gestion de l'affichage de l'avancement du traitement pour chaque vidéo.
+        duree = int(VideoFileClip(fichier).duration) #calcul la durée de la vidéo pour la gestion de l'affichage de l'avancement du traitement pour chaque vidéo.
         
         output_path = os.path.join(output_folder, "output_pellipop", os.path.basename(fichier).split('.')[0].strip().replace(' ', '_'))
         os.makedirs(output_path, exist_ok=True)
         
-        save_frame_range_sec(input_file, duree, intervalle_de_temps, output_path)
+        save_frame_range_sec(fichier, duree, intervalle_de_temps, output_path)
 
         if remove_duplicates:
             delete_duplicates(output_path)
 
     #Note : la valeur 500 (minutes)*60 (pour passer en secondes) est une valeur aléatoire, l'idée est juste de donnée une longueur max de film au-delà de laquelle on ne regarde pas. Mais si le film est plus court ça ne semble pas poser de soucis.
 
     print("Travail terminé !")
```

### Comparing `pellipop-0.2.0/pellipop.egg-info/PKG-INFO` & `pellipop-0.3.0/pellipop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pellipop
-Version: 0.2.0
+Version: 0.3.0
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Pellipop
 
 ## Installation
```

### Comparing `pellipop-0.2.0/setup.py` & `pellipop-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "pellipop"
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
@@ -32,8 +32,8 @@
                         ]
                     },
                     packages=find_packages())
 
     setup(**metadata)
 
 if __name__ == "__main__":
-    setup_package()
+    setup_package()
```

