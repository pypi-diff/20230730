# Comparing `tmp/atooms_database-0.2.0-py2.py3-none-any.whl.zip` & `tmp/atooms_database-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,27 @@
-Zip file size: 70030 bytes, number of entries: 37
+Zip file size: 61519 bytes, number of entries: 25
 -rw-rw-r--  2.0 unx      722 b- defN 23-Jun-06 05:58 atooms/__init__.py
 -rw-rw-r--  2.0 unx     2579 b- defN 23-Jun-07 18:30 atooms/database/__init__.py
 -rw-rw-r--  2.0 unx      859 b- defN 23-Jun-07 18:30 atooms/database/_cutoffs.py
 -rw-rw-r--  2.0 unx    12417 b- defN 23-Jul-27 20:15 atooms/database/_models.json
 -rw-rw-r--  2.0 unx     1634 b- defN 23-Jun-10 15:29 atooms/database/_potentials.py
 -rw-rw-r--  2.0 unx     1871 b- defN 23-Jun-07 16:16 atooms/database/_samples.json
 -rw-rw-r--  2.0 unx     1824 b- defN 23-Jun-06 05:58 atooms/database/_schemas.py
 -rw-rw-r--  2.0 unx     9607 b- defN 23-Jun-24 15:50 atooms/database/database.py
 -rw-rw-r--  2.0 unx     4664 b- defN 23-Jun-12 18:47 atooms/database/helpers.py
 -rw-rw-r--  2.0 unx     3233 b- defN 23-Jun-12 18:47 atooms/database/hooks.py
 -rw-rw-r--  2.0 unx     3214 b- defN 23-Jun-07 15:45 atooms/database/schema.py
--rw-rw-r--  2.0 unx     3106 b- defN 23-Jun-06 12:29 atooms/database/f90/__init__.py
--rw-rw-r--  2.0 unx     2875 b- defN 23-Jun-06 05:58 atooms/database/f90/cubic_spline.f90
--rw-rw-r--  2.0 unx      965 b- defN 23-Jun-06 05:58 atooms/database/f90/cut.f90
--rw-rw-r--  2.0 unx     2041 b- defN 23-Jun-06 05:58 atooms/database/f90/cut_shift.f90
--rw-rw-r--  2.0 unx      769 b- defN 23-Jun-06 05:58 atooms/database/f90/gaussian.f90
--rw-rw-r--  2.0 unx      993 b- defN 23-Jun-06 05:58 atooms/database/f90/harmonic_potential.f90
--rw-rw-r--  2.0 unx     1516 b- defN 23-Jun-06 05:58 atooms/database/f90/inverse_power.f90
--rw-rw-r--  2.0 unx     1780 b- defN 23-Jun-06 05:58 atooms/database/f90/inverse_power_exp.f90
--rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-06 05:58 atooms/database/f90/lennard_jones.f90
--rw-rw-r--  2.0 unx     2018 b- defN 23-Jun-06 05:58 atooms/database/f90/linear_cut_shift.f90
--rw-rw-r--  2.0 unx     2022 b- defN 23-Jun-06 05:58 atooms/database/f90/quadratic_cut_shift.f90
--rw-rw-r--  2.0 unx     1364 b- defN 23-Jun-06 05:58 atooms/database/f90/sum_inverse_power.f90
--rw-rw-r--  2.0 unx     1137 b- defN 23-Jun-06 05:58 atooms/database/f90/yukawa.f90
+-rw-rw-r--  2.0 unx     3082 b- defN 23-Jul-30 14:17 atooms/database/f90/__init__.py
 -rw-rw-r--  2.0 unx       35 b- defN 23-Jun-06 05:58 atooms/database/rumd/__init__.py
 -rw-rw-r--  2.0 unx     6469 b- defN 23-Jun-06 11:37 atooms/database/rumd/interaction.py
 -rw-rw-r--  2.0 unx     6774 b- defN 23-Jun-06 05:58 atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz
 -rw-rw-r--  2.0 unx     9280 b- defN 23-Jun-06 05:58 atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz
 -rw-rw-r--  2.0 unx    59127 b- defN 23-Jun-06 05:58 atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz
 -rw-rw-r--  2.0 unx     4656 b- defN 23-Jun-06 05:58 atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz
 -rw-rw-r--  2.0 unx     7888 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz
 -rw-rw-r--  2.0 unx     5927 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3475 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       64 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3561 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/RECORD
