# Comparing `tmp/lumigo_opentelemetry-1.0.89-py3-none-any.whl.zip` & `tmp/lumigo_opentelemetry-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,104 +1,82 @@
-Zip file size: 77820 bytes, number of entries: 102
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 ci/__init__.py
--rw-r--r--  2.0 unx    14467 b- defN 23-Jul-30 05:42 ci/tested_versions_utils.py
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-30 05:43 lumigo_opentelemetry/VERSION
--rw-r--r--  2.0 unx     7092 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/__init__.py
--rw-r--r--  2.0 unx     2089 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/dependencies/__init__.py
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/__init__.py
--rw-r--r--  2.0 unx    10112 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/__init__.py
--rw-r--r--  2.0 unx      622 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/package.py
--rw-r--r--  2.0 unx      608 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/version.py
--rw-r--r--  2.0 unx     1617 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/extensions/__init__.py
--rw-r--r--  2.0 unx    13523 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/extensions/dynamodb.py
--rw-r--r--  2.0 unx     4159 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/extensions/lmbd.py
--rw-r--r--  2.0 unx     5472 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/extensions/sqs.py
--rw-r--r--  2.0 unx     4954 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/external/botocore/extensions/types.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/__init__.py
--rw-r--r--  2.0 unx     1999 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/instrumentations.py
--rw-r--r--  2.0 unx      489 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/boto/__init__.py
--rw-r--r--  2.0 unx     1178 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/botocore/__init__.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py
--rw-r--r--  2.0 unx     1286 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/fastapi/__init__.py
--rw-r--r--  2.0 unx     2237 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py
--rw-r--r--  2.0 unx      972 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/flask/__init__.py
--rw-r--r--  2.0 unx     1146 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/grpcio/__init__.py
--rw-r--r--  2.0 unx     1184 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/grpcio/common.py
--rw-r--r--  2.0 unx     2759 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_client.py
--rw-r--r--  2.0 unx     2871 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_server.py
--rw-r--r--  2.0 unx      501 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/kafka_python/__init__.py
--rw-r--r--  2.0 unx      475 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/pika/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/pymongo/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/pymysql/__init__.py
--rw-r--r--  2.0 unx      719 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/requests/__init__.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/libs/__init__.py
--rw-r--r--  2.0 unx     2010 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/libs/general_utils.py
--rw-r--r--  2.0 unx      948 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/libs/json_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/resources/__init__.py
--rw-r--r--  2.0 unx     8250 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/resources/detectors.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/utils/__init__.py
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/utils/aws_utils.py
--rw-r--r--  2.0 unx      197 b- defN 23-Jul-30 05:42 lumigo_opentelemetry/utils/config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/ci/__init__.py
--rw-r--r--  2.0 unx     7385 b- defN 23-Jul-30 05:42 test/ci/test_tested_versions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/components/__init__.py
--rw-r--r--  2.0 unx     1023 b- defN 23-Jul-30 05:42 test/components/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/components/fastapi_external_apis/__init__.py
--rw-r--r--  2.0 unx      131 b- defN 23-Jul-30 05:42 test/components/fastapi_external_apis/app.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/components/tests/__init__.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jul-30 05:42 test/components/tests/test_attr_max_size.py
--rw-r--r--  2.0 unx     1204 b- defN 23-Jul-30 05:42 test/components/tests/test_execution_tags.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/conftest.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/boto3/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/boto3/conftest.py
--rw-r--r--  2.0 unx      460 b- defN 23-Jul-30 05:42 test/integration/boto3/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/boto3/tests/__init__.py
--rw-r--r--  2.0 unx     2425 b- defN 23-Jul-30 05:42 test/integration/boto3/tests/test_boto3.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/fastapi/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/fastapi/conftest.py
--rw-r--r--  2.0 unx      536 b- defN 23-Jul-30 05:42 test/integration/fastapi/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/fastapi/tests/__init__.py
--rw-r--r--  2.0 unx     4623 b- defN 23-Jul-30 05:42 test/integration/fastapi/tests/test_fastapi.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/flask/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/flask/conftest.py
--rw-r--r--  2.0 unx      285 b- defN 23-Jul-30 05:42 test/integration/flask/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/flask/tests/__init__.py
--rw-r--r--  2.0 unx     2560 b- defN 23-Jul-30 05:42 test/integration/flask/tests/test_flask.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/grpcio/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/grpcio/app/__init__.py
--rw-r--r--  2.0 unx     2211 b- defN 23-Jul-30 05:42 test/integration/grpcio/app/greeter_server.py
--rw-r--r--  2.0 unx     1922 b- defN 23-Jul-30 05:42 test/integration/grpcio/app/helloworld_pb2.py
--rw-r--r--  2.0 unx     7290 b- defN 23-Jul-30 05:42 test/integration/grpcio/app/helloworld_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/grpcio/tests/__init__.py
--rw-r--r--  2.0 unx     5270 b- defN 23-Jul-30 05:42 test/integration/grpcio/tests/test_grpcio.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/kafka_python/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/kafka_python/conftest.py
--rw-r--r--  2.0 unx     1661 b- defN 23-Jul-30 05:42 test/integration/kafka_python/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/kafka_python/tests/__init__.py
--rw-r--r--  2.0 unx     2768 b- defN 23-Jul-30 05:42 test/integration/kafka_python/tests/test_kafka_python.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/pika/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/pika/conftest.py
--rw-r--r--  2.0 unx     2442 b- defN 23-Jul-30 05:42 test/integration/pika/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/pika/tests/__init__.py
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-30 05:42 test/integration/pika/tests/test_pika.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/pymongo/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/pymongo/conftest.py
--rw-r--r--  2.0 unx      795 b- defN 23-Jul-30 05:42 test/integration/pymongo/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/pymongo/tests/__init__.py
--rw-r--r--  2.0 unx     1281 b- defN 23-Jul-30 05:42 test/integration/pymongo/tests/test_pymongo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/pymysql/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-30 05:42 test/integration/pymysql/conftest.py
--rw-r--r--  2.0 unx      277 b- defN 23-Jul-30 05:42 test/integration/pymysql/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/integration/pymysql/tests/__init__.py
--rw-r--r--  2.0 unx      887 b- defN 23-Jul-30 05:42 test/integration/pymysql/tests/test_pymysql.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 05:42 test/test_utils/__init__.py
--rw-r--r--  2.0 unx     2412 b- defN 23-Jul-30 05:42 test/test_utils/spans_parser.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-30 05:43 lumigo_opentelemetry-1.0.89.dist-info/LICENSE
--rw-r--r--  2.0 unx    21589 b- defN 23-Jul-30 05:43 lumigo_opentelemetry-1.0.89.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 05:43 lumigo_opentelemetry-1.0.89.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-30 05:43 lumigo_opentelemetry-1.0.89.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-30 05:43 lumigo_opentelemetry-1.0.89.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    10073 b- defN 23-Jul-30 05:43 lumigo_opentelemetry-1.0.89.dist-info/RECORD
-102 files, 203197 bytes uncompressed, 61186 bytes compressed:  69.9%
+Zip file size: 48220 bytes, number of entries: 80
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 ci/__init__.py
+-rw-r--r--  2.0 unx    14299 b- defN 22-Jul-25 13:33 ci/tested_versions_utils.py
+-rw-r--r--  2.0 unx        6 b- defN 22-Jul-25 13:34 lumigo_opentelemetry/VERSION
+-rw-r--r--  2.0 unx     5191 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/__init__.py
+-rw-r--r--  2.0 unx     1750 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/instrumentations.py
+-rw-r--r--  2.0 unx      537 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/aiohttp_client/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/aiopg/__init__.py
+-rw-r--r--  2.0 unx      484 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/asyncpg/__init__.py
+-rw-r--r--  2.0 unx      465 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/boto/__init__.py
+-rw-r--r--  2.0 unx      817 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/botocore/__init__.py
+-rw-r--r--  2.0 unx     5184 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/django/__init__.py
+-rw-r--r--  2.0 unx      553 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/elasticsearch/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/falcon/__init__.py
+-rw-r--r--  2.0 unx     1246 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/fastapi/__init__.py
+-rw-r--r--  2.0 unx     1958 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py
+-rw-r--r--  2.0 unx      932 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/flask/__init__.py
+-rw-r--r--  2.0 unx      477 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/grpc/__init__.py
+-rw-r--r--  2.0 unx      484 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/httpx/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/jinja2/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/kafka/__init__.py
+-rw-r--r--  2.0 unx      482 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/mysql/__init__.py
+-rw-r--r--  2.0 unx      465 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/pika/__init__.py
+-rw-r--r--  2.0 unx      493 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/psycopg2/__init__.py
+-rw-r--r--  2.0 unx      493 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/pymemcache/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/pymongo/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/pymysql/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/pyramid/__init__.py
+-rw-r--r--  2.0 unx      458 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/redis/__init__.py
+-rw-r--r--  2.0 unx      695 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/requests/__init__.py
+-rw-r--r--  2.0 unx     2132 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
+-rw-r--r--  2.0 unx      701 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/sklearn/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/sqlite3/__init__.py
+-rw-r--r--  2.0 unx      476 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/tornado/__init__.py
+-rw-r--r--  2.0 unx      465 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/urllib/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/instrumentations/urllib3/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/libs/__init__.py
+-rw-r--r--  2.0 unx     1306 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/libs/general_utils.py
+-rw-r--r--  2.0 unx     6819 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/libs/json_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/resources/__init__.py
+-rw-r--r--  2.0 unx     3875 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/resources/detectors.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/utils/__init__.py
+-rw-r--r--  2.0 unx      156 b- defN 22-Jul-25 13:33 lumigo_opentelemetry/utils/aws_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 22-Jul-25 13:33 test/integration/conftest.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/boto3/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 22-Jul-25 13:33 test/integration/boto3/conftest.py
+-rw-r--r--  2.0 unx      460 b- defN 22-Jul-25 13:33 test/integration/boto3/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/boto3/tests/__init__.py
+-rw-r--r--  2.0 unx     2376 b- defN 22-Jul-25 13:33 test/integration/boto3/tests/test_boto3.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/fastapi/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 22-Jul-25 13:33 test/integration/fastapi/conftest.py
+-rw-r--r--  2.0 unx      289 b- defN 22-Jul-25 13:33 test/integration/fastapi/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/fastapi/tests/__init__.py
+-rw-r--r--  2.0 unx     2964 b- defN 22-Jul-25 13:33 test/integration/fastapi/tests/test_fastapi.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/flask/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 22-Jul-25 13:33 test/integration/flask/conftest.py
+-rw-r--r--  2.0 unx      285 b- defN 22-Jul-25 13:33 test/integration/flask/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/flask/tests/__init__.py
+-rw-r--r--  2.0 unx     2593 b- defN 22-Jul-25 13:33 test/integration/flask/tests/test_flask.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/pymongo/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 22-Jul-25 13:33 test/integration/pymongo/conftest.py
+-rw-r--r--  2.0 unx      513 b- defN 22-Jul-25 13:33 test/integration/pymongo/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/pymongo/tests/__init__.py
+-rw-r--r--  2.0 unx      896 b- defN 22-Jul-25 13:33 test/integration/pymongo/tests/test_pymongo.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/pymysql/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 22-Jul-25 13:33 test/integration/pymysql/conftest.py
+-rw-r--r--  2.0 unx      277 b- defN 22-Jul-25 13:33 test/integration/pymysql/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/integration/pymysql/tests/__init__.py
+-rw-r--r--  2.0 unx      903 b- defN 22-Jul-25 13:33 test/integration/pymysql/tests/test_pymysql.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-25 13:33 test/test_utils/__init__.py
+-rw-r--r--  2.0 unx     2183 b- defN 22-Jul-25 13:33 test/test_utils/spans_parser.py
+-rw-r--r--  2.0 unx    11357 b- defN 22-Jul-25 13:35 lumigo_opentelemetry-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11840 b- defN 22-Jul-25 13:35 lumigo_opentelemetry-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jul-25 13:35 lumigo_opentelemetry-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 22-Jul-25 13:35 lumigo_opentelemetry-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       29 b- defN 22-Jul-25 13:35 lumigo_opentelemetry-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8064 b- defN 22-Jul-25 13:35 lumigo_opentelemetry-1.0.9.dist-info/RECORD
+80 files, 105318 bytes uncompressed, 34804 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,150 +6,135 @@
 
 Filename: lumigo_opentelemetry/VERSION
 Comment: 
 
 Filename: lumigo_opentelemetry/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/dependencies/__init__.py
