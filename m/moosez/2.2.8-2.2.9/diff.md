# Comparing `tmp/moosez-2.2.8.tar.gz` & `tmp/moosez-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.2.8.tar", last modified: Tue Jul 25 12:39:12 2023, max compression
+gzip compressed data, was "moosez-2.2.9.tar", last modified: Tue Jul 25 18:06:32 2023, max compression
```

## Comparing `moosez-2.2.8.tar` & `moosez-2.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:39:12.026388 moosez-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:38:54.000000 moosez-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:39:12.026388 moosez-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-25 12:38:54.000000 moosez-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:39:12.022388 moosez-2.2.8/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:39:12.022388 moosez-2.2.8/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:39:12.026388 moosez-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 12:38:54.000000 moosez-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:06:32.991168 moosez-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 18:06:16.000000 moosez-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 18:06:32.991168 moosez-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-07-25 18:06:16.000000 moosez-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:06:32.991168 moosez-2.2.9/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-25 18:06:16.000000 moosez-2.2.9/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:06:32.991168 moosez-2.2.9/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 18:06:32.000000 moosez-2.2.9/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 18:06:32.000000 moosez-2.2.9/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:06:32.000000 moosez-2.2.9/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 18:06:32.000000 moosez-2.2.9/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-25 18:06:32.000000 moosez-2.2.9/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 18:06:32.000000 moosez-2.2.9/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:06:32.991168 moosez-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-25 18:06:16.000000 moosez-2.2.9/setup.py
```

### Comparing `moosez-2.2.8/LICENSE` & `moosez-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.2.8/PKG-INFO` & `moosez-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.8
+Version: 2.2.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.8/README.md` & `moosez-2.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 ```
 
 Here `<path_to_image_dir>` refers to the directory containing your subject images and `<model_name>` is the name of the segmentation model you intend to utilize. 
 
 For instance, to perform clinical CT organ segmentation, the command would be:
 
 ```bash
-moosez -d <path_to_image_dir> -m clin_ct_organs_v2 
+moosez -d <path_to_image_dir> -m clin_ct_organs
 ```
 
 In this example, 'clin_ct_organs' is the segmentation model name for clinical CT organ segmentation.
 
 And that's it! With just one command, you're all set to explore the new horizons of 3D medical image segmentation with MOOSE 2.0.
 
 Need assistance along the way? Don't worry, we've got you covered. Simply type:
@@ -129,15 +129,15 @@
 2. `input_dir`: The directory containing the images (in nifti, either .nii or .nii.gz) to process.
 3. `output_dir`: The directory where the output will be saved.
 4. `accelerator`: The type of accelerator to use (e.g., "cpu", "cuda").
 
 Here's an example of how to call the `moose` function:
 
  ```python
