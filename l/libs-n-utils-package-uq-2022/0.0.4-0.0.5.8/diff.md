# Comparing `tmp/libs_n_utils_package_uq_2022-0.0.4.tar.gz` & `tmp/libs_n_utils_package_uq_2022-0.0.5.8.tar.gz`

## Comparing `libs_n_utils_package_uq_2022-0.0.4.tar` & `libs_n_utils_package_uq_2022-0.0.5.8.tar`

### file list

```diff
@@ -1,5 +1,72 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/__init__.py
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/LICENSE
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/README.md
--rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/.idea/libs_n_utils.iml
+-rwxr-xr-x   0        0        0      728 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/.idea/misc.xml
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/.idea/modules.xml
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/.idea/vcs.xml
+-rwxr-xr-x   0        0        0    13393 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/.idea/workspace.xml
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0     2910 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py
+-rwxr-xr-x   0        0        0     4170 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/MI_feature_importance.py
+-rwxr-xr-x   0        0        0     7434 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/RF_feature_importance.py
+-rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0     2042 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/__init__.py
+-rwxr-xr-x   0        0        0     5959 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/attack_types.py
+-rwxr-xr-x   0        0        0     1950 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/average_wasserstein.py
+-rwxr-xr-x   0        0        0     7707 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py
+-rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/boruta_visualisation.py
+-rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/combine_2feather.py
+-rwxr-xr-x   0        0        0     3106 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/combine_2pickles.py
+-rwxr-xr-x   0        0        0     3275 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/combine_3pickles.py
+-rwxr-xr-x   0        0        0     3853 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/combine_folder_csv.py
+-rwxr-xr-x   0        0        0      997 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py
+-rwxr-xr-x   0        0        0    25974 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/config_template.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py
+-rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py
+-rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/datasets_information.py
+-rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dict_manipulation.py
+-rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/edit_CIC.py
+-rwxr-xr-x   0        0        0     1445 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py
+-rwxr-xr-x   0        0        0     1300 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py
+-rwxr-xr-x   0        0        0    12326 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     3219 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     2758 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_NN_functional.py
+-rwxr-xr-x   0        0        0     6969 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_NN_models.py
+-rwxr-xr-x   0        0        0     1970 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_binary_classification.py
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py
+-rwxr-xr-x   0        0        0     3983 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py
+-rwxr-xr-x   0        0        0     9119 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_embedding.py
+-rwxr-xr-x   0        0        0    12694 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py
+-rwxr-xr-x   0        0        0    10597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py
+-rwxr-xr-x   0        0        0     3295 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_flow.py
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_helpers.py
+-rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_imbalance.py
+-rwxr-xr-x   0        0        0     5205 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py
+-rwxr-xr-x   0        0        0    37853 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_plotters.py
+-rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_small_utils.py
+-rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py
+-rwxr-xr-x   0        0        0     5405 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/make_cics_compatible.py
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py
+-rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/my_easy_logger.py
+-rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py
+-rwxr-xr-x   0        0        0     2333 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py
+-rwxr-xr-x   0        0        0     1403 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py
+-rwxr-xr-x   0        0        0     1830 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py
+-rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/reading_txt_files.py
+-rwxr-xr-x   0        0        0     4697 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py
+-rwxr-xr-x   0        0        0     4880 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py
+-rwxr-xr-x   0        0        0     3335 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0    79057 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl
+-rwxr-xr-x   0        0        0    51264 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz
+-rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl
+-rwxr-xr-x   0        0        0    56778 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz
+-rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl
+-rwxr-xr-x   0        0        0    83508 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl
+-rwxr-xr-x   0        0        0    56775 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz
+-rwxr-xr-x   0        0        0    56776 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/LICENSE
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/README.md
+-rwxr-xr-x   0        0        0      636 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.8/PKG-INFO
```

### Comparing `libs_n_utils_package_uq_2022-0.0.4/LICENSE` & `libs_n_utils_package_uq_2022-0.0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.4/pyproject.toml` & `libs_n_utils_package_uq_2022-0.0.5.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libs_n_utils_package_uq_2022"
-version = "0.0.4"
+version = "0.0.5.8"
 authors = [
   { name="siamak layeghy", email="siamak.layeghy@uq.net.au" },
 ]
-description = "A small library of utilities"
+description = "A small library of utilities, version 0.0.5.8 import issue is fixed."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.4/PKG-INFO` & `libs_n_utils_package_uq_2022-0.0.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: libs_n_utils_package_uq_2022
-Version: 0.0.4
-Summary: A small library of utilities
+Version: 0.0.5.8
+Summary: A small library of utilities, version 0.0.5.8 import issue is fixed.
 Project-URL: Homepage, https://github.com/layeghy/libs_n_utils
 Project-URL: Bug Tracker, https://github.com/layeghy/libs_n_utils/issues
 Author-email: siamak layeghy <siamak.layeghy@uq.net.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