-37 files, 171599 bytes uncompressed, 64162 bytes compressed:  62.6%
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3475 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       64 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2441 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/RECORD
+25 files, 151952 bytes uncompressed, 57441 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -30,50 +30,14 @@
 
 Filename: atooms/database/schema.py
 Comment: 
 
 Filename: atooms/database/f90/__init__.py
 Comment: 
 
-Filename: atooms/database/f90/cubic_spline.f90
-Comment: 
-
-Filename: atooms/database/f90/cut.f90
-Comment: 
-
-Filename: atooms/database/f90/cut_shift.f90
-Comment: 
-
-Filename: atooms/database/f90/gaussian.f90
-Comment: 
-
-Filename: atooms/database/f90/harmonic_potential.f90
-Comment: 
-
-Filename: atooms/database/f90/inverse_power.f90
-Comment: 
-
-Filename: atooms/database/f90/inverse_power_exp.f90
-Comment: 
-
-Filename: atooms/database/f90/lennard_jones.f90
-Comment: 
-
-Filename: atooms/database/f90/linear_cut_shift.f90
-Comment: 
-
-Filename: atooms/database/f90/quadratic_cut_shift.f90
-Comment: 
-
-Filename: atooms/database/f90/sum_inverse_power.f90
-Comment: 
-
-Filename: atooms/database/f90/yukawa.f90
-Comment: 
-
 Filename: atooms/database/rumd/__init__.py
 Comment: 
 
 Filename: atooms/database/rumd/interaction.py
 Comment: 
 
 Filename: atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz
@@ -90,23 +54,23 @@
 
 Filename: atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz
 Comment: 
 
 Filename: atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz
 Comment: 
 
-Filename: atooms_database-0.2.0.dist-info/LICENSE
+Filename: atooms_database-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: atooms_database-0.2.0.dist-info/METADATA
+Filename: atooms_database-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: atooms_database-0.2.0.dist-info/WHEEL
+Filename: atooms_database-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: atooms_database-0.2.0.dist-info/top_level.txt
+Filename: atooms_database-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: atooms_database-0.2.0.dist-info/RECORD
+Filename: atooms_database-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atooms/database/f90/__init__.py

```diff
@@ -20,17 +20,17 @@
             else:
                 # This may be a string, so we look for the model in the
                 # atooms-database database and replace the string with the dictionary
                 model = database.model(model)
 
         super(). __init__(model, neighbor_list, interaction, helpers,
                           inline=inline, inline_safe=inline_safe,
-                          debug=debug, parallel=parallel, search_dir=os.path.dirname(__file__)
-                          )
+                          debug=debug, parallel=parallel)
 
+# TODO: move this to atooms.backends.f90
 def available():
     """Pretty print the available potentials"""
     print('Available potentials:')
     for potential in _database_potential:
         print('- ', potential)
 
     print('Available cutoffs:')
```

## Comparing `atooms_database-0.2.0.dist-info/METADATA` & `atooms_database-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-database
-Version: 0.2.0
+Version: 0.3.0
 Summary: Database of interaction database for classical molecular dynamics and Monte Carlo simulations
 Home-page: https://framagit.org/atooms/database
 Author: Daniele Coslovich
 Author-email: dcoslovich@units.it
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

## Comparing `atooms_database-0.2.0.dist-info/RECORD` & `atooms_database-0.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -5,33 +5,21 @@
 atooms/database/_potentials.py,sha256=pMgcaVKcdt64EWDqWRu4guznohhkT6UVNRqXs6VTBAg,1634
 atooms/database/_samples.json,sha256=N340blAeCElnqgaKFBfDNSaGXwbW6RfEvGfQTXB9TE0,1871
 atooms/database/_schemas.py,sha256=B84mKnLIJwQYb4a7jV0Dfd6q1dVgUHcPVFG-iLtiWJY,1824
 atooms/database/database.py,sha256=M6LiZ3MQruhCLarOsxts6rBSYfBKbXS_T2UxXWG5n-M,9607
 atooms/database/helpers.py,sha256=hAE5qLdzKsyn37gRJbsip1MFLLW_zvli8FQGlFD2ghQ,4664
 atooms/database/hooks.py,sha256=661oTk9lIrCqSyEJL3lqtOCrtB893_yZyNLE3gPKiv8,3233
 atooms/database/schema.py,sha256=NlFFo1qe2sL6SnjKKTk4ktOg-NhE0xscXKkZ81LXykc,3214
