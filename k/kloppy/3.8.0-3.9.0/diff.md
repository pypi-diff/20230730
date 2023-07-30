# Comparing `tmp/kloppy-3.8.0.tar.gz` & `tmp/kloppy-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kloppy-3.8.0.tar", last modified: Sun Mar  5 19:15:04 2023, max compression
+gzip compressed data, was "kloppy-3.9.0.tar", last modified: Tue Mar 14 17:34:47 2023, max compression
```

## Comparing `kloppy-3.8.0.tar` & `kloppy-3.9.0.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.813911 kloppy-3.8.0/
--rw-r--r--   0 koen       (501) staff       (20)     1515 2021-12-16 13:21:19.000000 kloppy-3.8.0/LICENSE
--rw-r--r--   0 koen       (501) staff       (20)       42 2021-12-16 13:21:19.000000 kloppy-3.8.0/MANIFEST.in
--rw-r--r--   0 koen       (501) staff       (20)     4149 2023-03-05 19:15:04.813736 kloppy-3.8.0/PKG-INFO
--rw-r--r--   0 koen       (501) staff       (20)     3332 2022-10-12 08:23:34.000000 kloppy-3.8.0/README.md
--rw-r--r--   0 koen       (501) staff       (20)      172 2022-10-14 21:11:31.000000 kloppy-3.8.0/docs-requirements.txt
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.801423 kloppy-3.8.0/kloppy/
--rw-r--r--   0 koen       (501) staff       (20)      469 2023-03-05 19:11:16.000000 kloppy-3.8.0/kloppy/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.803252 kloppy-3.8.0/kloppy/_providers/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/_providers/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1065 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/_providers/datafactory.py
--rw-r--r--   0 koen       (501) staff       (20)     4461 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/_providers/metrica.py
--rw-r--r--   0 koen       (501) staff       (20)     1173 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/_providers/opta.py
--rw-r--r--   0 koen       (501) staff       (20)     1187 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/_providers/secondspectrum.py
--rw-r--r--   0 koen       (501) staff       (20)     1604 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/_providers/skillcorner.py
--rw-r--r--   0 koen       (501) staff       (20)     1227 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/_providers/sportec.py
--rw-r--r--   0 koen       (501) staff       (20)      600 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/_providers/sportscode.py
--rw-r--r--   0 koen       (501) staff       (20)     2845 2022-11-24 09:55:02.000000 kloppy-3.8.0/kloppy/_providers/statsbomb.py
--rw-r--r--   0 koen       (501) staff       (20)      851 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/_providers/tracab.py
--rw-r--r--   0 koen       (501) staff       (20)     1567 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/_providers/wyscout.py
--rw-r--r--   0 koen       (501) staff       (20)     7451 2022-06-03 11:08:35.000000 kloppy-3.8.0/kloppy/cmdline.py
--rw-r--r--   0 koen       (501) staff       (20)     2498 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/config.py
--rw-r--r--   0 koen       (501) staff       (20)       41 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/datafactory.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.803353 kloppy-3.8.0/kloppy/domain/
--rw-r--r--   0 koen       (501) staff       (20)       46 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.804204 kloppy-3.8.0/kloppy/domain/models/
--rw-r--r--   0 koen       (501) staff       (20)      108 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/models/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     2338 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/models/code.py
--rw-r--r--   0 koen       (501) staff       (20)    25301 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/models/common.py
--rw-r--r--   0 koen       (501) staff       (20)    23293 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/models/event.py
--rw-r--r--   0 koen       (501) staff       (20)     2539 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/models/formation.py
--rw-r--r--   0 koen       (501) staff       (20)     2223 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/models/pitch.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.804408 kloppy-3.8.0/kloppy/domain/models/statsbomb/
--rw-r--r--   0 koen       (501) staff       (20)        0 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/domain/models/statsbomb/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      723 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/domain/models/statsbomb/event.py
--rw-r--r--   0 koen       (501) staff       (20)     2503 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/models/tracking.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.804633 kloppy-3.8.0/kloppy/domain/services/
--rw-r--r--   0 koen       (501) staff       (20)     1033 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     3214 2022-11-24 09:55:02.000000 kloppy-3.8.0/kloppy/domain/services/event_factory.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.804841 kloppy-3.8.0/kloppy/domain/services/matchers/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/matchers/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1201 2022-03-12 11:33:31.000000 kloppy-3.8.0/kloppy/domain/services/matchers/css.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.805036 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     4686 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/event.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.805511 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/
--rw-r--r--   0 koen       (501) staff       (20)       65 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     5715 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/ast.py
--rw-r--r--   0 koen       (501) staff       (20)     5206 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/matchers.py
--rw-r--r--   0 koen       (501) staff       (20)    19652 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/regexp.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.805876 kloppy-3.8.0/kloppy/domain/services/state_builder/
--rw-r--r--   0 koen       (501) staff       (20)     1337 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      499 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/builder.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.806440 kloppy-3.8.0/kloppy/domain/services/state_builder/builders/
--rw-r--r--   0 koen       (501) staff       (20)      164 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/builders/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1260 2022-01-28 20:54:58.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/builders/formation.py
--rw-r--r--   0 koen       (501) staff       (20)     1629 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/builders/lineup.py
--rw-r--r--   0 koen       (501) staff       (20)      882 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/builders/score.py
--rw-r--r--   0 koen       (501) staff       (20)     1392 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/builders/sequence.py
--rw-r--r--   0 koen       (501) staff       (20)      954 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/domain/services/state_builder/registered.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.806875 kloppy-3.8.0/kloppy/domain/services/transformers/
--rw-r--r--   0 koen       (501) staff       (20)       40 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/transformers/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    11361 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/services/transformers/attribute.py
--rw-r--r--   0 koen       (501) staff       (20)     3517 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/domain/services/transformers/data_record.py
--rw-r--r--   0 koen       (501) staff       (20)    13906 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/domain/services/transformers/dataset.py
--rw-r--r--   0 koen       (501) staff       (20)       54 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/event_pattern_matching.py
--rw-r--r--   0 koen       (501) staff       (20)      487 2022-08-24 12:33:25.000000 kloppy-3.8.0/kloppy/exceptions.py
--rw-r--r--   0 koen       (501) staff       (20)     1708 2022-07-17 11:43:30.000000 kloppy-3.8.0/kloppy/helpers.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.806987 kloppy-3.8.0/kloppy/infra/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/infra/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.807075 kloppy-3.8.0/kloppy/infra/io/
--rw-r--r--   0 koen       (501) staff       (20)        0 2022-03-23 21:59:28.000000 kloppy-3.8.0/kloppy/infra/io/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.807484 kloppy-3.8.0/kloppy/infra/io/adapters/
--rw-r--r--   0 koen       (501) staff       (20)      295 2022-03-23 21:59:28.000000 kloppy-3.8.0/kloppy/infra/io/adapters/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      277 2022-03-23 21:59:28.000000 kloppy-3.8.0/kloppy/infra/io/adapters/adapter.py
--rw-r--r--   0 koen       (501) staff       (20)     1659 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/io/adapters/http.py
--rw-r--r--   0 koen       (501) staff       (20)      964 2022-03-23 21:59:28.000000 kloppy-3.8.0/kloppy/infra/io/adapters/s3.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.807594 kloppy-3.8.0/kloppy/infra/serializers/
--rw-r--r--   0 koen       (501) staff       (20)      451 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/infra/serializers/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.807906 kloppy-3.8.0/kloppy/infra/serializers/code/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/infra/serializers/code/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      474 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/code/base.py
--rw-r--r--   0 koen       (501) staff       (20)     4302 2022-08-24 12:33:25.000000 kloppy-3.8.0/kloppy/infra/serializers/code/sportscode.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.808137 kloppy-3.8.0/kloppy/infra/serializers/event/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/infra/serializers/event/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.808376 kloppy-3.8.0/kloppy/infra/serializers/event/datafactory/
--rw-r--r--   0 koen       (501) staff       (20)       69 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/datafactory/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    20032 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/datafactory/deserializer.py
--rw-r--r--   0 koen       (501) staff       (20)     2161 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/deserializer.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.808611 kloppy-3.8.0/kloppy/infra/serializers/event/metrica/
--rw-r--r--   0 koen       (501) staff       (20)      105 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/metrica/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    12593 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/metrica/json_deserializer.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.808856 kloppy-3.8.0/kloppy/infra/serializers/event/opta/
--rw-r--r--   0 koen       (501) staff       (20)       55 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/opta/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    24393 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/opta/deserializer.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.809096 kloppy-3.8.0/kloppy/infra/serializers/event/sportec/
--rw-r--r--   0 koen       (501) staff       (20)       66 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/sportec/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    19617 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/sportec/deserializer.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.809338 kloppy-3.8.0/kloppy/infra/serializers/event/statsbomb/
--rw-r--r--   0 koen       (501) staff       (20)       65 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/statsbomb/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    33098 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/infra/serializers/event/statsbomb/deserializer.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.809830 kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/
--rw-r--r--   0 koen       (501) staff       (20)       61 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)    15313 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/deserializer.py
--rw-r--r--   0 koen       (501) staff       (20)     1112 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/wyscout_events.py
--rw-r--r--   0 koen       (501) staff       (20)     1330 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/wyscout_tags.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.810556 kloppy-3.8.0/kloppy/infra/serializers/tracking/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1709 2022-07-17 11:43:30.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/deserializer.py
--rw-r--r--   0 koen       (501) staff       (20)     8174 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_csv.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.811200 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/
--rw-r--r--   0 koen       (501) staff       (20)      106 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     4411 2022-10-14 21:02:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/deserializer.py
--rw-r--r--   0 koen       (501) staff       (20)     9863 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/metadata.py
--rw-r--r--   0 koen       (501) staff       (20)     4640 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/models.py
--rw-r--r--   0 koen       (501) staff       (20)     3238 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/reader.py
--rw-r--r--   0 koen       (501) staff       (20)    10915 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/secondspectrum.py
--rw-r--r--   0 koen       (501) staff       (20)    13330 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/skillcorner.py
--rw-r--r--   0 koen       (501) staff       (20)     7190 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/infra/serializers/tracking/tracab.py
--rw-r--r--   0 koen       (501) staff       (20)     3340 2023-01-16 20:44:27.000000 kloppy-3.8.0/kloppy/io.py
--rw-r--r--   0 koen       (501) staff       (20)      119 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/metrica.py
--rw-r--r--   0 koen       (501) staff       (20)       34 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/opta.py
--rw-r--r--   0 koen       (501) staff       (20)       44 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/secondspectrum.py
--rw-r--r--   0 koen       (501) staff       (20)       57 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/skillcorner.py
--rw-r--r--   0 koen       (501) staff       (20)       37 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/sportec.py
--rw-r--r--   0 koen       (501) staff       (20)       46 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/sportscode.py
--rw-r--r--   0 koen       (501) staff       (20)       55 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/statsbomb.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.813481 kloppy-3.8.0/kloppy/tests/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/tests/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     2070 2023-01-09 20:57:35.000000 kloppy-3.8.0/kloppy/tests/test_adapter.py
--rw-r--r--   0 koen       (501) staff       (20)     1760 2023-03-03 19:57:50.000000 kloppy-3.8.0/kloppy/tests/test_config.py
--rw-r--r--   0 koen       (501) staff       (20)     2386 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/tests/test_datafactory.py
--rw-r--r--   0 koen       (501) staff       (20)     2572 2022-03-12 11:33:31.000000 kloppy-3.8.0/kloppy/tests/test_event.py
--rw-r--r--   0 koen       (501) staff       (20)    12864 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/tests/test_helpers.py
--rw-r--r--   0 koen       (501) staff       (20)      621 2021-12-16 13:21:19.000000 kloppy-3.8.0/kloppy/tests/test_metadata.py
--rw-r--r--   0 koen       (501) staff       (20)     2334 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/tests/test_metrica_csv.py
--rw-r--r--   0 koen       (501) staff       (20)     7090 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/tests/test_metrica_epts.py
--rw-r--r--   0 koen       (501) staff       (20)     2053 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/tests/test_metrica_events.py
--rw-r--r--   0 koen       (501) staff       (20)     3953 2022-10-12 08:23:34.000000 kloppy-3.8.0/kloppy/tests/test_opta.py
--rw-r--r--   0 koen       (501) staff       (20)     4100 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/tests/test_secondspectrum.py
--rw-r--r--   0 koen       (501) staff       (20)     4019 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/tests/test_skillcorner.py
--rw-r--r--   0 koen       (501) staff       (20)     2536 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/tests/test_sportec.py
--rw-r--r--   0 koen       (501) staff       (20)     4360 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/tests/test_state_builder.py
--rw-r--r--   0 koen       (501) staff       (20)     9795 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/tests/test_statsbomb.py
--rw-r--r--   0 koen       (501) staff       (20)     2530 2022-10-12 08:23:34.000000 kloppy-3.8.0/kloppy/tests/test_to_records.py
--rw-r--r--   0 koen       (501) staff       (20)     3252 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/tests/test_tracab.py
--rw-r--r--   0 koen       (501) staff       (20)      666 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/tests/test_wyscout.py
--rw-r--r--   0 koen       (501) staff       (20)     3301 2021-12-21 09:17:13.000000 kloppy-3.8.0/kloppy/tests/test_xml.py
--rw-r--r--   0 koen       (501) staff       (20)       36 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/tracab.py
--rw-r--r--   0 koen       (501) staff       (20)     4242 2023-03-05 18:34:50.000000 kloppy-3.8.0/kloppy/utils.py
--rw-r--r--   0 koen       (501) staff       (20)       53 2023-03-03 20:30:16.000000 kloppy-3.8.0/kloppy/wyscout.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-05 19:15:04.802084 kloppy-3.8.0/kloppy.egg-info/
--rw-r--r--   0 koen       (501) staff       (20)     4149 2023-03-05 19:15:04.000000 kloppy-3.8.0/kloppy.egg-info/PKG-INFO
--rw-r--r--   0 koen       (501) staff       (20)     4812 2023-03-05 19:15:04.000000 kloppy-3.8.0/kloppy.egg-info/SOURCES.txt
--rw-r--r--   0 koen       (501) staff       (20)        1 2023-03-05 19:15:04.000000 kloppy-3.8.0/kloppy.egg-info/dependency_links.txt
--rw-r--r--   0 koen       (501) staff       (20)       58 2023-03-05 19:15:04.000000 kloppy-3.8.0/kloppy.egg-info/entry_points.txt
--rw-r--r--   0 koen       (501) staff       (20)      308 2023-03-05 19:15:04.000000 kloppy-3.8.0/kloppy.egg-info/requires.txt
--rw-r--r--   0 koen       (501) staff       (20)        7 2023-03-05 19:15:04.000000 kloppy-3.8.0/kloppy.egg-info/top_level.txt
--rw-r--r--   0 koen       (501) staff       (20)      173 2021-12-16 13:21:19.000000 kloppy-3.8.0/pyproject.toml
--rw-r--r--   0 koen       (501) staff       (20)       94 2023-03-05 18:34:50.000000 kloppy-3.8.0/requirements.txt
--rw-r--r--   0 koen       (501) staff       (20)        3 2022-10-14 21:08:29.000000 kloppy-3.8.0/runtime.txt
--rw-r--r--   0 koen       (501) staff       (20)       38 2023-03-05 19:15:04.813957 kloppy-3.8.0/setup.cfg
--rw-r--r--   0 koen       (501) staff       (20)     2002 2023-03-05 18:34:50.000000 kloppy-3.8.0/setup.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.845324 kloppy-3.9.0/
+-rw-r--r--   0 koen       (501) staff       (20)     1515 2021-12-16 13:21:19.000000 kloppy-3.9.0/LICENSE
+-rw-r--r--   0 koen       (501) staff       (20)       42 2021-12-16 13:21:19.000000 kloppy-3.9.0/MANIFEST.in
+-rw-r--r--   0 koen       (501) staff       (20)     4149 2023-03-14 17:34:47.845123 kloppy-3.9.0/PKG-INFO
+-rw-r--r--   0 koen       (501) staff       (20)     3332 2022-10-12 08:23:34.000000 kloppy-3.9.0/README.md
+-rw-r--r--   0 koen       (501) staff       (20)      172 2022-10-14 21:11:31.000000 kloppy-3.9.0/docs-requirements.txt
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.827209 kloppy-3.9.0/kloppy/
+-rw-r--r--   0 koen       (501) staff       (20)      469 2023-03-14 17:33:45.000000 kloppy-3.9.0/kloppy/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.830120 kloppy-3.9.0/kloppy/_providers/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/_providers/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1065 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/_providers/datafactory.py
+-rw-r--r--   0 koen       (501) staff       (20)     4461 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/_providers/metrica.py
+-rw-r--r--   0 koen       (501) staff       (20)     1173 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/_providers/opta.py
+-rw-r--r--   0 koen       (501) staff       (20)     1187 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/_providers/secondspectrum.py
+-rw-r--r--   0 koen       (501) staff       (20)     1604 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/_providers/skillcorner.py
+-rw-r--r--   0 koen       (501) staff       (20)     1227 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/_providers/sportec.py
+-rw-r--r--   0 koen       (501) staff       (20)      600 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/_providers/sportscode.py
+-rw-r--r--   0 koen       (501) staff       (20)     2845 2022-11-24 09:55:02.000000 kloppy-3.9.0/kloppy/_providers/statsbomb.py
+-rw-r--r--   0 koen       (501) staff       (20)      851 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/_providers/tracab.py
+-rw-r--r--   0 koen       (501) staff       (20)     2577 2023-03-14 17:33:07.000000 kloppy-3.9.0/kloppy/_providers/wyscout.py
+-rw-r--r--   0 koen       (501) staff       (20)     7451 2022-06-03 11:08:35.000000 kloppy-3.9.0/kloppy/cmdline.py
+-rw-r--r--   0 koen       (501) staff       (20)     2498 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/config.py
+-rw-r--r--   0 koen       (501) staff       (20)       41 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/datafactory.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.830235 kloppy-3.9.0/kloppy/domain/
+-rw-r--r--   0 koen       (501) staff       (20)       46 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.831953 kloppy-3.9.0/kloppy/domain/models/
+-rw-r--r--   0 koen       (501) staff       (20)      108 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/models/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     2338 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/models/code.py
+-rw-r--r--   0 koen       (501) staff       (20)    25301 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/models/common.py
+-rw-r--r--   0 koen       (501) staff       (20)    23293 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/models/event.py
+-rw-r--r--   0 koen       (501) staff       (20)     2539 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/models/formation.py
+-rw-r--r--   0 koen       (501) staff       (20)     2223 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/models/pitch.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.832194 kloppy-3.9.0/kloppy/domain/models/statsbomb/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/domain/models/statsbomb/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      723 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/domain/models/statsbomb/event.py
+-rw-r--r--   0 koen       (501) staff       (20)     2503 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/models/tracking.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.832614 kloppy-3.9.0/kloppy/domain/services/
+-rw-r--r--   0 koen       (501) staff       (20)     1033 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     3214 2022-11-24 09:55:02.000000 kloppy-3.9.0/kloppy/domain/services/event_factory.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.832955 kloppy-3.9.0/kloppy/domain/services/matchers/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/matchers/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1201 2022-03-12 11:33:31.000000 kloppy-3.9.0/kloppy/domain/services/matchers/css.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.833272 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     4686 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/event.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.833907 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/
+-rw-r--r--   0 koen       (501) staff       (20)       65 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     5715 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/ast.py
+-rw-r--r--   0 koen       (501) staff       (20)     5206 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/matchers.py
+-rw-r--r--   0 koen       (501) staff       (20)    19652 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/regexp.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.834590 kloppy-3.9.0/kloppy/domain/services/state_builder/
+-rw-r--r--   0 koen       (501) staff       (20)     1337 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      499 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/builder.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.835418 kloppy-3.9.0/kloppy/domain/services/state_builder/builders/
+-rw-r--r--   0 koen       (501) staff       (20)      164 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/builders/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1260 2022-01-28 20:54:58.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/builders/formation.py
+-rw-r--r--   0 koen       (501) staff       (20)     1629 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/builders/lineup.py
+-rw-r--r--   0 koen       (501) staff       (20)      882 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/builders/score.py
+-rw-r--r--   0 koen       (501) staff       (20)     1392 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/builders/sequence.py
+-rw-r--r--   0 koen       (501) staff       (20)      954 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/domain/services/state_builder/registered.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.835952 kloppy-3.9.0/kloppy/domain/services/transformers/
+-rw-r--r--   0 koen       (501) staff       (20)       40 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/transformers/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    11361 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/services/transformers/attribute.py
+-rw-r--r--   0 koen       (501) staff       (20)     3517 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/domain/services/transformers/data_record.py
+-rw-r--r--   0 koen       (501) staff       (20)    13906 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/domain/services/transformers/dataset.py
+-rw-r--r--   0 koen       (501) staff       (20)       54 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/event_pattern_matching.py
+-rw-r--r--   0 koen       (501) staff       (20)      487 2022-08-24 12:33:25.000000 kloppy-3.9.0/kloppy/exceptions.py
+-rw-r--r--   0 koen       (501) staff       (20)     1708 2022-07-17 11:43:30.000000 kloppy-3.9.0/kloppy/helpers.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.836088 kloppy-3.9.0/kloppy/infra/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/infra/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.836174 kloppy-3.9.0/kloppy/infra/io/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2022-03-23 21:59:28.000000 kloppy-3.9.0/kloppy/infra/io/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.836859 kloppy-3.9.0/kloppy/infra/io/adapters/
+-rw-r--r--   0 koen       (501) staff       (20)      295 2022-03-23 21:59:28.000000 kloppy-3.9.0/kloppy/infra/io/adapters/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      277 2022-03-23 21:59:28.000000 kloppy-3.9.0/kloppy/infra/io/adapters/adapter.py
+-rw-r--r--   0 koen       (501) staff       (20)     1659 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/io/adapters/http.py
+-rw-r--r--   0 koen       (501) staff       (20)      964 2022-03-23 21:59:28.000000 kloppy-3.9.0/kloppy/infra/io/adapters/s3.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.836995 kloppy-3.9.0/kloppy/infra/serializers/
+-rw-r--r--   0 koen       (501) staff       (20)      451 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/infra/serializers/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.837415 kloppy-3.9.0/kloppy/infra/serializers/code/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/infra/serializers/code/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      474 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/code/base.py
+-rw-r--r--   0 koen       (501) staff       (20)     4302 2022-08-24 12:33:25.000000 kloppy-3.9.0/kloppy/infra/serializers/code/sportscode.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.837693 kloppy-3.9.0/kloppy/infra/serializers/event/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/infra/serializers/event/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.838067 kloppy-3.9.0/kloppy/infra/serializers/event/datafactory/
+-rw-r--r--   0 koen       (501) staff       (20)       69 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/datafactory/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    20032 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/datafactory/deserializer.py
+-rw-r--r--   0 koen       (501) staff       (20)     2161 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/deserializer.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.838541 kloppy-3.9.0/kloppy/infra/serializers/event/metrica/
+-rw-r--r--   0 koen       (501) staff       (20)      105 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/metrica/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    12593 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/metrica/json_deserializer.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.838851 kloppy-3.9.0/kloppy/infra/serializers/event/opta/
+-rw-r--r--   0 koen       (501) staff       (20)       55 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/opta/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    24393 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/opta/deserializer.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.839221 kloppy-3.9.0/kloppy/infra/serializers/event/sportec/
+-rw-r--r--   0 koen       (501) staff       (20)       66 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/sportec/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    19617 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/sportec/deserializer.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.839552 kloppy-3.9.0/kloppy/infra/serializers/event/statsbomb/
+-rw-r--r--   0 koen       (501) staff       (20)       65 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/statsbomb/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    33098 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/infra/serializers/event/statsbomb/deserializer.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.840524 kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/
+-rw-r--r--   0 koen       (501) staff       (20)      117 2023-03-14 17:33:07.000000 kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    15315 2023-03-14 17:33:07.000000 kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/deserializer_v2.py
+-rw-r--r--   0 koen       (501) staff       (20)    14239 2023-03-14 17:33:07.000000 kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/deserializer_v3.py
+-rw-r--r--   0 koen       (501) staff       (20)     1112 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/wyscout_events.py
+-rw-r--r--   0 koen       (501) staff       (20)     1330 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/wyscout_tags.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.841566 kloppy-3.9.0/kloppy/infra/serializers/tracking/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1709 2022-07-17 11:43:30.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/deserializer.py
+-rw-r--r--   0 koen       (501) staff       (20)     8174 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_csv.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.842431 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/
+-rw-r--r--   0 koen       (501) staff       (20)      106 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     4411 2022-10-14 21:02:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/deserializer.py
+-rw-r--r--   0 koen       (501) staff       (20)     9863 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/metadata.py
+-rw-r--r--   0 koen       (501) staff       (20)     4640 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/models.py
+-rw-r--r--   0 koen       (501) staff       (20)     3238 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/reader.py
+-rw-r--r--   0 koen       (501) staff       (20)    10915 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/secondspectrum.py
+-rw-r--r--   0 koen       (501) staff       (20)    13330 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/skillcorner.py
+-rw-r--r--   0 koen       (501) staff       (20)     7190 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/infra/serializers/tracking/tracab.py
+-rw-r--r--   0 koen       (501) staff       (20)     3340 2023-01-16 20:44:27.000000 kloppy-3.9.0/kloppy/io.py
+-rw-r--r--   0 koen       (501) staff       (20)      119 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/metrica.py
+-rw-r--r--   0 koen       (501) staff       (20)       34 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/opta.py
+-rw-r--r--   0 koen       (501) staff       (20)       44 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/secondspectrum.py
+-rw-r--r--   0 koen       (501) staff       (20)       57 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/skillcorner.py
+-rw-r--r--   0 koen       (501) staff       (20)       37 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/sportec.py
+-rw-r--r--   0 koen       (501) staff       (20)       46 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/sportscode.py
+-rw-r--r--   0 koen       (501) staff       (20)       55 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/statsbomb.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.844818 kloppy-3.9.0/kloppy/tests/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/tests/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     2070 2023-01-09 20:57:35.000000 kloppy-3.9.0/kloppy/tests/test_adapter.py
+-rw-r--r--   0 koen       (501) staff       (20)     1760 2023-03-03 19:57:50.000000 kloppy-3.9.0/kloppy/tests/test_config.py
+-rw-r--r--   0 koen       (501) staff       (20)     2386 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/tests/test_datafactory.py
+-rw-r--r--   0 koen       (501) staff       (20)     2572 2022-03-12 11:33:31.000000 kloppy-3.9.0/kloppy/tests/test_event.py
+-rw-r--r--   0 koen       (501) staff       (20)    12864 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/tests/test_helpers.py
+-rw-r--r--   0 koen       (501) staff       (20)      621 2021-12-16 13:21:19.000000 kloppy-3.9.0/kloppy/tests/test_metadata.py
+-rw-r--r--   0 koen       (501) staff       (20)     2334 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/tests/test_metrica_csv.py
+-rw-r--r--   0 koen       (501) staff       (20)     7090 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/tests/test_metrica_epts.py
+-rw-r--r--   0 koen       (501) staff       (20)     2053 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/tests/test_metrica_events.py
+-rw-r--r--   0 koen       (501) staff       (20)     3953 2022-10-12 08:23:34.000000 kloppy-3.9.0/kloppy/tests/test_opta.py
+-rw-r--r--   0 koen       (501) staff       (20)     4100 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/tests/test_secondspectrum.py
+-rw-r--r--   0 koen       (501) staff       (20)     4019 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/tests/test_skillcorner.py
+-rw-r--r--   0 koen       (501) staff       (20)     2536 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/tests/test_sportec.py
+-rw-r--r--   0 koen       (501) staff       (20)     4360 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/tests/test_state_builder.py
+-rw-r--r--   0 koen       (501) staff       (20)     9795 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/tests/test_statsbomb.py
+-rw-r--r--   0 koen       (501) staff       (20)     2530 2022-10-12 08:23:34.000000 kloppy-3.9.0/kloppy/tests/test_to_records.py
+-rw-r--r--   0 koen       (501) staff       (20)     3252 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/tests/test_tracab.py
+-rw-r--r--   0 koen       (501) staff       (20)     1432 2023-03-14 17:33:07.000000 kloppy-3.9.0/kloppy/tests/test_wyscout.py
+-rw-r--r--   0 koen       (501) staff       (20)     3301 2021-12-21 09:17:13.000000 kloppy-3.9.0/kloppy/tests/test_xml.py
+-rw-r--r--   0 koen       (501) staff       (20)       36 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/tracab.py
+-rw-r--r--   0 koen       (501) staff       (20)     4242 2023-03-05 18:34:50.000000 kloppy-3.9.0/kloppy/utils.py
+-rw-r--r--   0 koen       (501) staff       (20)       53 2023-03-03 20:30:16.000000 kloppy-3.9.0/kloppy/wyscout.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2023-03-14 17:34:47.827930 kloppy-3.9.0/kloppy.egg-info/
+-rw-r--r--   0 koen       (501) staff       (20)     4149 2023-03-14 17:34:47.000000 kloppy-3.9.0/kloppy.egg-info/PKG-INFO
+-rw-r--r--   0 koen       (501) staff       (20)     4873 2023-03-14 17:34:47.000000 kloppy-3.9.0/kloppy.egg-info/SOURCES.txt
+-rw-r--r--   0 koen       (501) staff       (20)        1 2023-03-14 17:34:47.000000 kloppy-3.9.0/kloppy.egg-info/dependency_links.txt
+-rw-r--r--   0 koen       (501) staff       (20)       58 2023-03-14 17:34:47.000000 kloppy-3.9.0/kloppy.egg-info/entry_points.txt
+-rw-r--r--   0 koen       (501) staff       (20)      308 2023-03-14 17:34:47.000000 kloppy-3.9.0/kloppy.egg-info/requires.txt
+-rw-r--r--   0 koen       (501) staff       (20)        7 2023-03-14 17:34:47.000000 kloppy-3.9.0/kloppy.egg-info/top_level.txt
+-rw-r--r--   0 koen       (501) staff       (20)      173 2021-12-16 13:21:19.000000 kloppy-3.9.0/pyproject.toml
+-rw-r--r--   0 koen       (501) staff       (20)       94 2023-03-05 18:34:50.000000 kloppy-3.9.0/requirements.txt
+-rw-r--r--   0 koen       (501) staff       (20)        3 2022-10-14 21:08:29.000000 kloppy-3.9.0/runtime.txt
+-rw-r--r--   0 koen       (501) staff       (20)       38 2023-03-14 17:34:47.845457 kloppy-3.9.0/setup.cfg
+-rw-r--r--   0 koen       (501) staff       (20)     2002 2023-03-05 18:34:50.000000 kloppy-3.9.0/setup.py
```

### Comparing `kloppy-3.8.0/LICENSE` & `kloppy-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/PKG-INFO` & `kloppy-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kloppy
-Version: 3.8.0
+Version: 3.9.0
 Summary: Standardizing soccer tracking- and event data
 Home-page: https://kloppy.pysport.org/
 Author: Koen Vossen
 Author-email: info@koenvossen.nl
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kloppy Version: 3.8.0 Summary: Standardizing soccer
+Metadata-Version: 2.1 Name: kloppy Version: 3.9.0 Summary: Standardizing soccer
 tracking- and event data Home-page: https://kloppy.pysport.org/ Author: Koen
 Vossen Author-email: info@koenvossen.nl License: BSD Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kloppy-3.8.0/README.md` & `kloppy-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/datafactory.py` & `kloppy-3.9.0/kloppy/_providers/datafactory.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/metrica.py` & `kloppy-3.9.0/kloppy/_providers/metrica.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/opta.py` & `kloppy-3.9.0/kloppy/_providers/opta.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/secondspectrum.py` & `kloppy-3.9.0/kloppy/_providers/secondspectrum.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/skillcorner.py` & `kloppy-3.9.0/kloppy/_providers/skillcorner.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/sportec.py` & `kloppy-3.9.0/kloppy/_providers/sportec.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/sportscode.py` & `kloppy-3.9.0/kloppy/_providers/sportscode.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/statsbomb.py` & `kloppy-3.9.0/kloppy/_providers/statsbomb.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/_providers/tracab.py` & `kloppy-3.9.0/kloppy/_providers/tracab.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/cmdline.py` & `kloppy-3.9.0/kloppy/cmdline.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/config.py` & `kloppy-3.9.0/kloppy/config.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/code.py` & `kloppy-3.9.0/kloppy/domain/models/code.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/common.py` & `kloppy-3.9.0/kloppy/domain/models/common.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/event.py` & `kloppy-3.9.0/kloppy/domain/models/event.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/formation.py` & `kloppy-3.9.0/kloppy/domain/models/formation.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/pitch.py` & `kloppy-3.9.0/kloppy/domain/models/pitch.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/statsbomb/event.py` & `kloppy-3.9.0/kloppy/domain/models/statsbomb/event.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/models/tracking.py` & `kloppy-3.9.0/kloppy/domain/models/tracking.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/__init__.py` & `kloppy-3.9.0/kloppy/domain/services/__init__.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/event_factory.py` & `kloppy-3.9.0/kloppy/domain/services/event_factory.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/matchers/css.py` & `kloppy-3.9.0/kloppy/domain/services/matchers/css.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/matchers/pattern/event.py` & `kloppy-3.9.0/kloppy/domain/services/matchers/pattern/event.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/ast.py` & `kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/ast.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/matchers.py` & `kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/matchers.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/matchers/pattern/regexp/regexp.py` & `kloppy-3.9.0/kloppy/domain/services/matchers/pattern/regexp/regexp.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/state_builder/__init__.py` & `kloppy-3.9.0/kloppy/domain/services/state_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/state_builder/builders/formation.py` & `kloppy-3.9.0/kloppy/domain/services/state_builder/builders/formation.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/state_builder/builders/lineup.py` & `kloppy-3.9.0/kloppy/domain/services/state_builder/builders/lineup.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/state_builder/builders/score.py` & `kloppy-3.9.0/kloppy/domain/services/state_builder/builders/score.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/state_builder/builders/sequence.py` & `kloppy-3.9.0/kloppy/domain/services/state_builder/builders/sequence.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/state_builder/registered.py` & `kloppy-3.9.0/kloppy/domain/services/state_builder/registered.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/transformers/attribute.py` & `kloppy-3.9.0/kloppy/domain/services/transformers/attribute.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/transformers/data_record.py` & `kloppy-3.9.0/kloppy/domain/services/transformers/data_record.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/domain/services/transformers/dataset.py` & `kloppy-3.9.0/kloppy/domain/services/transformers/dataset.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/helpers.py` & `kloppy-3.9.0/kloppy/helpers.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/io/adapters/http.py` & `kloppy-3.9.0/kloppy/infra/io/adapters/http.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/io/adapters/s3.py` & `kloppy-3.9.0/kloppy/infra/io/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/code/sportscode.py` & `kloppy-3.9.0/kloppy/infra/serializers/code/sportscode.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/datafactory/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/datafactory/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/metrica/json_deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/metrica/json_deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/opta/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/opta/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/sportec/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/sportec/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/statsbomb/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/statsbomb/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/deserializer_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     return {player.player_id: player for player in players}
 
 
 class WyscoutInputs(NamedTuple):
     event_data: IO[bytes]
 
 
