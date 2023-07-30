# Comparing `tmp/flota_app-0.1.1.tar.gz` & `tmp/flota_app-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flota_app-0.1.1.tar", max compression
+gzip compressed data, was "flota_app-0.1.2.tar", max compression
```

## Comparing `flota_app-0.1.1.tar` & `flota_app-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,100 @@
--rw-r--r--   0        0        0        0 2023-05-03 13:27:19.100299 flota_app-0.1.1/flota_app/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 15:36:13.240345 flota_app-0.1.1/flota_app/builders/__init__.py
--rw-r--r--   0        0        0      977 2023-07-24 20:51:14.495350 flota_app-0.1.1/flota_app/builders/basic_insurance_builder.py
--rw-r--r--   0        0        0      881 2023-07-24 20:44:39.799319 flota_app-0.1.1/flota_app/builders/basic_mot_builder.py
--rw-r--r--   0        0        0     1034 2023-07-25 18:04:48.287334 flota_app-0.1.1/flota_app/builders/car_builder.py
--rw-r--r--   0        0        0      130 2023-07-30 18:00:08.142786 flota_app-0.1.1/flota_app/config/config_files/.env
--rw-r--r--   0        0        0       96 2023-07-25 07:01:29.116904 flota_app-0.1.1/flota_app/config/config_files/mail.env
--rw-r--r--   0        0        0      559 2023-07-30 17:25:44.984000 flota_app-0.1.1/flota_app/data/cars.json
--rw-r--r--   0        0        0        0 2023-05-03 13:57:16.285857 flota_app-0.1.1/flota_app/factory/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 16:36:49.181783 flota_app-0.1.1/flota_app/factory/converters/__init__.py
--rw-r--r--   0        0        0      430 2023-07-24 15:11:17.518229 flota_app-0.1.1/flota_app/factory/converters/converter.py
--rw-r--r--   0        0        0      495 2023-07-21 12:08:48.669683 flota_app-0.1.1/flota_app/factory/converters/to_car_converter.py
--rw-r--r--   0        0        0        0 2023-05-17 17:14:10.354549 flota_app-0.1.1/flota_app/factory/factories/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 17:15:11.730729 flota_app-0.1.1/flota_app/factory/factories/car_factories/__init__.py
--rw-r--r--   0        0        0     1724 2023-07-21 12:33:55.944761 flota_app-0.1.1/flota_app/factory/factories/car_factories/csv_factories.py
--rw-r--r--   0        0        0     1607 2023-07-21 12:33:55.965598 flota_app-0.1.1/flota_app/factory/factories/car_factories/json_factories.py
--rw-r--r--   0        0        0     1608 2023-07-21 12:33:56.848695 flota_app-0.1.1/flota_app/factory/factories/car_factories/jsonl_factories.py
--rw-r--r--   0        0        0     1824 2023-07-21 12:33:55.994190 flota_app-0.1.1/flota_app/factory/factories/car_factories/sqlite_factories.py
--rw-r--r--   0        0        0     1724 2023-07-21 12:33:56.015011 flota_app-0.1.1/flota_app/factory/factories/car_factories/txt_factories.py
--rw-r--r--   0        0        0     1659 2023-07-21 12:33:56.038076 flota_app-0.1.1/flota_app/factory/factories/car_factories/xlsx_factories.py
--rw-r--r--   0        0        0      512 2023-07-21 12:08:48.706974 flota_app-0.1.1/flota_app/factory/factories/data_factory.py
--rw-r--r--   0        0        0        0 2023-05-03 13:58:05.313372 flota_app-0.1.1/flota_app/factory/loaders/__init__.py
--rw-r--r--   0        0        0      859 2023-07-21 12:33:56.081549 flota_app-0.1.1/flota_app/factory/loaders/csv_loader.py
--rw-r--r--   0        0        0      288 2023-07-21 12:44:48.062168 flota_app-0.1.1/flota_app/factory/loaders/data_loader.py
--rw-r--r--   0        0        0      527 2023-05-03 14:04:21.655117 flota_app-0.1.1/flota_app/factory/loaders/json_loader.py
--rw-r--r--   0        0        0      528 2023-05-03 22:04:35.547468 flota_app-0.1.1/flota_app/factory/loaders/jsonl_loader.py
--rw-r--r--   0        0        0     1296 2023-05-03 14:33:12.350814 flota_app-0.1.1/flota_app/factory/loaders/sqlite_loader.py
--rw-r--r--   0        0        0      784 2023-05-04 21:16:26.015658 flota_app-0.1.1/flota_app/factory/loaders/txt_loader.py
--rw-r--r--   0        0        0      701 2023-05-04 22:26:53.028748 flota_app-0.1.1/flota_app/factory/loaders/xlsx_loader.py
--rw-r--r--   0        0        0        0 2023-05-17 20:23:03.541251 flota_app-0.1.1/flota_app/factory/processors/__init__.py
--rw-r--r--   0        0        0      830 2023-07-21 12:44:47.978434 flota_app-0.1.1/flota_app/factory/processors/data_processor.py
--rw-r--r--   0        0        0        0 2023-05-15 16:25:29.857586 flota_app-0.1.1/flota_app/factory/validators/__init__.py
--rw-r--r--   0        0        0     1296 2023-07-21 12:44:48.004210 flota_app-0.1.1/flota_app/factory/validators/json_dict_validator.py
--rw-r--r--   0        0        0      284 2023-07-21 12:44:47.948826 flota_app-0.1.1/flota_app/factory/validators/validator.py
--rw-r--r--   0        0        0        0 2023-05-03 13:34:52.498293 flota_app-0.1.1/flota_app/models/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-27 20:28:54.103702 flota_app-0.1.1/flota_app/models/car.py
--rw-r--r--   0        0        0        0 2023-07-20 06:48:43.003964 flota_app-0.1.1/flota_app/models/insurances/__init__.py
--rw-r--r--   0        0        0      930 2023-07-24 07:08:17.357095 flota_app-0.1.1/flota_app/models/insurances/basic_insurance.py
--rw-r--r--   0        0        0      978 2023-07-24 07:08:17.365414 flota_app-0.1.1/flota_app/models/insurances/dealership_insurance.py
--rw-r--r--   0        0        0     2044 2023-07-24 07:08:17.331114 flota_app-0.1.1/flota_app/models/insurances/insurance.py
--rw-r--r--   0        0        0        0 2023-07-20 06:48:36.337811 flota_app-0.1.1/flota_app/models/mots/__init__.py
--rw-r--r--   0        0        0      427 2023-07-24 07:08:17.347877 flota_app-0.1.1/flota_app/models/mots/basic_mot.py
--rw-r--r--   0        0        0     1995 2023-07-24 07:08:17.340637 flota_app-0.1.1/flota_app/models/mots/mot.py
--rw-r--r--   0        0        0        0 2023-05-18 19:45:19.206696 flota_app-0.1.1/flota_app/repo/__init__.py
--rw-r--r--   0        0        0     1142 2023-07-24 13:49:26.516559 flota_app-0.1.1/flota_app/repo/cars_repo.py
--rw-r--r--   0        0        0     1278 2023-07-24 13:49:26.765344 flota_app-0.1.1/flota_app/repo/insurances_repo.py
--rw-r--r--   0        0        0     1065 2023-07-24 13:49:26.545794 flota_app-0.1.1/flota_app/repo/mots_repo.py
--rw-r--r--   0        0        0        0 2023-05-26 15:58:15.425850 flota_app-0.1.1/flota_app/services/__init__.py
--rw-r--r--   0        0        0     9336 2023-07-30 18:43:57.846488 flota_app-0.1.1/flota_app/services/cars_fleet_sevice.py
--rw-r--r--   0        0        0     1448 2023-07-27 18:57:51.609992 flota_app-0.1.1/flota_app/services/mailing_service.py
--rw-r--r--   0        0        0      224 2023-07-25 06:47:58.938118 flota_app-0.1.1/flota_app/utils.py
--rw-r--r--   0        0        0      548 2023-07-30 18:44:11.039751 flota_app-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 13:27:19.100299 flota_app-0.1.1/README.md
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 flota_app-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 13:27:19.100299 flota_app-0.1.2/flota_app/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:36:13.240345 flota_app-0.1.2/flota_app/builders/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-24 16:41:12.339486 flota_app-0.1.2/flota_app/builders/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2402 2023-07-24 20:51:18.038546 flota_app-0.1.2/flota_app/builders/__pycache__/basic_insurance_builder.cpython-311.pyc
+-rw-r--r--   0        0        0     2302 2023-07-24 20:44:43.012131 flota_app-0.1.2/flota_app/builders/__pycache__/basic_mot_builder.cpython-311.pyc
+-rw-r--r--   0        0        0     2532 2023-07-25 20:55:18.413492 flota_app-0.1.2/flota_app/builders/__pycache__/car_builder.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2023-07-24 20:51:14.495350 flota_app-0.1.2/flota_app/builders/basic_insurance_builder.py
+-rw-r--r--   0        0        0      881 2023-07-24 20:44:39.799319 flota_app-0.1.2/flota_app/builders/basic_mot_builder.py
+-rw-r--r--   0        0        0     1034 2023-07-25 18:04:48.287334 flota_app-0.1.2/flota_app/builders/car_builder.py
+-rw-r--r--   0        0        0      130 2023-07-30 18:00:08.142786 flota_app-0.1.2/flota_app/config/config_files/.env
+-rw-r--r--   0        0        0       96 2023-07-25 07:01:29.116904 flota_app-0.1.2/flota_app/config/config_files/mail.env
+-rw-r--r--   0        0        0      559 2023-07-30 17:25:44.984000 flota_app-0.1.2/flota_app/data/cars.json
+-rw-r--r--   0        0        0        0 2023-05-03 13:57:16.285857 flota_app-0.1.2/flota_app/factory/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-03 14:04:53.846055 flota_app-0.1.2/flota_app/factory/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-05-15 16:36:49.181783 flota_app-0.1.2/flota_app/factory/converters/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-17 17:34:44.930336 flota_app-0.1.2/flota_app/factory/converters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1075 2023-07-24 16:41:12.221484 flota_app-0.1.2/flota_app/factory/converters/__pycache__/converter.cpython-311.pyc
+-rw-r--r--   0        0        0     1551 2023-07-24 16:41:12.210485 flota_app-0.1.2/flota_app/factory/converters/__pycache__/to_car_converter.cpython-311.pyc
+-rw-r--r--   0        0        0      430 2023-07-24 15:11:17.518229 flota_app-0.1.2/flota_app/factory/converters/converter.py
+-rw-r--r--   0        0        0      495 2023-07-21 12:08:48.669683 flota_app-0.1.2/flota_app/factory/converters/to_car_converter.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:14:10.354549 flota_app-0.1.2/flota_app/factory/factories/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-17 20:13:37.493286 flota_app-0.1.2/flota_app/factory/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1241 2023-07-24 16:41:12.194486 flota_app-0.1.2/flota_app/factory/factories/__pycache__/data_factory.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-05-17 17:15:11.730729 flota_app-0.1.2/flota_app/factory/factories/car_factories/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-17 20:13:37.493286 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2877 2023-07-24 16:41:12.914198 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/csv_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     2746 2023-07-24 16:41:12.947196 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/json_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     2739 2023-07-24 16:41:12.965952 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/jsonl_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     3015 2023-07-24 16:41:12.181486 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/sqlite_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     2877 2023-07-24 16:41:13.091261 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/txt_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     2785 2023-07-24 16:41:13.166262 flota_app-0.1.2/flota_app/factory/factories/car_factories/__pycache__/xlsx_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     1724 2023-07-21 12:33:55.944761 flota_app-0.1.2/flota_app/factory/factories/car_factories/csv_factories.py
+-rw-r--r--   0        0        0     1607 2023-07-21 12:33:55.965598 flota_app-0.1.2/flota_app/factory/factories/car_factories/json_factories.py
+-rw-r--r--   0        0        0     1608 2023-07-21 12:33:56.848695 flota_app-0.1.2/flota_app/factory/factories/car_factories/jsonl_factories.py
+-rw-r--r--   0        0        0     1824 2023-07-21 12:33:55.994190 flota_app-0.1.2/flota_app/factory/factories/car_factories/sqlite_factories.py
+-rw-r--r--   0        0        0     1724 2023-07-21 12:33:56.015011 flota_app-0.1.2/flota_app/factory/factories/car_factories/txt_factories.py
+-rw-r--r--   0        0        0     1659 2023-07-21 12:33:56.038076 flota_app-0.1.2/flota_app/factory/factories/car_factories/xlsx_factories.py
+-rw-r--r--   0        0        0      512 2023-07-21 12:08:48.706974 flota_app-0.1.2/flota_app/factory/factories/data_factory.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:58:05.313372 flota_app-0.1.2/flota_app/factory/loaders/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-03 14:04:53.861680 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2097 2023-07-24 16:41:12.926196 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/csv_loader.cpython-311.pyc
+-rw-r--r--   0        0        0      920 2023-07-24 16:41:12.250485 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     1436 2023-05-03 14:04:53.861680 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/json_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     1592 2023-05-03 22:17:36.770317 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/jsonl_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     2770 2023-05-04 20:51:41.970009 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/sqlite_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     2688 2023-05-04 21:16:27.403940 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/txt_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     2073 2023-05-04 22:27:32.865033 flota_app-0.1.2/flota_app/factory/loaders/__pycache__/xlsx_loader.cpython-311.pyc
+-rw-r--r--   0        0        0      859 2023-07-21 12:33:56.081549 flota_app-0.1.2/flota_app/factory/loaders/csv_loader.py
+-rw-r--r--   0        0        0      288 2023-07-21 12:44:48.062168 flota_app-0.1.2/flota_app/factory/loaders/data_loader.py
+-rw-r--r--   0        0        0      527 2023-05-03 14:04:21.655117 flota_app-0.1.2/flota_app/factory/loaders/json_loader.py
+-rw-r--r--   0        0        0      528 2023-05-03 22:04:35.547468 flota_app-0.1.2/flota_app/factory/loaders/jsonl_loader.py
+-rw-r--r--   0        0        0     1296 2023-05-03 14:33:12.350814 flota_app-0.1.2/flota_app/factory/loaders/sqlite_loader.py
+-rw-r--r--   0        0        0      784 2023-05-04 21:16:26.015658 flota_app-0.1.2/flota_app/factory/loaders/txt_loader.py
+-rw-r--r--   0        0        0      701 2023-05-04 22:26:53.028748 flota_app-0.1.2/flota_app/factory/loaders/xlsx_loader.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:23:03.541251 flota_app-0.1.2/flota_app/factory/processors/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-17 20:27:22.905409 flota_app-0.1.2/flota_app/factory/processors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1778 2023-07-24 16:41:14.445689 flota_app-0.1.2/flota_app/factory/processors/__pycache__/data_processor.cpython-311.pyc
+-rw-r--r--   0        0        0      830 2023-07-21 12:44:47.978434 flota_app-0.1.2/flota_app/factory/processors/data_processor.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:25:29.857586 flota_app-0.1.2/flota_app/factory/validators/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-17 17:34:44.802308 flota_app-0.1.2/flota_app/factory/validators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2342 2023-07-24 16:41:12.264484 flota_app-0.1.2/flota_app/factory/validators/__pycache__/json_dict_validator.cpython-311.pyc
+-rw-r--r--   0        0        0      956 2023-07-24 16:41:12.276483 flota_app-0.1.2/flota_app/factory/validators/__pycache__/validator.cpython-311.pyc
+-rw-r--r--   0        0        0     1296 2023-07-21 12:44:48.004210 flota_app-0.1.2/flota_app/factory/validators/json_dict_validator.py
+-rw-r--r--   0        0        0      284 2023-07-21 12:44:47.948826 flota_app-0.1.2/flota_app/factory/validators/validator.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:34:52.498293 flota_app-0.1.2/flota_app/models/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-03 14:04:53.877357 flota_app-0.1.2/flota_app/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4147 2023-07-30 12:44:07.430216 flota_app-0.1.2/flota_app/models/__pycache__/car.cpython-311.pyc
+-rw-r--r--   0        0        0     2433 2023-07-27 20:28:54.103702 flota_app-0.1.2/flota_app/models/car.py
+-rw-r--r--   0        0        0        0 2023-07-20 06:48:43.003964 flota_app-0.1.2/flota_app/models/insurances/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-20 09:58:52.704897 flota_app-0.1.2/flota_app/models/insurances/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1725 2023-07-24 16:41:11.967387 flota_app-0.1.2/flota_app/models/insurances/__pycache__/basic_insurance.cpython-311.pyc
+-rw-r--r--   0        0        0     1830 2023-07-24 16:41:14.488170 flota_app-0.1.2/flota_app/models/insurances/__pycache__/dealership_insurance.cpython-311.pyc
+-rw-r--r--   0        0        0     3775 2023-07-24 16:41:11.982576 flota_app-0.1.2/flota_app/models/insurances/__pycache__/insurance.cpython-311.pyc
+-rw-r--r--   0        0        0      930 2023-07-24 07:08:17.357095 flota_app-0.1.2/flota_app/models/insurances/basic_insurance.py
+-rw-r--r--   0        0        0      978 2023-07-24 07:08:17.365414 flota_app-0.1.2/flota_app/models/insurances/dealership_insurance.py
+-rw-r--r--   0        0        0     2044 2023-07-24 07:08:17.331114 flota_app-0.1.2/flota_app/models/insurances/insurance.py
+-rw-r--r--   0        0        0        0 2023-07-20 06:48:36.337811 flota_app-0.1.2/flota_app/models/mots/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-20 07:01:05.675939 flota_app-0.1.2/flota_app/models/mots/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1190 2023-07-24 16:41:12.005649 flota_app-0.1.2/flota_app/models/mots/__pycache__/basic_mot.cpython-311.pyc
+-rw-r--r--   0        0        0     3674 2023-07-24 16:41:12.024484 flota_app-0.1.2/flota_app/models/mots/__pycache__/mot.cpython-311.pyc
+-rw-r--r--   0        0        0      427 2023-07-24 07:08:17.347877 flota_app-0.1.2/flota_app/models/mots/basic_mot.py
+-rw-r--r--   0        0        0     1995 2023-07-24 07:08:17.340637 flota_app-0.1.2/flota_app/models/mots/mot.py
+-rw-r--r--   0        0        0        0 2023-05-18 19:45:19.206696 flota_app-0.1.2/flota_app/repo/__init__.py
+-rw-r--r--   0        0        0      179 2023-05-26 17:08:24.550519 flota_app-0.1.2/flota_app/repo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2259 2023-07-24 16:41:11.932388 flota_app-0.1.2/flota_app/repo/__pycache__/cars_repo.cpython-311.pyc
+-rw-r--r--   0        0        0     2432 2023-07-24 16:41:11.954387 flota_app-0.1.2/flota_app/repo/__pycache__/insurances_repo.cpython-311.pyc
+-rw-r--r--   0        0        0     2230 2023-07-24 16:41:11.996579 flota_app-0.1.2/flota_app/repo/__pycache__/mots_repo.cpython-311.pyc
+-rw-r--r--   0        0        0     1142 2023-07-24 13:49:26.516559 flota_app-0.1.2/flota_app/repo/cars_repo.py
+-rw-r--r--   0        0        0     1278 2023-07-24 13:49:26.765344 flota_app-0.1.2/flota_app/repo/insurances_repo.py
+-rw-r--r--   0        0        0     1065 2023-07-24 13:49:26.545794 flota_app-0.1.2/flota_app/repo/mots_repo.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:58:15.425850 flota_app-0.1.2/flota_app/services/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-16 09:55:19.310125 flota_app-0.1.2/flota_app/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14817 2023-07-30 20:52:38.966442 flota_app-0.1.2/flota_app/services/__pycache__/cars_fleet_sevice.cpython-311.pyc
+-rw-r--r--   0        0        0     2932 2023-07-27 19:13:17.634016 flota_app-0.1.2/flota_app/services/__pycache__/mailing_service.cpython-311.pyc
+-rw-r--r--   0        0        0     9274 2023-07-30 20:52:34.729555 flota_app-0.1.2/flota_app/services/cars_fleet_sevice.py
+-rw-r--r--   0        0        0     1448 2023-07-27 18:57:51.609992 flota_app-0.1.2/flota_app/services/mailing_service.py
+-rw-r--r--   0        0        0      224 2023-07-25 06:47:58.938118 flota_app-0.1.2/flota_app/utils.py
+-rw-r--r--   0        0        0      548 2023-07-30 20:54:14.866224 flota_app-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 13:27:19.100299 flota_app-0.1.2/README.md
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 flota_app-0.1.2/PKG-INFO
```

### Comparing `flota_app-0.1.1/flota_app/builders/basic_insurance_builder.py` & `flota_app-0.1.2/flota_app/builders/basic_insurance_builder.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/builders/basic_mot_builder.py` & `flota_app-0.1.2/flota_app/builders/basic_mot_builder.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/builders/car_builder.py` & `flota_app-0.1.2/flota_app/builders/car_builder.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/data/cars.json` & `flota_app-0.1.2/flota_app/data/cars.json`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/car_factories/csv_factories.py` & `flota_app-0.1.2/flota_app/factory/factories/car_factories/csv_factories.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/car_factories/json_factories.py` & `flota_app-0.1.2/flota_app/factory/factories/car_factories/json_factories.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/car_factories/jsonl_factories.py` & `flota_app-0.1.2/flota_app/factory/factories/car_factories/jsonl_factories.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/car_factories/sqlite_factories.py` & `flota_app-0.1.2/flota_app/factory/factories/car_factories/sqlite_factories.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/car_factories/txt_factories.py` & `flota_app-0.1.2/flota_app/factory/factories/car_factories/txt_factories.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/car_factories/xlsx_factories.py` & `flota_app-0.1.2/flota_app/factory/factories/car_factories/xlsx_factories.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/factories/data_factory.py` & `flota_app-0.1.2/flota_app/factory/factories/data_factory.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/loaders/csv_loader.py` & `flota_app-0.1.2/flota_app/factory/loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/loaders/json_loader.py` & `flota_app-0.1.2/flota_app/factory/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/loaders/jsonl_loader.py` & `flota_app-0.1.2/flota_app/factory/loaders/jsonl_loader.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/loaders/sqlite_loader.py` & `flota_app-0.1.2/flota_app/factory/loaders/sqlite_loader.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/loaders/txt_loader.py` & `flota_app-0.1.2/flota_app/factory/loaders/txt_loader.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/loaders/xlsx_loader.py` & `flota_app-0.1.2/flota_app/factory/loaders/xlsx_loader.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/processors/data_processor.py` & `flota_app-0.1.2/flota_app/factory/processors/data_processor.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/factory/validators/json_dict_validator.py` & `flota_app-0.1.2/flota_app/factory/validators/json_dict_validator.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/models/car.py` & `flota_app-0.1.2/flota_app/models/car.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/models/insurances/basic_insurance.py` & `flota_app-0.1.2/flota_app/models/insurances/basic_insurance.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/models/insurances/dealership_insurance.py` & `flota_app-0.1.2/flota_app/models/insurances/dealership_insurance.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/models/insurances/insurance.py` & `flota_app-0.1.2/flota_app/models/insurances/insurance.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/models/mots/mot.py` & `flota_app-0.1.2/flota_app/models/mots/mot.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/repo/cars_repo.py` & `flota_app-0.1.2/flota_app/repo/cars_repo.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/repo/insurances_repo.py` & `flota_app-0.1.2/flota_app/repo/insurances_repo.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/repo/mots_repo.py` & `flota_app-0.1.2/flota_app/repo/mots_repo.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/flota_app/services/cars_fleet_sevice.py` & `flota_app-0.1.2/flota_app/services/cars_fleet_sevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,15 @@
 
     def update_mot(self, mot: BasicMot) -> int:
         """
         Deletes old mot and inserts new one
         :param mot: BasicMot object that needs to be deleted from database table
         :return: id of newly created record
         """
-        deleted_mot = self.mot_by_car_id(mot.car_id)
-        self.basic_mots_repo.delete_one(deleted_mot.id)
+        self.basic_mots_repo.delete_one(mot.id)
         return self.basic_mots_repo.insert(mot)
 
     def cars_with_insurances_by_deadline(self) -> list[datetime.date, Insurance, Car]:
         """
         List of elements that have structure of: [insurance_deadline, BasicInsurance object, Car object]
         in ascending order. Handy when user want to generate list of insurances that needs to be renewed
         :return: list of lists that have deadline, insurance and car
```

### Comparing `flota_app-0.1.1/flota_app/services/mailing_service.py` & `flota_app-0.1.2/flota_app/services/mailing_service.py`

 * *Files identical despite different names*

### Comparing `flota_app-0.1.1/pyproject.toml` & `flota_app-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flota-app"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Smolke <d.smolczynski1@gmail.com>"]
 readme = "README.md"
 packages = [{include = "flota_app"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `flota_app-0.1.1/PKG-INFO` & `flota_app-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flota-app
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbm-database-service (>=0.2.5,<0.3.0)
```