-Comment: 
-
-Filename: lumigo_opentelemetry/external/__init__.py
-Comment: 
-
-Filename: lumigo_opentelemetry/external/botocore/__init__.py
-Comment: 
-
-Filename: lumigo_opentelemetry/external/botocore/package.py
-Comment: 
-
-Filename: lumigo_opentelemetry/external/botocore/version.py
+Filename: lumigo_opentelemetry/instrumentations/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/external/botocore/extensions/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/instrumentations.py
 Comment: 
 
-Filename: lumigo_opentelemetry/external/botocore/extensions/dynamodb.py
+Filename: lumigo_opentelemetry/instrumentations/aiohttp_client/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/external/botocore/extensions/lmbd.py
+Filename: lumigo_opentelemetry/instrumentations/aiopg/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/external/botocore/extensions/sqs.py
+Filename: lumigo_opentelemetry/instrumentations/asyncpg/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/external/botocore/extensions/types.py
+Filename: lumigo_opentelemetry/instrumentations/boto/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/botocore/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/instrumentations.py
+Filename: lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/boto/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/django/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/botocore/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/elasticsearch/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/falcon/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/instrumentations/fastapi/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/instrumentations/flask/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/grpcio/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/grpc/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/grpcio/common.py
+Filename: lumigo_opentelemetry/instrumentations/httpx/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_client.py
+Filename: lumigo_opentelemetry/instrumentations/jinja2/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_server.py
+Filename: lumigo_opentelemetry/instrumentations/kafka/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/kafka_python/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/mysql/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/instrumentations/pika/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/pymongo/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/psycopg2/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/pymysql/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/pymemcache/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/instrumentations/requests/__init__.py
-Comment: 
-
-Filename: lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/pymongo/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/libs/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/pymysql/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/libs/general_utils.py
+Filename: lumigo_opentelemetry/instrumentations/pyramid/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/libs/json_utils.py
+Filename: lumigo_opentelemetry/instrumentations/redis/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/resources/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/requests/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/resources/detectors.py
+Filename: lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/utils/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/sklearn/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/utils/aws_utils.py
+Filename: lumigo_opentelemetry/instrumentations/sqlite3/__init__.py
 Comment: 
 
-Filename: lumigo_opentelemetry/utils/config.py
+Filename: lumigo_opentelemetry/instrumentations/tornado/__init__.py
 Comment: 
 
-Filename: test/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/urllib/__init__.py
 Comment: 
 
-Filename: test/ci/__init__.py
+Filename: lumigo_opentelemetry/instrumentations/urllib3/__init__.py
 Comment: 
 
-Filename: test/ci/test_tested_versions.py
+Filename: lumigo_opentelemetry/libs/__init__.py
 Comment: 
 
-Filename: test/components/__init__.py
+Filename: lumigo_opentelemetry/libs/general_utils.py
 Comment: 
 
-Filename: test/components/app/__init__.py
+Filename: lumigo_opentelemetry/libs/json_utils.py
 Comment: 
 
-Filename: test/components/fastapi_external_apis/__init__.py
+Filename: lumigo_opentelemetry/resources/__init__.py
 Comment: 
 
-Filename: test/components/fastapi_external_apis/app.py
+Filename: lumigo_opentelemetry/resources/detectors.py
 Comment: 
 
-Filename: test/components/tests/__init__.py
+Filename: lumigo_opentelemetry/utils/__init__.py
 Comment: 
 
-Filename: test/components/tests/test_attr_max_size.py
+Filename: lumigo_opentelemetry/utils/aws_utils.py
 Comment: 
 
-Filename: test/components/tests/test_execution_tags.py
+Filename: test/__init__.py
 Comment: 
 
 Filename: test/integration/__init__.py
 Comment: 
 
 Filename: test/integration/conftest.py
 Comment: 
@@ -195,65 +180,14 @@
 
 Filename: test/integration/flask/tests/__init__.py
 Comment: 
 
 Filename: test/integration/flask/tests/test_flask.py
 Comment: 
 
-Filename: test/integration/grpcio/__init__.py
-Comment: 
-
-Filename: test/integration/grpcio/app/__init__.py
-Comment: 
-
-Filename: test/integration/grpcio/app/greeter_server.py
-Comment: 
-
-Filename: test/integration/grpcio/app/helloworld_pb2.py
-Comment: 
-
-Filename: test/integration/grpcio/app/helloworld_pb2_grpc.py
-Comment: 
-
-Filename: test/integration/grpcio/tests/__init__.py
-Comment: 
-
-Filename: test/integration/grpcio/tests/test_grpcio.py
-Comment: 
-
-Filename: test/integration/kafka_python/__init__.py
-Comment: 
-
-Filename: test/integration/kafka_python/conftest.py
-Comment: 
-
-Filename: test/integration/kafka_python/app/__init__.py
-Comment: 
-
-Filename: test/integration/kafka_python/tests/__init__.py
-Comment: 
-
-Filename: test/integration/kafka_python/tests/test_kafka_python.py
-Comment: 
-
-Filename: test/integration/pika/__init__.py
-Comment: 
-
-Filename: test/integration/pika/conftest.py
-Comment: 
-
-Filename: test/integration/pika/app/__init__.py
-Comment: 
-
-Filename: test/integration/pika/tests/__init__.py
-Comment: 
-
-Filename: test/integration/pika/tests/test_pika.py
-Comment: 
-
 Filename: test/integration/pymongo/__init__.py
 Comment: 
 
 Filename: test/integration/pymongo/conftest.py
 Comment: 
 
 Filename: test/integration/pymongo/app/__init__.py
@@ -282,26 +216,26 @@
 
 Filename: test/test_utils/__init__.py
 Comment: 
 
 Filename: test/test_utils/spans_parser.py
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.89.dist-info/LICENSE
+Filename: lumigo_opentelemetry-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.89.dist-info/METADATA
+Filename: lumigo_opentelemetry-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.89.dist-info/WHEEL
+Filename: lumigo_opentelemetry-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.89.dist-info/entry_points.txt
+Filename: lumigo_opentelemetry-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.89.dist-info/top_level.txt
+Filename: lumigo_opentelemetry-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.89.dist-info/RECORD
+Filename: lumigo_opentelemetry-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ci/tested_versions_utils.py

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import attr
 import os
 import re
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import List, Optional, Union, cast, Any, Generator
+from typing import List, Optional, Union, cast
 
 # This regexp splits the version line across three capture groups:
 # `(!)?` captures whether or not the version is supported (if supported, the `!` character is missing)
 # `([^\s]+)` represents the actual version, as it is a list of non-whitespace characters
 # `(.*)` is the conent of the comment.
 # The various non-capturing groups `(?:\s*)` get rid of whitespace sequences before the ! mark,
 # in between `!` and the version, and in between the version and the (optional) comment, denoted by `#`
@@ -46,52 +46,52 @@
 
 @dataclass(frozen=True, repr=False, order=False)
 class NonSemanticVersion:
     supported: bool
     version: str
     comment: str
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other):
         if not isinstance(other, NonSemanticVersion):
             return False
 
         return self.version == other.version
 
-    def __lt__(self, other: Any) -> bool:
+    def __lt__(self, other):
         if not isinstance(other, NonSemanticVersion):
             return False
 
         return self.version < other.version
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return f"{'' if self.supported else '!'}{self.version}{' # ' + self.comment if self.comment else ''}"
 
 
 @dataclass(frozen=True, repr=False, order=False)
 class SemanticVersion:
     supported: bool
     version: str
     major: int
     minor: int
     patch: int
     suffix: str
     comment: str
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other):
         if not isinstance(other, SemanticVersion):
             return False
 
         return (
             self.major == other.major
             and self.minor == other.minor
             and self.patch == other.patch
             and self.suffix == other.suffix
         )
 
