# Comparing `tmp/django_ocr_translate-0.1.3.tar.gz` & `tmp/django_ocr_translate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ocr_translate-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ocr_translate-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ocr_translate-0.1.3.tar` & `django_ocr_translate-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1152 2023-07-27 00:26:54.434847 django_ocr_translate-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    35821 2023-07-17 20:52:55.210676 django_ocr_translate-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0    12769 2023-07-27 21:45:27.432567 django_ocr_translate-0.1.3/README.md
--rw-r--r--   0        0        0      761 2023-07-27 21:10:13.816065 django_ocr_translate-0.1.3/build.sh
--rw-r--r--   0        0        0     1593 2023-07-27 21:30:15.182242 django_ocr_translate-0.1.3/ocr_translate/__init__.py
--rw-r--r--   0        0        0     2354 2023-07-27 00:26:54.442034 django_ocr_translate-0.1.3/ocr_translate/admin.py
--rw-r--r--   0        0        0     1779 2023-07-27 00:26:54.443334 django_ocr_translate-0.1.3/ocr_translate/apps.py
--rw-r--r--   0        0        0    15700 2023-07-27 17:52:11.399422 django_ocr_translate-0.1.3/ocr_translate/messaging.py
--rw-r--r--   0        0        0     7500 2023-07-17 20:52:55.232594 django_ocr_translate-0.1.3/ocr_translate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-17 20:52:55.234224 django_ocr_translate-0.1.3/ocr_translate/migrations/__init__.py
--rw-r--r--   0        0        0     6533 2023-07-27 00:26:54.445903 django_ocr_translate-0.1.3/ocr_translate/models.py
--rw-r--r--   0        0        0     2017 2023-07-27 17:52:11.403664 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/__init__.py
--rw-r--r--   0        0        0     8816 2023-07-27 17:52:11.406532 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/box.py
--rw-r--r--   0        0        0     4424 2023-07-27 00:26:54.450181 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/full.py
--rw-r--r--   0        0        0     3918 2023-07-27 17:52:11.410024 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/huggingface.py
--rw-r--r--   0        0        0     5068 2023-07-27 17:52:11.410530 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/initializers.py
--rw-r--r--   0        0        0     2111 2023-07-27 00:26:54.451236 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/lang.py
--rw-r--r--   0        0        0    32920 2023-07-27 00:26:54.452276 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/languages.json
--rw-r--r--   0        0        0     3528 2023-07-27 00:26:54.452676 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/models.json
--rw-r--r--   0        0        0     8183 2023-07-27 17:52:11.414152 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/ocr.py
--rw-r--r--   0        0        0     5361 2023-07-27 17:52:11.414152 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tesseract.py
--rw-r--r--   0        0        0    10549 2023-07-27 17:52:11.427554 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tsl.py
--rw-r--r--   0        0        0     2331 2023-07-27 00:26:54.455809 django_ocr_translate-0.1.3/ocr_translate/queues.py
--rw-r--r--   0        0        0     2048 2023-07-27 00:26:54.458525 django_ocr_translate-0.1.3/ocr_translate/urls.py
--rw-r--r--   0        0        0    12645 2023-07-27 00:26:54.459099 django_ocr_translate-0.1.3/ocr_translate/views.py
--rw-r--r--   0        0        0     2950 2023-07-28 01:13:53.148150 django_ocr_translate-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       74 2023-07-27 00:26:54.461174 django_ocr_translate-0.1.3/requirements-torch-cpu.txt
--rw-r--r--   0        0        0       76 2023-07-27 21:10:13.818678 django_ocr_translate-0.1.3/requirements-torch-cuda.txt
--rw-r--r--   0        0        0      301 2023-07-27 00:26:54.463254 django_ocr_translate-0.1.3/requirements.txt
--rw-r--r--   0        0        0    14672 1970-01-01 00:00:00.000000 django_ocr_translate-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35821 2023-07-17 20:52:55.210676 django_ocr_translate-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0    13070 2023-07-30 19:55:47.143154 django_ocr_translate-0.1.4/README.md
+-rw-r--r--   0        0        0     1593 2023-07-30 19:55:47.145260 django_ocr_translate-0.1.4/ocr_translate/__init__.py
+-rw-r--r--   0        0        0     2354 2023-07-27 00:26:54.442034 django_ocr_translate-0.1.4/ocr_translate/admin.py
+-rw-r--r--   0        0        0     1779 2023-07-27 00:26:54.443334 django_ocr_translate-0.1.4/ocr_translate/apps.py
+-rw-r--r--   0        0        0    15700 2023-07-27 17:52:11.399422 django_ocr_translate-0.1.4/ocr_translate/messaging.py
+-rw-r--r--   0        0        0     7500 2023-07-17 20:52:55.232594 django_ocr_translate-0.1.4/ocr_translate/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1909 2023-07-30 19:55:47.146305 django_ocr_translate-0.1.4/ocr_translate/migrations/0002_ocrboxmodel_default_options_ocrmodel_default_options_and_more_squashed_0005_alter_ocrboxmodel_default_options_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-17 20:52:55.234224 django_ocr_translate-0.1.4/ocr_translate/migrations/__init__.py
+-rw-r--r--   0        0        0     7000 2023-07-30 19:55:47.146829 django_ocr_translate-0.1.4/ocr_translate/models.py
+-rw-r--r--   0        0        0     2017 2023-07-27 17:52:11.403664 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/__init__.py
+-rw-r--r--   0        0        0     8816 2023-07-27 17:52:11.406532 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/box.py
+-rw-r--r--   0        0        0     4424 2023-07-27 00:26:54.450181 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/full.py
+-rw-r--r--   0        0        0     3918 2023-07-27 17:52:11.410024 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/huggingface.py
+-rw-r--r--   0        0        0     5725 2023-07-30 19:55:47.147962 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/initializers.py
+-rw-r--r--   0        0        0     2111 2023-07-27 00:26:54.451236 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/lang.py
+-rw-r--r--   0        0        0    33089 2023-07-30 19:55:47.149581 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/languages.json
+-rw-r--r--   0        0        0     4072 2023-07-30 19:55:47.150630 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/models.json
+-rw-r--r--   0        0        0     8242 2023-07-30 19:55:47.151152 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/ocr.py
+-rw-r--r--   0        0        0     5361 2023-07-27 17:52:11.414152 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/tesseract.py
+-rw-r--r--   0        0        0    10921 2023-07-30 19:55:47.152087 django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/tsl.py
+-rw-r--r--   0        0        0     2331 2023-07-27 00:26:54.455809 django_ocr_translate-0.1.4/ocr_translate/queues.py
+-rw-r--r--   0        0        0     2048 2023-07-27 00:26:54.458525 django_ocr_translate-0.1.4/ocr_translate/urls.py
+-rw-r--r--   0        0        0    12645 2023-07-27 00:26:54.459099 django_ocr_translate-0.1.4/ocr_translate/views.py
+-rw-r--r--   0        0        0     3024 2023-07-30 20:00:40.095901 django_ocr_translate-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-07-27 00:26:54.461174 django_ocr_translate-0.1.4/requirements-torch-cpu.txt
+-rw-r--r--   0        0        0       76 2023-07-27 21:10:13.818678 django_ocr_translate-0.1.4/requirements-torch-cuda.txt
+-rw-r--r--   0        0        0      301 2023-07-27 00:26:54.463254 django_ocr_translate-0.1.4/requirements.txt
+-rw-r--r--   0        0        0    15005 1970-01-01 00:00:00.000000 django_ocr_translate-0.1.4/PKG-INFO
```

### Comparing `django_ocr_translate-0.1.3/LICENSE.txt` & `django_ocr_translate-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/README.md` & `django_ocr_translate-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,79 +2,46 @@
 
 This is a Django app for creating back-end server aimed at performing OCR and translation of images received via a POST request.
 
 The OCR and translation is performed using freely available machine learning models and packages (see below for what is currently implemented).
 
 The server is designed to be used together with [this browser extension](https://github.com/Crivella/ocr_extension), acting as a front-end providing the images and controlling the model languages and models being used.
 
-## Installation
-
-It is strongly suggested to install this project using a [virtual environment](https://docs.python.org/3/library/venv.html).
-
-### From Github
-
-- Clone or download the repository
-  - `git clone https://github.com/Crivella/ocr_translate.git`
-- Install the project dependencies (choose the appropriate files depending if you wanna run on GPU or CPU only):
-  - `pip install -r requirements-torch-[cpu/cuda].txt`
-  - `pip install -r requirements.txt`
-
-### From Docker
-Plan to add a CPU and a CUDA specific image to DockerHUB.
-For now you can create the image yourself by:
-
-- Create a .pip-cache-cpu directory inside your project.
-- Optional: re-install the project dependencies pointing this as the cache folder for pip (will make the build process much faster, by reusing the cached dependencies)
-- Run `docker build -t ocr_server .`
-
-
-### From PyPI
-
-Run the command
-
-- `pip install django-ocr_translate`
-
-By default torch 2.x will come in its CUDA enabled version. While this works also for CPU, it will also install ~1 GB of cuda dependencies.
-If you wish to run on CPU only, download the file [requirements-torch-cpu.txt](requirements-torch-cpu.txt) first and run
-
-- `pip install -r requirements-torch-cpu.txt`
-
-before installing the python package.
-
 ## Running the server
 
-By default the server will use a sqlite database named *db.sqlite3* inside the project main directory.
-If you plan to use a different database, you can either:
+If you plan to use a different settings (eg. database, or model location), you can either:
 
 - manually edit the [settings.py](mysite/settings.py)
 - Use the provided [Environment variables](#environment-variables)
 See below for a [list of supported databases](#supported-databases)
 
 You will also have to modify the `ALLOWED_HOSTS` in case you plan to access the server from somewhere other than *localhost*.
 
+All the different way to run the server may provide different set of default values (each of them is targeted for a different level of usage).
+
 ### From Release file
 
 (Tested on Windows 11)
-From the github releases you can download either:
-
-- The [CPU only version](/releases/latest/download/run_server-cpu.exe)
-- The GPU version split in [file 1](/releases/latest/download/run_server-gpu.zip.001) and [file 2](/releases/latest/download/run_server-gpu.zip.002) (The CUDA dependencies makes it take much more space), wich can be restored using tools like [7zip](https://www.7-zip.org/https://www.7-zip.org/) and [NanaZip](https://github.com/M2Team/NanaZip).
+From the [github releases page](/releases/) you can download either:
 
-Not that every time you run the EXE, it will decompress itself into a temporary folder so:
+- The [CPU only version](/../../releases/latest/download/run_server-cpu.exe)
+- The GPU version split in [file 1](/../../releases/latest/download/run_server-gpu.zip.001) and [file 2](/../../releases/latest/download/run_server-gpu.zip.002) (The CUDA dependencies makes it take much more space), wich can be restored using tools like [7zip](https://www.7-zip.org/https://www.7-zip.org/) and [NanaZip](https://github.com/M2Team/NanaZip).
 
-- The exe will appear as an empty console until all the file are extracted and the actual script start running.
-- By launching the server multiple times without restarting (especially the GPU one), you risk quickly filling up your drive
+Usage:
+Unzip the file and from inside the folder, run the `run_server-XXX.exe` file (XXX=cpu/gpu)
 
-You can either just start the server and it will run with sensible defaults. Most notably the models files and database will be downloaded/created under `%userprofile%/.ocr_translate`.
+The server will run with sensible defaults. Most notably the models files and database will be downloaded/created under `%userprofile%/.ocr_translate`.
 Also the gpu version will attempt to run on GPU by default, and fall-back to CPU if the former is not available.
 
-For customization, you can set the [environment variable](#environment-variables) yourself, either via powershell or by searching for *environment variable* in the settings menu
+For customization, you can set the [environment variable](#environment-variables) yourself, either via powershell or by searching for *environment variable* in the settings menu.
 
 ### From Github installation
 
+See the section on how to [install from Github](#from-github) first.
+
 The Github repo provides not only the Django app files, but also the already configured project files used to start the server.
 
 Create/Initialize your database by running
 
 - `python manage.py migrate`
 
 inside your project folder.
@@ -92,43 +59,85 @@
 Notes:
 
 - Gunicorn workers will each spawn a separate instance of the loaded models, each taking its own space in the memory. This can quickly fill up the memory especially if running on GPU. Ideally set this to 1.
 - Django development server will spawn new threads for handling incoming requests (if no currently existing thread is free), which share the same memory. Running more than one worker per loaded model concurrently might slow down the actual computation and in some case also block the execution.
 
 ### From PyPI installation
 
+See the section on how to [install from PyPI](#from-pypi) first.
+
 When installing the project from PyPI, only the app is available.
 This will need to be integrated in a Django project in order to be used.
 These are the minimal instruction for creating a project and start running the server:
 
 - Run `django-admin startproject mysite` to create a django project
 - Configure the server by replacing the automatically created files (strongly recommended):
   - [settings.py](mysite/settings.py) with the one available on the repo.
   - [urls.py](mysite/urls.py) with the one available on the repo.
 - or by manually editing the files:
   - settings.py: Add the `ocr_translated` app to the `INSTALLED_APPS`
   - urls.py: Include the `'ocr_translate.urls'` into your project urls.
 - From here follow the same instructions as when starting [from Github](#from-github)
 
-### From docker
+### From docker image
+
+See the section on how to [install from DockerHUB](#from-docker) first.
 
 This section assumes you have docker installed and the image of the project.
 
 Run the command:
 
-- `docker run --name CONTAINER_NAME -v PATH_TO_YOUR_MODEL_DIRECTORY:/models -v PATH_TO_DIR_WITH_SQLITE_FILE:/data --env-file=PATH_TO_AND_ENV_VARIABLE_FILE -p SERVER_PORT:4000 -d ocr_server`
+- `docker run --name CONTAINER_NAME -v PATH_TO_YOUR_MODEL_DIRECTORY:/models -v PATH_TO_DIR_WITH_SQLITE_FILE:/data --env-file=PATH_TO_AND_ENV_VARIABLE_FILE -p SERVER_PORT:4000 -d ocr_translate`
 
-See the [Environment variables](#environment-variables) section for configuring your environment variable file. Additionaly the docker image defines 2 other variable to automatically create an admin user for managing the database via the django-admin interface:
+See the [Environment variables](#environment-variables) section for configuring your environment variable file. Additionaly the docker image defines several other variables to automatically create an admin user for managing the database via the django-admin interface:
 
 - `UID`: UID of the user owning the files in /models and /data
 - `GID`: GID of the user owning the files in /models and /data
 - `NUM_WEB_WORKERS`: Number of gunicorn workers for the server
 - `DJANGO_SUPERUSER_USERNAME`: The username of the admin user to be created.
 - `DJANGO_SUPERUSER_PASSWORD`: The password of the admin user to be created.
 
+
+## Installation
+
+For both the Githyb and PyPI installation it is strongly suggested to install this project using a [virtual environment](https://docs.python.org/3/library/venv.html).
+
+### From Github
+
+- Clone or download the repository
+  - `git clone https://github.com/Crivella/ocr_translate.git`
+- Install the project dependencies (choose the appropriate files depending if you wanna run on GPU or CPU only):
+  - `pip install -r requirements-torch-[cpu/cuda].txt`
+  - `pip install -r requirements.txt`
+
+### From Docker
+
+CPU and CUDA specific images are available on [DockerHUB](https://hub.docker.com/r/crivella1/ocr_translate):
+
+- CPU: `docker pull crivella1/ocr_translate:latest-cpu`
+- GPU: `docker pull crivella1/ocr_translate:latest-gpu`
+
+Manually create your image:
+
+- Create a .pip-cache-[cpu/gpu] directory inside your project.
+- Optional: re-install the project dependencies pointing this as the cache folder for pip (will make the build process much faster, by reusing the cached dependencies)
+- Run `docker build -t IMAGE_TAG -f Dockerfile-[cpu/gpu] .`
+
+### From PyPI
+
+Run the command
+
+- `pip install django-ocr_translate`
+
+By default torch 2.x will come in its CUDA enabled version. While this works also for CPU, it will also install ~1 GB of cuda dependencies.
+If you wish to run on CPU only, download the file [requirements-torch-cpu.txt](requirements-torch-cpu.txt) first and run
+
+- `pip install -r requirements-torch-cpu.txt`
+
+before installing the python package.
 ## Supported Box OCR models
 
 - [EasyOCR](https://github.com/JaidedAI/EasyOCR)
 
 ## Supported text OCR models
 
 - Hugging Face [Transformers](https://huggingface.co/docs/transformers/index) VisionEncoderDecoder models
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/__init__.py` & `django_ocr_translate-0.1.4/ocr_translate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # You should have received a copy of the GNU General Public License               #
 # along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
 #                                                                                 #
 # Home: https://github.com/Crivella/ocr_translate                                 #
 ###################################################################################
 """OCR and translation of images."""
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/admin.py` & `django_ocr_translate-0.1.4/ocr_translate/admin.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/apps.py` & `django_ocr_translate-0.1.4/ocr_translate/apps.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/messaging.py` & `django_ocr_translate-0.1.4/ocr_translate/messaging.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/migrations/0001_initial.py` & `django_ocr_translate-0.1.4/ocr_translate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/models.py` & `django_ocr_translate-0.1.4/ocr_translate/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,46 +36,59 @@
     iso2t = models.CharField(max_length=8, unique=True)
     iso3 = models.CharField(max_length=32, unique=True)
 
     easyocr = models.CharField(max_length=32, null=True)
     tesseract = models.CharField(max_length=32, null=True)
     facebookM2M = models.CharField(max_length=32, null=True)
 
-    break_chars = models.CharField(max_length=512, null=True)
-    ignore_chars = models.CharField(max_length=512, null=True)
+    default_options = models.ForeignKey(
+        OptionDict, on_delete=models.CASCADE, related_name='lang_default_options', null=True
+        )
 
     def __str__(self):
         return str(self.iso1)
 
 class OCRModel(models.Model):
     """OCR model using hugging space naming convention"""
     name = models.CharField(max_length=128)
     languages = models.ManyToManyField(Language, related_name='ocr_models')
 
+    default_options = models.ForeignKey(
+        OptionDict, on_delete=models.SET_NULL, related_name='ocr_default_options', null=True
+        )
+
     language_format = models.CharField(max_length=32, null=True)
 
     def __str__(self):
         return str(self.name)
 
 class OCRBoxModel(models.Model):
     """OCR model for bounding boxes"""
     name = models.CharField(max_length=128)
     languages = models.ManyToManyField(Language, related_name='box_models')
 
+    default_options = models.ForeignKey(
+        OptionDict, on_delete=models.SET_NULL, related_name='box_default_options', null=True
+        )
+
     language_format = models.CharField(max_length=32, null=True)
 
     def __str__(self):
         return str(self.name)
 
 class TSLModel(models.Model):
     """Translation models using hugging space naming convention"""
     name = models.CharField(max_length=128)
     src_languages = models.ManyToManyField(Language, related_name='tsl_models_src')
     dst_languages = models.ManyToManyField(Language, related_name='tsl_models_dst')
 
+    default_options = models.ForeignKey(
+        OptionDict, on_delete=models.SET_NULL, related_name='tsl_default_options', null=True
+        )
+
     language_format = models.CharField(max_length=32, null=True)
 
     def __str__(self):
         return str(self.name)
 
 class Image(models.Model):
     """Image registered as the md5 of the uploaded file"""
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/__init__.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/box.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/box.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/full.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/full.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/huggingface.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/huggingface.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/initializers.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/initializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,51 +61,63 @@
     for lang in langs:
         logger.debug(f'Creating language: {lang}')
         name = lang.pop('name')
         iso1 = lang.pop('iso1')
         iso2t = lang.pop('iso2t')
         iso2b = lang.pop('iso2b')
         iso3 = lang.pop('iso3')
+        def_opt = lang.pop('default_options', {})
+        opt_obj, _ = m.OptionDict.objects.get_or_create(options=def_opt)
         l, _ = m.Language.objects.get_or_create(name=name, iso1=iso1, iso2t=iso2t, iso2b=iso2b, iso3=iso3)
+        l.default_options = opt_obj
         for k,v in lang.items():
             setattr(l, k, v)
         l.save()
 
 def auto_create_models():
     """Create OCR and TSL models from json file. Also create default OptionDict"""
     cwd = Path(__file__).parent
     with open(cwd / 'models.json', encoding='utf-8') as f:
         models = json.load(f)
 
     for box in models['box']:
         logger.debug(f'Creating box model: {box}')
         lang = box.pop('lang')
         lcode = box.pop('lang_code')
+        def_opt = box.pop('default_options', {})
+        opt_obj, _ = m.OptionDict.objects.get_or_create(options=def_opt)
         model, _ = m.OCRBoxModel.objects.get_or_create(**box)
+        model.default_options = opt_obj
         model.language_format = lcode
         for l in lang:
             model.languages.add(m.Language.objects.get(iso1=l))
         model.save()
 
     for ocr in models['ocr']:
         logger.debug(f'Creating ocr model: {ocr}')
         lang = ocr.pop('lang')
         lcode = ocr.pop('lang_code')
+        def_opt = ocr.pop('default_options', {})
+        opt_obj, _ = m.OptionDict.objects.get_or_create(options=def_opt)
         model, _ = m.OCRModel.objects.get_or_create(**ocr)
+        model.default_options = opt_obj
         model.language_format = lcode
         for l in lang:
             model.languages.add(m.Language.objects.get(iso1=l))
         model.save()
 
     for tsl in models['tsl']:
         logger.debug(f'Creating tsl model: {tsl}')
         src = tsl.pop('lang_src')
         dst = tsl.pop('lang_dst')
         lcode = tsl.pop('lang_code', None)
+        def_opt = tsl.pop('default_options', {})
+        opt_obj, _ = m.OptionDict.objects.get_or_create(options=def_opt)
         model, _ = m.TSLModel.objects.get_or_create(**tsl)
+        model.default_options = opt_obj
         model.language_format = lcode
         for l in src:
             logger.debug(f'Adding src language: {l}')
             kwargs = {lcode: l}
             model.src_languages.add(*m.Language.objects.filter(**kwargs))
 
         for l in dst:
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/lang.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/lang.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/languages.json` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/languages.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979139218269653%*

 * *Differences: {'41': "{'default_options': OrderedDict([('break_chars', '!?.'), ('restore_dash_newlines', "*

 * *       'True)])}',*

 * * '77': "{'default_options': OrderedDict([('break_chars', '!。?！？'), ('ignore_chars', '♥♡♪〜・.、')]), "*

 * *       "delete: ['break_chars', 'ignore_chars']}"}*

```diff
@@ -337,14 +337,18 @@
         "iso2b": "dzo",
         "iso2t": "dzo",
         "iso3": "dzo",
         "name": "Dzongkha",
         "tesseract": "dzo"
     },
     {
+        "default_options": {
+            "break_chars": "!?.",
+            "restore_dash_newlines": true
+        },
         "easyocr": "en",
         "facebookM2M": "en",
         "iso1": "en",
         "iso2b": "eng",
         "iso2t": "eng",
         "iso3": "eng",
         "name": "English",
@@ -638,18 +642,20 @@
         "iso2b": "ita",
         "iso2t": "ita",
         "iso3": "ita",
         "name": "Italian",
         "tesseract": "ita"
     },
     {
-        "break_chars": "!\u3002?\uff01\uff1f",
+        "default_options": {
+            "break_chars": "!\u3002?\uff01\uff1f",
+            "ignore_chars": "\u2665\u2661\u266a\u301c\u30fb.\u3001"
+        },
         "easyocr": "ja",
         "facebookM2M": "ja",
-        "ignore_chars": "\u2665\u2661\u266a\u301c\u30fb.\u3001",
         "iso1": "ja",
         "iso2b": "jpn",
         "iso2t": "jpn",
         "iso3": "jpn",
         "name": "Japanese",
         "tesseract": "jpn"
     },
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/models.json` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/models.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'tsl'": "{0: {'default_options': OrderedDict([('break_newlines', False)])}, 1: "*

 * *          "{'default_options': OrderedDict([('break_newlines', True)])}, 2: {'default_options': "*

 * *          "OrderedDict([('break_newlines', True)])}, 3: {'default_options': "*

 * *          "OrderedDict([('break_newlines', False)])}, 4: {'default_options': "*

 * *          "OrderedDict([('break_newlines', False)])}, 5: {'default_options': "*

 * *          "OrderedDict([('break_newlines', False)])}}"}*

```diff
@@ -28,54 +28,69 @@
             ],
             "lang_code": "tesseract",
             "name": "tesseract"
         }
     ],
     "tsl": [
         {
+            "default_options": {
+                "break_newlines": false
+            },
             "lang_code": "iso1",
             "lang_dst": [
                 "en"
             ],
             "lang_src": [
                 "zh"
             ],
             "name": "Helsinki-NLP/opus-mt-zh-en"
         },
         {
+            "default_options": {
+                "break_newlines": true
+            },
             "lang_code": "iso1",
             "lang_dst": [
                 "en"
             ],
             "lang_src": [
                 "ja"
             ],
             "name": "Helsinki-NLP/opus-mt-ja-en"
         },
         {
+            "default_options": {
+                "break_newlines": true
+            },
             "lang_code": "iso1",
             "lang_dst": [
                 "en"
             ],
             "lang_src": [
                 "ja"
             ],
             "name": "staka/fugumt-ja-en"
         },
         {
+            "default_options": {
+                "break_newlines": false
+            },
             "lang_code": "iso1",
             "lang_dst": [
                 "en"
             ],
             "lang_src": [
                 "ko"
             ],
             "name": "Helsinki-NLP/opus-mt-ko-en"
         },
         {
+            "default_options": {
+                "break_newlines": false
+            },
             "lang_code": "facebookM2M",
             "lang_dst": [
                 "af",
                 "am",
                 "ar",
                 "az",
                 "ba",
@@ -246,14 +261,17 @@
                 "yo",
                 "zh",
                 "zu"
             ],
             "name": "facebook/m2m100_418M"
         },
         {
+            "default_options": {
+                "break_newlines": false
+            },
             "lang_code": "facebookM2M",
             "lang_dst": [
                 "af",
                 "am",
                 "ar",
                 "az",
                 "ba",
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/ocr.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/ocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,17 @@
     else:
         pixel_values = OCR_IMAGE_PROCESSOR(img, return_tensors='pt').pixel_values
         if dev == 'cuda':
             pixel_values = pixel_values.cuda()
         generated_ids = OCR_MODEL.generate(pixel_values)
         generated_text = OCR_TOKENIZER.batch_decode(generated_ids, skip_special_tokens=True)[0]
 
+    if dev == 'cuda':
+        torch.cuda.empty_cache()
+
     return generated_text
 
 def ocr(*args, id_: Hashable, block: bool = True, **kwargs) -> Union[str, Message]:
     """Queue a text OCR pipeline.
 
     Args:
         id_ (Hashable): A unique identifier for the OCR task.
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tesseract.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/tesseract.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tsl.py` & `django_ocr_translate-0.1.4/ocr_translate/ocr_tsl/tsl.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,33 +66,40 @@
 
 def get_tsl_model() -> m.TSLModel:
     """Get the current TSL model."""
     return TSL_MODEL_OBJ
 
 def pre_tokenize(
         text: str,
-        ignore_chars: str = None, break_chars: str = None, break_newlines: bool = True
+        ignore_chars: str = None, break_chars: str = None, break_newlines: bool = False,
+        restore_dash_newlines: bool = False
         ) -> list[str]:
     """Pre-tokenize a text string.
 
     Args:
         text (str): Text to tokenize.
         ignore_chars (str, optional): String of characters to ignore. Defaults to None.
         break_chars (str, optional): String of characters to break on. Defaults to None.
         break_newlines (bool, optional): Whether to break on newlines. Defaults to True.
+        restore_dash_newlines (bool, optional): Whether to restore dash-newlines (word broken with a -newline).
+            Defaults to False.
 
     Returns:
         list[str]: List of string tokens.
     """
+    if restore_dash_newlines:
+        text = re.sub(r'(?<!\n)- *\n', '', text)
     if ignore_chars is not None:
         text = re.sub(f'[{ignore_chars}]+', '', text)
     if break_chars is None:
         break_chars = ''
     if break_newlines:
         break_chars += '\n'
+    else:
+        text = text.replace('\n', ' ')
 
     break_chars = re.escape(break_chars)
     tokens = text
     if len(break_chars) > 0:
         tokens = re.split(f'[{break_chars}+]', text)
 
     if isinstance(tokens, str):
@@ -140,23 +147,21 @@
     Returns:
         Union[str,list[str]]: Translated text. If text is a list, returns a list of translated strings.
     """
     if options is None:
         options = {}
     TSL_TOKENIZER.src_lang = lang_src
 
-    break_newlines = options.get('break_newlines', True)
-    break_chars = options.get('break_chars', None)
-    ignore_chars = options.get('ignore_chars', None)
+    pre_keys = ['ignore_chars', 'break_chars', 'break_newlines', 'restore_dash_newlines']
+    pre_dct = {k: options[k] for k in pre_keys if k in options}
 
-    args = (ignore_chars, break_chars, break_newlines)
     if isinstance(text, list):
-        tokens = [pre_tokenize(t, *args) for t in text]
+        tokens = [pre_tokenize(t, **pre_dct) for t in text]
     elif isinstance(text, str):
-        tokens = pre_tokenize(text, *args)
+        tokens = pre_tokenize(text, **pre_dct)
     else:
         raise TypeError(f'Unsupported type for text: {type(text)}')
 
     logger.debug(f'TSL: {tokens}')
     if len(tokens) == 0:
         return ''
     encoded = TSL_TOKENIZER(
@@ -185,14 +190,18 @@
         )
 
     tsl = TSL_TOKENIZER.batch_decode(generated_tokens, skip_special_tokens=True)
     logger.debug(f'TSL: {tsl}')
 
     if isinstance(text, str):
         tsl = tsl[0]
+
+    if dev == 'cuda':
+        torch.cuda.empty_cache()
+
     return tsl
 
 def tsl_pipeline(*args, id_: Hashable, batch_id: Hashable = None, block: bool = True, **kwargs):
     """Queue a text translation pipeline.
 
     Args:
         id_ (Hashable): A unique identifier for the OCR task.
@@ -251,17 +260,17 @@
     tsl_run_obj = m.TranslationRun.objects.filter(**params).first()
     if tsl_run_obj is None or force:
         if lazy:
             raise ValueError('Value not found for lazy TSL run')
         logger.info('Running TSL')
         id_ = (text_obj.id, model_obj.id, options_obj.id, src.id, dst.id)
         batch_id = (model_obj.id, options_obj.id, src.id, dst.id)
-        opt_dct = options_obj.options
-        opt_dct.setdefault('break_chars', src.break_chars)
-        opt_dct.setdefault('ignore_chars', src.ignore_chars)
+        lang_dct = getattr(src.default_options, 'options', {})
+        model_dct =  getattr(model_obj.default_options, 'options', {})
+        opt_dct = {**lang_dct, **model_dct, **options_obj.options}
         new = tsl_pipeline(
             text_obj.text,
             getattr(src, model_obj.language_format),
             getattr(dst, model_obj.language_format),
             options=opt_dct,
             id_=id_,
             batch_id=batch_id,
```

### Comparing `django_ocr_translate-0.1.3/ocr_translate/queues.py` & `django_ocr_translate-0.1.4/ocr_translate/queues.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/urls.py` & `django_ocr_translate-0.1.4/ocr_translate/urls.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/ocr_translate/views.py` & `django_ocr_translate-0.1.4/ocr_translate/views.py`

 * *Files identical despite different names*

### Comparing `django_ocr_translate-0.1.3/pyproject.toml` & `django_ocr_translate-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -117,69 +117,73 @@
 00000740: 6d6d 6974 7e3d 332e 332e 3322 2c0d 0a20  mmit~=3.3.3",.. 
 00000750: 2020 2022 7079 6c69 6e74 7e3d 322e 3137     "pylint~=2.17
 00000760: 2e34 222c 0d0a 2020 2020 2270 796c 696e  .4",..    "pylin
 00000770: 742d 7079 7465 7374 7e3d 312e 312e 3222  t-pytest~=1.1.2"
 00000780: 2c0d 0a20 2020 2022 7079 6c69 6e74 2d64  ,..    "pylint-d
 00000790: 6a61 6e67 6f7e 3d32 2e35 2e33 222c 0d0a  jango~=2.5.3",..
 000007a0: 5d0d 0a72 656c 6561 7365 203d 205b 0d0a  ]..release = [..
-000007b0: 2020 2020 2270 7969 6e73 7461 6c6c 6572      "pyinstaller
-000007c0: 220d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 666c  "..]....[tool.fl
-000007d0: 6974 2e6d 6f64 756c 655d 0d0a 6e61 6d65  it.module]..name
-000007e0: 203d 2022 6f63 725f 7472 616e 736c 6174   = "ocr_translat
-000007f0: 6522 0d0a 0d0a 5b74 6f6f 6c2e 666c 6974  e"....[tool.flit
-00000800: 2e73 6469 7374 5d0d 0a65 7863 6c75 6465  .sdist]..exclude
-00000810: 203d 205b 0d0a 2020 2020 222e 6769 7469   = [..    ".giti
-00000820: 676e 6f72 6522 2c20 222e 6769 7468 7562  gnore", ".github
-00000830: 222c 0d0a 2020 2020 2269 636f 6e2e 6963  ",..    "icon.ic
-00000840: 6f22 2c20 2272 756e 5f73 6572 7665 722e  o", "run_server.
-00000850: 7079 222c 0d0a 2020 2020 2244 6f63 6b65  py",..    "Docke
-00000860: 7266 696c 6522 2c20 226e 6769 6e78 2e64  rfile", "nginx.d
-00000870: 6566 6175 6c74 222c 2022 7374 6172 742d  efault", "start-
-00000880: 7365 7276 6572 2e73 6822 2c0d 0a20 2020  server.sh",..   
-00000890: 2022 6d79 7369 7465 2f22 2c20 226d 7973   "mysite/", "mys
-000008a0: 6974 652f 2a22 2c20 226d 616e 6167 652e  ite/*", "manage.
-000008b0: 7079 222c 2022 7465 7374 732f 222c 2022  py", "tests/", "
-000008c0: 7465 7374 732f 2a22 2c0d 0a20 2020 205d  tests/*",..    ]
-000008d0: 0d0a 0d0a 5b74 6f6f 6c2e 7079 7465 7374  ....[tool.pytest
-000008e0: 2e69 6e69 5f6f 7074 696f 6e73 5d0d 0a74  .ini_options]..t
-000008f0: 6573 7470 6174 6873 203d 205b 2274 6573  estpaths = ["tes
-00000900: 7473 225d 0d0a 444a 414e 474f 5f53 4554  ts"]..DJANGO_SET
-00000910: 5449 4e47 535f 4d4f 4455 4c45 203d 2022  TINGS_MODULE = "
-00000920: 6d79 7369 7465 2e73 6574 7469 6e67 7322  mysite.settings"
-00000930: 0d0a 6c6f 675f 636c 6920 3d20 310d 0a0d  ..log_cli = 1...
-00000940: 0a5b 746f 6f6c 2e70 796c 696e 742e 6d61  .[tool.pylint.ma
-00000950: 696e 5d0d 0a6c 6f61 642d 706c 7567 696e  in]..load-plugin
-00000960: 7320 3d20 5b0d 0a20 2020 2022 7079 6c69  s = [..    "pyli
-00000970: 6e74 5f64 6a61 6e67 6f22 2c0d 0a20 2020  nt_django",..   
-00000980: 2022 7079 6c69 6e74 5f70 7974 6573 7422   "pylint_pytest"
-00000990: 0d0a 5d0d 0a64 6a61 6e67 6f2d 7365 7474  ..]..django-sett
-000009a0: 696e 6773 2d6d 6f64 756c 6520 3d20 226d  ings-module = "m
-000009b0: 7973 6974 652e 7365 7474 696e 6773 220d  ysite.settings".
-000009c0: 0a0d 0a5b 746f 6f6c 2e70 796c 696e 742e  ...[tool.pylint.
-000009d0: 6d65 7373 6167 6573 5f63 6f6e 7472 6f6c  messages_control
-000009e0: 5d0d 0a64 6973 6162 6c65 203d 205b 0d0a  ]..disable = [..
-000009f0: 2020 2020 226c 6f67 6769 6e67 2d66 7374      "logging-fst
-00000a00: 7269 6e67 2d69 6e74 6572 706f 6c61 7469  ring-interpolati
-00000a10: 6f6e 222c 0d0a 2020 2020 2267 6c6f 6261  on",..    "globa
-00000a20: 6c2d 7374 6174 656d 656e 7422 2c0d 0a20  l-statement",.. 
-00000a30: 2020 2022 6272 6f61 642d 6578 6365 7074     "broad-except
-00000a40: 696f 6e2d 6361 7567 6874 222c 0d0a 2020  ion-caught",..  
-00000a50: 2020 2274 6f6f 2d66 6577 2d70 7562 6c69    "too-few-publi
-00000a60: 632d 6d65 7468 6f64 7322 2c0d 0a5d 0d0a  c-methods",..]..
-00000a70: 0d0a 0d0a 5b74 6f6f 6c2e 7079 6c69 6e74  ....[tool.pylint
-00000a80: 2e66 6f72 6d61 745d 0d0a 6d61 782d 6c69  .format]..max-li
-00000a90: 6e65 2d6c 656e 6774 6820 3d20 3132 300d  ne-length = 120.
-00000aa0: 0a67 6f6f 642d 6e61 6d65 7320 3d20 5b0d  .good-names = [.
-00000ab0: 0a20 2020 2022 5f22 2c0d 0a20 2020 2022  .    "_",..    "
-00000ac0: 6c22 2c20 2272 222c 2022 6222 2c20 2274  l", "r", "b", "t
-00000ad0: 222c 0d0a 2020 2020 226c 3122 2c20 2272  ",..    "l1", "r
-00000ae0: 3122 2c20 2262 3122 2c20 2274 3122 2c0d  1", "b1", "t1",.
-00000af0: 0a20 2020 2022 6c32 222c 2022 7232 222c  .    "l2", "r2",
-00000b00: 2022 6232 222c 2022 7432 222c 0d0a 2020   "b2", "t2",..  
-00000b10: 2020 2269 222c 2022 6a22 2c0d 0a20 2020    "i", "j",..   
-00000b20: 2022 6b22 2c20 2276 222c 0d0a 2020 2020   "k", "v",..    
-00000b30: 2266 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  "f",..]....[tool
-00000b40: 2e70 796c 696e 742e 6465 7369 676e 5d0d  .pylint.design].
-00000b50: 0a6d 6178 2d61 7267 7320 3d20 3130 0d0a  .max-args = 10..
-00000b60: 6d61 782d 6c6f 6361 6c73 203d 2032 300d  max-locals = 20.
-00000b70: 0a6d 6178 2d61 7474 7269 6275 7465 7320  .max-attributes 
-00000b80: 3d20 3132 0d0a                           = 12..
+000007b0: 2020 2020 2266 6c69 7422 2c0d 0a20 2020      "flit",..   
+000007c0: 2022 7079 696e 7374 616c 6c65 7222 0d0a   "pyinstaller"..
+000007d0: 5d0d 0a0d 0a5b 746f 6f6c 2e66 6c69 742e  ]....[tool.flit.
+000007e0: 6d6f 6475 6c65 5d0d 0a6e 616d 6520 3d20  module]..name = 
+000007f0: 226f 6372 5f74 7261 6e73 6c61 7465 220d  "ocr_translate".
+00000800: 0a0d 0a5b 746f 6f6c 2e66 6c69 742e 7364  ...[tool.flit.sd
+00000810: 6973 745d 0d0a 6578 636c 7564 6520 3d20  ist]..exclude = 
+00000820: 5b0d 0a20 2020 2022 2e67 6974 6967 6e6f  [..    ".gitigno
+00000830: 7265 222c 2022 2e67 6974 6875 6222 2c20  re", ".github", 
+00000840: 222e 7072 652d 636f 6d6d 6974 2d63 6f6e  ".pre-commit-con
+00000850: 6669 672e 7961 6d6c 222c 0d0a 2020 2020  fig.yaml",..    
+00000860: 2269 636f 6e2e 6963 6f22 2c20 2272 756e  "icon.ico", "run
+00000870: 5f73 6572 7665 722e 7079 222c 2022 6275  _server.py", "bu
+00000880: 696c 642e 7368 222c 0d0a 2020 2020 2244  ild.sh",..    "D
+00000890: 6f63 6b65 7266 696c 652d 6370 7522 2c20  ockerfile-cpu", 
+000008a0: 2244 6f63 6b65 7266 696c 652d 6770 7522  "Dockerfile-gpu"
+000008b0: 2c20 226e 6769 6e78 2e64 6566 6175 6c74  , "nginx.default
+000008c0: 222c 2022 7374 6172 742d 7365 7276 6572  ", "start-server
+000008d0: 2e73 6822 2c0d 0a20 2020 2022 6d79 7369  .sh",..    "mysi
+000008e0: 7465 2f22 2c20 226d 7973 6974 652f 2a22  te/", "mysite/*"
+000008f0: 2c20 226d 616e 6167 652e 7079 222c 2022  , "manage.py", "
+00000900: 7465 7374 732f 222c 2022 7465 7374 732f  tests/", "tests/
+00000910: 2a22 2c0d 0a20 2020 205d 0d0a 0d0a 5b74  *",..    ]....[t
+00000920: 6f6f 6c2e 7079 7465 7374 2e69 6e69 5f6f  ool.pytest.ini_o
+00000930: 7074 696f 6e73 5d0d 0a74 6573 7470 6174  ptions]..testpat
+00000940: 6873 203d 205b 2274 6573 7473 225d 0d0a  hs = ["tests"]..
+00000950: 444a 414e 474f 5f53 4554 5449 4e47 535f  DJANGO_SETTINGS_
+00000960: 4d4f 4455 4c45 203d 2022 6d79 7369 7465  MODULE = "mysite
+00000970: 2e73 6574 7469 6e67 7322 0d0a 6c6f 675f  .settings"..log_
+00000980: 636c 6920 3d20 310d 0a0d 0a5b 746f 6f6c  cli = 1....[tool
+00000990: 2e70 796c 696e 742e 6d61 696e 5d0d 0a6c  .pylint.main]..l
+000009a0: 6f61 642d 706c 7567 696e 7320 3d20 5b0d  oad-plugins = [.
+000009b0: 0a20 2020 2022 7079 6c69 6e74 5f64 6a61  .    "pylint_dja
+000009c0: 6e67 6f22 2c0d 0a20 2020 2022 7079 6c69  ngo",..    "pyli
+000009d0: 6e74 5f70 7974 6573 7422 0d0a 5d0d 0a64  nt_pytest"..]..d
+000009e0: 6a61 6e67 6f2d 7365 7474 696e 6773 2d6d  jango-settings-m
+000009f0: 6f64 756c 6520 3d20 226d 7973 6974 652e  odule = "mysite.
+00000a00: 7365 7474 696e 6773 220d 0a0d 0a5b 746f  settings"....[to
+00000a10: 6f6c 2e70 796c 696e 742e 6d65 7373 6167  ol.pylint.messag
+00000a20: 6573 5f63 6f6e 7472 6f6c 5d0d 0a64 6973  es_control]..dis
+00000a30: 6162 6c65 203d 205b 0d0a 2020 2020 226c  able = [..    "l
+00000a40: 6f67 6769 6e67 2d66 7374 7269 6e67 2d69  ogging-fstring-i
+00000a50: 6e74 6572 706f 6c61 7469 6f6e 222c 0d0a  nterpolation",..
+00000a60: 2020 2020 2267 6c6f 6261 6c2d 7374 6174      "global-stat
+00000a70: 656d 656e 7422 2c0d 0a20 2020 2022 6272  ement",..    "br
+00000a80: 6f61 642d 6578 6365 7074 696f 6e2d 6361  oad-exception-ca
+00000a90: 7567 6874 222c 0d0a 2020 2020 2274 6f6f  ught",..    "too
+00000aa0: 2d66 6577 2d70 7562 6c69 632d 6d65 7468  -few-public-meth
+00000ab0: 6f64 7322 2c0d 0a5d 0d0a 0d0a 0d0a 5b74  ods",..]......[t
+00000ac0: 6f6f 6c2e 7079 6c69 6e74 2e66 6f72 6d61  ool.pylint.forma
+00000ad0: 745d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  t]..max-line-len
+00000ae0: 6774 6820 3d20 3132 300d 0a67 6f6f 642d  gth = 120..good-
+00000af0: 6e61 6d65 7320 3d20 5b0d 0a20 2020 2022  names = [..    "
+00000b00: 5f22 2c0d 0a20 2020 2022 6c22 2c20 2272  _",..    "l", "r
+00000b10: 222c 2022 6222 2c20 2274 222c 0d0a 2020  ", "b", "t",..  
+00000b20: 2020 226c 3122 2c20 2272 3122 2c20 2262    "l1", "r1", "b
+00000b30: 3122 2c20 2274 3122 2c0d 0a20 2020 2022  1", "t1",..    "
+00000b40: 6c32 222c 2022 7232 222c 2022 6232 222c  l2", "r2", "b2",
+00000b50: 2022 7432 222c 0d0a 2020 2020 2269 222c   "t2",..    "i",
+00000b60: 2022 6a22 2c0d 0a20 2020 2022 6b22 2c20   "j",..    "k", 
+00000b70: 2276 222c 0d0a 2020 2020 2266 222c 0d0a  "v",..    "f",..
+00000b80: 5d0d 0a0d 0a5b 746f 6f6c 2e70 796c 696e  ]....[tool.pylin
+00000b90: 742e 6465 7369 676e 5d0d 0a6d 6178 2d61  t.design]..max-a
+00000ba0: 7267 7320 3d20 3130 0d0a 6d61 782d 6c6f  rgs = 10..max-lo
+00000bb0: 6361 6c73 203d 2032 300d 0a6d 6178 2d61  cals = 20..max-a
+00000bc0: 7474 7269 6275 7465 7320 3d20 3132 0d0a  ttributes = 12..
```

### Comparing `django_ocr_translate-0.1.3/PKG-INFO` & `django_ocr_translate-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ocr_translate
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django app for OCR and translation
 Keywords: django,ocr,translation
 Author: Davide Grassano
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
@@ -35,14 +35,15 @@
 Requires-Dist: sentencepiece~=0.1.99
 Requires-Dist: pymysql==1.1.0 ; extra == "mysql"
 Requires-Dist: psycopg[binary]==3.1.9 ; extra == "postgres"
 Requires-Dist: pre-commit~=3.3.3 ; extra == "pre-commit"
 Requires-Dist: pylint~=2.17.4 ; extra == "pre-commit"
 Requires-Dist: pylint-pytest~=1.1.2 ; extra == "pre-commit"
 Requires-Dist: pylint-django~=2.5.3 ; extra == "pre-commit"
+Requires-Dist: flit ; extra == "release"
 Requires-Dist: pyinstaller ; extra == "release"
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
 Requires-Dist: pytest-regressions~=2.4 ; extra == "tests"
 Requires-Dist: pytest-django~=4.5.2 ; extra == "tests"
 Project-URL: Source, https://github.com/crivella/ocr_translate
 Provides-Extra: mysql
@@ -55,79 +56,46 @@
 
 This is a Django app for creating back-end server aimed at performing OCR and translation of images received via a POST request.
 
 The OCR and translation is performed using freely available machine learning models and packages (see below for what is currently implemented).
 
 The server is designed to be used together with [this browser extension](https://github.com/Crivella/ocr_extension), acting as a front-end providing the images and controlling the model languages and models being used.
 
-## Installation
-
-It is strongly suggested to install this project using a [virtual environment](https://docs.python.org/3/library/venv.html).
-
-### From Github
-
-- Clone or download the repository
-  - `git clone https://github.com/Crivella/ocr_translate.git`
-- Install the project dependencies (choose the appropriate files depending if you wanna run on GPU or CPU only):
-  - `pip install -r requirements-torch-[cpu/cuda].txt`
-  - `pip install -r requirements.txt`
-
-### From Docker
-Plan to add a CPU and a CUDA specific image to DockerHUB.
-For now you can create the image yourself by:
-
-- Create a .pip-cache-cpu directory inside your project.
-- Optional: re-install the project dependencies pointing this as the cache folder for pip (will make the build process much faster, by reusing the cached dependencies)
-- Run `docker build -t ocr_server .`
-
-
-### From PyPI
-
-Run the command
-
-- `pip install django-ocr_translate`
-
-By default torch 2.x will come in its CUDA enabled version. While this works also for CPU, it will also install ~1 GB of cuda dependencies.
-If you wish to run on CPU only, download the file [requirements-torch-cpu.txt](requirements-torch-cpu.txt) first and run
-
-- `pip install -r requirements-torch-cpu.txt`
-
-before installing the python package.
-
 ## Running the server
 
-By default the server will use a sqlite database named *db.sqlite3* inside the project main directory.
-If you plan to use a different database, you can either:
+If you plan to use a different settings (eg. database, or model location), you can either:
 
 - manually edit the [settings.py](mysite/settings.py)
 - Use the provided [Environment variables](#environment-variables)
 See below for a [list of supported databases](#supported-databases)
 
 You will also have to modify the `ALLOWED_HOSTS` in case you plan to access the server from somewhere other than *localhost*.
 
+All the different way to run the server may provide different set of default values (each of them is targeted for a different level of usage).
+
 ### From Release file
 
 (Tested on Windows 11)
-From the github releases you can download either:
-
-- The [CPU only version](/releases/latest/download/run_server-cpu.exe)
-- The GPU version split in [file 1](/releases/latest/download/run_server-gpu.zip.001) and [file 2](/releases/latest/download/run_server-gpu.zip.002) (The CUDA dependencies makes it take much more space), wich can be restored using tools like [7zip](https://www.7-zip.org/https://www.7-zip.org/) and [NanaZip](https://github.com/M2Team/NanaZip).
+From the [github releases page](/releases/) you can download either:
 
-Not that every time you run the EXE, it will decompress itself into a temporary folder so:
+- The [CPU only version](/../../releases/latest/download/run_server-cpu.exe)
+- The GPU version split in [file 1](/../../releases/latest/download/run_server-gpu.zip.001) and [file 2](/../../releases/latest/download/run_server-gpu.zip.002) (The CUDA dependencies makes it take much more space), wich can be restored using tools like [7zip](https://www.7-zip.org/https://www.7-zip.org/) and [NanaZip](https://github.com/M2Team/NanaZip).
 
-- The exe will appear as an empty console until all the file are extracted and the actual script start running.
-- By launching the server multiple times without restarting (especially the GPU one), you risk quickly filling up your drive
+Usage:
+Unzip the file and from inside the folder, run the `run_server-XXX.exe` file (XXX=cpu/gpu)
 
-You can either just start the server and it will run with sensible defaults. Most notably the models files and database will be downloaded/created under `%userprofile%/.ocr_translate`.
+The server will run with sensible defaults. Most notably the models files and database will be downloaded/created under `%userprofile%/.ocr_translate`.
 Also the gpu version will attempt to run on GPU by default, and fall-back to CPU if the former is not available.
 
-For customization, you can set the [environment variable](#environment-variables) yourself, either via powershell or by searching for *environment variable* in the settings menu
+For customization, you can set the [environment variable](#environment-variables) yourself, either via powershell or by searching for *environment variable* in the settings menu.
 
 ### From Github installation
 
+See the section on how to [install from Github](#from-github) first.
+
 The Github repo provides not only the Django app files, but also the already configured project files used to start the server.
 
 Create/Initialize your database by running
 
 - `python manage.py migrate`
 
 inside your project folder.
@@ -145,43 +113,85 @@
 Notes:
 
 - Gunicorn workers will each spawn a separate instance of the loaded models, each taking its own space in the memory. This can quickly fill up the memory especially if running on GPU. Ideally set this to 1.
 - Django development server will spawn new threads for handling incoming requests (if no currently existing thread is free), which share the same memory. Running more than one worker per loaded model concurrently might slow down the actual computation and in some case also block the execution.
 
 ### From PyPI installation
 
+See the section on how to [install from PyPI](#from-pypi) first.
+
 When installing the project from PyPI, only the app is available.
 This will need to be integrated in a Django project in order to be used.
 These are the minimal instruction for creating a project and start running the server:
 
 - Run `django-admin startproject mysite` to create a django project
 - Configure the server by replacing the automatically created files (strongly recommended):
   - [settings.py](mysite/settings.py) with the one available on the repo.
   - [urls.py](mysite/urls.py) with the one available on the repo.
 - or by manually editing the files:
   - settings.py: Add the `ocr_translated` app to the `INSTALLED_APPS`
   - urls.py: Include the `'ocr_translate.urls'` into your project urls.
 - From here follow the same instructions as when starting [from Github](#from-github)
 
-### From docker
+### From docker image
+
+See the section on how to [install from DockerHUB](#from-docker) first.
 
 This section assumes you have docker installed and the image of the project.
 
 Run the command:
 
-- `docker run --name CONTAINER_NAME -v PATH_TO_YOUR_MODEL_DIRECTORY:/models -v PATH_TO_DIR_WITH_SQLITE_FILE:/data --env-file=PATH_TO_AND_ENV_VARIABLE_FILE -p SERVER_PORT:4000 -d ocr_server`
+- `docker run --name CONTAINER_NAME -v PATH_TO_YOUR_MODEL_DIRECTORY:/models -v PATH_TO_DIR_WITH_SQLITE_FILE:/data --env-file=PATH_TO_AND_ENV_VARIABLE_FILE -p SERVER_PORT:4000 -d ocr_translate`
 
-See the [Environment variables](#environment-variables) section for configuring your environment variable file. Additionaly the docker image defines 2 other variable to automatically create an admin user for managing the database via the django-admin interface:
+See the [Environment variables](#environment-variables) section for configuring your environment variable file. Additionaly the docker image defines several other variables to automatically create an admin user for managing the database via the django-admin interface:
 
 - `UID`: UID of the user owning the files in /models and /data
 - `GID`: GID of the user owning the files in /models and /data
 - `NUM_WEB_WORKERS`: Number of gunicorn workers for the server
 - `DJANGO_SUPERUSER_USERNAME`: The username of the admin user to be created.
 - `DJANGO_SUPERUSER_PASSWORD`: The password of the admin user to be created.
 
+
+## Installation
+
+For both the Githyb and PyPI installation it is strongly suggested to install this project using a [virtual environment](https://docs.python.org/3/library/venv.html).
+
+### From Github
+
+- Clone or download the repository
+  - `git clone https://github.com/Crivella/ocr_translate.git`
+- Install the project dependencies (choose the appropriate files depending if you wanna run on GPU or CPU only):
+  - `pip install -r requirements-torch-[cpu/cuda].txt`
+  - `pip install -r requirements.txt`
+
+### From Docker
+
+CPU and CUDA specific images are available on [DockerHUB](https://hub.docker.com/r/crivella1/ocr_translate):
+
+- CPU: `docker pull crivella1/ocr_translate:latest-cpu`
+- GPU: `docker pull crivella1/ocr_translate:latest-gpu`
+
+Manually create your image:
+
+- Create a .pip-cache-[cpu/gpu] directory inside your project.
+- Optional: re-install the project dependencies pointing this as the cache folder for pip (will make the build process much faster, by reusing the cached dependencies)
+- Run `docker build -t IMAGE_TAG -f Dockerfile-[cpu/gpu] .`
+
+### From PyPI
+
+Run the command
+
+- `pip install django-ocr_translate`
+
+By default torch 2.x will come in its CUDA enabled version. While this works also for CPU, it will also install ~1 GB of cuda dependencies.
+If you wish to run on CPU only, download the file [requirements-torch-cpu.txt](requirements-torch-cpu.txt) first and run
+
+- `pip install -r requirements-torch-cpu.txt`
+
+before installing the python package.
 ## Supported Box OCR models
 
 - [EasyOCR](https://github.com/JaidedAI/EasyOCR)
 
 ## Supported text OCR models
 
 - Hugging Face [Transformers](https://huggingface.co/docs/transformers/index) VisionEncoderDecoder models
```