-class WyscoutDeserializer(EventDataDeserializer[WyscoutInputs]):
+class WyscoutDeserializerV2(EventDataDeserializer[WyscoutInputs]):
     @property
     def provider(self) -> Provider:
         return Provider.WYSCOUT
 
     def deserialize(self, inputs: WyscoutInputs) -> EventDataset:
         transformer = self.get_transformer(length=100, width=100)
```

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/wyscout_events.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/wyscout_events.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/event/wyscout/wyscout_tags.py` & `kloppy-3.9.0/kloppy/infra/serializers/event/wyscout/wyscout_tags.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_csv.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_csv.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/deserializer.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/deserializer.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/metadata.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/metadata.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/models.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/models.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/metrica_epts/reader.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/metrica_epts/reader.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/secondspectrum.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/secondspectrum.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/skillcorner.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/skillcorner.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/infra/serializers/tracking/tracab.py` & `kloppy-3.9.0/kloppy/infra/serializers/tracking/tracab.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/io.py` & `kloppy-3.9.0/kloppy/io.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_adapter.py` & `kloppy-3.9.0/kloppy/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_config.py` & `kloppy-3.9.0/kloppy/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_datafactory.py` & `kloppy-3.9.0/kloppy/tests/test_datafactory.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_event.py` & `kloppy-3.9.0/kloppy/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_helpers.py` & `kloppy-3.9.0/kloppy/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_metadata.py` & `kloppy-3.9.0/kloppy/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_metrica_csv.py` & `kloppy-3.9.0/kloppy/tests/test_metrica_csv.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_metrica_epts.py` & `kloppy-3.9.0/kloppy/tests/test_metrica_epts.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_metrica_events.py` & `kloppy-3.9.0/kloppy/tests/test_metrica_events.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_opta.py` & `kloppy-3.9.0/kloppy/tests/test_opta.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_secondspectrum.py` & `kloppy-3.9.0/kloppy/tests/test_secondspectrum.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_skillcorner.py` & `kloppy-3.9.0/kloppy/tests/test_skillcorner.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_sportec.py` & `kloppy-3.9.0/kloppy/tests/test_sportec.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_state_builder.py` & `kloppy-3.9.0/kloppy/tests/test_state_builder.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_statsbomb.py` & `kloppy-3.9.0/kloppy/tests/test_statsbomb.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_to_records.py` & `kloppy-3.9.0/kloppy/tests/test_to_records.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_tracab.py` & `kloppy-3.9.0/kloppy/tests/test_tracab.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/tests/test_xml.py` & `kloppy-3.9.0/kloppy/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy/utils.py` & `kloppy-3.9.0/kloppy/utils.py`

 * *Files identical despite different names*