-    def __lt__(self, other: Any) -> bool:
+    def __lt__(self, other):
         if not isinstance(other, SemanticVersion):
             return True
 
         if self.major < other.major:
             return True
 
         if self.major > other.major:
@@ -113,15 +113,15 @@
             return True
 
         if self.suffix and not other.suffix:
             return False
 
         return self.suffix < other.suffix
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return f"{'' if self.supported else '!'}{self.version}{' # ' + self.comment if self.comment else ''}"
 
 
 def parse_version(version: str) -> Union[SemanticVersion, NonSemanticVersion]:
     res = re.search(_SPLIT_VERSION_FROM_COMMENT_PATTERN, version)
     if not res:
         raise Exception(f"Version does not parse as non-semantic: {version}")
@@ -155,22 +155,22 @@
     versions: List[Union[SemanticVersion, NonSemanticVersion]] = attr.ib(
         converter=sorted
     )
 
     @staticmethod
     def _add_version_to_file(
         directory: str, dependency_name: str, dependency_version: str, supported: bool
-    ) -> None:
+    ):
         dependency_file_path = TestedVersions.get_file_path(directory, dependency_name)
         TestedVersions.add_version_to_file(
             dependency_file_path, dependency_version, supported
         )
 
     @staticmethod
-    def add_version_to_file(path: str, version: str, supported: bool) -> None:
+    def add_version_to_file(path: str, version: str, supported: bool):
         tested_versions = TestedVersions.from_file(path)
 
         parsed_version = parse_version(("" if supported else "!") + version)
         previous_version: Optional[Union[SemanticVersion, NonSemanticVersion]] = None
 
         try:
             previous_version = next(
@@ -210,15 +210,15 @@
 
                 f.write("\n")
 
     @staticmethod
     @contextmanager
     def save_tests_result(
         directory: str, dependency_name: str, dependency_version: str
-    ) -> Generator[None, None, None]:
+    ):
         if should_test_only_untested_versions():
             try:
                 yield
             except Exception:
                 TestedVersions._add_version_to_file(
                     directory, dependency_name, dependency_version, False
                 )
@@ -267,16 +267,15 @@
 
 
 def should_test_only_untested_versions() -> bool:
     return os.getenv("TEST_ONLY_UNTESTED_NEW_VERSIONS", "").lower() == "true"
 
 
 def generate_support_matrix_markdown(
-    src_root: Optional[str] = None,
-    package_url_template: str = "https://pypi.org/project/{}",
+    src_root=None, package_url_template="https://pypi.org/project/{}"
 ) -> List[str]:
     project_root = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
 
     if src_root:
         project_root = os.path.join(project_root, src_root)
 
     # Find all the 'tested_versions' folders and the files inside
@@ -294,15 +293,15 @@
             package_support_version_directory, package_url_template
         )
 
     return res
 
 
 def _generate_support_matrix_markdown_row(
-    tested_versions_directory: str, package_url_template: str
+    tested_versions_directory, package_url_template
 ) -> List[str]:
     """Generate the markdown row for an instrumentation"""
 
     # The package name is the name of the parent of the 'tested_versions' directory
     # But there are cases, like FastAPI, where we actually test multiple packages,
     # like fastapi and uvicorn
     instrumentation = os.path.basename(os.path.dirname(tested_versions_directory))
```

## lumigo_opentelemetry/VERSION

```diff
@@ -1 +1 @@
-1.0.89
+1.0.9
```

## lumigo_opentelemetry/__init__.py

```diff
@@ -1,44 +1,31 @@
 from __future__ import annotations
 
 import logging
 import os
-from typing import Any, Callable, TypeVar, Dict, List
 
-LOG_FORMAT = "#LUMIGO# - %(asctime)s - %(levelname)s - %(message)s"
 
-T = TypeVar("T")
+LOG_FORMAT = "#LUMIGO# - %(asctime)s - %(levelname)s - %(message)s"
 
 
-def _setup_logger(logger_name: str = "lumigo-opentelemetry") -> logging.Logger:
+def _setup_logger(logger_name="lumigo-opentelemetry"):
     """
     This function returns Lumigo's logger. The Lumigo logger prints to stderr.
     The Lumigo logger is set to INFO by default. If the environment variable
     `LUMIGO_DEBUG=true` is set, the severity is set to DEBUG.
     """
     _logger = logging.getLogger(logger_name)
     _logger.propagate = False
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter(LOG_FORMAT))
     if os.environ.get("LUMIGO_DEBUG", "").lower() == "true":
         _logger.setLevel(logging.DEBUG)
     else:
         _logger.setLevel(logging.INFO)
     _logger.addHandler(handler)
-
-    # Suppress spurious warnings when the application is not running on ECS
-    logging.getLogger("opentelemetry.sdk.extension.aws.resource.ecs").setLevel(
-        logging.CRITICAL
-    )
-
-    # Suppress spurious warnings when the application is not running on EKS
-    logging.getLogger("opentelemetry.sdk.extension.aws.resource.eks").setLevel(
-        logging.CRITICAL
-    )
-
     return _logger
 
 
 logger = _setup_logger()
 
 
 def _get_lumigo_opentelemetry_version() -> str:
@@ -49,107 +36,75 @@
         logger.exception("failed getting lumigo_opentelemetry version", exc_info=err)
         return "unknown"
 
 
 __version__ = _get_lumigo_opentelemetry_version()
 
 
-def auto_load(_: Any) -> None:
+def auto_load(_):
     """
     Called when injection performed over `AUTOWRAPT_BOOTSTRAP`.
     """
     # Some versions of Python have issues with the 'argv' attribute when
     # auto-loading the tracer. See https://bugs.python.org/issue32573
     import sys
 
     if not hasattr(sys, "argv"):
         sys.argv = [""]
 
     # We do not need to init the package, it will happen automatically due
     # to the init() call at the end of this file.
 
 
-def init() -> Dict[str, Any]:
+def init():
     if str(os.environ.get("LUMIGO_SWITCH_OFF", False)).lower() == "true":
         logger.info(
             "Lumigo OpenTelemetry distribution disabled via the 'LUMIGO_SWITCH_OFF' environment variable"
         )
-        return {}
+        return
 
     # Multiple packages are passed to autowrapt in comma-separated form
     if "lumigo_opentelemetry" in os.getenv("AUTOWRAPT_BOOTSTRAP", "").split(","):
         activation_mode = "automatic injection"
     else:
         activation_mode = "import"
 
     logger.info(
-        f"Loading the Lumigo OpenTelemetry distribution v{__version__} (injection mode: %s)",
+        "Loading the Lumigo OpenTelemetry distribution (injection mode: %s)",
         activation_mode,
     )
 
     from opentelemetry import trace
     from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
-    from opentelemetry.sdk.trace import SpanLimits, TracerProvider
+    from opentelemetry.sdk.trace import TracerProvider
     from opentelemetry.sdk.trace.export import BatchSpanProcessor
 
     DEFAULT_LUMIGO_ENDPOINT = (
         "https://ga-otlp.lumigo-tracer-edge.golumigo.com/v1/traces"
     )
-    DEFAULT_DEPENDENCIES_ENDPOINT = (
-        "https://ga-otlp.lumigo-tracer-edge.golumigo.com/v1/dependencies"
-    )
     lumigo_endpoint = os.getenv("LUMIGO_ENDPOINT", DEFAULT_LUMIGO_ENDPOINT)
     lumigo_token = os.getenv("LUMIGO_TRACER_TOKEN")
-    lumigo_report_dependencies = os.getenv("LUMIGO_REPORT_DEPENDENCIES", "true").lower()
 
     # Activate instrumentations
     from lumigo_opentelemetry.instrumentations import instrumentations  # noqa
     from lumigo_opentelemetry.instrumentations.instrumentations import framework
     from lumigo_opentelemetry.resources.detectors import get_resource
-    from lumigo_opentelemetry.resources.detectors import (
-        get_infrastructure_resource,
-        get_process_resource,
-    )
-    from lumigo_opentelemetry.libs.general_utils import get_max_size
-
-    infrastructure_resource = get_infrastructure_resource()
-    process_resource = get_process_resource()
 
-    tracer_resource = get_resource(
-        infrastructure_resource, process_resource, {"framework": framework}
-    )
-
-    tracer_provider = TracerProvider(
-        resource=tracer_resource,
-        span_limits=(SpanLimits(max_span_attribute_length=(get_max_size()))),
-    )
+    tracer_resource = get_resource(attributes={"framework": framework})
+    tracer_provider = TracerProvider(resource=tracer_resource)
 
     if lumigo_token:
         tracer_provider.add_span_processor(
             BatchSpanProcessor(
                 OTLPSpanExporter(
                     endpoint=lumigo_endpoint,
                     headers={"Authorization": f"LumigoToken {lumigo_token}"},
                 ),
             )
         )
-
-        if lumigo_report_dependencies == "true":
-            from lumigo_opentelemetry.dependencies import report
-
-            try:
-                report(
-                    DEFAULT_DEPENDENCIES_ENDPOINT,
-                    lumigo_token,
-                    infrastructure_resource.attributes,
-                )
-            except Exception as e:
-                logger.debug("Cannot report dependencies to Lumigo", exc_info=e)
-        else:
-            logger.debug("Dependency reporting is turned off")
     else:
         logger.warning(
             "Lumigo token not provided (env var 'LUMIGO_TRACER_TOKEN' not set); "
             "no data will be sent to Lumigo"
         )
 
     spandump_file = os.getenv("LUMIGO_DEBUG_SPANDUMP")
@@ -171,35 +126,31 @@
             )
         )
 
         logger.debug("Storing a copy of the trace data under: %s", spandump_file)
 
     trace.set_tracer_provider(tracer_provider)
 
-    return {"tracer_provider": tracer_provider}
-
 