- model_name = 'clin_ct_organs_v2'
+ model_name = 'clin_ct_organs'
  input_dir = '/home/Documents/your_project/data/input'
  output_dir = '/home/Documents/your_project/data/output'
  accelerator = 'cuda'
  moose(model_name, input_dir, output_dir, accelerator)
  ```
 
 Remember to replace `model_name`, `input_dir`, `output_dir`, and `accelerator` with the actual values you want to use.
@@ -184,50 +184,50 @@
 ### Naming Conventions for NIFTI files 📝
 When using NIFTI files, you should name the file with the appropriate modality as a suffix. 
 
 For instance, if you have chosen the `model_name` as `clin_ct_organs`, the CT scan for subject 'S2' in NIFTI format, should have the modality tag 'CT_' attached to the file name, e.g. `CT_S2.nii`. In the directory shown above, every subject will be processed by `moosez` except S4.
 
 **Remember:** Adhering to these file naming and directory structure conventions ensures smooth and efficient processing with MOOSE 2.0. Happy segmenting! 🚀
 
-## :tada: Add and contribute Your Own nnUNetv1 as well as nnUNetv2 Models to MooseZ :rocket:
+## :tada: Add and contribute Your Own nnUNetv2 Models to MooseZ :rocket:
 
-Want to power-up your medical image segmentation tasks? :zap: Join the MooseZ community and contribute your own `nnUNetv2` models! 🥇
+Want to power-up your medical image segmentation tasks? :zap: Join the MooseZ community and contribute your own `nnUNetv2` models! 🥇:
 
-By adding your custom nnunet (both v1 and v2) models to MooseZ, you can enjoy:
+By adding your custom models to MooseZ, you can enjoy:
 
 - :fast_forward: **Increased Speed** - MooseZ is optimized for fast performance. Use it to get your results faster!
 - :floppy_disk: **Reduced Memory** - MooseZ is designed to be efficient and lean, so it uses less memory!
 
 So why wait? Make your models fly with MooseZ :airplane:
 
 ## How to Contribute Your Model :hammer_and_wrench:
 
 1. **Prepare Your Model** :file_folder:
 
-    Train your model either using `nnUNetv1`/`nnUNetv2` and get it ready for the big leagues!
+    Train your model using `nnUNetv2` and get it ready for the big leagues!
 
 2. **Update AVAILABLE_MODELS List** :pencil2:
 
-    Include your model's unique identifier to the `AVAILABLE_MODELS` list in the [resources.py](https://github.com/LalithShiyam/MOOSE/blob/d131a7c88b3d0defd43339c7d788f092a242f59d/moosez/resources.py#L29) file. The model name should follow a specific syntax: 'clin' or 'preclin' (indicating Clinical or Preclinical), modality tag (like 'ct', 'pt', 'mr'), the tissue of interest (e.g. brain, liver) and finally the version of nnunet you used to train (`v1` or `v2`). You theoretically don't need to stick to it, we just like it this way 😁!
+    Include your model's unique identifier to the `AVAILABLE_MODELS` list in the [resources.py](https://github.com/LalithShiyam/MOOSE/blob/d131a7c88b3d0defd43339c7d788f092a242f59d/moosez/resources.py#L29) file. The model name should follow a specific syntax: 'clin' or 'preclin' (indicating Clinical or Preclinical), modality tag (like 'ct', 'pt', 'mr'), and then the tissue of interest.
 
 3. **Update MODELS Dictionary** :clipboard:
 
     Add a new entry to the `MODELS` dictionary in the [resources.py](https://github.com/LalithShiyam/MOOSE/blob/d131a7c88b3d0defd43339c7d788f092a242f59d/moosez/resources.py#L49) file. Fill in the corresponding details (like URL, filename, directory, trainer type, voxel spacing, and multilabel prefix). 
 
 4. **Update expected_modality Function** :memo:
 
     Update the `expected_modality` function in the [resources.py](https://github.com/LalithShiyam/MOOSE/blob/d131a7c88b3d0defd43339c7d788f092a242f59d/moosez/resources.py#L100) file to return the imaging technique, modality, and tissue of interest for your model.
 
 5. **Update map_model_name_to_task_number Function** :world_map:
 
     Modify the `map_model_name_to_task_number` function in the [resources.py](https://github.com/LalithShiyam/MOOSE/blob/d131a7c88b3d0defd43339c7d788f092a242f59d/moosez/resources.py#L130) file to return the task number associated with your model.
 
-6. **Update ORGAN_INDICES dictionary** 🧠
+6. **Update `ORGAN_INDICES` in `constants.py`** 🧠
 
-   Append the `ORGAN_INDICES` dictionary in the [constants.py](https://github.com/LalithShiyam/MOOSE/blob/96c332860d8030c5c2d80d51ab4c57707b90e887/moosez/constants.py#L66) by including the intensity to region information  for your particular model. This is particularly useful if you want to extract stats from PET images using your CT masks.
+   Append the `ORGAN_INDICES` dictionary in the [constants.py](https://github.com/LalithShiyam/MOOSE/blob/3f5f9537365a41478060c96815c38c3824353bb9/moosez/constants.py#L66C1-L66C14) with your label intensity to region mapping. This is particularly important if you would like to have your stats from the PET images based on your CT masks.
 
 That's it! You've successfully contributed your own model to the MooseZ community! :confetti_ball:
 
 With your contribution 🙋, MooseZ becomes a stronger and more robust tool for medical image segmentation! :muscle:
 
 
 ## A Note on QIMP Python Packages: The 'Z' Factor 📚🚀
```