-atooms/database/f90/__init__.py,sha256=fWEkUygYIrr4S80Iox67LLiFaCAL7U66jG9r1FzjyMA,3106
-atooms/database/f90/cubic_spline.f90,sha256=eA-Pu0L2YTmD1HdqxPQpHj_grflmUWdDpXQlRKYxjlI,2875
-atooms/database/f90/cut.f90,sha256=0boB-73Vqzwn7aD0TXftY2m7YvPq6g2x0nh26IRONxI,965
-atooms/database/f90/cut_shift.f90,sha256=Xwkw8bB6pi25W_imuQYNX7UpdRt99QELE_OYCPLTOlc,2041
-atooms/database/f90/gaussian.f90,sha256=AzxqZBmaI_2aXiOVVN2dICkzrdlA9EHS3bj9iuJIQIA,769
-atooms/database/f90/harmonic_potential.f90,sha256=uRw6w1EWrwlfdTQthUTa6Aj3aecRsfT1TT18d89B8mw,993
-atooms/database/f90/inverse_power.f90,sha256=KN3SPqEVr-60Q0UqEKVt3t2DEhGfrwEByIvUVTzRb2E,1516
-atooms/database/f90/inverse_power_exp.f90,sha256=-t82Jxk1n5XVFtoN18T8ldTOx8sqwDvF9p_mxCRD4wQ,1780
-atooms/database/f90/lennard_jones.f90,sha256=sENXLN2gf_jKT5LoWTfivqb3T-niv5Oj8HSTHj4CLeU,1023
-atooms/database/f90/linear_cut_shift.f90,sha256=sejCNI4s_damweLJuq5-ZWY8U5GxXp1vd_W0Mq9MFFs,2018
-atooms/database/f90/quadratic_cut_shift.f90,sha256=M8LzhqLssN7r1Z0jGhC-p7zmyzE4auflW1ocbPOinps,2022
-atooms/database/f90/sum_inverse_power.f90,sha256=BIlWKctMdxdY8eRHnUI3kfyAc8trqHeIFPWNGl3di1I,1364
-atooms/database/f90/yukawa.f90,sha256=K9ZJqvQ-wjlaRd0MGrgYQEv1vHuax_n2cDo4aI4VKj0,1137
+atooms/database/f90/__init__.py,sha256=VoRwGacilfd98L8PAc_uG8Jl9Wr6OiSy761tXGJNbgQ,3082
 atooms/database/rumd/__init__.py,sha256=r-RCxnOOySa4xGnExnN0kytJHl9lC1v6ayNB_XyhoXg,35
 atooms/database/rumd/interaction.py,sha256=foD8T4xTfbYEUIhLf0qKOnGt5E_x4nknmAhoTHMAsH0,6469
 atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz,sha256=xak8Bt4Xakfkdoys1NijdyyN1cpMjoiqgK_ncxt3g3Q,6774
 atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz,sha256=QBpKZOyEb1C9hvXXQRdy74e0Sgfar8DvxaH5hKe85XE,9280
 atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz,sha256=9bZ2a_dH8F2o_HCxYgQd_-JYzaYHugiW-E1-Xd5uYmQ,59127
 atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz,sha256=KooMMAxC6GnJLHqdIgbPqyeQt9XtMEVoLVBEjDifUzg,4656
 atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz,sha256=5uaL3JeCkx5xySLCg3MeCeQalnwlAtYpwq4z4ONPaCI,7888
 atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz,sha256=V3ESAodJ1_-9FR4pmvTZTJK45y-a7weZ8EBLn4dpLkE,5927
-atooms_database-0.2.0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atooms_database-0.2.0.dist-info/METADATA,sha256=p1lRverZQ2sGnSv5nxjT0rqH2hukI2kBI4j67OTeB-M,3475
-atooms_database-0.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-atooms_database-0.2.0.dist-info/top_level.txt,sha256=9o7UGu0YidqgwDb_N4ceklT3bPAOArDUWo-qM9G4O5A,64
-atooms_database-0.2.0.dist-info/RECORD,,
+atooms_database-0.3.0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+atooms_database-0.3.0.dist-info/METADATA,sha256=tIjW-NyL5Tnnc1-JKkLzoLxaMSp9REsSZJnNxjlZII0,3475
+atooms_database-0.3.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+atooms_database-0.3.0.dist-info/top_level.txt,sha256=9o7UGu0YidqgwDb_N4ceklT3bPAOArDUWo-qM9G4O5A,64
+atooms_database-0.3.0.dist-info/RECORD,,
```