-def lumigo_wrapped(func: Callable[..., T]) -> Callable[..., T]:
+def lumigo_wrapped(func):
     CONTEXT_NAME = "lumigo"
     PARENT_IDENTICATOR = "LumigoRoot"
 
     from opentelemetry import trace
     from lumigo_opentelemetry.libs.json_utils import dump
 
-    def wrapper(*args: List[Any], **kwargs: Dict[Any, Any]) -> T:
+    def wrapper(*args, **kwargs):
         tracer = trace.get_tracer_provider().get_tracer(CONTEXT_NAME)
         with tracer.start_as_current_span(PARENT_IDENTICATOR) as span:
             span.set_attribute("input_args", dump(args))
             span.set_attribute("input_kwargs", dump(kwargs))
             return_value = func(*args, **kwargs)
             span.set_attribute("return_value", dump(return_value))
             return return_value
 
     return wrapper
 
 
-# Load the package on import
-init_data = init()
+__all__ = ["auto_load", "init", "lumigo_wrapped", "logger"]
 
-tracer_provider = init_data.get("tracer_provider")
-
-__all__ = ["auto_load", "init", "lumigo_wrapped", "logger", "tracer_provider"]
+# Load the package on import
+init()
```

## lumigo_opentelemetry/instrumentations/__init__.py

```diff
@@ -9,18 +9,18 @@
     # TODO Implement lookup of package versions based on the file-based version ranges we validate
 
     @abstractmethod
     def __init__(self, instrumentation_id: str):
         self._instrumentation_id = instrumentation_id
 
     @abstractmethod
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         # TODO Implement version lookup per instrumented package, and check that the version is supported
         raise Exception("'check_if_applicable' method not implemented!")
 
     @abstractmethod
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         raise Exception("'apply_instrumentation' method not implemented!")
 
     @property
     def instrumentation_id(self) -> str:
         return self._instrumentation_id
```

## lumigo_opentelemetry/instrumentations/instrumentations.py

```diff
@@ -1,34 +1,30 @@
 from typing import List
 
 from lumigo_opentelemetry import logger
 
+
 # Instrumentations
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 
 from .boto import instrumentor as boto_instrumentor
 from .botocore import instrumentor as botocore_instrumentor
 from .fastapi import instrumentor as fastapi_instrumentor
 from .flask import instrumentor as flask_instrumentor
-from .grpcio import instrumentor as grpc_instrumentor
-from .kafka_python import instrumentor as kafka_python_instrumentor
-from .pika import instrumentor as pika_instrumentor
 from .pymongo import instrumentor as pymongo_instrumentor
 from .pymysql import instrumentor as pymysql_instrumentor
 from .requests import instrumentor as requests_instrumentor
 
+
 installed_instrumentations: List[str] = []
 instrumentors: List[AbstractInstrumentor] = [
     boto_instrumentor,
     botocore_instrumentor,
     fastapi_instrumentor,
     flask_instrumentor,
-    grpc_instrumentor,
-    kafka_python_instrumentor,
-    pika_instrumentor,
     pymongo_instrumentor,
     pymysql_instrumentor,
     requests_instrumentor,
 ]
 for instrumentor in instrumentors:
     try:
         instrumentor.check_if_applicable()