### Comparing `moosez-2.2.8/moosez/constants.py` & `moosez-2.2.9/moosez/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 import os
 
 from moosez import file_utilities
 
 project_root = file_utilities.get_virtual_env_root()
 
-NNUNETV2_MODEL_FOLDER = os.path.join(project_root, 'models', 'nnunet_trained_models')
-NNUNETV1_MODEL_FOLDER = os.path.join(NNUNETV2_MODEL_FOLDER, 'nnUNet', '3d_fullres')
+NNUNET_RESULTS_FOLDER = os.path.join(project_root, 'models', 'nnunet_trained_models')
+MOOSEZ_MODEL_FOLDER = os.path.join(NNUNET_RESULTS_FOLDER, 'nnUNet', '3d_fullres')
 ALLOWED_MODALITIES = ['CT', 'PT', 'MR']
 TEMP_FOLDER = 'temp'
 
 # COLOR CODES
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[38;5;40m'
 ANSI_VIOLET = '\033[38;5;141m'
@@ -60,15 +60,15 @@
 RESAMPLED_MASK_FILE_NAME = 'resampled_mask.nii.gz'
 CHUNK_FILENAMES = ["chunk01_0000.nii.gz", "chunk02_0000.nii.gz", "chunk03_0000.nii.gz"]
 CHUNK_PREFIX = 'chunk'
 
 # ORGAN INDICES
 
 ORGAN_INDICES = {
-    "clin_ct_organs_v2": {
+    "clin_ct_organs": {
         1: "spleen",
         2: "kidney_right",
         3: "kidney_left",
         4: "gallbladder",
         5: "liver",
         6: "stomach",
         7: "aorta",
@@ -79,66 +79,24 @@
         12: "adrenal_gland_left",
         13: "lung_upper_lobe_left",
         14: "lung_lower_lobe_left",
         15: "lung_upper_lobe_right",
         16: "lung_middle_lobe_right",
         17: "lung_lower_lobe_right"
     },
-    "clin_ct_lungs_v2": {
+    "clin_ct_lungs": {
         1: "lung_upper_lobe_left",
         2: "lung_lower_lobe_left",
         3: "lung_upper_lobe_right",
         4: "lung_middle_lobe_right",
         5: "lung_lower_lobe_right"
     },
-    "clin_ct_body_v2": {
+    "clin_ct_body": {
         1: "whole-body"
     },
-    "clin_pt_fdg_tumor_v2": {
+    "clin_pt_fdg_tumor": {
         1: "tumor"
-    },
-    "clin_ct_organs_v1": {
-        1: 'Adrenal-glands',
-        2: 'Aorta',
-        3: 'Bladder',
-        4: 'Brain',
-        5: 'Heart',
-        6: 'Kidneys',
-        7: 'Liver',
-        8: 'Pancreas',
-        9: 'Spleen',
-        10: 'Thyroid',
-        11: 'Inferior-vena-cava',
-        12: 'Skeleton',
-        13: 'Lung'
-    },
-    "clin_ct_bones_v1": {
-        1: 'Carpal',
-        2: 'Clavicle',
-        3: 'Femur',
-        4: 'Fibula',
-        5: 'Humerus',
-        6: 'Metacarpal',
-        7: 'Metatarsal',
-        8: 'Patella',
-        9: 'Pelvis',
-        10: 'Phalanges-of-the-hand',
-        11: 'Radius',
-        12: 'Ribcage',
-        13: 'Scapula',
-        14: 'Skull',
-        15: 'Spine',
-        16: 'Sternum',
-        17: 'Tarsal',
-        18: 'Tibia',
-        19: 'Phalanges-of-the-feet',
-        20: 'Ulna'
-    },
-    "clin_ct_fat_muscles_v1": {
-        1: 'Skeletal-muscle',
-        2: 'Subcutaneous-fat',
-        3: 'Torso-fat'
-    },
+    }
     # More index-to-name dictionaries for other models...
 }
```

### Comparing `moosez-2.2.8/moosez/display.py` & `moosez-2.2.9/moosez/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,16 +68,15 @@
     else:
         modalities = [modality]
     expected_prefix = [m.replace('-', '_') + "_" for m in modalities]
 
     print(
         f" Imaging: {model_info['Imaging']} |"
         f" Modality: {modality} | "
-        f"Tissue of interest: {model_info['Tissue of interest']} | "
-        f"nnUNet version: {model_info['nnUNet version']} ")
+        f"Tissue of interest: {model_info['Tissue of interest']}")
     print(
         f" Required modalities: {modalities} | "
         f" No. of modalities: {len(modalities)}"
         f" | Required prefix for non-DICOM files: {expected_prefix}")
     logging.info(f" Required modalities: {modalities} |  No. of modalities: {len(modalities)} "
                  f"| Required prefix for non-DICOM files: {expected_prefix} ")
     print(
```

### Comparing `moosez-2.2.8/moosez/download.py` & `moosez-2.2.9/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.8/moosez/file_utilities.py` & `moosez-2.2.9/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.8/moosez/image_conversion.py` & `moosez-2.2.9/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.8/moosez/image_processing.py` & `moosez-2.2.9/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.8/moosez/input_validation.py` & `moosez-2.2.9/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.8/moosez/moosez.py` & `moosez-2.2.9/moosez/moosez.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,21 +84,15 @@
     # ----------------------------------
     # DOWNLOADING THE MODEL
     # ----------------------------------
 
     print('')
     print(f'{constants.ANSI_VIOLET} {emoji.emojize(":globe_with_meridians:")} MODEL DOWNLOAD:{constants.ANSI_RESET}')
     print('')
-    nnunet_version = MODELS[model_name]["nnunet_version"]
-    # if nnunet_version is v1, the model path = NNUNETV1_MODEL_FOLDER
-    # if nnunet_version is v2, the model_path = nnunet_results_folder
-    if nnunet_version == "v1":
-        model_path = constants.NNUNETV1_MODEL_FOLDER
-    elif nnunet_version == "v2":
-        model_path = constants.NNUNETV2_MODEL_FOLDER
+    model_path = constants.NNUNET_RESULTS_FOLDER
     file_utilities.create_directory(model_path)
     download.model(model_name, model_path)
 
     # ----------------------------------
     # INPUT STANDARDIZATION
     # ----------------------------------
 
@@ -200,15 +194,15 @@
 
     spinner.succeed(f'{constants.ANSI_GREEN} All predictions done! | Total elapsed time for '
                     f'{len(moose_compliant_subjects)} datasets: {round(total_elapsed_time, 1)} min'
                     f' | Time per dataset: {round(time_per_dataset, 2)} min {constants.ANSI_RESET}')
 
 
 def moose(model_name: str, input_dir: str, output_dir: str, accelerator: str):
-    model_path = constants.NNUNETV2_MODEL_FOLDER
+    model_path = constants.NNUNET_RESULTS_FOLDER
     file_utilities.create_directory(model_path)
     download.model(model_name, model_path)
     input_validation.make_nnunet_compatible(input_dir)
     spinner = Halo(text=f'{constants.ANSI_VIOLET} Running prediction...{constants.ANSI_RESET}',
                    spinner='dots')
     spinner.start()
     predict.predict(model_name, input_dir, output_dir, accelerator)
```

### Comparing `moosez-2.2.8/moosez/predict.py` & `moosez-2.2.9/moosez/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,41 +39,29 @@
     Runs the prediction using nnunet_predict.
     :param model_name: The name of the model.
     :param input_dir: The input directory.
     :param output_dir: The output directory.
     :param accelerator: The accelerator to use.
     :return: None
     """
-    # get nnunet version number
-    nnunet_version = MODELS[model_name]["nnunet_version"]
     task_number = map_model_name_to_task_number(model_name)
+    # set the environment variables
+    os.environ["nnUNet_results"] = constants.NNUNET_RESULTS_FOLDER
 
     # Preprocess the image
     temp_input_dir, resampled_image, moose_image_object = preprocess(input_dir, model_name)
     resampled_image_shape = resampled_image.shape
     resampled_image_affine = resampled_image.affine
 
-    command = []
+    # choose the appropriate trainer for the model
+    trainer = MODELS[model_name]["trainer"]
 
-    # set the parameters for nnunet_predict based on the nnunet version
-    if nnunet_version == "v1":
-        os.environ["RESULTS_FOLDER"] = constants.NNUNETV2_MODEL_FOLDER
-        # choose the appropriate model_type for the task
-        model_type = MODELS[model_name]["model_type"]
-        folds = MODELS[model_name]["fold"]
-        # Construct the command
-        command = f'nnUNet_predict -i {temp_input_dir} -o {output_dir} -t {task_number} -m {model_type} --fold {folds}' \
-                  f' --disable_tta'
-    elif nnunet_version == "v2":
-        os.environ["nnUNet_results"] = constants.NNUNETV2_MODEL_FOLDER
-        #  choose the appropriate trainer for the model
-        trainer = MODELS[model_name]["trainer"]
-        # Construct the command
-        command = f'nnUNetv2_predict -i {temp_input_dir} -o {output_dir} -d {task_number} -c 3d_fullres' \
-                  f' -f all -tr {trainer} --disable_tta -device {accelerator}'
+    # Construct the command
+    command = f'nnUNetv2_predict -i {temp_input_dir} -o {output_dir} -d {task_number} -c 3d_fullres' \
+              f' -f all -tr {trainer} --disable_tta -device {accelerator}'
 
     # Run the command
     subprocess.run(command, shell=True, stdout=subprocess.DEVNULL, env=os.environ)
 
     original_image_files = file_utilities.get_files(input_dir, '.nii.gz')
 
     # Postprocess the label
```

### Comparing `moosez-2.2.8/moosez/resources.py` & `moosez-2.2.9/moosez/resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,22 +22,19 @@
 
 # This list contains the unique identifiers for all available pre-trained models.
 # To make your model available, add its unique identifier to this list.
 # The model name or the unique identifier has a specific syntax:
 # 'clin' or 'preclin' (indicating Clinical or Preclinical),
 # modality tag (like 'ct', 'pt', 'mr'), and then the tissue of interest.
 
-AVAILABLE_MODELS = ["clin_ct_lungs_v2",
-                    "clin_ct_organs_v2",
-                    "clin_pt_fdg_tumor_v2",
-                    "clin_ct_body_v2",
-                    "preclin_mr_all_v2",
-                    "clin_ct_organs_v1",
-                    "clin_ct_bones_v1",
-                    "clin_ct_fat_muscles_v1"]
+AVAILABLE_MODELS = ["clin_ct_lungs",
+                    "clin_ct_organs",
+                    "clin_pt_fdg_tumor",
+                    "clin_ct_body",
+                    "preclin_mr_all"]
 
 # This dictionary holds the pre-trained models available in MooseZ library.
 # Each key is a unique model identifier following a specific syntax mentioned above
 # It should have the same name mentioned in AVAILABLE_MODELS list.
 # Each value is a dictionary containing the following keys:
 #    - url: The URL where the model files can be downloaded.
 #    - filename: The filename of the model's zip file.
@@ -46,103 +43,54 @@
 #    - voxel_spacing: The voxel spacing used in the model in the form [x, y, z], this is basically the median voxel
 #    spacing generated by nnunetv2, and you can find this in the plans.json file of the model.
 #    - multilabel_prefix: A prefix to distinguish between different types of labels in multi-label models.
 #
 # To include your own model, add a new entry to this dictionary following the above format.
 
 MODELS = {
-    "clin_ct_lungs_v2": {
-        "nnunet_version": "v2",
+    "clin_ct_lungs": {
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/clin_ct_lungs_24062023.zip",
         "filename": "Dataset333_HMS3dlungs.zip",
         "directory": "Dataset333_HMS3dlungs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Lungs_",
-        "model_type": None,
-        "fold": None,
+        "multilabel_prefix": "CT_Lungs_"
     },
-    "clin_ct_organs_v2": {
-        "nnunet_version": "v2",
+    "clin_ct_organs": {
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/MOOSEv2_bspline_organs23062023.zip",
         "filename": "Dataset123_Organs.zip",
         "directory": "Dataset123_Organs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Organs_",
-        "model_type": None,
-        "fold": None,
+        "multilabel_prefix": "CT_Organs_"
     },
-    "clin_pt_fdg_tumor_v2": {
-        "nnunet_version": "v2",
+    "clin_pt_fdg_tumor": {
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Dataset789_Tumors.zip",
         "filename": "Dataset789_Tumors.zip",
         "directory": "Dataset789_Tumors",
         "trainer": "nnUNetTrainerDA5",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "PT_FDG_Tumor_",
-        "model_type": None,
-        "fold": None,
+        "multilabel_prefix": "PT_FDG_Tumor_"
     },
-    "preclin_mr_all_v2": {
-        "nnunet_version": "v2",
+    "preclin_mr_all": {
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/preclin_mr_14062023.zip",
         "filename": "Dataset234_Preclin.zip",
         "directory": "Dataset234_Preclin",
         "trainer": "nnUNetTrainerNoMirroring",
         "voxel_spacing": [0.15, 0.15, 0.15],
-        "multilabel_prefix": "Preclin_MR_all_",
-        "model_type": None,
-        "fold": None,
+        "multilabel_prefix": "Preclin_MR_all_"
     },
-    "clin_ct_body_v2": {
-        "nnunet_version": "v2",
+    "clin_ct_body": {
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Dataset696_BodyContour.zip",
         "filename": "Dataset696_BodyContour.zip",
         "directory": "Dataset696_BodyContour",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [1.5, 1.5, 1.5],
-        "multilabel_prefix": "CT_Body_",
-        "model_type": None,
-        "fold": None,
+        "multilabel_prefix": "CT_Body_"
     },
-    "clin_ct_organs_v1": {
-        "nnunet_version": "v1",
-        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Task123_StOrgans40.zip",
-        "filename": "Task123_StOrgans40.zip",
-        "directory": "Task123_StOrgans40",
-        "trainer": None,
-        "voxel_spacing": [0.9765625, 0.9765625, 2.3440001],
-        "multilabel_prefix": "CT_Organs_V1_",
-        "model_type": "3d_fullres",
-        "fold": "all",
-    },
-    "clin_ct_bones_v1": {
-        "nnunet_version": "v1",
-        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Task517_Bones40.zip",
-        "filename": "Task517_Bones40.zip",
-        "directory": "Task517_Bones40",
-        "trainer": None,
-        "voxel_spacing": [0.9765625, 0.9765625, 2.3440001],
-        "multilabel_prefix": "CT_Bones_V1_",
-        "model_type": "3d_fullres",
-        "fold": "all",
-    },
-    "clin_ct_fat_muscles_v1": {
-        "nnunet_version": "v1",
-        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Task517_Bones40.zip",
-        "filename": "Task427_FM40.zip",
-        "directory": "Task427_FM40",
-        "trainer": None,
-        "voxel_spacing": [0.9765625, 0.9765625, 2.3440001],
-        "multilabel_prefix": "CT_Fat_Muscles_V1_",
-        "model_type": "3d_fullres",
-        "fold": "all",
-    },
-
 }
 
 
 # This function returns a dictionary indicating the expected modality for a given model_name, the imaging technique,
 # the type of tissue to be segmented. The model_name should be the same as the unique identifier mentioned in the
 # MODELS dictionary above and the AVAILABLE_MODELS list.
 # If the model_name is not found, it logs an error message and returns an error message.
@@ -152,30 +100,19 @@
 def expected_modality(model_name: str) -> dict:
     """
     Display expected modality for the model.
     :param model_name: The name of the model.
     :return: The expected modality for the model.
     """
     models = {
-        "clin_ct_lungs_v2": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Lungs",
-                          "nnUNet version": "v2"},
-        "clin_ct_organs_v2": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Organs",
-                           "nnUNet version": "v2"},
-        "clin_pt_fdg_tumor_v2": {"Imaging": "Clinical", "Modality": "PET", "Tissue of interest": "Tumor",
-                              "nnUNet version": "v2"},
-        "clin_ct_body_v2": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Body",
-                         "nnUNet version": "v2"},
-        "preclin_mr_all_v2": {"Imaging": "Pre-clinical", "Modality": "MR", "Tissue of interest": "All regions",
-                           "nnUNet version": "v2"},
-        "clin_ct_organs_v1": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Organs",
-                              "nnUNet version": "v1"},
-        "clin_ct_bones_v1": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Bones",
-                             "nnUNet version": "v1"},
-        "clin_ct_fat_muscles_v1": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Fat and Muscles",
-                                   "nnUNet version": "v1"},
+        "clin_ct_lungs": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Lungs"},
+        "clin_ct_organs": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Organs"},
+        "clin_pt_fdg_tumor": {"Imaging": "Clinical", "Modality": "PET", "Tissue of interest": "Tumor"},
+        "clin_ct_body": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Body"},
+        "preclin_mr_all": {"Imaging": "Pre-clinical", "Modality": "MR", "Tissue of interest": "All regions"},
     }
 
     if model_name in models:
         model = models[model_name]
         model["Model name"] = model_name
         return model
 
@@ -192,30 +129,24 @@
 
 def map_model_name_to_task_number(model_name: str):
     """
     Maps the model name to the task number.
     :param model_name: The name of the model.
     :return: The task number.
     """
-    if model_name == "clin_ct_lungs_v2":
+    if model_name == "clin_ct_lungs":
         return 333
-    elif model_name == "clin_ct_organs_v2":
+    elif model_name == "clin_ct_organs":
         return 123
-    elif model_name == "clin_pt_fdg_tumor_v2":
+    elif model_name == "clin_pt_fdg_tumor":
         return 789
-    elif model_name == "preclin_mr_all_v2":
+    elif model_name == "preclin_mr_all":
         return 234
-    elif model_name == "clin_ct_body_v2":
+    elif model_name == "clin_ct_body":
         return 696
-    elif model_name == "clin_ct_organs_v1":
-        return 123
-    elif model_name == "clin_ct_bones_v1":
-        return 517
-    elif model_name == "clin_ct_fat_muscles_v1":
-        return 427
     else:
         raise Exception(f"Error: The model name '{model_name}' is not valid.")
 
 
 def check_cuda() -> str:
     """
     This function checks if CUDA is available on the device and prints the device name and number of CUDA devices
```

### Comparing `moosez-2.2.8/moosez.egg-info/PKG-INFO` & `moosez-2.2.9/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.8
+Version: 2.2.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.8/setup.py` & `moosez-2.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.2.8',
+    version='2.2.9',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
@@ -27,15 +27,14 @@
 
     keywords='moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation'
              ' lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation'
              ' vertebral-segmentation rib-segmentation'
              ' preclinical-segmentation clinical-segmentation',
     packages=find_packages(),
     install_requires=[
-        'nnunet',
         'nnunetv2',
         'nibabel~=3.2.2',
         'halo~=0.0.31',
         'pandas~=1.4.1',
         'SimpleITK~=2.2.1',
         'pydicom~=2.2.2',
         'argparse~=1.4.0',
```