### Comparing `kloppy-3.8.0/kloppy.egg-info/PKG-INFO` & `kloppy-3.9.0/kloppy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kloppy
-Version: 3.8.0
+Version: 3.9.0
 Summary: Standardizing soccer tracking- and event data
 Home-page: https://kloppy.pysport.org/
 Author: Koen Vossen
 Author-email: info@koenvossen.nl
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kloppy Version: 3.8.0 Summary: Standardizing soccer
+Metadata-Version: 2.1 Name: kloppy Version: 3.9.0 Summary: Standardizing soccer
 tracking- and event data Home-page: https://kloppy.pysport.org/ Author: Koen
 Vossen Author-email: info@koenvossen.nl License: BSD Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kloppy-3.8.0/kloppy.egg-info/SOURCES.txt` & `kloppy-3.9.0/kloppy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,16 @@
 kloppy/infra/serializers/event/opta/__init__.py
 kloppy/infra/serializers/event/opta/deserializer.py
 kloppy/infra/serializers/event/sportec/__init__.py
 kloppy/infra/serializers/event/sportec/deserializer.py
 kloppy/infra/serializers/event/statsbomb/__init__.py
 kloppy/infra/serializers/event/statsbomb/deserializer.py
 kloppy/infra/serializers/event/wyscout/__init__.py
-kloppy/infra/serializers/event/wyscout/deserializer.py
+kloppy/infra/serializers/event/wyscout/deserializer_v2.py
+kloppy/infra/serializers/event/wyscout/deserializer_v3.py
 kloppy/infra/serializers/event/wyscout/wyscout_events.py
 kloppy/infra/serializers/event/wyscout/wyscout_tags.py
 kloppy/infra/serializers/tracking/__init__.py
 kloppy/infra/serializers/tracking/deserializer.py
 kloppy/infra/serializers/tracking/metrica_csv.py
 kloppy/infra/serializers/tracking/secondspectrum.py
 kloppy/infra/serializers/tracking/skillcorner.py
```

### Comparing `kloppy-3.8.0/setup.py` & `kloppy-3.9.0/setup.py`

 * *Files identical despite different names*