```

## lumigo_opentelemetry/instrumentations/boto/__init__.py

```diff
@@ -1,17 +1,17 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 
 
 class BotoInstrumentorWrapper(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("boto")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         import boto  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         from opentelemetry.instrumentation.boto import BotoInstrumentor
 
         BotoInstrumentor().instrument()
 
 
 instrumentor: AbstractInstrumentor = BotoInstrumentorWrapper()
```

## lumigo_opentelemetry/instrumentations/botocore/__init__.py

```diff
@@ -1,27 +1,22 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 from lumigo_opentelemetry.instrumentations.botocore.parsers import AwsParser
 
 
 class BotoCoreInstrumentorWrapper(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("botocore")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         from botocore.client import BaseClient  # noqa
         from botocore.endpoint import Endpoint  # noqa
         from botocore.exceptions import ClientError  # noqa
 
-    def install_instrumentation(self) -> None:
-        # We're using a copied version of this instrumentor until this PR will be merged:
-        # https://github.com/open-telemetry/opentelemetry-python-contrib/pull/1350
-        # After the merge, delete the following line and uncomment the next line
-        from lumigo_opentelemetry.external.botocore import BotocoreInstrumentor
-
-        # from opentelemetry.instrumentation.botocore import BotocoreInstrumentor
+    def install_instrumentation(self):
+        from opentelemetry.instrumentation.botocore import BotocoreInstrumentor
 
         BotocoreInstrumentor().instrument(
             request_hook=AwsParser.request_hook,
             response_hook=AwsParser.response_hook,
         )
```

## lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 
-import json
-from typing import Optional, Type, Dict, Any
+from typing import Optional, Type, Dict
 
 from opentelemetry.trace import Span
-from lumigo_core.triggers.event_trigger import parse_triggers
 
 from lumigo_opentelemetry.libs.general_utils import lumigo_safe_execute
-from lumigo_opentelemetry.libs.json_utils import dump_with_context
+from lumigo_opentelemetry.libs.json_utils import dump
 from lumigo_opentelemetry.utils.aws_utils import (
     extract_region_from_arn,
     get_resource_fullname,
 )
 
 
 class AwsParser:
@@ -25,83 +23,81 @@
             "lambda": LambdaParser,
             "dynamodb": DynamoParser,
         }
         return parsers.get(service_name, AwsParser)
 
     @staticmethod
     def parse_request(
-        span: Span, service_name: str, operation_name: str, api_params: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, api_params: dict
     ) -> None:
         attributes = {
-            "http.request.body": dump_with_context("requestBody", api_params),
+            "http.request.body": dump(api_params),
             "aws.service": service_name,
             "http.method": operation_name,
         }
         span.set_attributes(attributes)
 
     @staticmethod
     def request_hook(
-        span: Span, service_name: str, operation_name: str, api_params: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, api_params: dict
     ) -> None:
         with lumigo_safe_execute("aws: request_hook"):
             parser = AwsParser.get_parser(service_name=service_name)
             parser.parse_request(
                 span=span,
                 service_name=service_name,
                 operation_name=operation_name,
                 api_params=api_params,
             )
 
     @staticmethod
     def parse_response(
-        span: Span, service_name: str, operation_name: str, result: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, result: dict
     ) -> None:
         headers = result.get("ResponseMetadata", {}).get("HTTPHeaders", {})
         attributes = {
-            "http.response.body": dump_with_context("responseBody", result),
-            "http.response.headers": dump_with_context("responseHeaders", headers),
+            "http.response.body": dump(result),
+            "http.response.headers": dump(headers),
             "http.status_code": result.get("ResponseMetadata", {}).get(
                 "HTTPStatusCode", ""
             ),
             "messageId": result.get("MessageId")
             or headers.get("x-amzn-requestid")
             or headers.get("x-amz-requestid", ""),
         }
         span.set_attributes(attributes)
 
     @staticmethod
     def response_hook(
-        span: Span, service_name: str, operation_name: str, result: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, result: dict
     ) -> None:
         with lumigo_safe_execute("aws: response_hook"):
             parser = AwsParser.get_parser(service_name=service_name)
             parser.parse_response(
                 span=span,
                 service_name=service_name,
                 operation_name=operation_name,
                 result=result,
             )
 
 
 class SnsParser(AwsParser):
     @staticmethod
-    def safe_extract_arn(api_params: Dict[Any, Any]) -> Optional[str]:
+    def safe_extract_arn(api_params: dict) -> Optional[str]:
         return api_params.get("TargetArn")
 
     @staticmethod
     def parse_request(
-        span: Span, service_name: str, operation_name: str, api_params: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, api_params: dict
     ) -> None:
         arn = SnsParser.safe_extract_arn(api_params=api_params)
         region = extract_region_from_arn(arn=arn) if arn else None
 
         attributes = {
-            "http.request.body": dump_with_context(
-                "requestBody", api_params.get("Message", api_params or {})
-            ),
+            "http.request.body": dump(api_params.get("Message", api_params or {})),
             "aws.service": service_name,
             "region": region or "",
             "http.method": operation_name,
             "http.url": f"https://{service_name.lower()}.{region}.amazonaws.com",
             "aws.resource.name": get_resource_fullname(arn) if arn else "",
         }
         span.set_attributes(attributes)
@@ -110,69 +106,51 @@
 class SqsParser(AwsParser):
     @staticmethod
     def extract_queue_name_from_url(queue_url: str) -> str:
         return queue_url.split("/")[-1]
 
     @staticmethod
     def parse_request(
-        span: Span, service_name: str, operation_name: str, api_params: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, api_params: dict
     ) -> None:
         queue_url = api_params.get("QueueUrl")
         resource_name = (
             SqsParser.extract_queue_name_from_url(queue_url=queue_url)
             if queue_url
             else None
         )
         attributes = {
-            "http.request.body": dump_with_context(
-                "requestBody", api_params.get("MessageBody", api_params or {})
-            ),
+            "http.request.body": dump(api_params.get("MessageBody", api_params or {})),
             "aws.service": service_name,
             "http.method": operation_name,
             "http.url": queue_url or "",
             "aws.resource.name": resource_name or "",
         }
         span.set_attributes(attributes)
 
-    @staticmethod
-    def parse_response(
-        span: Span, service_name: str, operation_name: str, result: Dict[Any, Any]
-    ) -> None:
-        trigger_details = parse_triggers(
-            {"service_name": service_name, "operation_name": operation_name, **result}
-        )
-        if trigger_details:
-            span.set_attributes(
-                {"lumigoData": json.dumps({"trigger": trigger_details})}
-            )
-
 
 class LambdaParser(AwsParser):
     @staticmethod
     def parse_request(
-        span: Span, service_name: str, operation_name: str, api_params: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, api_params: dict
     ) -> None:
-        resource_name = api_params.get("FunctionName")
         attributes = {
-            "http.request.body": dump_with_context(
-                "requestBody", api_params.get("Payload", api_params or {})
-            ),
-            "aws.resource.name": resource_name or "",
+            "http.request.body": dump(api_params.get("Payload", api_params or {})),
             "aws.service": service_name,
             "http.method": operation_name,
         }
         span.set_attributes(attributes)
 
 
 class DynamoParser(AwsParser):
     @staticmethod
     def parse_request(
-        span: Span, service_name: str, operation_name: str, api_params: Dict[Any, Any]
+        span: Span, service_name: str, operation_name: str, api_params: dict
     ) -> None:
         attributes = {
-            "http.request.body": dump_with_context("requestBody", api_params),
+            "http.request.body": dump(api_params),
             "aws.service": service_name,
             "http.method": operation_name,
             "aws.resource.name": api_params.get("TableName", ""),
             "aws.dynamodb.method": operation_name,
         }
         span.set_attributes(attributes)
```

## lumigo_opentelemetry/instrumentations/fastapi/__init__.py

```diff
@@ -1,25 +1,25 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 from .parsers import FastAPIParser
 
 
 class FastApiInstrumentorWrapper(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("fast-api")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         import fastapi  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         import wrapt
 
         from lumigo_opentelemetry import logger
 
         @wrapt.patch_function_wrapper("fastapi", "FastAPI.__init__")
-        def init_otel_middleware(wrapped, instance, args, kwargs):  # type: ignore
+        def init_otel_middleware(wrapped, instance, args, kwargs):
             try:
                 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 
                 return_value = wrapped(*args, **kwargs)
                 FastAPIInstrumentor().instrument_app(
                     instance,
                     server_request_hook=FastAPIParser.server_request_hook,
```

## lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py

```diff
@@ -1,58 +1,49 @@
 from typing import Dict, Any
 
 from lumigo_opentelemetry import logger
 from lumigo_opentelemetry.libs.general_utils import lumigo_safe_execute
-from lumigo_opentelemetry.libs.json_utils import (
-    dump,
-    safe_convert_bytes_to_string,
-    dump_with_context,
-)
+from lumigo_opentelemetry.libs.json_utils import dump, safe_convert_bytes_to_string
 
 from opentelemetry.trace import Span
 
 
 class FastAPIParser:
     @staticmethod
     def safe_extract_headers_bytes(headers: Any) -> Dict[str, str]:
         with lumigo_safe_execute("safe_extract_headers_bytes"):
             return {
                 key.decode("utf-8"): value.decode("utf-8") for key, value in headers
             }
         return {}
 
     @staticmethod
-    def server_request_hook(span: Span, scope: Dict[str, Any]) -> None:
+    def server_request_hook(span: Span, scope: dict):
         with lumigo_safe_execute("FastAPIParser: server_request_hook"):
             headers = FastAPIParser.safe_extract_headers_bytes(
                 headers=scope.get("headers", [])
             )
             query_string = scope.get("query_string", "")
             path = scope.get("path", "")
             attributes = {
-                "http.request.headers": dump_with_context("requestHeaders", headers),
+                "http.request.headers": dump(headers),
                 "http.request.query_string": dump(query_string),
                 "http.request.path": dump(path),
             }
             span.set_attributes(attributes)
 
     @staticmethod
-    def client_request_hook(span: Span, scope: Dict[Any, Any]) -> None:
+    def client_request_hook(span: Span, scope: dict):
         with lumigo_safe_execute("FastAPIParser: client_request_hook"):
             logger.debug(f"client_request_hook span: {span}, scope: {scope}")
 
     @staticmethod
-    def client_response_hook(span: Span, message: Dict[str, Any]) -> None:
+    def client_response_hook(span: Span, message: dict):
         with lumigo_safe_execute("FastAPIParser: client_response_hook"):
             body = safe_convert_bytes_to_string(message.get("body"))
             if body:
-                span.set_attribute(
-                    "http.response.body", dump_with_context("responseBody", body)
-                )
+                span.set_attribute("http.response.body", dump(body))
             headers = FastAPIParser.safe_extract_headers_bytes(
                 headers=message.get("headers", [])
             )
             if headers:
-                span.set_attribute(
-                    "http.response.headers",
-                    dump_with_context("responseHeaders", headers),
-                )
+                span.set_attribute("http.response.headers", dump(headers))
```

## lumigo_opentelemetry/instrumentations/flask/__init__.py

```diff
@@ -1,23 +1,23 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 
 
 class FlaskInstrumentorWrapper(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("flask")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         import flask  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         import wrapt
         from lumigo_opentelemetry import logger
 
         @wrapt.patch_function_wrapper("flask", "Flask.__init__")
-        def init_otel_flask_instrumentation(wrapped, instance, args, kwargs):  # type: ignore
+        def init_otel_flask_instrumentation(wrapped, instance, args, kwargs):
             try:
                 from opentelemetry.instrumentation.flask import FlaskInstrumentor
 
                 return_value = wrapped(*args, **kwargs)
                 FlaskInstrumentor().instrument_app(instance)
                 return return_value
             except Exception as e:
```

## lumigo_opentelemetry/instrumentations/pika/__init__.py

```diff
@@ -1,17 +1,17 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 
 
-class PikaInstrumentor(AbstractInstrumentor):
-    def __init__(self) -> None:
+class PikaInstrumentorWrapper(AbstractInstrumentor):
+    def __init__(self):
         super().__init__("pika")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         import pika  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         from opentelemetry.instrumentation.pika import PikaInstrumentor
 
         PikaInstrumentor().instrument()
 
 
-instrumentor: AbstractInstrumentor = PikaInstrumentor()
+instrumentor: AbstractInstrumentor = PikaInstrumentorWrapper()
```

## lumigo_opentelemetry/instrumentations/pymongo/__init__.py

```diff
@@ -1,17 +1,17 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 
 
 class PymongoInstrumentor(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("pymongo")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         import pymongo  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         from opentelemetry.instrumentation.pymongo import PymongoInstrumentor
 
         PymongoInstrumentor().instrument()
 
 
 instrumentor: AbstractInstrumentor = PymongoInstrumentor()
```

## lumigo_opentelemetry/instrumentations/pymysql/__init__.py

```diff
@@ -1,17 +1,17 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 
 
 class PyMySqlInstrumentor(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("pymysql")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         import pymysql  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         from opentelemetry.instrumentation.pymysql import PyMySQLInstrumentor
 
         PyMySQLInstrumentor().instrument()
 
 
 instrumentor: AbstractInstrumentor = PyMySqlInstrumentor()
```

## lumigo_opentelemetry/instrumentations/requests/__init__.py

```diff
@@ -1,20 +1,20 @@
 from lumigo_opentelemetry.instrumentations import AbstractInstrumentor
 from .parsers import HttpParser
 
 
 class RequestsInstrumentor(AbstractInstrumentor):
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__("requests")
 
-    def check_if_applicable(self) -> None:
+    def check_if_applicable(self):
         from requests.models import Response  # noqa
         from requests.sessions import Session  # noqa
         from requests.structures import CaseInsensitiveDict  # noqa
 
-    def install_instrumentation(self) -> None:
+    def install_instrumentation(self):
         from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
         RequestsInstrumentor().instrument(span_callback=HttpParser.request_callback)
 
 
 instrumentor: AbstractInstrumentor = RequestsInstrumentor()
```

## lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from typing import Dict, Any
 from requests import Response
 
 from opentelemetry.trace import Span
 
 from lumigo_opentelemetry.libs.general_utils import lumigo_safe_execute
-from lumigo_opentelemetry.libs.json_utils import dump_with_context
+from lumigo_opentelemetry.libs.json_utils import dump
 
 
 @dataclass(frozen=True)
 class HttpParser:
     response: Response
 
     @staticmethod
@@ -22,26 +22,22 @@
             attributes = HttpParser.get_parser(response=response).get_attributes()
 
             span.set_attributes(attributes)
 
     def parse_request(self) -> Dict[str, Any]:
         request = self.response.request
         return {
-            "http.request.body": dump_with_context("requestBody", request.body),
-            "http.request.headers": dump_with_context(
-                "requestHeaders", request.headers
-            ),
+            "http.request.body": dump(request.body),
+            "http.request.headers": dump(request.headers),
         }
 
     def parse_response(self) -> Dict[str, Any]:
         return {
-            "http.response.body": dump_with_context("responseBody", self.response.text),
-            "http.response.headers": dump_with_context(
-                "responseHeaders", self.response.headers
-            ),
+            "http.response.body": dump(self.response.text),
+            "http.response.headers": dump(self.response.headers),
         }
 
     def extract_custom_attributes(self) -> Dict[str, Any]:
         return {}
 
     def get_attributes(self) -> Dict[str, Any]:
         return {
```

## lumigo_opentelemetry/libs/general_utils.py

```diff
@@ -1,72 +1,45 @@
 try:
     from collections import Iterable
 except ImportError:
     # collections.Iterables was removed in Python 3.10
     from collections.abc import Iterable
 
 from contextlib import contextmanager
-from typing import Union, Generator, Optional, TypeVar, List
-import os
+from typing import Union
 
 from lumigo_opentelemetry import logger
 
-from opentelemetry.sdk.environment_variables import (
-    OTEL_SPAN_ATTRIBUTE_VALUE_LENGTH_LIMIT,
-    OTEL_ATTRIBUTE_VALUE_LENGTH_LIMIT,
-)
-
-DEFAULT_MAX_ENTRY_SIZE = 2048
-
-T = TypeVar("T")
-
 
 @contextmanager
-def lumigo_safe_execute(part_name: str = "") -> Generator[None, None, None]:
+def lumigo_safe_execute(part_name=""):
     try:
         yield
     except Exception as e:
         logger.exception(
             f"An exception occurred in lumigo's code {part_name}", exc_info=e
         )
 
 
-def safe_split_get(
-    string: str, sep: str, index: int, default: Optional[str] = None
-) -> Optional[str]:
+def safe_split_get(string: str, sep: str, index: int, default=None) -> str:
     """
     This function splits the given string using the sep, and returns the organ in the `index` place.
     If such index doesn't exist, returns default.
     """
     if not isinstance(string, str):
         return default
     return safe_get_list(string.split(sep), index, default)
 
 
-def safe_get_list(
-    lst: List[T], index: Union[int, str], default: Optional[T] = None
-) -> Optional[T]:
+def safe_get_list(lst: list, index: Union[int, str], default=None):
     """
     This function return the organ in the `index` place from the given list.
     If this values doesn't exist, return default.
     """
     if isinstance(index, str):
         try:
             index = int(index)
         except ValueError:
             return default
     if not isinstance(lst, Iterable):
         return default
     return lst[index] if len(lst) > index else default
-
-
-def get_max_size() -> int:
-    """
-    This function return the max size by environment variables.
-    If this values doesn't exist, return default size.
-    """
-    return int(
-        os.environ.get(
-            OTEL_SPAN_ATTRIBUTE_VALUE_LENGTH_LIMIT,
-            os.environ.get(OTEL_ATTRIBUTE_VALUE_LENGTH_LIMIT, DEFAULT_MAX_ENTRY_SIZE),
-        )
-    )
```

## lumigo_opentelemetry/libs/json_utils.py

```diff
@@ -1,38 +1,213 @@
-from typing import Any, Optional, List
-
-from lumigo_opentelemetry.libs.general_utils import get_max_size
-from lumigo_core.scrubbing import lumigo_dumps, lumigo_dumps_with_context
+import json
+import os
+import decimal
+import re
+from collections import OrderedDict
+from decimal import Decimal
+from functools import lru_cache, reduce
+from typing import Any, Optional, List, TypeVar, Pattern, Dict, Tuple
+
+
+TRUNCATE_SUFFIX = "...[too long]"
+LUMIGO_SECRET_MASKING_REGEX = "LUMIGO_SECRET_MASKING_REGEX"
+Container = TypeVar("Container", dict, list)
+EXECUTION_TAGS_KEY = "lumigo_execution_tags_no_scrub"
+SKIP_SCRUBBING_KEYS = [EXECUTION_TAGS_KEY]
+DEFAULT_MAX_ENTRY_SIZE = 2048
+MAX_SIZE = int(os.environ.get("LUMIGO_MAX_ENTRY_SIZE", DEFAULT_MAX_ENTRY_SIZE))
+OMITTING_KEYS_REGEXES = [
+    ".*pass.*",
+    ".*key.*",
+    ".*secret.*",
+    ".*credential.*",
+    "SessionToken",
+    "x-amz-security-token",
+    "Signature",
+    "Authorization",
+]
+
+
+@lru_cache(maxsize=1)
+def get_omitting_regex() -> Optional[Pattern[str]]:
+    if LUMIGO_SECRET_MASKING_REGEX in os.environ:
+        given_regexes = json.loads(os.environ[LUMIGO_SECRET_MASKING_REGEX])
+    else:
+        given_regexes = OMITTING_KEYS_REGEXES
+    if not given_regexes:
+        return None
+    return re.compile(fr"({'|'.join(given_regexes)})", re.IGNORECASE)
+
+
+def _recursive_omitting(
+    prev_result: Tuple[Container, int],
+    item: Tuple[Optional[str], Any],
+    regex: Optional[Pattern[str]],
+    enforce_jsonify: bool,
+    decimal_safe: bool = False,
+    omit_skip_path: Optional[List[str]] = None,
+) -> Tuple[Container, int]:
+    """
+    This function omitting keys until the given max_size.
+    This function should be used in a reduce iteration over dict.items().
+
+    :param prev_result: the reduce result until now: the current dict and the remaining space
+    :param item: the next yield from the iterator dict.items()
+    :param regex: the regex of the keys that we should omit
+    :param enforce_jsonify: should we abort if the object can not be jsonify.
+    :param decimal_safe: should we accept decimal values
+    :return: the intermediate result, after adding the current item (recursively).
+    """
+    key, value = item
+    d, free_space = prev_result
+    if free_space < 0:
+        return d, free_space
+    should_skip_key = False
+    if isinstance(d, dict) and omit_skip_path:
+        should_skip_key = omit_skip_path[0] == key
+        omit_skip_path = omit_skip_path[1:] if should_skip_key else None
+    if key in SKIP_SCRUBBING_KEYS:
+        new_value = value
+        free_space -= (
+            len(value) if isinstance(value, str) else len(aws_dump({key: value}))
+        )
+    elif isinstance(key, str) and regex and regex.match(key) and not should_skip_key:
+        new_value = "****"
+        free_space -= 4
+    elif isinstance(value, (dict, OrderedDict)):
+        new_value, free_space = reduce(
+            lambda p, i: _recursive_omitting(
+                p, i, regex, enforce_jsonify, omit_skip_path=omit_skip_path
+            ),
+            value.items(),
+            ({}, free_space),
+        )
+    elif isinstance(value, decimal.Decimal):
+        new_value = float(value)
+        free_space -= 5
+    elif isinstance(value, list):
+        new_value, free_space = reduce(
+            lambda p, i: _recursive_omitting(
+                p, (None, i), regex, enforce_jsonify, omit_skip_path=omit_skip_path
+            ),
+            value,
+            ([], free_space),
+        )
+    elif isinstance(value, str):
+        new_value = value
+        free_space -= len(new_value)
+    else:
+        try:
+            free_space -= len(aws_dump({key: value}, decimal_safe=decimal_safe))
+            new_value = value
+        except TypeError:
+            if enforce_jsonify:
+                raise
+            new_value = str(value)
+            free_space -= len(new_value)
+    if isinstance(d, list):
+        d.append(new_value)
+    else:
+        d[key] = new_value
+    return d, free_space
+
+
+def omit_keys(
+    value: Dict,
+    in_max_size: Optional[int] = None,
+    regexes: Optional[Pattern[str]] = None,
+    enforce_jsonify: bool = False,
+    decimal_safe: bool = False,
+    omit_skip_path: Optional[List[str]] = None,
+) -> Tuple[Dict, bool]:
+    """
+    This function omit problematic keys from the given value.
+    We do so in the following cases:
+    * if the value is dictionary, then we omit values by keys (recursively)
+    """
+    regexes = regexes or get_omitting_regex()
+    max_size = in_max_size or MAX_SIZE
+    omitted, size = reduce(  # type: ignore
+        lambda p, i: _recursive_omitting(
+            prev_result=p,  # type: ignore
+            item=i,
+            regex=regexes,
+            enforce_jsonify=enforce_jsonify,
+            decimal_safe=decimal_safe,
+            omit_skip_path=omit_skip_path,
+        ),
+        value.items(),
+        ({}, max_size),
+    )
+    return omitted, bool((size or 0) < 0)
 
 
 def dump(
     to_dump: Any,
-    decimal_safe: bool = False,
+    decimal_safe=False,
     omit_skip_path: Optional[List[str]] = None,
     max_size: Optional[int] = None,
     enforce_jsonify: bool = False,
 ) -> str:
-    return lumigo_dumps(  # type: ignore
-        d=to_dump,
-        max_size=max_size or get_max_size(),
-        decimal_safe=decimal_safe,
-        omit_skip_path=omit_skip_path,
-        enforce_jsonify=enforce_jsonify,
+    max_size = max_size or MAX_SIZE
+    is_truncated = False
+
+    if isinstance(to_dump, bytes):
+        try:
+            to_dump = to_dump.decode()
+        except Exception:
+            to_dump = str(to_dump)
+    if isinstance(to_dump, str) and to_dump.startswith("{"):
+        try:
+            to_dump = json.loads(to_dump)
+        except Exception:
+            pass
+    if isinstance(to_dump, dict):
+        to_dump, is_truncated = omit_keys(
+            value=to_dump,
+            decimal_safe=decimal_safe,
+            omit_skip_path=omit_skip_path,
+            enforce_jsonify=enforce_jsonify,
+        )
+    elif isinstance(to_dump, list):
+        size = 0
+        organs = []
+        for a in to_dump:
+            organs.append(dump(a, omit_skip_path=omit_skip_path))
+            size += len(organs[-1])
+            if size > max_size:
+                break
+        return "[" + ", ".join(organs) + "]"
+    try:
+        if isinstance(to_dump, str) and to_dump.endswith(TRUNCATE_SUFFIX):
+            return to_dump
+        retval = aws_dump(to_dump, decimal_safe=decimal_safe)
+    except TypeError:
+        retval = str(to_dump)
+    return (
+        (retval[:max_size] + TRUNCATE_SUFFIX)
+        if len(retval) >= max_size or is_truncated
+        else retval
     )
 
 
-def dump_with_context(
-    context: str,
-    to_dump: Any,
-) -> str:
-    return lumigo_dumps_with_context(  # type: ignore
-        context=context,
-        d=to_dump,
-        max_size=get_max_size(),
-    )
+def aws_dump(d: Any, decimal_safe=False, **kwargs) -> str:
+    if decimal_safe:
+        return json.dumps(d, cls=DecimalEncoder, **kwargs)
+    return json.dumps(d, **kwargs)
+
+
+class DecimalEncoder(json.JSONEncoder):
+    # copied from python's runtime: runtime/lambda_runtime_marshaller.py:7-11
+    def default(self, o):
+        if isinstance(o, Decimal):
+            return float(o)
+        raise TypeError(
+            f"Object of type {o.__class__.__name__} is not JSON serializable"
+        )
 
 
 def safe_convert_bytes_to_string(value: Any) -> Any:
     try:
         return value.decode("utf-8")
     except Exception:
         return value
```

## lumigo_opentelemetry/resources/detectors.py

```diff
@@ -1,35 +1,28 @@
 import json
-import logging
 import os
 import sys
 import urllib.request
-from typing import Any, Dict, Optional
 
 from opentelemetry.sdk.extension.aws.resource.ecs import AwsEcsResourceDetector
-from opentelemetry.sdk.extension.aws.resource.eks import AwsEksResourceDetector
 from opentelemetry.sdk.resources import (
     ResourceDetector,
     Resource,
     PROCESS_RUNTIME_DESCRIPTION,
     PROCESS_RUNTIME_NAME,
     PROCESS_RUNTIME_VERSION,
     OTELResourceDetector,
     get_aggregated_resources,
 )
 from opentelemetry.semconv.resource import ResourceAttributes
 
 import lumigo_opentelemetry
-from lumigo_opentelemetry.libs.json_utils import dump_with_context
-
-logger = logging.getLogger(__name__)
-
+from lumigo_opentelemetry.libs.json_utils import dump
 
 LUMIGO_DISTRO_VERSION_ATTR_NAME = "lumigo.distro.version"
-LUMIGO_TAG_ATTR_NAME = "lumigo.tag"
 ENV_ATTR_NAME = "process.environ"
 
 
 # TODO: ProcessResourceDetector will be part of the next release of opentelemetry-sdk. After the release - delete it.
 class ProcessResourceDetector(ResourceDetector):
     # pylint: disable=no-self-use
     def detect(self) -> "Resource":
@@ -57,58 +50,26 @@
         return Resource(
             {
                 LUMIGO_DISTRO_VERSION_ATTR_NAME: lumigo_opentelemetry.__version__,
             }
         )
 
 
-class LumigoTagDetector(ResourceDetector):
-    def detect(self) -> "Resource":
-        lumigo_tag = os.environ.get("LUMIGO_TAG")
-        if not lumigo_tag:
-            return Resource.get_empty()
-        if ";" in lumigo_tag:
-            logger.warning(
-                "LUMIGO_TAG contains a semicolon, which is not allowed.",
-                extra={"lumigo_tag": lumigo_tag},
-            )
-            return Resource.get_empty()
-        return Resource(
-            {
-                LUMIGO_TAG_ATTR_NAME: lumigo_tag,
-            }
-        )
-
-
-class LumigoContainerNameDetector(ResourceDetector):
-    def detect(self) -> "Resource":
-        container_name = os.environ.get("LUMIGO_CONTAINER_NAME")
-        if not container_name:
-            return Resource.get_empty()
-        return Resource(
-            {
-                ResourceAttributes.K8S_CONTAINER_NAME: container_name,
-            }
-        )
-
-
 class EnvVarsDetector(ResourceDetector):
     def detect(self) -> "Resource":
-        return Resource(
-            {ENV_ATTR_NAME: dump_with_context("environment", dict(os.environ))}
-        )
+        return Resource({ENV_ATTR_NAME: dump(dict(os.environ))})
 
 
 class LumigoAwsEcsResourceDetector(ResourceDetector):
     """Implements the lookup of the `aws.ecs` resource attributes using the Metadata v4 endpoint."""
 
     @staticmethod
-    def _http_get(url: str) -> Dict[Any, Any]:
+    def _http_get(url: str) -> dict:
         with urllib.request.urlopen(url, timeout=1) as response:
-            return json.loads(response.read().decode())  # type: ignore
+            return json.loads(response.read().decode())
 
     def detect(self) -> "Resource":
         metadata_endpoint = os.environ.get("ECS_CONTAINER_METADATA_URI_V4")
 
         if not metadata_endpoint:
             return Resource.get_empty()
 
@@ -135,113 +96,19 @@
                 ResourceAttributes.AWS_ECS_TASK_ARN: task_arn,
                 ResourceAttributes.AWS_ECS_TASK_FAMILY: metadata_task["Family"],
                 ResourceAttributes.AWS_ECS_TASK_REVISION: metadata_task["Revision"],
             }
         )
 
 
-#
-# Kubernetes Pod UUID, based on https://github.com/open-telemetry/opentelemetry-python-contrib/pull/1489
-#
-
-_POD_ID_LENGTH = 36
-_CONTAINER_ID_LENGTH = 64
-
-
-def is_container_on_kubernetes() -> bool:
-    # Kubernetes manages the /etc/hosts file inside the pods' containers,
-    # using a distinctive header, see https://github.com/kubernetes/kubernetes/commit/fd72938dd569bd041f11a76eecfe9b8b4bcf5ae8
-    with open("/etc/hosts", "r", encoding="utf8") as hosts_file:
-        first_line = hosts_file.readline()
-        return first_line.startswith("# Kubernetes-managed hosts file")
-
-
-def get_kubenertes_pod_uid_v1() -> Optional[str]:
-    pod_id = None
-    with open("/proc/self/mountinfo", "r", encoding="utf8") as container_info_file:
-        for raw_line in container_info_file.readlines():
-            line = raw_line.strip()
-            # Subsequent IDs should be the same, exit if found one
-            if len(line) > _POD_ID_LENGTH and "/pods/" in line:
-                pod_id = line.split("/pods/")[1][:_POD_ID_LENGTH]
-                break
-    return pod_id
-
-
-def get_kubenertes_pod_uid_v2() -> Optional[str]:
-    pod_id = None
-    with open("/proc/self/cgroup", "r", encoding="utf8") as container_info_file:
-        for raw_line in container_info_file.readlines():
-            line = raw_line.strip()
-            # Subsequent IDs should be the same, exit if found one
-            if len(line) > _CONTAINER_ID_LENGTH:
-                line_info = line.split("/")
-                if (
-                    len(line_info) > 2
-                    and line_info[-2][:3] == "pod"
-                    and len(line_info[-2]) == _POD_ID_LENGTH + 3
-                ):
-                    pod_id = line_info[-2][3 : 3 + _POD_ID_LENGTH]  # noqa: E203
-                else:
-                    pod_id = line_info[-2]
-                break
-    return pod_id
-
-
-class LumigoKubernetesResourceDetector(ResourceDetector):
-    """Detects attribute values only available when the app is running on kubernetes
-    container and returns a resource object.
-    """
-
-    def detect(self) -> "Resource":
-        if is_container_on_kubernetes():
-            try:
-                pod_uid = get_kubenertes_pod_uid_v1() or get_kubenertes_pod_uid_v2()
-                if pod_uid:
-                    return Resource(
-                        {
-                            ResourceAttributes.K8S_POD_UID: pod_uid,
-                        }
-                    )
-            except Exception as exception:
-                logger.warning(
-                    "Failed to get pod ID on kubernetes container: %s.",
-                    exception,
-                )
-
-        return Resource.get_empty()
-
-
-def get_infrastructure_resource() -> "Resource":
+def get_resource(attributes: dict) -> "Resource":
     return get_aggregated_resources(
         detectors=[
             OTELResourceDetector(),
-            LumigoDistroDetector(),
-            LumigoTagDetector(),
-            LumigoContainerNameDetector(),
-            LumigoAwsEcsResourceDetector(),
-            LumigoKubernetesResourceDetector(),
-            AwsEcsResourceDetector(),
-            AwsEksResourceDetector(),
-        ],
-    )
-
-
-def get_process_resource() -> "Resource":
-    return get_aggregated_resources(
-        detectors=[
             EnvVarsDetector(),
             ProcessResourceDetector(),
+            LumigoDistroDetector(),
+            AwsEcsResourceDetector(),
+            LumigoAwsEcsResourceDetector(),
         ],
-    )
-
-
-def get_resource(
-    infrastructure_resource: "Resource",
-    process_resource: "Resource",
-    attributes: Dict[str, Any],
-) -> "Resource":
-    return (
-        Resource.create(attributes=attributes)
-        .merge(process_resource)
-        .merge(infrastructure_resource)
+        initial_resource=Resource.create(attributes=attributes),
     )
```

## test/integration/boto3/tests/test_boto3.py

```diff
@@ -1,60 +1,58 @@
 import json
+
+import requests
 import time
 import unittest
-from test.test_utils.spans_parser import SpansContainer
 
-import requests
+from test.test_utils.spans_parser import SpansContainer
 
 
 class TestFastApiSpans(unittest.TestCase):
     def assert_is_version(self, version: str):
         major, minor, patch = version.split(".")
         self.assertTrue(major.isdigit())
         self.assertTrue(minor.isdigit())
         self.assertTrue(patch.isdigit())
 
     def assert_have_env_vars(self, root: dict):
-        collected_envs: str = root["resource"]["attributes"]["process.environ"]
+        collected_envs: str = root["resource"]["process.environ"]
         self.assertTrue(isinstance(collected_envs, str))
         self.assertGreaterEqual(len(collected_envs), 1)
         self.assertTrue(
             collected_envs.endswith("...[too long]") or json.loads(collected_envs)
         )
 
     def assert_otel_detector(self, root: dict):
-        self.assertEqual(root["resource"]["attributes"]["K0"], "V0")
-        self.assertEqual(root["resource"]["attributes"]["K1"], "V1")
-        self.assertEqual(root["resource"]["attributes"]["service.name"], "app")
+        self.assertEqual(root["resource"]["K0"], "V0")
+        self.assertEqual(root["resource"]["K1"], "V1")
+        self.assertEqual(root["resource"]["service.name"], "app")
 
     def test_boto3_instrumentation(self):
         response = requests.post("http://localhost:8001/invoke-boto3")
 
         response.raise_for_status()
 
         body = response.json()
 
         self.assertEqual(body, {"status": "ok"})
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
         self.assertEqual(4, len(spans_container.spans))
 
         # assert root
         root = spans_container.get_root()
         self.assertEqual(root["attributes"]["http.method"], "POST")
-        self.assertEqual(
-            root["resource"]["attributes"]["process.runtime.name"], "cpython"
-        )
-        self.assertTrue(
-            root["resource"]["attributes"]["process.runtime.version"].startswith("3.")
-        )
-        self.assert_is_version(root["resource"]["attributes"]["lumigo.distro.version"])
+        self.assertEqual(root["resource"]["process.runtime.name"], "cpython")
+        self.assertTrue(root["resource"]["process.runtime.version"].startswith("3."))
+        self.assert_is_version(root["resource"]["process.runtime.version"])
+        self.assert_is_version(root["resource"]["lumigo.distro.version"])
         self.assert_have_env_vars(root)
         self.assert_otel_detector(root)
 
         # assert child spans
         children = spans_container.get_non_internal_children()
         self.assertEqual(1, len(children))
         self.assertIsNotNone(children[0]["attributes"]["aws.service"])
```

## test/integration/fastapi/app/__init__.py

```diff
@@ -1,24 +1,16 @@
 import requests
 from fastapi import FastAPI
 
+
 app = FastAPI()
 
 
 @app.get("/")
 async def root():
     return {"message": "Hello FastAPI!"}
 
 
 @app.get("/invoke-requests")
 def invoke_requests():
     response = requests.get("https://api.chucknorris.io/jokes/random")
     return response.json()
-
-
-@app.get("/invoke-requests-large-response")
-def invoke_requests_big_response():
-    response = requests.get(
-        "http://universities.hipolabs.com/search?country=United+States"
-    )
-    response.raise_for_status()
-    return response.json()
```

## test/integration/fastapi/tests/test_fastapi.py

```diff
@@ -1,25 +1,25 @@
+import requests
 import time
 import unittest
-from test.test_utils.spans_parser import SpansContainer
 
-import requests
+from test.test_utils.spans_parser import SpansContainer
 
 
 class TestFastApiSpans(unittest.TestCase):
     def test_200_OK(self):
         response = requests.get("http://localhost:8000/")
         response.raise_for_status()
 
         body = response.json()
 
         self.assertEqual(body, {"message": "Hello FastAPI!"})
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
         self.assertEqual(3, len(spans_container.spans))
 
         # assert root
         root = spans_container.get_root()
         self.assertIsNotNone(root)
@@ -47,15 +47,15 @@
         response.raise_for_status()
 
         body = response.json()
 
         self.assertIn("https://api.chucknorris.io/jokes/", body["url"])
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
         self.assertEqual(4, len(spans_container.spans))
 
         # assert root
         root = spans_container.get_root()
         self.assertIsNotNone(root)
@@ -73,47 +73,7 @@
             children[0]["attributes"]["http.url"],
             "https://api.chucknorris.io/jokes/random",
         )
         self.assertEqual(children[0]["attributes"]["http.status_code"], 200)
         self.assertIsNotNone(children[0]["attributes"]["http.request.headers"])
         self.assertIsNotNone(children[0]["attributes"]["http.response.headers"])
         self.assertIsNotNone(children[0]["attributes"]["http.response.body"])
-
-    def test_large_span_attribute_size_default_max_size(self):
-        response = requests.get("http://localhost:8000/invoke-requests-large-response")
-        response.raise_for_status()
-
-        body = response.json()
-
-        assert body is not None
-
-        # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
-
-        spans_container = SpansContainer.get_spans_from_file()
-        self.assertEqual(4, len(spans_container.spans))
-
-        # assert root
-        root = spans_container.get_root()
-        self.assertIsNotNone(root)
-        root_attributes = root["attributes"]
-        self.assertEqual(root_attributes["http.status_code"], 200)
-        self.assertEqual(
-            root_attributes["http.url"],
-            "http://127.0.0.1:8000/invoke-requests-large-response",
-        )
-        self.assertEqual(root_attributes["http.method"], "GET")
-
-        # assert child spans
-        children = spans_container.get_non_internal_children()
-        self.assertEqual(1, len(children))
-        children_attributes = children[0]["attributes"]
-        self.assertEqual(children_attributes["http.method"], "GET")
-        self.assertEqual(
-            children_attributes["http.url"],
-            "http://universities.hipolabs.com/search?country=United+States",
-        )
-        self.assertEqual(len(children_attributes["http.response.body"]), 2048)
-        self.assertEqual(children_attributes["http.status_code"], 200)
-        self.assertIsNotNone(children_attributes["http.request.headers"])
-        self.assertIsNotNone(children_attributes["http.response.headers"])
-        self.assertIsNotNone(children_attributes["http.response.body"])
```

## test/integration/flask/tests/test_flask.py

```diff
@@ -1,25 +1,26 @@
-import time
 import unittest
-from test.test_utils.spans_parser import SpansContainer
 
 import requests
+import time
+
+from test.test_utils.spans_parser import SpansContainer
 
 
 class TestFlaskSpans(unittest.TestCase):
     def test_200_OK(self):
         response = requests.get("http://localhost:5000/")
         response.raise_for_status()
 
         body = response.json()
 
         self.assertEqual(body, {"message": "Hello Flask!"})
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
         self.assertEqual(1, len(spans_container.spans))
 
         # assert root
         root = spans_container.get_root()
         self.assertIsNotNone(root)
@@ -34,15 +35,15 @@
         response.raise_for_status()
 
         body = response.json()
 
         self.assertIn("https://api.chucknorris.io/jokes/", body["url"])
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
         self.assertEqual(2, len(spans_container.spans))
 
         # assert root
         root = spans_container.get_root()
         self.assertIsNotNone(root)
```

## test/integration/pymongo/app/__init__.py

```diff
@@ -1,35 +1,24 @@
 from fastapi import FastAPI
-from pymongo import MongoClient
 from testcontainers.mongodb import MongoDbContainer
 
 
 app = FastAPI()
 
 
 @app.get("/")
 async def root():
     return {"message": "Hello FastAPI!"}
 
 
 @app.get("/invoke-mongo")
 def invoke_mongo():
-    # Using MongoDB 4 as not to have issues with retired opscodes.
-    with MongoDbContainer("mongo:4") as mongo:
-        mongo.get_connection_client().test  # Wait that is is connected
-
-        db = MongoClient(mongo.get_connection_url()).test
-
+    with MongoDbContainer() as mongo:
+        db = mongo.get_connection_client().test
         doc = {
             "address": {
                 "street": "2 Avenue",
             },
             "restaurant_id": "41704620",
         }
-
-        result = db.items.insert_one(doc)
-
-        assert result.acknowledged
-
-        assert db.items.find_one() == doc
-
+        db.items.insert_one(doc)
     return {"status": "ok"}
```

## test/integration/pymongo/tests/test_pymongo.py

```diff
@@ -1,40 +1,27 @@
+import requests
 import time
 import unittest
-from test.test_utils.spans_parser import SpansContainer
 
-import requests
+from test.test_utils.spans_parser import SpansContainer
 
 
 class TestFastApiSpans(unittest.TestCase):
     def test_mongo_instrumentation(self):
         response = requests.get("http://localhost:8002/invoke-mongo")
 
         response.raise_for_status()
 
         body = response.json()
 
         self.assertEqual(body, {"status": "ok"})
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
 
         # assert mongo children spans
-        assert spans_container.find_child_span(
-            lambda span: (
-                span["kind"] == "SpanKind.CLIENT"
-                and span["attributes"]["db.system"] == "mongodb"
-                and span["attributes"]["db.name"] == "test"
-                and span["attributes"]["db.statement"] == "insert items"
-            )
-        )
-
-        assert spans_container.find_child_span(
-            lambda span: (
-                span["kind"] == "SpanKind.CLIENT"
-                and span["attributes"]["db.system"] == "mongodb"
-                and span["attributes"]["db.name"] == "test"
-                and span["attributes"]["db.statement"] == "find items"
-            )
-        )
+        children = spans_container.get_non_internal_children(name_filter="insert.items")
+        self.assertEqual(1, len(children))
+        self.assertEqual(children[0]["attributes"]["db.system"], "mongodb")
+        self.assertEqual(children[0]["attributes"]["db.statement"], "insert items")
```

## test/integration/pymysql/tests/test_pymysql.py

```diff
@@ -1,26 +1,26 @@
+import requests
 import time
 import unittest
-from test.test_utils.spans_parser import SpansContainer
 
-import requests
+from test.test_utils.spans_parser import SpansContainer
 
 
 class TestFastApiSpans(unittest.TestCase):
     def test_pymysql_instrumentation(self):
         response = requests.get("http://localhost:8003/invoke-pymysql")
 
         response.raise_for_status()
 
         body = response.json()
 
         self.assertEqual(body, {"status": "ok"})
 
         # TODO Do something deterministic
-        time.sleep(3)  # Sleep to allow the exporter to catch up
+        time.sleep(3)  # Sleep for two seconds to allow the exporter to catch up
 
         spans_container = SpansContainer.get_spans_from_file()
 
         # assert mongo children spans
         children = spans_container.get_non_internal_children(name_filter="SELECT")
         self.assertGreaterEqual(len(children), 1)
         self.assertEqual(children[0]["attributes"]["db.system"], "mysql")
```

## test/test_utils/spans_parser.py

```diff
@@ -21,23 +21,23 @@
     spans: List[Dict[str, Any]]
 
     @staticmethod
     def increment_spans():
         spanCounter.counter = sum(1 for line in open(SPANS_FILE_FULL_PATH))
 
     @staticmethod
-    def parse_spans_from_file(path: Optional[str] = None) -> SpansContainer:
-        with open(path or SPANS_FILE_FULL_PATH) as file:
+    def parse_spans_from_file() -> SpansContainer:
+        with open(SPANS_FILE_FULL_PATH) as file:
             spans = [json.loads(line) for line in file.readlines()]
 
         return SpansContainer(spans=spans)
 
     @staticmethod
-    def get_spans_from_file(path: Optional[str] = None) -> SpansContainer:
-        spans = SpansContainer.parse_spans_from_file(path).spans
+    def get_spans_from_file() -> SpansContainer:
+        spans = SpansContainer.parse_spans_from_file().spans
         return SpansContainer(spans=spans[spanCounter.counter :])  # noqa
 
     def get_root(self) -> Dict[str, Any]:
         return list(filter(lambda item: item["parent_id"] is None, self.spans))[0]
 
     def get_children(self) -> List[Dict[str, Any]]:
         return list(
@@ -50,20 +50,14 @@
     def get_internals(self) -> List[Dict[str, Any]]:
         return list(
             filter(
                 lambda item: item["kind"] == "SpanKind.INTERNAL", self.get_children()
             )
         )
 
-    def find_child_span(self, predicate):
-        for span in self.get_children():
-            if predicate(span):
-                yield span
-                break
-
     def get_non_internal_children(
         self, name_filter: Optional[str] = None
     ) -> List[Dict[str, Any]]:
         children = [
             item for item in self.get_children() if item not in self.get_internals()
         ]
         if not name_filter:
```

## Comparing `lumigo_opentelemetry-1.0.89.dist-info/LICENSE` & `lumigo_opentelemetry-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

